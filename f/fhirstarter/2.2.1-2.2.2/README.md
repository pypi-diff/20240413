# Comparing `tmp/fhirstarter-2.2.1.tar.gz` & `tmp/fhirstarter-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fhirstarter-2.2.1.tar", max compression
+gzip compressed data, was "fhirstarter-2.2.2.tar", max compression
```

## Comparing `fhirstarter-2.2.1.tar` & `fhirstarter-2.2.2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0     1071 2023-09-17 03:53:46.172448 fhirstarter-2.2.1/LICENSE.md
--rw-r--r--   0        0        0     7650 2024-03-23 03:58:13.336858 fhirstarter-2.2.1/README.md
--rw-r--r--   0        0        0      618 2024-03-23 03:58:13.338365 fhirstarter-2.2.1/fhirstarter/__init__.py
--rw-r--r--   0        0        0        0 2023-09-20 03:13:49.647138 fhirstarter-2.2.1/fhirstarter/examples/__init__.py
--rw-r--r--   0        0        0      151 2024-03-19 15:17:26.545996 fhirstarter-2.2.1/fhirstarter/examples/config.toml
--rw-r--r--   0        0        0     5920 2024-03-23 16:52:35.690093 fhirstarter-2.2.1/fhirstarter/examples/example.py
--rw-r--r--   0        0        0     6289 2024-03-21 13:53:51.390759 fhirstarter-2.2.1/fhirstarter/exceptions.py
--rw-r--r--   0        0        0       92 2023-09-17 03:52:52.629289 fhirstarter-2.2.1/fhirstarter/fhir_specification/__init__.py
--rw-r--r--   0        0        0    10722 2024-03-21 13:53:51.392805 fhirstarter-2.2.1/fhirstarter/fhir_specification/scripts/create_sequence_data.py
--rw-r--r--   0        0        0        0 2023-09-02 19:22:45.000000 fhirstarter-2.2.1/fhirstarter/fhir_specification/sequences/R4/__init__.py
--rw-r--r--   0        0        0   392011 2023-09-19 05:19:49.123097 fhirstarter-2.2.1/fhirstarter/fhir_specification/sequences/R4/examples.zip
--rw-r--r--   0        0        0     2814 2023-09-17 03:53:25.323156 fhirstarter-2.2.1/fhirstarter/fhir_specification/sequences/R4/extra-search-parameters.json
--rw-r--r--   0        0        0     3334 2023-09-19 05:19:49.123371 fhirstarter-2.2.1/fhirstarter/fhir_specification/sequences/R4/resource_types.json
--rw-r--r--   0        0        0   113904 2023-09-19 05:19:49.126489 fhirstarter-2.2.1/fhirstarter/fhir_specification/sequences/R4/search-parameters.zip
--rw-r--r--   0        0        0        0 2023-09-02 19:22:45.000000 fhirstarter-2.2.1/fhirstarter/fhir_specification/sequences/R4B/__init__.py
--rw-r--r--   0        0        0   397649 2023-09-19 05:19:49.131072 fhirstarter-2.2.1/fhirstarter/fhir_specification/sequences/R4B/examples.zip
--rw-r--r--   0        0        0     1800 2023-09-17 03:53:25.323449 fhirstarter-2.2.1/fhirstarter/fhir_specification/sequences/R4B/extra-search-parameters.json
--rw-r--r--   0        0        0     3081 2023-09-19 05:19:49.131415 fhirstarter-2.2.1/fhirstarter/fhir_specification/sequences/R4B/resource_types.json
--rw-r--r--   0        0        0   117431 2023-09-19 05:19:49.134023 fhirstarter-2.2.1/fhirstarter/fhir_specification/sequences/R4B/search-parameters.zip
--rw-r--r--   0        0        0        0 2023-09-02 19:22:45.000000 fhirstarter-2.2.1/fhirstarter/fhir_specification/sequences/R5/__init__.py
--rw-r--r--   0        0        0   436165 2023-09-19 05:19:49.138801 fhirstarter-2.2.1/fhirstarter/fhir_specification/sequences/R5/examples.zip
--rw-r--r--   0        0        0     2356 2023-09-17 03:53:25.323792 fhirstarter-2.2.1/fhirstarter/fhir_specification/sequences/R5/extra-search-parameters.json
--rw-r--r--   0        0        0     3526 2023-09-19 05:19:49.141504 fhirstarter-2.2.1/fhirstarter/fhir_specification/sequences/R5/resource_types.json
--rw-r--r--   0        0        0   112399 2023-09-19 05:19:49.164799 fhirstarter-2.2.1/fhirstarter/fhir_specification/sequences/R5/search-parameters.zip
--rw-r--r--   0        0        0        0 2023-09-02 19:22:45.000000 fhirstarter-2.2.1/fhirstarter/fhir_specification/sequences/STU3/__init__.py
--rw-r--r--   0        0        0   361150 2023-09-19 05:19:49.169451 fhirstarter-2.2.1/fhirstarter/fhir_specification/sequences/STU3/examples.zip
--rw-r--r--   0        0        0     2624 2023-09-17 03:53:25.324061 fhirstarter-2.2.1/fhirstarter/fhir_specification/sequences/STU3/extra-search-parameters.json
--rw-r--r--   0        0        0     2416 2023-09-19 05:19:49.169722 fhirstarter-2.2.1/fhirstarter/fhir_specification/sequences/STU3/resource_types.json
--rw-r--r--   0        0        0    91155 2023-09-19 05:19:49.171719 fhirstarter-2.2.1/fhirstarter/fhir_specification/sequences/STU3/search-parameters.zip
--rw-r--r--   0        0        0       32 2023-09-17 03:52:52.629752 fhirstarter-2.2.1/fhirstarter/fhir_specification/sequences/__init__.py
--rw-r--r--   0        0        0     4692 2024-03-21 13:53:51.411033 fhirstarter-2.2.1/fhirstarter/fhir_specification/utils.py
--rw-r--r--   0        0        0    22399 2024-03-23 03:58:13.341116 fhirstarter-2.2.1/fhirstarter/fhirstarter.py
--rw-r--r--   0        0        0    20633 2024-03-23 03:58:13.342603 fhirstarter-2.2.1/fhirstarter/functions.py
--rw-r--r--   0        0        0     3354 2024-03-23 03:58:13.344738 fhirstarter-2.2.1/fhirstarter/interactions.py
--rw-r--r--   0        0        0     3135 2024-03-23 03:58:13.345906 fhirstarter-2.2.1/fhirstarter/json_patch.py
--rw-r--r--   0        0        0    10517 2024-03-23 03:58:13.347067 fhirstarter-2.2.1/fhirstarter/openapi.py
--rw-r--r--   0        0        0     7222 2024-03-23 03:58:13.348407 fhirstarter-2.2.1/fhirstarter/providers.py
--rw-r--r--   0        0        0     1691 2024-03-21 22:03:08.619634 fhirstarter-2.2.1/fhirstarter/resources.py
--rw-r--r--   0        0        0     6375 2024-03-21 13:53:51.421803 fhirstarter-2.2.1/fhirstarter/search_parameters.py
--rw-r--r--   0        0        0       68 2023-09-17 03:54:43.806486 fhirstarter-2.2.1/fhirstarter/testclient.py
--rw-r--r--   0        0        0        0 2023-09-02 19:22:45.000000 fhirstarter-2.2.1/fhirstarter/tests/__init__.py
--rw-r--r--   0        0        0     6330 2024-03-23 03:58:13.349705 fhirstarter-2.2.1/fhirstarter/tests/config.py
--rw-r--r--   0        0        0     1373 2024-03-23 03:58:13.350754 fhirstarter-2.2.1/fhirstarter/tests/conftest.py
--rw-r--r--   0        0        0     1500 2023-09-26 04:54:47.778966 fhirstarter-2.2.1/fhirstarter/tests/resources.py
--rw-r--r--   0        0        0     6667 2024-03-23 03:58:13.351831 fhirstarter-2.2.1/fhirstarter/tests/test_capability_statement.py
--rw-r--r--   0        0        0     3547 2024-03-21 13:53:51.427449 fhirstarter-2.2.1/fhirstarter/tests/test_dependencies.py
--rw-r--r--   0        0        0    10310 2024-03-23 03:58:13.372069 fhirstarter-2.2.1/fhirstarter/tests/test_errors.py
--rw-r--r--   0        0        0    14721 2024-03-23 03:58:13.373491 fhirstarter-2.2.1/fhirstarter/tests/test_interactions.py
--rw-r--r--   0        0        0    13703 2024-03-23 03:58:13.374911 fhirstarter-2.2.1/fhirstarter/tests/test_openapi.py
--rw-r--r--   0        0        0     7438 2024-03-23 03:58:13.376541 fhirstarter-2.2.1/fhirstarter/tests/test_utils.py
--rw-r--r--   0        0        0     2552 2024-03-23 03:58:13.380923 fhirstarter-2.2.1/fhirstarter/tests/utils.py
--rw-r--r--   0        0        0    18870 2024-03-23 03:58:13.382586 fhirstarter-2.2.1/fhirstarter/utils.py
--rw-r--r--   0        0        0     3050 2024-03-23 16:52:27.149272 fhirstarter-2.2.1/pyproject.toml
--rw-r--r--   0        0        0     9714 1970-01-01 00:00:00.000000 fhirstarter-2.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-13 04:02:48.301721 fhirstarter-2.2.2/LICENSE.md
+-rw-r--r--   0        0        0     7650 2024-04-13 04:02:48.301721 fhirstarter-2.2.2/README.md
+-rw-r--r--   0        0        0      618 2024-04-13 04:02:48.301721 fhirstarter-2.2.2/fhirstarter/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 04:02:48.301721 fhirstarter-2.2.2/fhirstarter/examples/__init__.py
+-rw-r--r--   0        0        0      151 2024-04-13 04:02:48.301721 fhirstarter-2.2.2/fhirstarter/examples/config.toml
+-rw-r--r--   0        0        0     6464 2024-04-13 04:02:48.301721 fhirstarter-2.2.2/fhirstarter/examples/example.py
+-rw-r--r--   0        0        0     6289 2024-04-13 04:02:48.301721 fhirstarter-2.2.2/fhirstarter/exceptions.py
+-rw-r--r--   0        0        0       92 2024-04-13 04:02:48.301721 fhirstarter-2.2.2/fhirstarter/fhir_specification/__init__.py
+-rw-r--r--   0        0        0    10722 2024-04-13 04:02:48.301721 fhirstarter-2.2.2/fhirstarter/fhir_specification/scripts/create_sequence_data.py
+-rw-r--r--   0        0        0        0 2024-04-13 04:02:48.301721 fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/R4/__init__.py
+-rw-r--r--   0        0        0   392011 2024-04-13 04:02:48.301721 fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/R4/examples.zip
+-rw-r--r--   0        0        0     2814 2024-04-13 04:02:48.301721 fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/R4/extra-search-parameters.json
+-rw-r--r--   0        0        0     3334 2024-04-13 04:02:48.301721 fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/R4/resource_types.json
+-rw-r--r--   0        0        0   113904 2024-04-13 04:02:48.305722 fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/R4/search-parameters.zip
+-rw-r--r--   0        0        0        0 2024-04-13 04:02:48.305722 fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/R4B/__init__.py
+-rw-r--r--   0        0        0   397649 2024-04-13 04:02:48.305722 fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/R4B/examples.zip
+-rw-r--r--   0        0        0     1800 2024-04-13 04:02:48.305722 fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/R4B/extra-search-parameters.json
+-rw-r--r--   0        0        0     3081 2024-04-13 04:02:48.305722 fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/R4B/resource_types.json
+-rw-r--r--   0        0        0   117431 2024-04-13 04:02:48.305722 fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/R4B/search-parameters.zip
+-rw-r--r--   0        0        0        0 2024-04-13 04:02:48.305722 fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/R5/__init__.py
+-rw-r--r--   0        0        0   436165 2024-04-13 04:02:48.309722 fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/R5/examples.zip
+-rw-r--r--   0        0        0     2356 2024-04-13 04:02:48.309722 fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/R5/extra-search-parameters.json
+-rw-r--r--   0        0        0     3526 2024-04-13 04:02:48.309722 fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/R5/resource_types.json
+-rw-r--r--   0        0        0   112399 2024-04-13 04:02:48.309722 fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/R5/search-parameters.zip
+-rw-r--r--   0        0        0        0 2024-04-13 04:02:48.309722 fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/STU3/__init__.py
+-rw-r--r--   0        0        0   361150 2024-04-13 04:02:48.309722 fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/STU3/examples.zip
+-rw-r--r--   0        0        0     2624 2024-04-13 04:02:48.309722 fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/STU3/extra-search-parameters.json
+-rw-r--r--   0        0        0     2416 2024-04-13 04:02:48.309722 fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/STU3/resource_types.json
+-rw-r--r--   0        0        0    91155 2024-04-13 04:02:48.309722 fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/STU3/search-parameters.zip
+-rw-r--r--   0        0        0       32 2024-04-13 04:02:48.309722 fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/__init__.py
+-rw-r--r--   0        0        0     4692 2024-04-13 04:02:48.309722 fhirstarter-2.2.2/fhirstarter/fhir_specification/utils.py
+-rw-r--r--   0        0        0    22399 2024-04-13 04:02:48.309722 fhirstarter-2.2.2/fhirstarter/fhirstarter.py
+-rw-r--r--   0        0        0    20633 2024-04-13 04:02:48.309722 fhirstarter-2.2.2/fhirstarter/functions.py
+-rw-r--r--   0        0        0     3354 2024-04-13 04:02:48.309722 fhirstarter-2.2.2/fhirstarter/interactions.py
+-rw-r--r--   0        0        0     3135 2024-04-13 04:02:48.313722 fhirstarter-2.2.2/fhirstarter/json_patch.py
+-rw-r--r--   0        0        0    10517 2024-04-13 04:02:48.313722 fhirstarter-2.2.2/fhirstarter/openapi.py
+-rw-r--r--   0        0        0     7222 2024-04-13 04:02:48.313722 fhirstarter-2.2.2/fhirstarter/providers.py
+-rw-r--r--   0        0        0     1691 2024-04-13 04:02:48.313722 fhirstarter-2.2.2/fhirstarter/resources.py
+-rw-r--r--   0        0        0     6375 2024-04-13 04:02:48.313722 fhirstarter-2.2.2/fhirstarter/search_parameters.py
+-rw-r--r--   0        0        0       68 2024-04-13 04:02:48.313722 fhirstarter-2.2.2/fhirstarter/testclient.py
+-rw-r--r--   0        0        0        0 2024-04-13 04:02:48.313722 fhirstarter-2.2.2/fhirstarter/tests/__init__.py
+-rw-r--r--   0        0        0     6330 2024-04-13 04:02:48.313722 fhirstarter-2.2.2/fhirstarter/tests/config.py
+-rw-r--r--   0        0        0     1373 2024-04-13 04:02:48.313722 fhirstarter-2.2.2/fhirstarter/tests/conftest.py
+-rw-r--r--   0        0        0     1500 2024-04-13 04:02:48.313722 fhirstarter-2.2.2/fhirstarter/tests/resources.py
+-rw-r--r--   0        0        0     6667 2024-04-13 04:02:48.313722 fhirstarter-2.2.2/fhirstarter/tests/test_capability_statement.py
+-rw-r--r--   0        0        0     3547 2024-04-13 04:02:48.313722 fhirstarter-2.2.2/fhirstarter/tests/test_dependencies.py
+-rw-r--r--   0        0        0    10310 2024-04-13 04:02:48.313722 fhirstarter-2.2.2/fhirstarter/tests/test_errors.py
+-rw-r--r--   0        0        0    14721 2024-04-13 04:02:48.313722 fhirstarter-2.2.2/fhirstarter/tests/test_interactions.py
+-rw-r--r--   0        0        0    13703 2024-04-13 04:02:48.313722 fhirstarter-2.2.2/fhirstarter/tests/test_openapi.py
+-rw-r--r--   0        0        0     7438 2024-04-13 04:02:48.313722 fhirstarter-2.2.2/fhirstarter/tests/test_utils.py
+-rw-r--r--   0        0        0     2552 2024-04-13 04:02:48.313722 fhirstarter-2.2.2/fhirstarter/tests/utils.py
+-rw-r--r--   0        0        0    18870 2024-04-13 04:02:48.313722 fhirstarter-2.2.2/fhirstarter/utils.py
+-rw-r--r--   0        0        0     3050 2024-04-13 04:02:48.313722 fhirstarter-2.2.2/pyproject.toml
+-rw-r--r--   0        0        0     9714 1970-01-01 00:00:00.000000 fhirstarter-2.2.2/PKG-INFO
```

### Comparing `fhirstarter-2.2.1/LICENSE.md` & `fhirstarter-2.2.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.1/README.md` & `fhirstarter-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.1/fhirstarter/__init__.py` & `fhirstarter-2.2.2/fhirstarter/__init__.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.1/fhirstarter/examples/example.py` & `fhirstarter-2.2.2/fhirstarter/examples/example.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 """
 An example FHIR server implementation using FHIRStarter, with examples showing how to create FHIR
 interactions (i.e. endpoints) that perform create, read, search-type, and update operations.
 """
 
 import contextlib
