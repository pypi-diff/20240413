# Comparing `tmp/botocore-a-la-carte-iotwireless-1.34.83.tar.gz` & `tmp/botocore-a-la-carte-iotwireless-1.34.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-iotwireless-1.34.83.tar", last modified: Fri Apr 12 01:01:06 2024, max compression
+gzip compressed data, was "botocore-a-la-carte-iotwireless-1.34.9.tar", last modified: Thu Dec 28 01:06:45 2023, max compression
```

## Comparing `botocore-a-la-carte-iotwireless-1.34.83.tar` & `botocore-a-la-carte-iotwireless-1.34.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 01:01:06.948897 botocore-a-la-carte-iotwireless-1.34.83/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-12 01:01:06.000000 botocore-a-la-carte-iotwireless-1.34.83/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-12 01:01:06.948897 botocore-a-la-carte-iotwireless-1.34.83/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 01:01:06.948897 botocore-a-la-carte-iotwireless-1.34.83/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 01:01:06.948897 botocore-a-la-carte-iotwireless-1.34.83/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 01:01:06.948897 botocore-a-la-carte-iotwireless-1.34.83/botocore/data/iotwireless/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 01:01:06.948897 botocore-a-la-carte-iotwireless-1.34.83/botocore/data/iotwireless/2020-11-22/
--rw-r--r--   0 runner    (1001) docker     (127)    13762 2024-04-12 01:00:49.000000 botocore-a-la-carte-iotwireless-1.34.83/botocore/data/iotwireless/2020-11-22/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-12 01:00:49.000000 botocore-a-la-carte-iotwireless-1.34.83/botocore/data/iotwireless/2020-11-22/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-12 01:00:49.000000 botocore-a-la-carte-iotwireless-1.34.83/botocore/data/iotwireless/2020-11-22/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)   316538 2024-04-12 01:00:49.000000 botocore-a-la-carte-iotwireless-1.34.83/botocore/data/iotwireless/2020-11-22/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 01:01:06.948897 botocore-a-la-carte-iotwireless-1.34.83/botocore_a_la_carte_iotwireless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-12 01:01:06.000000 botocore-a-la-carte-iotwireless-1.34.83/botocore_a_la_carte_iotwireless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-12 01:01:06.000000 botocore-a-la-carte-iotwireless-1.34.83/botocore_a_la_carte_iotwireless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 01:01:06.000000 botocore-a-la-carte-iotwireless-1.34.83/botocore_a_la_carte_iotwireless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 01:01:06.000000 botocore-a-la-carte-iotwireless-1.34.83/botocore_a_la_carte_iotwireless.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 01:01:06.948897 botocore-a-la-carte-iotwireless-1.34.83/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-12 01:01:06.000000 botocore-a-la-carte-iotwireless-1.34.83/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:45.874311 botocore-a-la-carte-iotwireless-1.34.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2023-12-28 01:06:45.000000 botocore-a-la-carte-iotwireless-1.34.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2023-12-28 01:06:45.874311 botocore-a-la-carte-iotwireless-1.34.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:45.874311 botocore-a-la-carte-iotwireless-1.34.9/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:45.874311 botocore-a-la-carte-iotwireless-1.34.9/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:45.874311 botocore-a-la-carte-iotwireless-1.34.9/botocore/data/iotwireless/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:45.874311 botocore-a-la-carte-iotwireless-1.34.9/botocore/data/iotwireless/2020-11-22/
+-rw-r--r--   0 runner    (1001) docker     (127)    13762 2023-12-28 01:06:26.000000 botocore-a-la-carte-iotwireless-1.34.9/botocore/data/iotwireless/2020-11-22/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2023-12-28 01:06:26.000000 botocore-a-la-carte-iotwireless-1.34.9/botocore/data/iotwireless/2020-11-22/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-28 01:06:26.000000 botocore-a-la-carte-iotwireless-1.34.9/botocore/data/iotwireless/2020-11-22/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   305595 2023-12-28 01:06:26.000000 botocore-a-la-carte-iotwireless-1.34.9/botocore/data/iotwireless/2020-11-22/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:45.874311 botocore-a-la-carte-iotwireless-1.34.9/botocore_a_la_carte_iotwireless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2023-12-28 01:06:45.000000 botocore-a-la-carte-iotwireless-1.34.9/botocore_a_la_carte_iotwireless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2023-12-28 01:06:45.000000 botocore-a-la-carte-iotwireless-1.34.9/botocore_a_la_carte_iotwireless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-28 01:06:45.000000 botocore-a-la-carte-iotwireless-1.34.9/botocore_a_la_carte_iotwireless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-28 01:06:45.000000 botocore-a-la-carte-iotwireless-1.34.9/botocore_a_la_carte_iotwireless.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-28 01:06:45.874311 botocore-a-la-carte-iotwireless-1.34.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2023-12-28 01:06:45.000000 botocore-a-la-carte-iotwireless-1.34.9/setup.py
```

### Comparing `botocore-a-la-carte-iotwireless-1.34.83/LICENSE.txt` & `botocore-a-la-carte-iotwireless-1.34.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-iotwireless-1.34.83/PKG-INFO` & `botocore-a-la-carte-iotwireless-1.34.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-iotwireless
-Version: 1.34.83
+Version: 1.34.9
 Summary: iotwireless data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-iotwireless-1.34.83/botocore/data/iotwireless/2020-11-22/endpoint-rule-set-1.json` & `botocore-a-la-carte-iotwireless-1.34.9/botocore/data/iotwireless/2020-11-22/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-iotwireless-1.34.83/botocore/data/iotwireless/2020-11-22/service-2.json` & `botocore-a-la-carte-iotwireless-1.34.9/botocore/data/iotwireless/2020-11-22/service-2.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8923426279369728%*

 * *Differences: {"'documentation'": "'<p>AWS IoT Wireless provides bi-directional communication between "*

 * *                    'internet-connected wireless devices and the AWS Cloud. To onboard both '*

 * *                    'LoRaWAN and Sidewalk devices to AWS IoT, use the IoT Wireless API. These '*

 * *                    'wireless devices use the Low Power Wide Area Networking (LPWAN) communication '*

 * *                    'protocol to communicate with AWS IoT.</p> <p>Using the API, you can perform '*

 * *                    'create, rea […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "documentation": "<p>AWS IoT Wireless provides bi-directional communication between internet-connected wireless devices and the AWS Cloud. To onboard both LoRaWAN and Sidewalk devices to AWS IoT, use the IoT Wireless API. These wireless devices use the Low Power Wide Area Networking (LPWAN) communication protocol to communicate with AWS IoT.</p> <p>Using the API, you can perform create, read, update, and delete operations for your wireless devices, gateways, destinations, and profiles. After onboarding your devices, you can use the API operations to set log levels and monitor your devices with CloudWatch.</p> <p>You can also use the API operations to create multicast groups and schedule a multicast session for sending a downlink message to devices in the group. By using Firmware Updates Over-The-Air (FUOTA) API operations, you can create a FUOTA task and schedule a session to update the firmware of individual devices or an entire group of devices in a multicast group.</p> <p>To connect to the AWS IoT Wireless Service, use the Service endpoints as described in <a href=\"https://docs.aws.amazon.com/general/latest/gr/iot-lorawan.html#iot-wireless_region\">IoT Wireless Service endpoints</a> in the <i>AWS General Reference</i>.</p>",
+    "documentation": "<p>AWS IoT Wireless provides bi-directional communication between internet-connected wireless devices and the AWS Cloud. To onboard both LoRaWAN and Sidewalk devices to AWS IoT, use the IoT Wireless API. These wireless devices use the Low Power Wide Area Networking (LPWAN) communication protocol to communicate with AWS IoT.</p> <p>Using the API, you can perform create, read, update, and delete operations for your wireless devices, gateways, destinations, and profiles. After onboarding your devices, you can use the API operations to set log levels and monitor your devices with CloudWatch.</p> <p>You can also use the API operations to create multicast groups and schedule a multicast session for sending a downlink message to devices in the group. By using Firmware Updates Over-The-Air (FUOTA) API operations, you can create a FUOTA task and schedule a session to update the firmware of individual devices or an entire group of devices in a multicast group.</p>",
     "metadata": {
         "apiVersion": "2020-11-22",
         "endpointPrefix": "api.iotwireless",
         "protocol": "rest-json",
         "serviceFullName": "AWS IoT Wireless",
         "serviceId": "IoT Wireless",
         "signatureVersion": "v4",
@@ -1436,83 +1436,14 @@
                 "shape": "GetLogLevelsByResourceTypesRequest"
             },
             "name": "GetLogLevelsByResourceTypes",
             "output": {
                 "shape": "GetLogLevelsByResourceTypesResponse"
             }
         },
