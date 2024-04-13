# Comparing `tmp/apache_airflow_providers_slack-8.6.2.tar.gz` & `tmp/apache_airflow_providers_slack-8.6.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_slack-8.6.2.tar", last modified: Tue Apr  9 12:41:24 2024, max compression
+gzip compressed data, was "apache_airflow_providers_slack-8.6.2rc1.tar", last modified: Tue Apr  9 12:41:24 2024, max compression
```

## Comparing `apache_airflow_providers_slack-8.6.2.tar` & `apache_airflow_providers_slack-8.6.2rc1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     4397 2024-04-09 12:41:24.000000 apache_airflow_providers_slack-8.6.2/README.rst
--rw-r--r--   0        0        0    13569 2024-04-09 12:41:24.000000 apache_airflow_providers_slack-8.6.2/airflow/providers/slack/LICENSE
--rw-r--r--   0        0        0     1580 2024-04-09 12:41:24.000000 apache_airflow_providers_slack-8.6.2/airflow/providers/slack/__init__.py
--rw-r--r--   0        0        0     5361 2024-04-09 12:41:24.000000 apache_airflow_providers_slack-8.6.2/airflow/providers/slack/get_provider_info.py
--rw-r--r--   0        0        0      787 2024-04-09 12:41:24.000000 apache_airflow_providers_slack-8.6.2/airflow/providers/slack/hooks/__init__.py
--rw-r--r--   0        0        0    17643 2024-04-09 12:41:24.000000 apache_airflow_providers_slack-8.6.2/airflow/providers/slack/hooks/slack.py
--rw-r--r--   0        0        0    12938 2024-04-09 12:41:24.000000 apache_airflow_providers_slack-8.6.2/airflow/providers/slack/hooks/slack_webhook.py
--rw-r--r--   0        0        0      785 2024-04-09 12:41:24.000000 apache_airflow_providers_slack-8.6.2/airflow/providers/slack/notifications/__init__.py
--rw-r--r--   0        0        0     3891 2024-04-09 12:41:24.000000 apache_airflow_providers_slack-8.6.2/airflow/providers/slack/notifications/slack.py
--rw-r--r--   0        0        0     1250 2024-04-09 12:41:24.000000 apache_airflow_providers_slack-8.6.2/airflow/providers/slack/notifications/slack_notifier.py
--rw-r--r--   0        0        0     3844 2024-04-09 12:41:24.000000 apache_airflow_providers_slack-8.6.2/airflow/providers/slack/notifications/slack_webhook.py
--rw-r--r--   0        0        0      787 2024-04-09 12:41:24.000000 apache_airflow_providers_slack-8.6.2/airflow/providers/slack/operators/__init__.py
--rw-r--r--   0        0        0     9784 2024-04-09 12:41:24.000000 apache_airflow_providers_slack-8.6.2/airflow/providers/slack/operators/slack.py
--rw-r--r--   0        0        0     5012 2024-04-09 12:41:24.000000 apache_airflow_providers_slack-8.6.2/airflow/providers/slack/operators/slack_webhook.py
--rw-r--r--   0        0        0      785 2024-04-09 12:41:24.000000 apache_airflow_providers_slack-8.6.2/airflow/providers/slack/transfers/__init__.py
--rw-r--r--   0        0        0     3308 2024-04-09 12:41:24.000000 apache_airflow_providers_slack-8.6.2/airflow/providers/slack/transfers/base_sql_to_slack.py
--rw-r--r--   0        0        0     8623 2024-04-09 12:41:24.000000 apache_airflow_providers_slack-8.6.2/airflow/providers/slack/transfers/sql_to_slack.py
--rw-r--r--   0        0        0     8156 2024-04-09 12:41:24.000000 apache_airflow_providers_slack-8.6.2/airflow/providers/slack/transfers/sql_to_slack_webhook.py
--rw-r--r--   0        0        0     5200 2024-04-09 12:41:24.000000 apache_airflow_providers_slack-8.6.2/airflow/providers/slack/utils/__init__.py
--rw-r--r--   0        0        0     3096 2024-04-09 12:41:24.000000 apache_airflow_providers_slack-8.6.2/pyproject.toml
--rw-r--r--   0        0        0     6239 1970-01-01 00:00:00.000000 apache_airflow_providers_slack-8.6.2/PKG-INFO
+-rw-r--r--   0        0        0     4401 2024-04-09 12:41:24.000000 apache_airflow_providers_slack-8.6.2rc1/README.rst
+-rw-r--r--   0        0        0    13569 2024-04-09 12:41:24.000000 apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/LICENSE
+-rw-r--r--   0        0        0     1580 2024-04-09 12:41:24.000000 apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/__init__.py
+-rw-r--r--   0        0        0     5361 2024-04-09 12:41:24.000000 apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/get_provider_info.py
+-rw-r--r--   0        0        0      787 2024-04-09 12:41:24.000000 apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/hooks/__init__.py
+-rw-r--r--   0        0        0    17643 2024-04-09 12:41:24.000000 apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/hooks/slack.py
+-rw-r--r--   0        0        0    12938 2024-04-09 12:41:24.000000 apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/hooks/slack_webhook.py
+-rw-r--r--   0        0        0      785 2024-04-09 12:41:24.000000 apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/notifications/__init__.py
+-rw-r--r--   0        0        0     3891 2024-04-09 12:41:24.000000 apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/notifications/slack.py
+-rw-r--r--   0        0        0     1250 2024-04-09 12:41:24.000000 apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/notifications/slack_notifier.py
+-rw-r--r--   0        0        0     3844 2024-04-09 12:41:24.000000 apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/notifications/slack_webhook.py
+-rw-r--r--   0        0        0      787 2024-04-09 12:41:24.000000 apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/operators/__init__.py
+-rw-r--r--   0        0        0     9784 2024-04-09 12:41:24.000000 apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/operators/slack.py
+-rw-r--r--   0        0        0     5012 2024-04-09 12:41:24.000000 apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/operators/slack_webhook.py
+-rw-r--r--   0        0        0      785 2024-04-09 12:41:24.000000 apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/transfers/__init__.py
+-rw-r--r--   0        0        0     3308 2024-04-09 12:41:24.000000 apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/transfers/base_sql_to_slack.py
+-rw-r--r--   0        0        0     8623 2024-04-09 12:41:24.000000 apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/transfers/sql_to_slack.py
+-rw-r--r--   0        0        0     8156 2024-04-09 12:41:24.000000 apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/transfers/sql_to_slack_webhook.py
+-rw-r--r--   0        0        0     5200 2024-04-09 12:41:24.000000 apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/utils/__init__.py
+-rw-r--r--   0        0        0     3106 2024-04-09 12:41:24.000000 apache_airflow_providers_slack-8.6.2rc1/pyproject.toml
+-rw-r--r--   0        0        0     6252 1970-01-01 00:00:00.000000 apache_airflow_providers_slack-8.6.2rc1/PKG-INFO
```

### Comparing `apache_airflow_providers_slack-8.6.2/README.rst` & `apache_airflow_providers_slack-8.6.2rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-slack``
 