-from copy import deepcopy
+import json
 from pathlib import Path
-from typing import Any, Dict, List, MutableMapping, Union, cast
+from typing import Any, Dict, List, MutableMapping, Union
 from uuid import uuid4
 
 import jsonpatch
 import uvicorn
 from fhir.resources.bundle import Bundle
 from fhir.resources.fhirtypes import Id
-from fhir.resources.humanname import HumanName
 from fhir.resources.patient import Patient
 from fhir.resources.practitioner import Practitioner
 from starlette.responses import RedirectResponse
 
 import fhirstarter
 from fhirstarter import (
     FHIRProvider,
@@ -25,24 +24,27 @@
     InteractionContext,
     JSONPatch,
     Request,
     Response,
     convert_json_patch,
     examples,
 )
-from fhirstarter.exceptions import FHIRResourceNotFoundError
+from fhirstarter.exceptions import (
+    FHIRResourceNotFoundError,
+    FHIRUnprocessableEntityError,
+)
 
 # Create the app with the provided config file
 app = FHIRStarter(
     title="FHIRStarter Example Implementation",
     config_file=Path(examples.__file__).parent / "config.toml",
 )
 
 # Create a "database"
-DATABASE: Dict[str, Patient] = {}
+DATABASE: Dict[str, Dict[str, str]] = {"Patient": {}, "Practitioner": {}}
 
 # Create a provider
 provider = FHIRProvider()
 
 # To register FHIR interactions with  a provider, the pieces of information the developer has to
 # provide are:
 # * FHIR interaction type (this affects what the endpoint will look like)