-        "GetMetricConfiguration": {
-            "documentation": "<p>Get the metric configuration status for this account.</p>",
-            "errors": [
-                {
-                    "shape": "ValidationException"
-                },
-                {
-                    "shape": "ResourceNotFoundException"
-                },
-                {
-                    "shape": "AccessDeniedException"
-                },
-                {
-                    "shape": "ConflictException"
-                },
-                {
-                    "shape": "InternalServerException"
-                },
-                {
-                    "shape": "ThrottlingException"
-                }
-            ],
-            "http": {
-                "method": "GET",
-                "requestUri": "/metric-configuration",
-                "responseCode": 200
-            },
-            "input": {
-                "shape": "GetMetricConfigurationRequest"
-            },
-            "name": "GetMetricConfiguration",
-            "output": {
-                "shape": "GetMetricConfigurationResponse"
-            }
-        },
-        "GetMetrics": {
-            "documentation": "<p>Get metrics.</p>",
-            "errors": [
-                {
-                    "shape": "ValidationException"
-                },
-                {
-                    "shape": "ResourceNotFoundException"
-                },
-                {
-                    "shape": "AccessDeniedException"
-                },
-                {
-                    "shape": "ConflictException"
-                },
-                {
-                    "shape": "InternalServerException"
-                },
-                {
-                    "shape": "ThrottlingException"
-                }
-            ],
-            "http": {
-                "method": "POST",
-                "requestUri": "/metrics"
-            },
-            "input": {
-                "shape": "GetMetricsRequest"
-            },
-            "name": "GetMetrics",
-            "output": {
-                "shape": "GetMetricsResponse"
-            }
-        },
         "GetMulticastGroup": {
             "documentation": "<p>Gets information about a multicast group.</p>",
             "errors": [
                 {
                     "shape": "ValidationException"
                 },
                 {
@@ -3287,50 +3218,14 @@
                 "shape": "UpdateLogLevelsByResourceTypesRequest"
             },
             "name": "UpdateLogLevelsByResourceTypes",
             "output": {
                 "shape": "UpdateLogLevelsByResourceTypesResponse"
             }
         },
-        "UpdateMetricConfiguration": {
-            "documentation": "<p>Update the metric configuration.</p>",
-            "errors": [
-                {
-                    "shape": "ValidationException"
-                },
-                {
-                    "shape": "ResourceNotFoundException"
-                },
-                {
-                    "shape": "AccessDeniedException"
-                },
-                {
-                    "shape": "ConflictException"
-                },
-                {
-                    "shape": "InternalServerException"
-                },
-                {
-                    "shape": "ThrottlingException"
-                }
-            ],
-            "http": {
-                "method": "PUT",
-                "requestUri": "/metric-configuration",
-                "responseCode": 204
-            },
-            "idempotent": true,
-            "input": {
-                "shape": "UpdateMetricConfigurationRequest"
-            },
-            "name": "UpdateMetricConfiguration",
-            "output": {
-                "shape": "UpdateMetricConfigurationResponse"
-            }
-        },
         "UpdateMulticastGroup": {
             "documentation": "<p>Updates properties of a multicast group session.</p>",
             "errors": [
                 {
                     "shape": "ValidationException"
                 },
                 {
@@ -3695,22 +3590,14 @@
             "max": 604800,
             "min": 0,
             "type": "integer"
         },
         "AddGwMetadata": {
             "type": "boolean"
         },
-        "AggregationPeriod": {
-            "enum": [
-                "OneHour",
-                "OneDay",
-                "OneWeek"
-            ],
-            "type": "string"
-        },
         "AmazonId": {
             "documentation": "<p>The Sidewalk Amazon ID.</p>",
             "max": 2048,
             "type": "string"
         },
         "AmazonResourceName": {
             "max": 1011,
@@ -3954,17 +3841,14 @@
         "AssociateWirelessGatewayWithThingResponse": {
             "members": {},
             "type": "structure"
         },
         "AutoCreateTasks": {
             "type": "boolean"
         },
-        "Avg": {
-            "type": "double"
-        },
         "BCCH": {
             "max": 1023,
             "min": 0,
             "type": "integer"
         },
         "BSIC": {
             "max": 63,
@@ -5197,46 +5081,14 @@
             ],
             "type": "string"
         },
         "DeviceTypeId": {
             "max": 2048,
             "type": "string"
         },
-        "Dimension": {
-            "documentation": "<p>The required list of dimensions for the metric.</p>",
-            "members": {
-                "name": {
-                    "documentation": "<p>The name of the dimension.</p>",
-                    "shape": "DimensionName"
-                },
-                "value": {
-                    "documentation": "<p>The dimension's value.</p>",
-                    "shape": "DimensionValue"
-                }
-            },
-            "type": "structure"
-        },
-        "DimensionName": {
-            "enum": [
-                "DeviceId",
-                "GatewayId"
-            ],
-            "max": 256,
-            "type": "string"
-        },
-        "DimensionValue": {
-            "max": 256,
-            "type": "string"
-        },
-        "Dimensions": {
-            "member": {
-                "shape": "Dimension"
-            },
-            "type": "list"
-        },
         "DisassociateAwsAccountFromPartnerAccountRequest": {
             "members": {
                 "PartnerAccountId": {
                     "documentation": "<p>The partner account ID to disassociate from the AWS account.</p>",
                     "location": "uri",
                     "locationName": "PartnerAccountId",
                     "shape": "PartnerAccountId"
@@ -5961,45 +5813,14 @@
                 },
                 "WirelessGatewayLogOptions": {
                     "shape": "WirelessGatewayLogOptionList"
                 }
             },
             "type": "structure"
         },
-        "GetMetricConfigurationRequest": {
-            "members": {},
-            "type": "structure"
-        },
-        "GetMetricConfigurationResponse": {
-            "members": {
-                "SummaryMetric": {
-                    "documentation": "<p>The account's configuration status for summary metric aggregation.</p>",
-                    "shape": "SummaryMetricConfiguration"
-                }
-            },
-            "type": "structure"
-        },
-        "GetMetricsRequest": {
-            "members": {
-                "SummaryMetricQueries": {
-                    "documentation": "<p>The list of queries to retrieve summary metrics.</p>",
-                    "shape": "SummaryMetricQueries"
-                }
-            },
-            "type": "structure"
-        },
-        "GetMetricsResponse": {
-            "members": {
-                "SummaryMetricQueryResults": {
-                    "documentation": "<p>The list of retrieved metrics.</p>",
-                    "shape": "SummaryMetricQueryResults"
-                }
-            },
-            "type": "structure"
-        },
         "GetMulticastGroupRequest": {
             "members": {
                 "Id": {
                     "location": "uri",
                     "locationName": "Id",
                     "shape": "MulticastGroupId"
                 }
@@ -8453,17 +8274,14 @@
             "pattern": "^([0-9A-Fa-f]{2}[:-]?){5}([0-9A-Fa-f]{2})$",
             "type": "string"
         },
         "MacVersion": {
             "max": 64,
             "type": "string"
         },
-        "Max": {
-            "type": "double"
-        },
         "MaxAllowedSignature": {
             "type": "integer"
         },
         "MaxDutyCycle": {
             "max": 100,
             "min": 0,
             "type": "integer"
@@ -8520,123 +8338,14 @@
                 "CUSTOM_COMMAND_ID_NOTIFY",
                 "CUSTOM_COMMAND_ID_GET",
                 "CUSTOM_COMMAND_ID_SET",
                 "CUSTOM_COMMAND_ID_RESP"
             ],
             "type": "string"
         },
-        "MetricName": {
-            "enum": [
-                "DeviceRSSI",
-                "DeviceSNR",
-                "DeviceUplinkCount",
-                "DeviceDownlinkCount",
-                "DeviceUplinkLostCount",
-                "DeviceUplinkLostRate",
-                "DeviceJoinRequestCount",
-                "DeviceJoinAcceptCount",
-                "DeviceRoamingUplinkCount",
-                "DeviceRoamingDownlinkCount",
-                "GatewayUpTime",
-                "GatewayDownTime",
-                "GatewayRSSI",
-                "GatewaySNR",
-                "GatewayUplinkCount",
-                "GatewayDownlinkCount",
-                "GatewayJoinRequestCount",
-                "GatewayJoinAcceptCount",
-                "AwsAccountUplinkCount",
-                "AwsAccountDownlinkCount",
-                "AwsAccountUplinkLostCount",
-                "AwsAccountUplinkLostRate",
-                "AwsAccountJoinRequestCount",
-                "AwsAccountJoinAcceptCount",
-                "AwsAccountRoamingUplinkCount",
-                "AwsAccountRoamingDownlinkCount",
-                "AwsAccountDeviceCount",
-                "AwsAccountGatewayCount",
-                "AwsAccountActiveDeviceCount",
-                "AwsAccountActiveGatewayCount"
-            ],
-            "max": 256,
-            "type": "string"
-        },
-        "MetricQueryEndTimestamp": {
-            "type": "timestamp"
-        },
-        "MetricQueryError": {
-            "max": 256,
-            "type": "string"
-        },
-        "MetricQueryId": {
-            "max": 256,
-            "type": "string"
-        },
-        "MetricQueryStartTimestamp": {
-            "type": "timestamp"
-        },
-        "MetricQueryStatus": {
-            "enum": [
-                "Succeeded",
-                "Failed"
-            ],
-            "type": "string"
-        },
-        "MetricQueryTimestamp": {
-            "type": "timestamp"
-        },
-        "MetricQueryTimestamps": {
-            "member": {
-                "shape": "MetricQueryTimestamp"
-            },
-            "type": "list"
-        },
-        "MetricQueryValue": {
-            "documentation": "<p>The aggregated values of the metric.</p>",
-            "members": {
-                "Avg": {
-                    "documentation": "<p>The average of the values of the all data points collected during the period.</p>",
-                    "shape": "Avg"
-                },
-                "Max": {
-                    "documentation": "<p>The maximum of the values of the all data points collected during the period.</p>",
-                    "shape": "Max"
-                },
-                "Min": {
-                    "documentation": "<p>The minimum of the values of the all data points collected during the period.</p>",
-                    "shape": "Min"
-                },
-                "P90": {
-                    "documentation": "<p>The 90th percentile of the values of the all data points collected during the period.</p>",
-                    "shape": "P90"
-                },
-                "Std": {
-                    "documentation": "<p>The standard deviation of the values of the all data points collected during the period.</p>",
-                    "shape": "Std"
-                },
-                "Sum": {
-                    "documentation": "<p>The sum of the values of the all data points collected during the period.</p>",
-                    "shape": "Sum"
-                }
-            },
-            "type": "structure"
-        },
-        "MetricQueryValues": {
-            "member": {
-                "shape": "MetricQueryValue"
-            },
-            "type": "list"
-        },
-        "MetricUnit": {
-            "max": 256,
-            "type": "string"
-        },
-        "Min": {
-            "type": "double"
-        },
         "MinGwDiversity": {
             "max": 100,
             "min": 1,
             "type": "integer"
         },
         "Model": {
             "max": 4096,
@@ -8826,27 +8535,27 @@
         "OnboardStatusReason": {
             "type": "string"
         },
         "OtaaV1_0_x": {
             "documentation": "<p>OTAA device object for v1.0.x</p>",
             "members": {
                 "AppEui": {
-                    "documentation": "<p>The AppEUI value. You specify this value when using LoRaWAN versions v1.0.2 or v1.0.3.</p>",
+                    "documentation": "<p>The AppEUI value.</p>",
                     "shape": "AppEui"
                 },
                 "AppKey": {
                     "documentation": "<p>The AppKey value.</p>",
                     "shape": "AppKey"
                 },
                 "GenAppKey": {
                     "documentation": "<p>The GenAppKey value.</p>",
                     "shape": "GenAppKey"
                 },
                 "JoinEui": {
-                    "documentation": "<p>The JoinEUI value. You specify this value instead of the AppEUI when using LoRaWAN version v1.0.4.</p>",
+                    "documentation": "<p>The JoinEUI value.</p>",
                     "shape": "JoinEui"
                 }
             },
             "type": "structure"
         },
         "OtaaV1_1": {
             "documentation": "<p>OTAA device object for v1.1</p>",
@@ -8862,17 +8571,14 @@
                 "NwkKey": {
                     "documentation": "<p>The NwkKey value.</p>",
                     "shape": "NwkKey"
                 }
             },
             "type": "structure"
         },
-        "P90": {
-            "type": "double"
-        },
         "PCI": {
             "max": 503,
             "min": 0,
             "type": "integer"
         },
         "PSC": {
             "max": 511,
@@ -9981,17 +9687,14 @@
             "max": 4096,
             "min": 1,
             "type": "string"
         },
         "StatusReason": {
             "type": "string"
         },
-        "Std": {
-            "type": "double"
-        },
         "SubBand": {
             "documentation": "<p>A subset of supported frequency channels in a certain RFRegion.</p>",
             "max": 8,
             "min": 1,
             "type": "integer"
         },
         "SubBands": {
@@ -9999,126 +9702,14 @@
             "max": 8,
             "member": {
                 "shape": "SubBand"
             },
             "min": 0,
             "type": "list"
         },
-        "Sum": {
-            "type": "double"
-        },
-        "SummaryMetricConfiguration": {
-            "documentation": "<p>The configuration of summary metric.</p>",
-            "members": {
-                "Status": {
-                    "documentation": "<p>The configuration of summary metric.</p>",
-                    "shape": "SummaryMetricConfigurationStatus"
-                }
-            },
-            "type": "structure"
-        },
-        "SummaryMetricConfigurationStatus": {
-            "enum": [
-                "Enabled",
-                "Disabled"
-            ],
-            "type": "string"
-        },
-        "SummaryMetricQueries": {
-            "member": {
-                "shape": "SummaryMetricQuery"
-            },
-            "type": "list"
-        },
-        "SummaryMetricQuery": {
-            "documentation": "<p>The metric query object.</p>",
-            "members": {
-                "AggregationPeriod": {
-                    "documentation": "<p>The aggregation period of the metric.</p>",
-                    "shape": "AggregationPeriod"
-                },
-                "Dimensions": {
-                    "documentation": "<p>The dimensions of the metric.</p>",
-                    "shape": "Dimensions"
-                },
-                "EndTimestamp": {
-                    "documentation": "<p>The end timestamp for summary metric query.</p>",
-                    "shape": "MetricQueryEndTimestamp"
-                },
-                "MetricName": {
-                    "documentation": "<p>The name of the metric.</p>",
-                    "shape": "MetricName"
-                },
-                "QueryId": {
-                    "documentation": "<p>The id of the query.</p>",
-                    "shape": "MetricQueryId"
-                },
-                "StartTimestamp": {
-                    "documentation": "<p>The start timestamp for summary metric query.</p>",
-                    "shape": "MetricQueryStartTimestamp"
-                }
-            },
-            "type": "structure"
-        },
-        "SummaryMetricQueryResult": {
-            "documentation": "<p>The result of metrics aggregation operation.</p>",
-            "members": {
-                "AggregationPeriod": {
-                    "documentation": "<p>The aggregation period of the metric.</p>",
-                    "shape": "AggregationPeriod"
-                },
-                "Dimensions": {
-                    "documentation": "<p>The dimensions of the metric.</p>",
-                    "shape": "Dimensions"
-                },
-                "EndTimestamp": {
-                    "documentation": "<p>The end timestamp for summary metric query.</p>",
-                    "shape": "MetricQueryEndTimestamp"
-                },
-                "Error": {
-                    "documentation": "<p>The error message for the summary metric query.</p>",
-                    "shape": "MetricQueryError"
-                },
-                "MetricName": {
-                    "documentation": "<p>The name of the metric.</p>",
-                    "shape": "MetricName"
-                },
-                "QueryId": {
-                    "documentation": "<p>The id of the query.</p>",
-                    "shape": "MetricQueryId"
-                },
-                "QueryStatus": {
-                    "documentation": "<p>The status of the metric query.</p>",
-                    "shape": "MetricQueryStatus"
-                },
-                "StartTimestamp": {
-                    "documentation": "<p>The start timestamp for summary metric query.</p>",
-                    "shape": "MetricQueryStartTimestamp"
-                },
-                "Timestamps": {
-                    "documentation": "<p>The timestamp of each aggregation result.</p>",
-                    "shape": "MetricQueryTimestamps"
-                },
-                "Unit": {
-                    "documentation": "<p>The units of measurement to be used for interpreting the aggregation result.</p>",
-                    "shape": "MetricUnit"
-                },
-                "Values": {
-                    "documentation": "<p>The list of aggregated metrics.</p>",
-                    "shape": "MetricQueryValues"
-                }
-            },
-            "type": "structure"
-        },
-        "SummaryMetricQueryResults": {
-            "member": {
-                "shape": "SummaryMetricQueryResult"
-            },
-            "type": "list"
-        },
         "SupportedRfRegion": {
             "documentation": "<p>Supported RfRegions</p>",
             "enum": [
                 "EU868",
                 "US915",
                 "AU915",
                 "AS923-1",
@@ -10635,27 +10226,14 @@
             },
             "type": "structure"
         },
         "UpdateLogLevelsByResourceTypesResponse": {
             "members": {},
             "type": "structure"
         },
-        "UpdateMetricConfigurationRequest": {
-            "members": {
-                "SummaryMetric": {
-                    "documentation": "<p>The value to be used to set summary metric configuration.</p>",
-                    "shape": "SummaryMetricConfiguration"
-                }
-            },
-            "type": "structure"
-        },
-        "UpdateMetricConfigurationResponse": {
-            "members": {},
-            "type": "structure"
-        },
         "UpdateMulticastGroupRequest": {
             "members": {
                 "Description": {
                     "shape": "Description"
                 },
                 "Id": {
                     "location": "uri",
```

### Comparing `botocore-a-la-carte-iotwireless-1.34.83/botocore_a_la_carte_iotwireless.egg-info/PKG-INFO` & `botocore-a-la-carte-iotwireless-1.34.9/botocore_a_la_carte_iotwireless.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-iotwireless
-Version: 1.34.83
+Version: 1.34.9
 Summary: iotwireless data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-iotwireless-1.34.83/setup.py` & `botocore-a-la-carte-iotwireless-1.34.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-iotwireless',
-    version="1.34.83",
+    version="1.34.9",
     description='iotwireless data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/iotwireless/*/*.json'],
```

