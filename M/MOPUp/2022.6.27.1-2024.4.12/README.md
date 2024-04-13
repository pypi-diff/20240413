# Comparing `tmp/MOPUp-2022.6.27.1.tar.gz` & `tmp/mopup-2024.4.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MOPUp-2022.6.27.1.tar", max compression
+gzip compressed data, was "mopup-2024.4.12.tar", max compression
```

## Comparing `MOPUp-2022.6.27.1.tar` & `mopup-2024.4.12.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1087 2022-05-05 21:22:41.894459 MOPUp-2022.6.27.1/LICENSE.rst
--rw-r--r--   0        0        0     3097 2022-06-28 00:34:32.769777 MOPUp-2022.6.27.1/README.rst
--rw-r--r--   0        0        0     1805 2022-06-28 00:30:19.788816 MOPUp-2022.6.27.1/pyproject.toml
--rw-r--r--   0        0        0     4509 2022-06-27 23:58:47.041851 MOPUp-2022.6.27.1/src/mopup/__init__.py
--rw-r--r--   0        0        0      738 2022-06-27 23:52:33.579607 MOPUp-2022.6.27.1/src/mopup/__main__.py
--rw-r--r--   0        0        0        0 2022-05-05 21:22:41.923729 MOPUp-2022.6.27.1/src/mopup/py.typed
--rw-r--r--   0        0        0     4054 2022-06-28 00:35:16.184233 MOPUp-2022.6.27.1/setup.py
--rw-r--r--   0        0        0     4025 2022-06-28 00:35:16.184396 MOPUp-2022.6.27.1/PKG-INFO
+-rw-r--r--   0        0        0     1087 2022-05-05 21:22:41.894459 mopup-2024.4.12/LICENSE.rst
+-rw-r--r--   0        0        0     3097 2022-10-26 00:48:06.745505 mopup-2024.4.12/README.rst
+-rw-r--r--   0        0        0     1855 2024-04-13 05:34:42.734220 mopup-2024.4.12/pyproject.toml
+-rw-r--r--   0        0        0     5337 2024-04-11 06:12:47.870641 mopup-2024.4.12/src/mopup/__init__.py
+-rw-r--r--   0        0        0     1074 2022-10-26 04:14:06.449904 mopup-2024.4.12/src/mopup/__main__.py
+-rw-r--r--   0        0        0        0 2022-05-05 21:22:41.923729 mopup-2024.4.12/src/mopup/py.typed
+-rw-r--r--   0        0        0     4209 1970-01-01 00:00:00.000000 mopup-2024.4.12/PKG-INFO
```

### Comparing `MOPUp-2022.6.27.1/LICENSE.rst` & `mopup-2024.4.12/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `MOPUp-2022.6.27.1/README.rst` & `mopup-2024.4.12/README.rst`

 * *Files identical despite different names*

