# Comparing `tmp/onnxscript-0.1.0.dev20240411.tar.gz` & `tmp/onnxscript-0.1.0.dev20240412.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnxscript-0.1.0.dev20240411.tar", last modified: Thu Apr 11 00:01:34 2024, max compression
+gzip compressed data, was "onnxscript-0.1.0.dev20240412.tar", last modified: Fri Apr 12 00:02:28 2024, max compression
```

## Comparing `onnxscript-0.1.0.dev20240411.tar` & `onnxscript-0.1.0.dev20240412.tar`

### file list

```diff
@@ -1,213 +1,214 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-11 00:01:34.459064 onnxscript-0.1.0.dev20240411/
--rw-r--r--   0 vsts      (1001) docker     (127)     1073 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)      211 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)    10846 2024-04-11 00:01:34.459064 onnxscript-0.1.0.dev20240411/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     8680 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/README.md
--rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/VERSION
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-11 00:01:34.423064 onnxscript-0.1.0.dev20240411/onnxscript/
--rw-r--r--   0 vsts      (1001) docker     (127)     2282 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-11 00:01:34.427064 onnxscript-0.1.0.dev20240411/onnxscript/_internal/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/_internal/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9313 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/_internal/analysis.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2228 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/_internal/ast_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9811 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/_internal/autocast.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2560 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/_internal/deprecation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5166 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/_internal/param_manipulation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1081 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/_internal/runtime_typing.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3523 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/_internal/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1018 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/_internal/version_utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-11 00:01:34.427064 onnxscript-0.1.0.dev20240411/onnxscript/_legacy_ir/
--rw-r--r--   0 vsts      (1001) docker     (127)    11068 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/_legacy_ir/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8872 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/_legacy_ir/irbuilder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5929 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/_legacy_ir/protobuilder.py
--rw-r--r--   0 vsts      (1001) docker     (127)    36193 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/_legacy_ir/visitor.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-11 00:01:34.427064 onnxscript-0.1.0.dev20240411/onnxscript/_thirdparty/
--rw-r--r--   0 vsts      (1001) docker     (127)    10608 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/_thirdparty/asciichartpy.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-11 00:01:34.431064 onnxscript-0.1.0.dev20240411/onnxscript/backend/
--rw-r--r--   0 vsts      (1001) docker     (127)      247 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/backend/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11498 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/backend/onnx_backend.py
--rw-r--r--   0 vsts      (1001) docker     (127)    30612 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/backend/onnx_export.py
--rw-r--r--   0 vsts      (1001) docker     (127)    61554 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/converter.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-11 00:01:34.419064 onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-11 00:01:34.431064 onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/
--rw-r--r--   0 vsts      (1001) docker     (127)      583 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11045 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/_infra.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13086 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/context.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5544 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/decorator.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3364 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/formatter.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-11 00:01:34.439064 onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/
--rw-r--r--   0 vsts      (1001) docker     (127)     4364 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1716 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_address.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2980 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_artifact.py
--rw-r--r--   0 vsts      (1001) docker     (127)      875 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_artifact_change.py
--rw-r--r--   0 vsts      (1001) docker     (127)      996 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_artifact_content.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1029 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_artifact_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1195 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_attachment.py
--rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_code_flow.py
--rw-r--r--   0 vsts      (1001) docker     (127)      986 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_configuration_override.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1154 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_conversion.py
--rw-r--r--   0 vsts      (1001) docker     (127)      937 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_edge.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1065 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_edge_traversal.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1133 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_exception.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3794 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_external_properties.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1089 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3819 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1034 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_fix.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1051 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_graph.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1388 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_graph_traversal.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4561 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_invocation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1552 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      946 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_location_relationship.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1282 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_logical_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_message.py
--rw-r--r--   0 vsts      (1001) docker     (127)      787 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1036 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_node.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1892 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_notification.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1305 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_physical_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      488 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_property_bag.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1141 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_rectangle.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2013 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_region.py
--rw-r--r--   0 vsts      (1001) docker     (127)      870 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_replacement.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1104 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2700 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1109 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1090 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5002 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_result.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_result_provenance.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5246 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_run.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1118 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_run_automation_details.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1198 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_sarif_log.py
--rw-r--r--   0 vsts      (1001) docker     (127)      751 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_special_locations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      824 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_stack.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1070 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_stack_frame.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1231 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_suppression.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1333 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_thread_flow.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2473 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      830 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_tool.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4941 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_tool_component.py
--rw-r--r--   0 vsts      (1001) docker     (127)      915 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_translation_metadata.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1391 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_version_control_details.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1498 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_web_request.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1566 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_web_response.py
--rw-r--r--   0 vsts      (1001) docker     (127)      193 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/version.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2515 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    22081 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/evaluator.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-11 00:01:34.419064 onnxscript-0.1.0.dev20240411/onnxscript/function_libs/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-11 00:01:34.419064 onnxscript-0.1.0.dev20240411/onnxscript/function_libs/tools/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-11 00:01:34.439064 onnxscript-0.1.0.dev20240411/onnxscript/function_libs/tools/torch_lib/
--rw-r--r--   0 vsts      (1001) docker     (127)    16361 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11767 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11834 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-11 00:01:34.443064 onnxscript-0.1.0.dev20240411/onnxscript/function_libs/torch_lib/
--rw-r--r--   0 vsts      (1001) docker     (127)      149 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/function_libs/torch_lib/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)       77 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/function_libs/torch_lib/_constants.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1285 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/function_libs/torch_lib/_flags.py
--rw-r--r--   0 vsts      (1001) docker     (127)    43814 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/function_libs/torch_lib/graph_building.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-11 00:01:34.443064 onnxscript-0.1.0.dev20240411/onnxscript/function_libs/torch_lib/ops/
--rw-r--r--   0 vsts      (1001) docker     (127)      208 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/function_libs/torch_lib/ops/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1991 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/function_libs/torch_lib/ops/common.py
--rw-r--r--   0 vsts      (1001) docker     (127)   288377 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/function_libs/torch_lib/ops/core.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12343 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/function_libs/torch_lib/ops/fft.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13256 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/function_libs/torch_lib/ops/linalg.py
--rw-r--r--   0 vsts      (1001) docker     (127)      911 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/function_libs/torch_lib/ops/nested.py
--rw-r--r--   0 vsts      (1001) docker     (127)    86028 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/function_libs/torch_lib/ops/nn.py
--rw-r--r--   0 vsts      (1001) docker     (127)    20667 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/function_libs/torch_lib/ops/prims.py
--rw-r--r--   0 vsts      (1001) docker     (127)      920 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/function_libs/torch_lib/ops/sparse.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11262 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/function_libs/torch_lib/ops/special.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1155 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/function_libs/torch_lib/ops/vision.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5547 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/function_libs/torch_lib/registration.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2118 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/function_libs/torch_lib/tensor_typing.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-11 00:01:34.447064 onnxscript-0.1.0.dev20240411/onnxscript/ir/
--rw-r--r--   0 vsts      (1001) docker     (127)     2306 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/ir/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    59114 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/ir/_core.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1775 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/ir/_display.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2696 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/ir/_enums.py
--rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/ir/_graph_comparison.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1853 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/ir/_invariants.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10417 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/ir/_linked_list.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2525 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/ir/_metadata.py
--rw-r--r--   0 vsts      (1001) docker     (127)    17302 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/ir/_protocols.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1489 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/ir/convenience.py
--rw-r--r--   0 vsts      (1001) docker     (127)    44088 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/ir/serde.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19643 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/irbuilder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6457 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/main.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-11 00:01:34.447064 onnxscript-0.1.0.dev20240411/onnxscript/onnx_opset/
--rw-r--r--   0 vsts      (1001) docker     (127)     4852 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/onnx_opset/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-11 00:01:34.451064 onnxscript-0.1.0.dev20240411/onnxscript/onnx_opset/_impl/
--rw-r--r--   0 vsts      (1001) docker     (127)   153815 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/onnx_opset/_impl/opset1.py
--rw-r--r--   0 vsts      (1001) docker     (127)    53445 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/onnx_opset/_impl/opset10.py
--rw-r--r--   0 vsts      (1001) docker     (127)   157597 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/onnx_opset/_impl/opset11.py
--rw-r--r--   0 vsts      (1001) docker     (127)    43533 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/onnx_opset/_impl/opset12.py
--rw-r--r--   0 vsts      (1001) docker     (127)   140743 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/onnx_opset/_impl/opset13.py
--rw-r--r--   0 vsts      (1001) docker     (127)    41780 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/onnx_opset/_impl/opset14.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19290 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/onnx_opset/_impl/opset15.py
--rw-r--r--   0 vsts      (1001) docker     (127)    50662 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/onnx_opset/_impl/opset16.py
--rw-r--r--   0 vsts      (1001) docker     (127)    21513 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/onnx_opset/_impl/opset17.py
--rw-r--r--   0 vsts      (1001) docker     (127)    70208 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/onnx_opset/_impl/opset18.py
--rw-r--r--   0 vsts      (1001) docker     (127)    75098 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/onnx_opset/_impl/opset19.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7937 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/onnx_opset/_impl/opset2.py
--rw-r--r--   0 vsts      (1001) docker     (127)    28284 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/onnx_opset/_impl/opset20.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7645 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/onnx_opset/_impl/opset3.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1966 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/onnx_opset/_impl/opset4.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2572 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/onnx_opset/_impl/opset5.py
--rw-r--r--   0 vsts      (1001) docker     (127)    33248 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/onnx_opset/_impl/opset6.py
--rw-r--r--   0 vsts      (1001) docker     (127)    49053 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/onnx_opset/_impl/opset7.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19393 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/onnx_opset/_impl/opset8.py
--rw-r--r--   0 vsts      (1001) docker     (127)    58411 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/onnx_opset/_impl/opset9.py
--rw-r--r--   0 vsts      (1001) docker     (127)    39030 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4439 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13894 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5368 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24713 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5875 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/onnx_types.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-11 00:01:34.455064 onnxscript-0.1.0.dev20240411/onnxscript/optimizer/
--rw-r--r--   0 vsts      (1001) docker     (127)     4288 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/optimizer/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10166 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/optimizer/constant_folding.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2872 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/optimizer/copy_propagation.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15445 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/optimizer/evaluator.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8554 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/optimizer/fold_constants_v0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3994 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/optimizer/remove_unused.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2080 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/optimizer/remove_unused_function.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9852 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/optimizer/simple_function_folding.py
--rw-r--r--   0 vsts      (1001) docker     (127)       41 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/py.typed
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-11 00:01:34.455064 onnxscript-0.1.0.dev20240411/onnxscript/rewriter/
--rw-r--r--   0 vsts      (1001) docker     (127)     1424 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/rewriter/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6698 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/rewriter/broadcast_to_matmul.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2165 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/rewriter/cast_constant_of_shape.py
--rw-r--r--   0 vsts      (1001) docker     (127)      686 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/rewriter/erfgelu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8844 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/rewriter/function_rule.py
--rw-r--r--   0 vsts      (1001) docker     (127)      756 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/rewriter/gemm_to_matmul_add.py
--rw-r--r--   0 vsts      (1001) docker     (127)    43596 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/rewriter/generic_pattern.py
--rw-r--r--   0 vsts      (1001) docker     (127)      828 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/rewriter/no_op.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-11 00:01:34.455064 onnxscript-0.1.0.dev20240411/onnxscript/rewriter/onnxruntime/
--rw-r--r--   0 vsts      (1001) docker     (127)     2216 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/rewriter/onnxruntime/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1222 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5082 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1943 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/rewriter/onnxruntime/softmax.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-11 00:01:34.455064 onnxscript-0.1.0.dev20240411/onnxscript/rewriter/onnxruntime/transformers/
--rw-r--r--   0 vsts      (1001) docker     (127)      488 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/rewriter/onnxruntime/transformers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      885 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1628 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/rewriter/onnxruntime/transformers/layernorm.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24688 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py
--rw-r--r--   0 vsts      (1001) docker     (127)    39591 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/rewriter/pattern.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1700 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/sourceinfo.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7658 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/tensor.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-11 00:01:34.459064 onnxscript-0.1.0.dev20240411/onnxscript/testing/
--rw-r--r--   0 vsts      (1001) docker     (127)    17350 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/testing/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11025 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/type_annotation.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-11 00:01:34.459064 onnxscript-0.1.0.dev20240411/onnxscript/utils/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/utils/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2239 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/utils/evaluation_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)      706 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/utils/timing_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2505 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/utils/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24781 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/onnxscript/values.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-11 00:01:34.459064 onnxscript-0.1.0.dev20240411/onnxscript.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)    10846 2024-04-11 00:01:34.000000 onnxscript-0.1.0.dev20240411/onnxscript.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     7962 2024-04-11 00:01:34.000000 onnxscript-0.1.0.dev20240411/onnxscript.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-11 00:01:34.000000 onnxscript-0.1.0.dev20240411/onnxscript.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       35 2024-04-11 00:01:34.000000 onnxscript-0.1.0.dev20240411/onnxscript.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-04-11 00:01:34.000000 onnxscript-0.1.0.dev20240411/onnxscript.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)     6525 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-04-11 00:01:34.459064 onnxscript-0.1.0.dev20240411/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)     1292 2024-04-11 00:00:56.000000 onnxscript-0.1.0.dev20240411/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 00:02:28.861608 onnxscript-0.1.0.dev20240412/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1073 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)      211 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)    10846 2024-04-12 00:02:28.861608 onnxscript-0.1.0.dev20240412/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     8680 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/VERSION
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 00:02:28.825608 onnxscript-0.1.0.dev20240412/onnxscript/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2282 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 00:02:28.829608 onnxscript-0.1.0.dev20240412/onnxscript/_internal/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/_internal/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9313 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/_internal/analysis.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2228 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/_internal/ast_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9811 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/_internal/autocast.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2560 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/_internal/deprecation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5166 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/_internal/param_manipulation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1081 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/_internal/runtime_typing.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3523 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/_internal/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1018 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/_internal/version_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 00:02:28.829608 onnxscript-0.1.0.dev20240412/onnxscript/_legacy_ir/
+-rw-r--r--   0 vsts      (1001) docker     (127)    11068 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/_legacy_ir/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8872 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/_legacy_ir/irbuilder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5929 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/_legacy_ir/protobuilder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    36193 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/_legacy_ir/visitor.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 00:02:28.829608 onnxscript-0.1.0.dev20240412/onnxscript/_thirdparty/
+-rw-r--r--   0 vsts      (1001) docker     (127)    10608 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/_thirdparty/asciichartpy.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 00:02:28.829608 onnxscript-0.1.0.dev20240412/onnxscript/backend/
+-rw-r--r--   0 vsts      (1001) docker     (127)      247 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/backend/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11498 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/backend/onnx_backend.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    30612 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/backend/onnx_export.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    61554 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/converter.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 00:02:28.821608 onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 00:02:28.829608 onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/
+-rw-r--r--   0 vsts      (1001) docker     (127)      583 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11045 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/_infra.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13086 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/context.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5544 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/decorator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3364 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/formatter.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 00:02:28.841608 onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4364 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1716 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_address.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2980 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_artifact.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      875 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_artifact_change.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      996 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_artifact_content.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1029 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_artifact_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1195 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_attachment.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_code_flow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      986 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_configuration_override.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1154 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_conversion.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      937 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_edge.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1065 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_edge_traversal.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1133 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_exception.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3794 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_external_properties.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1089 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3819 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1034 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_fix.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1051 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_graph.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1388 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_graph_traversal.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4561 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_invocation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1552 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      946 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_location_relationship.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1282 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_logical_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_message.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      787 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1036 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_node.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1892 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_notification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1305 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_physical_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      488 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_property_bag.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1141 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_rectangle.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2013 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_region.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      870 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_replacement.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1104 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2700 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1109 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1090 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5002 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_result.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_result_provenance.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5246 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_run.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1118 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_run_automation_details.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1198 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_sarif_log.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      751 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_special_locations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      824 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_stack.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1070 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_stack_frame.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1231 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_suppression.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1333 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_thread_flow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2473 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      830 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_tool.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4941 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_tool_component.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      915 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_translation_metadata.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1391 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_version_control_details.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1498 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_web_request.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1566 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_web_response.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      193 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/version.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2515 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    22081 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/evaluator.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 00:02:28.821608 onnxscript-0.1.0.dev20240412/onnxscript/function_libs/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 00:02:28.821608 onnxscript-0.1.0.dev20240412/onnxscript/function_libs/tools/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 00:02:28.841608 onnxscript-0.1.0.dev20240412/onnxscript/function_libs/tools/torch_lib/
+-rw-r--r--   0 vsts      (1001) docker     (127)    16361 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11767 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11834 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 00:02:28.841608 onnxscript-0.1.0.dev20240412/onnxscript/function_libs/torch_lib/
+-rw-r--r--   0 vsts      (1001) docker     (127)      149 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/function_libs/torch_lib/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       77 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/function_libs/torch_lib/_constants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1285 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/function_libs/torch_lib/_flags.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    43814 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/function_libs/torch_lib/graph_building.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 00:02:28.845608 onnxscript-0.1.0.dev20240412/onnxscript/function_libs/torch_lib/ops/
+-rw-r--r--   0 vsts      (1001) docker     (127)      208 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/function_libs/torch_lib/ops/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1991 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/function_libs/torch_lib/ops/common.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   288377 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/function_libs/torch_lib/ops/core.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12343 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/function_libs/torch_lib/ops/fft.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13256 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/function_libs/torch_lib/ops/linalg.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      911 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/function_libs/torch_lib/ops/nested.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    86028 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/function_libs/torch_lib/ops/nn.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    20667 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/function_libs/torch_lib/ops/prims.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      920 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/function_libs/torch_lib/ops/sparse.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11262 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/function_libs/torch_lib/ops/special.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1155 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/function_libs/torch_lib/ops/vision.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5547 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/function_libs/torch_lib/registration.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2118 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/function_libs/torch_lib/tensor_typing.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 00:02:28.849608 onnxscript-0.1.0.dev20240412/onnxscript/ir/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2338 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/ir/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    64439 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/ir/_core.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1775 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/ir/_display.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2696 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/ir/_enums.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/ir/_graph_comparison.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1853 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/ir/_invariants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10417 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/ir/_linked_list.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2525 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/ir/_metadata.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1064 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/ir/_name_authority.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    18653 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/ir/_protocols.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1489 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/ir/convenience.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    44162 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/ir/serde.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19643 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/irbuilder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6457 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/main.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 00:02:28.849608 onnxscript-0.1.0.dev20240412/onnxscript/onnx_opset/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4852 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/onnx_opset/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 00:02:28.853608 onnxscript-0.1.0.dev20240412/onnxscript/onnx_opset/_impl/
+-rw-r--r--   0 vsts      (1001) docker     (127)   153815 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/onnx_opset/_impl/opset1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    53445 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/onnx_opset/_impl/opset10.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   157597 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/onnx_opset/_impl/opset11.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    43533 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/onnx_opset/_impl/opset12.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   140743 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/onnx_opset/_impl/opset13.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    41780 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/onnx_opset/_impl/opset14.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19290 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/onnx_opset/_impl/opset15.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    50662 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/onnx_opset/_impl/opset16.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    21513 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/onnx_opset/_impl/opset17.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    70208 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/onnx_opset/_impl/opset18.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    75098 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/onnx_opset/_impl/opset19.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7937 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/onnx_opset/_impl/opset2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    28284 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/onnx_opset/_impl/opset20.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7645 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/onnx_opset/_impl/opset3.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1966 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/onnx_opset/_impl/opset4.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2572 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/onnx_opset/_impl/opset5.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    33248 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/onnx_opset/_impl/opset6.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    49053 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/onnx_opset/_impl/opset7.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19393 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/onnx_opset/_impl/opset8.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    58411 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/onnx_opset/_impl/opset9.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    39030 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4439 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13894 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5368 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24713 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5875 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/onnx_types.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 00:02:28.853608 onnxscript-0.1.0.dev20240412/onnxscript/optimizer/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4288 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/optimizer/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10166 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/optimizer/constant_folding.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2872 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/optimizer/copy_propagation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15445 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/optimizer/evaluator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8554 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/optimizer/fold_constants_v0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3994 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/optimizer/remove_unused.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2080 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/optimizer/remove_unused_function.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9852 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/optimizer/simple_function_folding.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       41 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/py.typed
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 00:02:28.857608 onnxscript-0.1.0.dev20240412/onnxscript/rewriter/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1424 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/rewriter/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6698 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/rewriter/broadcast_to_matmul.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2165 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/rewriter/cast_constant_of_shape.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      686 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/rewriter/erfgelu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8844 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/rewriter/function_rule.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      756 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/rewriter/gemm_to_matmul_add.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    43596 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/rewriter/generic_pattern.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      828 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/rewriter/no_op.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 00:02:28.857608 onnxscript-0.1.0.dev20240412/onnxscript/rewriter/onnxruntime/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2216 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/rewriter/onnxruntime/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1222 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5082 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1943 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/rewriter/onnxruntime/softmax.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 00:02:28.857608 onnxscript-0.1.0.dev20240412/onnxscript/rewriter/onnxruntime/transformers/
+-rw-r--r--   0 vsts      (1001) docker     (127)      488 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/rewriter/onnxruntime/transformers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      885 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1628 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/rewriter/onnxruntime/transformers/layernorm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24688 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    39591 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/rewriter/pattern.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1700 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/sourceinfo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7658 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/tensor.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 00:02:28.857608 onnxscript-0.1.0.dev20240412/onnxscript/testing/
+-rw-r--r--   0 vsts      (1001) docker     (127)    17350 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/testing/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11025 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/type_annotation.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 00:02:28.857608 onnxscript-0.1.0.dev20240412/onnxscript/utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2239 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/utils/evaluation_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      706 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/utils/timing_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2505 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/utils/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24781 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/onnxscript/values.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 00:02:28.857608 onnxscript-0.1.0.dev20240412/onnxscript.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)    10846 2024-04-12 00:02:28.000000 onnxscript-0.1.0.dev20240412/onnxscript.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     7995 2024-04-12 00:02:28.000000 onnxscript-0.1.0.dev20240412/onnxscript.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-12 00:02:28.000000 onnxscript-0.1.0.dev20240412/onnxscript.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       35 2024-04-12 00:02:28.000000 onnxscript-0.1.0.dev20240412/onnxscript.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-04-12 00:02:28.000000 onnxscript-0.1.0.dev20240412/onnxscript.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)     6525 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-04-12 00:02:28.861608 onnxscript-0.1.0.dev20240412/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)     1292 2024-04-12 00:01:03.000000 onnxscript-0.1.0.dev20240412/setup.py
```

### Comparing `onnxscript-0.1.0.dev20240411/LICENSE` & `onnxscript-0.1.0.dev20240412/LICENSE`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/PKG-INFO` & `onnxscript-0.1.0.dev20240412/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnxscript
-Version: 0.1.0.dev20240411
+Version: 0.1.0.dev20240412
 Summary: Naturally author ONNX functions and models using a subset of Python
 Home-page: https://onnxscript.ai/
 Author-email: Microsoft Corporation <onnx@microsoft.com>
 License: MIT License
         
         Copyright (c) Microsoft Corporation
```

