# Comparing `tmp/layrz-forms-1.0.9.tar.gz` & `tmp/layrz-forms-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "layrz-forms-1.0.9.tar", last modified: Mon Nov  6 20:15:25 2023, max compression
+gzip compressed data, was "layrz-forms-2.0.0.tar", last modified: Fri Apr 12 23:42:08 2024, max compression
```

## Comparing `layrz-forms-1.0.9.tar` & `layrz-forms-2.0.0.tar`

### file list

```diff
@@ -1,24 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-06 20:15:25.833826 layrz-forms-1.0.9/
--rw-rw-r--   0 root         (0) root         (0)     1052 2023-11-06 20:14:33.000000 layrz-forms-1.0.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3094 2023-11-06 20:15:25.833826 layrz-forms-1.0.9/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     2321 2023-11-06 20:14:33.000000 layrz-forms-1.0.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-06 20:15:25.829826 layrz-forms-1.0.9/layrz/
--rw-rw-r--   0 root         (0) root         (0)      213 2023-11-06 20:14:33.000000 layrz-forms-1.0.9/layrz/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-06 20:15:25.829826 layrz-forms-1.0.9/layrz/forms/
--rw-rw-r--   0 root         (0) root         (0)     5934 2023-11-06 20:14:33.000000 layrz-forms-1.0.9/layrz/forms/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-06 20:15:25.829826 layrz-forms-1.0.9/layrz/forms/fields/
--rw-rw-r--   0 root         (0) root         (0)       19 2023-11-06 20:14:33.000000 layrz-forms-1.0.9/layrz/forms/fields/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1275 2023-11-06 20:14:33.000000 layrz-forms-1.0.9/layrz/forms/fields/base.py
--rw-rw-r--   0 root         (0) root         (0)      845 2023-11-06 20:14:33.000000 layrz-forms-1.0.9/layrz/forms/fields/boolean.py
--rw-rw-r--   0 root         (0) root         (0)     2558 2023-11-06 20:14:33.000000 layrz-forms-1.0.9/layrz/forms/fields/char.py
--rw-rw-r--   0 root         (0) root         (0)     1508 2023-11-06 20:14:33.000000 layrz-forms-1.0.9/layrz/forms/fields/email.py
--rw-rw-r--   0 root         (0) root         (0)     1171 2023-11-06 20:14:33.000000 layrz-forms-1.0.9/layrz/forms/fields/id.py
--rw-rw-r--   0 root         (0) root         (0)     1564 2023-11-06 20:14:33.000000 layrz-forms-1.0.9/layrz/forms/fields/json.py
--rw-rw-r--   0 root         (0) root         (0)     2203 2023-11-06 20:14:33.000000 layrz-forms-1.0.9/layrz/forms/fields/number.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-06 20:15:25.833826 layrz-forms-1.0.9/layrz_forms.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3094 2023-11-06 20:15:25.000000 layrz-forms-1.0.9/layrz_forms.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      438 2023-11-06 20:15:25.000000 layrz-forms-1.0.9/layrz_forms.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-11-06 20:15:25.000000 layrz-forms-1.0.9/layrz_forms.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-11-06 20:15:25.000000 layrz-forms-1.0.9/layrz_forms.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)     7622 2023-11-06 20:14:33.000000 layrz-forms-1.0.9/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-11-06 20:15:25.833826 layrz-forms-1.0.9/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 23:42:08.614047 layrz-forms-2.0.0/
+-rw-rw-r--   0 root         (0) root         (0)     1052 2024-04-12 23:41:13.000000 layrz-forms-2.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3086 2024-04-12 23:42:08.614047 layrz-forms-2.0.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     2313 2024-04-12 23:41:13.000000 layrz-forms-2.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 23:42:08.614047 layrz-forms-2.0.0/layrz_forms/
+-rw-rw-r--   0 root         (0) root         (0)     6220 2024-04-12 23:41:13.000000 layrz-forms-2.0.0/layrz_forms/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 23:42:08.614047 layrz-forms-2.0.0/layrz_forms/fields/
+-rw-rw-r--   0 root         (0) root         (0)      605 2024-04-12 23:41:13.000000 layrz-forms-2.0.0/layrz_forms/fields/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1377 2024-04-12 23:41:13.000000 layrz-forms-2.0.0/layrz_forms/fields/base.py
+-rw-rw-r--   0 root         (0) root         (0)      873 2024-04-12 23:41:13.000000 layrz-forms-2.0.0/layrz_forms/fields/boolean.py
+-rw-rw-r--   0 root         (0) root         (0)     2627 2024-04-12 23:41:13.000000 layrz-forms-2.0.0/layrz_forms/fields/char.py
+-rw-rw-r--   0 root         (0) root         (0)     1555 2024-04-12 23:41:13.000000 layrz-forms-2.0.0/layrz_forms/fields/email.py
+-rw-rw-r--   0 root         (0) root         (0)     1209 2024-04-12 23:41:13.000000 layrz-forms-2.0.0/layrz_forms/fields/id.py
+-rw-rw-r--   0 root         (0) root         (0)     1618 2024-04-12 23:41:13.000000 layrz-forms-2.0.0/layrz_forms/fields/json.py
+-rw-rw-r--   0 root         (0) root         (0)     2263 2024-04-12 23:41:13.000000 layrz-forms-2.0.0/layrz_forms/fields/number.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 23:42:08.614047 layrz-forms-2.0.0/layrz_forms.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3086 2024-04-12 23:42:08.000000 layrz-forms-2.0.0/layrz_forms.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      420 2024-04-12 23:42:08.000000 layrz-forms-2.0.0/layrz_forms.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 23:42:08.000000 layrz-forms-2.0.0/layrz_forms.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-04-12 23:42:08.000000 layrz-forms-2.0.0/layrz_forms.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)     7634 2024-04-12 23:41:13.000000 layrz-forms-2.0.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-12 23:42:08.614047 layrz-forms-2.0.0/setup.cfg
```

### Comparing `layrz-forms-1.0.9/LICENSE` & `layrz-forms-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `layrz-forms-1.0.9/PKG-INFO` & `layrz-forms-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: layrz-forms
-Version: 1.0.9
+Version: 2.0.0
 Summary: Layrz forms and tools for Python
 Author-email: "Golden M, Inc." <software@goldenm.com>
 Maintainer-email: Kenny Mochizuki <kenny@goldenm.com>, Miguel Zauzich <miguel@goldenm.com>
 License: MIT License
 Project-URL: Repository, https://github.com/goldenm-software/layrz-forms
 Project-URL: Changelog, https://github.com/goldenm-software/layrz-forms/blob/main/CHANGELOG.md
 Keywords: sdk,goldenm,layrz,django forms,django,forms
@@ -22,15 +22,15 @@
 ## Motivation
 This project is a collection of tools that we use to make django developers life easier. I hope you find them useful too.
 
 ## Usage
 The idea is simple, replace the django forms to a more easier way to use them. Also provide the ability to return the errors key to support i18n.
 
 ```python