@@ -51,92 +53,100 @@
 # * the handler (expected signature and annotations need to match the defined protocols, because
 #   these values affect route creation in FastAPI)
 
 
 # Register the patient read FHIR interaction with the provider
 @provider.read(Patient)
 async def patient_read(context: InteractionContext, id_: Id) -> Patient:
-    patient = DATABASE.get(id_)
+    patient = DATABASE["Patient"].get(id_)
     if not patient:
         raise FHIRResourceNotFoundError
 
-    return patient
+    return Patient(**json.loads(patient))
 
 
 # Register the patient update FHIR interaction with the provider
 @provider.update(Patient)
 async def patient_update(context: InteractionContext, id_: Id, resource: Patient) -> Id:
-    if id_ not in DATABASE:
+    if id_ not in DATABASE["Patient"]:
         raise FHIRResourceNotFoundError
 
-    patient = deepcopy(resource)
-    DATABASE[id_] = patient
+    DATABASE["Patient"][id_] = resource.json(separators=(",", ":"))
 
-    return Id(patient.id)
+    return Id(id_)
 
 
 # Register the patient patch FHIR interaction with the provider
 @provider.patch(Patient)
 async def patient_patch(
     context: InteractionContext, id_: Id, json_patch: JSONPatch
 ) -> Id:
