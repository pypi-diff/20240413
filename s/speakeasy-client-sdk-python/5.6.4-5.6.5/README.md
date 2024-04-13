# Comparing `tmp/speakeasy-client-sdk-python-5.6.4.tar.gz` & `tmp/speakeasy-client-sdk-python-5.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speakeasy-client-sdk-python-5.6.4.tar", last modified: Tue Apr  9 00:13:09 2024, max compression
+gzip compressed data, was "speakeasy-client-sdk-python-5.6.5.tar", last modified: Fri Apr 12 00:14:09 2024, max compression
```

## Comparing `speakeasy-client-sdk-python-5.6.4.tar` & `speakeasy-client-sdk-python-5.6.5.tar`

### file list

```diff
@@ -1,111 +1,120 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:13:09.016119 speakeasy-client-sdk-python-5.6.4/
--rw-r--r--   0 runner    (1001) docker     (127)    20475 2024-04-09 00:13:09.016119 speakeasy-client-sdk-python-5.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13565 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 00:13:09.016119 speakeasy-client-sdk-python-5.6.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:13:09.000119 speakeasy-client-sdk-python-5.6.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:13:09.000119 speakeasy-client-sdk-python-5.6.4/src/speakeasy/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:13:09.004119 speakeasy-client-sdk-python-5.6.4/src/speakeasy/_hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/_hooks/registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/_hooks/sdkhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/_hooks/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    28727 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/apiendpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)    21661 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)    13757 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    10349 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/embeds.py
--rw-r--r--   0 runner    (1001) docker     (127)    12566 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/events.py
--rw-r--r--   0 runner    (1001) docker     (127)    10618 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:13:09.004119 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:13:09.004119 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/errors/error.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/errors/sdkerror.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:13:09.004119 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/internal/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/internal/globals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:13:09.008119 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/
--rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/deleteapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/deleteapiendpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/deleteschema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/deleteversionmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/downloadschema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/downloadschemarevision.py
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/findapiendpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/generateopenapispec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/generateopenapispecforapiendpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/generatepostmancollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/generatepostmancollectionforapiendpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/generaterequestpostmancollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getaccesstoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getallapiendpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getallapiversions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getallforversionapiendpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getapiendpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getapis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getembedaccesstoken.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getorganizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getrequestfromeventlog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getschema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getschemadiff.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getschemarevision.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getschemas.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getuser.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getvalidembedaccesstokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getversionmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getworkspaceaccess.py
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getworkspaceevents.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getworkspacetargets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/insertversionmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/postworkspaceevents.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/queryeventlog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/registerschema.py
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/revokeembedaccesstoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/upsertapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/upsertapiendpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/validateapikey.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:13:09.012119 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/accessdetails.py
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/accesstoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/api_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/apiendpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/apiendpoint_input.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/apikeydetails.py
--rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/boundedrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)    13210 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/clievent.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/embedaccesstokenresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/embedtoken.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/filter_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/generateopenapispecdiff.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/interactiontype.py
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/organization.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/requestmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/schemadiff.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/security.py
--rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/targetsdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/unboundedrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/versionmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/versionmetadata_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/organizations.py
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)    28253 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/sdkconfiguration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:13:09.012119 speakeasy-client-sdk-python-5.6.4/src/speakeasy/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/utils/retries.py
--rw-r--r--   0 runner    (1001) docker     (127)    32089 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:13:09.016119 speakeasy-client-sdk-python-5.6.4/src/speakeasy_client_sdk_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20475 2024-04-09 00:13:08.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy_client_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-04-09 00:13:08.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy_client_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 00:13:08.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy_client_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-09 00:13:08.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy_client_sdk_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-09 00:13:08.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy_client_sdk_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:14:09.110529 speakeasy-client-sdk-python-5.6.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    21158 2024-04-12 00:14:09.110529 speakeasy-client-sdk-python-5.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13908 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 00:14:09.114529 speakeasy-client-sdk-python-5.6.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:14:09.094529 speakeasy-client-sdk-python-5.6.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:14:09.098528 speakeasy-client-sdk-python-5.6.5/src/speakeasy/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:14:09.098528 speakeasy-client-sdk-python-5.6.5/src/speakeasy/_hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/_hooks/registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/_hooks/sdkhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/_hooks/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28727 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/apiendpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21661 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10253 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13757 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10349 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/embeds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12566 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10618 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:14:09.098528 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:14:09.098528 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/errors/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/errors/sdkerror.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:14:09.098528 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/internal/globals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:14:09.106529 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/deleteapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/deleteapiendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/deleteschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/deleteversionmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/downloadschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/downloadschemarevision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/findapiendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/generateopenapispec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/generateopenapispecforapiendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/generatepostmancollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/generatepostmancollectionforapiendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/generaterequestpostmancollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/getaccesstoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/getallapiendpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/getallapiversions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/getallforversionapiendpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/getapiendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/getapis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/getembedaccesstoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/getnamespaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/getorganizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/getrequestfromeventlog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/getrevisions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/getschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/getschemadiff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/getschemarevision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/getschemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/getuser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/getvalidembedaccesstokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/getversionmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/getworkspaceaccess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/getworkspaceevents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/getworkspacetargets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/insertversionmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/postworkspaceevents.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/preflight.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/queryeventlog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/registerschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/revokeembedaccesstoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/upsertapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/upsertapiendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/validateapikey.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:14:09.110529 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/shared/accessdetails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/shared/accesstoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/shared/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/shared/api_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/shared/apiendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/shared/apiendpoint_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/shared/apikeydetails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/shared/boundedrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13210 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/shared/clievent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/shared/embedaccesstokenresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/shared/embedtoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/shared/filter_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/shared/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/shared/generateopenapispecdiff.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/shared/getnamespacesresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/shared/getrevisionsresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/shared/interactiontype.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/shared/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/shared/organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/shared/preflighttoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/shared/requestmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/shared/revision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/shared/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/shared/schemadiff.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/shared/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/shared/targetsdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/shared/unboundedrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/shared/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/shared/versionmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/shared/versionmetadata_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28253 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4457 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/sdkconfiguration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:14:09.110529 speakeasy-client-sdk-python-5.6.5/src/speakeasy/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/utils/retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32089 2024-04-12 00:14:00.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:14:09.110529 speakeasy-client-sdk-python-5.6.5/src/speakeasy_client_sdk_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21158 2024-04-12 00:14:08.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy_client_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-04-12 00:14:09.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy_client_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 00:14:08.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy_client_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-12 00:14:08.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy_client_sdk_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-12 00:14:08.000000 speakeasy-client-sdk-python-5.6.5/src/speakeasy_client_sdk_python.egg-info/top_level.txt
```

### Comparing `speakeasy-client-sdk-python-5.6.4/PKG-INFO` & `speakeasy-client-sdk-python-5.6.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speakeasy-client-sdk-python
-Version: 5.6.4
+Version: 5.6.5
 Summary: Speakeasy API Client SDK for Python
 Home-page: https://github.com/speakeasy-api/speakeasy-client-sdk-python.git
 Author: Speakeasy
 License: UNKNOWN
 Description: # speakeasy-client-sdk-python
         
         <!-- Start SDK Installation [installation] -->