-import layrz.forms as forms
+import layrz_forms as forms
 
 
 class ExampleForm(forms.Form):
   """ Example form """
   id_test = forms.IdField(required=True)
   email_text = forms.EmailField(required=True)
   json_list_test = forms.JsonField(required=True, datatype=list)
@@ -75,11 +75,11 @@
   #> form.errors(): {'rangeTextTest': [{'code': 'minLength', 'expected': 5, 'received': 4}], 'clean1': [{'code': 'error1'}, {'code': 'error2'}], 'clean2': [{'code': 'error1'}]}
 ```
 
 ## Work with us
 Golden M is a software/hardware development company what is working on
 a new, innovative and disruptive technologies.
 
-For more information, contact us at [sales@goldenmcorp.com](mailto:sales@goldenmcorp.com)
+For more information, contact us at [sales@goldenm.com](mailto:sales@goldenm.com)
 
 ## License
 This project is under MIT License, for more information, check out the `LICENCE`
```

### Comparing `layrz-forms-1.0.9/README.md` & `layrz-forms-2.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 ## Motivation
 This project is a collection of tools that we use to make django developers life easier. I hope you find them useful too.
 
 ## Usage
 The idea is simple, replace the django forms to a more easier way to use them. Also provide the ability to return the errors key to support i18n.
 
 ```python
-import layrz.forms as forms
+import layrz_forms as forms
 
 
 class ExampleForm(forms.Form):
   """ Example form """
   id_test = forms.IdField(required=True)
   email_text = forms.EmailField(required=True)
   json_list_test = forms.JsonField(required=True, datatype=list)
@@ -57,11 +57,11 @@
   #> form.errors(): {'rangeTextTest': [{'code': 'minLength', 'expected': 5, 'received': 4}], 'clean1': [{'code': 'error1'}, {'code': 'error2'}], 'clean2': [{'code': 'error1'}]}
 ```
 
 ## Work with us
 Golden M is a software/hardware development company what is working on
 a new, innovative and disruptive technologies.
 
