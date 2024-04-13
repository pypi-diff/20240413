# Comparing `tmp/retried-7.2.0.tar.gz` & `tmp/retried-7.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retried-7.2.0.tar", last modified: Fri Apr 12 21:03:31 2024, max compression
+gzip compressed data, was "retried-7.3.0.tar", last modified: Fri Apr 12 21:24:44 2024, max compression
```

## Comparing `retried-7.2.0.tar` & `retried-7.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      102 2024-04-12 21:03:17.070032 retried-7.2.0/README.md
--rw-r--r--   0        0        0     1061 2024-04-12 21:03:31.806179 retried-7.2.0/pyproject.toml
--rw-r--r--   0        0        0      162 2024-04-12 21:03:17.070032 retried-7.2.0/src/retried/__init__.py
--rw-r--r--   0        0        0       18 2024-04-12 21:03:17.070032 retried-7.2.0/src/retried/__version__.py
--rw-r--r--   0        0        0     2290 2024-04-12 21:03:17.070032 retried-7.2.0/src/retried/aretry.py
--rw-r--r--   0        0        0     3340 2024-04-12 21:03:17.070032 retried-7.2.0/src/retried/retry.py
--rw-r--r--   0        0        0      189 2024-04-12 21:03:17.070032 retried-7.2.0/src/retried/utils.py
--rw-r--r--   0        0        0        0 2024-04-12 21:03:17.070032 retried-7.2.0/tests/__init__.py
--rw-r--r--   0        0        0      657 2024-04-12 21:03:17.070032 retried-7.2.0/tests/test_aretry.py
--rw-r--r--   0        0        0      276 1970-01-01 00:00:00.000000 retried-7.2.0/PKG-INFO
+-rw-r--r--   0        0        0      102 2024-04-12 21:24:29.312009 retried-7.3.0/README.md
+-rw-r--r--   0        0        0     1061 2024-04-12 21:24:44.663996 retried-7.3.0/pyproject.toml
+-rw-r--r--   0        0        0      162 2024-04-12 21:24:29.316009 retried-7.3.0/src/retried/__init__.py
+-rw-r--r--   0        0        0       18 2024-04-12 21:24:29.316009 retried-7.3.0/src/retried/__version__.py
+-rw-r--r--   0        0        0     2290 2024-04-12 21:24:29.316009 retried-7.3.0/src/retried/aretry.py
+-rw-r--r--   0        0        0     3932 2024-04-12 21:24:29.316009 retried-7.3.0/src/retried/retry.py
+-rw-r--r--   0        0        0      189 2024-04-12 21:24:29.316009 retried-7.3.0/src/retried/utils.py
+-rw-r--r--   0        0        0        0 2024-04-12 21:24:29.316009 retried-7.3.0/tests/__init__.py
+-rw-r--r--   0        0        0      657 2024-04-12 21:24:29.316009 retried-7.3.0/tests/test_aretry.py
+-rw-r--r--   0        0        0      276 1970-01-01 00:00:00.000000 retried-7.3.0/PKG-INFO
```

### Comparing `retried-7.2.0/pyproject.toml` & `retried-7.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "retried"
-version = "7.2.0"
+version = "7.3.0"
 requires-python = ">=3.9"
 description = "A simple and powerful retrying library for Python"
 readme = "README.md"
 dependencies = []
 
 [build-system]
 requires = [
```

### Comparing `retried-7.2.0/src/retried/aretry.py` & `retried-7.3.0/src/retried/aretry.py`

 * *Files identical despite different names*

### Comparing `retried-7.2.0/src/retried/retry.py` & `retried-7.3.0/src/retried/retry.py`

 * *Files 13% similar despite different names*

```diff
@@ -37,14 +37,38 @@
         self._logf = logf
         super().__init__(__package__)
 
     def _log(self, level, msg, *args, **kwargs):
         self._logf(msg)
 
 
+def sleep_on_start(
+    seconds: DelayT,
+    *,
+    sleep: SleepT = time.sleep,
+    logger: logging.Logger = logger,
+):
+    if not isinstance(logger, logging.Logger):
+        logger = DummyLogger(logger)
+
+    def decorator(f):
+        @wraps(f)
+        def wrapper(*args, **kwds):
+            logger.debug(
+                f'sleep {seconds} seconds on start: '
+                f'{f.__qualname__} {relative_to_cwd(f.__code__.co_filename)}:{f.__code__.co_firstlineno}'
+            )
+            sleep(seconds)
+            return f(*args, **kwds)
+
+        return wrapper
+
+    return decorator
+
+
 def retry(
     retries: RetriesT = None,
     *,
     exceptions: SingleOrTuple[t.Type[Exception]] = Exception,
     error_callback: t.Optional[t.Callable[[int, Exception, DelayT, RetriesT, FuncT], None]] = None,
     sleep: SleepT = time.sleep,
     delays: SingleOrIterable[DelayT] = 0,
```

### Comparing `retried-7.2.0/tests/test_aretry.py` & `retried-7.3.0/tests/test_aretry.py`

 * *Files identical despite different names*

