# Comparing `tmp/iam_actions-1.2.20240411.tar.gz` & `tmp/iam_actions-1.2.20240412.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20240411.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20240412.tar", max compression
```

## Comparing `iam_actions-1.2.20240411.tar` & `iam_actions-1.2.20240412.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2024-04-11 02:17:43.686671 iam_actions-1.2.20240411/LICENSE
--rw-r--r--   0        0        0     2302 2024-04-11 02:17:43.686671 iam_actions-1.2.20240411/README.md
--rw-r--r--   0        0        0      228 2024-04-11 02:17:43.686671 iam_actions-1.2.20240411/iam_actions/__init__.py
--rw-r--r--   0        0        0  4785599 2024-04-11 02:19:34.302694 iam_actions-1.2.20240411/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2024-04-11 02:17:43.686671 iam_actions-1.2.20240411/iam_actions/data.py
--rw-r--r--   0        0        0       80 2024-04-11 02:17:43.686671 iam_actions-1.2.20240411/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2024-04-11 02:17:43.686671 iam_actions-1.2.20240411/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2024-04-11 02:17:43.686671 iam_actions-1.2.20240411/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2024-04-11 02:17:43.686671 iam_actions-1.2.20240411/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2024-04-11 02:17:43.686671 iam_actions-1.2.20240411/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2024-04-11 02:17:43.686671 iam_actions-1.2.20240411/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2024-04-11 02:17:43.686671 iam_actions-1.2.20240411/iam_actions/generate/services.py
--rw-r--r--   0        0        0   622194 2024-04-11 02:19:34.302694 iam_actions-1.2.20240411/iam_actions/policies.json
--rw-r--r--   0        0        0   207247 2024-04-11 02:19:34.302694 iam_actions-1.2.20240411/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   603630 2024-04-11 02:19:34.302694 iam_actions-1.2.20240411/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2024-04-11 02:19:34.982694 iam_actions-1.2.20240411/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20240411/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20240411/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-12 02:19:32.327636 iam_actions-1.2.20240412/LICENSE
+-rw-r--r--   0        0        0     2302 2024-04-12 02:19:32.327636 iam_actions-1.2.20240412/README.md
+-rw-r--r--   0        0        0      228 2024-04-12 02:19:32.327636 iam_actions-1.2.20240412/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4797419 2024-04-12 02:21:45.063691 iam_actions-1.2.20240412/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2024-04-12 02:19:32.327636 iam_actions-1.2.20240412/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2024-04-12 02:19:32.327636 iam_actions-1.2.20240412/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2024-04-12 02:19:32.327636 iam_actions-1.2.20240412/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2024-04-12 02:19:32.327636 iam_actions-1.2.20240412/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2024-04-12 02:19:32.327636 iam_actions-1.2.20240412/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2024-04-12 02:19:32.327636 iam_actions-1.2.20240412/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2024-04-12 02:19:32.327636 iam_actions-1.2.20240412/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2024-04-12 02:19:32.327636 iam_actions-1.2.20240412/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   623513 2024-04-12 02:21:45.063691 iam_actions-1.2.20240412/iam_actions/policies.json
+-rw-r--r--   0        0        0   208021 2024-04-12 02:21:45.063691 iam_actions-1.2.20240412/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   604906 2024-04-12 02:21:45.063691 iam_actions-1.2.20240412/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2024-04-12 02:21:45.719691 iam_actions-1.2.20240412/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20240412/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20240412/PKG-INFO
```

### Comparing `iam_actions-1.2.20240411/LICENSE` & `iam_actions-1.2.20240412/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240411/README.md` & `iam_actions-1.2.20240412/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240411/iam_actions/actions.json` & `iam_actions-1.2.20240412/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995363692220164%*

 * *Differences: {"'glue'": "{'GetExecutorsThreads': OrderedDict([('access_level', 'Undocumented'), ('action', "*

 * *           "'GetExecutorsThreads'), ('condition_keys', []), ('description', 'Not Documented by "*

 * *           "AWS'), ('orphan', False), ('resources', [])]), 'GetStageAttemptTaskList': "*

 * *           "OrderedDict([('access_level', 'Undocumented'), ('action', 'GetStageAttemptTaskList'), "*

 * *           "('condition_keys', []), ('description', 'Not Documented by AWS'), ('orphan', False), "*

 * *           "('resources', [])]), […]*

```diff
@@ -75496,14 +75496,22 @@
             "orphan": false,
             "resources": [
                 "catalog",
                 "database",
                 "table"
             ]
         },
+        "BatchGetStageFiles": {
+            "access_level": "Undocumented",
+            "action": "BatchGetStageFiles",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "BatchGetTableOptimizer": {
             "access_level": "Read",
             "action": "BatchGetTableOptimizer",
             "condition_keys": [],
             "description": "Grants permission to return the configuration for the specified table optimizers",
             "orphan": false,
             "resources": [
@@ -76412,14 +76420,38 @@
             "access_level": "Read",
             "action": "GetDevEndpoints",
             "condition_keys": [],
             "description": "Grants permission to retrieve all development endpoints",
             "orphan": false,
             "resources": []
         },
+        "GetEnvironment": {
+            "access_level": "Undocumented",
+            "action": "GetEnvironment",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetExecutors": {
+            "access_level": "Undocumented",
+            "action": "GetExecutors",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetExecutorsThreads": {
+            "access_level": "Undocumented",
+            "action": "GetExecutorsThreads",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "GetJob": {
             "access_level": "Read",
             "action": "GetJob",
             "condition_keys": [],
             "description": "Grants permission to retrieve a job",
             "orphan": false,
             "resources": [
@@ -76458,14 +76490,22 @@
             "access_level": "Read",
             "action": "GetJobs",
             "condition_keys": [],
             "description": "Grants permission to retrieve all current jobs",
             "orphan": false,
             "resources": []
         },
+        "GetLogParsingStatus": {
+            "access_level": "Undocumented",
+            "action": "GetLogParsingStatus",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "GetMLTaskRun": {
             "access_level": "Read",
             "action": "GetMLTaskRun",
             "condition_keys": [],
             "description": "Grants permission to retrieve an ML Task Run",
             "orphan": false,
             "resources": [
@@ -76558,14 +76598,30 @@
             "access_level": "Read",
             "action": "GetPlan",
             "condition_keys": [],
             "description": "Grants permission to retrieve a mapping for a script",
             "orphan": false,
             "resources": []
         },
+        "GetQueries": {
+            "access_level": "Undocumented",
+            "action": "GetQueries",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetQuery": {
+            "access_level": "Undocumented",
+            "action": "GetQuery",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "GetRegistry": {
             "access_level": "Read",
             "action": "GetRegistry",
             "condition_keys": [],
             "description": "Grants permission to retrieve a schema registry",
             "orphan": false,
             "resources": [
@@ -76658,24 +76714,88 @@
             "condition_keys": [],
             "description": "Grants permission to retrieve an interactive session",
             "orphan": false,
             "resources": [
                 "session"
             ]
         },
+        "GetStage": {
+            "access_level": "Undocumented",
+            "action": "GetStage",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetStageAttempt": {
+            "access_level": "Undocumented",
+            "action": "GetStageAttempt",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetStageAttemptTaskList": {
+            "access_level": "Undocumented",
+            "action": "GetStageAttemptTaskList",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetStageAttemptTaskSummary": {
+            "access_level": "Undocumented",
+            "action": "GetStageAttemptTaskSummary",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetStageFiles": {
+            "access_level": "Undocumented",
+            "action": "GetStageFiles",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetStages": {
+            "access_level": "Undocumented",
+            "action": "GetStages",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "GetStatement": {
             "access_level": "Read",
             "action": "GetStatement",
             "condition_keys": [],
             "description": "Grants permission to retrieve result and information about a statement in an interactive session",
             "orphan": false,
             "resources": [
                 "session"
             ]
         },
+        "GetStorage": {
+            "access_level": "Undocumented",
+            "action": "GetStorage",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetStorageUnit": {
+            "access_level": "Undocumented",
+            "action": "GetStorageUnit",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "GetTable": {
             "access_level": "Read",
             "action": "GetTable",
             "condition_keys": [],
             "description": "Grants permission to retrieve a table",
             "orphan": false,
             "resources": [
@@ -77137,14 +77257,22 @@
             "description": "Grants permission to remove metadata from schema version",
             "orphan": false,
             "resources": [
                 "registry",
                 "schema"
             ]
         },
+        "RequestLogParsing": {
+            "access_level": "Undocumented",
+            "action": "RequestLogParsing",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ResetJobBookmark": {
             "access_level": "Write",
             "action": "ResetJobBookmark",
             "condition_keys": [],
             "description": "Grants permission to reset a job bookmark",
             "orphan": false,
             "resources": []
@@ -106296,14 +106424,68 @@
             "description": "Grants permission to create a channel",
             "orphan": false,
             "resources": [
                 "channel",
                 "input"
             ]
         },
+        "CreateCloudWatchAlarmTemplate": {
+            "access_level": "Write",
+            "action": "CreateCloudWatchAlarmTemplate",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys"
+            ],
+            "description": "Grants permission to create a cloudwatch alarm template",
+            "orphan": false,
+            "resources": [
+                "cloudwatch-alarm-template",
+                "cloudwatch-alarm-template-group"
+            ]
+        },
+        "CreateCloudWatchAlarmTemplateGroup": {
+            "access_level": "Write",
+            "action": "CreateCloudWatchAlarmTemplateGroup",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys"
+            ],
+            "description": "Grants permission to create a cloudwatch alarm template group",
+            "orphan": false,
+            "resources": [
+                "cloudwatch-alarm-template-group"
+            ]
+        },
+        "CreateEventBridgeRuleTemplate": {
+            "access_level": "Write",
+            "action": "CreateEventBridgeRuleTemplate",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys"
+            ],
+            "description": "Grants permission to create a eventbridge rule template",
+            "orphan": false,
+            "resources": [
+                "eventbridge-rule-template",
+                "eventbridge-rule-template-group"
+            ]
+        },
+        "CreateEventBridgeRuleTemplateGroup": {
+            "access_level": "Write",
+            "action": "CreateEventBridgeRuleTemplateGroup",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys"
+            ],
+            "description": "Grants permission to create a eventbridge rule template group",
+            "orphan": false,
+            "resources": [
+                "eventbridge-rule-template-group"
+            ]
+        },
         "CreateInput": {
             "access_level": "Write",
             "action": "CreateInput",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
@@ -106359,41 +106541,99 @@
             ],
             "description": "Grants permission to create a partner input",
             "orphan": false,
             "resources": [
                 "input"
             ]
         },
+        "CreateSignalMap": {
+            "access_level": "Write",
+            "action": "CreateSignalMap",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys"
+            ],
+            "description": "Grants permission to create a signal map",
+            "orphan": false,
+            "resources": [
+                "signal-map"
+            ]
+        },
         "CreateTags": {
             "access_level": "Tagging",
             "action": "CreateTags",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
-            "description": "Grants permission to create tags for channels, inputs, input security groups, multiplexes, and reservations",
+            "description": "Grants permission to create tags for channels, inputs, input security groups, multiplexes, reservations, signal maps, template groups, and templates",
             "orphan": false,
             "resources": [
                 "channel",
+                "cloudwatch-alarm-template",
+                "cloudwatch-alarm-template-group",
+                "eventbridge-rule-template",
+                "eventbridge-rule-template-group",
                 "input",
                 "input-security-group",
                 "multiplex",
-                "reservation"
+                "reservation",
+                "signal-map"
             ]
         },
         "DeleteChannel": {
             "access_level": "Write",
             "action": "DeleteChannel",
             "condition_keys": [],
             "description": "Grants permission to delete a channel",
             "orphan": false,
             "resources": [
                 "channel"
             ]
         },
+        "DeleteCloudWatchAlarmTemplate": {
+            "access_level": "Write",
+            "action": "DeleteCloudWatchAlarmTemplate",
+            "condition_keys": [],
+            "description": "Grants permission to delete a cloudwatch alarm template",
+            "orphan": false,
+            "resources": [
+                "cloudwatch-alarm-template"
+            ]
+        },
+        "DeleteCloudWatchAlarmTemplateGroup": {
+            "access_level": "Write",
+            "action": "DeleteCloudWatchAlarmTemplateGroup",
+            "condition_keys": [],
+            "description": "Grants permission to delete a cloudwatch alarm template group",
+            "orphan": false,
+            "resources": [
+                "cloudwatch-alarm-template-group"
+            ]
+        },
+        "DeleteEventBridgeRuleTemplate": {
+            "access_level": "Write",
+            "action": "DeleteEventBridgeRuleTemplate",
+            "condition_keys": [],
+            "description": "Grants permission to delete a eventbridge rule template",
+            "orphan": false,
+            "resources": [
+                "eventbridge-rule-template"
+            ]
+        },
+        "DeleteEventBridgeRuleTemplateGroup": {
+            "access_level": "Write",
+            "action": "DeleteEventBridgeRuleTemplateGroup",
+            "condition_keys": [],
+            "description": "Grants permission to delete a eventbridge rule template group",
+            "orphan": false,
+            "resources": [
+                "eventbridge-rule-template-group"
+            ]
+        },
         "DeleteInput": {
             "access_level": "Write",
             "action": "DeleteInput",
             "condition_keys": [],
             "description": "Grants permission to delete an input",
             "orphan": false,
             "resources": [
@@ -106446,28 +106686,43 @@
             "condition_keys": [],
             "description": "Grants permission to delete all schedule actions for a channel",
             "orphan": false,
             "resources": [
                 "channel"
             ]
         },
+        "DeleteSignalMap": {
+            "access_level": "Write",
+            "action": "DeleteSignalMap",
+            "condition_keys": [],
+            "description": "Grants permission to delete a signal map",
+            "orphan": false,
+            "resources": [
+                "signal-map"
+            ]
+        },
         "DeleteTags": {
             "access_level": "Tagging",
             "action": "DeleteTags",
             "condition_keys": [
                 "aws:TagKeys"
             ],
-            "description": "Grants permission to delete tags from channels, inputs, input security groups, multiplexes, and reservations",
+            "description": "Grants permission to delete tags from channels, inputs, input security groups, multiplexes, reservations, signal maps, template groups, and templates",
             "orphan": false,
             "resources": [
                 "channel",
+                "cloudwatch-alarm-template",
+                "cloudwatch-alarm-template-group",
+                "eventbridge-rule-template",
+                "eventbridge-rule-template-group",
                 "input",
                 "input-security-group",
                 "multiplex",
-                "reservation"
+                "reservation",
+                "signal-map"
             ]
         },
         "DescribeAccountConfiguration": {
             "access_level": "Read",
             "action": "DescribeAccountConfiguration",
             "condition_keys": [],
             "description": "Grants permission to view the account configuration of the customer",
@@ -106580,22 +106835,104 @@
             "condition_keys": [],
             "description": "Grants permission to view the thumbnails for a channel",
             "orphan": false,
             "resources": [
                 "channel"
             ]
         },
+        "GetCloudWatchAlarmTemplate": {
+            "access_level": "Read",
+            "action": "GetCloudWatchAlarmTemplate",
+            "condition_keys": [],
+            "description": "Grants permission to get a cloudwatch alarm template",
+            "orphan": false,
+            "resources": [
+                "cloudwatch-alarm-template"
+            ]
+        },
+        "GetCloudWatchAlarmTemplateGroup": {
+            "access_level": "Read",
+            "action": "GetCloudWatchAlarmTemplateGroup",
+            "condition_keys": [],
+            "description": "Grants permission to get a cloudwatch alarm template group",
+            "orphan": false,
+            "resources": [
+                "cloudwatch-alarm-template-group"
+            ]
+        },
+        "GetEventBridgeRuleTemplate": {
+            "access_level": "Read",
+            "action": "GetEventBridgeRuleTemplate",
+            "condition_keys": [],
+            "description": "Grants permission to get a eventbridge rule template",
+            "orphan": false,
+            "resources": [
+                "eventbridge-rule-template"
+            ]
+        },
+        "GetEventBridgeRuleTemplateGroup": {
+            "access_level": "Read",
+            "action": "GetEventBridgeRuleTemplateGroup",
+            "condition_keys": [],
+            "description": "Grants permission to get a eventbridge rule template group",
+            "orphan": false,
+            "resources": [
+                "eventbridge-rule-template-group"
+            ]
+        },
+        "GetSignalMap": {
+            "access_level": "Read",
+            "action": "GetSignalMap",
+            "condition_keys": [],
+            "description": "Grants permission to get a signal map",
+            "orphan": false,
+            "resources": [
+                "signal-map"
+            ]
+        },
         "ListChannels": {
             "access_level": "List",
             "action": "ListChannels",
             "condition_keys": [],
             "description": "Grants permission to list channels",
             "orphan": false,
             "resources": []
         },
+        "ListCloudWatchAlarmTemplateGroups": {
+            "access_level": "List",
+            "action": "ListCloudWatchAlarmTemplateGroups",
+            "condition_keys": [],
+            "description": "Grants permission to list cloudwatch alarm template groups",
+            "orphan": false,
+            "resources": []
+        },
+        "ListCloudWatchAlarmTemplates": {
+            "access_level": "List",
+            "action": "ListCloudWatchAlarmTemplates",
+            "condition_keys": [],
+            "description": "Grants permission to list cloudwatch alarm templates",
+            "orphan": false,
+            "resources": []
+        },
+        "ListEventBridgeRuleTemplateGroups": {
+            "access_level": "List",
+            "action": "ListEventBridgeRuleTemplateGroups",
+            "condition_keys": [],
+            "description": "Grants permission to list eventbridge rule template groups",
+            "orphan": false,
+            "resources": []
+        },
+        "ListEventBridgeRuleTemplates": {
+            "access_level": "List",
+            "action": "ListEventBridgeRuleTemplates",
+            "condition_keys": [],
+            "description": "Grants permission to list eventbridge rule templates",
+            "orphan": false,
+            "resources": []
+        },
         "ListInputDeviceTransfers": {
             "access_level": "List",
             "action": "ListInputDeviceTransfers",
             "condition_keys": [],
             "description": "Grants permission to list input device transfers",
             "orphan": false,
             "resources": []
@@ -106652,26 +106989,39 @@
             "access_level": "List",
             "action": "ListReservations",
             "condition_keys": [],
             "description": "Grants permission to list reservations",
             "orphan": false,
             "resources": []
         },
+        "ListSignalMaps": {
+            "access_level": "List",
+            "action": "ListSignalMaps",
+            "condition_keys": [],
+            "description": "Grants permission to list signal maps",
+            "orphan": false,
+            "resources": []
+        },
         "ListTagsForResource": {
             "access_level": "List",
             "action": "ListTagsForResource",
             "condition_keys": [],
-            "description": "Grants permission to list tags for channels, inputs, input security groups, multiplexes, and reservations",
+            "description": "Grants permission to list tags for channels, inputs, input security groups, multiplexes, reservations, signal maps, template groups, and templates",
             "orphan": false,
             "resources": [
                 "channel",
+                "cloudwatch-alarm-template",
+                "cloudwatch-alarm-template-group",
+                "eventbridge-rule-template",
+                "eventbridge-rule-template-group",
                 "input",
                 "input-security-group",
                 "multiplex",
-                "reservation"
+                "reservation",
+                "signal-map"
             ]
         },
         "PurchaseOffering": {
             "access_level": "Write",
             "action": "PurchaseOffering",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
@@ -106720,14 +107070,24 @@
             "condition_keys": [],
             "description": "Grants permission to start a channel",
             "orphan": false,
             "resources": [
                 "channel"
             ]
         },
+        "StartDeleteMonitorDeployment": {
+            "access_level": "Write",
+            "action": "StartDeleteMonitorDeployment",
+            "condition_keys": [],
+            "description": "Grants permission to start deletion of a signal map's monitor",
+            "orphan": false,
+            "resources": [
+                "signal-map"
+            ]
+        },
         "StartInputDevice": {
             "access_level": "Write",
             "action": "StartInputDevice",
             "condition_keys": [],
             "description": "Grants permission to start an input device attached to a MediaConnect flow",
             "orphan": false,
             "resources": [
@@ -106740,24 +107100,44 @@
             "condition_keys": [],
             "description": "Grants permission to start a maintenance window for an input device",
             "orphan": false,
             "resources": [
                 "input-device"
             ]
         },
+        "StartMonitorDeployment": {
+            "access_level": "Write",
+            "action": "StartMonitorDeployment",
+            "condition_keys": [],
+            "description": "Grants permission to start a signal map monitor deployment",
+            "orphan": false,
+            "resources": [
+                "signal-map"
+            ]
+        },
         "StartMultiplex": {
             "access_level": "Write",
             "action": "StartMultiplex",
             "condition_keys": [],
             "description": "Grants permission to start a multiplex",
             "orphan": false,
             "resources": [
                 "multiplex"
             ]
         },
+        "StartUpdateSignalMap": {
+            "access_level": "Write",
+            "action": "StartUpdateSignalMap",
+            "condition_keys": [],
+            "description": "Grants permission to start a signal map update",
+            "orphan": false,
+            "resources": [
+                "signal-map"
+            ]
+        },
         "StopChannel": {
             "access_level": "Write",
             "action": "StopChannel",
             "condition_keys": [],
             "description": "Grants permission to stop a channel",
             "orphan": false,
             "resources": [
@@ -106818,14 +107198,56 @@
             "condition_keys": [],
             "description": "Grants permission to update the class of a channel",
             "orphan": false,
             "resources": [
                 "channel"
             ]
         },
+        "UpdateCloudWatchAlarmTemplate": {
+            "access_level": "Write",
+            "action": "UpdateCloudWatchAlarmTemplate",
+            "condition_keys": [],
+            "description": "Grants permission to update a cloudwatch alarm template",
+            "orphan": false,
+            "resources": [
+                "cloudwatch-alarm-template",
+                "cloudwatch-alarm-template-group"
+            ]
+        },
+        "UpdateCloudWatchAlarmTemplateGroup": {
+            "access_level": "Write",
+            "action": "UpdateCloudWatchAlarmTemplateGroup",
+            "condition_keys": [],
+            "description": "Grants permission to update a cloudwatch alarm template group",
+            "orphan": false,
+            "resources": [
+                "cloudwatch-alarm-template-group"
+            ]
+        },
+        "UpdateEventBridgeRuleTemplate": {
+            "access_level": "Write",
+            "action": "UpdateEventBridgeRuleTemplate",
+            "condition_keys": [],
+            "description": "Grants permission to update a eventbridge rule template",
+            "orphan": false,
+            "resources": [
+                "eventbridge-rule-template",
+                "eventbridge-rule-template-group"
+            ]
+        },
+        "UpdateEventBridgeRuleTemplateGroup": {
+            "access_level": "Write",
+            "action": "UpdateEventBridgeRuleTemplateGroup",
+            "condition_keys": [],
+            "description": "Grants permission to update a eventbridge rule template group",
+            "orphan": false,
+            "resources": [
+                "eventbridge-rule-template-group"
+            ]
+        },
         "UpdateInput": {
             "access_level": "Write",
             "action": "UpdateInput",
             "condition_keys": [],
             "description": "Grants permission to update an input",
             "orphan": false,
             "resources": [
```

### Comparing `iam_actions-1.2.20240411/iam_actions/generate/action_map.py` & `iam_actions-1.2.20240412/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240411/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20240412/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240411/iam_actions/generate/generate.py` & `iam_actions-1.2.20240412/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240411/iam_actions/generate/notifier.py` & `iam_actions-1.2.20240412/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240411/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20240412/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240411/iam_actions/generate/services.py` & `iam_actions-1.2.20240412/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240411/iam_actions/policies.json` & `iam_actions-1.2.20240412/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999996327676028%*

 * *Differences: {"'serviceMap'": "{'AWS Elemental MediaLive': {'Actions': {insert: [(8, "*

 * *                 "'CreateCloudWatchAlarmTemplate'), (9, 'CreateCloudWatchAlarmTemplateGroup'), "*

 * *                 "(10, 'CreateEventBridgeRuleTemplate'), (11, "*

 * *                 "'CreateEventBridgeRuleTemplateGroup'), (17, 'CreateSignalMap'), (20, "*

 * *                 "'DeleteCloudWatchAlarmTemplate'), (21, 'DeleteCloudWatchAlarmTemplateGroup'), "*

 * *                 "(22, 'DeleteEventBridgeRuleTemplate'), (23, "*

 * *                 "'DeleteE […]*

```diff
@@ -4218,65 +4218,92 @@
                 "BatchDelete",
                 "BatchStart",
                 "BatchStop",
                 "BatchUpdateSchedule",
                 "CancelInputDeviceTransfer",
                 "ClaimDevice",
                 "CreateChannel",
+                "CreateCloudWatchAlarmTemplate",
+                "CreateCloudWatchAlarmTemplateGroup",
+                "CreateEventBridgeRuleTemplate",
+                "CreateEventBridgeRuleTemplateGroup",
                 "CreateInput",
                 "CreateInputSecurityGroup",
                 "CreateMultiplex",
                 "CreateMultiplexProgram",
                 "CreatePartnerInput",
+                "CreateSignalMap",
                 "CreateTags",
                 "DeleteChannel",
+                "DeleteCloudWatchAlarmTemplate",
+                "DeleteCloudWatchAlarmTemplateGroup",
+                "DeleteEventBridgeRuleTemplate",
+                "DeleteEventBridgeRuleTemplateGroup",
                 "DeleteInput",
                 "DeleteInputSecurityGroup",
                 "DeleteMultiplex",
                 "DeleteMultiplexProgram",
                 "DeleteReservation",
                 "DeleteSchedule",
+                "DeleteSignalMap",
                 "DeleteTags",
                 "DescribeAccountConfiguration",
                 "DescribeChannel",
                 "DescribeInput",
                 "DescribeInputDevice",
                 "DescribeInputDeviceThumbnail",
                 "DescribeInputSecurityGroup",
                 "DescribeMultiplex",
                 "DescribeMultiplexProgram",
                 "DescribeOffering",
                 "DescribeReservation",
                 "DescribeSchedule",
                 "DescribeThumbnails",
+                "GetCloudWatchAlarmTemplate",
+                "GetCloudWatchAlarmTemplateGroup",
+                "GetEventBridgeRuleTemplate",
+                "GetEventBridgeRuleTemplateGroup",
+                "GetSignalMap",
                 "ListChannels",
+                "ListCloudWatchAlarmTemplateGroups",
+                "ListCloudWatchAlarmTemplates",
+                "ListEventBridgeRuleTemplateGroups",
+                "ListEventBridgeRuleTemplates",
                 "ListInputDeviceTransfers",
                 "ListInputDevices",
                 "ListInputSecurityGroups",
                 "ListInputs",
                 "ListMultiplexPrograms",
                 "ListMultiplexes",
                 "ListOfferings",
                 "ListReservations",
+                "ListSignalMaps",
                 "ListTagsForResource",
                 "PurchaseOffering",
                 "RebootInputDevice",
                 "RejectInputDeviceTransfer",
                 "RestartChannelPipelines",
                 "StartChannel",
+                "StartDeleteMonitorDeployment",
                 "StartInputDevice",
                 "StartInputDeviceMaintenanceWindow",
+                "StartMonitorDeployment",
                 "StartMultiplex",
+                "StartUpdateSignalMap",
                 "StopChannel",
                 "StopInputDevice",
                 "StopMultiplex",
                 "TransferInputDevice",
                 "UpdateAccountConfiguration",
                 "UpdateChannel",
                 "UpdateChannelClass",
+                "UpdateCloudWatchAlarmTemplate",
+                "UpdateCloudWatchAlarmTemplateGroup",
+                "UpdateEventBridgeRuleTemplate",
+                "UpdateEventBridgeRuleTemplateGroup",
                 "UpdateInput",
                 "UpdateInputDevice",
                 "UpdateInputSecurityGroup",
                 "UpdateMultiplex",
                 "UpdateMultiplexProgram",
                 "UpdateReservation"
             ],
@@ -4746,14 +4773,15 @@
                 "BatchDeleteTableVersion",
                 "BatchGetBlueprints",
                 "BatchGetCrawlers",
                 "BatchGetCustomEntityTypes",
                 "BatchGetDevEndpoints",
                 "BatchGetJobs",
                 "BatchGetPartition",
+                "BatchGetStageFiles",
                 "BatchGetTableOptimizer",
                 "BatchGetTriggers",
                 "BatchGetWorkflows",
                 "BatchStopJobRun",
                 "BatchUpdatePartition",
                 "CancelDataQualityRuleRecommendationRun",
                 "CancelDataQualityRulesetEvaluationRun",
@@ -4833,40 +4861,54 @@
                 "GetDataQualityRuleset",
                 "GetDataQualityRulesetEvaluationRun",
                 "GetDatabase",
                 "GetDatabases",
                 "GetDataflowGraph",
                 "GetDevEndpoint",
                 "GetDevEndpoints",
+                "GetEnvironment",
+                "GetExecutors",
+                "GetExecutorsThreads",
                 "GetJob",
                 "GetJobBookmark",
                 "GetJobRun",
                 "GetJobRuns",
                 "GetJobs",
+                "GetLogParsingStatus",
                 "GetMLTaskRun",
                 "GetMLTaskRuns",
                 "GetMLTransform",
                 "GetMLTransforms",
                 "GetMapping",
                 "GetNotebookInstanceStatus",
                 "GetPartition",
                 "GetPartitionIndexes",
                 "GetPartitions",
                 "GetPlan",
+                "GetQueries",
+                "GetQuery",
                 "GetRegistry",
                 "GetResourcePolicies",
                 "GetResourcePolicy",
                 "GetSchema",
                 "GetSchemaByDefinition",
                 "GetSchemaVersion",
                 "GetSchemaVersionsDiff",
                 "GetSecurityConfiguration",
                 "GetSecurityConfigurations",
                 "GetSession",
+                "GetStage",
+                "GetStageAttempt",
+                "GetStageAttemptTaskList",
+                "GetStageAttemptTaskSummary",
+                "GetStageFiles",
+                "GetStages",
                 "GetStatement",
+                "GetStorage",
+                "GetStorageUnit",
                 "GetTable",
                 "GetTableOptimizer",
                 "GetTableVersion",
                 "GetTableVersions",
                 "GetTables",
                 "GetTags",
                 "GetTrigger",
@@ -4906,14 +4948,15 @@
                 "PutDataCatalogEncryptionSettings",
                 "PutResourcePolicy",
                 "PutSchemaVersionMetadata",
                 "PutWorkflowRunProperties",
                 "QuerySchemaVersionMetadata",
                 "RegisterSchemaVersion",
                 "RemoveSchemaVersionMetadata",
+                "RequestLogParsing",
                 "ResetJobBookmark",
                 "ResumeWorkflowRun",
                 "RunDataPreviewStatement",
                 "RunStatement",
                 "SearchTables",
                 "SendFeedback",
                 "StartBlueprintRun",
```

### Comparing `iam_actions-1.2.20240411/iam_actions/resourcetypes.json` & `iam_actions-1.2.20240412/iam_actions/resourcetypes.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994658119658119%*

 * *Differences: {"'medialive'": "{'signal-map': OrderedDict([('arn_pattern', 'arn:*:medialive:*:*:signal-map:*'), "*

 * *                "('condition_keys', 'aws:ResourceTag/${TagKey}')]), "*

 * *                "'cloudwatch-alarm-template-group': OrderedDict([('arn_pattern', "*

 * *                "'arn:*:medialive:*:*:cloudwatch-alarm-template-group:*'), ('condition_keys', "*

 * *                "'aws:ResourceTag/${TagKey}')]), 'cloudwatch-alarm-template': "*

 * *                "OrderedDict([('arn_pattern', 'arn:*:medialive:*:*:cloudwatch-alarm […]*

```diff
@@ -4372,14 +4372,30 @@
     },
     "mediaimport": {},
     "medialive": {
         "channel": {
             "arn_pattern": "arn:*:medialive:*:*:channel:*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
+        "cloudwatch-alarm-template": {
+            "arn_pattern": "arn:*:medialive:*:*:cloudwatch-alarm-template:*",
+            "condition_keys": "aws:ResourceTag/${TagKey}"
+        },
+        "cloudwatch-alarm-template-group": {
+            "arn_pattern": "arn:*:medialive:*:*:cloudwatch-alarm-template-group:*",
+            "condition_keys": "aws:ResourceTag/${TagKey}"
+        },
+        "eventbridge-rule-template": {
+            "arn_pattern": "arn:*:medialive:*:*:eventbridge-rule-template:*",
+            "condition_keys": "aws:ResourceTag/${TagKey}"
+        },
+        "eventbridge-rule-template-group": {
+            "arn_pattern": "arn:*:medialive:*:*:eventbridge-rule-template-group:*",
+            "condition_keys": "aws:ResourceTag/${TagKey}"
+        },
         "input": {
             "arn_pattern": "arn:*:medialive:*:*:input:*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
         "input-device": {
             "arn_pattern": "arn:*:medialive:*:*:inputDevice:*",
             "condition_keys": null
@@ -4395,14 +4411,18 @@
         "offering": {
             "arn_pattern": "arn:*:medialive:*:*:offering:*",
             "condition_keys": null
         },
         "reservation": {
             "arn_pattern": "arn:*:medialive:*:*:reservation:*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
+        },
+        "signal-map": {
+            "arn_pattern": "arn:*:medialive:*:*:signal-map:*",
+            "condition_keys": "aws:ResourceTag/${TagKey}"
         }
     },
     "mediapackage": {
         "channels": {
             "arn_pattern": "arn:*:mediapackage:*:*:channels/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
```

### Comparing `iam_actions-1.2.20240411/iam_actions/services.json` & `iam_actions-1.2.20240412/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999615818415225%*

 * *Differences: {"'glue'": "{'Actions': {insert: [(11, 'BatchGetStageFiles'), (99, 'GetEnvironment'), (100, "*

 * *           "'GetExecutors'), (101, 'GetExecutorsThreads'), (107, 'GetLogParsingStatus'), (118, "*

 * *           "'GetQueries'), (119, 'GetQuery'), (130, 'GetStage'), (131, 'GetStageAttempt'), (132, "*

 * *           "'GetStageAttemptTaskList'), (133, 'GetStageAttemptTaskSummary'), (134, "*

 * *           "'GetStageFiles'), (135, 'GetStages'), (137, 'GetStorage'), (138, 'GetStorageUnit'), "*

 * *           "(186, 'RequestLogParsing')] […]*

```diff
@@ -10349,14 +10349,15 @@
             "BatchDeleteTableVersion",
             "BatchGetBlueprints",
             "BatchGetCrawlers",
             "BatchGetCustomEntityTypes",
             "BatchGetDevEndpoints",
             "BatchGetJobs",
             "BatchGetPartition",
+            "BatchGetStageFiles",
             "BatchGetTableOptimizer",
             "BatchGetTriggers",
             "BatchGetWorkflows",
             "BatchStopJobRun",
             "BatchUpdatePartition",
             "CancelDataQualityRuleRecommendationRun",
             "CancelDataQualityRulesetEvaluationRun",
@@ -10436,40 +10437,54 @@
             "GetDataQualityRuleset",
             "GetDataQualityRulesetEvaluationRun",
             "GetDatabase",
             "GetDatabases",
             "GetDataflowGraph",
             "GetDevEndpoint",
             "GetDevEndpoints",
+            "GetEnvironment",
+            "GetExecutors",
+            "GetExecutorsThreads",
             "GetJob",
             "GetJobBookmark",
             "GetJobRun",
             "GetJobRuns",
             "GetJobs",
+            "GetLogParsingStatus",
             "GetMLTaskRun",
             "GetMLTaskRuns",
             "GetMLTransform",
             "GetMLTransforms",
             "GetMapping",
             "GetNotebookInstanceStatus",
             "GetPartition",
             "GetPartitionIndexes",
             "GetPartitions",
             "GetPlan",
+            "GetQueries",
+            "GetQuery",
             "GetRegistry",
             "GetResourcePolicies",
             "GetResourcePolicy",
             "GetSchema",
             "GetSchemaByDefinition",
             "GetSchemaVersion",
             "GetSchemaVersionsDiff",
             "GetSecurityConfiguration",
             "GetSecurityConfigurations",
             "GetSession",
+            "GetStage",
+            "GetStageAttempt",
+            "GetStageAttemptTaskList",
+            "GetStageAttemptTaskSummary",
+            "GetStageFiles",
+            "GetStages",
             "GetStatement",
+            "GetStorage",
+            "GetStorageUnit",
             "GetTable",
             "GetTableOptimizer",
             "GetTableVersion",
             "GetTableVersions",
             "GetTables",
             "GetTags",
             "GetTrigger",
@@ -10509,14 +10524,15 @@
             "PutDataCatalogEncryptionSettings",
             "PutResourcePolicy",
             "PutSchemaVersionMetadata",
             "PutWorkflowRunProperties",
             "QuerySchemaVersionMetadata",
             "RegisterSchemaVersion",
             "RemoveSchemaVersionMetadata",
+            "RequestLogParsing",
             "ResetJobBookmark",
             "ResumeWorkflowRun",
             "RunDataPreviewStatement",
             "RunStatement",
             "SearchTables",
             "SendFeedback",
             "StartBlueprintRun",
@@ -14777,65 +14793,92 @@
             "BatchDelete",
             "BatchStart",
             "BatchStop",
             "BatchUpdateSchedule",
             "CancelInputDeviceTransfer",
             "ClaimDevice",
             "CreateChannel",
+            "CreateCloudWatchAlarmTemplate",
+            "CreateCloudWatchAlarmTemplateGroup",
+            "CreateEventBridgeRuleTemplate",
+            "CreateEventBridgeRuleTemplateGroup",
             "CreateInput",
             "CreateInputSecurityGroup",
             "CreateMultiplex",
             "CreateMultiplexProgram",
             "CreatePartnerInput",
+            "CreateSignalMap",
             "CreateTags",
             "DeleteChannel",
+            "DeleteCloudWatchAlarmTemplate",
+            "DeleteCloudWatchAlarmTemplateGroup",
+            "DeleteEventBridgeRuleTemplate",
+            "DeleteEventBridgeRuleTemplateGroup",
             "DeleteInput",
             "DeleteInputSecurityGroup",
             "DeleteMultiplex",
             "DeleteMultiplexProgram",
             "DeleteReservation",
             "DeleteSchedule",
+            "DeleteSignalMap",
             "DeleteTags",
             "DescribeAccountConfiguration",
             "DescribeChannel",
             "DescribeInput",
             "DescribeInputDevice",
             "DescribeInputDeviceThumbnail",
             "DescribeInputSecurityGroup",
             "DescribeMultiplex",
             "DescribeMultiplexProgram",
             "DescribeOffering",
             "DescribeReservation",
             "DescribeSchedule",
             "DescribeThumbnails",
+            "GetCloudWatchAlarmTemplate",
+            "GetCloudWatchAlarmTemplateGroup",
+            "GetEventBridgeRuleTemplate",
+            "GetEventBridgeRuleTemplateGroup",
+            "GetSignalMap",
             "ListChannels",
+            "ListCloudWatchAlarmTemplateGroups",
+            "ListCloudWatchAlarmTemplates",
+            "ListEventBridgeRuleTemplateGroups",
+            "ListEventBridgeRuleTemplates",
             "ListInputDeviceTransfers",
             "ListInputDevices",
             "ListInputSecurityGroups",
             "ListInputs",
             "ListMultiplexPrograms",
             "ListMultiplexes",
             "ListOfferings",
             "ListReservations",
+            "ListSignalMaps",
             "ListTagsForResource",
             "PurchaseOffering",
             "RebootInputDevice",
             "RejectInputDeviceTransfer",
             "RestartChannelPipelines",
             "StartChannel",
+            "StartDeleteMonitorDeployment",
             "StartInputDevice",
             "StartInputDeviceMaintenanceWindow",
+            "StartMonitorDeployment",
             "StartMultiplex",
+            "StartUpdateSignalMap",
             "StopChannel",
             "StopInputDevice",
             "StopMultiplex",
             "TransferInputDevice",
             "UpdateAccountConfiguration",
             "UpdateChannel",
             "UpdateChannelClass",
+            "UpdateCloudWatchAlarmTemplate",
+            "UpdateCloudWatchAlarmTemplateGroup",
+            "UpdateEventBridgeRuleTemplate",
+            "UpdateEventBridgeRuleTemplateGroup",
             "UpdateInput",
             "UpdateInputDevice",
             "UpdateInputSecurityGroup",
             "UpdateMultiplex",
             "UpdateMultiplexProgram",
             "UpdateReservation"
         ],
```

### Comparing `iam_actions-1.2.20240411/pyproject.toml` & `iam_actions-1.2.20240412/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20240411"
+version = "1.2.20240412"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20240411/setup.py` & `iam_actions-1.2.20240412/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20240411',
+    'version': '1.2.20240412',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20240411/PKG-INFO` & `iam_actions-1.2.20240412/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20240411
+Version: 1.2.20240412
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