-For more information, contact us at [sales@goldenmcorp.com](mailto:sales@goldenmcorp.com)
+For more information, contact us at [sales@goldenm.com](mailto:sales@goldenm.com)
 
 ## License
 This project is under MIT License, for more information, check out the `LICENCE`
```

### Comparing `layrz-forms-1.0.9/layrz/forms/__init__.py` & `layrz-forms-2.0.0/layrz_forms/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,12 @@
-""" Init file """
+""" Layrz Forms """
 import inspect
+from typing import Any
 
-from .fields.base import Field
-from .fields.boolean import BooleanField
-from .fields.char import CharField
-from .fields.email import EmailField
-from .fields.id import IdField
-from .fields.json import JsonField
-from .fields.number import NumberField
+from .fields import (BooleanField, CharField, EmailField, Field, IdField, JsonField, NumberField)
 
 
 class Form:
   """
   Form class
   ---
   Notes:
@@ -21,75 +16,89 @@
   _obj = {}
   _errors = {}
   _clean_functions = []
   _attributes = {}
   _nested_attrs = {}
   _sub_forms_attrs = {}
 
-  def __init__(self, obj=dict):
+  def __init__(self, obj: dict = None):
     """ Constructor """
-    self._obj = obj
+    self._obj = obj if obj is not None else {}
+
     self.calculate_members()
 
   @property
-  def cleaned_data(self):
+  def cleaned_data(self) -> dict:
     """ Returns the cleaned data """
     return self._obj
 
-  def calculate_members(self):
+  def calculate_members(self) -> None:
     """ Calculate members """
     self._errors = {}
     self._clean_functions = []
     self._attributes = {}
     self._nested_attrs = {}
     self._sub_forms_attrs = {}
 
     for item in inspect.getmembers(self):
       if item[0] in self._reserverd_words:
         continue
       if item[0].startswith('_'):
         continue
-      elif item[0].startswith('clean'):
+
+      if item[0].startswith('clean'):
         self._clean_functions.append(item[0])
-      elif isinstance(item[1], Field):
+        continue
+
+      if isinstance(item[1], Field):
         self._attributes[item[0]] = item[1]
-      elif isinstance(item[1], list):
+        continue
+
+      if isinstance(item[1], list):
         self._nested_attrs[item[0]] = item[1]
-      elif isinstance(item[1], Form):
+        continue
+
+      if isinstance(item[1], Form):
         self._sub_forms_attrs[item[0]] = item[1]
-      else:
-        print('Unknown field', item[0])
+        continue
 
-  def set_obj(self, obj):
+  def set_obj(self, obj: dict) -> None:
     """ Set the object """
     self._obj = obj
 
-  def is_valid(self):
+  def is_valid(self) -> bool:
     """ Returns if the form is valid """
     self._errors = {}
 
     for field in self._attributes.items():
       self._validate_field(field=field)
 
     for field, form in self._sub_forms_attrs.items():
       self._validate_sub_form(field=field, form=form, data=self._obj.get(field, {}))
 
     for field, form in self._nested_attrs.items():
-      self._validate_sub_form_as_list(field=field, form=form[0])
+      if isinstance(form[0], Field):
+        self._validate_sub_form(
+          field=field,
+          form=form[0],
+          data=self._obj.get(field, {}),
+        )
+      else:
+        self._validate_sub_form_as_list(field=field, form=form[0])
 
     for func in self._clean_functions:
       self._clean(clean_func=func)
 
     return len(self._errors) == 0
 
-  def errors(self):
+  def errors(self) -> dict:
     """ Returns the list of errors """
     return self._errors
 
-  def add_errors(self, key='', code='', extra_args=dict):
+  def add_errors(self, key: str = '', code: str = '', extra_args: dict = None) -> None:
     """ Add custom errors
     This function is designed to be used in a clean function
     ---
     Arguments
       key: str
         Key of the field
       code: str
