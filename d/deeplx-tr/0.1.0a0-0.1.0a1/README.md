# Comparing `tmp/deeplx_tr-0.1.0a0.tar.gz` & `tmp/deeplx_tr-0.1.0a1.tar.gz`

## Comparing `deeplx_tr-0.1.0a0.tar` & `deeplx_tr-0.1.0a1.tar`

### file list

```diff
@@ -1,22 +1,29 @@
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 deeplx_tr-0.1.0a0/.flake8
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 deeplx_tr-0.1.0a0/.python-version
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 deeplx_tr-0.1.0a0/.ruff.toml
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 deeplx_tr-0.1.0a0/nodemon.json
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 deeplx_tr-0.1.0a0/package.json
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 deeplx_tr-0.1.0a0/poetry.toml
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 deeplx_tr-0.1.0a0/pylintrc
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 deeplx_tr-0.1.0a0/pyrightconfig.json
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 deeplx_tr-0.1.0a0/requirements-dev.lock
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 deeplx_tr-0.1.0a0/requirements.lock
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 deeplx_tr-0.1.0a0/.github/workflows/routine-tests.yml
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 deeplx_tr-0.1.0a0/.husky/pre-commit
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 deeplx_tr-0.1.0a0/src/deeplx_tr/__init__.py
--rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 deeplx_tr-0.1.0a0/src/deeplx_tr/__main__.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 deeplx_tr-0.1.0a0/src/deeplx_tr/deeplx_tr.py
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 deeplx_tr-0.1.0a0/tests/__init__.py
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 deeplx_tr-0.1.0a0/tests/test_deeplx_tr.py
--rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 deeplx_tr-0.1.0a0/.gitignore
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 deeplx_tr-0.1.0a0/LICENSE
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 deeplx_tr-0.1.0a0/README.md
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 deeplx_tr-0.1.0a0/pyproject.toml
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 deeplx_tr-0.1.0a0/PKG-INFO
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 deeplx_tr-0.1.0a1/.flake8
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 deeplx_tr-0.1.0a1/.python-version
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 deeplx_tr-0.1.0a1/.ruff.toml
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 deeplx_tr-0.1.0a1/nodemon.json
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 deeplx_tr-0.1.0a1/package.json
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 deeplx_tr-0.1.0a1/poetry.toml
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 deeplx_tr-0.1.0a1/pylintrc
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 deeplx_tr-0.1.0a1/pyrightconfig.json
+-rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 deeplx_tr-0.1.0a1/requirements-dev.lock
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 deeplx_tr-0.1.0a1/requirements.lock
+-rw-r--r--   0        0        0    42373 2020-02-02 00:00:00.000000 deeplx_tr-0.1.0a1/yarn.lock
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 deeplx_tr-0.1.0a1/.github/workflows/routine-tests.yml
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 deeplx_tr-0.1.0a1/.husky/pre-commit
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 deeplx_tr-0.1.0a1/src/deeplx_tr/__init__.py
+-rw-r--r--   0        0        0     3141 2020-02-02 00:00:00.000000 deeplx_tr-0.1.0a1/src/deeplx_tr/__main__.py
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 deeplx_tr-0.1.0a1/src/deeplx_tr/__main__.py-
+-rw-r--r--   0        0        0     3730 2020-02-02 00:00:00.000000 deeplx_tr-0.1.0a1/src/deeplx_tr/deeplx_client.py
+-rw-r--r--   0        0        0     4609 2020-02-02 00:00:00.000000 deeplx_tr-0.1.0a1/src/deeplx_tr/deeplx_client_async.py
+-rw-r--r--   0        0        0     7395 2020-02-02 00:00:00.000000 deeplx_tr-0.1.0a1/src/deeplx_tr/deeplx_tr.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 deeplx_tr-0.1.0a1/src/deeplx_tr/deeplx_tr.py-
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 deeplx_tr-0.1.0a1/tests/__init__.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 deeplx_tr-0.1.0a1/tests/test_deeplx_client.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 deeplx_tr-0.1.0a1/tests/test_deeplx_client_asycn.py
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 deeplx_tr-0.1.0a1/tests/test_deeplx_tr.py
+-rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 deeplx_tr-0.1.0a1/.gitignore
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 deeplx_tr-0.1.0a1/LICENSE
+-rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 deeplx_tr-0.1.0a1/README.md
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 deeplx_tr-0.1.0a1/pyproject.toml
+-rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 deeplx_tr-0.1.0a1/PKG-INFO
```

### Comparing `deeplx_tr-0.1.0a0/package.json` & `deeplx_tr-0.1.0a1/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9944444444444445%*

 * *Differences: {"'scripts'": "{'test': 'nodemon -w tests -w src -e .py -x cross-env LOGURU_LEVEL=TRACE rye run "*

 * *              "pytest -k test_deeplx_tr'}"}*

