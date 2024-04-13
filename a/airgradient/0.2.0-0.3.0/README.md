# Comparing `tmp/airgradient-0.2.0.tar.gz` & `tmp/airgradient-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airgradient-0.2.0.tar", max compression
+gzip compressed data, was "airgradient-0.3.0.tar", max compression
```

## Comparing `airgradient-0.2.0.tar` & `airgradient-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1070 2024-03-24 15:24:50.969033 airgradient-0.2.0/LICENSE.md
--rw-r--r--   0        0        0     4793 2024-03-24 15:24:50.969033 airgradient-0.2.0/README.md
--rw-r--r--   0        0        0     3856 2024-03-24 15:25:01.200922 airgradient-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      339 2024-03-24 15:24:50.973033 airgradient-0.2.0/src/airgradient/__init__.py
--rw-r--r--   0        0        0     2801 2024-03-24 15:24:50.973033 airgradient-0.2.0/src/airgradient/airgradient.py
--rw-r--r--   0        0        0      214 2024-03-24 15:24:50.973033 airgradient-0.2.0/src/airgradient/exceptions.py
--rw-r--r--   0        0        0     1494 2024-03-24 15:24:50.973033 airgradient-0.2.0/src/airgradient/models.py
--rw-r--r--   0        0        0        0 2024-03-24 15:24:50.973033 airgradient-0.2.0/src/airgradient/py.typed
--rw-r--r--   0        0        0     6127 1970-01-01 00:00:00.000000 airgradient-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-13 11:01:43.923260 airgradient-0.3.0/LICENSE.md
+-rw-r--r--   0        0        0     4673 2024-04-13 11:01:43.923260 airgradient-0.3.0/README.md
+-rw-r--r--   0        0        0     3856 2024-04-13 11:01:55.550829 airgradient-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      540 2024-04-13 11:01:43.927260 airgradient-0.3.0/src/airgradient/__init__.py
+-rw-r--r--   0        0        0     3808 2024-04-13 11:01:43.927260 airgradient-0.3.0/src/airgradient/airgradient.py
+-rw-r--r--   0        0        0      214 2024-04-13 11:01:43.927260 airgradient-0.3.0/src/airgradient/exceptions.py
+-rw-r--r--   0        0        0     2733 2024-04-13 11:01:43.927260 airgradient-0.3.0/src/airgradient/models.py
+-rw-r--r--   0        0        0        0 2024-04-13 11:01:43.927260 airgradient-0.3.0/src/airgradient/py.typed
+-rw-r--r--   0        0        0     6007 1970-01-01 00:00:00.000000 airgradient-0.3.0/PKG-INFO
```

### Comparing `airgradient-0.2.0/LICENSE.md` & `airgradient-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `airgradient-0.2.0/README.md` & `airgradient-0.3.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -105,26 +105,25 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 
 [build-shield]: https://github.com/airgradienthq/python-airgradient/actions/workflows/tests.yaml/badge.svg
 [build]: https://github.com/airgradienthq/python-airgradient/actions
-[code-smells]: https://sonarcloud.io/api/project_badges/measure?project=joostlek_python-withings&metric=code_smells
 [codecov-shield]: https://codecov.io/gh/airgradienthq/python-airgradient/branch/master/graph/badge.svg
 [codecov]: https://codecov.io/gh/airgradienthq/python-airgradient
 [commits-shield]: https://img.shields.io/github/commit-activity/y/airgradienthq/python-airgradient.svg
 [commits]: https://github.com/airgradienthq/python-airgradient/commits/master
 [contributors]: https://github.com/airgradienthq/python-airgradient/graphs/contributors
 [joostlek]: https://github.com/joostlek
 [keepchangelog]: http://keepachangelog.com/en/1.0.0/
 [license-shield]: https://img.shields.io/github/license/airgradienthq/python-airgradient.svg
 [maintenance-shield]: https://img.shields.io/maintenance/yes/2024.svg
 [poetry-install]: https://python-poetry.org/docs/#installation
 [poetry]: https://python-poetry.org
 [pre-commit]: https://pre-commit.com/
 [project-stage-shield]: https://img.shields.io/badge/project%20stage-stable-green.svg
-[python-versions-shield]: https://img.shields.io/pypi/pyversions/airgradienthq
+[python-versions-shield]: https://img.shields.io/pypi/pyversions/airgradient
 [releases-shield]: https://img.shields.io/github/release/airgradienthq/python-airgradient.svg
 [releases]: https://github.com/airgradienthq/python-airgradient/releases
 [semver]: http://semver.org/spec/v2.0.0.html
-[pypi]: https://pypi.org/project/airgradienthq/
+[pypi]: https://pypi.org/project/airgradient/
```