@@ -108,15 +117,15 @@
     if extra_args and isinstance(extra_args, dict):
       if callable(extra_args):
         extra_args = extra_args()
 
       new_error.update(extra_args)
     self._errors[camel_key].append(new_error)
 
-  def _validate_field(self, field, new_key=None):
+  def _validate_field(self, field: tuple, new_key: str = None) -> None:
     """ Validate field """
     if isinstance(field[1], Field):
       func = getattr(field[1], 'validate')
       if callable(func):
         # Validate if the validate function has the correct parameters
         params = [p for p, _ in inspect.signature(func).parameters.items()]
         valid_params = ['key', 'value', 'errors']
@@ -143,68 +152,69 @@
           key=field[0] if new_key is None else new_key,
           value=self._obj.get(field[0], None),
           errors=self._errors,
         )
       else:
         raise Exception(f'{type(field[1])} has no validate method')  #pylint: disable=W0719
 
-  def _clean(self, clean_func):
+  def _clean(self, clean_func: str) -> None:
     """ Clean function """
     func = getattr(self, clean_func)
     if callable(func):
       func()
 
-  def _convert_to_camel(self, key):
+  def _convert_to_camel(self, key: str) -> str:
     """
     Convert the key to camel case
     """
     init, *temp = key.split('_')
 
     field = ''.join([init, *map(str.title, temp)])
     field_items = field.split('.')
 
     field_final = []
     for item in field_items:
       field_final.append(''.join([item[0].lower(), item[1:]]))
 
     return '.'.join(field_final)
 
-  def _validate_sub_form(self, field, form, data):
+  def _validate_sub_form(self, field: str, form: Any, data: dict) -> None:
     """ Validate sub form """
     if not isinstance(form, Form):
       return
+
     form.set_obj(data)
     form.calculate_members()
     if not form.is_valid():
       for key, errors in form.errors().items():
         for error in errors:
           code = error['code']
           del error['code']
           self.add_errors(key=f'{field}.{key}', code=code, extra_args=error)
 
-  def _validate_sub_form_as_list(self, field, form):
+  def _validate_sub_form_as_list(self, field: str, form: Any) -> None:
     """ Validate sub form for list """
     list_obj = self._obj.get(field, [])
 
     if isinstance(list_obj, (list, tuple)):
       for i, obj in enumerate(list_obj):
-        if isinstance(obj, Field):
+        if isinstance(form, Field):
           self._validate_field(
             field=obj,
             new_key=f'{field}.{i}',
           )
-        elif isinstance(obj, Form):
+        elif isinstance(form, Form):
           self._validate_sub_form(
             field=f'{field}.{i}',
             form=form,
             data=obj,
           )
 
   @property