### Comparing `onnxscript-0.1.0.dev20240411/README.md` & `onnxscript-0.1.0.dev20240412/README.md`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/__init__.py` & `onnxscript-0.1.0.dev20240412/onnxscript/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/_internal/analysis.py` & `onnxscript-0.1.0.dev20240412/onnxscript/_internal/analysis.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/_internal/ast_utils.py` & `onnxscript-0.1.0.dev20240412/onnxscript/_internal/ast_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/_internal/autocast.py` & `onnxscript-0.1.0.dev20240412/onnxscript/_internal/autocast.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/_internal/deprecation.py` & `onnxscript-0.1.0.dev20240412/onnxscript/_internal/deprecation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/_internal/param_manipulation.py` & `onnxscript-0.1.0.dev20240412/onnxscript/_internal/param_manipulation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/_internal/runtime_typing.py` & `onnxscript-0.1.0.dev20240412/onnxscript/_internal/runtime_typing.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/_internal/utils.py` & `onnxscript-0.1.0.dev20240412/onnxscript/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/_internal/version_utils.py` & `onnxscript-0.1.0.dev20240412/onnxscript/_internal/version_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/_legacy_ir/__init__.py` & `onnxscript-0.1.0.dev20240412/onnxscript/_legacy_ir/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/_legacy_ir/irbuilder.py` & `onnxscript-0.1.0.dev20240412/onnxscript/_legacy_ir/irbuilder.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/_legacy_ir/protobuilder.py` & `onnxscript-0.1.0.dev20240412/onnxscript/_legacy_ir/protobuilder.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/_legacy_ir/visitor.py` & `onnxscript-0.1.0.dev20240412/onnxscript/_legacy_ir/visitor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/_thirdparty/asciichartpy.py` & `onnxscript-0.1.0.dev20240412/onnxscript/_thirdparty/asciichartpy.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/backend/onnx_backend.py` & `onnxscript-0.1.0.dev20240412/onnxscript/backend/onnx_backend.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/backend/onnx_export.py` & `onnxscript-0.1.0.dev20240412/onnxscript/backend/onnx_export.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/converter.py` & `onnxscript-0.1.0.dev20240412/onnxscript/converter.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/__init__.py` & `onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/_infra.py` & `onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/_infra.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/context.py` & `onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/context.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/decorator.py` & `onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/decorator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/formatter.py` & `onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/formatter.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/__init__.py` & `onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_address.py` & `onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_address.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_artifact.py` & `onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_artifact.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_artifact_change.py` & `onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_artifact_change.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_artifact_content.py` & `onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_artifact_content.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_artifact_location.py` & `onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_artifact_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_attachment.py` & `onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_attachment.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_code_flow.py` & `onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_code_flow.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_configuration_override.py` & `onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_configuration_override.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_conversion.py` & `onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_conversion.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_edge.py` & `onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_edge.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_edge_traversal.py` & `onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_edge_traversal.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_exception.py` & `onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_exception.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_external_properties.py` & `onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_external_properties.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py` & `onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py` & `onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_fix.py` & `onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_fix.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_graph.py` & `onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_graph.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_graph_traversal.py` & `onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_graph_traversal.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_invocation.py` & `onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_invocation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_location.py` & `onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_location_relationship.py` & `onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_location_relationship.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_logical_location.py` & `onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_logical_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_message.py` & `onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_message.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py` & `onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_node.py` & `onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_node.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_notification.py` & `onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_notification.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_physical_location.py` & `onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_physical_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_rectangle.py` & `onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_rectangle.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_region.py` & `onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_region.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_replacement.py` & `onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_replacement.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py` & `onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py` & `onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py` & `onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py` & `onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_result.py` & `onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_result.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_result_provenance.py` & `onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_result_provenance.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_run.py` & `onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_run.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_run_automation_details.py` & `onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_run_automation_details.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_sarif_log.py` & `onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_sarif_log.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_special_locations.py` & `onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_special_locations.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_stack.py` & `onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_stack.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_stack_frame.py` & `onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_stack_frame.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_suppression.py` & `onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_suppression.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_thread_flow.py` & `onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_thread_flow.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py` & `onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_tool.py` & `onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_tool.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_tool_component.py` & `onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_tool_component.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py` & `onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_translation_metadata.py` & `onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_translation_metadata.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_version_control_details.py` & `onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_version_control_details.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_web_request.py` & `onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_web_request.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/sarif/_web_response.py` & `onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/sarif/_web_response.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/diagnostics/infra/utils.py` & `onnxscript-0.1.0.dev20240412/onnxscript/diagnostics/infra/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/evaluator.py` & `onnxscript-0.1.0.dev20240412/onnxscript/evaluator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py` & `onnxscript-0.1.0.dev20240412/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py` & `onnxscript-0.1.0.dev20240412/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py` & `onnxscript-0.1.0.dev20240412/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/function_libs/torch_lib/_flags.py` & `onnxscript-0.1.0.dev20240412/onnxscript/function_libs/torch_lib/_flags.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/function_libs/torch_lib/graph_building.py` & `onnxscript-0.1.0.dev20240412/onnxscript/function_libs/torch_lib/graph_building.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/function_libs/torch_lib/ops/common.py` & `onnxscript-0.1.0.dev20240412/onnxscript/function_libs/torch_lib/ops/common.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/function_libs/torch_lib/ops/core.py` & `onnxscript-0.1.0.dev20240412/onnxscript/function_libs/torch_lib/ops/core.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/function_libs/torch_lib/ops/fft.py` & `onnxscript-0.1.0.dev20240412/onnxscript/function_libs/torch_lib/ops/fft.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/function_libs/torch_lib/ops/linalg.py` & `onnxscript-0.1.0.dev20240412/onnxscript/function_libs/torch_lib/ops/linalg.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/function_libs/torch_lib/ops/nested.py` & `onnxscript-0.1.0.dev20240412/onnxscript/function_libs/torch_lib/ops/nested.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/function_libs/torch_lib/ops/nn.py` & `onnxscript-0.1.0.dev20240412/onnxscript/function_libs/torch_lib/ops/nn.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/function_libs/torch_lib/ops/prims.py` & `onnxscript-0.1.0.dev20240412/onnxscript/function_libs/torch_lib/ops/prims.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/function_libs/torch_lib/ops/sparse.py` & `onnxscript-0.1.0.dev20240412/onnxscript/function_libs/torch_lib/ops/sparse.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/function_libs/torch_lib/ops/special.py` & `onnxscript-0.1.0.dev20240412/onnxscript/function_libs/torch_lib/ops/special.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/function_libs/torch_lib/ops/vision.py` & `onnxscript-0.1.0.dev20240412/onnxscript/function_libs/torch_lib/ops/vision.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/function_libs/torch_lib/registration.py` & `onnxscript-0.1.0.dev20240412/onnxscript/function_libs/torch_lib/registration.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/function_libs/torch_lib/tensor_typing.py` & `onnxscript-0.1.0.dev20240412/onnxscript/function_libs/torch_lib/tensor_typing.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/ir/__init__.py` & `onnxscript-0.1.0.dev20240412/onnxscript/ir/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     "AttrTensor",
     "AttrTensors",
     "AttrTypeProto",
     "Dimension",
     "ExternalTensor",
     "Function",
     "Graph",