-    if id_ not in DATABASE:
+    patient = json.loads(DATABASE["Patient"].get(id_, "{}"))
+    if not patient:
         raise FHIRResourceNotFoundError
 
-    patient = DATABASE[id_].dict()
-
     # Convert the JSONPatch object to a list of dicts using the helper function, and use the
     # jsonpatch package to apply the patch to the patient resource
     patch = convert_json_patch(json_patch)
     jsonpatch.apply_patch(patient, jsonpatch.JsonPatch(patch), in_place=True)
 
-    DATABASE[id_] = Patient(**patient)
+    # Validate the change
+    try:
+        Patient.validate(patient)
+    except Exception as exception:
+        raise FHIRUnprocessableEntityError(
+            code="invalid", details_text="Validation of patched resource failed"
+        ) from exception
+
+    DATABASE["Patient"][id_] = json.dumps(patient, separators=(",", ":"))
 
     return Id(id_)
 
 
 @provider.delete(Patient)
 async def patient_delete(context: InteractionContext, id_: Id) -> None:
     with contextlib.suppress(KeyError):
-        del DATABASE[id_]
+        del DATABASE["Patient"][id_]
 
     return None
 
 
 # Register the patient create FHIR interaction with the provider
 @provider.create(Patient)
 async def patient_create(context: InteractionContext, resource: Patient) -> Id:
