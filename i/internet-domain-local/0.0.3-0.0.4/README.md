# Comparing `tmp/internet-domain-local-0.0.3.tar.gz` & `tmp/internet_domain_local-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "internet-domain-local-0.0.3.tar", last modified: Sun Feb 11 16:11:00 2024, max compression
+gzip compressed data, was "internet_domain_local-0.0.4.tar", last modified: Sat Apr 13 19:11:14 2024, max compression
```

## Comparing `internet-domain-local-0.0.3.tar` & `internet_domain_local-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:11:00.822442 internet-domain-local-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-02-11 16:11:00.822442 internet-domain-local-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-11 16:10:33.000000 internet-domain-local-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:11:00.818442 internet-domain-local-0.0.3/internet_domain_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:11:00.822442 internet-domain-local-0.0.3/internet_domain_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-11 16:10:33.000000 internet-domain-local-0.0.3/internet_domain_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7581 2024-02-11 16:10:33.000000 internet-domain-local-0.0.3/internet_domain_local/src/internet_domain_local.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-02-11 16:10:33.000000 internet-domain-local-0.0.3/internet_domain_local/src/internet_domain_local_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:11:00.822442 internet-domain-local-0.0.3/internet_domain_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-02-11 16:11:00.000000 internet-domain-local-0.0.3/internet_domain_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-02-11 16:11:00.000000 internet-domain-local-0.0.3/internet_domain_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-11 16:11:00.000000 internet-domain-local-0.0.3/internet_domain_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-02-11 16:11:00.000000 internet-domain-local-0.0.3/internet_domain_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-11 16:11:00.000000 internet-domain-local-0.0.3/internet_domain_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-02-11 16:10:33.000000 internet-domain-local-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-11 16:11:00.822442 internet-domain-local-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-02-11 16:10:33.000000 internet-domain-local-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:11:14.191152 internet_domain_local-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-13 19:11:14.191152 internet_domain_local-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-13 19:10:43.000000 internet_domain_local-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:11:14.187152 internet_domain_local-0.0.4/internet_domain_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:11:14.191152 internet_domain_local-0.0.4/internet_domain_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 19:10:43.000000 internet_domain_local-0.0.4/internet_domain_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8543 2024-04-13 19:10:43.000000 internet_domain_local-0.0.4/internet_domain_local/src/internet_domain_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-13 19:10:43.000000 internet_domain_local-0.0.4/internet_domain_local/src/internet_domain_local_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:11:14.191152 internet_domain_local-0.0.4/internet_domain_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-13 19:11:14.000000 internet_domain_local-0.0.4/internet_domain_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-13 19:11:14.000000 internet_domain_local-0.0.4/internet_domain_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 19:11:14.000000 internet_domain_local-0.0.4/internet_domain_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-13 19:11:14.000000 internet_domain_local-0.0.4/internet_domain_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-13 19:11:14.000000 internet_domain_local-0.0.4/internet_domain_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-13 19:10:43.000000 internet_domain_local-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 19:11:14.191152 internet_domain_local-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-13 19:10:43.000000 internet_domain_local-0.0.4/setup.py
```

### Comparing `internet-domain-local-0.0.3/PKG-INFO` & `internet_domain_local-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: internet-domain-local
-Version: 0.0.3
+Version: 0.0.4
 Summary: PyPI Package for Circles internet-domain-local Python
 Home-page: https://github.com/circles-zone/internet-domain-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `internet-domain-local-0.0.3/internet_domain_local/src/internet_domain_local.py` & `internet_domain_local-0.0.4/internet_domain_local/src/internet_domain_local.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,15 +39,14 @@
         self.tld_regex = re.compile(r'^(?:http[s]?://)?(?:www\.)?[^\.]+\.(.*?)(?:/|$)')
 
         GenericMapping.__init__(self, default_schema_name=default_schema_name,
                                 default_table_name=default_table_name, default_view_table_name=default_view_table_name,
                                 default_id_column_name=default_id_column_name, default_entity_name1=default_entity_name1,
                                 default_entity_name2=default_entity_name2, is_test_data=is_test_data)
 
