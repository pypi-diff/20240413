# Comparing `tmp/betterproto_rust_codec-0.1.0.tar.gz` & `tmp/betterproto_rust_codec-0.1.1.tar.gz`

## Comparing `betterproto_rust_codec-0.1.0.tar` & `betterproto_rust_codec-0.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      432 1970-01-01 00:00:00.000000 betterproto_rust_codec-0.1.0/Cargo.toml
--rw-r--r--   0     1001      127     2821 2023-12-04 19:22:19.000000 betterproto_rust_codec-0.1.0/.github/workflows/CI.yml
--rw-r--r--   0     1001      127      686 2023-12-04 19:22:19.000000 betterproto_rust_codec-0.1.0/.gitignore
--rw-r--r--   0     1001      127     1077 2023-12-04 19:22:19.000000 betterproto_rust_codec-0.1.0/LICENSE
--rw-r--r--   0     1001      127      282 2023-12-04 19:22:19.000000 betterproto_rust_codec-0.1.0/README.md
--rw-r--r--   0     1001      127      326 2023-12-04 19:22:19.000000 betterproto_rust_codec-0.1.0/betterproto_rust_codec.pyi
--rw-r--r--   0     1001      127      583 2023-12-04 19:22:19.000000 betterproto_rust_codec-0.1.0/src/betterproto_interop/error.rs
--rw-r--r--   0     1001      127     4710 2023-12-04 19:22:19.000000 betterproto_rust_codec-0.1.0/src/betterproto_interop/field_meta.rs
--rw-r--r--   0     1001      127     2915 2023-12-04 19:22:19.000000 betterproto_rust_codec-0.1.0/src/betterproto_interop/message.rs
--rw-r--r--   0     1001      127     1315 2023-12-04 19:22:19.000000 betterproto_rust_codec-0.1.0/src/betterproto_interop/message_class.rs
--rw-r--r--   0     1001      127     1575 2023-12-04 19:22:19.000000 betterproto_rust_codec-0.1.0/src/betterproto_interop/message_meta.rs
--rw-r--r--   0     1001      127      759 2023-12-04 19:22:19.000000 betterproto_rust_codec-0.1.0/src/betterproto_interop/mod.rs
--rw-r--r--   0     1001      127     3714 2023-12-04 19:22:19.000000 betterproto_rust_codec-0.1.0/src/decode/custom_message.rs
--rw-r--r--   0     1001      127      720 2023-12-04 19:22:19.000000 betterproto_rust_codec-0.1.0/src/decode/error.rs
--rw-r--r--   0     1001      127     1442 2023-12-04 19:22:19.000000 betterproto_rust_codec-0.1.0/src/decode/field.rs
--rw-r--r--   0     1001      127     1178 2023-12-04 19:22:19.000000 betterproto_rust_codec-0.1.0/src/decode/map_entry.rs
--rw-r--r--   0     1001      127     1390 2023-12-04 19:22:19.000000 betterproto_rust_codec-0.1.0/src/decode/mod.rs
--rw-r--r--   0     1001      127    10559 2023-12-04 19:22:19.000000 betterproto_rust_codec-0.1.0/src/decode/value.rs
--rw-r--r--   0     1001      127     2330 2023-12-04 19:22:19.000000 betterproto_rust_codec-0.1.0/src/descriptors.rs
--rw-r--r--   0     1001      127     2274 2023-12-04 19:22:19.000000 betterproto_rust_codec-0.1.0/src/encode/chunk.rs
--rw-r--r--   0     1001      127      862 2023-12-04 19:22:19.000000 betterproto_rust_codec-0.1.0/src/encode/error.rs
--rw-r--r--   0     1001      127    14769 2023-12-04 19:22:19.000000 betterproto_rust_codec-0.1.0/src/encode/message.rs
--rw-r--r--   0     1001      127      124 2023-12-04 19:22:19.000000 betterproto_rust_codec-0.1.0/src/encode/mod.rs
--rw-r--r--   0     1001      127      917 2023-12-04 19:22:19.000000 betterproto_rust_codec-0.1.0/src/lib.rs
--rw-r--r--   0     1001      127     8366 2023-12-04 19:22:19.000000 betterproto_rust_codec-0.1.0/src/well_known_types.rs
--rw-r--r--   0     1001      127     9455 2023-12-04 19:22:19.000000 betterproto_rust_codec-0.1.0/Cargo.lock
--rw-r--r--   0     1001      127      718 2023-12-04 19:22:19.000000 betterproto_rust_codec-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      934 1970-01-01 00:00:00.000000 betterproto_rust_codec-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      460 1970-01-01 00:00:00.000000 betterproto_rust_codec-0.1.1/Cargo.toml
+-rw-r--r--   0     1001      127     2821 2024-04-13 13:08:24.000000 betterproto_rust_codec-0.1.1/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127      686 2024-04-13 13:08:24.000000 betterproto_rust_codec-0.1.1/.gitignore
+-rw-r--r--   0     1001      127     1077 2024-04-13 13:08:24.000000 betterproto_rust_codec-0.1.1/LICENSE
+-rw-r--r--   0     1001      127      282 2024-04-13 13:08:24.000000 betterproto_rust_codec-0.1.1/README.md
+-rw-r--r--   0     1001      127      326 2024-04-13 13:08:24.000000 betterproto_rust_codec-0.1.1/betterproto_rust_codec.pyi
+-rw-r--r--   0     1001      127      583 2024-04-13 13:08:24.000000 betterproto_rust_codec-0.1.1/src/betterproto_interop/error.rs
+-rw-r--r--   0     1001      127     4619 2024-04-13 13:08:24.000000 betterproto_rust_codec-0.1.1/src/betterproto_interop/field_meta.rs
+-rw-r--r--   0     1001      127     2943 2024-04-13 13:08:24.000000 betterproto_rust_codec-0.1.1/src/betterproto_interop/message.rs
+-rw-r--r--   0     1001      127     1259 2024-04-13 13:08:24.000000 betterproto_rust_codec-0.1.1/src/betterproto_interop/message_class.rs
+-rw-r--r--   0     1001      127     1623 2024-04-13 13:08:24.000000 betterproto_rust_codec-0.1.1/src/betterproto_interop/message_meta.rs
+-rw-r--r--   0     1001      127      759 2024-04-13 13:08:24.000000 betterproto_rust_codec-0.1.1/src/betterproto_interop/mod.rs
+-rw-r--r--   0     1001      127     3715 2024-04-13 13:08:24.000000 betterproto_rust_codec-0.1.1/src/decode/custom_message.rs
+-rw-r--r--   0     1001      127      833 2024-04-13 13:08:24.000000 betterproto_rust_codec-0.1.1/src/decode/error.rs
+-rw-r--r--   0     1001      127     1442 2024-04-13 13:08:24.000000 betterproto_rust_codec-0.1.1/src/decode/field.rs
+-rw-r--r--   0     1001      127     1178 2024-04-13 13:08:24.000000 betterproto_rust_codec-0.1.1/src/decode/map_entry.rs
+-rw-r--r--   0     1001      127     1430 2024-04-13 13:08:24.000000 betterproto_rust_codec-0.1.1/src/decode/mod.rs
+-rw-r--r--   0     1001      127    10629 2024-04-13 13:08:24.000000 betterproto_rust_codec-0.1.1/src/decode/value.rs
+-rw-r--r--   0     1001      127     2556 2024-04-13 13:08:24.000000 betterproto_rust_codec-0.1.1/src/descriptors.rs
+-rw-r--r--   0     1001      127     2274 2024-04-13 13:08:24.000000 betterproto_rust_codec-0.1.1/src/encode/chunk.rs
+-rw-r--r--   0     1001      127     1077 2024-04-13 13:08:24.000000 betterproto_rust_codec-0.1.1/src/encode/error.rs
+-rw-r--r--   0     1001      127    14860 2024-04-13 13:08:24.000000 betterproto_rust_codec-0.1.1/src/encode/message.rs
+-rw-r--r--   0     1001      127      118 2024-04-13 13:08:24.000000 betterproto_rust_codec-0.1.1/src/encode/mod.rs
+-rw-r--r--   0     1001      127      931 2024-04-13 13:08:24.000000 betterproto_rust_codec-0.1.1/src/lib.rs
+-rw-r--r--   0     1001      127     7258 2024-04-13 13:08:24.000000 betterproto_rust_codec-0.1.1/src/well_known_types.rs
+-rw-r--r--   0     1001      127    15779 2024-04-13 13:08:24.000000 betterproto_rust_codec-0.1.1/Cargo.lock
+-rw-r--r--   0     1001      127      718 2024-04-13 13:08:24.000000 betterproto_rust_codec-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      934 1970-01-01 00:00:00.000000 betterproto_rust_codec-0.1.1/PKG-INFO
```

### Comparing `betterproto_rust_codec-0.1.0/.github/workflows/CI.yml` & `betterproto_rust_codec-0.1.1/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `betterproto_rust_codec-0.1.0/.gitignore` & `betterproto_rust_codec-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `betterproto_rust_codec-0.1.0/LICENSE` & `betterproto_rust_codec-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `betterproto_rust_codec-0.1.0/src/betterproto_interop/error.rs` & `betterproto_rust_codec-0.1.1/src/betterproto_interop/error.rs`

 * *Files identical despite different names*

