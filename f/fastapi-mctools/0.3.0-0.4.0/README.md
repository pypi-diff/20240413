# Comparing `tmp/fastapi_mctools-0.3.0.tar.gz` & `tmp/fastapi_mctools-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_mctools-0.3.0.tar", max compression
+gzip compressed data, was "fastapi_mctools-0.4.0.tar", max compression
```

## Comparing `fastapi_mctools-0.3.0.tar` & `fastapi_mctools-0.4.0.tar`

### file list

```diff
@@ -1,44 +1,45 @@
--rw-r--r--   0        0        0     1072 2024-03-21 08:00:13.490253 fastapi_mctools-0.3.0/LICENSE
--rw-r--r--   0        0        0     7941 2024-03-21 08:00:13.490253 fastapi_mctools-0.3.0/README.md
--rw-r--r--   0        0        0        0 2024-03-21 08:00:13.490253 fastapi_mctools-0.3.0/fastapi_mctools/__init__.py
--rw-r--r--   0        0        0        0 2024-03-21 08:00:13.490253 fastapi_mctools-0.3.0/fastapi_mctools/aws/__init__.py
--rw-r--r--   0        0        0     2155 2024-03-21 08:00:13.490253 fastapi_mctools-0.3.0/fastapi_mctools/aws/s3.py
--rw-r--r--   0        0        0      230 2024-03-21 08:00:13.490253 fastapi_mctools-0.3.0/fastapi_mctools/cache/__init__.py
--rw-r--r--   0        0        0     1400 2024-03-21 08:00:13.490253 fastapi_mctools-0.3.0/fastapi_mctools/cache/base.py
--rw-r--r--   0        0        0     2747 2024-03-21 08:00:13.490253 fastapi_mctools-0.3.0/fastapi_mctools/cache/memory.py
--rw-r--r--   0        0        0     1807 2024-03-21 08:00:13.490253 fastapi_mctools-0.3.0/fastapi_mctools/cache/redis.py
--rw-r--r--   0        0        0        0 2024-03-21 08:00:13.490253 fastapi_mctools-0.3.0/fastapi_mctools/commands/__init__.py
--rw-r--r--   0        0        0      546 2024-03-21 08:00:13.490253 fastapi_mctools-0.3.0/fastapi_mctools/commands/_templates/async_session.py-tpl
--rw-r--r--   0        0        0     3293 2024-03-21 08:00:13.490253 fastapi_mctools-0.3.0/fastapi_mctools/commands/_templates/gitignore-tpl
--rw-r--r--   0        0        0      266 2024-03-21 08:00:13.490253 fastapi_mctools-0.3.0/fastapi_mctools/commands/_templates/gunicorn.config.py-tpl
--rw-r--r--   0        0        0       46 2024-03-21 08:00:13.490253 fastapi_mctools-0.3.0/fastapi_mctools/commands/_templates/main.py-tpl
--rw-r--r--   0        0        0      421 2024-03-21 08:00:13.490253 fastapi_mctools-0.3.0/fastapi_mctools/commands/_templates/pre-commit-tpl
--rw-r--r--   0        0        0       53 2024-03-21 08:00:13.490253 fastapi_mctools-0.3.0/fastapi_mctools/commands/_templates/routers.py-tpl
--rw-r--r--   0        0        0      578 2024-03-21 08:00:13.490253 fastapi_mctools-0.3.0/fastapi_mctools/commands/_templates/session.py-tpl
--rw-r--r--   0        0        0     2236 2024-03-21 08:00:13.490253 fastapi_mctools-0.3.0/fastapi_mctools/commands/_templates/settings.py-tpl
--rw-r--r--   0        0        0       82 2024-03-21 08:00:13.490253 fastapi_mctools-0.3.0/fastapi_mctools/commands/_templates/sqlalchemy_base.py-tpl
--rw-r--r--   0        0        0      500 2024-03-21 08:00:13.490253 fastapi_mctools-0.3.0/fastapi_mctools/commands/gunicorn.py
--rw-r--r--   0        0        0      581 2024-03-21 08:00:13.490253 fastapi_mctools-0.3.0/fastapi_mctools/commands/main.py
--rw-r--r--   0        0        0     1141 2024-03-21 08:00:13.490253 fastapi_mctools-0.3.0/fastapi_mctools/commands/run.py
--rw-r--r--   0        0        0     1376 2024-03-21 08:00:13.490253 fastapi_mctools-0.3.0/fastapi_mctools/commands/startproject.py
--rw-r--r--   0        0        0     2313 2024-03-21 08:00:13.490253 fastapi_mctools-0.3.0/fastapi_mctools/commands/types.py
--rw-r--r--   0        0        0        0 2024-03-21 08:00:13.490253 fastapi_mctools-0.3.0/fastapi_mctools/db/__init__.py
--rw-r--r--   0        0        0     1617 2024-03-21 08:00:13.494253 fastapi_mctools-0.3.0/fastapi_mctools/db/sqlalchemy.py
--rw-r--r--   0        0        0     2297 2024-03-21 08:00:13.494253 fastapi_mctools-0.3.0/fastapi_mctools/dependencies.py
--rw-r--r--   0        0        0     1650 2024-03-21 08:00:13.494253 fastapi_mctools-0.3.0/fastapi_mctools/exceptions.py
--rw-r--r--   0        0        0        0 2024-03-21 08:00:13.494253 fastapi_mctools-0.3.0/fastapi_mctools/middlewares/__init__.py
--rw-r--r--   0        0        0     6828 2024-03-21 08:00:13.494253 fastapi_mctools-0.3.0/fastapi_mctools/middlewares/logging.py
--rw-r--r--   0        0        0     1173 2024-03-21 08:00:13.494253 fastapi_mctools-0.3.0/fastapi_mctools/middlewares/trustedhost.py
--rw-r--r--   0        0        0     2306 2024-03-21 08:00:13.494253 fastapi_mctools-0.3.0/fastapi_mctools/orms/__init__.py
--rw-r--r--   0        0        0        0 2024-03-21 08:00:13.494253 fastapi_mctools-0.3.0/fastapi_mctools/orms/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     3957 2024-03-21 08:00:13.494253 fastapi_mctools-0.3.0/fastapi_mctools/orms/sqlalchemy/async_base.py
--rw-r--r--   0        0        0     2507 2024-03-21 08:00:13.494253 fastapi_mctools-0.3.0/fastapi_mctools/orms/sqlalchemy/filters.py
--rw-r--r--   0        0        0     3404 2024-03-21 08:00:13.494253 fastapi_mctools-0.3.0/fastapi_mctools/orms/sqlalchemy/sync_base.py
--rw-r--r--   0        0        0        0 2024-03-21 08:00:13.494253 fastapi_mctools-0.3.0/fastapi_mctools/test_tools/__init__.py
--rw-r--r--   0        0        0     1964 2024-03-21 08:00:13.494253 fastapi_mctools-0.3.0/fastapi_mctools/test_tools/db_managers.py
--rw-r--r--   0        0        0        0 2024-03-21 08:00:13.494253 fastapi_mctools-0.3.0/fastapi_mctools/utils/__init__.py
--rw-r--r--   0        0        0     2805 2024-03-21 08:00:13.494253 fastapi_mctools-0.3.0/fastapi_mctools/utils/requests.py
--rw-r--r--   0        0        0     1277 2024-03-21 08:00:13.494253 fastapi_mctools-0.3.0/fastapi_mctools/utils/responses.py
--rw-r--r--   0        0        0     1625 2024-03-21 08:00:13.494253 fastapi_mctools-0.3.0/fastapi_mctools/utils/time.py
--rw-r--r--   0        0        0     1029 2024-03-21 08:00:13.494253 fastapi_mctools-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     8748 1970-01-01 00:00:00.000000 fastapi_mctools-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-13 06:43:32.541092 fastapi_mctools-0.4.0/LICENSE
+-rw-r--r--   0        0        0     8669 2024-04-13 06:43:32.541092 fastapi_mctools-0.4.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-13 06:43:32.541092 fastapi_mctools-0.4.0/fastapi_mctools/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 06:43:32.541092 fastapi_mctools-0.4.0/fastapi_mctools/aws/__init__.py
+-rw-r--r--   0        0        0     2155 2024-04-13 06:43:32.541092 fastapi_mctools-0.4.0/fastapi_mctools/aws/s3.py
+-rw-r--r--   0        0        0      230 2024-04-13 06:43:32.541092 fastapi_mctools-0.4.0/fastapi_mctools/cache/__init__.py
+-rw-r--r--   0        0        0     1400 2024-04-13 06:43:32.541092 fastapi_mctools-0.4.0/fastapi_mctools/cache/base.py
+-rw-r--r--   0        0        0     2747 2024-04-13 06:43:32.541092 fastapi_mctools-0.4.0/fastapi_mctools/cache/memory.py
+-rw-r--r--   0        0        0     1807 2024-04-13 06:43:32.541092 fastapi_mctools-0.4.0/fastapi_mctools/cache/redis.py
+-rw-r--r--   0        0        0        0 2024-04-13 06:43:32.541092 fastapi_mctools-0.4.0/fastapi_mctools/commands/__init__.py
+-rw-r--r--   0        0        0      127 2024-04-13 06:43:32.541092 fastapi_mctools-0.4.0/fastapi_mctools/commands/_templates/async_session.py-tpl
+-rw-r--r--   0        0        0     3293 2024-04-13 06:43:32.541092 fastapi_mctools-0.4.0/fastapi_mctools/commands/_templates/gitignore-tpl
+-rw-r--r--   0        0        0      266 2024-04-13 06:43:32.541092 fastapi_mctools-0.4.0/fastapi_mctools/commands/_templates/gunicorn.config.py-tpl
+-rw-r--r--   0        0        0       46 2024-04-13 06:43:32.541092 fastapi_mctools-0.4.0/fastapi_mctools/commands/_templates/main.py-tpl
+-rw-r--r--   0        0        0      455 2024-04-13 06:43:32.541092 fastapi_mctools-0.4.0/fastapi_mctools/commands/_templates/pre-commit-tpl
+-rw-r--r--   0        0        0       53 2024-04-13 06:43:32.541092 fastapi_mctools-0.4.0/fastapi_mctools/commands/_templates/routers.py-tpl
+-rw-r--r--   0        0        0      578 2024-04-13 06:43:32.541092 fastapi_mctools-0.4.0/fastapi_mctools/commands/_templates/session.py-tpl
+-rw-r--r--   0        0        0     2256 2024-04-13 06:43:32.545092 fastapi_mctools-0.4.0/fastapi_mctools/commands/_templates/settings.py-tpl
+-rw-r--r--   0        0        0       82 2024-04-13 06:43:32.545092 fastapi_mctools-0.4.0/fastapi_mctools/commands/_templates/sqlalchemy_base.py-tpl
+-rw-r--r--   0        0        0      500 2024-04-13 06:43:32.545092 fastapi_mctools-0.4.0/fastapi_mctools/commands/gunicorn.py
+-rw-r--r--   0        0        0      675 2024-04-13 06:43:32.545092 fastapi_mctools-0.4.0/fastapi_mctools/commands/main.py
+-rw-r--r--   0        0        0     2031 2024-04-13 06:43:32.545092 fastapi_mctools-0.4.0/fastapi_mctools/commands/run.py
+-rw-r--r--   0        0        0      803 2024-04-13 06:43:32.545092 fastapi_mctools-0.4.0/fastapi_mctools/commands/shell.py
+-rw-r--r--   0        0        0     1525 2024-04-13 06:43:32.545092 fastapi_mctools-0.4.0/fastapi_mctools/commands/startproject.py
+-rw-r--r--   0        0        0     2313 2024-04-13 06:43:32.545092 fastapi_mctools-0.4.0/fastapi_mctools/commands/types.py
+-rw-r--r--   0        0        0        0 2024-04-13 06:43:32.545092 fastapi_mctools-0.4.0/fastapi_mctools/db/__init__.py
+-rw-r--r--   0        0        0     1617 2024-04-13 06:43:32.545092 fastapi_mctools-0.4.0/fastapi_mctools/db/sqlalchemy.py
+-rw-r--r--   0        0        0     2297 2024-04-13 06:43:32.545092 fastapi_mctools-0.4.0/fastapi_mctools/dependencies.py
+-rw-r--r--   0        0        0     1650 2024-04-13 06:43:32.545092 fastapi_mctools-0.4.0/fastapi_mctools/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-13 06:43:32.545092 fastapi_mctools-0.4.0/fastapi_mctools/middlewares/__init__.py
+-rw-r--r--   0        0        0     6828 2024-04-13 06:43:32.545092 fastapi_mctools-0.4.0/fastapi_mctools/middlewares/logging.py
+-rw-r--r--   0        0        0     1173 2024-04-13 06:43:32.545092 fastapi_mctools-0.4.0/fastapi_mctools/middlewares/trustedhost.py
+-rw-r--r--   0        0        0     2306 2024-04-13 06:43:32.545092 fastapi_mctools-0.4.0/fastapi_mctools/orms/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 06:43:32.545092 fastapi_mctools-0.4.0/fastapi_mctools/orms/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     3957 2024-04-13 06:43:32.545092 fastapi_mctools-0.4.0/fastapi_mctools/orms/sqlalchemy/async_base.py
+-rw-r--r--   0        0        0     2507 2024-04-13 06:43:32.545092 fastapi_mctools-0.4.0/fastapi_mctools/orms/sqlalchemy/filters.py
+-rw-r--r--   0        0        0     3404 2024-04-13 06:43:32.545092 fastapi_mctools-0.4.0/fastapi_mctools/orms/sqlalchemy/sync_base.py
+-rw-r--r--   0        0        0        0 2024-04-13 06:43:32.545092 fastapi_mctools-0.4.0/fastapi_mctools/test_tools/__init__.py
+-rw-r--r--   0        0        0     1964 2024-04-13 06:43:32.545092 fastapi_mctools-0.4.0/fastapi_mctools/test_tools/db_managers.py
+-rw-r--r--   0        0        0        0 2024-04-13 06:43:32.545092 fastapi_mctools-0.4.0/fastapi_mctools/utils/__init__.py
+-rw-r--r--   0        0        0     2805 2024-04-13 06:43:32.545092 fastapi_mctools-0.4.0/fastapi_mctools/utils/requests.py
+-rw-r--r--   0        0        0     1277 2024-04-13 06:43:32.545092 fastapi_mctools-0.4.0/fastapi_mctools/utils/responses.py
+-rw-r--r--   0        0        0     1625 2024-04-13 06:43:32.545092 fastapi_mctools-0.4.0/fastapi_mctools/utils/time.py
+-rw-r--r--   0        0        0     1029 2024-04-13 06:43:32.545092 fastapi_mctools-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     9476 1970-01-01 00:00:00.000000 fastapi_mctools-0.4.0/PKG-INFO
```

### Comparing `fastapi_mctools-0.3.0/LICENSE` & `fastapi_mctools-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_mctools-0.3.0/README.md` & `fastapi_mctools-0.4.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -11,24 +11,34 @@
 pip install fastapi-mctools
 ```
 
 ## Usage
 
 ### CLI
 
-### 1. run
+### 1-1. run dev
 
-- run uvicorn server for development
+- run uvicorn server for development, this command wraps uvicorn command.
 - this command will find `main.py` and run uvicorn server
-- use this command when running in local environment
+- use this command when running in local environment and use --port and --host for setting port and host. default is 8000 and 127.0.0.1
 
 ```bash
 mct run dev
 ```
 
+### 1-2. run prod
+
+- run gunicorn server for production, this command wraps gunicorn command.
+- this command will find `gunicorn.config.py` and run gunicorn server
+- if not existing `gunicorn.config.py`, it will make basic gunicorn config file
+
+```bash
+mct run prod
+```
+
 ### 2. startproject
 
 - create a new FastAPI project in ordinary way
 
 ```bash
 mct startproject
 ```
@@ -47,14 +57,37 @@
 - this command will find all functions in the file or directory and check if there is any missing type hint
 - use this if you are very strict about type hinting
 
 ```bash
 mct types <path: directory or file>
 ```
 
+### 5. shell
+
+- simple ipython shell
+- need to install ipython
+
+```bash
+mct shell
+```
+
+```python
+# in ipython shell
+# need to import session that made by generator or async generator
+
+# sync session
+from app.session import get_db
+db = next(get_db())
+
+# async session
+from app.session import get_db
+db = await anxet(get_db())
+
+```
+
 ## DB Session
 
 - DB, AsyncDB
 - when you want to make db session in the fast way, use this
 
 ```python
 from fastapi_mctools.db import DB, AsyncDB