-  def _reserverd_words(self):
+  def _reserverd_words(self) -> tuple[str]:
     """ Reserved words """
     return (
       'add_errors',
       'change_obj',
       'clean',
       'errors',
       'is_valid',
```

### Comparing `layrz-forms-1.0.9/layrz/forms/fields/base.py` & `layrz-forms-2.0.0/layrz_forms/fields/base.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """ Base class for the fields """
 
+from typing import Any
+
 
 class Field:
   """ Field abstract class """
 
-  def __init__(self, required=False):
+  def __init__(self, required: bool = False) -> None:
     self.required = required
 
-  def validate(self, key, value, errors):
+  def validate(self, key: str, value: Any, errors: dict) -> None:
     """ Validate is the field is blank or None if is required
     ---
     Arguments
       key: str
         Key of the field
       value: any
         Value to validate
@@ -19,30 +21,30 @@
         Dict of errors
     """
 
     if self.required:
       if value is None:
         self._append_error(key=key, errors=errors, to_add={'code': 'required'})
 
-  def _convert_to_camel(self, key):
+  def _convert_to_camel(self, key: str) -> str:
     """
     Convert the key to camel case
     """
     init, *temp = key.split('_')
 
     field = ''.join([init, *map(str.title, temp)])
-    field_items = field.split(".")
+    field_items = field.split('.')
 
     field_final = []
     for item in field_items:
       field_final.append(''.join([item[0].lower(), item[1:]]))
 
     return '.'.join(field_final)
 
-  def _append_error(self, key, errors, to_add):
+  def _append_error(self, key: str, errors: dict, to_add: dict) -> None:
     """
     Append an error to a dict of errors
     ---
     Arguments
       key: str
         Key of the error
       errors: dict
@@ -51,8 +53,8 @@
         Error to add
     """
 
     key = self._convert_to_camel(key=key)
     if key in errors:
       errors[key].append(to_add)
     else:
-      errors[key] = [to_add]
+      errors[key] = [to_add]
```

### Comparing `layrz-forms-1.0.9/layrz/forms/fields/boolean.py` & `layrz-forms-2.0.0/layrz_forms/fields/boolean.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 """ Boolean field """
+from typing import Any
+
 from .base import Field
 
 
 class BooleanField(Field):
   """
   IdField class for validation
   ---
   Attributes
     required: bool
       Indicates if the field is required or not
   """
 
-  def __init__(self, required=False):
-    super(BooleanField, self).__init__(required=required)
+  def __init__(self, required: bool = False) -> None:
+    super().__init__(required=required)
 
-  def validate(self, key, value, errors):
+  def validate(self, key: str, value: Any, errors: dict) -> None:
     """
     Validate the field with the following rules:
     - Should be a bool
     ---
     Arguments
       key: str
         Key of the field
       value: any
         Value to validate
       errors: dict
         Dict of errors
     """
 
-    super(BooleanField, self).validate(key=key, value=value, errors=errors)
+    super().validate(key=key, value=value, errors=errors)
 
     if not isinstance(value, bool) and (self.required and value is not None):
       self._append_error(
         key=key,
         errors=errors,
         to_add={'code': 'invalid'},
       )
```

### Comparing `layrz-forms-1.0.9/layrz/forms/fields/char.py` & `layrz-forms-2.0.0/layrz_forms/fields/char.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 """ Email field """
+from typing import Any
+
 from .base import Field
 
 
 class CharField(Field):
   """
   CharField class for validation
   ---
@@ -17,27 +19,27 @@
       Indicates if the field can be empty or not
     choices: tuple
       Indicates the choices of the field
   """
 
   def __init__(
     self,
-    required=False,
-    max_length=None,
-    min_length=None,
-    empty=False,
-    choices=None,
-  ):
-    super(CharField, self).__init__(required=required)
+    required: bool = False,
+    max_length: int = None,
+    min_length: int = None,
+    empty: bool = False,
+    choices: list[str] = None,
+  ) -> None:
+    super().__init__(required=required)
     self.max_length = max_length
     self.min_length = min_length
     self.empty = empty
     self.choices = choices
 
-  def validate(self, key, value, errors):
+  def validate(self, key: str, value: Any, errors: dict) -> None:
     """
     Validate the field with the following rules:
     - Should not be empty if required
     - Should be one of the choices indicated if choices is not None
     - Should be less than max_length if max_length is not None
     - Should be greater than min_length if min_length is not None
     ---
@@ -46,15 +48,15 @@
         Key of the field
       value: any
         Value to validate
       errors: dict
         Dict of errors
     """
 
-    super(CharField, self).validate(key=key, value=value, errors=errors)
+    super().validate(key=key, value=value, errors=errors)
 
     if value is not None:
       if not self.empty:
         if len(value) == 0:
           self._append_error(
             key=key,
             errors=errors,
```

### Comparing `layrz-forms-1.0.9/layrz/forms/fields/email.py` & `layrz-forms-2.0.0/layrz_forms/fields/email.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """ Email field """
 import re
+from typing import Any
+
 from .base import Field
 
 
 class EmailField(Field):
   """
   EmailField class for validation
   ---
@@ -14,37 +16,37 @@
       Indicates if the field can be empty or not
     regex: str
       Regex to validate the email
   """
 
   def __init__(
     self,
-    required=False,
-    empty=False,
-    regex=r'^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-z]{2,63}$',
-  ):
-    super(EmailField, self).__init__(required=required)
+    required: bool = False,
+    empty: bool = False,
+    regex: str = r'^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-z]{2,63}$',
+  ) -> None:
+    super().__init__(required=required)
     self.empty = empty
     self.regex = regex
 