-Release: ``8.6.2``
+Release: ``8.6.2.rc1``
 
 
 `Slack <https://slack.com/>`__ services integration including:
 
   - `Slack API <https://api.slack.com/>`__
   - `Slack Incoming Webhook <https://api.slack.com/messaging/webhooks>`__
```

### Comparing `apache_airflow_providers_slack-8.6.2/airflow/providers/slack/LICENSE` & `apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_slack-8.6.2/airflow/providers/slack/__init__.py` & `apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_slack-8.6.2/airflow/providers/slack/get_provider_info.py` & `apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_slack-8.6.2/airflow/providers/slack/hooks/__init__.py` & `apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_slack-8.6.2/airflow/providers/slack/hooks/slack.py` & `apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/hooks/slack.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_slack-8.6.2/airflow/providers/slack/hooks/slack_webhook.py` & `apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/hooks/slack_webhook.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_slack-8.6.2/airflow/providers/slack/notifications/__init__.py` & `apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_slack-8.6.2/airflow/providers/slack/notifications/slack.py` & `apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/notifications/slack.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_slack-8.6.2/airflow/providers/slack/notifications/slack_notifier.py` & `apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/notifications/slack_notifier.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_slack-8.6.2/airflow/providers/slack/notifications/slack_webhook.py` & `apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/notifications/slack_webhook.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_slack-8.6.2/airflow/providers/slack/operators/__init__.py` & `apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_slack-8.6.2/airflow/providers/slack/operators/slack.py` & `apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/operators/slack.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_slack-8.6.2/airflow/providers/slack/operators/slack_webhook.py` & `apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/operators/slack_webhook.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_slack-8.6.2/airflow/providers/slack/transfers/__init__.py` & `apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_slack-8.6.2/airflow/providers/slack/transfers/base_sql_to_slack.py` & `apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/transfers/base_sql_to_slack.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_slack-8.6.2/airflow/providers/slack/transfers/sql_to_slack.py` & `apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/transfers/sql_to_slack.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_slack-8.6.2/airflow/providers/slack/transfers/sql_to_slack_webhook.py` & `apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/transfers/sql_to_slack_webhook.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_slack-8.6.2/airflow/providers/slack/utils/__init__.py` & `apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_slack-8.6.2/pyproject.toml` & `apache_airflow_providers_slack-8.6.2rc1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-slack"
-version = "8.6.2"
+version = "8.6.2.rc1"
 description = "Provider package apache-airflow-providers-slack for Apache Airflow"
 readme = "README.rst"
 authors = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
 ]
 maintainers = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
