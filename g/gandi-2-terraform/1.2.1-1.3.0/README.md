# Comparing `tmp/gandi_2_terraform-1.2.1.tar.gz` & `tmp/gandi_2_terraform-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gandi_2_terraform-1.2.1.tar", max compression
+gzip compressed data, was "gandi_2_terraform-1.3.0.tar", max compression
```

## Comparing `gandi_2_terraform-1.2.1.tar` & `gandi_2_terraform-1.3.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1078 2023-10-02 19:00:54.809534 gandi_2_terraform-1.2.1/LICENSE
--rw-r--r--   0        0        0     3538 2023-10-02 19:00:54.809534 gandi_2_terraform-1.2.1/README.md
--rw-r--r--   0        0        0      168 2023-10-02 19:00:54.809534 gandi_2_terraform-1.2.1/gandi_tf/__init__.py
--rw-r--r--   0        0        0     6367 2023-10-02 19:00:54.809534 gandi_2_terraform-1.2.1/gandi_tf/main.py
--rw-r--r--   0        0        0     1572 2023-10-02 19:00:54.809534 gandi_2_terraform-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     4528 1970-01-01 00:00:00.000000 gandi_2_terraform-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-04-12 22:04:29.955474 gandi_2_terraform-1.3.0/LICENSE
+-rw-r--r--   0        0        0     3538 2024-04-12 22:04:29.955474 gandi_2_terraform-1.3.0/README.md
+-rw-r--r--   0        0        0      169 2024-04-12 22:04:29.955474 gandi_2_terraform-1.3.0/gandi_tf/__init__.py
+-rw-r--r--   0        0        0     6559 2024-04-12 22:04:29.955474 gandi_2_terraform-1.3.0/gandi_tf/main.py
+-rw-r--r--   0        0        0     1704 2024-04-12 22:04:29.955474 gandi_2_terraform-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4673 1970-01-01 00:00:00.000000 gandi_2_terraform-1.3.0/PKG-INFO
```

### Comparing `gandi_2_terraform-1.2.1/README.md` & `gandi_2_terraform-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `gandi_2_terraform-1.2.1/gandi_tf/main.py` & `gandi_2_terraform-1.3.0/gandi_tf/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Main module for the CLI."""
+
 import os
 
 import click
 import requests
 
 
 # pylint: disable = too-few-public-methods
@@ -20,18 +21,15 @@
 
 def fetch_records(domain):
     """
     Fetch DNS records for a given domain name.
     """
     req = requests.get(
         f"https://dns.api.gandi.net/api/v5/domains/{domain}/records",
-        headers={
-            "X-Api-Key": os.getenv("GANDI_KEY"),
-            "Accept": "text/plain",
-        },
+        headers={**{"Accept": "text/plain"}, **get_authentication_header()},
         timeout=5,
     )
     req.raise_for_status()
     return req.text
 
 
 def fetch_domains_list(organization_id):
@@ -42,37 +40,46 @@
     payload = {"per_page": 1, "sort_by": "fqdn", "nameserver": "livedns"}
     if organization_id is not None:
         payload["sharing_id"] = organization_id
 
     # Get total count of domain to fetch them all in one request
     fake_head = requests.get(
         "https://api.gandi.net/v5/domain/domains",
-        headers={"authorization": f'Apikey {os.getenv("GANDI_KEY")}'},
+        headers=get_authentication_header(),
         params=payload,
         timeout=5,
     )
     fake_head.raise_for_status()
 
     try:
         total_count = int(fake_head.headers.get("total-count", 0))
     except ValueError:
         total_count = 0
     if total_count > 0:
         payload["per_page"] = total_count
 
     req = requests.get(
         "https://api.gandi.net/v5/domain/domains",
-        headers={"authorization": f'Apikey {os.getenv("GANDI_KEY")}'},
+        headers=get_authentication_header(),
         params=payload,
         timeout=5,
     )
     req.raise_for_status()
     return req.json()
 
 
+def get_authentication_header():
+    """
+    Returns the correct authentication header based on the GANDI_KEY environment variable.
+    """
+    key = os.getenv("GANDI_KEY", "")
+    header = "Apikey" if len(key) < 25 else "Bearer"
+    return {"Authorization": f"{header} {key}"}
+
+
 def parse_content(content):
     """
     Parser for the API response to return a list of Record objects."""
     entries = {}
     for line in content.splitlines():
         words = line.strip().split(" ", maxsplit=4)
         r_name = words[0]
```

### Comparing `gandi_2_terraform-1.2.1/pyproject.toml` & `gandi_2_terraform-1.3.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,64 +1,65 @@
 [tool.poetry]
 name = "gandi-2-terraform"
-version = "1.2.1"
+version = "1.3.0"
 description = "CLI to read Gandi.net live DNS records and generate corresponding TF gandi_livedns_record resources"
 readme = 'README.md'
-license = "MIT"
+license = "AGPL"
 authors = ["Marc-Aurèle Brothier <m@brothier.org>"]
 packages = [
   { include = "gandi_tf" },
 ]
 repository = "https://github.com/marcaurele/gandi-2-terraform"
 homepage = "https://github.com/marcaurele/gandi-2-terraform"
 keywords = ['gandi', 'terraform', 'DNS']
 classifiers = [
   "Topic :: Internet :: Name Service (DNS)",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
-  "License :: OSI Approved :: MIT License"
+  "Programming Language :: Python :: 3.12",
+  "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)"
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 requests = "^2.27.1"
 click = "^8.0.3"
 
 [tool.poetry.scripts]
 gandi2tf = "gandi_tf.main:generate"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/marcaurele/gandi-2-terraform/issues"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.2.2"
-black = "^23.3.0"
+pytest = ">=7.2.2,<9.0.0"
+black = ">=23.3,<25.0"
 flake8-import-order = "^0.18.2"
-pylint = "^2.17.1"
+pylint = ">=2.17.1,<4.0.0"
 mypy = "^1.1.1"
-ruff = "^0.0.291"
+ruff = ">=0.0.291,<0.3.5"
 
 [tool.black]
-target-version = ["py38", "py39", "py310", "py311"]
+target-version = ["py38", "py39", "py310", "py311", "py312"]
 line-length = 119
 
 [tool.pylint]
 max-line-length = 119
 
 [tool.isort]
 line_length = 119
 
 [tool.mypy]
 non_interactive = true
 install_types = true
 
 [tool.ruff]
-select = ["E", "F"]
+lint.select = ["E", "F"]
 line-length = 119
 target-version = "py38"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `gandi_2_terraform-1.2.1/PKG-INFO` & `gandi_2_terraform-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: gandi-2-terraform
-Version: 1.2.1
+Version: 1.3.0
 Summary: CLI to read Gandi.net live DNS records and generate corresponding TF gandi_livedns_record resources
 Home-page: https://github.com/marcaurele/gandi-2-terraform
-License: MIT
+License: AGPL
 Keywords: gandi,terraform,DNS
 Author: Marc-Aurèle Brothier
 Author-email: m@brothier.org
 Requires-Python: >=3.8.1,<4.0
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
+Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Internet :: Name Service (DNS)
 Requires-Dist: click (>=8.0.3,<9.0.0)
 Requires-Dist: requests (>=2.27.1,<3.0.0)
 Project-URL: Bug Tracker, https://github.com/marcaurele/gandi-2-terraform/issues
 Project-URL: Repository, https://github.com/marcaurele/gandi-2-terraform
 Description-Content-Type: text/markdown
```