### Comparing `MOPUp-2022.6.27.1/pyproject.toml` & `mopup-2024.4.12/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "MOPUp"
-version = "2022.6.27.1"
+version = "2024.04.12"
 description = "MOPUp"
 authors = ["Glyph Lefkowitz <glyph@glyph.im>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/glyph/MOPUp"
 repository = "https://github.com/glyph/MOPUp"
 documentation = "https://MOPUp.readthedocs.io"
@@ -20,15 +20,17 @@
 
 [tool.poetry.dependencies]
 python = ">=3.7,<4.0"
 click = ">=8.0.1"
 html5lib = ">=1.1"
 requests = ">=2.27.1"
 hyperlink = "*"
-rich = "^12.4.4"
+rich = ">=12.4.4,<14.0.0"
+types-click = "^7.1.8"
+packaging = "^24.0"
 
 [tool.poetry.dev-dependencies]
 pytest = ">=6.2.5"
 coverage = {extras = ["toml"], version = ">=6.1"}
 safety = ">=1.10.3"
 mypy = ">=0.910"
 typeguard = ">=2.13.2"
@@ -62,15 +64,15 @@
 
 [tool.coverage.run]
 branch = true
 source = ["mopup", "tests"]
 
 [tool.coverage.report]
 show_missing = true
-fail_under = 100
+fail_under = 50
 
 [tool.mypy]
 strict = true
 warn_unreachable = true
 show_column_numbers = true
 show_error_codes = true
 show_error_context = true
```

### Comparing `MOPUp-2022.6.27.1/src/mopup/__init__.py` & `mopup-2024.4.12/src/mopup/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,90 +1,109 @@
 """Auto-updater for official python.org builds of python."""
 import collections
-from os import makedirs
-from os import rename
-from os import rmdir
-from os import unlink
+from os import makedirs, rename, rmdir, unlink
 from os.path import expanduser
 from os.path import join as pathjoin
 from platform import mac_ver
 from re import compile as compile_re
 from subprocess import run  # noqa: S404
 from sys import version_info
-from typing import Dict
-from typing import Iterable
-from typing import Match
-from typing import Pattern
-from typing import Tuple
+from typing import Dict, Iterable, List, Match, Pattern, Tuple
 from uuid import uuid4
 
 import html5lib
 import requests
 from hyperlink import DecodedURL
+from packaging.version import Version, parse
 from rich.progress import Progress
 
 
 def alllinksin(
     u: DecodedURL, e: Pattern[str]
 ) -> Iterable[Tuple[Match[str], DecodedURL]]:
     """Get all the links in the given URL whose text matches the given pattern."""
     for a in html5lib.parse(
-        requests.get(u.to_text()).text, namespaceHTMLElements=False
+        requests.get(u.to_text(), timeout=30).text, namespaceHTMLElements=False
     ).findall(".//a"):
         match = e.fullmatch(a.text or "")
         if match is not None:
             yield match, u.click(a.attrib["href"])
 
 
-def main(interactive: bool, force: bool) -> None:
+def main(interactive: bool, force: bool, minor_upgrade: bool, dry_run: bool) -> None:
     """Do an update."""
     this_mac_ver = tuple(map(int, mac_ver()[0].split(".")[:2]))
     ver = compile_re(r"(\d+)\.(\d+).(\d+)/")
     macpkg = compile_re("python-(.+)-macosx?(.*).pkg")
 
-    thismajor, thisminor, thismicro, *other = version_info
+    thismajor, thisminor, thismicro, level, serial = version_info
 
-    # major, minor, micro, macos
+    thispkgver = Version(
+        f"{thismajor}.{thisminor}.{thismicro}"
+        + (f".{level}{serial}" if level != "final" else "")
+    )
+
+    # {macos, major, minor: [(Version, URL)]}
+    # major, minor, micro, macos: [(version, URL)]
     versions: Dict[
-        int, Dict[int, Dict[int, Dict[str, DecodedURL]]]
+        int, Dict[int, Dict[int, Dict[str, List[Tuple[Version, DecodedURL]]]]]
     ] = collections.defaultdict(
-        lambda: collections.defaultdict(lambda: collections.defaultdict(dict))
+        lambda: collections.defaultdict(
+            lambda: collections.defaultdict(lambda: collections.defaultdict(list))
+        )
     )
 
     baseurl = DecodedURL.from_text("https://www.python.org/ftp/python/")
 
     for eachver, suburl in alllinksin(baseurl, ver):
         major, minor, micro = map(int, eachver.groups())
         if major != thismajor:
             continue
-        if minor != thisminor:
+        if minor != thisminor and not minor_upgrade:
             continue
         for eachmac, pkgdl in alllinksin(suburl, macpkg):
             pyver, macver = eachmac.groups()
-            if pyver == f"{major}.{minor}.{micro}":
-                versions[major][minor][micro][macver] = pkgdl
-
-    newmicro = max(versions[thismajor][thisminor].keys())
-    available_mac_vers = versions[thismajor][thisminor][newmicro].keys()
+            fullversion = parse(pyver)
+            if fullversion.pre and not thispkgver.pre:
+                continue
+            if (
+                fullversion.major,
+                fullversion.minor,
+                fullversion.micro,
+            ) == (
+                major,
+                minor,
+                micro,
+            ):
+                versions[major][minor][micro][macver].append((fullversion, pkgdl))
+
+    newminor = max(versions[thismajor].keys())
+    newmicro = max(versions[thismajor][newminor].keys())
+    available_mac_vers = versions[thismajor][newminor][newmicro].keys()
     best_available_mac = max(
         available_mac_ver
         for available_mac_ver in available_mac_vers
         if this_mac_ver >= tuple(int(x) for x in available_mac_ver.split("."))
     )
 
-    update_needed = newmicro > thismicro
-    download_url = versions[thismajor][thisminor][newmicro][best_available_mac]
+    download_urls = versions[thismajor][newminor][newmicro][best_available_mac]
+
+    best_ver, download_url = sorted(download_urls, reverse=True)[0]
+
+    print(f"this version: {thispkgver}; new version: {best_ver}")
+    update_needed = best_ver > thispkgver
+
     print(
         "update",
         "needed" if update_needed else "not needed",
         "from",
         download_url,
     )
 
-    if not (update_needed or force):
+    if dry_run or not (update_needed or force):
         return
 
     finalname = do_download(download_url)
     if interactive:
         argv = ["/usr/bin/open", "-b", "com.apple.installer", finalname]
     else:
         print("Enter your administrative password to run the update:")
@@ -109,15 +128,17 @@
     basename = download_url.path[-1]
     partial = basename + ".mopup-partial"
     downloads_dir = expanduser("~/Downloads/")
     partialdir = pathjoin(downloads_dir, partial)
     contentname = pathjoin(partialdir, f"{uuid4()}.content")
     finalname = pathjoin(downloads_dir, basename)
 
-    with requests.get(download_url.to_uri().to_text(), stream=True) as response:
+    with requests.get(
+        download_url.to_uri().to_text(), stream=True, timeout=30
+    ) as response:
         response.raise_for_status()
         try:
             makedirs(partialdir, exist_ok=True)
             total_size = int(response.headers["content-length"])
             with open(contentname, "wb") as f:
                 with Progress() as progress:
                     task = progress.add_task(
```

### Comparing `MOPUp-2022.6.27.1/src/mopup/__main__.py` & `mopup-2024.4.12/src/mopup/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,14 +13,24 @@
          version.
          """
 )
 @click.option("--interactive", default=False, help="use the installer GUI", type=bool)
 @click.option(
     "--force", default=False, help="reinstall python even if it's up to date", type=bool
 )
-def main(interactive: bool, force: bool) -> None:
+@click.option(
+    "--minor",
+    default=False,
+    help="do a minor version upgrade rather than the default (a micro-version)",
+)
+@click.option(
+    "--dry-run",
+    default=False,
+    help="don't actually download or install anything even if we're not up to date",
+)
+def main(interactive: bool, force: bool, minor: bool, dry_run: bool) -> None:
     """MOPUp."""
-    libmain(interactive=interactive, force=force)
+    libmain(interactive=interactive, force=force, minor_upgrade=minor, dry_run=dry_run)
 
 
 if __name__ == "__main__":
     main(prog_name="mopup")  # pragma: no cover
```

### Comparing `MOPUp-2022.6.27.1/PKG-INFO` & `mopup-2024.4.12/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 Metadata-Version: 2.1
-Name: mopup
-Version: 2022.6.27.1
+Name: MOPUp
+Version: 2024.4.12
 Summary: MOPUp
 Home-page: https://github.com/glyph/MOPUp
 License: MIT
 Author: Glyph Lefkowitz
 Author-email: glyph@glyph.im
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.0.1)
 Requires-Dist: html5lib (>=1.1)
 Requires-Dist: hyperlink
+Requires-Dist: packaging (>=24.0,<25.0)
 Requires-Dist: requests (>=2.27.1)
-Requires-Dist: rich (>=12.4.4,<13.0.0)
+Requires-Dist: rich (>=12.4.4,<14.0.0)
+Requires-Dist: types-click (>=7.1.8,<8.0.0)
 Project-URL: Changelog, https://github.com/glyph/MOPUp/releases
 Project-URL: Documentation, https://MOPUp.readthedocs.io
 Project-URL: Repository, https://github.com/glyph/MOPUp
 Description-Content-Type: text/x-rst
 
 MOPUp
 =====
```