```

### Comparing `fastapi_mctools-0.3.0/fastapi_mctools/aws/s3.py` & `fastapi_mctools-0.4.0/fastapi_mctools/aws/s3.py`

 * *Files identical despite different names*

### Comparing `fastapi_mctools-0.3.0/fastapi_mctools/cache/base.py` & `fastapi_mctools-0.4.0/fastapi_mctools/cache/base.py`

 * *Files identical despite different names*

### Comparing `fastapi_mctools-0.3.0/fastapi_mctools/cache/memory.py` & `fastapi_mctools-0.4.0/fastapi_mctools/cache/memory.py`

 * *Files identical despite different names*

### Comparing `fastapi_mctools-0.3.0/fastapi_mctools/cache/redis.py` & `fastapi_mctools-0.4.0/fastapi_mctools/cache/redis.py`

 * *Files identical despite different names*

### Comparing `fastapi_mctools-0.3.0/fastapi_mctools/commands/_templates/gitignore-tpl` & `fastapi_mctools-0.4.0/fastapi_mctools/commands/_templates/gitignore-tpl`

 * *Files identical despite different names*

### Comparing `fastapi_mctools-0.3.0/fastapi_mctools/commands/_templates/session.py-tpl` & `fastapi_mctools-0.4.0/fastapi_mctools/commands/_templates/session.py-tpl`

 * *Files identical despite different names*

### Comparing `fastapi_mctools-0.3.0/fastapi_mctools/commands/_templates/settings.py-tpl` & `fastapi_mctools-0.4.0/fastapi_mctools/commands/_templates/settings.py-tpl`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 BASE_DIR = Path(__file__).resolve().parent.parent
 config = AutoConfig(search_path=BASE_DIR)
 
 
 class AppSettings(BaseSettings):
     DEBUG: bool = config("DEBUG", cast=bool, default=True)
     OPENAPI_URL: str | None = "/openapi.json" if DEBUG else None
-    API_PREFIX: str = "/api/v1/dev" if DEBUG else "/api/v1"
+    API_PREFIX: str = "/api/v1"
+    DB_URL: str = ""
     TIMEZONE_LOCATION: str = "Asia/Seoul"
     ALLOWED_HOSTS: list = []
     CORS_ORIGINS: list = []
 
     SWAGGER_UI_PARAMS: dict = {
         "deepLinking": True,
         "defaultModelsExpandDepth": 1,
@@ -72,7 +73,10 @@
             },
         },
     }
 
     @property
     def TIMEZONE(self) -> ZoneInfo:
         return ZoneInfo(self.TIMEZONE_LOCATION)
+
+
+settings = AppSettings()
```