### Comparing `airgradient-0.2.0/pyproject.toml` & `airgradient-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "airgradient"
-version = "0.2.0"
+version = "0.3.0"
 description = "Asynchronous Python client for AirGradient."
 authors = ["Joost Lekkerkerker <joostlek@outlook.com>"]
 maintainers = ["Joost Lekkerkerker <joostlek@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/airgradienthq/python-airgradient"
 repository = "https://github.com/airgradienthq/python-airgradient"
@@ -32,22 +32,22 @@
 orjson = ">=3.9.0"
 
 [tool.poetry.group.dev.dependencies]
 codespell = "2.2.6"
 covdefaults = "2.3.0"
 coverage = {version = "7.4.4", extras = ["toml"]}
 mypy = "1.9.0"
-pre-commit = "3.6.2"
-pre-commit-hooks = "4.5.0"
+pre-commit = "3.7.0"
+pre-commit-hooks = "4.6.0"
 pylint = "3.1.0"
 pytest = "8.1.1"
 pytest-asyncio = "0.23.6"
-pytest-cov = "4.1.0"
-ruff = "0.3.4"
-safety = "3.0.1"
+pytest-cov = "5.0.0"
+ruff = "0.3.7"
+safety = "3.1.0"
 yamllint = "1.35.1"
 syrupy = "4.6.1"
 aioresponses = "0.7.6"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/airgradienthq/python-airgradient/issues"
 Changelog = "https://github.com/airgradienthq/python-airgradient/releases"
```

### Comparing `airgradient-0.2.0/src/airgradient/airgradient.py` & `airgradient-0.3.0/src/airgradient/airgradient.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 """Asynchronous Python client for AirGradient."""
 
 from __future__ import annotations
 
-import asyncio
 from dataclasses import dataclass
 from importlib import metadata
 from typing import TYPE_CHECKING, Any
 
 from aiohttp import ClientSession
-from aiohttp.hdrs import METH_GET
+from aiohttp.hdrs import METH_GET, METH_PUT
 from yarl import URL
 
-from .exceptions import AirGradientConnectionError, AirGradientError
-from .models import Measures
+from .exceptions import AirGradientConnectionError
+from .models import (
+    Config,
+    ConfigurationControl,
+    LedBarMode,
+    Measures,
+    PmStandard,
+    TemperatureUnit,
+)
 
 if TYPE_CHECKING:
     from typing_extensions import Self
 
 
 VERSION = metadata.version(__package__)
 
@@ -30,57 +36,79 @@
     request_timeout: int = 10
     _close_session: bool = False
 
     async def _request(
         self,
         uri: str,
         *,
+        method: str = METH_GET,
         data: dict[str, Any] | None = None,
     ) -> str:
         """Handle a request to AirGradient."""
         url = URL.build(scheme="http", host=self.host).joinpath(uri)
 
         headers = {
             "User-Agent": f"PythonAirGradient/{VERSION}",
             "Accept": "application/json, text/plain, */*",
         }
 
         if self.session is None:
             self.session = ClientSession()
             self._close_session = True
 
-        try:
-            async with asyncio.timeout(self.request_timeout):
-                response = await self.session.request(
-                    METH_GET,
-                    url,
-                    headers=headers,
-                    data=data,
-                )
-        except asyncio.TimeoutError as exception:
-            msg = "Timeout occurred while connecting to AirGradient"
-            raise AirGradientConnectionError(msg) from exception
+        response = await self.session.request(
+            method,
+            url,
+            headers=headers,
+            data=data,
+        )
 
-        content_type = response.headers.get("Content-Type", "")
-
-        if "application/json" not in content_type:
+        if response.status != 200:
+            content_type = response.headers.get("Content-Type", "")
             text = await response.text()
             msg = "Unexpected response from AirGradient"
-            raise AirGradientError(
+            raise AirGradientConnectionError(
                 msg,
                 {"Content-Type": content_type, "response": text},
             )
 
         return await response.text()
 
     async def get_current_measures(self) -> Measures:
         """Get current measures from AirGradient."""
         response = await self._request("measures/current")
         return Measures.from_json(response)
 
+    async def get_config(self) -> Config:
+        """Get config from AirGradient device."""
+        response = await self._request("config")
+        return Config.from_json(response)
+
+    async def _set_config(self, field: str, value: Any) -> None:
+        """Set config on AirGradient device."""
+        await self._request("config", method=METH_PUT, data={field: value})
+
+    async def set_pm_standard(self, pm_standard: PmStandard) -> None:
+        """Set PM standard on AirGradient device."""
+        await self._set_config("pmStandard", pm_standard)
+
+    async def set_temperature_unit(self, temperature_unit: TemperatureUnit) -> None:
+        """Set temperature unit on AirGradient device."""
+        await self._set_config("temperatureUnit", temperature_unit)
+
+    async def set_configuration_control(
+        self, configuration_control: ConfigurationControl
+    ) -> None:
+        """Set configuration control on AirGradient device."""
+        await self._set_config("configurationControl", configuration_control)
+
+    async def set_led_bar_mode(self, led_bar_mode: LedBarMode) -> None:
+        """Set LED bar mode on AirGradient device."""
+        await self._set_config("ledBarMode", led_bar_mode)
+
     async def close(self) -> None:
         """Close open client session."""
         if self.session and self._close_session:
             await self.session.close()
 
     async def __aenter__(self) -> Self:
         """Async enter.
```

### Comparing `airgradient-0.2.0/PKG-INFO` & `airgradient-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airgradient
-Version: 0.2.0
+Version: 0.3.0
 Summary: Asynchronous Python client for AirGradient.
 Home-page: https://github.com/airgradienthq/python-airgradient
 License: MIT
 Keywords: Airgradient,api,async,client
 Author: Joost Lekkerkerker
 Author-email: joostlek@outlook.com
 Maintainer: Joost Lekkerkerker
@@ -136,27 +136,26 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 
 [build-shield]: https://github.com/airgradienthq/python-airgradient/actions/workflows/tests.yaml/badge.svg
 [build]: https://github.com/airgradienthq/python-airgradient/actions
-[code-smells]: https://sonarcloud.io/api/project_badges/measure?project=joostlek_python-withings&metric=code_smells
 [codecov-shield]: https://codecov.io/gh/airgradienthq/python-airgradient/branch/master/graph/badge.svg
 [codecov]: https://codecov.io/gh/airgradienthq/python-airgradient
 [commits-shield]: https://img.shields.io/github/commit-activity/y/airgradienthq/python-airgradient.svg
 [commits]: https://github.com/airgradienthq/python-airgradient/commits/master
 [contributors]: https://github.com/airgradienthq/python-airgradient/graphs/contributors
 [joostlek]: https://github.com/joostlek
 [keepchangelog]: http://keepachangelog.com/en/1.0.0/
 [license-shield]: https://img.shields.io/github/license/airgradienthq/python-airgradient.svg
 [maintenance-shield]: https://img.shields.io/maintenance/yes/2024.svg
 [poetry-install]: https://python-poetry.org/docs/#installation
 [poetry]: https://python-poetry.org
 [pre-commit]: https://pre-commit.com/
 [project-stage-shield]: https://img.shields.io/badge/project%20stage-stable-green.svg
-[python-versions-shield]: https://img.shields.io/pypi/pyversions/airgradienthq
+[python-versions-shield]: https://img.shields.io/pypi/pyversions/airgradient
 [releases-shield]: https://img.shields.io/github/release/airgradienthq/python-airgradient.svg
 [releases]: https://github.com/airgradienthq/python-airgradient/releases
 [semver]: http://semver.org/spec/v2.0.0.html
-[pypi]: https://pypi.org/project/airgradienthq/
+[pypi]: https://pypi.org/project/airgradient/
```