### Comparing `betterproto_rust_codec-0.1.0/src/betterproto_interop/field_meta.rs` & `betterproto_rust_codec-0.1.1/src/betterproto_interop/field_meta.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,49 +1,50 @@
+use std::ops::Deref;
+
 use super::{
     error::{InteropError, InteropResult},
     message_class::BetterprotoMessageClass,
     message_meta::BetterprotoMessageMeta,
     BetterprotoEnumClass,
 };
 use crate::{
     descriptors::{FieldAttribute, FieldDescriptor, ProtoType},
     Str,
 };
-use pyo3::{FromPyObject, IntoPy, Python};
+use pyo3::{types::PyTypeMethods, FromPyObject};
 
 #[derive(FromPyObject)]
 pub struct BetterprotoFieldMeta {
     pub number: u32,
     pub map_types: Option<(String, String)>,
     pub proto_type: String,
     pub wraps: Option<String>,
     pub optional: bool,
 }
 
 impl BetterprotoFieldMeta {
     pub fn into_descriptor(
         self,
-        py: Python,
         field_name: Str,
         msg_meta: &BetterprotoMessageMeta,
     ) -> InteropResult<FieldDescriptor> {
         if let Some((key_type, value_type)) = self.map_types {
             let key_type = convert_key_type(&key_type)?;
             let value_type =
-                convert_value_type(py, &value_type, &format!("{field_name}.value"), msg_meta)?;
+                convert_value_type(&value_type, &format!("{field_name}.value"), msg_meta)?;
             return Ok(FieldDescriptor {
                 name: field_name,
                 attribute: FieldAttribute::Map(key_type),
                 value_type,
             });
         }
 
         let value_type = match self.wraps {
             Some(wrapped_type) => convert_wrapped_type(&wrapped_type)?,
-            None => convert_value_type(py, &self.proto_type, &field_name, msg_meta)?,
+            None => convert_value_type(&self.proto_type, &field_name, msg_meta)?,
         };
 
         let attribute = if self.optional {
             FieldAttribute::Optional
         } else if let Some(group) = msg_meta.oneof_group_by_field.get(field_name.as_ref()) {
             FieldAttribute::Group(Str::from(group.as_ref()))
         } else if msg_meta.is_list_field(&field_name)? {
@@ -57,15 +58,14 @@
             value_type,
             attribute,
         })
     }
 }
 
 fn convert_value_type(
-    py: Python,
     type_name: &str,
     field_name: &str,
     msg_meta: &BetterprotoMessageMeta,
 ) -> InteropResult<ProtoType> {
     match type_name {
         "bool" => Ok(ProtoType::Bool),
         "int32" => Ok(ProtoType::Int32),
@@ -79,27 +79,25 @@
         "fixed32" => Ok(ProtoType::Fixed32),
         "sfixed32" => Ok(ProtoType::Sfixed32),
         "fixed64" => Ok(ProtoType::Fixed64),
         "sfixed64" => Ok(ProtoType::Sfixed64),
         "string" => Ok(ProtoType::String),
         "bytes" => Ok(ProtoType::Bytes),
         "enum" => Ok(ProtoType::Enum(BetterprotoEnumClass(
-            msg_meta.get_class(field_name)?.into_py(py),
+            msg_meta.get_class(field_name)?.clone().unbind(),
         ))),
         "message" => {
             let cls = msg_meta.get_class(field_name)?;
-            if cls.getattr("__module__")?.extract::<&str>()? == "datetime" {
-                match cls.name()? {
-                    "datetime" => return Ok(ProtoType::Timestamp),
-                    "timedelta" => return Ok(ProtoType::Duration),
-                    _ => {}
-                }
+            match cls.name()?.deref() {
+                "datetime.datetime" => return Ok(ProtoType::Timestamp),
+                "datetime.timedelta" => return Ok(ProtoType::Duration),
+                _ => {}
             }
             Ok(ProtoType::CustomMessage(BetterprotoMessageClass(
-                cls.into_py(py),
+                cls.clone().unbind(),
             )))
         }
         _ => Err(InteropError::UnsupportedValueType(type_name.to_string())),
     }
 }
 
 fn convert_key_type(type_name: &str) -> InteropResult<ProtoType> {
```

### Comparing `betterproto_rust_codec-0.1.0/src/betterproto_interop/message.rs` & `betterproto_rust_codec-0.1.1/src/betterproto_interop/message.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 use super::{error::InteropResult, BetterprotoMessageClass};
 use indoc::indoc;
 use pyo3::{
     intern,
     sync::GILOnceCell,
-    types::{PyBytes, PyModule},
-    FromPyObject, IntoPy, PyAny, PyObject, Python, ToPyObject,
+    types::{PyAnyMethods, PyBytes, PyModule},
+    Bound, FromPyObject, PyAny, PyObject, Python, ToPyObject,
 };
 
-#[derive(FromPyObject, Clone, Copy)]
-pub struct BetterprotoMessage<'py>(pub(super) &'py PyAny);
+#[derive(FromPyObject, Clone)]
+pub struct BetterprotoMessage<'py>(pub(super) Bound<'py, PyAny>);
 
 impl<'py> BetterprotoMessage<'py> {
     pub fn class(&self) -> BetterprotoMessageClass {
-        BetterprotoMessageClass(self.0.get_type().into_py(self.0.py()))
+        BetterprotoMessageClass(self.0.get_type().unbind())
     }
 
-    pub fn py(&self) -> Python {
+    pub fn py(&self) -> Python<'py> {
         self.0.py()
     }
 
     pub fn set_field(&self, field_name: &str, value: impl ToPyObject) -> InteropResult<()> {
         self.0.setattr(field_name, value)?;
         Ok(())
     }
 
-    pub fn get_field(&'py self, field_name: &str) -> InteropResult<Option<&'py PyAny>> {
+    pub fn get_field(&self, field_name: &str) -> InteropResult<Option<Bound<'py, PyAny>>> {
         let py = self.py();
         static GETTER_CACHE: GILOnceCell<PyObject> = GILOnceCell::new();
         let getter = GETTER_CACHE
             .get_or_init(py, || {
-                PyModule::from_code(
+                PyModule::from_code_bound(
                     py,
                     indoc! {"
                         from betterproto import PLACEHOLDER
 
                         def getter(msg, field_name):
                             value = msg._Message__raw_get(field_name)
                             if value is PLACEHOLDER:
@@ -44,27 +44,27 @@
                     "",
                 )
                 .expect("This is a valid Python module")
                 .getattr("getter")
                 .expect("Attribute exists")
                 .to_object(py)
             })
-            .as_ref(py);
+            .bind(py);
 
-        let res = getter.call1((self.0, field_name))?.extract()?;
+        let res = getter.call1((self.0.clone(), field_name))?.extract()?;
         Ok(res)
     }
 
     pub fn append_unknown_fields(&self, mut data: Vec<u8>) -> InteropResult<()> {
         let attr_name = intern!(self.py(), "_unknown_fields");
         if !data.is_empty() {
             let mut unknown_fields = self.0.getattr(attr_name)?.extract::<Vec<u8>>()?;
             unknown_fields.append(&mut data);
             self.0
-                .setattr(attr_name, PyBytes::new(self.py(), &unknown_fields))?;
+                .setattr(attr_name, PyBytes::new_bound(self.py(), &unknown_fields))?;
         }
         Ok(())
     }
 
     pub fn get_unknown_fields(&self) -> InteropResult<Vec<u8>> {
         Ok(self
             .0
```

### Comparing `betterproto_rust_codec-0.1.0/src/betterproto_interop/message_class.rs` & `betterproto_rust_codec-0.1.1/src/lib.rs`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,32 @@
-use super::{
-    error::InteropResult, message::BetterprotoMessage, message_meta::BetterprotoMessageMeta,
-};
-use crate::descriptors::MessageDescriptor;
-use pyo3::{intern, pyclass, types::PyType, FromPyObject, Py, PyCell, Python};
+mod betterproto_interop;
+mod decode;
+mod descriptors;
+mod encode;
+mod well_known_types;
 
-#[derive(FromPyObject, Debug)]
-pub struct BetterprotoMessageClass(pub(super) Py<PyType>);
+use betterproto_interop::BetterprotoMessage;
+use decode::{merge_into_message, DecodeResult};
+use encode::{EncodeResult, MessageEncoder};
+use pyo3::{prelude::*, types::PyBytes};
+use std::sync::Arc;
 
-impl BetterprotoMessageClass {
-    pub fn create_instance<'py>(
-        &'py self,
-        py: Python<'py>,
-    ) -> InteropResult<BetterprotoMessage<'py>> {
-        Ok(BetterprotoMessage(self.0.as_ref(py).call0()?))
-    }
+pub type Str = Arc<str>;
 
-    pub fn descriptor<'py>(&'py self, py: Python<'py>) -> InteropResult<&'py MessageDescriptor> {
-        let cls = self.0.as_ref(py);
-        if let Ok(attr) = cls.getattr(intern!(py, "_betterproto_rust_codec")) {
-            if let Ok(cell) = attr.downcast::<PyCell<DescriptorWrapper>>() {
-                return Ok(&cell.get().0);
-            }
-        }
+#[pyfunction]
+fn deserialize(obj: BetterprotoMessage, mut buf: &[u8]) -> DecodeResult<()> {
+    merge_into_message(&obj, &mut buf)
+}
 
-        let desc = cls
-            .call0()?
-            .getattr(intern!(py, "_betterproto"))?
-            .extract::<BetterprotoMessageMeta>()?
-            .into_descriptor(py)?;
-        let cell = PyCell::new(py, DescriptorWrapper(desc))?;
-        cls.setattr(intern!(py, "_betterproto_rust_codec"), cell)?;
-        Ok(&cell.get().0)
-    }
+#[pyfunction]
+fn serialize<'py>(py: Python<'py>, msg: BetterprotoMessage) -> EncodeResult<Bound<'py, PyBytes>> {
+    let cls = msg.class();
+    let encoder = MessageEncoder::from_betterproto_msg(msg, cls.descriptor(py)?.get())?;
+    Ok(PyBytes::new_bound(py, &encoder.into_vec()))
 }
 
-#[pyclass(frozen)]
-struct DescriptorWrapper(MessageDescriptor);
+#[pymodule]
+fn betterproto_rust_codec(m: &Bound<PyModule>) -> PyResult<()> {
+    m.add_function(wrap_pyfunction!(deserialize, m)?)?;
+    m.add_function(wrap_pyfunction!(serialize, m)?)?;
+    Ok(())
+}
```

### Comparing `betterproto_rust_codec-0.1.0/src/betterproto_interop/message_meta.rs` & `betterproto_rust_codec-0.1.1/src/betterproto_interop/message_meta.rs`

 * *Files 16% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 use std::collections::HashMap;
 
 use pyo3::{
-    types::{PyDict, PyList, PyType},
-    FromPyObject, PyAny, Python,
+    types::{PyAnyMethods, PyDict, PyDictMethods, PyList, PyType},
+    Bound, FromPyObject, PyAny,
 };
 
 use crate::descriptors::MessageDescriptor;
 
 use super::{
     error::{InteropError, InteropResult},
     field_meta::BetterprotoFieldMeta,
 };
 
 #[derive(FromPyObject)]
 pub struct BetterprotoMessageMeta<'py> {
-    pub cls_by_field: HashMap<String, &'py PyType>,
-    pub meta_by_field_name: &'py PyDict,
+    pub cls_by_field: HashMap<String, Bound<'py, PyType>>,
+    pub meta_by_field_name: Bound<'py, PyDict>,
     pub oneof_group_by_field: HashMap<String, String>,
-    pub default_gen: HashMap<String, &'py PyAny>,
+    pub default_gen: HashMap<String, Bound<'py, PyAny>>,
 }
 
 impl<'py> BetterprotoMessageMeta<'py> {
     pub fn is_list_field(&self, field_name: &str) -> InteropResult<bool> {
         let cls = self
             .default_gen
             .get(field_name)
             .ok_or(InteropError::IncompleteMetadata)?;
-        Ok(cls.is(cls.py().get_type::<PyList>()))
+        Ok(cls.is(&cls.py().get_type_bound::<PyList>()))
     }
 
-    pub fn get_class(&self, field_name: &str) -> InteropResult<&'py PyType> {
+    pub fn get_class(&self, field_name: &str) -> InteropResult<&Bound<'py, PyType>> {
         let cls = self
             .cls_by_field
             .get(field_name)
             .ok_or(InteropError::IncompleteMetadata)?;
         Ok(cls)
     }
 
-    pub fn into_descriptor(self, py: Python) -> InteropResult<MessageDescriptor> {
+    pub fn into_descriptor(self) -> InteropResult<MessageDescriptor> {
         let fields = self
             .meta_by_field_name
             .iter()
             .map(|(name, meta)| {
                 let name = name.extract::<String>()?;
                 let meta = meta.extract::<BetterprotoFieldMeta>()?;
-                Ok((meta.number, meta.into_descriptor(py, name.into(), &self)?))
+                Ok((meta.number, meta.into_descriptor(name.into(), &self)?))
             })
             .collect::<InteropResult<Vec<_>>>()?;
         Ok(MessageDescriptor { fields })
     }
 }
```

### Comparing `betterproto_rust_codec-0.1.0/src/betterproto_interop/mod.rs` & `betterproto_rust_codec-0.1.1/src/betterproto_interop/mod.rs`

 * *Files identical despite different names*

### Comparing `betterproto_rust_codec-0.1.0/src/decode/custom_message.rs` & `betterproto_rust_codec-0.1.1/src/decode/custom_message.rs`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
                 .map(|(tag, descriptor)| (*tag, FieldBuilder::new(py, descriptor)))
                 .collect(),
             active_groups: HashMap::new(),
             unknown_fields: Vec::new(),
         }
     }
 
-    pub fn merge_into(self, msg: BetterprotoMessage) -> InteropResult<()> {
+    pub fn merge_into(self, msg: &BetterprotoMessage) -> InteropResult<()> {
         for (name, value) in self
             .fields
             .into_values()
             .filter_map(|field| field.into_result())
         {
             msg.set_field(name, value)?;
         }
```

### Comparing `betterproto_rust_codec-0.1.0/src/decode/error.rs` & `betterproto_rust_codec-0.1.1/src/decode/error.rs`

 * *Files 13% similar despite different names*

```diff
@@ -8,14 +8,16 @@
     Interop(#[from] InteropError),
     #[error("The given binary data does not match the protobuf schema.")]
     ProstDecode(#[from] prost::DecodeError),
     #[error("The given binary data does not match the protobuf schema.")]
     InvalidMapEntryTag,
     #[error("The given binary data is not a valid protobuf message.")]
     InvalidData,
+    #[error("Decoded timestamp {0} is out of bounds.")]
+    TimestampOutOfBounds(chrono::DateTime<chrono::Utc>),
 }
 
 pub type DecodeResult<T> = Result<T, DecodeError>;
 
 impl From<DecodeError> for PyErr {
     fn from(value: DecodeError) -> Self {
         PyRuntimeError::new_err(value.to_string())
```

### Comparing `betterproto_rust_codec-0.1.0/src/decode/field.rs` & `betterproto_rust_codec-0.1.1/src/decode/field.rs`

 * *Files identical despite different names*

### Comparing `betterproto_rust_codec-0.1.0/src/decode/map_entry.rs` & `betterproto_rust_codec-0.1.1/src/decode/map_entry.rs`

 * *Files identical despite different names*

### Comparing `betterproto_rust_codec-0.1.0/src/decode/mod.rs` & `betterproto_rust_codec-0.1.1/src/decode/mod.rs`

 * *Files 4% similar despite different names*

```diff
@@ -8,18 +8,19 @@
 pub use self::error::{DecodeError, DecodeResult};
 use crate::betterproto_interop::BetterprotoMessage;
 use prost::{
     bytes::Buf,
     encoding::{check_wire_type, decode_varint, WireType},
 };
 
-pub fn merge_into_message(msg: BetterprotoMessage, buf: &mut impl Buf) -> DecodeResult<()> {
+pub fn merge_into_message(msg: &BetterprotoMessage, buf: &mut impl Buf) -> DecodeResult<()> {
     let py = msg.py();
     let cls = msg.class();
-    let mut builder = CustomMessageBuilder::new(py, cls.descriptor(py)?);
+    let descriptor = cls.descriptor(py)?;
+    let mut builder = CustomMessageBuilder::new(py, descriptor.get());
     while buf.has_remaining() {
         builder.parse_next_field(buf)?;
     }
     builder.merge_into(msg)?;
     Ok(())
 }
```

### Comparing `betterproto_rust_codec-0.1.0/src/decode/value.rs` & `betterproto_rust_codec-0.1.1/src/decode/value.rs`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
     pub fn into_object(self) -> Option<PyObject> {
         let py = self.py;
         match self.value {
             Value::Unset => None,
             Value::Single(obj) => Some(obj),
             Value::Repeated(ls) => Some(ls.to_object(py)),
-            Value::Map(ls) => Some(ls.into_py_dict(py).to_object(py)),
+            Value::Map(ls) => Some(ls.into_py_dict_bound(py).to_object(py)),
         }
     }
 
     pub fn into_object_or_default(self) -> DecodeResult<PyObject> {
         let py = self.py;
         let proto_type = self.proto_type;
         self.into_object()
@@ -140,15 +140,15 @@
             let mut value = Default::default();
             enc::bool::merge(wire_type, &mut value, buf, ctx)?;
             Ok(value.into_py(py))
         }
         ProtoType::Bytes => {
             let mut value = vec![];
             enc::bytes::merge(wire_type, &mut value, buf, ctx)?;
-            Ok(PyBytes::new(py, &value).to_object(py))
+            Ok(PyBytes::new_bound(py, &value).to_object(py))
         }
         ProtoType::Double => {
             let mut value = Default::default();
             enc::double::merge(wire_type, &mut value, buf, ctx)?;
             Ok(value.into_py(py))
         }
         ProtoType::Float => {
@@ -213,31 +213,32 @@
         }
         ProtoType::Enum(cls) => {
             let mut value = Default::default();
             enc::int32::merge(wire_type, &mut value, buf, ctx)?;
             Ok(cls.create_instance(py, value)?)
         }
         ProtoType::CustomMessage(cls) => {
-            let mut builder = CustomMessageBuilder::new(py, cls.descriptor(py)?);
+            let descriptor = cls.descriptor(py)?;
+            let mut builder = CustomMessageBuilder::new(py, descriptor.get());
             builder.parse_next_length_delimited(wire_type, buf)?;
             let msg = cls.create_instance(py)?;
-            builder.merge_into(msg)?;
+            builder.merge_into(&msg)?;
             Ok(msg.to_object(py))
         }
         ProtoType::BoolValue => Ok(BoolValue::decode_length_delimited(buf)?.to_object(py)),
         ProtoType::BytesValue => Ok(BytesValue::decode_length_delimited(buf)?.to_object(py)),
         ProtoType::DoubleValue => Ok(DoubleValue::decode_length_delimited(buf)?.to_object(py)),
         ProtoType::FloatValue => Ok(FloatValue::decode_length_delimited(buf)?.to_object(py)),
         ProtoType::Int32Value => Ok(Int32Value::decode_length_delimited(buf)?.to_object(py)),
         ProtoType::Int64Value => Ok(Int64Value::decode_length_delimited(buf)?.to_object(py)),
         ProtoType::UInt32Value => Ok(UInt32Value::decode_length_delimited(buf)?.to_object(py)),
         ProtoType::UInt64Value => Ok(UInt64Value::decode_length_delimited(buf)?.to_object(py)),
         ProtoType::StringValue => Ok(StringValue::decode_length_delimited(buf)?.to_object(py)),
-        ProtoType::Timestamp => Ok(Timestamp::decode_length_delimited(buf)?.to_object(py)),
-        ProtoType::Duration => Ok(Duration::decode_length_delimited(buf)?.to_object(py)),
+        ProtoType::Timestamp => Ok(Timestamp::decode_length_delimited(buf)?.try_to_object(py)?),
+        ProtoType::Duration => Ok(Duration::decode_length_delimited(buf)?.try_to_object(py)?),
     }
 }
 
 fn try_parse_next_packed(
     py: Python,
     proto_type: &ProtoType,
     buf: &mut impl Buf,
```

### Comparing `betterproto_rust_codec-0.1.0/src/descriptors.rs` & `betterproto_rust_codec-0.1.1/src/descriptors.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 use pyo3::{
+    pyclass,
     types::{PyBytes, PyString},
     PyObject, Python, ToPyObject,
 };
 
 use crate::{
     betterproto_interop::{BetterprotoEnumClass, BetterprotoMessageClass, InteropResult},
     well_known_types::{Duration, Timestamp},
     Str,
 };
 
 #[derive(Debug)]
+#[pyclass(frozen)]
 pub struct MessageDescriptor {
     pub fields: Vec<(u32, FieldDescriptor)>,
 }
 
 #[derive(Debug)]
 pub struct FieldDescriptor {
     pub name: Str,
@@ -62,36 +64,40 @@
     Timestamp,
 }
 
 impl ProtoType {
     pub fn default_value(&self, py: Python) -> InteropResult<PyObject> {
         match self {
             Self::Bool => Ok(false.to_object(py)),
-            Self::Bytes => Ok(PyBytes::new(py, &[]).to_object(py)),
+            Self::Bytes => Ok(PyBytes::new_bound(py, &[]).to_object(py)),
             Self::Double | Self::Float => Ok(0_f64.to_object(py)),
             Self::Int32
             | Self::Int64
             | Self::Sint32
             | Self::Sint64
             | Self::Uint32
             | Self::Uint64
             | Self::Fixed32
             | Self::Fixed64
             | Self::Sfixed32
             | Self::Sfixed64 => Ok(0_i64.to_object(py)),
-            Self::String => Ok(PyString::new(py, "").to_object(py)),
+            Self::String => Ok(PyString::new_bound(py, "").to_object(py)),
             Self::Enum(cls) => cls.create_instance(py, 0),
             Self::CustomMessage(cls) => Ok(cls.create_instance(py)?.to_object(py)),
             Self::BoolValue
             | Self::BytesValue
             | Self::FloatValue
             | Self::DoubleValue
             | Self::Int32Value
             | Self::Int64Value
             | Self::StringValue
             | Self::UInt32Value
             | Self::UInt64Value => Ok(py.None()),
-            Self::Timestamp => Ok(Timestamp::default().to_object(py)),
-            Self::Duration => Ok(Duration::default().to_object(py)),
+            Self::Timestamp => Ok(Timestamp::default()
+                .try_to_object(py)
+                .expect("Default converts into valid Python object.")),
+            Self::Duration => Ok(Duration::default()
+                .try_to_object(py)
+                .expect("Default converts into valid Python object.")),
         }
     }
 }
```

### Comparing `betterproto_rust_codec-0.1.0/src/encode/chunk.rs` & `betterproto_rust_codec-0.1.1/src/encode/chunk.rs`

 * *Files identical despite different names*

### Comparing `betterproto_rust_codec-0.1.0/src/encode/error.rs` & `betterproto_rust_codec-0.1.1/src/encode/error.rs`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 use crate::betterproto_interop::InteropError;
-use pyo3::{exceptions::PyRuntimeError, PyDowncastError, PyErr};
+use pyo3::{exceptions::PyRuntimeError, DowncastError, PyErr};
 use thiserror::Error;
 
 #[derive(Error, Debug)]
 pub enum EncodeError {
-    #[error("Given object is not a valid betterproto message.")]
-    NoBetterprotoMessage(#[from] PyErr),
+    #[error(transparent)]
+    PythonInteropFailed(#[from] PyErr),
     #[error("Given object is not a valid betterproto message.")]
     DowncastFailed,
     #[error(transparent)]
     Interop(#[from] InteropError),
     #[error("Given object is not a valid betterproto message.")]
     ProstEncode(#[from] prost::EncodeError),
+    #[error("Offset-naive datetime {0} is invalid for the current local timezone.")]
+    OffsetNaiveDateTimeDoesNotMap(chrono::NaiveDateTime),
 }
 
 pub type EncodeResult<T> = Result<T, EncodeError>;
 
-impl From<PyDowncastError<'_>> for EncodeError {
-    fn from(_: PyDowncastError) -> Self {
+impl From<DowncastError<'_, '_>> for EncodeError {
+    fn from(_: DowncastError) -> Self {
         Self::DowncastFailed
     }
 }
 
 impl From<EncodeError> for PyErr {
     fn from(value: EncodeError) -> Self {
-        PyRuntimeError::new_err(value.to_string())
+        if let EncodeError::PythonInteropFailed(pyerr) = value {
+            pyerr
+        } else {
+            PyRuntimeError::new_err(value.to_string())
+        }
     }
 }
```

### Comparing `betterproto_rust_codec-0.1.0/src/encode/message.rs` & `betterproto_rust_codec-0.1.1/src/encode/message.rs`

 * *Files 1% similar despite different names*

```diff
@@ -6,29 +6,29 @@
         BoolValue, BytesValue, DoubleValue, Duration, FloatValue, Int32Value, Int64Value,
         StringValue, Timestamp, UInt32Value, UInt64Value,
     },
 };
 use prost::{encoding as enc, Message};
 use pyo3::{
     intern,
-    types::{PyDict, PyList},
-    PyAny, PyResult,
+    types::{PyAnyMethods, PyDict, PyDictMethods, PyList, PyListMethods},
+    Bound, PyAny, PyResult,
 };
 
 pub struct MessageEncoder(Vec<Chunk>);
 
 impl MessageEncoder {
     pub fn from_betterproto_msg(
         msg: BetterprotoMessage,
         descriptor: &MessageDescriptor,
     ) -> EncodeResult<Self> {
         let mut encoder = MessageEncoder::new();
         for (tag, field) in descriptor.fields.iter() {
             if let Some(value) = msg.get_field(&field.name)? {
-                encoder.load_field(*tag, field, value)?;
+                encoder.load_field(*tag, field, &value)?;
             }
         }
         encoder.load_unknown_fields(msg.get_unknown_fields()?);
         Ok(encoder)
     }
 
     pub fn into_vec(self) -> Vec<u8> {
@@ -60,43 +60,42 @@
         self.0.push(Chunk::from_encoded(unknowns))
     }
 
     fn load_field(
         &mut self,
         tag: u32,
         descriptor: &FieldDescriptor,
-        value: &PyAny,
+        value: &Bound<PyAny>,
     ) -> EncodeResult<()> {
         match &descriptor.attribute {
             FieldAttribute::Repeated => {
                 if !self.try_load_packed(tag, &descriptor.value_type, value)? {
                     for value in value.downcast::<PyList>()?.iter() {
-                        self.load_single::<false>(tag, &descriptor.value_type, value)?;
+                        self.load_single::<false>(tag, &descriptor.value_type, &value)?;
                     }
                 }
             }
             FieldAttribute::Map(key_type) => {
                 for (key, value) in value.downcast::<PyDict>()?.iter() {
-                    self.load_map_entry(tag, key_type, &descriptor.value_type, key, value)?;
+                    self.load_map_entry(tag, key_type, &descriptor.value_type, &key, &value)?;
                 }
             }
             FieldAttribute::None => self.load_single::<true>(tag, &descriptor.value_type, value)?,
             _ => self.load_single::<false>(tag, &descriptor.value_type, value)?,
         }
 
         Ok(())
     }
 
     fn load_single<const SKIP_DEFAULT: bool>(
         &mut self,
         tag: u32,
         proto_type: &ProtoType,
-        value: &PyAny,
+        value: &Bound<PyAny>,
     ) -> EncodeResult<()> {
-        let py = value.py();
         let chunk = match proto_type {
             ProtoType::Bool => {
                 let value: bool = value.extract()?;
                 if SKIP_DEFAULT && !value {
                     return Ok(());
                 }
                 Chunk::from_encoder(tag, &value, enc::bool::encoded_len, enc::bool::encode)?
@@ -207,30 +206,30 @@
                 if SKIP_DEFAULT && value == 0 {
                     return Ok(());
                 }
                 Chunk::from_encoder(tag, &value, enc::uint64::encoded_len, enc::uint64::encode)?
             }
             ProtoType::Enum(_) => {
                 let value: i32 = value
-                    .getattr(intern!(py, "value"))
-                    .unwrap_or(value)
+                    .getattr(intern!(value.py(), "value"))
+                    .unwrap_or(value.clone())
                     .extract()?;
                 if SKIP_DEFAULT && value == 0 {
                     return Ok(());
                 }
                 Chunk::from_encoder(tag, &value, enc::int32::encoded_len, enc::int32::encode)?
             }
             ProtoType::CustomMessage(cls) => {
                 let msg: BetterprotoMessage = value.extract()?;
                 if SKIP_DEFAULT && !msg.should_be_serialized()? {
                     return Ok(());
                 }
                 Chunk::from_message(
                     tag,
-                    MessageEncoder::from_betterproto_msg(msg, cls.descriptor(py)?)?,
+                    MessageEncoder::from_betterproto_msg(msg, cls.descriptor(value.py())?.get())?,
                 )
             }
             ProtoType::BoolValue => Chunk::from_known_message::<BoolValue>(tag, value.extract()?)?,
             ProtoType::BytesValue => {
                 Chunk::from_known_message::<BytesValue>(tag, value.extract()?)?
             }
             ProtoType::DoubleValue => {
@@ -274,15 +273,15 @@
         Ok(())
     }
 
     fn try_load_packed(
         &mut self,
         tag: u32,
         proto_type: &ProtoType,
-        value: &PyAny,
+        value: &Bound<PyAny>,
     ) -> EncodeResult<bool> {
         let chunk = match proto_type {
             ProtoType::Bool => Some(Chunk::from_encoder(
                 tag,
                 value.extract::<Vec<_>>()?.as_ref(),
                 enc::bool::encoded_len_packed,
                 enc::bool::encode_packed,
@@ -387,16 +386,16 @@
     }
 
     fn load_map_entry(
         &mut self,
         tag: u32,
         key_type: &ProtoType,
         value_type: &ProtoType,
-        key: &PyAny,
-        value: &PyAny,
+        key: &Bound<PyAny>,
+        value: &Bound<PyAny>,
     ) -> EncodeResult<()> {
         let mut encoder = MessageEncoder::new();
         encoder.load_single::<true>(1, key_type, key)?;
         encoder.load_single::<true>(2, value_type, value)?;
         self.0.push(Chunk::from_message(tag, encoder));
         Ok(())
     }
```

### Comparing `betterproto_rust_codec-0.1.0/src/well_known_types.rs` & `betterproto_rust_codec-0.1.1/src/well_known_types.rs`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,22 @@
-use indoc::indoc;
+use chrono::Datelike;
 use prost::Message;
 use pyo3::{
-    sync::GILOnceCell,
-    types::{PyBytes, PyModule},
+    prelude::Bound,
+    types::{PyAnyMethods, PyBytes},
     FromPyObject, PyAny, PyObject, PyResult, Python, ToPyObject,
 };
 
+use crate::{
+    decode::{DecodeError, DecodeResult},
+    encode::{EncodeError, EncodeResult},
+};
+
+const NANOS_PER_SEC: u32 = 1_000_000_000;
+
 #[derive(Message)]
 pub struct BoolValue {
     #[prost(bool, tag = "1")]
     pub value: bool,
 }
 
 #[derive(Message)]
@@ -73,164 +80,184 @@
     #[prost(int64, tag = "1")]
     pub seconds: i64,
     #[prost(int32, tag = "2")]
     pub nanos: i32,
 }
 
 impl<'py> FromPyObject<'py> for BoolValue {
-    fn extract(ob: &'py PyAny) -> PyResult<Self> {
+    fn extract_bound(ob: &Bound<'py, PyAny>) -> PyResult<Self> {
         let res = BoolValue {
             value: ob.extract()?,
         };
         Ok(res)
     }
 }
 
 impl<'py> FromPyObject<'py> for BytesValue {
-    fn extract(ob: &'py PyAny) -> PyResult<Self> {
+    fn extract_bound(ob: &Bound<'py, PyAny>) -> PyResult<Self> {
         let res = BytesValue {
             value: ob.extract()?,
         };
         Ok(res)
     }
 }
 
 impl<'py> FromPyObject<'py> for DoubleValue {
-    fn extract(ob: &'py PyAny) -> PyResult<Self> {
+    fn extract_bound(ob: &Bound<'py, PyAny>) -> PyResult<Self> {
         let res = DoubleValue {
             value: ob.extract()?,
         };
         Ok(res)
     }
 }
 
 impl<'py> FromPyObject<'py> for FloatValue {
-    fn extract(ob: &'py PyAny) -> PyResult<Self> {
+    fn extract_bound(ob: &Bound<'py, PyAny>) -> PyResult<Self> {
         let res = FloatValue {
             value: ob.extract()?,
         };
         Ok(res)
     }
 }
 
 impl<'py> FromPyObject<'py> for Int32Value {
-    fn extract(ob: &'py PyAny) -> PyResult<Self> {
+    fn extract_bound(ob: &Bound<'py, PyAny>) -> PyResult<Self> {
         let res = Int32Value {
             value: ob.extract()?,
         };
         Ok(res)
     }
 }
 
 impl<'py> FromPyObject<'py> for Int64Value {
-    fn extract(ob: &'py PyAny) -> PyResult<Self> {
+    fn extract_bound(ob: &Bound<'py, PyAny>) -> PyResult<Self> {
         let res = Int64Value {
             value: ob.extract()?,
         };
         Ok(res)
     }
 }
 
 impl<'py> FromPyObject<'py> for UInt32Value {
-    fn extract(ob: &'py PyAny) -> PyResult<Self> {
+    fn extract_bound(ob: &Bound<'py, PyAny>) -> PyResult<Self> {
         let res = UInt32Value {
             value: ob.extract()?,
         };
         Ok(res)
     }
 }
 
 impl<'py> FromPyObject<'py> for UInt64Value {
-    fn extract(ob: &'py PyAny) -> PyResult<Self> {
+    fn extract_bound(ob: &Bound<'py, PyAny>) -> PyResult<Self> {
         let res = UInt64Value {
             value: ob.extract()?,
         };
         Ok(res)
     }
 }
 
 impl<'py> FromPyObject<'py> for StringValue {
-    fn extract(ob: &'py PyAny) -> PyResult<Self> {
+    fn extract_bound(ob: &Bound<'py, PyAny>) -> PyResult<Self> {
         let res = StringValue {
             value: ob.extract()?,
         };
         Ok(res)
     }
 }
 
+impl From<chrono::TimeDelta> for Duration {
+    fn from(value: chrono::TimeDelta) -> Self {
+        Self {
+            seconds: value.num_seconds(),
+            nanos: value.subsec_nanos(),
+        }
+    }
+}
+
 impl<'py> FromPyObject<'py> for Duration {
-    fn extract(ob: &'py PyAny) -> PyResult<Self> {
-        let py = ob.py();
-        static DECONSTRUCTOR_CACHE: GILOnceCell<PyObject> = GILOnceCell::new();
-        let deconstructor = DECONSTRUCTOR_CACHE
-            .get_or_init(py, || {
-                PyModule::from_code(
-                    py,
-                    indoc! {"
-                        from datetime import timedelta
-                        
-                        def deconstructor(delta, *, _1_microsecond = timedelta(microseconds=1)):
-                            total_ms = delta // _1_microsecond
-                            seconds = int(total_ms / 1e6)
-                            nanos = int((total_ms % 1e6) * 1e3)
-                            return (seconds, nanos)
-                    "},
-                    "",
-                    "",
-                )
-                .expect("This is a valid Python module")
-                .getattr("deconstructor")
-                .expect("Attribute exists")
-                .to_object(py)
-            })
-            .as_ref(py);
-        let (seconds, nanos) = deconstructor.call1((ob,))?.extract()?;
-        let res = Duration { seconds, nanos };
-        Ok(res)
+    fn extract_bound(ob: &Bound<'py, PyAny>) -> PyResult<Self> {
+        Ok(ob.extract::<chrono::TimeDelta>()?.into())
+    }
+}
+
+impl TryFrom<&Duration> for chrono::Duration {
+    type Error = DecodeError;
+
+    fn try_from(value: &Duration) -> Result<Self, Self::Error> {
+        let (secs, nanos) = if value.nanos < 0 {
+            (value.seconds - 1, value.nanos + NANOS_PER_SEC as i32)
+        } else {
+            (value.seconds, value.nanos)
+        };
+        let nanos = u32::try_from(nanos).map_err(|_| DecodeError::InvalidData)?;
+        chrono::Duration::new(secs, nanos).ok_or(DecodeError::InvalidData)
+    }
+}
+
+impl Duration {
+    pub fn try_to_object(&self, py: Python) -> DecodeResult<PyObject> {
+        Ok(chrono::TimeDelta::try_from(self)?.to_object(py))
+    }
+}
+
+impl Timestamp {
+    fn try_from_any(ob: &Bound<PyAny>) -> EncodeResult<Self> {
+        // try to extract an offset-aware datetime object
+        if let Ok(dt) = ob.extract::<chrono::DateTime<chrono::FixedOffset>>() {
+            return Ok(dt.to_utc().into());
+        }
+
+        // fallback to extract an offset-naive datetime object, interpreted relative to the user's local timezone
+        let dt = ob.extract::<chrono::NaiveDateTime>()?;
+        Ok(dt
+            .and_local_timezone(chrono::Local)
+            .single()
+            .ok_or(EncodeError::OffsetNaiveDateTimeDoesNotMap(dt))?
+            .to_utc()
+            .into())
+    }
+
+    pub fn try_to_object(&self, py: Python) -> DecodeResult<PyObject> {
+        let nanos = u32::try_from(self.nanos).map_err(|_| DecodeError::InvalidData)?;
+        let dt = chrono::DateTime::from_timestamp(self.seconds, nanos)
+            .ok_or(DecodeError::InvalidData)?;
+        if !(1..=9999).contains(&dt.year()) {
+            return Err(DecodeError::TimestampOutOfBounds(dt));
+        }
+        Ok(dt.to_object(py))
+    }
+}
+
+impl From<chrono::DateTime<chrono::Utc>> for Timestamp {
+    fn from(value: chrono::DateTime<chrono::Utc>) -> Self {
+        let nanos = value.timestamp_subsec_nanos();
+        debug_assert!(nanos < NANOS_PER_SEC, "Python datetimes do not have leap seconds, so this value should always satisfy the Protobuf specification.");
+
+        Self {
+            seconds: value.timestamp(),
+            nanos: nanos as i32,
+        }
     }
 }
 
 impl<'py> FromPyObject<'py> for Timestamp {
-    fn extract(ob: &'py PyAny) -> PyResult<Self> {
-        let py = ob.py();
-        static DECONSTRUCTOR_CACHE: GILOnceCell<PyObject> = GILOnceCell::new();
-        let deconstructor = DECONSTRUCTOR_CACHE
-            .get_or_init(py, || {
-                PyModule::from_code(
-                    py,
-                    indoc! {"
-                        def deconstructor(dt):
-                            seconds = int(dt.timestamp())
-                            nanos = int(dt.microsecond * 1e3)
-                            return (seconds, nanos)
-                    "},
-                    "",
-                    "",
-                )
-                .expect("This is a valid Python module")
-                .getattr("deconstructor")
-                .expect("Attribute exists")
-                .to_object(py)
-            })
-            .as_ref(py);
-        let (seconds, nanos) = deconstructor.call1((ob,))?.extract()?;
-        let res = Timestamp { seconds, nanos };
-        Ok(res)
+    fn extract_bound(ob: &Bound<'py, PyAny>) -> PyResult<Self> {
+        Ok(Self::try_from_any(ob)?)
     }
 }
 
 impl ToPyObject for BoolValue {
     fn to_object(&self, py: Python) -> PyObject {
         self.value.to_object(py)
     }
 }
 
 impl ToPyObject for BytesValue {
     fn to_object(&self, py: Python) -> PyObject {
-        PyBytes::new(py, &self.value).to_object(py)
+        PyBytes::new_bound(py, &self.value).to_object(py)
     }
 }
 
 impl ToPyObject for DoubleValue {
     fn to_object(&self, py: Python) -> PyObject {
         self.value.to_object(py)
     }
@@ -267,60 +294,7 @@
 }
 
 impl ToPyObject for StringValue {
     fn to_object(&self, py: Python) -> PyObject {
         self.value.to_object(py)
     }
 }
-
-impl ToPyObject for Duration {
-    fn to_object(&self, py: Python) -> PyObject {
-        static CONSTRUCTOR_CACHE: GILOnceCell<PyObject> = GILOnceCell::new();
-        let constructor = CONSTRUCTOR_CACHE.get_or_init(py, || {
-            PyModule::from_code(
-                py,
-                indoc! {"
-                    from datetime import timedelta
-                    
-                    def constructor(s, ms):
-                        return timedelta(seconds=s, microseconds=ms)
-                "},
-                "",
-                "",
-            )
-            .expect("This is a valid Python module")
-            .getattr("constructor")
-            .expect("Attribute exists")
-            .to_object(py)
-        });
-        constructor
-            .call1(py, (self.seconds as f64, (self.nanos as f64) / 1e3))
-            .expect("static function will not fail")
-    }
-}
-
-impl ToPyObject for Timestamp {
-    fn to_object(&self, py: Python) -> PyObject {
-        static CONSTRUCTOR_CACHE: GILOnceCell<PyObject> = GILOnceCell::new();
-        let constructor = CONSTRUCTOR_CACHE.get_or_init(py, || {
-            PyModule::from_code(
-                py,
-                indoc! {"
-                    from datetime import datetime, timezone
-                    
-                    def constructor(ts):
-                        return datetime.fromtimestamp(ts, tz=timezone.utc)
-                "},
-                "",
-                "",
-            )
-            .expect("This is a valid Python module")
-            .getattr("constructor")
-            .expect("Attribute exists")
-            .to_object(py)
-        });
-        let ts = (self.seconds as f64) + (self.nanos as f64) / 1e9;
-        constructor
-            .call1(py, (ts,))
-            .expect("static function will not fail")
-    }
-}
```

### Comparing `betterproto_rust_codec-0.1.0/pyproject.toml` & `betterproto_rust_codec-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `betterproto_rust_codec-0.1.0/PKG-INFO` & `betterproto_rust_codec-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: betterproto-rust-codec
-Version: 0.1.0
+Version: 0.1.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Fast conversion between betterproto messages and Protobuf wire format.
 Author-email: Erik Friese <e.friese0@gmail.com>
 License: MIT
```