-    patient = deepcopy(resource)
-    patient.id = Id(uuid4().hex)
-    DATABASE[patient.id] = patient
+    id_ = str(uuid4())
 
-    return Id(patient.id)
+    resource.id = id_
+    DATABASE["Patient"][id_] = resource.json(separators=(",", ":"))
+
+    return Id(id_)
 
 
 # Register the patient search-type FHIR interaction with the provider
 @provider.search_type(Patient)
 async def patient_search_type(
     context: InteractionContext,
     birthdate: Union[List[str], None],
     general_practitioner: Union[str, None],
     family: Union[str, None],
     nickname: Union[str, None],
     _last_updated: Union[str, None],
 ) -> Bundle:
     patients = []
-    for patient in DATABASE.values():
-        for name in patient.name:
-            if cast(HumanName, name).family == family:
+    for patient_serialized in DATABASE["Patient"].values():
+        patient = json.loads(patient_serialized)
+        for name in patient.get("name", {}):
+            if name.get("family") == family:
                 patients.append(patient)
 
     bundle = Bundle(
         **{
             "type": "searchset",
             "total": len(patients),
-            "entry": [{"resource": patient.dict()} for patient in patients],
+            "entry": [{"resource": patient} for patient in patients],
         }
     )
 
     return bundle
 
 
 # Optional: Provide a custom example for the automatic documentation by defining a subclass of the