+    "GraphView",
     "Input",
     "Model",
     "Node",
     "RefAttr",
     "Shape",
     "Tensor",
     "Value",
@@ -76,14 +77,15 @@
     AttrTensor,
     AttrTensors,
     AttrTypeProto,
     Dimension,
     ExternalTensor,
     Function,
     Graph,
+    GraphView,
     Input,
     Model,
     Node,
     OptionalType,
     RefAttr,
     SequenceType,
     Shape,
```

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/ir/_core.py` & `onnxscript-0.1.0.dev20240412/onnxscript/ir/_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 import numpy as np
 
 from onnxscript.ir import (
     _display,
     _enums,
     _linked_list,
     _metadata,
+    _name_authority,
     _protocols,
 )
 
 if typing.TYPE_CHECKING:
     from typing_extensions import TypeGuard
 
 TArrayCompatible = typing.TypeVar(
@@ -233,15 +234,38 @@
         array = self.numpy()
         if not IS_LITTLE_ENDIAN:
             return array.view(array.dtype.newbyteorder("<")).tobytes()
         return array.tobytes()
 
 
 class ExternalTensor(TensorBase, _protocols.TensorProtocol):
-    """A tensor with the data as external data on disk."""
+    """An immutable concrete tensor with its data store on disk.
+
+    This class uses memory mapping to avoid loading the tensor into memory,
+    when the data type is supported by numpy. Otherwise, the tensor is loaded
+    into memory lazily when accessed.
+
+    Calling :attr:`shape` does not incur IO. Checking shape before loading
+    the tensor is recommended if IO overhead and memory usage is a concern.
+
+    To obtain an array, call :meth:`numpy`. To obtain the bytes,
+    call :meth:`tobytes`.
+
+    The :attribute:`path` can be a relative path or an absolute path.
+    Serializers should handle the path correctly to conform with the ONNX spec.
+
+    Attributes:
+        path: The path to the data file. This can be a relative path or an absolute path.
+        offset: The offset in bytes from the start of the file.
+        length: The length of the data in bytes.
+        dtype: The data type of the tensor.
+        shape: The shape of the tensor.
+        name: The name of the tensor. It must be specified.
+        doc_string: The documentation string.
+    """
 
     __slots__ = (
         "_path",
         "_offset",
         "_length",
         "_dtype",
         "_shape",
@@ -258,38 +282,14 @@
         length: int | None,
         dtype: _enums.DataType,
         *,
         shape: Shape,
         name: str,
         doc_string: str | None = None,
     ) -> None:
-        """An immutable concrete tensor with its data store on disk.
-
-        This class uses memory mapping to avoid loading the tensor into memory,
-        when the data type is supported by numpy. Otherwise, the tensor is loaded
-        into memory lazily when accessed.
-
-        Calling :attr:`shape` does not incur IO. Checking shape before loading
-        the tensor is recommended if IO overhead and memory usage is a concern.
-
-        To obtain an array, call :method:`numpy`. To obtain the bytes,
-        call :method:`tobytes`.
-
-        The :attribute:`path` can be a relative path or an absolute path.
-        Serializers should handle the path correctly to conform with the ONNX spec.
-
-        Args:
-            path: The path to the data file. This can be a relative path or an absolute path.
-            offset: The offset in bytes from the start of the file.
-            length: The length of the data in bytes.
-            dtype: The data type of the tensor.
-            shape: The shape of the tensor.
-            name: The name of the tensor. It must be specified.
-            doc_string: The documentation string.
-        """
         self._path = path
         self._offset: int | None = offset
         self._length: int | None = length
         self._dtype: _enums.DataType = dtype
         self.name: str = name  # mutable
         self._shape: Shape = shape
         self.doc_string: str | None = doc_string  # mutable
@@ -346,14 +346,18 @@
     def __dlpack__(self, *, stream: Any = None) -> Any:
         return self.numpy().__dlpack__(stream=stream)
 
     def __repr__(self) -> str:
         return f"{self._repr_base()}(path='{self._path}', name={self.name!r}, offset={self._offset!r}), length={self._length!r})"
 
     def numpy(self) -> np.ndarray:
+        """Return the tensor as a numpy array.
+
+        The data will be memory mapped into memory and will not taken up physical memory space.
+        """
         if self._array is None:
             self._load()
         assert self._array is not None
         return self._array
 
     def tobytes(self) -> bytes:
         """Return the bytes of the tensor.
@@ -492,27 +496,50 @@
         """Return a string representation of the shape.
 
         E.g. [n,1,3]
         """
         return f"[{','.join([str(dim) for dim in self._dims])}]"
 
     def __eq__(self, other: object) -> bool:
-        raise NotImplementedError("Not implemented yet")
+        """Return True if the shapes are equal.
+
+        Two shapes are eqaul if all their dimensions are equal.
+        """
+        if isinstance(other, Shape):
+            return self._dims == other._dims
+        if not isinstance(other, Iterable):
+            return False
+        return self.dims == tuple(other)
+
+    def __ne__(self, other: object) -> bool:
+        return not self.__eq__(other)
 
 
 def _quoted(string: str) -> str:
     """Return a quoted string.
 
     This function is used to quote value/node names in the IR for better readability.
     """
     return f'"{string}"'
 
 
 class Node(_protocols.NodeProtocol, _display.PrettyPrintable):
-    """IR Node."""
+    """IR Node.
+
+    If the ``graph`` is provided, the node will be added to the graph. Otherwise,
+    user is responsible to call ``graph.append(node)`` (or other mutation methods
+    in :class:`Graph`) to add the node to the graph.
+
+    After the node is initialized, it will add itself as a user of the input values.
+
+    The output values of the node are created during node initialization and are immutable.
+    To change the output values, create a new node and replace the output.users.inputs with
+    the new output values by calling :meth:`replace_input_with` on the user nodes
+    of this node's outputs.
+    """
 
     __slots__ = (
         "_name",
         "_domain",
         "_op_type",
         "_inputs",
         "_outputs",
@@ -537,24 +564,14 @@
         version: int | None = None,
         graph: Graph | None = None,
         name: str | None = None,
         doc_string: str | None = None,
     ):
         """Initialize a node and add it as a user of the input values.
 
-        When the node is initialized, it does not belong to any graph. It is the
-        responsibility of the caller to add the node to a graph, by calling :func:`Graph.absorb_nodes`.
-
-        After the node is initialized, it will add itself as a user of the input values.
-
-        The output values of the node are created during node initialization and are immutable.
-        To change the output values, create a new node and replace the output.users.inputs with
-        the new output values by calling :method:`replace_input_with` on the user nodes
-        of this node's outputs.
-
         Args:
             domain: The domain of the operator. For onnx operators, this is an empty string.
             op_type: The name of the operator.
             inputs: The input values. When an input is None, it is an empty input.
             attributes: The attributes. RefAttr can be used only when the node is defined in a Function.
             overload: The overload name when the node is invoking a function.
             num_outputs: The number of outputs of the node.
@@ -585,15 +602,15 @@
         self._metadata_props: dict[str, str] | None = None
         self._graph: Graph | None = graph
         self.doc_string = doc_string
 
         # Add the node as a user of the inputs
         for i, input_value in enumerate(self._inputs):
             if input_value is not None:
-                input_value.add_user(self, i)
+                input_value._add_user(self, i)  # pylint: disable=protected-access
 
         # Add the node to the graph if graph is specified
         if self._graph is not None:
             self._graph.append(self)
 
     def __str__(self) -> str:
         node_type_text = f"{self._domain}::{self._op_type}" + f":{self._overload}" * (
@@ -685,17 +702,17 @@
         if index < 0 or index >= len(self.inputs):
             raise ValueError(f"Index out of range: {index}")
         old_input = self.inputs[index]
         self._inputs = tuple(
             value if i == index else old_input for i, old_input in enumerate(self.inputs)
         )
         if old_input is not None:
-            old_input.remove_user(self, index)
+            old_input._remove_user(self, index)  # pylint: disable=protected-access
         if value is not None:
-            value.add_user(self, index)
+            value._add_user(self, index)  # pylint: disable=protected-access
 
     def prepend(self, /, nodes: Node | Iterable[Node]) -> None:
         """Insert a node before this node in the list of nodes in the graph.
 
         It is the same as calling ``graph.insert_before(self, nodes)``.
 
         Example::
@@ -931,21 +948,33 @@
         return self._def_node
 
     def def_index(self) -> int | None:
         """The index of the output of the defining node."""
         return self._def_index
 
     def users(self) -> frozenset[tuple[Node, int]]:
+        """Return a set of users of the value.
+
+        The set contains tuples of ``(Node, index)`` where the index is the index of the input
+        of the node. For example, if ``node.inputs[1] == value``, then the user is ``(node, 1)``.
+        """
         return frozenset(self._users)
 
-    def add_user(self, user: Node, index: int) -> None:
+    def _add_user(self, user: Node, index: int) -> None:
+        """Add a user node.
+
+        This is an internal method. It should only be called by the Node class.
+        """
         self._users.add((user, index))
 
-    def remove_user(self, user: Node, index: int) -> None:
-        """Reduce a user node."""
+    def _remove_user(self, user: Node, index: int) -> None:
+        """Remove a node from the users of this value.
+
+        This is an internal method. It should only be called by the Node class.
+        """
         self._users.remove((user, index))
 
     @property
     def name(self) -> str | None:
         return self._name
 
     @name.setter
@@ -1069,23 +1098,24 @@
     The graph can be used as a sequence of nodes::
 
         for node in graph:
             print(node)
     """
 
     __slots__ = (
-        "_name",
+        "name",
         "_inputs",
         "_outputs",
         "_initializers",
         "_doc_string",
         "_opset_imports",
         "_nodes",
         "_metadata",
         "_metadata_props",
+        "_name_authority",
     )
 
     def __init__(
         self,
         inputs: Sequence[Input],
         outputs: Sequence[Value],
         *,
@@ -1105,14 +1135,17 @@
                 raise ValueError(f"Initializer must have a name: {initializer}")
         self._initializers = {tensor.name: tensor for tensor in initializers}
         self._doc_string = doc_string
         self._opset_imports = opset_imports or {}
         self._metadata: _metadata.MetadataStore | None = None
         self._metadata_props: dict[str, str] | None = None
         self._nodes: _linked_list.DoublyLinkedSet[Node] = _linked_list.DoublyLinkedSet()
+        # Be sure the initialize the name authority before extending the nodes
+        # because it is used to name the nodes and their outputs
+        self._name_authority = _name_authority.NameAuthority()
         # Call self.extend not self._nodes.extend so the graph reference is added to the nodes
         self.extend(nodes)
 
     @property
     def inputs(self) -> list[Input]:
         return self._inputs
 
@@ -1148,46 +1181,52 @@
 
     def __iter__(self) -> Iterator[Node]:
         return iter(self._nodes)
 
     def __reversed__(self) -> Iterator[Node]:
         return reversed(self._nodes)
 
-    def _set_node_graph_to_self(self, node: Node) -> Node:
-        """Set the graph reference for the node."""
+    def _set_node_graph_to_self_and_assign_names(self, node: Node) -> Node:
+        """Set the graph reference for the node and assign names to it and its outputs if they don't have one."""
         if node.graph is not None and node.graph is not self:
             raise ValueError(
                 f"The node {node} belongs to another graph. Please remove it first with Graph.remove()."
             )
+        # Give the node and its output values names if they don't not have one
+        if node.name is None:
+            self._name_authority.name_node(node)
+        for value in node._outputs:  # pylint: disable=protected-access
+            if value.name is None:
+                self._name_authority.name_value(value)
         node.graph = self
         return node
 
     # Mutation methods
     def append(self, node: Node, /) -> None:
         """Append a node to the graph in O(1) time.
 
         Args:
             node: The node to append.
 
         Raises:
             ValueError: If the node belongs to another graph.
         """
-        self._set_node_graph_to_self(node)
+        self._set_node_graph_to_self_and_assign_names(node)
         self._nodes.append(node)
 
     def extend(self, nodes: Iterable[Node], /) -> None:
         """Extend the graph with the given nodes in O(#new_nodes) time.
 
         Args:
             nodes: The nodes to extend the graph with.
 
         Raises:
             ValueError: If any node belongs to another graph.
         """
-        nodes = [self._set_node_graph_to_self(node) for node in nodes]
+        nodes = [self._set_node_graph_to_self_and_assign_names(node) for node in nodes]
         self._nodes.extend(nodes)
 
     def remove(self, node: Node, /) -> None:
         """Remove a node from the graph in O(1) time.
 
         Args:
             node: The node to remove.
@@ -1208,30 +1247,30 @@
             new_nodes: The new nodes to insert.
 
         Raises:
             ValueError: If any node belongs to another graph.
         """
         if isinstance(new_nodes, Node):
             new_nodes = (new_nodes,)
-        new_nodes = [self._set_node_graph_to_self(node) for node in new_nodes]
+        new_nodes = [self._set_node_graph_to_self_and_assign_names(node) for node in new_nodes]
         self._nodes.insert_after(node, new_nodes)
 
     def insert_before(self, node: Node, new_nodes: Iterable[Node] | Node, /) -> None:
         """Insert new nodes before the given node in O(#new_nodes) time.
 
         Args:
             node: The node to insert before.
             new_nodes: The new nodes to insert.
 
         Raises:
             ValueError: If any node belongs to another graph.
         """
         if isinstance(new_nodes, Node):
             new_nodes = (new_nodes,)
-        new_nodes = [self._set_node_graph_to_self(node) for node in new_nodes]
+        new_nodes = [self._set_node_graph_to_self_and_assign_names(node) for node in new_nodes]
         self._nodes.insert_before(node, new_nodes)
 
     def sort(self) -> None:
         """Topologically sort the nodes in the graph."""
         raise NotImplementedError("Not implemented yet")
 
     # End of mutation methods
@@ -1250,69 +1289,184 @@
     @property
     def metadata_props(self) -> dict[str, str]:
         if self._metadata_props is None:
             self._metadata_props = {}
         return self._metadata_props
 
     def __str__(self) -> str:
-        # TODO(justinchuby): Show docstrings and metadata
-        inputs_text = "\n" + ",\n".join(str(x) for x in self.inputs)
-        outputs_text = "\n" + ",\n".join(str(x) for x in self.outputs)
-        initializers_text = ",\n".join(str(x) for x in self.initializers.values())
-        if initializers_text:
-            initializers_text = (
-                "\ninitializers=(\n" + textwrap.indent(initializers_text, " " * 4) + "\n),"
-            )
-        signature = f"""\
+        return _graph_str(self)
+
+    def __repr__(self) -> str:
+        return _graph_repr(self)
+
+
+def _graph_str(graph: Graph | GraphView) -> str:
+    """Return a string representation of the graph."""
+    # TODO(justinchuby): Show docstrings and metadata
+    inputs_text = "\n" + ",\n".join(str(x) for x in graph.inputs)
+    outputs_text = "\n" + ",\n".join(str(x) for x in graph.outputs)
+    initializers_text = ",\n".join(str(x) for x in graph.initializers.values())
+    if initializers_text:
+        initializers_text = (
+            "\ninitializers=(\n" + textwrap.indent(initializers_text, " " * 4) + "\n),"
+        )
+    signature = f"""\
 graph(
-    name={self.name or ':anonymous_graph:' + str(id(self))},
-    inputs=({textwrap.indent(inputs_text, ' '*8)}
-    ),
-    outputs=({textwrap.indent(outputs_text, ' '*8)}
-    ),{textwrap.indent(initializers_text, ' '*4)}
+name={graph.name or 'anonymous_graph:' + str(id(graph))},
+inputs=({textwrap.indent(inputs_text, ' '*8)}
+),
+outputs=({textwrap.indent(outputs_text, ' '*8)}
+),{textwrap.indent(initializers_text, ' '*4)}
 )"""
-        node_count = len(self._nodes)
-        number_width = len(str(node_count))
-        node_lines = []
-        for i, node in enumerate(self._nodes):
-            node_name = node.name if node.name else f":anonymous_node:{id(node)}"
-            node_text = f"# {node_name}\n{node}"
-            indented_node_text = textwrap.indent(node_text, " " * (number_width + 4))
-            # Remove the leading spaces
-            indented_node_text = indented_node_text.strip()
-            node_lines.append(f"{i:>{number_width}} |  {indented_node_text}")
-        returns = ", ".join(str(x) for x in self.outputs)
-        body = (
-            "{\n"
-            + textwrap.indent("\n".join(node_lines), " " * 4)
-            + textwrap.indent(f"\nreturn {returns}", " " * 4)
-            + "\n}"
-        )
+    node_count = len(graph)
+    number_width = len(str(node_count))
+    node_lines = []
+    for i, node in enumerate(graph.nodes):
+        node_name = node.name if node.name else f":anonymous_node:{id(node)}"
+        node_text = f"# {node_name}\n{node}"
+        indented_node_text = textwrap.indent(node_text, " " * (number_width + 4))
+        # Remove the leading spaces
+        indented_node_text = indented_node_text.strip()
+        node_lines.append(f"{i:>{number_width}} |  {indented_node_text}")
+    returns = ", ".join(str(x) for x in graph.outputs)
+    body = (
+        "{\n"
+        + textwrap.indent("\n".join(node_lines), " " * 4)
+        + textwrap.indent(f"\nreturn {returns}", " " * 4)
+        + "\n}"
+    )
 
-        return f"{signature} {body}"
+    return f"{signature} {body}"
 
-    def __repr__(self) -> str:
-        inputs_text = "\n" + ",\n".join(str(x) for x in self.inputs)
-        outputs_text = "\n" + ",\n".join(str(x) for x in self.outputs)
-        initializers_text = ",\n".join(str(x) for x in self.initializers.values())
-        if initializers_text:
-            initializers_text = (
-                "\ninitializers=(\n" + textwrap.indent(initializers_text, " " * 4) + "\n),"
-            )
-        return f"""\
-{self.__class__.__name__}(
-    name={self.name or ':anonymous_graph:' + str(id(self))!r},
+
+def _graph_repr(graph: Graph | GraphView) -> str:
+    """Return an repr string of the graph."""
+    inputs_text = "\n" + ",\n".join(str(x) for x in graph.inputs)
+    outputs_text = "\n" + ",\n".join(str(x) for x in graph.outputs)
+    initializers_text = ",\n".join(str(x) for x in graph.initializers.values())
+    if initializers_text:
+        initializers_text = (
+            "\ninitializers=(\n" + textwrap.indent(initializers_text, " " * 4) + "\n),"
+        )
+    return f"""\
+{graph.__class__.__name__}(
+    name={graph.name or 'anonymous_graph:' + str(id(graph))!r},
     inputs=({textwrap.indent(inputs_text, ' '*8)}
     ),
     outputs=({textwrap.indent(outputs_text, ' '*8)}
     ),{textwrap.indent(initializers_text, ' '*4)}
-    len(nodes)={len(self._nodes)}
+    len()={len(graph)}
 )"""
 
 
+class GraphView(Sequence[Node], _display.PrettyPrintable):
+    """A read-only view on a graph.
+
+    The GraphView is useful for analysis of a subgraph. It can be initialized
+    with a subset of nodes from a :class:`Graph`. Creating GraphView does not
+    change the ownership of the nodes, and so it is possible to create multiple
+    GraphViews that contain the same nodes. If the underlying nodes / connections
+    are mutated, the mutation will be reflected in all views as well.
+
+    The graph view can be serialized to ONNX::
+
+            graph_proto = ir.serde.serialize_graph(graph_view)
+
+    It can also be used to create a model::
+
+            model = ir.Model(graph_view, ir_version=8)
+            model_proto = ir.serde.serialize_model(model)
+
+    The model created with a GraphView will have a fixed topology, and its graph
+    will remain read-only as a GraphView. No copying will be done during the
+    initialization process.
+
+    Attributes:
+        name: The name of the graph.
+        inputs: The input values of the graph.
+        outputs: The output values of the graph.
+        nodes: All nodes visible in this view. They do not have to be sorted.
+        initializers: The initializers in the graph.
+        doc_string: Documentation string.
+        opset_imports: Opsets imported by the graph.
+        metadata_props: Metadata.
+    """
+
+    __slots__ = (
+        "name",
+        "inputs",
+        "outputs",
+        "initializers",
+        "doc_string",
+        "opset_imports",
+        "nodes",
+        "_metadata",
+        "_metadata_props",
+    )
+
+    def __init__(
+        self,
+        inputs: Sequence[Value],
+        outputs: Sequence[Value],
+        *,
+        nodes: Iterable[Node],
+        initializers: Sequence[_protocols.TensorProtocol] = (),
+        doc_string: str | None = None,
+        opset_imports: dict[str, int] | None = None,
+        name: str | None = None,
+    ):
+        self.name = name
+        self.inputs = tuple(inputs)
+        self.outputs = tuple(outputs)
+        for initializer in initializers:
+            if initializer.name is None:
+                raise ValueError(f"Initializer must have a name: {initializer}")
+        self.initializers = {tensor.name: tensor for tensor in initializers}
+        self.doc_string = doc_string
+        self.opset_imports = opset_imports or {}
+        self._metadata: _metadata.MetadataStore | None = None
+        self._metadata_props: dict[str, str] | None = None
+        self.nodes: tuple[Node, ...] = tuple(nodes)
+
+    def __getitem__(self, index: int) -> Node:
+        return self.nodes[index]
+
+    def __len__(self) -> int:
+        return len(self.nodes)
+
+    def __iter__(self) -> Iterator[Node]:
+        return iter(self.nodes)
+
+    def __reversed__(self) -> Iterator[Node]:
+        return reversed(self.nodes)
+
+    @property
+    def meta(self) -> _metadata.MetadataStore:
+        """The metadata store for intermediate analysis.
+
+        Write to the :attribute:`metadata_props` if you would like the metadata to be serialized
+        to the ONNX proto.
+        """
+        if self._metadata is None:
+            self._metadata = _metadata.MetadataStore()
+        return self._metadata
+
+    @property
+    def metadata_props(self) -> dict[str, str]:
+        if self._metadata_props is None:
+            self._metadata_props = {}
+        return self._metadata_props
+
+    def __str__(self) -> str:
+        return _graph_str(self)
+
+    def __repr__(self) -> str:
+        return _graph_repr(self)
+
+
 class Model(_protocols.ModelProtocol, _display.PrettyPrintable):
     __slots__ = (
         "graph",
         "ir_version",
         "producer_name",
         "producer_version",
         "domain",
@@ -1336,25 +1490,25 @@
         doc_string: Documentation string.
         functions: The functions defined in the model.
         metadata_props: Metadata.
     """
 
     def __init__(
         self,
-        graph: Graph,
+        graph: Graph | GraphView,
         *,
         ir_version: int,
         producer_name: str | None = None,
         producer_version: str | None = None,
         domain: str | None = None,
         model_version: int | None = None,
         doc_string: str | None = None,
         functions: Sequence[Function] = (),
     ) -> None:
-        self.graph: Graph = graph  # type: ignore[assignment]
+        self.graph: Graph | GraphView = graph  # type: ignore[assignment]
         self.ir_version = ir_version
         self.producer_name = producer_name
         self.producer_version = producer_version
         self.domain = domain
         self.model_version = model_version
         self.doc_string = doc_string
         self._functions = {func.identifier(): func for func in functions}
@@ -1549,15 +1703,15 @@
     # End of mutation methods
 
     def __str__(self) -> str:
         full_name = f"{self.domain}::{self.name}" + f":{self.overload}" * (self.overload != "")
         inputs_text = ",\n".join(str(x) for x in self.inputs)
         outputs_text = ",\n".join(str(x) for x in self.outputs)
         attributes_text = ",\n".join(
-            attr.name + f": {attr.type}" + f"= {attr.value}" * (attr.value is None)
+            f"{attr.name}: {attr.type}" + f" = {attr.value}" * (attr.value is None)
             for attr in self.attributes.values()
         )
         if attributes_text:
             attributes_text = (
                 "\nattributes={\n" + textwrap.indent(attributes_text, " " * 4) + "\n}"
             )
         signature = f"""\
```

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/ir/_display.py` & `onnxscript-0.1.0.dev20240412/onnxscript/ir/_display.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/ir/_enums.py` & `onnxscript-0.1.0.dev20240412/onnxscript/ir/_enums.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/ir/_graph_comparison.py` & `onnxscript-0.1.0.dev20240412/onnxscript/ir/_graph_comparison.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/ir/_invariants.py` & `onnxscript-0.1.0.dev20240412/onnxscript/ir/_invariants.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/ir/_linked_list.py` & `onnxscript-0.1.0.dev20240412/onnxscript/ir/_linked_list.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/ir/_metadata.py` & `onnxscript-0.1.0.dev20240412/onnxscript/ir/_metadata.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/ir/_protocols.py` & `onnxscript-0.1.0.dev20240412/onnxscript/ir/_protocols.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import typing
 from typing import (
     AbstractSet,
     Any,
     Iterable,
     Iterator,
     Mapping,
+    MutableSequence,
     OrderedDict,
     Protocol,
     Sequence,
     Tuple,
     Union,
 )
 