-
     def get_domain_name(self, url: str) -> Optional[str]:
         """
         Extracts the domain name from a URL.
         """
         if not self.valid_url(url):
             return None
         match = self.domain_regex.search(url)
@@ -88,15 +87,15 @@
             return match.group(1)
         return None
 
     def valid_url(self, url: str) -> bool:
         """
         Validates the URL format.
         """
-        return re.match(r'^http[s]?://', url) is not None
+        return re.match(r'^(http[s]?://|www\.)', url) is not None
 
     def is_commercial_domain(self, url: str) -> bool:
         """
         Checks if the domain of a URL is a commercial domain (.com).
         """
         tld = self.get_tld(url)
         return tld == 'com'
@@ -138,28 +137,52 @@
             if internet_domain_id:
                 internet_domain_id = internet_domain_id[0]
             else:
                 internet_domain_id = self.insert(
                     table_name='internet_domain_table', data_json=data_to_insert, ignore_duplicate=True)
             self.set_schema(schema_name='contact_internet_domain')
             # link the contact to the domain
-            contact_internet_domain_id = self.insert_mapping(
-                entity_id1=contact_id, entity_id2=internet_domain_id,
-                ignore_duplicate=True
+            # check if the mapping already exists
+            contact_internet_domain_id = self.select_one_value_by_where(
+                select_clause_value='contact_internet_domain_id',
+                view_table_name='contact_internet_domain_view',
+                where="contact_id = %s AND internet_domain_id = %s",
+                params=(contact_id, internet_domain_id)
+            )
+            if contact_internet_domain_id is None:
+                contact_internet_domain_id = self.insert_mapping(
+                    entity_id1=contact_id, entity_id2=internet_domain_id,
+                    ignore_duplicate=True
+                )
+            # Add url to url_table
+            # TODO: add url type
+            data_json = {
+                'url': url
+            }
+            data_json_compare = {
+                'url': url
+            }
+            url_id = self.upsert(
+                schema_name='url',
+                table_name='url_table',
+                view_table_name='url_view',
+                data_json=data_json,
+                data_json_compare=data_json_compare
             )
         except Exception as e:
             logger.error("link_contact_to_domain", object={
                          'contact_id': contact_id, 'url': url}, data=e)
             raise e
         insert_information = {
             'contact_id': contact_id,
             'url': url,
             'profile_id': logger.user_context.get_effective_profile_id(),
             'internet_domain_id': internet_domain_id,
-            'contact_internet_domain_id': contact_internet_domain_id
+            'contact_internet_domain_id': contact_internet_domain_id,
+            'url_id': url_id
         }
         logger.end("link_contact_to_domain", object={
                    'contact_internet_domain_id': contact_internet_domain_id})
         return insert_information
 
     def is_email_assign_profile_organization_to_people(self, domain: str) -> bool:
         logger.start()
```

### Comparing `internet-domain-local-0.0.3/internet_domain_local/src/internet_domain_local_constants.py` & `internet_domain_local-0.0.4/internet_domain_local/src/internet_domain_local_constants.py`

 * *Files identical despite different names*

### Comparing `internet-domain-local-0.0.3/internet_domain_local.egg-info/PKG-INFO` & `internet_domain_local-0.0.4/internet_domain_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: internet-domain-local
-Version: 0.0.3
+Version: 0.0.4
 Summary: PyPI Package for Circles internet-domain-local Python
 Home-page: https://github.com/circles-zone/internet-domain-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `internet-domain-local-0.0.3/setup.py` & `internet_domain_local-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PACKAGE_NAME = "internet-domain-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.3',  # update only the minor version each time # https://pypi.org/project/internet-domain-local/
+    version='0.0.4',  # update only the minor version each time # https://pypi.org/project/internet-domain-local/
     author="Circles",
     author_email="info@circlez.ai",
     description="PyPI Package for Circles internet-domain-local Python",
     long_description="PyPI Package for Circles internet-domain-local Python",
     long_description_content_type='text/markdown',
     url="https://github.com/circles-zone/internet-domain-local-python-package",
     packages=[package_dir],
```