@@ -152,15 +162,19 @@
             }
         }
 
 
 # Register the practitioner read FHIR interaction with the provider using the custom subclass
 @provider.read(PractitionerCustom)
 async def practitioner_read(context: InteractionContext, id_: Id) -> PractitionerCustom:
-    return PractitionerCustom(**PractitionerCustom.Config.schema_extra["example"])
+    practitioner = DATABASE["Practitioner"].get(id_)
+    if not practitioner:
+        raise FHIRResourceNotFoundError
+
+    return PractitionerCustom(**json.loads(practitioner))
 
 
 # Add the provider to the app. This will automatically generate the API routes for the interactions
 # provided by the providers (e.g. create, read, search-type, and update).
 app.add_providers(provider)
```

### Comparing `fhirstarter-2.2.1/fhirstarter/exceptions.py` & `fhirstarter-2.2.2/fhirstarter/exceptions.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.1/fhirstarter/fhir_specification/scripts/create_sequence_data.py` & `fhirstarter-2.2.2/fhirstarter/fhir_specification/scripts/create_sequence_data.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.1/fhirstarter/fhir_specification/sequences/R4/examples.zip` & `fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/R4/examples.zip`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.1/fhirstarter/fhir_specification/sequences/R4/extra-search-parameters.json` & `fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/R4/extra-search-parameters.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.1/fhirstarter/fhir_specification/sequences/R4/resource_types.json` & `fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/R4/resource_types.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.1/fhirstarter/fhir_specification/sequences/R4/search-parameters.zip` & `fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/R4/search-parameters.zip`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.1/fhirstarter/fhir_specification/sequences/R4B/examples.zip` & `fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/R4B/examples.zip`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.1/fhirstarter/fhir_specification/sequences/R4B/extra-search-parameters.json` & `fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/R4B/extra-search-parameters.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.1/fhirstarter/fhir_specification/sequences/R4B/resource_types.json` & `fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/R4B/resource_types.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.1/fhirstarter/fhir_specification/sequences/R4B/search-parameters.zip` & `fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/R4B/search-parameters.zip`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.1/fhirstarter/fhir_specification/sequences/R5/examples.zip` & `fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/R5/examples.zip`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.1/fhirstarter/fhir_specification/sequences/R5/extra-search-parameters.json` & `fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/R5/extra-search-parameters.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.1/fhirstarter/fhir_specification/sequences/R5/resource_types.json` & `fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/R5/resource_types.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.1/fhirstarter/fhir_specification/sequences/R5/search-parameters.zip` & `fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/R5/search-parameters.zip`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.1/fhirstarter/fhir_specification/sequences/STU3/examples.zip` & `fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/STU3/examples.zip`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.1/fhirstarter/fhir_specification/sequences/STU3/extra-search-parameters.json` & `fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/STU3/extra-search-parameters.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.1/fhirstarter/fhir_specification/sequences/STU3/resource_types.json` & `fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/STU3/resource_types.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.1/fhirstarter/fhir_specification/sequences/STU3/search-parameters.zip` & `fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/STU3/search-parameters.zip`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.1/fhirstarter/fhir_specification/utils.py` & `fhirstarter-2.2.2/fhirstarter/fhir_specification/utils.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.1/fhirstarter/fhirstarter.py` & `fhirstarter-2.2.2/fhirstarter/fhirstarter.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.1/fhirstarter/functions.py` & `fhirstarter-2.2.2/fhirstarter/functions.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.1/fhirstarter/interactions.py` & `fhirstarter-2.2.2/fhirstarter/interactions.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.1/fhirstarter/json_patch.py` & `fhirstarter-2.2.2/fhirstarter/json_patch.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.1/fhirstarter/openapi.py` & `fhirstarter-2.2.2/fhirstarter/openapi.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.1/fhirstarter/providers.py` & `fhirstarter-2.2.2/fhirstarter/providers.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.1/fhirstarter/resources.py` & `fhirstarter-2.2.2/fhirstarter/resources.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.1/fhirstarter/search_parameters.py` & `fhirstarter-2.2.2/fhirstarter/search_parameters.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.1/fhirstarter/tests/config.py` & `fhirstarter-2.2.2/fhirstarter/tests/config.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.1/fhirstarter/tests/conftest.py` & `fhirstarter-2.2.2/fhirstarter/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.1/fhirstarter/tests/resources.py` & `fhirstarter-2.2.2/fhirstarter/tests/resources.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.1/fhirstarter/tests/test_capability_statement.py` & `fhirstarter-2.2.2/fhirstarter/tests/test_capability_statement.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.1/fhirstarter/tests/test_dependencies.py` & `fhirstarter-2.2.2/fhirstarter/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.1/fhirstarter/tests/test_errors.py` & `fhirstarter-2.2.2/fhirstarter/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.1/fhirstarter/tests/test_interactions.py` & `fhirstarter-2.2.2/fhirstarter/tests/test_interactions.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.1/fhirstarter/tests/test_openapi.py` & `fhirstarter-2.2.2/fhirstarter/tests/test_openapi.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.1/fhirstarter/tests/test_utils.py` & `fhirstarter-2.2.2/fhirstarter/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.1/fhirstarter/tests/utils.py` & `fhirstarter-2.2.2/fhirstarter/tests/utils.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.1/fhirstarter/utils.py` & `fhirstarter-2.2.2/fhirstarter/utils.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.1/pyproject.toml` & `fhirstarter-2.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fhirstarter"
-version = "2.2.1"
+version = "2.2.2"
 description = "An ASGI FHIR API framework built on top of FastAPI and FHIR Resources"
 authors = ["Christopher Sande <christopher.sande@canvasmedical.com>"]
 maintainers = ["Canvas Medical Engineering <engineering@canvasmedical.com>"]
 readme = "README.md"
 homepage = "https://github.com/canvas-medical/fhirstarter"
 repository = "https://github.com/canvas-medical/fhirstarter"
 keywords = ["fhir", "api", "server", "resources", "framework", "fastapi", "healthcare", "hl7"]