@@ -125,17 +126,17 @@
     in the ONNX specification.
 
     A :class:`Value` is always not owned or owned by exactly one node. When the value is not
     owned, it must be an input of a graph or a function. ``def_node`` and ``def_index``
     are ``None``.
 
     When the value is owned by a node, it is an output of the node.
-    The node that produces the value can be accessed with :method:`def_node`.
+    The node that produces the value can be accessed with :meth:`def_node`.
     The index of the output of the node that produces the value can be accessed with
-    :method:`def_index`.
+    :meth:`def_index`.
 
     To find all the nodes that use this value as an input, call :meth:`users`.
 
     To check if the value is an output of a graph, call :meth:`is_graph_output`.
 
     Attributes:
         name: The name of the value. A value is always named when it is part of a graph.
@@ -246,16 +247,16 @@
         doc_string: Documentation string.
         opset_imports: Opsets imported by the graph.
         metadata_props: Metadata.
     """
 
     # TODO(justinchuby): Support quantization_annotation
     name: str | None
-    inputs: Sequence[ValueProtocol]
-    outputs: Sequence[ValueProtocol]
+    inputs: MutableSequence[ValueProtocol]
+    outputs: MutableSequence[ValueProtocol]
     nodes: Sequence[NodeProtocol]
     initializers: Mapping[str, TensorProtocol]
     doc_string: str
     opset_imports: Mapping[str, int]
     metadata_props: Mapping[str, str]
     meta: Mapping[str, Any]
 
@@ -287,14 +288,50 @@
 
     def sort(self) -> None:
         """Topologically sort the nodes in the graph."""
         ...
 
 
 @typing.runtime_checkable
+class GraphViewProtocol(Protocol):
+    """Protocol for a read-only view on a graph.
+
+    The GraphView is useful for analysis of a subgraph. It can be initialized
+    with a subset of nodes from a :class:`Graph`. Creating GraphView does not
+    change the ownership of the nodes, and so it is possible to create multiple
+    GraphViews that contain the same nodes.
+
+    Attributes:
+        name: The name of the graph.
+        inputs: The input values of the graph.
+        outputs: The output values of the graph.
+        nodes: All nodes this graph directly owns. They do not have to be sorted.
+        initializers: The initializers in the graph.
+        doc_string: Documentation string.
+        opset_imports: Opsets imported by the graph.
+        metadata_props: Metadata.
+    """
+
+    name: str | None
+    inputs: Sequence[ValueProtocol]
+    outputs: Sequence[ValueProtocol]
+    nodes: Sequence[NodeProtocol]
+    initializers: Mapping[str, TensorProtocol]
+    doc_string: str
+    opset_imports: Mapping[str, int]
+    metadata_props: Mapping[str, str]
+    meta: Mapping[str, Any]
+
+    def __getitem__(self, index: int) -> NodeProtocol: ...
+    def __len__(self) -> int: ...
+    def __iter__(self) -> Iterator[NodeProtocol]: ...
+    def __reversed__(self) -> Iterator[NodeProtocol]: ...
+
+
+@typing.runtime_checkable
 class ModelProtocol(Protocol):
     """Protocol for models.
 
     A model is a container for a graph and metadata. It is the top-level object
     that represents an ONNX model.
 
     Attributes:
