# Comparing `tmp/pwright-9.0.0.tar.gz` & `tmp/pwright-9.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwright-9.0.0.tar", last modified: Wed Apr 10 14:54:56 2024, max compression
+gzip compressed data, was "pwright-9.1.0.tar", last modified: Sat Apr 13 17:04:52 2024, max compression
```

## Comparing `pwright-9.0.0.tar` & `pwright-9.1.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0     1067 2024-04-10 14:54:56.627755 pwright-9.0.0/pyproject.toml
--rw-r--r--   0        0        0      104 2024-04-10 14:54:39.791647 pwright-9.0.0/src/pwright/__init__.py
--rw-r--r--   0        0        0       18 2024-04-10 14:54:39.791647 pwright-9.0.0/src/pwright/__version__.py
--rw-r--r--   0        0        0      260 2024-04-10 14:54:39.791647 pwright-9.0.0/src/pwright/_constants.py
--rw-r--r--   0        0        0      575 2024-04-10 14:54:39.795647 pwright-9.0.0/src/pwright/_utils.py
--rw-r--r--   0        0        0     1380 2024-04-10 14:54:39.795647 pwright-9.0.0/src/pwright/async_api/__init__.py
--rw-r--r--   0        0        0      619 2024-04-10 14:54:39.795647 pwright-9.0.0/src/pwright/async_api/_apis.py
--rw-r--r--   0        0        0     2029 2024-04-10 14:54:39.795647 pwright-9.0.0/src/pwright/async_api/_briefs.py
--rw-r--r--   0        0        0     4700 2024-04-10 14:54:39.795647 pwright-9.0.0/src/pwright/async_api/_cms.py
--rw-r--r--   0        0        0      608 2024-04-10 14:54:39.795647 pwright-9.0.0/src/pwright/async_api/_compatibilities.py
--rw-r--r--   0        0        0      908 2024-04-10 14:54:39.795647 pwright-9.0.0/src/pwright/async_api/utils.py
--rw-r--r--   0        0        0     1075 2024-04-10 14:54:39.795647 pwright-9.0.0/src/pwright/sync_api/__init__.py
--rw-r--r--   0        0        0      608 2024-04-10 14:54:39.795647 pwright-9.0.0/src/pwright/sync_api/_apis.py
--rw-r--r--   0        0        0     1975 2024-04-10 14:54:39.795647 pwright-9.0.0/src/pwright/sync_api/_briefs.py
--rw-r--r--   0        0        0     4590 2024-04-10 14:54:39.795647 pwright-9.0.0/src/pwright/sync_api/_cms.py
--rw-r--r--   0        0        0      860 2024-04-10 14:54:39.795647 pwright-9.0.0/src/pwright/sync_api/utils.py
--rw-r--r--   0        0        0      484 2024-04-10 14:54:39.795647 pwright-9.0.0/src/pwright/typealiases.py
--rw-r--r--   0        0        0        0 2024-04-10 14:54:39.795647 pwright-9.0.0/tests/__init__.py
--rw-r--r--   0        0        0     1444 2024-04-10 14:54:39.795647 pwright-9.0.0/tests/test_apw.py
--rw-r--r--   0        0        0     1196 2024-04-10 14:54:39.795647 pwright-9.0.0/tests/test_pw.py
--rw-r--r--   0        0        0      108 1970-01-01 00:00:00.000000 pwright-9.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1205 2024-04-13 17:04:52.052861 pwright-9.1.0/pyproject.toml
+-rw-r--r--   0        0        0      104 2024-04-13 17:04:38.852855 pwright-9.1.0/src/pwright/__init__.py
+-rw-r--r--   0        0        0       18 2024-04-13 17:04:38.852855 pwright-9.1.0/src/pwright/__version__.py
+-rw-r--r--   0        0        0      575 2024-04-13 17:04:38.852855 pwright-9.1.0/src/pwright/_utils.py
+-rw-r--r--   0        0        0     1380 2024-04-13 17:04:38.852855 pwright-9.1.0/src/pwright/async_api/__init__.py
+-rw-r--r--   0        0        0      679 2024-04-13 17:04:38.852855 pwright-9.1.0/src/pwright/async_api/_apis.py
+-rw-r--r--   0        0        0     2169 2024-04-13 17:04:38.852855 pwright-9.1.0/src/pwright/async_api/_briefs.py
+-rw-r--r--   0        0        0     4904 2024-04-13 17:04:38.852855 pwright-9.1.0/src/pwright/async_api/_cms.py
+-rw-r--r--   0        0        0      608 2024-04-13 17:04:38.852855 pwright-9.1.0/src/pwright/async_api/_compatibilities.py
+-rw-r--r--   0        0        0      908 2024-04-13 17:04:38.852855 pwright-9.1.0/src/pwright/async_api/utils.py
+-rw-r--r--   0        0        0      260 2024-04-13 17:04:38.852855 pwright-9.1.0/src/pwright/constants.py
+-rw-r--r--   0        0        0     1075 2024-04-13 17:04:38.852855 pwright-9.1.0/src/pwright/sync_api/__init__.py
+-rw-r--r--   0        0        0      667 2024-04-13 17:04:38.852855 pwright-9.1.0/src/pwright/sync_api/_apis.py
+-rw-r--r--   0        0        0     2115 2024-04-13 17:04:38.852855 pwright-9.1.0/src/pwright/sync_api/_briefs.py
+-rw-r--r--   0        0        0     4794 2024-04-13 17:04:38.852855 pwright-9.1.0/src/pwright/sync_api/_cms.py
+-rw-r--r--   0        0        0      860 2024-04-13 17:04:38.852855 pwright-9.1.0/src/pwright/sync_api/utils.py
+-rw-r--r--   0        0        0      541 2024-04-13 17:04:38.852855 pwright-9.1.0/src/pwright/typealiases.py
+-rw-r--r--   0        0        0        0 2024-04-13 17:04:38.856855 pwright-9.1.0/tests/__init__.py
+-rw-r--r--   0        0        0      126 2024-04-13 17:04:38.856855 pwright-9.1.0/tests/conftest.py
+-rw-r--r--   0        0        0     1635 2024-04-13 17:04:38.856855 pwright-9.1.0/tests/test_apw.py
+-rw-r--r--   0        0        0     1387 2024-04-13 17:04:38.856855 pwright-9.1.0/tests/test_pw.py
+-rw-r--r--   0        0        0      108 1970-01-01 00:00:00.000000 pwright-9.1.0/PKG-INFO
```

### Comparing `pwright-9.0.0/pyproject.toml` & `pwright-9.1.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,39 @@
+[build-system]
+requires = [
+    "pdm-backend",
+]
+build-backend = "pdm.backend"
+
 [project]
 name = "pwright"