### Comparing `fastapi_mctools-0.3.0/fastapi_mctools/commands/main.py` & `fastapi_mctools-0.4.0/fastapi_mctools/commands/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import click
 from fastapi_mctools.commands.startproject import main as startproject_main
 from fastapi_mctools.commands.gunicorn import main as gunicorn_main
 from fastapi_mctools.commands.run import main as run_main
 from fastapi_mctools.commands.types import main as types_main
+from fastapi_mctools.commands.shell import main as shell_main
 
 
 @click.group()
 @click.version_option()
 def cli():
     pass
 
 
 def command_main():
     cli.add_command(startproject_main)
     cli.add_command(gunicorn_main)
     cli.add_command(run_main)
     cli.add_command(types_main)
+    cli.add_command(shell_main)
     cli(prog_name="fastapi-mctools")
 
 
 if __name__ == "__main__":
     command_main()
```

### Comparing `fastapi_mctools-0.3.0/fastapi_mctools/commands/run.py` & `fastapi_mctools-0.4.0/fastapi_mctools/commands/run.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,33 +14,62 @@
     일일히 터미널에 입력하기 귀찮아서 만든 명령어
     출력되면 복사해서 터미널에 입력하면 됨
     """
     click.echo("uvicorn app.main:app --reload --host 127.0.0.1")
 
 
 @main.command("dev", help="uvicorn 서버 실행")
-def dev():
+@click.option("--host", default="127.0.0.1", help="서버 호스트 주소")
+@click.option("--port", default=8000, help="서버 포트 번호")
+def dev(port: int, host: str):
     main_py = find_main_py()
 
     if main_py:
         module_path = str(main_py).replace("/", ".").rstrip(".py")
         if module_path.startswith("."):
             module_path = module_path[1:]
         uvicorn_command = [
             "uvicorn",
             f"{module_path}:app",
             "--reload",
             "--host",
-            "127.0.0.1",
+            host,
+            "--port",
+            str(port),
         ]
         subprocess.run(uvicorn_command)
     else:
         click.echo("main.py 파일을 찾을 수 없습니다.")
 
 
 def find_main_py():
     """
     현재 디렉토리부터 시작하여 main.py 파일을 찾습니다.
     """
     for path in Path(".").rglob("main.py"):
         return path
     return None
+
+
+@main.command("prod", help="gunicorn 서버 실행")
+def prod():
+    def run_gunicorn():
+        gunicorn_config = find_gunicorn_config()
+
+        if gunicorn_config:
+            gunicorn_command = ["gunicorn", "-c", str(gunicorn_config)]
+            subprocess.run(gunicorn_command)
+        else:
+            # when gunicorn_config not found, make it by mct gunicorn
+            subprocess.run(["mct", "gunicorn"])
+            run_gunicorn()
+
+    run_gunicorn()
+
+
+def find_gunicorn_config():
+    """
+    현재 디렉토리부터 시작하여 gunicorn.config.py 파일을 찾습니다.
+    """
+    for path in Path(".").rglob("gunicorn.config.py"):
+        return path
+    return None
```

### Comparing `fastapi_mctools-0.3.0/fastapi_mctools/commands/startproject.py` & `fastapi_mctools-0.4.0/fastapi_mctools/commands/startproject.py`

 * *Files 16% similar despite different names*

```diff
@@ -45,8 +45,11 @@
         "models/base.py",
         ".gitignore",
         ".pre-commit-config.yaml",
     ]
 
     for template, file in zip(TEMPLATES, FILES):
         with resources.path(TEMPLATE_PATH, template) as template_path:
-            shutil.copy(str(template_path), "./app/" + file)
+            if file in [".gitignore", ".pre-commit-config.yaml"]:
+                shutil.copy(str(template_path), "./" + file)
+            else:
+                shutil.copy(str(template_path), "./app/" + file)
```

### Comparing `fastapi_mctools-0.3.0/fastapi_mctools/commands/types.py` & `fastapi_mctools-0.4.0/fastapi_mctools/commands/types.py`

 * *Files identical despite different names*

### Comparing `fastapi_mctools-0.3.0/fastapi_mctools/db/sqlalchemy.py` & `fastapi_mctools-0.4.0/fastapi_mctools/db/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `fastapi_mctools-0.3.0/fastapi_mctools/dependencies.py` & `fastapi_mctools-0.4.0/fastapi_mctools/dependencies.py`

 * *Files identical despite different names*

### Comparing `fastapi_mctools-0.3.0/fastapi_mctools/exceptions.py` & `fastapi_mctools-0.4.0/fastapi_mctools/exceptions.py`

 * *Files identical despite different names*

### Comparing `fastapi_mctools-0.3.0/fastapi_mctools/middlewares/logging.py` & `fastapi_mctools-0.4.0/fastapi_mctools/middlewares/logging.py`

 * *Files identical despite different names*

### Comparing `fastapi_mctools-0.3.0/fastapi_mctools/middlewares/trustedhost.py` & `fastapi_mctools-0.4.0/fastapi_mctools/middlewares/trustedhost.py`

 * *Files identical despite different names*

### Comparing `fastapi_mctools-0.3.0/fastapi_mctools/orms/__init__.py` & `fastapi_mctools-0.4.0/fastapi_mctools/orms/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_mctools-0.3.0/fastapi_mctools/orms/sqlalchemy/async_base.py` & `fastapi_mctools-0.4.0/fastapi_mctools/orms/sqlalchemy/async_base.py`

 * *Files identical despite different names*

### Comparing `fastapi_mctools-0.3.0/fastapi_mctools/orms/sqlalchemy/filters.py` & `fastapi_mctools-0.4.0/fastapi_mctools/orms/sqlalchemy/filters.py`

 * *Files identical despite different names*

### Comparing `fastapi_mctools-0.3.0/fastapi_mctools/orms/sqlalchemy/sync_base.py` & `fastapi_mctools-0.4.0/fastapi_mctools/orms/sqlalchemy/sync_base.py`

 * *Files identical despite different names*

### Comparing `fastapi_mctools-0.3.0/fastapi_mctools/test_tools/db_managers.py` & `fastapi_mctools-0.4.0/fastapi_mctools/test_tools/db_managers.py`

 * *Files identical despite different names*

### Comparing `fastapi_mctools-0.3.0/fastapi_mctools/utils/requests.py` & `fastapi_mctools-0.4.0/fastapi_mctools/utils/requests.py`

 * *Files identical despite different names*

### Comparing `fastapi_mctools-0.3.0/fastapi_mctools/utils/responses.py` & `fastapi_mctools-0.4.0/fastapi_mctools/utils/responses.py`

 * *Files identical despite different names*

### Comparing `fastapi_mctools-0.3.0/fastapi_mctools/utils/time.py` & `fastapi_mctools-0.4.0/fastapi_mctools/utils/time.py`

 * *Files identical despite different names*

### Comparing `fastapi_mctools-0.3.0/pyproject.toml` & `fastapi_mctools-0.4.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-mctools"
-version = "0.3.0"
+version = "0.4.0"
 description = "Fastapi mc style tools to make it easier to develop."
 authors = ["Jungminchae <minchae3618@gmail.com>"]
 readme = "README.md"
 packages = [{include = "fastapi_mctools"}]
 
 [tool.poetry.dependencies]
 python =  ">=3.10,<4.0"
```

### Comparing `fastapi_mctools-0.3.0/PKG-INFO` & `fastapi_mctools-0.4.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-mctools
-Version: 0.3.0
+Version: 0.4.0
 Summary: Fastapi mc style tools to make it easier to develop.
 Author: Jungminchae
 Author-email: minchae3618@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -31,24 +31,34 @@
 pip install fastapi-mctools
 ```
 
 ## Usage
 
 ### CLI
 
-### 1. run
+### 1-1. run dev
 
-- run uvicorn server for development
+- run uvicorn server for development, this command wraps uvicorn command.
 - this command will find `main.py` and run uvicorn server
-- use this command when running in local environment
+- use this command when running in local environment and use --port and --host for setting port and host. default is 8000 and 127.0.0.1
 
 ```bash
 mct run dev
 ```
 
+### 1-2. run prod
+
+- run gunicorn server for production, this command wraps gunicorn command.
+- this command will find `gunicorn.config.py` and run gunicorn server
+- if not existing `gunicorn.config.py`, it will make basic gunicorn config file
+
+```bash
+mct run prod
+```
+
 ### 2. startproject
 
 - create a new FastAPI project in ordinary way
 
 ```bash
 mct startproject
 ```
@@ -67,14 +77,37 @@
 - this command will find all functions in the file or directory and check if there is any missing type hint
 - use this if you are very strict about type hinting
 
 ```bash
 mct types <path: directory or file>
 ```
 
+### 5. shell
+
+- simple ipython shell
+- need to install ipython
+
+```bash
+mct shell
+```
+
+```python
+# in ipython shell
+# need to import session that made by generator or async generator
+
+# sync session
+from app.session import get_db
+db = next(get_db())
+
+# async session
+from app.session import get_db
+db = await anxet(get_db())
+
+```
+
 ## DB Session
 
 - DB, AsyncDB
 - when you want to make db session in the fast way, use this
 
 ```python
 from fastapi_mctools.db import DB, AsyncDB
```