@@ -52,16 +52,16 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: System :: Monitoring",
 ]
 requires-python = "~=3.8"
 dependencies = [
-    "apache-airflow-providers-common-sql>=1.3.1",
-    "apache-airflow>=2.6.0",
+    "apache-airflow-providers-common-sql>=1.3.1rc0",
+    "apache-airflow>=2.6.0rc0",
     "slack_sdk>=3.19.0",
 ]
 
 [project.urls]
 "Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-slack/8.6.2"
 "Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-slack/8.6.2/changelog.html"
 "Bug Tracker" = "https://github.com/apache/airflow/issues"
```

### Comparing `apache_airflow_providers_slack-8.6.2/PKG-INFO` & `apache_airflow_providers_slack-8.6.2rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-slack
-Version: 8.6.2
+Version: 8.6.2rc1
 Summary: Provider package apache-airflow-providers-slack for Apache Airflow
 Keywords: airflow-provider,slack,airflow,integration
 Author-email: Apache Software Foundation <dev@airflow.apache.org>
 Maintainer-email: Apache Software Foundation <dev@airflow.apache.org>
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,16 +17,16 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Monitoring
-Requires-Dist: apache-airflow-providers-common-sql>=1.3.1
-Requires-Dist: apache-airflow>=2.6.0
+Requires-Dist: apache-airflow-providers-common-sql>=1.3.1rc0
+Requires-Dist: apache-airflow>=2.6.0rc0
 Requires-Dist: slack_sdk>=3.19.0
 Requires-Dist: apache-airflow-providers-common-sql ; extra == "common.sql"
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-slack/8.6.2/changelog.html
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-slack/8.6.2
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
@@ -74,15 +74,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-slack``
 
-Release: ``8.6.2``
+Release: ``8.6.2.rc1``
 
 
 `Slack <https://slack.com/>`__ services integration including:
 
   - `Slack API <https://api.slack.com/>`__
   - `Slack Incoming Webhook <https://api.slack.com/messaging/webhooks>`__
```