```

### Comparing `fhirstarter-2.2.1/PKG-INFO` & `fhirstarter-2.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fhirstarter
-Version: 2.2.1
+Version: 2.2.2
 Summary: An ASGI FHIR API framework built on top of FastAPI and FHIR Resources
 Home-page: https://github.com/canvas-medical/fhirstarter
 Keywords: fhir,api,server,resources,framework,fastapi,healthcare,hl7
 Author: Christopher Sande
 Author-email: christopher.sande@canvasmedical.com
 Maintainer: Canvas Medical Engineering
 Maintainer-email: engineering@canvasmedical.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fhirstarter Version: 2.2.1 Summary: An ASGI FHIR
+Metadata-Version: 2.1 Name: fhirstarter Version: 2.2.2 Summary: An ASGI FHIR
 API framework built on top of FastAPI and FHIR Resources Home-page: https://
 github.com/canvas-medical/fhirstarter Keywords:
 fhir,api,server,resources,framework,fastapi,healthcare,hl7 Author: Christopher
 Sande Author-email: christopher.sande@canvasmedical.com Maintainer: Canvas
 Medical Engineering Maintainer-email: engineering@canvasmedical.com Requires-
 Python: >=3.8.0,<3.13.0 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment Classifier: Framework :: AsyncIO
```

