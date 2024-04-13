# Comparing `tmp/curseforge-1.6.0.tar.gz` & `tmp/curseforge-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curseforge-1.6.0.tar", last modified: Fri Nov  3 04:25:38 2023, max compression
+gzip compressed data, was "curseforge-1.6.1.tar", last modified: Sat Apr 13 20:02:01 2024, max compression
```

## Comparing `curseforge-1.6.0.tar` & `curseforge-1.6.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-11-03 04:25:38.823150 curseforge-1.6.0/
--rw-rw-rw-   0        0        0     1083 2023-11-03 03:56:37.000000 curseforge-1.6.0/LICENSE.txt
--rw-rw-rw-   0        0        0     2853 2023-11-03 04:25:38.822175 curseforge-1.6.0/PKG-INFO
--rw-rw-rw-   0        0        0     2193 2023-11-03 03:56:37.000000 curseforge-1.6.0/README.md
-drwxrwxrwx   0        0        0        0 2023-11-03 04:25:38.792365 curseforge-1.6.0/curseforge/
--rw-rw-rw-   0        0        0       21 2023-11-03 03:56:37.000000 curseforge-1.6.0/curseforge/__init__.py
--rw-rw-rw-   0        0        0     1695 2023-11-03 04:16:54.000000 curseforge-1.6.0/curseforge/__main__.py
--rw-rw-rw-   0        0        0     5147 2023-11-03 04:10:35.000000 curseforge-1.6.0/curseforge/base.py
-drwxrwxrwx   0        0        0        0 2023-11-03 04:25:38.810446 curseforge-1.6.0/curseforge/classes/
--rw-rw-rw-   0        0        0      174 2023-11-03 03:56:37.000000 curseforge-1.6.0/curseforge/classes/__init__.py
--rw-rw-rw-   0        0        0      255 2023-11-03 03:56:37.000000 curseforge-1.6.0/curseforge/classes/base.py
--rw-rw-rw-   0        0        0      909 2023-11-03 03:56:37.000000 curseforge-1.6.0/curseforge/classes/cursecategory.py
--rw-rw-rw-   0        0        0      754 2023-11-03 03:56:37.000000 curseforge-1.6.0/curseforge/classes/cursegame.py
--rw-rw-rw-   0        0        0      219 2023-11-03 03:56:37.000000 curseforge-1.6.0/curseforge/classes/curseimage.py
--rw-rw-rw-   0        0        0     5032 2023-11-03 03:56:37.000000 curseforge-1.6.0/curseforge/classes/cursemod.py
--rw-rw-rw-   0        0        0      306 2023-11-03 03:56:37.000000 curseforge-1.6.0/curseforge/classes/hashe.py
--rw-rw-rw-   0        0        0     1088 2023-11-03 03:56:37.000000 curseforge-1.6.0/curseforge/classes/manifest.py
-drwxrwxrwx   0        0        0        0 2023-11-03 04:25:38.821151 curseforge-1.6.0/curseforge/util/
--rw-rw-rw-   0        0        0       30 2023-11-03 03:56:37.000000 curseforge-1.6.0/curseforge/util/__init__.py
--rw-rw-rw-   0        0        0      330 2023-11-03 03:56:37.000000 curseforge-1.6.0/curseforge/util/manifest_parser.py
--rw-rw-rw-   0        0        0      379 2023-11-03 04:18:29.000000 curseforge-1.6.0/curseforge/util/probe_cursecache.py
-drwxrwxrwx   0        0        0        0 2023-11-03 04:25:38.801396 curseforge-1.6.0/curseforge.egg-info/
--rw-rw-rw-   0        0        0     2853 2023-11-03 04:25:38.000000 curseforge-1.6.0/curseforge.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      612 2023-11-03 04:25:38.000000 curseforge-1.6.0/curseforge.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-03 04:25:38.000000 curseforge-1.6.0/curseforge.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-11-03 04:25:38.000000 curseforge-1.6.0/curseforge.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-11-03 04:25:38.000000 curseforge-1.6.0/curseforge.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-11-03 04:25:38.823150 curseforge-1.6.0/setup.cfg
--rw-rw-rw-   0        0        0     1120 2023-11-03 04:12:51.000000 curseforge-1.6.0/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-13 20:02:01.005748 curseforge-1.6.1/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1062 2024-04-13 19:42:56.000000 curseforge-1.6.1/LICENSE.txt
+-rw-r--r--   0 codespace  (1000) codespace  (1000)     2684 2024-04-13 20:02:01.005748 curseforge-1.6.1/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2116 2024-04-13 19:44:13.000000 curseforge-1.6.1/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-13 20:02:00.993748 curseforge-1.6.1/curseforge/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       37 2024-04-13 19:50:19.000000 curseforge-1.6.1/curseforge/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4013 2024-04-13 19:42:56.000000 curseforge-1.6.1/curseforge/__main__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5005 2024-04-13 19:42:56.000000 curseforge-1.6.1/curseforge/base.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-13 20:02:01.001748 curseforge-1.6.1/curseforge/classes/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      168 2024-04-13 19:42:56.000000 curseforge-1.6.1/curseforge/classes/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      246 2024-04-13 19:42:56.000000 curseforge-1.6.1/curseforge/classes/base.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      878 2024-04-13 19:42:56.000000 curseforge-1.6.1/curseforge/classes/cursecategory.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      725 2024-04-13 19:42:56.000000 curseforge-1.6.1/curseforge/classes/cursegame.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      207 2024-04-13 19:42:56.000000 curseforge-1.6.1/curseforge/classes/curseimage.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4859 2024-04-13 19:42:56.000000 curseforge-1.6.1/curseforge/classes/cursemod.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      292 2024-04-13 19:42:56.000000 curseforge-1.6.1/curseforge/classes/hashe.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1050 2024-04-13 19:42:56.000000 curseforge-1.6.1/curseforge/classes/manifest.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-13 20:02:01.001748 curseforge-1.6.1/curseforge/util/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       30 2024-04-13 19:42:56.000000 curseforge-1.6.1/curseforge/util/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      320 2024-04-13 19:42:56.000000 curseforge-1.6.1/curseforge/util/manifest_parser.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      362 2024-04-13 19:42:56.000000 curseforge-1.6.1/curseforge/util/probe_cursecache.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-13 20:02:01.005748 curseforge-1.6.1/curseforge.egg-info/
+-rw-r--r--   0 codespace  (1000) codespace  (1000)     2684 2024-04-13 20:02:00.000000 curseforge-1.6.1/curseforge.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      612 2024-04-13 20:02:00.000000 curseforge-1.6.1/curseforge.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-04-13 20:02:00.000000 curseforge-1.6.1/curseforge.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       19 2024-04-13 20:02:00.000000 curseforge-1.6.1/curseforge.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       11 2024-04-13 20:02:00.000000 curseforge-1.6.1/curseforge.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-04-13 20:02:01.005748 curseforge-1.6.1/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1147 2024-04-13 19:52:29.000000 curseforge-1.6.1/setup.py
```

### Comparing `curseforge-1.6.0/LICENSE.txt` & `curseforge-1.6.1/LICENSE.txt`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 Advik
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2022 Advik
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `curseforge-1.6.0/PKG-INFO` & `curseforge-1.6.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,92 +1,91 @@
-Metadata-Version: 2.1
-Name: curseforge
-Version: 1.6.0
-Summary: A no-compromises wrapper for the CurseForge API
-Home-page: https://github.com/Advik-B/curseforge-api
-Author: Advik
-Author-email: <advik.b@gmail.com>
-Keywords: CMPDL,Minecraft,Curseforge,API,Wrapper
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-Requires-Dist: requests
-Requires-Dist: diskcache
-
-
-# Curseforge API
-
-[cfapi]: https://wow.curseforge.com/api
-[cfapi-docs]: https://wow.curseforge.com/api/docs
-[not-working-cfapi]: https://github.com/Owen-Cochell/cursepy
-[cmpdl]: https://github.com/Advik-B/CMPDL
-
-This is a no-compromise CurseForge API wrapper for python. It is a re-write of [cursepy][not-working-cfapi] which is maintained but not actively developed.
-This project is a complete re-write of the original project, with a focus on simplicity and ease of use.
-
-This project is still in development, and is not yet ready for production use.
-It also speeds up the process by using disk caching, It will cache the response from the API and will only make a new request if the request is not cached.
-
-This, of course can be disabled by setting the cache to False.
-
-## Features
-
-- Simple and easy to use
-- Caches responses from the API to disk for faster response times
-- Allows direct access to the API via the `fetch` method
-- Allows exporting of the objects to DICT, JSON, or YAML
-- Can directly parse a manifest file from a curseforge modpack
-- 
-
-## Installation
-
-```bash
-pip install curseforge
-```
-
-## Usage
-
-```python
-from curseforge import CurseClient
-
-client = CurseClient("API-KEY", cache=True)
-
-minecraft = client.game(432) # 432 is the ID of Minecraft
-
-# or we can list all the games
-games = client.games()
-
-for game in games:
-    print(game.name)
-
-# The search is up to the user to implement, this is just a wrapper
-
-# We can also get the latest files for a project
-
-JourneyMap = client.mod(2238) # 2238 is the ID of JourneyMap
-
-for file in JourneyMap.files:
-    print(file.name)
-```
-
-## TODO
-
-- [x] Implement the export methods
-- [x] Implement the cache
-- [x] Implement the fetch method
-- [x] Deal with the download URL being a null value
-- [ ] Implement the search method
-- [ ] Wrap the ENTIRE API
-- [x] Rename the classes so they have a `Curse` prefix
-
-## Contributing
-
-Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
-
-Please make sure to update tests as appropriate.
-
-## License
-
-[MIT](https://choosealicense.com/licenses/mit/)
+Metadata-Version: 2.1
+Name: curseforge
+Version: 1.6.1
+Summary: A no-compromises wrapper for the CurseForge API
+Home-page: https://github.com/Advik-B/curseforge-api
+Author: Advik
+Author-email: <advik.b@gmail.com>
+Keywords: CMPDL,Minecraft,Curseforge,API,Wrapper
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: requests
+Requires-Dist: diskcache
+
+
+# Curseforge API
+
+[cfapi]: https://wow.curseforge.com/api
+[cfapi-docs]: https://wow.curseforge.com/api/docs
+[not-working-cfapi]: https://github.com/Owen-Cochell/cursepy
+[cmpdl]: https://github.com/Advik-B/CMPDL
+
+This is a no-compromise CurseForge API wrapper for python. It is a re-write of [cursepy][not-working-cfapi] which is maintained but not actively developed.
+This project is a complete re-write of the original project, with a focus on simplicity and ease of use.
+
+This project is still in development, and is not yet ready for production use.
+It also speeds up the process by using disk caching, It will cache the response from the API and will only make a new request if the request is not cached.
+
+This, of course can be disabled by setting the cache to False.
+
+## Features
+
+- Simple and easy to use
+- Caches responses from the API to disk for faster response times
+- Allows direct access to the API via the `fetch` method
+- Allows exporting of the objects to DICT, JSON, or YAML
+- Can directly parse a manifest file from a curseforge modpack
+
+## Installation
+
+```bash
+pip install curseforge
+```
+
+## Usage
+
+```python
+from curseforge import CurseClient
+
+client = CurseClient("API-KEY", cache=True)
+
+minecraft = client.game(432) # 432 is the ID of Minecraft
+
+# or we can list all the games
+games = client.games()
+
+for game in games:
+    print(game.name)
+
+# The search is up to the user to implement, this is just a wrapper
+
+# We can also get the latest files for a project
+
+JourneyMap = client.mod(2238) # 2238 is the ID of JourneyMap
+
+for file in JourneyMap.files:
+    print(file.name)
+```
+
+## TODO
+
+- [x] Implement the export methods
+- [x] Implement the cache
+- [x] Implement the fetch method
+- [x] Deal with the download URL being a null value
+- [ ] Implement the search method
+- [ ] Wrap the ENTIRE API
+- [x] Rename the classes so they have a `Curse` prefix
+
+## Contributing
+
+Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
+
+Please make sure to update tests as appropriate.
+
+## License
+
+[MIT](https://choosealicense.com/licenses/mit/)
```

### Comparing `curseforge-1.6.0/curseforge/classes/cursecategory.py` & `curseforge-1.6.1/curseforge/classes/cursecategory.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-from dataclasses import dataclass
-from .base import CurseObject
-
-@dataclass
-class CurseCategory(CurseObject):
-    id: int
-    game_id: int
-    name: str
-    slug: str
-    url: str
-    icon_url: str
-    date_modified: str
-    is_Class: bool
-    class_id: int
-    parentCategory_id: int
-    displayIndex: int
-
-    @staticmethod
-    def from_dict(data: dict) -> "CurseCategory":
-        return CurseCategory(
-            id=data.get("id"),
-            game_id=data.get("gameId"),
-            name=data.get("name"),
-            slug=data.get("slug"),
-            url=data.get("url"),
-            icon_url=data.get("iconUrl"),
-            date_modified=data.get("dateModified"),
-            is_Class=data.get("isClass"),
-            class_id=data.get("classId"),
-            parentCategory_id=data.get("parentCategoryId"),
-            displayIndex=data.get("displayIndex"),
+from dataclasses import dataclass
+from .base import CurseObject
+
+@dataclass
+class CurseCategory(CurseObject):
+    id: int
+    game_id: int
+    name: str
+    slug: str
+    url: str
+    icon_url: str
+    date_modified: str
+    is_Class: bool
+    class_id: int
+    parentCategory_id: int
+    displayIndex: int
+
+    @staticmethod
+    def from_dict(data: dict) -> "CurseCategory":
+        return CurseCategory(
+            id=data.get("id"),
+            game_id=data.get("gameId"),
+            name=data.get("name"),
+            slug=data.get("slug"),
+            url=data.get("url"),
+            icon_url=data.get("iconUrl"),
+            date_modified=data.get("dateModified"),
+            is_Class=data.get("isClass"),
+            class_id=data.get("classId"),
+            parentCategory_id=data.get("parentCategoryId"),
+            displayIndex=data.get("displayIndex"),
         )
```

### Comparing `curseforge-1.6.0/curseforge/classes/cursegame.py` & `curseforge-1.6.1/curseforge/classes/cursegame.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-from dataclasses import dataclass
-from .base import CurseObject
-
-@dataclass
-class CurseGameAssets(CurseObject):
-    icon_url: str
-    tile_url: str
-    cover_url: str
-
-@dataclass
-class CurseGame(CurseObject):
-    id: int
-    name: str
-    slug: str
-    assets: CurseGameAssets
-    status: int
-    api_status: int
-    date_modified: str
-
-    @staticmethod
-    def from_dict(data: dict):
-        return CurseGame(
-            id=data.get("id"),
-            name=data.get("name"),
-            slug=data.get("slug"),
-            assets=CurseGameAssets(*data.get("assets").values()),
-            status=data.get("status"),
-            api_status=data.get("apiStatus"),
-            date_modified=data.get("dateModified"),
+from dataclasses import dataclass
+from .base import CurseObject
+
+@dataclass
+class CurseGameAssets(CurseObject):
+    icon_url: str
+    tile_url: str
+    cover_url: str
+
+@dataclass
+class CurseGame(CurseObject):
+    id: int
+    name: str
+    slug: str
+    assets: CurseGameAssets
+    status: int
+    api_status: int
+    date_modified: str
+
+    @staticmethod
+    def from_dict(data: dict):
+        return CurseGame(
+            id=data.get("id"),
+            name=data.get("name"),
+            slug=data.get("slug"),
+            assets=CurseGameAssets(*data.get("assets").values()),
+            status=data.get("status"),
+            api_status=data.get("apiStatus"),
+            date_modified=data.get("dateModified"),
         )
```

### Comparing `curseforge-1.6.0/curseforge/classes/cursemod.py` & `curseforge-1.6.1/curseforge/classes/cursemod.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,173 +1,173 @@
-from dataclasses import dataclass
-from .curseimage import CurseImage
-from .base import CurseObject
-from .cursecategory import CurseCategory
-from .hashe import CurseHash
-
-
-@dataclass
-class CurseModAuthor(CurseObject):
-    id: int
-    name: str
-    url: str
-
-
-@dataclass
-class CurseModLinks(CurseObject):
-    website_url: str
-    wiki_url: str
-    issue_tracker_url: str
-    source_code_url: str
-
-
-# CurseModLogo and CurseScreenShot are a subclass of CurseImage because they share the same attributes
-@dataclass
-class CurseModLogo(CurseImage): pass
-
-@dataclass
-class CurseScreenShot(CurseImage): pass
-
-@dataclass
-class CurseSortableGameVersion(CurseObject):
-    game_version_name: str
-    game_version_padded: str
-    game_version: str
-    game_version_release_date: str
-    game_version_type_id: int
-
-    @staticmethod
-    def from_dict(data: dict):
-        return CurseSortableGameVersion(
-            game_version_name=data.get("gameVersionName"),
-            game_version_padded=data.get("gameVersionPadded"),
-            game_version=data.get("gameVersion"),
-            game_version_release_date=data.get("gameVersionReleaseDate"),
-            game_version_type_id=data.get("gameVersionTypeId")
-        )
-
-@dataclass
-class CurseDependency(CurseObject):
-    mod_id: int
-    relation_type: int
-
-    @staticmethod
-    def from_dict(data: dict):
-        return CurseDependency(
-            mod_id=data.get("mod_id"),
-            relation_type=data.get("relation_type")
-        )
-
-
-@dataclass
-class CurseModule(CurseObject):
-    name: str
-    fingerprint: int
-
-    @staticmethod
-    def from_dict(data: dict):
-        return CurseModule(
-            name=data.get("name"),
-            fingerprint=data.get("fingerprint")
-        )
-
-@dataclass
-class CurseFileIndex(CurseObject):
-    game_version: str
-    file_id: int
-    file_name: str
-    release_type: int
-    game_version_type_id: int
-    mod_loader: int
-
-
-@dataclass
-class CurseModFile(CurseObject):
-    id: int
-    game_id: int
-    mod_id: int
-    isAvailable: bool
-    display_name: str
-    file_name: str
-    release_type: int
-    file_status: int
-    hashes: tuple[CurseHash]
-    file_date: str
-    file_length: int
-    download_count: int
-    download_url: str
-    game_versions: tuple[str]
-    sortable_game_version: tuple[CurseSortableGameVersion]
-    dependencies: tuple[CurseDependency]
-    expose_as_alternate: bool
-    parent_project_file_id: int
-    altername_file_id: int
-    is_server_pack: bool
-    server_pack_file_id: int
-    file_finger_print: str
-    modules: tuple[CurseModule]
-
-    @staticmethod
-    def from_dict(data: dict):
-        return CurseModFile(
-            id=data.get("id"),
-            game_id=data.get("gameId"),
-            mod_id=data.get("modId"),
-            isAvailable=data.get("isAvailable"),
-            display_name=data.get("displayName"),
-            file_name=data.get("fileName"),
-            release_type=data.get("releaseType"),
-            file_status=data.get("fileStatus"),
-            hashes=tuple(CurseHash.from_dict(hash_) for hash_ in data.get("hashes")), # type: ignore
-            file_date=data.get("fileDate"),
-            file_length=data.get("fileLength"),
-            download_count=data.get("downloadCount"),
-            download_url=data.get("downloadUrl"),
-            game_versions=tuple(data.get("gameVersions")),
-            sortable_game_version=tuple(CurseSortableGameVersion.from_dict(version) for version in data.get("sortableGameVersions")),
-            dependencies=tuple(CurseDependency.from_dict(dependency) for dependency in data.get("dependencies")),
-            expose_as_alternate=data.get("exposeAsAlternate"),
-            parent_project_file_id=data.get("parentProjectFileId"),
-            altername_file_id=data.get("alternameFileId"),
-            is_server_pack=data.get("isServerPack"),
-            server_pack_file_id=data.get("serverPackFileId"),
-            file_finger_print=data.get("fileFingerPrint"),
-            modules=tuple(CurseModule.from_dict(module_) for module_ in data.get("modules")),
-        )
-
-
-@dataclass
-class CurseMod(CurseObject):
-    id: int
-    game_id: int
-    name: str
-    slug: str
-    links: CurseModLinks
-    summary: str
-    status: int
-    download_count: int
-    is_featured: bool
-    primary_category_id: int
-    categories: tuple[CurseCategory]
-    class_id: int
-    authors: tuple[CurseModAuthor]
-    logo: CurseModLogo
-    screenshots: tuple[CurseScreenShot]
-    mainFile_id: int
-    latestFiles: tuple[CurseModFile]
-    latestFilesIndexes: tuple[CurseFileIndex]
-    data_created: str
-    data_modified: str
-    data_released: str
-    allow_mod_distribution: bool
-    game_popularity_rank: int
-    is_available: bool
-    thumbs_up_count: int
-
-    @staticmethod
-    def from_dict(data: dict):
-        """
-        Returns a CurseMod instance from a dict
-        """
-
-        return
-
+from dataclasses import dataclass
+from .curseimage import CurseImage
+from .base import CurseObject
+from .cursecategory import CurseCategory
+from .hashe import CurseHash
+
+
+@dataclass
+class CurseModAuthor(CurseObject):
+    id: int
+    name: str
+    url: str
+
+
+@dataclass
+class CurseModLinks(CurseObject):
+    website_url: str
+    wiki_url: str
+    issue_tracker_url: str
+    source_code_url: str
+
+
+# CurseModLogo and CurseScreenShot are a subclass of CurseImage because they share the same attributes
+@dataclass
+class CurseModLogo(CurseImage): pass
+
+@dataclass
+class CurseScreenShot(CurseImage): pass
+
+@dataclass
+class CurseSortableGameVersion(CurseObject):
+    game_version_name: str
+    game_version_padded: str
+    game_version: str
+    game_version_release_date: str
+    game_version_type_id: int
+
+    @staticmethod
+    def from_dict(data: dict):
+        return CurseSortableGameVersion(
+            game_version_name=data.get("gameVersionName"),
+            game_version_padded=data.get("gameVersionPadded"),
+            game_version=data.get("gameVersion"),
+            game_version_release_date=data.get("gameVersionReleaseDate"),
+            game_version_type_id=data.get("gameVersionTypeId")
+        )
+
+@dataclass
+class CurseDependency(CurseObject):
+    mod_id: int
+    relation_type: int
+
+    @staticmethod
+    def from_dict(data: dict):
+        return CurseDependency(
+            mod_id=data.get("mod_id"),
+            relation_type=data.get("relation_type")
+        )
+
+
+@dataclass
+class CurseModule(CurseObject):
+    name: str
+    fingerprint: int
+
+    @staticmethod
+    def from_dict(data: dict):
+        return CurseModule(
+            name=data.get("name"),
+            fingerprint=data.get("fingerprint")
+        )
+
+@dataclass
+class CurseFileIndex(CurseObject):
+    game_version: str
+    file_id: int
+    file_name: str
+    release_type: int
+    game_version_type_id: int
+    mod_loader: int
+
+
+@dataclass
+class CurseModFile(CurseObject):
+    id: int
+    game_id: int
+    mod_id: int
+    isAvailable: bool
+    display_name: str
+    file_name: str
+    release_type: int
+    file_status: int
+    hashes: tuple[CurseHash]
+    file_date: str
+    file_length: int
+    download_count: int
+    download_url: str
+    game_versions: tuple[str]
+    sortable_game_version: tuple[CurseSortableGameVersion]
+    dependencies: tuple[CurseDependency]
+    expose_as_alternate: bool
+    parent_project_file_id: int
+    altername_file_id: int
+    is_server_pack: bool
+    server_pack_file_id: int
+    file_finger_print: str
+    modules: tuple[CurseModule]
+
+    @staticmethod
+    def from_dict(data: dict):
+        return CurseModFile(
+            id=data.get("id"),
+            game_id=data.get("gameId"),
+            mod_id=data.get("modId"),
+            isAvailable=data.get("isAvailable"),
+            display_name=data.get("displayName"),
+            file_name=data.get("fileName"),
+            release_type=data.get("releaseType"),
+            file_status=data.get("fileStatus"),
+            hashes=tuple(CurseHash.from_dict(hash_) for hash_ in data.get("hashes")), # type: ignore
+            file_date=data.get("fileDate"),
+            file_length=data.get("fileLength"),
+            download_count=data.get("downloadCount"),
+            download_url=data.get("downloadUrl"),
+            game_versions=tuple(data.get("gameVersions")),
+            sortable_game_version=tuple(CurseSortableGameVersion.from_dict(version) for version in data.get("sortableGameVersions")),
+            dependencies=tuple(CurseDependency.from_dict(dependency) for dependency in data.get("dependencies")),
+            expose_as_alternate=data.get("exposeAsAlternate"),
+            parent_project_file_id=data.get("parentProjectFileId"),
+            altername_file_id=data.get("alternameFileId"),
+            is_server_pack=data.get("isServerPack"),
+            server_pack_file_id=data.get("serverPackFileId"),
+            file_finger_print=data.get("fileFingerPrint"),
+            modules=tuple(CurseModule.from_dict(module_) for module_ in data.get("modules")),
+        )
+
+
+@dataclass
+class CurseMod(CurseObject):
+    id: int
+    game_id: int
+    name: str
+    slug: str
+    links: CurseModLinks
+    summary: str
+    status: int
+    download_count: int
+    is_featured: bool
+    primary_category_id: int
+    categories: tuple[CurseCategory]
+    class_id: int
+    authors: tuple[CurseModAuthor]
+    logo: CurseModLogo
+    screenshots: tuple[CurseScreenShot]
+    mainFile_id: int
+    latestFiles: tuple[CurseModFile]
+    latestFilesIndexes: tuple[CurseFileIndex]
+    data_created: str
+    data_modified: str
+    data_released: str
+    allow_mod_distribution: bool
+    game_popularity_rank: int
+    is_available: bool
+    thumbs_up_count: int
+
+    @staticmethod
+    def from_dict(data: dict):
+        """
+        Returns a CurseMod instance from a dict
+        """
+
+        return
+
```

### Comparing `curseforge-1.6.0/curseforge/classes/manifest.py` & `curseforge-1.6.1/curseforge/classes/manifest.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-from dataclasses import dataclass
-from .base import CurseObject
-
-@dataclass
-class CurseModFileManifest(CurseObject):
-    project_id: int
-    file_id: int
-    required: bool
-
-    @staticmethod
-    def from_dict(data: dict):
-        return CurseModFileManifest(
-            project_id=data.get("projectID"),
-            file_id=data.get("fileID"),
-            required=data.get("required")
-        )
-
-@dataclass
-class CurseManifest(CurseObject):
-    manifest_type: str
-    manifest_version: int
-    name: str
-    version: str
-    author: list[str]
-    files: list[CurseModFileManifest]
-    overrides: str
-
-    @staticmethod
-    def from_dict(data: dict):
-        return CurseManifest(
-            manifest_type=data.get("manifestType"),
-            manifest_version=data.get("manifestVersion"),
-            name=data.get("name"),
-            version=data.get("version"),
-            author=data.get("author"),
-            files=[CurseModFileManifest.from_dict(file) for file in data.get("files")],
-            overrides=data.get("overrides")
-        )
+from dataclasses import dataclass
+from .base import CurseObject
+
+@dataclass
+class CurseModFileManifest(CurseObject):
+    project_id: int
+    file_id: int
+    required: bool
+
+    @staticmethod
+    def from_dict(data: dict):
+        return CurseModFileManifest(
+            project_id=data.get("projectID"),
+            file_id=data.get("fileID"),
+            required=data.get("required")
+        )
+
+@dataclass
+class CurseManifest(CurseObject):
+    manifest_type: str
+    manifest_version: int
+    name: str
+    version: str
+    author: list[str]
+    files: list[CurseModFileManifest]
+    overrides: str
+
+    @staticmethod
+    def from_dict(data: dict):
+        return CurseManifest(
+            manifest_type=data.get("manifestType"),
+            manifest_version=data.get("manifestVersion"),
+            name=data.get("name"),
+            version=data.get("version"),
+            author=data.get("author"),
+            files=[CurseModFileManifest.from_dict(file) for file in data.get("files")],
+            overrides=data.get("overrides")
+        )
```

### Comparing `curseforge-1.6.0/curseforge.egg-info/PKG-INFO` & `curseforge-1.6.1/curseforge.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,92 +1,91 @@
-Metadata-Version: 2.1
-Name: curseforge
-Version: 1.6.0
-Summary: A no-compromises wrapper for the CurseForge API
-Home-page: https://github.com/Advik-B/curseforge-api
-Author: Advik
-Author-email: <advik.b@gmail.com>
-Keywords: CMPDL,Minecraft,Curseforge,API,Wrapper
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-Requires-Dist: requests
-Requires-Dist: diskcache
-
-
-# Curseforge API
-
-[cfapi]: https://wow.curseforge.com/api
-[cfapi-docs]: https://wow.curseforge.com/api/docs
-[not-working-cfapi]: https://github.com/Owen-Cochell/cursepy
-[cmpdl]: https://github.com/Advik-B/CMPDL
-
-This is a no-compromise CurseForge API wrapper for python. It is a re-write of [cursepy][not-working-cfapi] which is maintained but not actively developed.
-This project is a complete re-write of the original project, with a focus on simplicity and ease of use.
-
-This project is still in development, and is not yet ready for production use.
-It also speeds up the process by using disk caching, It will cache the response from the API and will only make a new request if the request is not cached.
-
-This, of course can be disabled by setting the cache to False.
-
-## Features
-
-- Simple and easy to use
-- Caches responses from the API to disk for faster response times
-- Allows direct access to the API via the `fetch` method
-- Allows exporting of the objects to DICT, JSON, or YAML
-- Can directly parse a manifest file from a curseforge modpack
-- 
-
-## Installation
-
-```bash
-pip install curseforge
-```
-
-## Usage
-
-```python
-from curseforge import CurseClient
-
-client = CurseClient("API-KEY", cache=True)
-
-minecraft = client.game(432) # 432 is the ID of Minecraft
-
-# or we can list all the games
-games = client.games()
-
-for game in games:
-    print(game.name)
-
-# The search is up to the user to implement, this is just a wrapper
-
-# We can also get the latest files for a project
-
-JourneyMap = client.mod(2238) # 2238 is the ID of JourneyMap
-
-for file in JourneyMap.files:
-    print(file.name)
-```
-
-## TODO
-
-- [x] Implement the export methods
-- [x] Implement the cache
-- [x] Implement the fetch method
-- [x] Deal with the download URL being a null value
-- [ ] Implement the search method
-- [ ] Wrap the ENTIRE API
-- [x] Rename the classes so they have a `Curse` prefix
-
-## Contributing
-
-Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
-
-Please make sure to update tests as appropriate.
-
-## License
-
-[MIT](https://choosealicense.com/licenses/mit/)
+Metadata-Version: 2.1
+Name: curseforge
+Version: 1.6.1
+Summary: A no-compromises wrapper for the CurseForge API
+Home-page: https://github.com/Advik-B/curseforge-api
+Author: Advik
+Author-email: <advik.b@gmail.com>
+Keywords: CMPDL,Minecraft,Curseforge,API,Wrapper
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: requests
+Requires-Dist: diskcache
+
+
+# Curseforge API
+
+[cfapi]: https://wow.curseforge.com/api
+[cfapi-docs]: https://wow.curseforge.com/api/docs
+[not-working-cfapi]: https://github.com/Owen-Cochell/cursepy
+[cmpdl]: https://github.com/Advik-B/CMPDL
+
+This is a no-compromise CurseForge API wrapper for python. It is a re-write of [cursepy][not-working-cfapi] which is maintained but not actively developed.
+This project is a complete re-write of the original project, with a focus on simplicity and ease of use.
+
+This project is still in development, and is not yet ready for production use.
+It also speeds up the process by using disk caching, It will cache the response from the API and will only make a new request if the request is not cached.
+
+This, of course can be disabled by setting the cache to False.
+
+## Features
+
+- Simple and easy to use
+- Caches responses from the API to disk for faster response times
+- Allows direct access to the API via the `fetch` method
+- Allows exporting of the objects to DICT, JSON, or YAML
+- Can directly parse a manifest file from a curseforge modpack
+
+## Installation
+
+```bash
+pip install curseforge
+```
+
+## Usage
+
+```python
+from curseforge import CurseClient
+
+client = CurseClient("API-KEY", cache=True)
+
+minecraft = client.game(432) # 432 is the ID of Minecraft
+
+# or we can list all the games
+games = client.games()
+
+for game in games:
+    print(game.name)
+
+# The search is up to the user to implement, this is just a wrapper
+
+# We can also get the latest files for a project
+
+JourneyMap = client.mod(2238) # 2238 is the ID of JourneyMap
+
+for file in JourneyMap.files:
+    print(file.name)
+```
+
+## TODO
+
+- [x] Implement the export methods
+- [x] Implement the cache
+- [x] Implement the fetch method
+- [x] Deal with the download URL being a null value
+- [ ] Implement the search method
+- [ ] Wrap the ENTIRE API
+- [x] Rename the classes so they have a `Curse` prefix
+
+## Contributing
+
+Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
+
+Please make sure to update tests as appropriate.
+
+## License
+
+[MIT](https://choosealicense.com/licenses/mit/)
```

### Comparing `curseforge-1.6.0/curseforge.egg-info/SOURCES.txt` & `curseforge-1.6.1/curseforge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