-version = "9.0.0"
+version = "9.1.0"
 requires-python = ">=3.8"
 dependencies = [
     "playwright>=1.34.0",
 ]
 
-[build-system]
-requires = [
-    "pdm-backend",
-]
-build-backend = "pdm.backend"
-
 [tool.pdm]
 distribution = true
 
 [tool.pdm.dev-dependencies]
 dev = [
     "pytest>=8.0.2",
+    "pytest-xdist>=3.5.0",
 ]
 
 [tool.pdm.scripts]
-pw_install = "playwright install --with-deps chromium"
-test = "pytest -s"
+pw = "playwright"
+test = "pytest -n auto -v"
+
+[tool.pdm.scripts.pw_install]
+composite = [
+    "python -c \"print('playwright install...\\n')\"",
+    "playwright install --with-deps",
+]
 
 [tool.semantic_release]
 version_toml = [
     "pyproject.toml:project.version",
 ]
 version_variables = [
     "src/pwright/__version__.py:VERSION",
```

### Comparing `pwright-9.0.0/src/pwright/_utils.py` & `pwright-9.1.0/src/pwright/_utils.py`

 * *Files identical despite different names*

### Comparing `pwright-9.0.0/src/pwright/async_api/__init__.py` & `pwright-9.1.0/src/pwright/async_api/__init__.py`

 * *Files identical despite different names*

### Comparing `pwright-9.0.0/src/pwright/async_api/_apis.py` & `pwright-9.1.0/src/pwright/async_api/_apis.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from playwright.async_api import Browser as Browser
 from playwright.async_api import BrowserContext as BrowserContext
+from playwright.async_api import BrowserType as BrowserType
 from playwright.async_api import Dialog as Dialog
 from playwright.async_api import ElementHandle as ElementHandle
 from playwright.async_api import Page as Page
 from playwright.async_api import Playwright as Playwright
 from playwright.async_api import ProxySettings as ProxySettings
 from playwright.async_api import Route as Route
 from playwright.async_api import TimeoutError as TimeoutError
```

### Comparing `pwright-9.0.0/src/pwright/async_api/_briefs.py` & `pwright-9.1.0/src/pwright/async_api/_briefs.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from contextlib import asynccontextmanager
 from pathlib import Path
 import typing as t
 
-from .._constants import INIT_SCRIPT_HIDE_NAVIGATOR
+from ..constants import INIT_SCRIPT_HIDE_NAVIGATOR
+from ..typealiases import BrowserTypeT
 from ..typealiases import SecondsT
 from ._apis import ProxySettings
 from ._cms import playwright_browser
 from ._cms import playwright_context
 from ._cms import playwright_page
 
 
 pw_browser = playwright_browser
 
 
 @asynccontextmanager
 async def pw_context(
     *,
     # [browser]
+    browser_type: t.Optional[BrowserTypeT] = None,
     executable_path: t.Optional[t.Union[str, Path]] = None,
     headed: t.Optional[bool] = None,
     proxy: t.Optional[ProxySettings] = None,
     slow_mo: t.Optional[SecondsT] = None,
     traces_dir: t.Optional[t.Union[str, Path]] = None,
     # [context]
     no_viewport: t.Optional[bool] = True,
@@ -40,14 +42,15 @@
         yield context
 
 
 @asynccontextmanager
 async def pw_page(
     *,
     # [browser]
+    browser_type: t.Optional[BrowserTypeT] = None,
     executable_path: t.Optional[t.Union[str, Path]] = None,
     headed: t.Optional[bool] = None,
     proxy: t.Optional[ProxySettings] = None,
     slow_mo: t.Optional[SecondsT] = None,
     traces_dir: t.Optional[t.Union[str, Path]] = None,
     # [context]
     no_viewport: t.Optional[bool] = True,
```

### Comparing `pwright-9.0.0/src/pwright/async_api/_cms.py` & `pwright-9.1.0/src/pwright/async_api/_cms.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 from contextlib import asynccontextmanager
 import logging
 from pathlib import Path
 import typing as t
 
-from .._constants import INIT_SCRIPT_HIDE_NAVIGATOR
 from .._utils import to_milliseconds
+from ..constants import INIT_SCRIPT_HIDE_NAVIGATOR
+from ..typealiases import BrowserTypeT
 from ..typealiases import SecondsT
+from ._apis import BrowserType
 from ._apis import ProxySettings
 from ._apis import playwright
 
 
 logger = logging.getLogger(__name__)
 
 
 @asynccontextmanager
 async def playwright_browser(
     *,
     # [browser]
+    browser_type: t.Optional[BrowserTypeT] = None,
     executable_path: t.Optional[t.Union[str, Path]] = None,
     headed: t.Optional[bool] = None,
     proxy: t.Optional[ProxySettings] = None,
     slow_mo: t.Optional[SecondsT] = None,
     traces_dir: t.Optional[t.Union[str, Path]] = None,
 ):
+    browser_type = browser_type or 'chromium'
     # https://playwright.dev/python/docs/test-runners#fixtures
     async with playwright() as _playwright:
         logger.debug(f'{_playwright = }')
-        async with await _playwright.chromium.launch(
+        async with await t.cast(BrowserType, getattr(_playwright, browser_type)).launch(
             executable_path=executable_path,
             headless=not headed,
             proxy=proxy,
             slow_mo=to_milliseconds(slow_mo),
             traces_dir=traces_dir,
         ) as browser:
-            browser_type = browser.browser_type
-            logger.debug(f'{browser_type = }')
-            logger.debug(f'{browser = }')
-            browser_name = browser_type.name
-            logger.debug(f'{browser_name = }')
+            logger.debug(f'{browser.browser_type.name = }')
             yield browser
 
 
 @asynccontextmanager
 async def playwright_context(
     *,
     # [browser]
+    browser_type: t.Optional[BrowserTypeT] = None,
     executable_path: t.Optional[t.Union[str, Path]] = None,
     headed: t.Optional[bool] = None,
     proxy: t.Optional[ProxySettings] = None,
     slow_mo: t.Optional[SecondsT] = None,
     traces_dir: t.Optional[t.Union[str, Path]] = None,
     # [context]
     no_viewport: t.Optional[bool] = True,
@@ -59,14 +60,15 @@
     tracing=False,
     snapshots=True,
     screenshots=True,
     sources=True,
     path='trace.zip',
 ):
     async with playwright_browser(
+        browser_type=browser_type,
         executable_path=executable_path,
         headed=headed,
         proxy=proxy,
         slow_mo=slow_mo,
         traces_dir=traces_dir,
     ) as browser:
         async with await browser.new_context(
@@ -89,14 +91,15 @@
                 )
 
 
 @asynccontextmanager
 async def playwright_page(
     *,
     # [browser]
+    browser_type: t.Optional[BrowserTypeT] = None,
     executable_path: t.Optional[t.Union[str, Path]] = None,
     headed: t.Optional[bool] = None,
     proxy: t.Optional[ProxySettings] = None,
     slow_mo: t.Optional[SecondsT] = None,
     traces_dir: t.Optional[t.Union[str, Path]] = None,
     # [context]
     no_viewport: t.Optional[bool] = True,
@@ -112,14 +115,15 @@
     # [page]
     default_navigation_timeout: t.Optional[SecondsT] = None,
     default_timeout: t.Optional[SecondsT] = None,
     init_script: t.Optional[str] = INIT_SCRIPT_HIDE_NAVIGATOR,
     init_script_path: t.Optional[t.Union[str, Path]] = None,
 ):
     async with playwright_context(
+        browser_type=browser_type,
         executable_path=executable_path,
         headed=headed,
         proxy=proxy,
         slow_mo=slow_mo,
         traces_dir=traces_dir,
         no_viewport=no_viewport,
         user_agent=user_agent,
```

### Comparing `pwright-9.0.0/src/pwright/async_api/_compatibilities.py` & `pwright-9.1.0/src/pwright/async_api/_compatibilities.py`

 * *Files identical despite different names*

### Comparing `pwright-9.0.0/src/pwright/async_api/utils.py` & `pwright-9.1.0/src/pwright/async_api/utils.py`

 * *Files identical despite different names*

### Comparing `pwright-9.0.0/src/pwright/sync_api/__init__.py` & `pwright-9.1.0/src/pwright/sync_api/__init__.py`

 * *Files identical despite different names*

### Comparing `pwright-9.0.0/src/pwright/sync_api/_apis.py` & `pwright-9.1.0/src/pwright/sync_api/_apis.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from playwright.sync_api import Browser as Browser
 from playwright.sync_api import BrowserContext as BrowserContext
+from playwright.sync_api import BrowserType as BrowserType
 from playwright.sync_api import Dialog as Dialog
 from playwright.sync_api import ElementHandle as ElementHandle
 from playwright.sync_api import Page as Page
 from playwright.sync_api import Playwright as Playwright
 from playwright.sync_api import ProxySettings as ProxySettings
 from playwright.sync_api import Route as Route
 from playwright.sync_api import TimeoutError as TimeoutError
```

### Comparing `pwright-9.0.0/src/pwright/sync_api/_briefs.py` & `pwright-9.1.0/src/pwright/sync_api/_briefs.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from contextlib import contextmanager
 from pathlib import Path
 import typing as t
 
-from .._constants import INIT_SCRIPT_HIDE_NAVIGATOR
+from ..constants import INIT_SCRIPT_HIDE_NAVIGATOR
+from ..typealiases import BrowserTypeT
 from ..typealiases import SecondsT
 from ._apis import ProxySettings
 from ._cms import playwright_browser
 from ._cms import playwright_context
 from ._cms import playwright_page
 
 
 pw_browser = playwright_browser
 
 
 @contextmanager
 def pw_context(
     *,
     # [browser]
+    browser_type: t.Optional[BrowserTypeT] = None,
     executable_path: t.Optional[t.Union[str, Path]] = None,
     headed: t.Optional[bool] = None,
     proxy: t.Optional[ProxySettings] = None,
     slow_mo: t.Optional[SecondsT] = None,
     traces_dir: t.Optional[t.Union[str, Path]] = None,
     # [context]
     no_viewport: t.Optional[bool] = True,
@@ -38,14 +40,15 @@
         yield context
 
 
 @contextmanager
 def pw_page(
     *,
     # [browser]
+    browser_type: t.Optional[BrowserTypeT] = None,
     executable_path: t.Optional[t.Union[str, Path]] = None,
     headed: t.Optional[bool] = None,
     proxy: t.Optional[ProxySettings] = None,
     slow_mo: t.Optional[SecondsT] = None,
     traces_dir: t.Optional[t.Union[str, Path]] = None,
     # [context]
     no_viewport: t.Optional[bool] = True,
```

### Comparing `pwright-9.0.0/src/pwright/sync_api/_cms.py` & `pwright-9.1.0/src/pwright/sync_api/_cms.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 from contextlib import contextmanager
 import logging
 from pathlib import Path
 import typing as t
 
-from .._constants import INIT_SCRIPT_HIDE_NAVIGATOR
 from .._utils import to_milliseconds
+from ..constants import INIT_SCRIPT_HIDE_NAVIGATOR
+from ..typealiases import BrowserTypeT
 from ..typealiases import SecondsT
+from ._apis import BrowserType
 from ._apis import ProxySettings
 from ._apis import playwright
 
 
 logger = logging.getLogger(__name__)
 
 
 @contextmanager
 def playwright_browser(
     *,
     # [browser]
+    browser_type: t.Optional[BrowserTypeT] = None,
     executable_path: t.Optional[t.Union[str, Path]] = None,
     headed: t.Optional[bool] = None,
     proxy: t.Optional[ProxySettings] = None,
     slow_mo: t.Optional[SecondsT] = None,
     traces_dir: t.Optional[t.Union[str, Path]] = None,
 ):
+    browser_type = browser_type or 'chromium'
     # https://playwright.dev/python/docs/test-runners#fixtures
     with playwright() as _playwright:
         logger.debug(f'{_playwright = }')
-        with _playwright.chromium.launch(
+        with t.cast(BrowserType, getattr(_playwright, browser_type)).launch(
             executable_path=executable_path,
             headless=not headed,
             proxy=proxy,
             slow_mo=to_milliseconds(slow_mo),
             traces_dir=traces_dir,
         ) as browser:
-            browser_type = browser.browser_type
-            logger.debug(f'{browser_type = }')
-            logger.debug(f'{browser = }')
-            browser_name = browser_type.name
-            logger.debug(f'{browser_name = }')
+            logger.debug(f'{browser.browser_type.name = }')
             yield browser
 
 
 @contextmanager
 def playwright_context(
     *,
     # [browser]
+    browser_type: t.Optional[BrowserTypeT] = None,
     executable_path: t.Optional[t.Union[str, Path]] = None,
     headed: t.Optional[bool] = None,
     proxy: t.Optional[ProxySettings] = None,
     slow_mo: t.Optional[SecondsT] = None,
     traces_dir: t.Optional[t.Union[str, Path]] = None,
     # [context]
     no_viewport: t.Optional[bool] = True,
@@ -59,14 +60,15 @@
     tracing=False,
     snapshots=True,
     screenshots=True,
     sources=True,
     path='trace.zip',
 ):
     with playwright_browser(
+        browser_type=browser_type,
         executable_path=executable_path,
         headed=headed,
         proxy=proxy,
         slow_mo=slow_mo,
         traces_dir=traces_dir,
     ) as browser:
         with browser.new_context(
@@ -89,14 +91,15 @@
                 )
 
 
 @contextmanager
 def playwright_page(
     *,
     # [browser]
+    browser_type: t.Optional[BrowserTypeT] = None,
     executable_path: t.Optional[t.Union[str, Path]] = None,
     headed: t.Optional[bool] = None,
     proxy: t.Optional[ProxySettings] = None,
     slow_mo: t.Optional[SecondsT] = None,
     traces_dir: t.Optional[t.Union[str, Path]] = None,
     # [context]
     no_viewport: t.Optional[bool] = True,
@@ -112,14 +115,15 @@
     # [page]
     default_navigation_timeout: t.Optional[SecondsT] = None,
     default_timeout: t.Optional[SecondsT] = None,
     init_script: t.Optional[str] = INIT_SCRIPT_HIDE_NAVIGATOR,
     init_script_path: t.Optional[t.Union[str, Path]] = None,
 ):
     with playwright_context(
+        browser_type=browser_type,
         executable_path=executable_path,
         headed=headed,
         proxy=proxy,
         slow_mo=slow_mo,
         traces_dir=traces_dir,
         no_viewport=no_viewport,
         user_agent=user_agent,
```

### Comparing `pwright-9.0.0/src/pwright/sync_api/utils.py` & `pwright-9.1.0/src/pwright/sync_api/utils.py`

 * *Files identical despite different names*

### Comparing `pwright-9.0.0/tests/test_apw.py` & `pwright-9.1.0/tests/test_apw.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 import asyncio
 from contextlib import asynccontextmanager
 import sys
 import time
 
 from pwright import apw as pw
+from pwright.typealiases import BrowserTypeT
 
 
 if sys.version_info < (3, 10):
     anext = pw.anext
 
 
-def test_pw_page():
+def test_pw_page(browser_type):
     async def get_title(*, url: str):
-        async with pw.pw_page() as page:
+        async with pw.pw_page(browser_type=browser_type) as page:
             await page.goto(url)
             title = await page.title()
             return title
 
     assert 'Playwright' in asyncio.run(get_title(url='https://playwright.dev/'))
 
 
-async def _test_renew(headed=True):
+async def _test_renew(*, browser_type: BrowserTypeT = 'firefox', headed=True):
     @asynccontextmanager
     async def gen_page():
-        async with pw.pw_page(headed=headed) as page:
+        async with pw.pw_page(browser_type=browser_type, headed=headed) as page:
             yield page
 
     gen_page_cm: pw.AsyncGeneratorContextManager[pw.Page] = gen_page
 
     async def run(*, page_gen: pw.AsyncGenerator[pw.Page]):
         for _ in range(5):
             page = await anext(page_gen)
@@ -43,13 +44,13 @@
     await run(page_gen=auto_renew_page_gen)
 
     renewing: pw.AsyncGeneratorContextManagerAsyncGenerator[pw.Page] = pw.renewing(gen_page_cm, 3)
     async with renewing as agen:
         await run(page_gen=agen)
 
 
-def test_renew():
-    asyncio.run(_test_renew(headed=False))
+def test_renew(browser_type):
+    asyncio.run(_test_renew(browser_type=browser_type, headed=False))
 
 
 if __name__ == '__main__':
     asyncio.run(_test_renew())
```

### Comparing `pwright-9.0.0/tests/test_pw.py` & `pwright-9.1.0/tests/test_pw.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from contextlib import contextmanager
 import time
 
 from pwright import pw
+from pwright.typealiases import BrowserTypeT
 
 
-def test_pw_page():
+def test_pw_page(browser_type):
     def get_title(*, url: str):
-        with pw.pw_page() as page:
+        with pw.pw_page(browser_type=browser_type) as page:
             page.goto(url)
             title = page.title()
             return title
 
     assert 'Playwright' in get_title(url='https://playwright.dev/')
 
 
-def _test_renew(headed=True):
+def _test_renew(*, browser_type: BrowserTypeT = 'firefox', headed=True):
     @contextmanager
     def gen_page():
-        with pw.pw_page(headed=headed) as page:
+        with pw.pw_page(browser_type=browser_type, headed=headed) as page:
             yield page
 
     gen_page_cm: pw.GeneratorContextManager[pw.Page] = gen_page
 
     def run(*, page_gen: pw.Generator[pw.Page]):
         for _ in range(5):
             page = next(page_gen)
@@ -37,13 +38,13 @@
     run(page_gen=auto_renew_page_gen)
 
     renewing: pw.GeneratorContextManagerGenerator[pw.Page] = pw.renewing(gen_page_cm, 3)
     with renewing as page_gen:
         run(page_gen=page_gen)
 
 
-def test_renew():
-    _test_renew(headed=False)
+def test_renew(browser_type):
+    _test_renew(browser_type=browser_type, headed=False)
 
 
 if __name__ == '__main__':
     _test_renew()
```