```diff
@@ -14,12 +14,12 @@
         "prepare": "husky install",
         "publish": "rye build && rye publish",
         "pylint": "nodemon -w deeplx_tr -e .py -x pylint deeplx_tr",
         "pyright": "nodemon -w deeplx_tr -w .venv -e .py -x pyright deeplx_tr tests",
         "pytest": "nodemon -w tests -w deeplx_tr -e .py -x pytest tests deeplx_tr",
         "start": "pyright && pytest && yarn style",
         "style": "nodemon -w deeplx_tr -w tests -x \"black tests deeplx_tr && python -m flake8\"",
-        "test": "nodemon -w tests -w src -e .py -x cross-env LOGURU_LEVEL=TRACE rye run pytest",
+        "test": "nodemon -w tests -w src -e .py -x cross-env LOGURU_LEVEL=TRACE rye run pytest -k test_deeplx_tr",
         "test:deeplx_tr": "nodemon -w tests -e .py -x pytest -k deeplx_tr tests"
     },
     "version": "0.1.0a0"
 }
```

### Comparing `deeplx_tr-0.1.0a0/requirements-dev.lock` & `deeplx_tr-0.1.0a1/requirements-dev.lock`

 * *Files 20% similar despite different names*

```diff
@@ -4,65 +4,107 @@
 # last locked with the following flags:
 #   pre: false
 #   features: []
 #   all-features: false
 #   with-sources: false
 
 -e file:.
+anyio==4.3.0
+    # via httpx
 asttokens==2.4.1
     # via stack-data
+certifi==2024.2.2
+    # via httpcore
+    # via httpx
+click==8.1.7
+    # via typer
 colorama==0.4.6
+    # via click
     # via ipython
     # via loguru
+    # via logzero
     # via pytest
 decorator==5.1.1
     # via ipython
+environs==9.5.0
+    # via set-loglevel
 exceptiongroup==1.2.0
+    # via anyio
     # via ipython
     # via pytest
 executing==2.0.1
     # via stack-data
+h11==0.14.0
+    # via httpcore
+httpcore==1.0.5
+    # via httpx
+httpx==0.27.0
+    # via deeplx-tr
+idna==3.6
+    # via anyio
+    # via httpx
 iniconfig==2.0.0
     # via pytest
 ipython==8.23.0
 jedi==0.19.1
     # via ipython
 loguru==0.7.2
     # via deeplx-tr
+logzero==1.7.0
+    # via set-loglevel
 markdown-it-py==3.0.0
     # via rich
+marshmallow==3.21.1
+    # via environs
 matplotlib-inline==0.1.6
     # via ipython
 mdurl==0.1.2
     # via markdown-it-py
 packaging==24.0
+    # via marshmallow
     # via pytest
 parso==0.8.4
     # via jedi
 pluggy==1.4.0
     # via pytest
 prompt-toolkit==3.0.43
     # via ipython
 pure-eval==0.2.2
     # via stack-data
 pygments==2.17.2
     # via ipython
     # via rich
+pyperclip==1.8.2
+    # via deeplx-tr
 pytest==8.1.1
+python-dotenv==1.0.1
+    # via environs
 rich==13.7.1
     # via deeplx-tr
+    # via typer
 ruff==0.3.5
+set-loglevel==0.1.2
+    # via deeplx-tr
+shellingham==1.5.4
+    # via typer
 six==1.16.0
     # via asttokens
+sniffio==1.3.1
+    # via anyio
+    # via httpx
 stack-data==0.6.3
     # via ipython
 tomli==2.0.1
     # via pytest
 traitlets==5.14.2
     # via ipython
     # via matplotlib-inline
+typer==0.12.3
+    # via deeplx-tr
 typing-extensions==4.11.0
+    # via anyio
     # via ipython
+    # via typer
 wcwidth==0.2.13
     # via prompt-toolkit
 win32-setctime==1.1.0
     # via loguru
```

### Comparing `deeplx_tr-0.1.0a0/.github/workflows/routine-tests.yml` & `deeplx_tr-0.1.0a1/.github/workflows/routine-tests.yml`

 * *Files identical despite different names*

### Comparing `deeplx_tr-0.1.0a0/src/deeplx_tr/__main__.py` & `deeplx_tr-0.1.0a1/src/deeplx_tr/__main__.py-`

 * *Files 12% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 del sys
 # logger.remove()
 # logger.add(sys.stderr, level="TRACE")
 
 del Path, logger, deeplx_tr
 
 app = typer.Typer(
-    name="deeplx_tr",
+    name="deeplx-tr",
     add_completion=False,
-    help="deeplx_tr help",
+    help="deeplx-tr help",
 )
 
 
 def _version_callback(value: bool) -> None:
     if value:
         typer.echo(f"{app.info.name} v.{__version__} -- ...")
         raise typer.Exit()
@@ -37,11 +37,12 @@
         "-V",
         help="Show version info and exit.",
         callback=_version_callback,
         is_eager=True,
     ),
 ):
     """Define."""
+    print("hello")
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `deeplx_tr-0.1.0a0/.gitignore` & `deeplx_tr-0.1.0a1/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -138,8 +138,9 @@
 cython_debug/
 *.bat
 *.swp
 links/
 # .gitignore
 node_modules
 .ruff_cache
-.yarn
+.yarn
+.pnp.cjs
```

### Comparing `deeplx_tr-0.1.0a0/LICENSE` & `deeplx_tr-0.1.0a1/LICENSE`

 * *Files identical despite different names*