-  def validate(self, key, value, errors):
+  def validate(self, key: str, value: Any, errors: dict) -> None:
     """
     Validate the field with the following rules:
     - Should be a valid email, the validation will compile the regex
     ---
     Arguments
       key: str
         Key of the field
       value: any
         Value to validate
       errors: dict
         Dict of errors
     """
 
-    super(EmailField, self).validate(key=key, value=value, errors=errors)
+    super().validate(key=key, value=value, errors=errors)
 
     if isinstance(value, str):
       if not self.empty:
         if value == '' or value is None:
           self._append_error(
             key=key,
             errors=errors,
```

### Comparing `layrz-forms-1.0.9/layrz/forms/fields/id.py` & `layrz-forms-2.0.0/layrz_forms/fields/id.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 """ ID field """
+from typing import Any
+
 from .base import Field
 
 
 class IdField(Field):
   """
   IdField class for validation
   ---
   Attributes
     required: bool
       Indicates if the field is required or not
   """
 
-  def __init__(self, required=False):
-    super(IdField, self).__init__(required=required)
+  def __init__(self, required: bool = False) -> None:
+    super().__init__(required=required)
 
-  def validate(self, key, value, errors):
+  def validate(self, key: str, value: Any, errors: dict) -> None:
     """
     Validate the field with the following rules:
     - Should be a number or a string that can be converted to a number
     - The number should be greater than 0
     ---
     Arguments
       key: str
         Key of the field
       value: any
         Value to validate
       errors: dict
         Dict of errors
     """
 
-    super(IdField, self).validate(key=key, value=value, errors=errors)
+    super().validate(key=key, value=value, errors=errors)
 
     if not isinstance(value, (int, str)) and (self.required and value is not None):
       self._append_error(
         key=key,
         errors=errors,
         to_add={'code': 'invalid'},
       )
```

### Comparing `layrz-forms-1.0.9/layrz/forms/fields/json.py` & `layrz-forms-2.0.0/layrz_forms/fields/json.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 """ JSON Field """
+from typing import Any
+
 from .base import Field
 
 
 class JsonField(Field):
   """
   JsonField class for validation
   ---
@@ -13,23 +15,23 @@
       Indicates if the field can be empty or not
     datatype: (dict, list)
       Indicates the datatype of the field
   """
 
   def __init__(
     self,
-    required=False,
-    empty=False,
-    datatype=dict,
-  ):
-    super(JsonField, self).__init__(required=required)
+    required: bool = False,
+    empty: bool = False,
+    datatype: callable = dict,
+  ) -> None:
+    super().__init__(required=required)
     self.empty = empty
     self.datatype = datatype
 
-  def validate(self, key, value, errors):
+  def validate(self, key: str, value: Any, errors: dict) -> None:
     """
     Validate the field with the following rules:
     - Should be a dict or list (Depending of the datatype)
     - If `empty` is False, the field should not be empty
       * For `dict`, should have at least 1 key
       * For `list`, should have at least 1 item
     ---
@@ -38,15 +40,15 @@
         Key of the field
       value: any
         Value to validate
       errors: dict
         Dict of errors
     """
 
-    super(JsonField, self).validate(key=key, value=value, errors=errors)
+    super().validate(key=key, value=value, errors=errors)
 
     if not isinstance(value, self.datatype):
       self._append_error(
         key=key,
         errors=errors,
         to_add={'code': 'invalid'},
       )