@@ -78,14 +78,20 @@
         * [download_schema_revision](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/schemas/README.md#download_schema_revision) - Download a particular schema revision for an Api.
         * [get_schema](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/schemas/README.md#get_schema) - Get information about the latest schema.
         * [get_schema_diff](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/schemas/README.md#get_schema_diff) - Get a diff of two schema revisions for an Api.
         * [get_schema_revision](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/schemas/README.md#get_schema_revision) - Get information about a particular schema revision for an Api.
         * [get_schemas](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/schemas/README.md#get_schemas) - Get information about all schemas associated with a particular apiID.
         * [register_schema](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/schemas/README.md#register_schema) - Register a schema.
         
+        ### [artifacts](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/artifacts/README.md)
+        
+        * [get_namespaces](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/artifacts/README.md#get_namespaces) - Each namespace contains many revisions.
+        * [get_revisions](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/artifacts/README.md#get_revisions)
+        * [preflight](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/artifacts/README.md#preflight) - Get access token for communicating with OCI distribution endpoints
+        
         ### [auth](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/auth/README.md)
         
         * [get_access_token](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/auth/README.md#get_access_token) - Get or refresh an access token for the current workspace.
         * [get_user](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/auth/README.md#get_user) - Get information about the current user.
         * [get_workspace_access](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/auth/README.md#get_workspace_access) - Get access allowances for a particular workspace
         * [validate_api_key](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/auth/README.md#validate_api_key) - Validate the current api key.
```

### Comparing `speakeasy-client-sdk-python-5.6.4/README.md` & `speakeasy-client-sdk-python-5.6.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -71,14 +71,20 @@
 * [download_schema_revision](docs/sdks/schemas/README.md#download_schema_revision) - Download a particular schema revision for an Api.
 * [get_schema](docs/sdks/schemas/README.md#get_schema) - Get information about the latest schema.
 * [get_schema_diff](docs/sdks/schemas/README.md#get_schema_diff) - Get a diff of two schema revisions for an Api.
 * [get_schema_revision](docs/sdks/schemas/README.md#get_schema_revision) - Get information about a particular schema revision for an Api.
 * [get_schemas](docs/sdks/schemas/README.md#get_schemas) - Get information about all schemas associated with a particular apiID.
 * [register_schema](docs/sdks/schemas/README.md#register_schema) - Register a schema.
 
+### [artifacts](docs/sdks/artifacts/README.md)
+
+* [get_namespaces](docs/sdks/artifacts/README.md#get_namespaces) - Each namespace contains many revisions.
+* [get_revisions](docs/sdks/artifacts/README.md#get_revisions)
+* [preflight](docs/sdks/artifacts/README.md#preflight) - Get access token for communicating with OCI distribution endpoints
+
 ### [auth](docs/sdks/auth/README.md)
 
 * [get_access_token](docs/sdks/auth/README.md#get_access_token) - Get or refresh an access token for the current workspace.
 * [get_user](docs/sdks/auth/README.md#get_user) - Get information about the current user.
 * [get_workspace_access](docs/sdks/auth/README.md#get_workspace_access) - Get access allowances for a particular workspace
 * [validate_api_key](docs/sdks/auth/README.md#validate_api_key) - Validate the current api key.
```

### Comparing `speakeasy-client-sdk-python-5.6.4/setup.py` & `speakeasy-client-sdk-python-5.6.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             long_description,
         )
 except FileNotFoundError:
     long_description = ''
 
 setuptools.setup(
     name='speakeasy-client-sdk-python',
-    version='5.6.4',
+    version='5.6.5',
     author='Speakeasy',
     description='Speakeasy API Client SDK for Python',
     url='https://github.com/speakeasy-api/speakeasy-client-sdk-python.git',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(where='src'),
     install_requires=[
```

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/_hooks/registration.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/_hooks/registration.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/_hooks/sdkhooks.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/_hooks/sdkhooks.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/_hooks/types.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/_hooks/types.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/apiendpoints.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/apiendpoints.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/apis.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/apis.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/auth.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/auth.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/embeds.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/embeds.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/events.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/events.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/metadata.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/metadata.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/errors/error.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/errors/error.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/errors/sdkerror.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/errors/sdkerror.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/__init__.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,29 +15,32 @@
 from .getaccesstoken import *
 from .getallapiendpoints import *
 from .getallapiversions import *
 from .getallforversionapiendpoints import *
 from .getapiendpoint import *
 from .getapis import *
 from .getembedaccesstoken import *
+from .getnamespaces import *
 from .getorganizations import *
 from .getrequestfromeventlog import *
+from .getrevisions import *
 from .getschema import *
 from .getschemadiff import *
 from .getschemarevision import *
 from .getschemas import *
 from .getuser import *
 from .getvalidembedaccesstokens import *
 from .getversionmetadata import *
 from .getworkspaceaccess import *
 from .getworkspaceevents import *
 from .getworkspacetargets import *
 from .insertversionmetadata import *
 from .postworkspaceevents import *
+from .preflight import *
 from .queryeventlog import *
 from .registerschema import *
 from .revokeembedaccesstoken import *
 from .upsertapi import *
 from .upsertapiendpoint import *
 from .validateapikey import *
 
-__all__ = ["DeleteAPIEndpointRequest","DeleteAPIEndpointResponse","DeleteAPIRequest","DeleteAPIResponse","DeleteSchemaRequest","DeleteSchemaResponse","DeleteVersionMetadataRequest","DeleteVersionMetadataResponse","DownloadSchemaRequest","DownloadSchemaResponse","DownloadSchemaRevisionRequest","DownloadSchemaRevisionResponse","File","FindAPIEndpointRequest","FindAPIEndpointResponse","GenerateOpenAPISpecForAPIEndpointRequest","GenerateOpenAPISpecForAPIEndpointResponse","GenerateOpenAPISpecRequest","GenerateOpenAPISpecResponse","GeneratePostmanCollectionForAPIEndpointRequest","GeneratePostmanCollectionForAPIEndpointResponse","GeneratePostmanCollectionRequest","GeneratePostmanCollectionResponse","GenerateRequestPostmanCollectionRequest","GenerateRequestPostmanCollectionResponse","GetAPIEndpointRequest","GetAPIEndpointResponse","GetAccessTokenRequest","GetAccessTokenResponse","GetAllAPIEndpointsRequest","GetAllAPIEndpointsResponse","GetAllAPIVersionsRequest","GetAllAPIVersionsResponse","GetAllForVersionAPIEndpointsRequest","GetAllForVersionAPIEndpointsResponse","GetApisRequest","GetApisResponse","GetEmbedAccessTokenRequest","GetEmbedAccessTokenResponse","GetOrganizationsResponse","GetRequestFromEventLogRequest","GetRequestFromEventLogResponse","GetSchemaDiffRequest","GetSchemaDiffResponse","GetSchemaRequest","GetSchemaResponse","GetSchemaRevisionRequest","GetSchemaRevisionResponse","GetSchemasRequest","GetSchemasResponse","GetUserResponse","GetValidEmbedAccessTokensResponse","GetVersionMetadataRequest","GetVersionMetadataResponse","GetWorkspaceAccessRequest","GetWorkspaceAccessResponse","GetWorkspaceEventsGlobals","GetWorkspaceEventsRequest","GetWorkspaceEventsResponse","GetWorkspaceTargetsGlobals","GetWorkspaceTargetsRequest","GetWorkspaceTargetsResponse","InsertVersionMetadataRequest","InsertVersionMetadataResponse","Op","PostWorkspaceEventsGlobals","PostWorkspaceEventsRequest","PostWorkspaceEventsResponse","QueryEventLogRequest","QueryEventLogResponse","QueryParamOp","RegisterSchemaRequest","RegisterSchemaRequestBody","RegisterSchemaResponse","RevokeEmbedAccessTokenRequest","RevokeEmbedAccessTokenResponse","UpsertAPIEndpointRequest","UpsertAPIEndpointResponse","UpsertAPIRequest","UpsertAPIResponse","ValidateAPIKeyResponse"]
+__all__ = ["DeleteAPIEndpointRequest","DeleteAPIEndpointResponse","DeleteAPIRequest","DeleteAPIResponse","DeleteSchemaRequest","DeleteSchemaResponse","DeleteVersionMetadataRequest","DeleteVersionMetadataResponse","DownloadSchemaRequest","DownloadSchemaResponse","DownloadSchemaRevisionRequest","DownloadSchemaRevisionResponse","File","FindAPIEndpointRequest","FindAPIEndpointResponse","GenerateOpenAPISpecForAPIEndpointRequest","GenerateOpenAPISpecForAPIEndpointResponse","GenerateOpenAPISpecRequest","GenerateOpenAPISpecResponse","GeneratePostmanCollectionForAPIEndpointRequest","GeneratePostmanCollectionForAPIEndpointResponse","GeneratePostmanCollectionRequest","GeneratePostmanCollectionResponse","GenerateRequestPostmanCollectionRequest","GenerateRequestPostmanCollectionResponse","GetAPIEndpointRequest","GetAPIEndpointResponse","GetAccessTokenRequest","GetAccessTokenResponse","GetAllAPIEndpointsRequest","GetAllAPIEndpointsResponse","GetAllAPIVersionsRequest","GetAllAPIVersionsResponse","GetAllForVersionAPIEndpointsRequest","GetAllForVersionAPIEndpointsResponse","GetApisRequest","GetApisResponse","GetEmbedAccessTokenRequest","GetEmbedAccessTokenResponse","GetNamespacesResponse","GetOrganizationsResponse","GetRequestFromEventLogRequest","GetRequestFromEventLogResponse","GetRevisionsRequest","GetRevisionsResponse","GetSchemaDiffRequest","GetSchemaDiffResponse","GetSchemaRequest","GetSchemaResponse","GetSchemaRevisionRequest","GetSchemaRevisionResponse","GetSchemasRequest","GetSchemasResponse","GetUserResponse","GetValidEmbedAccessTokensResponse","GetVersionMetadataRequest","GetVersionMetadataResponse","GetWorkspaceAccessRequest","GetWorkspaceAccessResponse","GetWorkspaceEventsGlobals","GetWorkspaceEventsRequest","GetWorkspaceEventsResponse","GetWorkspaceTargetsGlobals","GetWorkspaceTargetsRequest","GetWorkspaceTargetsResponse","InsertVersionMetadataRequest","InsertVersionMetadataResponse","Op","PostWorkspaceEventsGlobals","PostWorkspaceEventsRequest","PostWorkspaceEventsResponse","PreflightResponse","QueryEventLogRequest","QueryEventLogResponse","QueryParamOp","RegisterSchemaRequest","RegisterSchemaRequestBody","RegisterSchemaResponse","RevokeEmbedAccessTokenRequest","RevokeEmbedAccessTokenResponse","UpsertAPIEndpointRequest","UpsertAPIEndpointResponse","UpsertAPIRequest","UpsertAPIResponse","ValidateAPIKeyResponse"]
```

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/deleteapi.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/deleteapi.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/deleteapiendpoint.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/deleteapiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/deleteschema.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/deleteschema.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/deleteversionmetadata.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/deleteversionmetadata.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/downloadschema.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/downloadschema.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/downloadschemarevision.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/downloadschemarevision.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/findapiendpoint.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/findapiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/generateopenapispec.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/generateopenapispec.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/generateopenapispecforapiendpoint.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/generateopenapispecforapiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/generatepostmancollection.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/generatepostmancollection.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/generatepostmancollectionforapiendpoint.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/generatepostmancollectionforapiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/generaterequestpostmancollection.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/generaterequestpostmancollection.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getaccesstoken.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/getaccesstoken.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getallapiendpoints.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/getallapiendpoints.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getallapiversions.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/getallapiversions.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getallforversionapiendpoints.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/getallforversionapiendpoints.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getapiendpoint.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/getapiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getapis.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/getapis.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getembedaccesstoken.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/getembedaccesstoken.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getorganizations.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/getorganizations.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getrequestfromeventlog.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/getrequestfromeventlog.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getschema.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/getschema.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getschemadiff.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/getschemadiff.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getschemarevision.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/getschemarevision.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getschemas.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/getschemas.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getuser.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/getuser.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getvalidembedaccesstokens.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/getvalidembedaccesstokens.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getversionmetadata.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/getversionmetadata.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getworkspaceaccess.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/getworkspaceaccess.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getworkspaceevents.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/getworkspaceevents.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getworkspacetargets.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/getworkspacetargets.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/insertversionmetadata.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/insertversionmetadata.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/postworkspaceevents.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/postworkspaceevents.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/queryeventlog.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/queryeventlog.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/registerschema.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/registerschema.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/revokeembedaccesstoken.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/revokeembedaccesstoken.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/upsertapi.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/upsertapi.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/upsertapiendpoint.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/upsertapiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/validateapikey.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/operations/validateapikey.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/__init__.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/shared/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,20 +10,25 @@
 from .boundedrequest import *
 from .clievent import *
 from .embedaccesstokenresponse import *
 from .embedtoken import *
 from .filter_ import *
 from .filters import *
 from .generateopenapispecdiff import *
+from .getnamespacesresponse import *
+from .getrevisionsresponse import *
 from .interactiontype import *
+from .namespace import *
 from .organization import *
+from .preflighttoken import *
 from .requestmetadata import *
+from .revision import *
 from .schema import *
 from .schemadiff import *
 from .security import *
 from .targetsdk import *
 from .unboundedrequest import *
 from .user import *
 from .versionmetadata import *
 from .versionmetadata_input import *
 
-__all__ = ["API","APIEndpoint","APIEndpointInput","APIInput","APIKeyDetails","AccessDetails","AccessToken","AccessTokenUser","AccountType","BoundedRequest","Claims","CliEvent","EmbedAccessTokenResponse","EmbedToken","Filter","Filters","GenerateBumpType","GenerateOpenAPISpecDiff","InteractionType","Level","Organization","OrganizationAccountType","RequestMetadata","Schema","SchemaDiff","Security","TargetSDK","UnboundedRequest","User","ValueChange","VersionMetadata","VersionMetadataInput","Workspaces"]
+__all__ = ["API","APIEndpoint","APIEndpointInput","APIInput","APIKeyDetails","AccessDetails","AccessToken","AccessTokenUser","AccountType","BoundedRequest","Claims","CliEvent","EmbedAccessTokenResponse","EmbedToken","Filter","Filters","GenerateBumpType","GenerateOpenAPISpecDiff","GetNamespacesResponse","GetRevisionsResponse","InteractionType","Level","Namespace","Organization","OrganizationAccountType","PreflightToken","RequestMetadata","Revision","Schema","SchemaDiff","Security","TargetSDK","UnboundedRequest","User","ValueChange","VersionMetadata","VersionMetadataInput","Workspaces"]
```

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/accessdetails.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/shared/accessdetails.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/accesstoken.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/shared/accesstoken.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/api.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/shared/api.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/api_input.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/shared/api_input.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/apiendpoint.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/shared/apiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/apiendpoint_input.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/shared/apiendpoint_input.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/apikeydetails.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/shared/apikeydetails.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/boundedrequest.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/shared/boundedrequest.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/clievent.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/shared/clievent.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/embedaccesstokenresponse.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/shared/embedaccesstokenresponse.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/embedtoken.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/shared/embedtoken.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/filter_.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/shared/filter_.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/filters.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/shared/filters.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/generateopenapispecdiff.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/shared/generateopenapispecdiff.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/organization.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/shared/organization.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/requestmetadata.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/shared/requestmetadata.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/schema.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/shared/schema.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/schemadiff.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/shared/schemadiff.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/security.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/shared/security.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/targetsdk.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/shared/targetsdk.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/unboundedrequest.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/shared/unboundedrequest.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/user.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/shared/user.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/versionmetadata.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/shared/versionmetadata.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/versionmetadata_input.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/models/shared/versionmetadata_input.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/organizations.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/organizations.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/requests.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/requests.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/schemas.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/schemas.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/sdk.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/sdk.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .apiendpoints import APIEndpoints
 from .apis import Apis
+from .artifacts import Artifacts
 from .auth import Auth
 from .embeds import Embeds
 from .events import Events
 from .metadata import Metadata
 from .organizations import Organizations
 from .requests import Requests
 from .schemas import Schemas
@@ -25,14 +26,15 @@
     r"""REST APIs for managing Api entities"""
     api_endpoints: APIEndpoints
     r"""REST APIs for managing ApiEndpoint entities"""
     metadata: Metadata
     r"""REST APIs for managing Version Metadata entities"""
     schemas: Schemas
     r"""REST APIs for managing Schema entities"""
+    artifacts: Artifacts
     auth: Auth
     r"""REST APIs for managing Authentication"""
     requests: Requests
     r"""REST APIs for retrieving request information"""
     organizations: Organizations
     embeds: Embeds
     r"""REST APIs for managing embeds"""
@@ -101,12 +103,13 @@
 
 
     def _init_sdks(self):
         self.apis = Apis(self.sdk_configuration)
         self.api_endpoints = APIEndpoints(self.sdk_configuration)
         self.metadata = Metadata(self.sdk_configuration)
         self.schemas = Schemas(self.sdk_configuration)
+        self.artifacts = Artifacts(self.sdk_configuration)
         self.auth = Auth(self.sdk_configuration)
         self.requests = Requests(self.sdk_configuration)
         self.organizations = Organizations(self.sdk_configuration)
         self.embeds = Embeds(self.sdk_configuration)
         self.events = Events(self.sdk_configuration)
```

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/sdkconfiguration.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/sdkconfiguration.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,17 +22,17 @@
     client: requests_http.Session
     globals: internal.Globals
     security: Union[shared.Security,Callable[[], shared.Security]] = None
     server_url: Optional[str] = ''
     server: Optional[str] = ''
     language: str = 'python'
     openapi_doc_version: str = '0.4.0'
-    sdk_version: str = '5.6.4'
-    gen_version: str = '2.301.0'
-    user_agent: str = 'speakeasy-sdk/python 5.6.4 2.301.0 0.4.0 speakeasy-client-sdk-python'
+    sdk_version: str = '5.6.5'
+    gen_version: str = '2.304.1'
+    user_agent: str = 'speakeasy-sdk/python 5.6.5 2.304.1 0.4.0 speakeasy-client-sdk-python'
     retry_config: Optional[RetryConfig] = None
 
     def __post_init__(self):
         self._hooks = SDKHooks()
 
     def get_server_details(self) -> Tuple[str, Dict[str, str]]:
         if self.server_url is not None and self.server_url != '':
```

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/utils/retries.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/utils/retries.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy/utils/utils.py` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy/utils/utils.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy_client_sdk_python.egg-info/PKG-INFO` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy_client_sdk_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speakeasy-client-sdk-python
-Version: 5.6.4
+Version: 5.6.5
 Summary: Speakeasy API Client SDK for Python
 Home-page: https://github.com/speakeasy-api/speakeasy-client-sdk-python.git
 Author: Speakeasy
 License: UNKNOWN
 Description: # speakeasy-client-sdk-python
         
         <!-- Start SDK Installation [installation] -->
@@ -78,14 +78,20 @@
         * [download_schema_revision](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/schemas/README.md#download_schema_revision) - Download a particular schema revision for an Api.
         * [get_schema](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/schemas/README.md#get_schema) - Get information about the latest schema.
         * [get_schema_diff](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/schemas/README.md#get_schema_diff) - Get a diff of two schema revisions for an Api.
         * [get_schema_revision](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/schemas/README.md#get_schema_revision) - Get information about a particular schema revision for an Api.
         * [get_schemas](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/schemas/README.md#get_schemas) - Get information about all schemas associated with a particular apiID.
         * [register_schema](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/schemas/README.md#register_schema) - Register a schema.
         
+        ### [artifacts](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/artifacts/README.md)
+        
+        * [get_namespaces](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/artifacts/README.md#get_namespaces) - Each namespace contains many revisions.
+        * [get_revisions](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/artifacts/README.md#get_revisions)
+        * [preflight](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/artifacts/README.md#preflight) - Get access token for communicating with OCI distribution endpoints
+        
         ### [auth](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/auth/README.md)
         
         * [get_access_token](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/auth/README.md#get_access_token) - Get or refresh an access token for the current workspace.
         * [get_user](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/auth/README.md#get_user) - Get information about the current user.
         * [get_workspace_access](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/auth/README.md#get_workspace_access) - Get access allowances for a particular workspace
         * [validate_api_key](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/auth/README.md#validate_api_key) - Validate the current api key.
```

### Comparing `speakeasy-client-sdk-python-5.6.4/src/speakeasy_client_sdk_python.egg-info/SOURCES.txt` & `speakeasy-client-sdk-python-5.6.5/src/speakeasy_client_sdk_python.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 README.md
 setup.py
 src/speakeasy/__init__.py
 src/speakeasy/apiendpoints.py
 src/speakeasy/apis.py
+src/speakeasy/artifacts.py
 src/speakeasy/auth.py
 src/speakeasy/embeds.py
 src/speakeasy/events.py
 src/speakeasy/metadata.py
 src/speakeasy/organizations.py
 src/speakeasy/requests.py
 src/speakeasy/schemas.py
@@ -38,28 +39,31 @@
 src/speakeasy/models/operations/getaccesstoken.py
 src/speakeasy/models/operations/getallapiendpoints.py
 src/speakeasy/models/operations/getallapiversions.py
 src/speakeasy/models/operations/getallforversionapiendpoints.py
 src/speakeasy/models/operations/getapiendpoint.py
 src/speakeasy/models/operations/getapis.py
 src/speakeasy/models/operations/getembedaccesstoken.py
+src/speakeasy/models/operations/getnamespaces.py
 src/speakeasy/models/operations/getorganizations.py
 src/speakeasy/models/operations/getrequestfromeventlog.py
+src/speakeasy/models/operations/getrevisions.py
 src/speakeasy/models/operations/getschema.py
 src/speakeasy/models/operations/getschemadiff.py
 src/speakeasy/models/operations/getschemarevision.py
 src/speakeasy/models/operations/getschemas.py
 src/speakeasy/models/operations/getuser.py
 src/speakeasy/models/operations/getvalidembedaccesstokens.py
 src/speakeasy/models/operations/getversionmetadata.py
 src/speakeasy/models/operations/getworkspaceaccess.py
 src/speakeasy/models/operations/getworkspaceevents.py
 src/speakeasy/models/operations/getworkspacetargets.py
 src/speakeasy/models/operations/insertversionmetadata.py
 src/speakeasy/models/operations/postworkspaceevents.py
+src/speakeasy/models/operations/preflight.py
 src/speakeasy/models/operations/queryeventlog.py
 src/speakeasy/models/operations/registerschema.py
 src/speakeasy/models/operations/revokeembedaccesstoken.py
 src/speakeasy/models/operations/upsertapi.py
 src/speakeasy/models/operations/upsertapiendpoint.py
 src/speakeasy/models/operations/validateapikey.py
 src/speakeasy/models/shared/__init__.py
@@ -73,17 +77,22 @@
 src/speakeasy/models/shared/boundedrequest.py
 src/speakeasy/models/shared/clievent.py
 src/speakeasy/models/shared/embedaccesstokenresponse.py
 src/speakeasy/models/shared/embedtoken.py
 src/speakeasy/models/shared/filter_.py
 src/speakeasy/models/shared/filters.py
 src/speakeasy/models/shared/generateopenapispecdiff.py
+src/speakeasy/models/shared/getnamespacesresponse.py
+src/speakeasy/models/shared/getrevisionsresponse.py
 src/speakeasy/models/shared/interactiontype.py
+src/speakeasy/models/shared/namespace.py
 src/speakeasy/models/shared/organization.py
+src/speakeasy/models/shared/preflighttoken.py
 src/speakeasy/models/shared/requestmetadata.py
+src/speakeasy/models/shared/revision.py
 src/speakeasy/models/shared/schema.py
 src/speakeasy/models/shared/schemadiff.py
 src/speakeasy/models/shared/security.py
 src/speakeasy/models/shared/targetsdk.py
 src/speakeasy/models/shared/unboundedrequest.py
 src/speakeasy/models/shared/user.py
 src/speakeasy/models/shared/versionmetadata.py
```