```

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/ir/convenience.py` & `onnxscript-0.1.0.dev20240412/onnxscript/ir/convenience.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/ir/serde.py` & `onnxscript-0.1.0.dev20240412/onnxscript/ir/serde.py`

 * *Files 1% similar despite different names*

```diff
@@ -810,22 +810,25 @@
         from_: The mapping of metadata properties to serialize.
     """
     # Sort names for deterministic serialization
     for key in sorted(from_):
         string_string_entries.add(key=key, value=from_[key])
 
 
-def serialize_graph(graph: _protocols.GraphProtocol) -> onnx.GraphProto:
+def serialize_graph(
+    graph: _protocols.GraphProtocol | _protocols.GraphViewProtocol,
+) -> onnx.GraphProto:
     graph_proto = onnx.GraphProto()
     serialize_graph_into(graph_proto, from_=graph)
     return graph_proto
 
 
 def serialize_graph_into(
-    graph_proto: onnx.GraphProto, from_: _protocols.GraphProtocol
+    graph_proto: onnx.GraphProto,
+    from_: _protocols.GraphProtocol | _protocols.GraphViewProtocol,
 ) -> None:
     if from_.name:
         graph_proto.name = from_.name
     if from_.doc_string:
         graph_proto.doc_string = from_.doc_string
     for input_ in from_.inputs:
         serialize_value_into(graph_proto.input.add(), input_)
```

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/irbuilder.py` & `onnxscript-0.1.0.dev20240412/onnxscript/irbuilder.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/main.py` & `onnxscript-0.1.0.dev20240412/onnxscript/main.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/onnx_opset/__init__.py` & `onnxscript-0.1.0.dev20240412/onnxscript/onnx_opset/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/onnx_opset/_impl/opset1.py` & `onnxscript-0.1.0.dev20240412/onnxscript/onnx_opset/_impl/opset1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/onnx_opset/_impl/opset10.py` & `onnxscript-0.1.0.dev20240412/onnxscript/onnx_opset/_impl/opset10.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/onnx_opset/_impl/opset11.py` & `onnxscript-0.1.0.dev20240412/onnxscript/onnx_opset/_impl/opset11.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/onnx_opset/_impl/opset12.py` & `onnxscript-0.1.0.dev20240412/onnxscript/onnx_opset/_impl/opset12.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/onnx_opset/_impl/opset13.py` & `onnxscript-0.1.0.dev20240412/onnxscript/onnx_opset/_impl/opset13.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/onnx_opset/_impl/opset14.py` & `onnxscript-0.1.0.dev20240412/onnxscript/onnx_opset/_impl/opset14.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/onnx_opset/_impl/opset15.py` & `onnxscript-0.1.0.dev20240412/onnxscript/onnx_opset/_impl/opset15.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/onnx_opset/_impl/opset16.py` & `onnxscript-0.1.0.dev20240412/onnxscript/onnx_opset/_impl/opset16.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/onnx_opset/_impl/opset17.py` & `onnxscript-0.1.0.dev20240412/onnxscript/onnx_opset/_impl/opset17.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/onnx_opset/_impl/opset18.py` & `onnxscript-0.1.0.dev20240412/onnxscript/onnx_opset/_impl/opset18.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/onnx_opset/_impl/opset19.py` & `onnxscript-0.1.0.dev20240412/onnxscript/onnx_opset/_impl/opset19.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/onnx_opset/_impl/opset2.py` & `onnxscript-0.1.0.dev20240412/onnxscript/onnx_opset/_impl/opset2.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/onnx_opset/_impl/opset20.py` & `onnxscript-0.1.0.dev20240412/onnxscript/onnx_opset/_impl/opset20.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/onnx_opset/_impl/opset3.py` & `onnxscript-0.1.0.dev20240412/onnxscript/onnx_opset/_impl/opset3.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/onnx_opset/_impl/opset4.py` & `onnxscript-0.1.0.dev20240412/onnxscript/onnx_opset/_impl/opset4.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/onnx_opset/_impl/opset5.py` & `onnxscript-0.1.0.dev20240412/onnxscript/onnx_opset/_impl/opset5.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/onnx_opset/_impl/opset6.py` & `onnxscript-0.1.0.dev20240412/onnxscript/onnx_opset/_impl/opset6.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/onnx_opset/_impl/opset7.py` & `onnxscript-0.1.0.dev20240412/onnxscript/onnx_opset/_impl/opset7.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/onnx_opset/_impl/opset8.py` & `onnxscript-0.1.0.dev20240412/onnxscript/onnx_opset/_impl/opset8.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/onnx_opset/_impl/opset9.py` & `onnxscript-0.1.0.dev20240412/onnxscript/onnx_opset/_impl/opset9.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py` & `onnxscript-0.1.0.dev20240412/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py` & `onnxscript-0.1.0.dev20240412/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py` & `onnxscript-0.1.0.dev20240412/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py` & `onnxscript-0.1.0.dev20240412/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py` & `onnxscript-0.1.0.dev20240412/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/onnx_types.py` & `onnxscript-0.1.0.dev20240412/onnxscript/onnx_types.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/optimizer/__init__.py` & `onnxscript-0.1.0.dev20240412/onnxscript/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/optimizer/constant_folding.py` & `onnxscript-0.1.0.dev20240412/onnxscript/optimizer/constant_folding.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/optimizer/copy_propagation.py` & `onnxscript-0.1.0.dev20240412/onnxscript/optimizer/copy_propagation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/optimizer/evaluator.py` & `onnxscript-0.1.0.dev20240412/onnxscript/optimizer/evaluator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/optimizer/fold_constants_v0.py` & `onnxscript-0.1.0.dev20240412/onnxscript/optimizer/fold_constants_v0.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/optimizer/remove_unused.py` & `onnxscript-0.1.0.dev20240412/onnxscript/optimizer/remove_unused.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/optimizer/remove_unused_function.py` & `onnxscript-0.1.0.dev20240412/onnxscript/optimizer/remove_unused_function.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/optimizer/simple_function_folding.py` & `onnxscript-0.1.0.dev20240412/onnxscript/optimizer/simple_function_folding.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/rewriter/__init__.py` & `onnxscript-0.1.0.dev20240412/onnxscript/rewriter/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/rewriter/broadcast_to_matmul.py` & `onnxscript-0.1.0.dev20240412/onnxscript/rewriter/broadcast_to_matmul.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/rewriter/cast_constant_of_shape.py` & `onnxscript-0.1.0.dev20240412/onnxscript/rewriter/cast_constant_of_shape.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/rewriter/erfgelu.py` & `onnxscript-0.1.0.dev20240412/onnxscript/rewriter/erfgelu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/rewriter/function_rule.py` & `onnxscript-0.1.0.dev20240412/onnxscript/rewriter/function_rule.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/rewriter/gemm_to_matmul_add.py` & `onnxscript-0.1.0.dev20240412/onnxscript/rewriter/gemm_to_matmul_add.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/rewriter/generic_pattern.py` & `onnxscript-0.1.0.dev20240412/onnxscript/rewriter/generic_pattern.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/rewriter/no_op.py` & `onnxscript-0.1.0.dev20240412/onnxscript/rewriter/no_op.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/rewriter/onnxruntime/__init__.py` & `onnxscript-0.1.0.dev20240412/onnxscript/rewriter/onnxruntime/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py` & `onnxscript-0.1.0.dev20240412/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py` & `onnxscript-0.1.0.dev20240412/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/rewriter/onnxruntime/softmax.py` & `onnxscript-0.1.0.dev20240412/onnxscript/rewriter/onnxruntime/softmax.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py` & `onnxscript-0.1.0.dev20240412/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/rewriter/onnxruntime/transformers/layernorm.py` & `onnxscript-0.1.0.dev20240412/onnxscript/rewriter/onnxruntime/transformers/layernorm.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py` & `onnxscript-0.1.0.dev20240412/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/rewriter/pattern.py` & `onnxscript-0.1.0.dev20240412/onnxscript/rewriter/pattern.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/sourceinfo.py` & `onnxscript-0.1.0.dev20240412/onnxscript/sourceinfo.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/tensor.py` & `onnxscript-0.1.0.dev20240412/onnxscript/tensor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/testing/__init__.py` & `onnxscript-0.1.0.dev20240412/onnxscript/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/type_annotation.py` & `onnxscript-0.1.0.dev20240412/onnxscript/type_annotation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/utils/evaluation_utils.py` & `onnxscript-0.1.0.dev20240412/onnxscript/utils/evaluation_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/utils/timing_utils.py` & `onnxscript-0.1.0.dev20240412/onnxscript/utils/timing_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/utils/utils.py` & `onnxscript-0.1.0.dev20240412/onnxscript/utils/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript/values.py` & `onnxscript-0.1.0.dev20240412/onnxscript/values.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript.egg-info/PKG-INFO` & `onnxscript-0.1.0.dev20240412/onnxscript.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnxscript
-Version: 0.1.0.dev20240411
+Version: 0.1.0.dev20240412
 Summary: Naturally author ONNX functions and models using a subset of Python
 Home-page: https://onnxscript.ai/
 Author-email: Microsoft Corporation <onnx@microsoft.com>
 License: MIT License
         
         Copyright (c) Microsoft Corporation
```

### Comparing `onnxscript-0.1.0.dev20240411/onnxscript.egg-info/SOURCES.txt` & `onnxscript-0.1.0.dev20240412/onnxscript.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -122,14 +122,15 @@
 onnxscript/ir/_core.py
 onnxscript/ir/_display.py
 onnxscript/ir/_enums.py
 onnxscript/ir/_graph_comparison.py
 onnxscript/ir/_invariants.py
 onnxscript/ir/_linked_list.py
 onnxscript/ir/_metadata.py
+onnxscript/ir/_name_authority.py
 onnxscript/ir/_protocols.py
 onnxscript/ir/convenience.py
 onnxscript/ir/serde.py
 onnxscript/onnx_opset/__init__.py
 onnxscript/onnx_opset/_impl/opset1.py
 onnxscript/onnx_opset/_impl/opset10.py
 onnxscript/onnx_opset/_impl/opset11.py
```

### Comparing `onnxscript-0.1.0.dev20240411/pyproject.toml` & `onnxscript-0.1.0.dev20240412/pyproject.toml`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240411/setup.py` & `onnxscript-0.1.0.dev20240412/setup.py`

 * *Files identical despite different names*