```

### Comparing `layrz-forms-1.0.9/layrz/forms/fields/number.py` & `layrz-forms-2.0.0/layrz_forms/fields/number.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 """ Boolean field """
+from typing import Any
+
 from .base import Field
 
 
 class NumberField(Field):
   """
   NumberField class for validation
   ---
@@ -15,39 +17,39 @@
       Indicates the minimum value of the field
     max_value: int
       Indicates the maximum value of the field
   """
 
   def __init__(
     self,
-    required=False,
-    datatype=float,
-    min_value=None,
-    max_value=None,
-  ):
-    super(NumberField, self).__init__(required=required)
+    required: bool = False,
+    datatype: callable = float,
+    min_value: float = None,
+    max_value: float = None,
+  ) -> None:
+    super().__init__(required=required)
     self.datatype = datatype
     self.min_value = min_value
     self.max_value = max_value
 
-  def validate(self, key, value, errors):
+  def validate(self, key: str, value: Any, errors: dict) -> None:
     """
     Validate the field with the following rules:
     - Should be a int or float (Depending of the datatype)
     ---
     Arguments
       key: str
         Key of the field
       value: any
         Value to validate
       errors: dict
         Dict of errors
     """
 
-    super(NumberField, self).validate(key=key, value=value, errors=errors)
+    super().validate(key=key, value=value, errors=errors)
 
     if not isinstance(value, self.datatype) and (self.required and value is not None):
       self._append_error(key=key, errors=errors, to_add={'code': 'invalid'})
     else:
       try:
         if self.min_value is not None:
           if self.datatype(value) < self.datatype(self.min_value):
```

### Comparing `layrz-forms-1.0.9/layrz_forms.egg-info/PKG-INFO` & `layrz-forms-2.0.0/layrz_forms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: layrz-forms
-Version: 1.0.9
+Version: 2.0.0
 Summary: Layrz forms and tools for Python
 Author-email: "Golden M, Inc." <software@goldenm.com>
 Maintainer-email: Kenny Mochizuki <kenny@goldenm.com>, Miguel Zauzich <miguel@goldenm.com>
 License: MIT License
 Project-URL: Repository, https://github.com/goldenm-software/layrz-forms
 Project-URL: Changelog, https://github.com/goldenm-software/layrz-forms/blob/main/CHANGELOG.md
 Keywords: sdk,goldenm,layrz,django forms,django,forms
@@ -22,15 +22,15 @@
 ## Motivation
 This project is a collection of tools that we use to make django developers life easier. I hope you find them useful too.
 
 ## Usage
 The idea is simple, replace the django forms to a more easier way to use them. Also provide the ability to return the errors key to support i18n.
 
 ```python
-import layrz.forms as forms
+import layrz_forms as forms
 
 
 class ExampleForm(forms.Form):
   """ Example form """
   id_test = forms.IdField(required=True)
   email_text = forms.EmailField(required=True)
   json_list_test = forms.JsonField(required=True, datatype=list)
@@ -75,11 +75,11 @@
   #> form.errors(): {'rangeTextTest': [{'code': 'minLength', 'expected': 5, 'received': 4}], 'clean1': [{'code': 'error1'}, {'code': 'error2'}], 'clean2': [{'code': 'error1'}]}
 ```
 
 ## Work with us
 Golden M is a software/hardware development company what is working on
 a new, innovative and disruptive technologies.
 
-For more information, contact us at [sales@goldenmcorp.com](mailto:sales@goldenmcorp.com)
+For more information, contact us at [sales@goldenm.com](mailto:sales@goldenm.com)
 
 ## License
 This project is under MIT License, for more information, check out the `LICENCE`
```

### Comparing `layrz-forms-1.0.9/pyproject.toml` & `layrz-forms-2.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "layrz-forms"
-version = "1.0.9"
+version = "2.0.0"
 description = "Layrz forms and tools for Python"
 authors = [
   {name = "Golden M, Inc.", email = "software@goldenm.com"}
 ]
 requires-python = ">=3.10"
 
 maintainers = [
@@ -34,16 +34,16 @@
 [project.urls]
 Repository = "https://github.com/goldenm-software/layrz-forms"
 Changelog = "https://github.com/goldenm-software/layrz-forms/blob/main/CHANGELOG.md"
 
 [tool.setuptools.packages.find]
 where = ["."]
 include = [
-  "layrz",
-  "layrz.*",
+  "layrz_forms",
+  "layrz_forms.*",
 ]
 namespaces = true
 
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
```

