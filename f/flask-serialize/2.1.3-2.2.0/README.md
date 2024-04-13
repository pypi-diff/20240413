# Comparing `tmp/flask-serialize-2.1.3.tar.gz` & `tmp/flask-serialize-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-serialize-2.1.3.tar", last modified: Sun Mar  5 10:05:18 2023, max compression
+gzip compressed data, was "flask-serialize-2.2.0.tar", last modified: Sat Apr 13 07:08:19 2024, max compression
```

## Comparing `flask-serialize-2.1.3.tar` & `flask-serialize-2.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 10:05:18.016602 flask-serialize-2.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-05 10:05:08.000000 flask-serialize-2.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-05 10:05:08.000000 flask-serialize-2.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    35299 2023-03-05 10:05:18.016602 flask-serialize-2.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    34031 2023-03-05 10:05:08.000000 flask-serialize-2.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-05 10:05:08.000000 flask-serialize-2.1.3/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 10:05:18.016602 flask-serialize-2.1.3/flask_serialize/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-03-05 10:05:08.000000 flask-serialize-2.1.3/flask_serialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30377 2023-03-05 10:05:08.000000 flask-serialize-2.1.3/flask_serialize/flask_serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-03-05 10:05:08.000000 flask-serialize-2.1.3/flask_serialize/form_page.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 10:05:18.016602 flask-serialize-2.1.3/flask_serialize.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    35299 2023-03-05 10:05:17.000000 flask-serialize-2.1.3/flask_serialize.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-03-05 10:05:17.000000 flask-serialize-2.1.3/flask_serialize.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-05 10:05:17.000000 flask-serialize-2.1.3/flask_serialize.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-05 10:05:17.000000 flask-serialize-2.1.3/flask_serialize.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-05 10:05:17.000000 flask-serialize-2.1.3/flask_serialize.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-05 10:05:18.016602 flask-serialize-2.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-03-05 10:05:08.000000 flask-serialize-2.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 10:05:18.016602 flask-serialize-2.1.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)    32748 2023-03-05 10:05:08.000000 flask-serialize-2.1.3/test/test_app.py
--rw-r--r--   0 runner    (1001) docker     (123)    15695 2023-03-05 10:05:08.000000 flask-serialize-2.1.3/test/test_flask_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:08:19.325251 flask-serialize-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-13 07:08:10.000000 flask-serialize-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-13 07:08:10.000000 flask-serialize-2.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    36078 2024-04-13 07:08:19.325251 flask-serialize-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    34829 2024-04-13 07:08:10.000000 flask-serialize-2.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-13 07:08:10.000000 flask-serialize-2.2.0/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:08:19.325251 flask-serialize-2.2.0/flask_serialize/
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-13 07:08:10.000000 flask-serialize-2.2.0/flask_serialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32256 2024-04-13 07:08:10.000000 flask-serialize-2.2.0/flask_serialize/flask_serialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-04-13 07:08:10.000000 flask-serialize-2.2.0/flask_serialize/form_page.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:08:19.325251 flask-serialize-2.2.0/flask_serialize.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    36078 2024-04-13 07:08:19.000000 flask-serialize-2.2.0/flask_serialize.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-13 07:08:19.000000 flask-serialize-2.2.0/flask_serialize.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 07:08:19.000000 flask-serialize-2.2.0/flask_serialize.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-13 07:08:19.000000 flask-serialize-2.2.0/flask_serialize.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-13 07:08:19.000000 flask-serialize-2.2.0/flask_serialize.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-13 07:08:19.325251 flask-serialize-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-13 07:08:10.000000 flask-serialize-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:08:19.325251 flask-serialize-2.2.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    37102 2024-04-13 07:08:10.000000 flask-serialize-2.2.0/test/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15759 2024-04-13 07:08:10.000000 flask-serialize-2.2.0/test/test_flask_app.py
```

### Comparing `flask-serialize-2.1.3/LICENSE` & `flask-serialize-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flask-serialize-2.1.3/PKG-INFO` & `flask-serialize-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 Metadata-Version: 2.1
 Name: flask-serialize
-Version: 2.1.3
+Version: 2.2.0
 Summary: Easy to use JSON serialization and update/create for Flask and SQLAlchemy.
 Home-page: https://github.com/Martlark/flask-serialize
-Download-URL: https://github.com/Martlark/flask-serialize/archive/2.1.3.tar.gz
+Download-URL: https://github.com/Martlark/flask-serialize/archive/2.2.0.tar.gz
 Author: Andrew Rowe
 Author-email: rowe.andrew.d@gmail.com
 License: Apache Software License
 Keywords: flask sqlalchemy serialize serialization serialise
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Framework :: Flask
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: Permissive-Dict
 
 # flask-serialize
 
 # DB Model JSON serialization with PUT, POST write for Flask applications using SQLAlchemy
 
 ## Installation
 
@@ -114,65 +114,65 @@
 
     def __repr__(self):
         return '<Setting %r %r %r>' % (self.id, self.setting_type, self.value)
 ```
 
 ## Routes setup
 
-Get a single item as json.
+Get a single item as JSON.
 
 ```python
 @app.route('/get_setting/<item_id>', methods=['GET'])
 def get_setting( item_id ):
     return Setting.fs_get_delete_put_post(item_id)
 
-# Returns a Flask response with a json object, example:
+# Returns a Flask response with a JSON object, example:
 ```
 
 ```JavaScript
 {id:1, value: "hello"}
 ```
 
-Put an update to a single item as json.
+Put an update to a single item as JSON.
 
 ```python
 @app.route('/update_setting/<item_id>', methods=['PUT'])
 def update_setting( item_id ):
     return Setting.fs_get_delete_put_post(item_id)
 
-# Returns a Flask response with the result as a json object:
+# Returns a Flask response with the result as a JSON object:
 
 ```
 
 ```JavaScript
 {message: "success message"}
 ```
 
 Delete a single item.
 
 ```python
 @app.route('/delete_setting/<item_id>', methods=['DELETE'])
 def delete_setting( item_id ):
     return Setting.fs_get_delete_put_post(item_id)
 
-# Returns a Flask response with the result and item deleted as a json response:
+# Returns a Flask response with the result and item deleted as a JSON response:
 ```
 
 ```JavaScript
 {message: "success message", item: {"id":5, name: "gone"}}
 ```
 
-Get all items as a json list.
+Get all items as a JSON list.
 
 ```python
 @app.route('/get_setting_all', methods=['GET'])
 def get_setting_all():
     return Setting.fs_get_delete_put_post()
 
-# Returns a Flask response with a list of json objects, example:
+# Returns a Flask response with a list of JSON objects, example:
 ```
 
 ```JavaScript
 [{id:1, value: "hello"},{id:2, value: "there"},{id:3, value: "programmer"}]
 ```
 
 All of: get-all, get, put, post, and delete can be combined in one route.
@@ -180,15 +180,15 @@
 ```python
 @app.route('/setting/<int:item_id>', methods=['GET', 'PUT', 'DELETE', 'POST'])
 @app.route('/setting', methods=['GET', 'POST'])
 def route_setting_all(item_id=None):
     return Setting.fs_get_delete_put_post(item_id)
 ```
 
-Updating from a json object in the flask put request
+Updating from a JSON object in the Flask put request
 
 JQuery example:
 
 ```javascript
 function put(setting_id) {
         return $.ajax({
             url: `/update_setting/${setting_id}`,
@@ -283,20 +283,20 @@
 ```
 
 # Writing and creating
 
 When using any of the convenience methods to update, create or delete an object these properties and
 methods control how flask-serialize handles the operation.
 
-## Updating from a form or json
+## Updating from a form or JSON
 
 ```python
 def fs_request_update_json():
     """
-    Update an item from request json data or PUT params, probably from a PUT or PATCH.
+    Update an item from request JSON data or PUT params, probably from a PUT or PATCH.
     Throws exception if not valid
 
     :return: True if item updated
 
     """
 ```
 
@@ -311,15 +311,15 @@
         if message.fs_request_update_json():
             return 'Updated'
 ```
 
 ```python
 def fs_request_update_json():
     """
-    Update an item from request json data or PUT params, probably from a PUT or PATCH.
+    Update an item from request JSON data or PUT params, probably from a PUT or PATCH.
     Throws exception if not valid
 
     :return: True if item updated
 
     """
 ```
 
@@ -392,16 +392,17 @@
 ```
 
 Override the mixin `__fs_can_access__` to provide control over when an
 item can be read or accessed.  Return False to exclude from results.
 
 ## Private fields
 
-Fields can be made private for certain reasons by overriding the `__fs_private_field__` method
-and returning `True` if the field is to be private.
+Fields can be made private by overriding the `__fs_private_field__` method
+and returning `True` if the field is to be private.  These fields will not be returned
+in JSON results.
 
 Private fields will be excluded for any get, put and post methods.
 
 Example:
 
 To exclude private fields when a user is not the admin.
 
@@ -448,15 +449,15 @@
 ```
 
 This can be used to communicate from the model on the server to the JavaScript code
 interesting things from updates
 
 ## `__fs_create_fields__`
 
-List of model fields to be read from a form or json when creating an object.  Can be the specified as either 'text' or
+List of model fields to be read from a form or JSON when creating an object.  Can be the specified as either 'text' or
 the field. Do not put primary keys here.  Do not put foreign keys here if using SQLAlchemy child insertion.
 This is usually the same as `__fs_update_fields__`.  When `__fs_create_fields__` is empty all column fields can be inserted.
 
 Used by these methods:
 
 - fs_request_create_form
 - fs_get_delete_put_post
@@ -510,38 +511,58 @@
 
 List of model field names to not serialize at all.
 
 ```python
 __fs_exclude_serialize_fields__ = []
 ```
 
-List of model field names to not serialize when returning as json.
+List of model field names to not serialize when returning as JSON.
 
 ```python
 __fs_exclude_json_serialize_fields__ = []
 ```
 
-## Filtering json list results
+## Built in query_by using request arg on GET
+
+`fs_get_delete_put_post` by default supports automatic passing of GET request args to the query method using
+a `filter_by` clause. Example using a Flask route that be default returns all messages:
+
+
+```python
+    @route('/message/', methods=['GET'])
+    def route_message():
+        return Message.fs_get_by_user_or_404()
+```
+
+Call the endpoint using URL like:
+
+  /message/?name=hello&lines=12
+
+Will return any message records with the name of 'hello' and with 12 lines.
+
+This feature can be disabled by using `__fs_filter_by = False` on the model definition.
+
+## Filtering JSON list results
 
 Json result lists can be filtered by using the `prop_filters` parameter on either
 the `fs_get_delete_put_post` method or the `fs_json_list` method.
 
-The filter consists of one or more properties in the json result and
+The filter consists of one or more properties in the JSON result and
 the value that it must match.  Filter items will match against the
 first `prop_filter` property to exactly equal the value.
 
 NOTE: The filter is not applied with single a GET or, the PUT, POST and DELETE methods.
 
 Example to only return dogs:
 
 ```python
 result = fs_get_delete_put_post(prop_filters = {'key':'dogs'})
 ```
 
-## Sorting json list results
+## Sorting JSON list results
 
 Json result lists can be sorted by using the `__fs_order_by_field__` or the `__fs_order_by_field_desc__` properties.  The results
 are sorted after the query is converted to JSON.  As such you can use any property from a class to sort. To sort by id
 ascending use this example:
 
 ```python
 __fs_order_by_field__ = 'id'
@@ -561,15 +582,15 @@
 
 The `fs_query_by_access` method can be used to filter a SQLAlchemy result set so that
 the `user` property and `__fs_can_access__` hook method are used to restrict to allowable items.
 
 Example:
 
 ```python
-result_list = Setting. fs_query_by_access(user='Andrew', setting_type='test')
+result_list = Setting.fs_query_by_access(user='Andrew', setting_type='test')
 ```
 
 Any keyword can be supplied after `user` to be passed to `filter_by` method of `query`.
 
 ## Relationships list of property names that are to be included in serialization
 
 ```python
@@ -680,17 +701,17 @@
 - `user`: user to user as query filter.
 - `prop_filters`: dictionary of key:value pairs to limit results when returning get-all.
 
 | Method Operation | item_id     | Response                                                                                                                                                                                                                                                                                                 |
 |------------------|-------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | GET              | primary key | returns one item when `item_id` is a primary key.  {property1:value1,property2:value2,...}                                                                                                                                                                                                               |
 | GET              | None        | returns all items when `item_id` is None. [{item1},{item2},...]                                                                                                                                                                                                                                          |
-| PUT              | primary key | updates item using `item_id` as the id from request json data.  Calls the model `__fs_verify__`    `{message:message,item:{model_fields,...}`, properties:{`__fs_update_properties__`}} before updating.  Returns new item as {item}                                                                       |
+| PUT              | primary key | updates item using `item_id` as the id from request JSON data.  Calls the model `__fs_verify__`    `{message:message,item:{model_fields,...}`, properties:{`__fs_update_properties__`}} before updating.  Returns new item as {item}                                                                       |
 | DELETE           | primary key | removes the item with primary key of `item_id` if self.__fs_can_delete__ does not throw an error.  `{property1:value1,property2:value2,...}`                                                                                         Returns the item removed.  Calls `__fs_can_delete__` before delete. |
-| POST             | None        | creates and returns a Flask response with a new item as json from form body data or JSON body data {property1:value1,property2:value2,...} When `item_id` is None. Calls the model `__fs_verify__` method before creating.                                                                               |
+| POST             | None        | creates and returns a Flask response with a new item as JSON from form body data or JSON body data {property1:value1,property2:value2,...} When `item_id` is None. Calls the model `__fs_verify__` method before creating.                                                                               |
 | POST             | primary key | updates an item from form data using `item_id`. Calls the model ` __fs_verify__` method before updating.                                                                                                                                                                                                 |
 
 On error returns a response of 'error message' with http status code of 400.
 
 Set the `user` parameter to restrict a certain user.  By default uses the
 relationship of `user`.  Set another relationship field by setting the `__fs_user_field__` to the name of the
 relationship.
@@ -705,33 +726,33 @@
 ```python
 item = Setting.query.get_or_404(2)
 dict_item = item.fs_as_dict()
 ```
 
 ## fs_as_json
 
-Convert a db object into a json Flask response using `jsonify`.  Example:
+Convert a db object into a JSON Flask response using `jsonify`.  Example:
 
 ```python
 @app.route('/setting/<int:item_id>')
 def get_setting(item_id):
     item = Setting.query.get_or_404(item_id)
     return item.fs_as_json()
 ```
 
-## `__fs_after_commit__(self, create=False)`
+## __fs_after_commit__(self, create=False)
 
+Hook to call after any of `fs_update_from_dict`, `fs_request_update_form`, `fs_request_update_json` has been called so that
+you can do what you like.  `self` is the updated or created (create==True) item. Example:
 
 ```python
 def  __fs_after_commit__(self, create=False):
+        logging.info(f'changed! {self}')
 ```
 
-Hook to call after any `fs_update_from_dict`, `fs_request_update_form`, `fs_request_update_json` has been called so that
-you do what you like.  `self` is the updated or created (create==True) item.
-
 NOTE: not called after a `DELETE`
 
 ## `__fs_before_update__(cls, data_dict)`
 
 - data_dict: a dictionary of new data to apply to the item
 - return: the new `data_dict` to use when updating
 
@@ -760,70 +781,70 @@
 def get_items():
     items = Setting.query.all()
     return jsonify(Setting.fs_dict_list(items))
 ```
 
 ## fs_json_list(query_result)
 
-Return a flask response in json list format from a sql alchemy query result.
+Return a flask response in JSON list format from a sql alchemy query result.
 
 .. code:: python
 python
 
 ```
 @bp.route('/address/list', methods=['GET'])
 @login_required
 def address_list():
     items = Address.query.filter_by(user=current_user)
     return Address.fs_json_list(items)
 ```
 
 ## fs_json_filter_by(kw_args)
 
-Return a flask list response in json format using a filter_by query.
+Return a flask list response in JSON format using a filter_by query.
 
 Example:
 
 ```python
 @bp.route('/address/list', methods=['GET'])
 @login_required
 def address_list():
-    return Address.filter_by(user=current_user)
+    return Address.fs_json_filter_by(user=current_user)
 ```
 
 ## fs_json_first(kwargs)
 
-Return the first result in json format using filter_by arguments.
+Return the first result in JSON format using filter_by arguments.
 
 Example:
 
 ```python
 @bp.route('/score/<course>', methods=['GET'])
 @login_required
 def score(course):
     return Score.fs_json_first(class_name=course)
 ```
 
-## `__fs_previous_field_value__`
+## __fs_previous_field_value__
 
-A dictionary of the previous field values before an update is applied from a dict, form or json update operation. Helpful
+A dictionary of the previous field values before an update is applied from a dict, form or JSON update operation. Helpful
 in the `__fs_verify__` method to see if field values are to be changed.
 
 Example:
 
 ```python
 def __fs_verify__(self, create=False):
     previous_value = self.__fs_previous_field_value__.get('value')
     if previous_value != self.value:
         current_app.logger.warning(f'value is changing from {previous_value}')
 ```
 
 ## fs_request_create_form(kwargs)
 
-Use the contents of a Flask request form or request json data to create a item
+Use the contents of a Flask request form or request JSON data to create a item
 in the database.   Calls `__fs_verify__(create=True)`.  Returns the new item or throws error.
 Use kwargs to set the object properties of the newly created item.
 
 Example:
 
 Create a `score` item with the parent being a `course`.
 
@@ -833,15 +854,15 @@
 def score(course_id):
     course = Course.query.get_or_404(course_id)
     return Score.fs_request_create_form(course_id=course.id).fs_as_dict
 ```
 
 ## fs_request_update_form()
 
-Use the contents of a Flask request form or request json data to update an item
+Use the contents of a Flask request form or request JSON data to update an item
 in the database.   Calls `__fs_verify__()` and `__fs_can_update__()` to check
 if can update.  Returns True on success.
 
 Example:
 
 Update a score item.
 
@@ -963,14 +984,15 @@
 - Hook methods start with `__fs_` and end with `__`.
 - Control properties start with `__fs_` and end with `__`.
 - Some hook functions can now return False or True rather than just raise Exceptions
 - fs_get_delete_put_post now returns a HTTP code that is more accurate of the cause
 
 ## Release Notes
 
+- 2.2.0 - Allow arg parameters to be used in `fs_get_delete_put_post` 'GET' as query_by filters
 - 2.1.3 - Allow sorting by lambda
 - 2.1.2 - Fix readme table format
 - 2.1.1 - Improve sqlite JSON handling
 - 2.1.0 - Convert readme to markdown.  Add support for JSON columns.  Withdraw Python 3.6 Support. Use unittest instead of pytest.  NOTE: Changes `__fs_convert_types__` to a `dict`.
 - 2.0.3 - Allow more use of model column variables instead of "quoted" field names.  Fix missing import for FlaskSerialize.
 - 2.0.2 - Fix table formatting.
 - 2.0.1 - Try to get properties and methods to use more appropriate names.
@@ -978,25 +1000,25 @@
 - 1.5.1 - Fix TypeError: unsupported operand type(s) for +=: 'ImmutableColumnCollection' and 'list' with newer versions of SQLAlchemy
 - 1.5.0 - Return item from POST/PUT updates. Allow `__fs_create_fields__` and `__fs_update_fields__` to be specified using the column fields.  None values serialize as null/None.  Restore previous `__fs_update_properties__` behaviour.  By default, updates/creates using all fields. Exclude primary key from create and update.
 - 1.4.2 - by default return all props with `__fs_update_properties__`
 - 1.4.1 - Add better exception message when `db` mixin property not set.  Add `FlaskSerialize` factory method.
 - 1.4.0 - Add `__fs_private_field__` method.
 - 1.3.1 - Fix incorrect method signatures.  Add fs_query_by_access method.
 - 1.3.0 - Add `__fs_can_update__` and `__fs_can_access__` methods for controlling update and access.
-- 1.2.1 - Add support to change the user field name for get_put_post_delete user= parameter.
+- 1.2.1 - Add support to change the user field name for fs_get_delete_put_post user= parameter.
 - 1.2.0 - Add support for decimal, numeric and clob.  Treat all VARCHARS the same.  Convert non-list relationship.
 - 1.1.9 - Allow FlaskSerializeMixin to be converted when a property value.
 - 1.1.8 - Move form_page to separate MixIn.  Slight refactoring.  Add support for complex type to db.
 - 1.1.6 - Make sure all route returns use jsonify as required for older Flask versions.  Add `__fs_before_update__` hook.
 - 1.1.5 - Add `__fs_previous_field_value__` array that is set during update.  Allows comparing new and previous values during  `__fs_verify__`.
 - 1.1.4 - Fix doco typos and JavaScript examples.  Add form_page method.  Improve test and example apps.  Remove Python 2, 3.4 testing and support.
 - 1.1.3 - Fix duplicate db writes.  Return item on delete.  Remove obsolete code structures.  Do not update with non-existent fields.
 - 1.1.2 - Add 400 http status code for errors, remove error dict.  Improve documentation.
 - 1.1.0 - Suppress silly errors. Improve documentation.
 - 1.0.9 - Add kwargs to fs_request_create_form to pass Object props to be used when creating the Object instance
 - 1.0.8 - Cache introspection to improve performance.  All model definitions are cached after first use.  It is no longer possible to alter model definitions dynamically.
-- 1.0.7 - Add json request body support to post update.
-- 1.0.5 - Allow sorting of json lists.
+- 1.0.7 - Add JSON request body support to post update.
+- 1.0.5 - Allow sorting of JSON lists.
 
 ## Licensing
 
 - Apache 2.0
```

### Comparing `flask-serialize-2.1.3/README.md` & `flask-serialize-2.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -85,65 +85,65 @@
 
     def __repr__(self):
         return '<Setting %r %r %r>' % (self.id, self.setting_type, self.value)
 ```
 
 ## Routes setup
 
-Get a single item as json.
+Get a single item as JSON.
 
 ```python
 @app.route('/get_setting/<item_id>', methods=['GET'])
 def get_setting( item_id ):
     return Setting.fs_get_delete_put_post(item_id)
 
-# Returns a Flask response with a json object, example:
+# Returns a Flask response with a JSON object, example:
 ```
 
 ```JavaScript
 {id:1, value: "hello"}
 ```
 
-Put an update to a single item as json.
+Put an update to a single item as JSON.
 
 ```python
 @app.route('/update_setting/<item_id>', methods=['PUT'])
 def update_setting( item_id ):
     return Setting.fs_get_delete_put_post(item_id)
 
-# Returns a Flask response with the result as a json object:
+# Returns a Flask response with the result as a JSON object:
 
 ```
 
 ```JavaScript
 {message: "success message"}
 ```
 
 Delete a single item.
 
 ```python
 @app.route('/delete_setting/<item_id>', methods=['DELETE'])
 def delete_setting( item_id ):
     return Setting.fs_get_delete_put_post(item_id)
 
-# Returns a Flask response with the result and item deleted as a json response:
+# Returns a Flask response with the result and item deleted as a JSON response:
 ```
 
 ```JavaScript
 {message: "success message", item: {"id":5, name: "gone"}}
 ```
 
-Get all items as a json list.
+Get all items as a JSON list.
 
 ```python
 @app.route('/get_setting_all', methods=['GET'])
 def get_setting_all():
     return Setting.fs_get_delete_put_post()
 
-# Returns a Flask response with a list of json objects, example:
+# Returns a Flask response with a list of JSON objects, example:
 ```
 
 ```JavaScript
 [{id:1, value: "hello"},{id:2, value: "there"},{id:3, value: "programmer"}]
 ```
 
 All of: get-all, get, put, post, and delete can be combined in one route.
@@ -151,15 +151,15 @@
 ```python
 @app.route('/setting/<int:item_id>', methods=['GET', 'PUT', 'DELETE', 'POST'])
 @app.route('/setting', methods=['GET', 'POST'])
 def route_setting_all(item_id=None):
     return Setting.fs_get_delete_put_post(item_id)
 ```
 
-Updating from a json object in the flask put request
+Updating from a JSON object in the Flask put request
 
 JQuery example:
 
 ```javascript
 function put(setting_id) {
         return $.ajax({
             url: `/update_setting/${setting_id}`,
@@ -254,20 +254,20 @@
 ```
 
 # Writing and creating
 
 When using any of the convenience methods to update, create or delete an object these properties and
 methods control how flask-serialize handles the operation.
 
-## Updating from a form or json
+## Updating from a form or JSON
 
 ```python
 def fs_request_update_json():
     """
-    Update an item from request json data or PUT params, probably from a PUT or PATCH.
+    Update an item from request JSON data or PUT params, probably from a PUT or PATCH.
     Throws exception if not valid
 
     :return: True if item updated
 
     """
 ```
 
@@ -282,15 +282,15 @@
         if message.fs_request_update_json():
             return 'Updated'
 ```
 
 ```python
 def fs_request_update_json():
     """
-    Update an item from request json data or PUT params, probably from a PUT or PATCH.
+    Update an item from request JSON data or PUT params, probably from a PUT or PATCH.
     Throws exception if not valid
 
     :return: True if item updated
 
     """
 ```
 
@@ -363,16 +363,17 @@
 ```
 
 Override the mixin `__fs_can_access__` to provide control over when an
 item can be read or accessed.  Return False to exclude from results.
 
 ## Private fields
 
-Fields can be made private for certain reasons by overriding the `__fs_private_field__` method
-and returning `True` if the field is to be private.
+Fields can be made private by overriding the `__fs_private_field__` method
+and returning `True` if the field is to be private.  These fields will not be returned
+in JSON results.
 
 Private fields will be excluded for any get, put and post methods.
 
 Example:
 
 To exclude private fields when a user is not the admin.
 
@@ -419,15 +420,15 @@
 ```
 
 This can be used to communicate from the model on the server to the JavaScript code
 interesting things from updates
 
 ## `__fs_create_fields__`
 
-List of model fields to be read from a form or json when creating an object.  Can be the specified as either 'text' or
+List of model fields to be read from a form or JSON when creating an object.  Can be the specified as either 'text' or
 the field. Do not put primary keys here.  Do not put foreign keys here if using SQLAlchemy child insertion.
 This is usually the same as `__fs_update_fields__`.  When `__fs_create_fields__` is empty all column fields can be inserted.
 
 Used by these methods:
 
 - fs_request_create_form
 - fs_get_delete_put_post
@@ -481,38 +482,58 @@
 
 List of model field names to not serialize at all.
 
 ```python
 __fs_exclude_serialize_fields__ = []
 ```
 
-List of model field names to not serialize when returning as json.
+List of model field names to not serialize when returning as JSON.
 
 ```python
 __fs_exclude_json_serialize_fields__ = []
 ```
 
-## Filtering json list results
+## Built in query_by using request arg on GET
+
+`fs_get_delete_put_post` by default supports automatic passing of GET request args to the query method using
+a `filter_by` clause. Example using a Flask route that be default returns all messages:
+
+
+```python
+    @route('/message/', methods=['GET'])
+    def route_message():
+        return Message.fs_get_by_user_or_404()
+```
+
+Call the endpoint using URL like:
+
+  /message/?name=hello&lines=12
+
+Will return any message records with the name of 'hello' and with 12 lines.
+
+This feature can be disabled by using `__fs_filter_by = False` on the model definition.
+
+## Filtering JSON list results
 
 Json result lists can be filtered by using the `prop_filters` parameter on either
 the `fs_get_delete_put_post` method or the `fs_json_list` method.
 
-The filter consists of one or more properties in the json result and
+The filter consists of one or more properties in the JSON result and
 the value that it must match.  Filter items will match against the
 first `prop_filter` property to exactly equal the value.
 
 NOTE: The filter is not applied with single a GET or, the PUT, POST and DELETE methods.
 
 Example to only return dogs:
 
 ```python
 result = fs_get_delete_put_post(prop_filters = {'key':'dogs'})
 ```
 
-## Sorting json list results
+## Sorting JSON list results
 
 Json result lists can be sorted by using the `__fs_order_by_field__` or the `__fs_order_by_field_desc__` properties.  The results
 are sorted after the query is converted to JSON.  As such you can use any property from a class to sort. To sort by id
 ascending use this example:
 
 ```python
 __fs_order_by_field__ = 'id'
@@ -532,15 +553,15 @@
 
 The `fs_query_by_access` method can be used to filter a SQLAlchemy result set so that
 the `user` property and `__fs_can_access__` hook method are used to restrict to allowable items.
 
 Example:
 
 ```python
-result_list = Setting. fs_query_by_access(user='Andrew', setting_type='test')
+result_list = Setting.fs_query_by_access(user='Andrew', setting_type='test')
 ```
 
 Any keyword can be supplied after `user` to be passed to `filter_by` method of `query`.
 
 ## Relationships list of property names that are to be included in serialization
 
 ```python
@@ -651,17 +672,17 @@
 - `user`: user to user as query filter.
 - `prop_filters`: dictionary of key:value pairs to limit results when returning get-all.
 
 | Method Operation | item_id     | Response                                                                                                                                                                                                                                                                                                 |
 |------------------|-------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | GET              | primary key | returns one item when `item_id` is a primary key.  {property1:value1,property2:value2,...}                                                                                                                                                                                                               |
 | GET              | None        | returns all items when `item_id` is None. [{item1},{item2},...]                                                                                                                                                                                                                                          |
-| PUT              | primary key | updates item using `item_id` as the id from request json data.  Calls the model `__fs_verify__`    `{message:message,item:{model_fields,...}`, properties:{`__fs_update_properties__`}} before updating.  Returns new item as {item}                                                                       |
+| PUT              | primary key | updates item using `item_id` as the id from request JSON data.  Calls the model `__fs_verify__`    `{message:message,item:{model_fields,...}`, properties:{`__fs_update_properties__`}} before updating.  Returns new item as {item}                                                                       |
 | DELETE           | primary key | removes the item with primary key of `item_id` if self.__fs_can_delete__ does not throw an error.  `{property1:value1,property2:value2,...}`                                                                                         Returns the item removed.  Calls `__fs_can_delete__` before delete. |
-| POST             | None        | creates and returns a Flask response with a new item as json from form body data or JSON body data {property1:value1,property2:value2,...} When `item_id` is None. Calls the model `__fs_verify__` method before creating.                                                                               |
+| POST             | None        | creates and returns a Flask response with a new item as JSON from form body data or JSON body data {property1:value1,property2:value2,...} When `item_id` is None. Calls the model `__fs_verify__` method before creating.                                                                               |
 | POST             | primary key | updates an item from form data using `item_id`. Calls the model ` __fs_verify__` method before updating.                                                                                                                                                                                                 |
 
 On error returns a response of 'error message' with http status code of 400.
 
 Set the `user` parameter to restrict a certain user.  By default uses the
 relationship of `user`.  Set another relationship field by setting the `__fs_user_field__` to the name of the
 relationship.
@@ -676,33 +697,33 @@
 ```python
 item = Setting.query.get_or_404(2)
 dict_item = item.fs_as_dict()
 ```
 
 ## fs_as_json
 
-Convert a db object into a json Flask response using `jsonify`.  Example:
+Convert a db object into a JSON Flask response using `jsonify`.  Example:
 
 ```python
 @app.route('/setting/<int:item_id>')
 def get_setting(item_id):
     item = Setting.query.get_or_404(item_id)
     return item.fs_as_json()
 ```
 
-## `__fs_after_commit__(self, create=False)`
+## __fs_after_commit__(self, create=False)
 
+Hook to call after any of `fs_update_from_dict`, `fs_request_update_form`, `fs_request_update_json` has been called so that
+you can do what you like.  `self` is the updated or created (create==True) item. Example:
 
 ```python
 def  __fs_after_commit__(self, create=False):
+        logging.info(f'changed! {self}')
 ```
 
-Hook to call after any `fs_update_from_dict`, `fs_request_update_form`, `fs_request_update_json` has been called so that
-you do what you like.  `self` is the updated or created (create==True) item.
-
 NOTE: not called after a `DELETE`
 
 ## `__fs_before_update__(cls, data_dict)`
 
 - data_dict: a dictionary of new data to apply to the item
 - return: the new `data_dict` to use when updating
 
@@ -731,70 +752,70 @@
 def get_items():
     items = Setting.query.all()
     return jsonify(Setting.fs_dict_list(items))
 ```
 
 ## fs_json_list(query_result)
 
-Return a flask response in json list format from a sql alchemy query result.
+Return a flask response in JSON list format from a sql alchemy query result.
 
 .. code:: python
 python
 
 ```
 @bp.route('/address/list', methods=['GET'])
 @login_required
 def address_list():
     items = Address.query.filter_by(user=current_user)
     return Address.fs_json_list(items)
 ```
 
 ## fs_json_filter_by(kw_args)
 
-Return a flask list response in json format using a filter_by query.
+Return a flask list response in JSON format using a filter_by query.
 
 Example:
 
 ```python
 @bp.route('/address/list', methods=['GET'])
 @login_required
 def address_list():
-    return Address.filter_by(user=current_user)
+    return Address.fs_json_filter_by(user=current_user)
 ```
 
 ## fs_json_first(kwargs)
 
-Return the first result in json format using filter_by arguments.
+Return the first result in JSON format using filter_by arguments.
 
 Example:
 
 ```python
 @bp.route('/score/<course>', methods=['GET'])
 @login_required
 def score(course):
     return Score.fs_json_first(class_name=course)
 ```
 
-## `__fs_previous_field_value__`
+## __fs_previous_field_value__
 
-A dictionary of the previous field values before an update is applied from a dict, form or json update operation. Helpful
+A dictionary of the previous field values before an update is applied from a dict, form or JSON update operation. Helpful
 in the `__fs_verify__` method to see if field values are to be changed.
 
 Example:
 
 ```python
 def __fs_verify__(self, create=False):
     previous_value = self.__fs_previous_field_value__.get('value')
     if previous_value != self.value:
         current_app.logger.warning(f'value is changing from {previous_value}')
 ```
 
 ## fs_request_create_form(kwargs)
 
-Use the contents of a Flask request form or request json data to create a item
+Use the contents of a Flask request form or request JSON data to create a item
 in the database.   Calls `__fs_verify__(create=True)`.  Returns the new item or throws error.
 Use kwargs to set the object properties of the newly created item.
 
 Example:
 
 Create a `score` item with the parent being a `course`.
 
@@ -804,15 +825,15 @@
 def score(course_id):
     course = Course.query.get_or_404(course_id)
     return Score.fs_request_create_form(course_id=course.id).fs_as_dict
 ```
 
 ## fs_request_update_form()
 
-Use the contents of a Flask request form or request json data to update an item
+Use the contents of a Flask request form or request JSON data to update an item
 in the database.   Calls `__fs_verify__()` and `__fs_can_update__()` to check
 if can update.  Returns True on success.
 
 Example:
 
 Update a score item.
 
@@ -934,14 +955,15 @@
 - Hook methods start with `__fs_` and end with `__`.
 - Control properties start with `__fs_` and end with `__`.
 - Some hook functions can now return False or True rather than just raise Exceptions
 - fs_get_delete_put_post now returns a HTTP code that is more accurate of the cause
 
 ## Release Notes
 
+- 2.2.0 - Allow arg parameters to be used in `fs_get_delete_put_post` 'GET' as query_by filters
 - 2.1.3 - Allow sorting by lambda
 - 2.1.2 - Fix readme table format
 - 2.1.1 - Improve sqlite JSON handling
 - 2.1.0 - Convert readme to markdown.  Add support for JSON columns.  Withdraw Python 3.6 Support. Use unittest instead of pytest.  NOTE: Changes `__fs_convert_types__` to a `dict`.
 - 2.0.3 - Allow more use of model column variables instead of "quoted" field names.  Fix missing import for FlaskSerialize.
 - 2.0.2 - Fix table formatting.
 - 2.0.1 - Try to get properties and methods to use more appropriate names.
@@ -949,25 +971,25 @@
 - 1.5.1 - Fix TypeError: unsupported operand type(s) for +=: 'ImmutableColumnCollection' and 'list' with newer versions of SQLAlchemy
 - 1.5.0 - Return item from POST/PUT updates. Allow `__fs_create_fields__` and `__fs_update_fields__` to be specified using the column fields.  None values serialize as null/None.  Restore previous `__fs_update_properties__` behaviour.  By default, updates/creates using all fields. Exclude primary key from create and update.
 - 1.4.2 - by default return all props with `__fs_update_properties__`
 - 1.4.1 - Add better exception message when `db` mixin property not set.  Add `FlaskSerialize` factory method.
 - 1.4.0 - Add `__fs_private_field__` method.
 - 1.3.1 - Fix incorrect method signatures.  Add fs_query_by_access method.
 - 1.3.0 - Add `__fs_can_update__` and `__fs_can_access__` methods for controlling update and access.
-- 1.2.1 - Add support to change the user field name for get_put_post_delete user= parameter.
+- 1.2.1 - Add support to change the user field name for fs_get_delete_put_post user= parameter.
 - 1.2.0 - Add support for decimal, numeric and clob.  Treat all VARCHARS the same.  Convert non-list relationship.
 - 1.1.9 - Allow FlaskSerializeMixin to be converted when a property value.
 - 1.1.8 - Move form_page to separate MixIn.  Slight refactoring.  Add support for complex type to db.
 - 1.1.6 - Make sure all route returns use jsonify as required for older Flask versions.  Add `__fs_before_update__` hook.
 - 1.1.5 - Add `__fs_previous_field_value__` array that is set during update.  Allows comparing new and previous values during  `__fs_verify__`.
 - 1.1.4 - Fix doco typos and JavaScript examples.  Add form_page method.  Improve test and example apps.  Remove Python 2, 3.4 testing and support.
 - 1.1.3 - Fix duplicate db writes.  Return item on delete.  Remove obsolete code structures.  Do not update with non-existent fields.
 - 1.1.2 - Add 400 http status code for errors, remove error dict.  Improve documentation.
 - 1.1.0 - Suppress silly errors. Improve documentation.
 - 1.0.9 - Add kwargs to fs_request_create_form to pass Object props to be used when creating the Object instance
 - 1.0.8 - Cache introspection to improve performance.  All model definitions are cached after first use.  It is no longer possible to alter model definitions dynamically.
-- 1.0.7 - Add json request body support to post update.
-- 1.0.5 - Allow sorting of json lists.
+- 1.0.7 - Add JSON request body support to post update.
+- 1.0.5 - Allow sorting of JSON lists.
 
 ## Licensing
 
 - Apache 2.0
```

### Comparing `flask-serialize-2.1.3/flask_serialize/__init__.py` & `flask-serialize-2.2.0/flask_serialize/__init__.py`

 * *Files identical despite different names*

### Comparing `flask-serialize-2.1.3/flask_serialize/flask_serialize.py` & `flask-serialize-2.2.0/flask_serialize/flask_serialize.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,26 @@
 from datetime import datetime, time
 from typing import Type, List
 
 from flask import request, jsonify, abort, current_app, Response
 from permissive_dict import PermissiveDict
 
 
+TRUTHY_VALUES = ("y", "Y", "yes", "Yes", "YES", True, "true", "True", "TRUE", 1, "1")
+
+
+def is_truthy(value) -> bool:
+    """
+    return True if value seems to be a true value.
+    :param value:
+    :return: True or False
+    """
+    return value in TRUTHY_VALUES
+
+
 class FlaskSerializeNoDb(Exception):
     def __init__(self):
         super().__init__('FlaskSerializeMixin property "db" is not set')
 
 
 class FlaskSerializeMixin:
     """
@@ -47,22 +59,24 @@
     __fs_convert_types_original__ = __fs_convert_types__.copy()
     # types that can be converted to json
     __fs_json_types = [str, dict, list, int, float, bool]
     # default field name when restricting to a particular user
     __fs_user_field__ = "user"
     # properties or fields to return when updating using get or post
     __fs_update_properties__ = []
+    # allow auto request filter_by on fs_get_delete_put_post
+    __fs_filter_by__ = True
     # db is required to be set for updating/deletion functions
     db = None
     # cache model properties
     __fs_model_props = {}
     # previous values of an instance before update attempted
     __fs_previous_field_value__ = {}
     # current version
-    __fs_version__ = "2.1.1"
+    __fs_version__ = "2.2.0"
 
     @staticmethod
     def __fs_json_converter__(value):
         """
         convert a json string to a dict using json if required.
         if encoder error try converting from direct Python
         If not a string then use the value directly
@@ -354,15 +368,15 @@
 
         :param value: string to convert
         :return: decoded string
         """
         if value in ["", None]:
             return {}
 
-        if type(value) == str:
+        if isinstance(value, str):
             return json.loads(value)
 
         if type(value) in FlaskSerializeMixin.__fs_json_types:
             return value
 
         return {"value": str(value)}
 
@@ -410,15 +424,18 @@
                 "DECIMAL": float,
                 "LOB": self.__fs_lob_converter,
                 "BLOB": self.__fs_lob_converter,
                 "CLOB": self.__fs_lob_converter,
             }
 
             # SQL columns
-            props.__exclude_fields = ["fs_as_dict", "fs_as_json",] + [
+            props.__exclude_fields = [
+                "fs_as_dict",
+                "fs_as_json",
+            ] + [
                 self._fs_get_field_name(f) for f in self.__fs_exclude_serialize_fields__
             ]
             field_list = list(self.__table__.columns)
             if "sqlite" in self.__table__.dialect_options:
                 props.DIALECT = "sqlite"
                 self.__fs_convert_types__[
                     str(datetime)
@@ -509,16 +526,18 @@
 
             if v is None:
                 d[c.name] = ""
             elif c.converter:
                 try:
                     d[c.name] = c.converter(v)
                 except Exception as e:
-                    d[c.name] = 'Error:"{}". Failed to convert [{}] type:{}'.format(
-                        e, c.name, c.c_type
+                    d[
+                        c.name
+                    ] = 'Error:"{}". Failed to convert [{}] type:{} value:{}'.format(
+                        e, c.name, c.c_type, v
                     )
                     current_app.logger.warning(d[c.name])
         return d
 
     def __fs_get_update_field_type(self, field, value):
         """
         get the type of the update to db field from cached table properties
@@ -800,21 +819,15 @@
         if user is not None and item_id is not None:
             item = cls.fs_get_by_user_or_404(item_id, user=user)
         elif item_id is not None:
             item = cls.query.get_or_404(item_id)
             if not item.__fs_can_access__():
                 return Response("Access forbidden", 403)
         elif request.method == "GET":
-            # no item id get a list of items
-            if user:
-                kwargs = {cls.__fs_user_field__: user}
-                result = cls.query.filter_by(**kwargs)
-            else:
-                result = cls.query.all()
-            return cls.fs_json_list(result, prop_filters=prop_filters)
+            return cls.__get_all(prop_filters, user)
 
         try:
             if not item:
                 if request.method == "POST":
                     return cls.fs_request_create_form().fs_as_json
                 return Response("METHOD forbidden", 405)
 
@@ -846,14 +859,68 @@
                     return jsonify(dict(item=item.fs_as_dict, message="Deleted"))
                 return Response("DELETE forbidden", 403)
 
         except Exception as e:
             return str(e), cls.__fs_http_error_code
 
     @classmethod
+    def __get_all(cls, prop_filters, user):
+        """
+        get all the items as per arg filters and user
+
+        :param prop_filters: after query prop filters
+        :param user: user to filter by
+        :return:
+        """
+
+        def convert_value(field_name, value):
+            """
+            convert arg to db value
+
+            :param field_name:
+            :param value:
+            :return:
+            """
+            column_attr = getattr(cls, field_name)
+            if not column_attr:
+                return value
+            try:
+                if column_attr.type.python_type == int:
+                    return int(value)
+                if column_attr.type.python_type == float:
+                    return float(value)
+                if column_attr.type.python_type == bool:
+                    return is_truthy(value)
+            except:
+                pass
+            return value
+
+        kwargs = dict()
+
+        if cls.__fs_filter_by__ and request.method == "GET":
+            kwargs = dict(request.args)
+
+        try:
+            # don't allow filtering by excluded fields
+            for field_name, value in kwargs.items():
+                if field_name in cls.__fs_exclude_serialize_fields__:
+                    del kwargs[field_name]
+                else:
+                    kwargs[field_name] = convert_value(field_name, value)
+
+            if user:
+                kwargs[cls.__fs_user_field__] = user
+
+            result = cls.query.filter_by(**kwargs)
+        except Exception as e:
+            return str(e), cls.__fs_http_error_code
+
+        return cls.fs_json_list(result, prop_filters=prop_filters)
+
+    @classmethod
     def fs_json_first(cls, **kwargs):
         """
         return the first result in json response format using the filter_by arguments, or {} if no result
         or not __fs_can_access__()
 
         :param kwargs: SQLAlchemy query.filter_by arguments
         :return: flask response json item or {} if no result
```

### Comparing `flask-serialize-2.1.3/flask_serialize/form_page.py` & `flask-serialize-2.2.0/flask_serialize/form_page.py`

 * *Files identical despite different names*

### Comparing `flask-serialize-2.1.3/flask_serialize.egg-info/PKG-INFO` & `flask-serialize-2.2.0/flask_serialize.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 Metadata-Version: 2.1
 Name: flask-serialize
-Version: 2.1.3
+Version: 2.2.0
 Summary: Easy to use JSON serialization and update/create for Flask and SQLAlchemy.
 Home-page: https://github.com/Martlark/flask-serialize
-Download-URL: https://github.com/Martlark/flask-serialize/archive/2.1.3.tar.gz
+Download-URL: https://github.com/Martlark/flask-serialize/archive/2.2.0.tar.gz
 Author: Andrew Rowe
 Author-email: rowe.andrew.d@gmail.com
 License: Apache Software License
 Keywords: flask sqlalchemy serialize serialization serialise
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Framework :: Flask
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: Permissive-Dict
 
 # flask-serialize
 
 # DB Model JSON serialization with PUT, POST write for Flask applications using SQLAlchemy
 
 ## Installation
 
@@ -114,65 +114,65 @@
 
     def __repr__(self):
         return '<Setting %r %r %r>' % (self.id, self.setting_type, self.value)
 ```
 
 ## Routes setup
 
-Get a single item as json.
+Get a single item as JSON.
 
 ```python
 @app.route('/get_setting/<item_id>', methods=['GET'])
 def get_setting( item_id ):
     return Setting.fs_get_delete_put_post(item_id)
 
-# Returns a Flask response with a json object, example:
+# Returns a Flask response with a JSON object, example:
 ```
 
 ```JavaScript
 {id:1, value: "hello"}
 ```
 
-Put an update to a single item as json.
+Put an update to a single item as JSON.
 
 ```python
 @app.route('/update_setting/<item_id>', methods=['PUT'])
 def update_setting( item_id ):
     return Setting.fs_get_delete_put_post(item_id)
 
-# Returns a Flask response with the result as a json object:
+# Returns a Flask response with the result as a JSON object:
 
 ```
 
 ```JavaScript
 {message: "success message"}
 ```
 
 Delete a single item.
 
 ```python
 @app.route('/delete_setting/<item_id>', methods=['DELETE'])
 def delete_setting( item_id ):
     return Setting.fs_get_delete_put_post(item_id)
 
-# Returns a Flask response with the result and item deleted as a json response:
+# Returns a Flask response with the result and item deleted as a JSON response:
 ```
 
 ```JavaScript
 {message: "success message", item: {"id":5, name: "gone"}}
 ```
 
-Get all items as a json list.
+Get all items as a JSON list.
 
 ```python
 @app.route('/get_setting_all', methods=['GET'])
 def get_setting_all():
     return Setting.fs_get_delete_put_post()
 
-# Returns a Flask response with a list of json objects, example:
+# Returns a Flask response with a list of JSON objects, example:
 ```
 
 ```JavaScript
 [{id:1, value: "hello"},{id:2, value: "there"},{id:3, value: "programmer"}]
 ```
 
 All of: get-all, get, put, post, and delete can be combined in one route.
@@ -180,15 +180,15 @@
 ```python
 @app.route('/setting/<int:item_id>', methods=['GET', 'PUT', 'DELETE', 'POST'])
 @app.route('/setting', methods=['GET', 'POST'])
 def route_setting_all(item_id=None):
     return Setting.fs_get_delete_put_post(item_id)
 ```
 
-Updating from a json object in the flask put request
+Updating from a JSON object in the Flask put request
 
 JQuery example:
 
 ```javascript
 function put(setting_id) {
         return $.ajax({
             url: `/update_setting/${setting_id}`,
@@ -283,20 +283,20 @@
 ```
 
 # Writing and creating
 
 When using any of the convenience methods to update, create or delete an object these properties and
 methods control how flask-serialize handles the operation.
 
-## Updating from a form or json
+## Updating from a form or JSON
 
 ```python
 def fs_request_update_json():
     """
-    Update an item from request json data or PUT params, probably from a PUT or PATCH.
+    Update an item from request JSON data or PUT params, probably from a PUT or PATCH.
     Throws exception if not valid
 
     :return: True if item updated
 
     """
 ```
 
@@ -311,15 +311,15 @@
         if message.fs_request_update_json():
             return 'Updated'
 ```
 
 ```python
 def fs_request_update_json():
     """
-    Update an item from request json data or PUT params, probably from a PUT or PATCH.
+    Update an item from request JSON data or PUT params, probably from a PUT or PATCH.
     Throws exception if not valid
 
     :return: True if item updated
 
     """
 ```
 
@@ -392,16 +392,17 @@
 ```
 
 Override the mixin `__fs_can_access__` to provide control over when an
 item can be read or accessed.  Return False to exclude from results.
 
 ## Private fields
 
-Fields can be made private for certain reasons by overriding the `__fs_private_field__` method
-and returning `True` if the field is to be private.
+Fields can be made private by overriding the `__fs_private_field__` method
+and returning `True` if the field is to be private.  These fields will not be returned
+in JSON results.
 
 Private fields will be excluded for any get, put and post methods.
 
 Example:
 
 To exclude private fields when a user is not the admin.
 
@@ -448,15 +449,15 @@
 ```
 
 This can be used to communicate from the model on the server to the JavaScript code
 interesting things from updates
 
 ## `__fs_create_fields__`
 
-List of model fields to be read from a form or json when creating an object.  Can be the specified as either 'text' or
+List of model fields to be read from a form or JSON when creating an object.  Can be the specified as either 'text' or
 the field. Do not put primary keys here.  Do not put foreign keys here if using SQLAlchemy child insertion.
 This is usually the same as `__fs_update_fields__`.  When `__fs_create_fields__` is empty all column fields can be inserted.
 
 Used by these methods:
 
 - fs_request_create_form
 - fs_get_delete_put_post
@@ -510,38 +511,58 @@
 
 List of model field names to not serialize at all.
 
 ```python
 __fs_exclude_serialize_fields__ = []
 ```
 
-List of model field names to not serialize when returning as json.
+List of model field names to not serialize when returning as JSON.
 
 ```python
 __fs_exclude_json_serialize_fields__ = []
 ```
 
-## Filtering json list results
+## Built in query_by using request arg on GET
+
+`fs_get_delete_put_post` by default supports automatic passing of GET request args to the query method using
+a `filter_by` clause. Example using a Flask route that be default returns all messages:
+
+
+```python
+    @route('/message/', methods=['GET'])
+    def route_message():
+        return Message.fs_get_by_user_or_404()
+```
+
+Call the endpoint using URL like:
+
+  /message/?name=hello&lines=12
+
+Will return any message records with the name of 'hello' and with 12 lines.
+
+This feature can be disabled by using `__fs_filter_by = False` on the model definition.
+
+## Filtering JSON list results
 
 Json result lists can be filtered by using the `prop_filters` parameter on either
 the `fs_get_delete_put_post` method or the `fs_json_list` method.
 
-The filter consists of one or more properties in the json result and
+The filter consists of one or more properties in the JSON result and
 the value that it must match.  Filter items will match against the
 first `prop_filter` property to exactly equal the value.
 
 NOTE: The filter is not applied with single a GET or, the PUT, POST and DELETE methods.
 
 Example to only return dogs:
 
 ```python
 result = fs_get_delete_put_post(prop_filters = {'key':'dogs'})
 ```
 
-## Sorting json list results
+## Sorting JSON list results
 
 Json result lists can be sorted by using the `__fs_order_by_field__` or the `__fs_order_by_field_desc__` properties.  The results
 are sorted after the query is converted to JSON.  As such you can use any property from a class to sort. To sort by id
 ascending use this example:
 
 ```python
 __fs_order_by_field__ = 'id'
@@ -561,15 +582,15 @@
 
 The `fs_query_by_access` method can be used to filter a SQLAlchemy result set so that
 the `user` property and `__fs_can_access__` hook method are used to restrict to allowable items.
 
 Example:
 
 ```python
-result_list = Setting. fs_query_by_access(user='Andrew', setting_type='test')
+result_list = Setting.fs_query_by_access(user='Andrew', setting_type='test')
 ```
 
 Any keyword can be supplied after `user` to be passed to `filter_by` method of `query`.
 
 ## Relationships list of property names that are to be included in serialization
 
 ```python
@@ -680,17 +701,17 @@
 - `user`: user to user as query filter.
 - `prop_filters`: dictionary of key:value pairs to limit results when returning get-all.
 
 | Method Operation | item_id     | Response                                                                                                                                                                                                                                                                                                 |
 |------------------|-------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | GET              | primary key | returns one item when `item_id` is a primary key.  {property1:value1,property2:value2,...}                                                                                                                                                                                                               |
 | GET              | None        | returns all items when `item_id` is None. [{item1},{item2},...]                                                                                                                                                                                                                                          |
-| PUT              | primary key | updates item using `item_id` as the id from request json data.  Calls the model `__fs_verify__`    `{message:message,item:{model_fields,...}`, properties:{`__fs_update_properties__`}} before updating.  Returns new item as {item}                                                                       |
+| PUT              | primary key | updates item using `item_id` as the id from request JSON data.  Calls the model `__fs_verify__`    `{message:message,item:{model_fields,...}`, properties:{`__fs_update_properties__`}} before updating.  Returns new item as {item}                                                                       |
 | DELETE           | primary key | removes the item with primary key of `item_id` if self.__fs_can_delete__ does not throw an error.  `{property1:value1,property2:value2,...}`                                                                                         Returns the item removed.  Calls `__fs_can_delete__` before delete. |
-| POST             | None        | creates and returns a Flask response with a new item as json from form body data or JSON body data {property1:value1,property2:value2,...} When `item_id` is None. Calls the model `__fs_verify__` method before creating.                                                                               |
+| POST             | None        | creates and returns a Flask response with a new item as JSON from form body data or JSON body data {property1:value1,property2:value2,...} When `item_id` is None. Calls the model `__fs_verify__` method before creating.                                                                               |
 | POST             | primary key | updates an item from form data using `item_id`. Calls the model ` __fs_verify__` method before updating.                                                                                                                                                                                                 |
 
 On error returns a response of 'error message' with http status code of 400.
 
 Set the `user` parameter to restrict a certain user.  By default uses the
 relationship of `user`.  Set another relationship field by setting the `__fs_user_field__` to the name of the
 relationship.
@@ -705,33 +726,33 @@
 ```python
 item = Setting.query.get_or_404(2)
 dict_item = item.fs_as_dict()
 ```
 
 ## fs_as_json
 
-Convert a db object into a json Flask response using `jsonify`.  Example:
+Convert a db object into a JSON Flask response using `jsonify`.  Example:
 
 ```python
 @app.route('/setting/<int:item_id>')
 def get_setting(item_id):
     item = Setting.query.get_or_404(item_id)
     return item.fs_as_json()
 ```
 
-## `__fs_after_commit__(self, create=False)`
+## __fs_after_commit__(self, create=False)
 
+Hook to call after any of `fs_update_from_dict`, `fs_request_update_form`, `fs_request_update_json` has been called so that
+you can do what you like.  `self` is the updated or created (create==True) item. Example:
 
 ```python
 def  __fs_after_commit__(self, create=False):
+        logging.info(f'changed! {self}')
 ```
 
-Hook to call after any `fs_update_from_dict`, `fs_request_update_form`, `fs_request_update_json` has been called so that
-you do what you like.  `self` is the updated or created (create==True) item.
-
 NOTE: not called after a `DELETE`
 
 ## `__fs_before_update__(cls, data_dict)`
 
 - data_dict: a dictionary of new data to apply to the item
 - return: the new `data_dict` to use when updating
 
@@ -760,70 +781,70 @@
 def get_items():
     items = Setting.query.all()
     return jsonify(Setting.fs_dict_list(items))
 ```
 
 ## fs_json_list(query_result)
 
-Return a flask response in json list format from a sql alchemy query result.
+Return a flask response in JSON list format from a sql alchemy query result.
 
 .. code:: python
 python
 
 ```
 @bp.route('/address/list', methods=['GET'])
 @login_required
 def address_list():
     items = Address.query.filter_by(user=current_user)
     return Address.fs_json_list(items)
 ```
 
 ## fs_json_filter_by(kw_args)
 
-Return a flask list response in json format using a filter_by query.
+Return a flask list response in JSON format using a filter_by query.
 
 Example:
 
 ```python
 @bp.route('/address/list', methods=['GET'])
 @login_required
 def address_list():
-    return Address.filter_by(user=current_user)
+    return Address.fs_json_filter_by(user=current_user)
 ```
 
 ## fs_json_first(kwargs)
 
-Return the first result in json format using filter_by arguments.
+Return the first result in JSON format using filter_by arguments.
 
 Example:
 
 ```python
 @bp.route('/score/<course>', methods=['GET'])
 @login_required
 def score(course):
     return Score.fs_json_first(class_name=course)
 ```
 
-## `__fs_previous_field_value__`
+## __fs_previous_field_value__
 
-A dictionary of the previous field values before an update is applied from a dict, form or json update operation. Helpful
+A dictionary of the previous field values before an update is applied from a dict, form or JSON update operation. Helpful
 in the `__fs_verify__` method to see if field values are to be changed.
 
 Example:
 
 ```python
 def __fs_verify__(self, create=False):
     previous_value = self.__fs_previous_field_value__.get('value')
     if previous_value != self.value:
         current_app.logger.warning(f'value is changing from {previous_value}')
 ```
 
 ## fs_request_create_form(kwargs)
 
-Use the contents of a Flask request form or request json data to create a item
+Use the contents of a Flask request form or request JSON data to create a item
 in the database.   Calls `__fs_verify__(create=True)`.  Returns the new item or throws error.
 Use kwargs to set the object properties of the newly created item.
 
 Example:
 
 Create a `score` item with the parent being a `course`.
 
@@ -833,15 +854,15 @@
 def score(course_id):
     course = Course.query.get_or_404(course_id)
     return Score.fs_request_create_form(course_id=course.id).fs_as_dict
 ```
 
 ## fs_request_update_form()
 
-Use the contents of a Flask request form or request json data to update an item
+Use the contents of a Flask request form or request JSON data to update an item
 in the database.   Calls `__fs_verify__()` and `__fs_can_update__()` to check
 if can update.  Returns True on success.
 
 Example:
 
 Update a score item.
 
@@ -963,14 +984,15 @@
 - Hook methods start with `__fs_` and end with `__`.
 - Control properties start with `__fs_` and end with `__`.
 - Some hook functions can now return False or True rather than just raise Exceptions
 - fs_get_delete_put_post now returns a HTTP code that is more accurate of the cause
 
 ## Release Notes
 
+- 2.2.0 - Allow arg parameters to be used in `fs_get_delete_put_post` 'GET' as query_by filters
 - 2.1.3 - Allow sorting by lambda
 - 2.1.2 - Fix readme table format
 - 2.1.1 - Improve sqlite JSON handling
 - 2.1.0 - Convert readme to markdown.  Add support for JSON columns.  Withdraw Python 3.6 Support. Use unittest instead of pytest.  NOTE: Changes `__fs_convert_types__` to a `dict`.
 - 2.0.3 - Allow more use of model column variables instead of "quoted" field names.  Fix missing import for FlaskSerialize.
 - 2.0.2 - Fix table formatting.
 - 2.0.1 - Try to get properties and methods to use more appropriate names.
@@ -978,25 +1000,25 @@
 - 1.5.1 - Fix TypeError: unsupported operand type(s) for +=: 'ImmutableColumnCollection' and 'list' with newer versions of SQLAlchemy
 - 1.5.0 - Return item from POST/PUT updates. Allow `__fs_create_fields__` and `__fs_update_fields__` to be specified using the column fields.  None values serialize as null/None.  Restore previous `__fs_update_properties__` behaviour.  By default, updates/creates using all fields. Exclude primary key from create and update.
 - 1.4.2 - by default return all props with `__fs_update_properties__`
 - 1.4.1 - Add better exception message when `db` mixin property not set.  Add `FlaskSerialize` factory method.
 - 1.4.0 - Add `__fs_private_field__` method.
 - 1.3.1 - Fix incorrect method signatures.  Add fs_query_by_access method.
 - 1.3.0 - Add `__fs_can_update__` and `__fs_can_access__` methods for controlling update and access.
-- 1.2.1 - Add support to change the user field name for get_put_post_delete user= parameter.
+- 1.2.1 - Add support to change the user field name for fs_get_delete_put_post user= parameter.
 - 1.2.0 - Add support for decimal, numeric and clob.  Treat all VARCHARS the same.  Convert non-list relationship.
 - 1.1.9 - Allow FlaskSerializeMixin to be converted when a property value.
 - 1.1.8 - Move form_page to separate MixIn.  Slight refactoring.  Add support for complex type to db.
 - 1.1.6 - Make sure all route returns use jsonify as required for older Flask versions.  Add `__fs_before_update__` hook.
 - 1.1.5 - Add `__fs_previous_field_value__` array that is set during update.  Allows comparing new and previous values during  `__fs_verify__`.
 - 1.1.4 - Fix doco typos and JavaScript examples.  Add form_page method.  Improve test and example apps.  Remove Python 2, 3.4 testing and support.
 - 1.1.3 - Fix duplicate db writes.  Return item on delete.  Remove obsolete code structures.  Do not update with non-existent fields.
 - 1.1.2 - Add 400 http status code for errors, remove error dict.  Improve documentation.
 - 1.1.0 - Suppress silly errors. Improve documentation.
 - 1.0.9 - Add kwargs to fs_request_create_form to pass Object props to be used when creating the Object instance
 - 1.0.8 - Cache introspection to improve performance.  All model definitions are cached after first use.  It is no longer possible to alter model definitions dynamically.
-- 1.0.7 - Add json request body support to post update.
-- 1.0.5 - Allow sorting of json lists.
+- 1.0.7 - Add JSON request body support to post update.
+- 1.0.5 - Allow sorting of JSON lists.
 
 ## Licensing
 
 - Apache 2.0
```

### Comparing `flask-serialize-2.1.3/setup.py` & `flask-serialize-2.2.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,15 +36,14 @@
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Framework :: Flask",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Operating System :: POSIX",
         "Operating System :: MacOS",
         "Operating System :: Unix",
```

### Comparing `flask-serialize-2.1.3/test/test_app.py` & `flask-serialize-2.2.0/test/test_app.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import json
 import random
 import string
 import time
+import unittest
 from http import HTTPStatus
 from datetime import datetime
 from pathlib import Path
-from sqlalchemy import text, exc
-from sqlalchemy.exc import OperationalError
+from sqlalchemy import text
 
 import flask_unittest
 
-
-from test.test_flask_app import app, db, Setting, SubSetting, SimpleModel, DateTest
+from flask_serialize import FlaskSerializeMixin
+from test.test_flask_app import db, Setting, SubSetting, SimpleModel, DateTest
 
 
 def random_string(length=20):
     """
     return a <length> long character random string of ascii_letters
     :param length: {int} number of characters to return
     :return:
@@ -38,14 +38,16 @@
         :return:
         """
         with app.app_context():
             db.drop_all()
             db.create_all()
 
     def create_app(self):
+        from test.test_flask_app import app
+
         app.config["TESTING"] = True
         app.config["SECRET_KEY"] = "Testing"
         app.config["WTF_CSRF_ENABLED"] = False
         app.testing = True
         yield app
 
     def tearDown(self, app, client):
@@ -54,15 +56,16 @@
 
 
 class TestAll(TestBase):
     def tearDown(self, app, client):
         Setting.__fs_order_by_field__ = "value"
         Setting.__fs_order_by_field_desc__ = None
 
-    def add_setting(self, client, key=random_string(), value="test-value", number=0):
+    @staticmethod
+    def add_setting(client, key=random_string(), value="test-value", number=0):
         rv = client.post(
             "/setting_add",
             data=dict(setting_type="test", key=key, value=value, number=number),
         )
         assert rv.status_code == 302
         item = Setting.query.filter_by(key=key).first()
         assert item
@@ -140,14 +143,64 @@
             assert rv.json[0]["key"] == key
         # all as dict list
         result = Setting.query.all()
         fs_dict_list = Setting.fs_dict_list(result)
         assert len(fs_dict_list) == 1
         assert fs_dict_list[0]["key"] == key
 
+    def test_get_filter_keywords(self, app, client):
+        # test add
+        key = random_string()
+        item = self.add_setting(client, key=key, value="123", number=9)
+        item = self.add_setting(client, key=key, value="456")
+
+        # one value
+        rv = client.get("/setting_get_all?value=123")
+        assert rv.status_code == HTTPStatus.OK, rv.data
+        assert len(rv.json) == 1
+        assert rv.json[0]["value"] == "123"
+        assert rv.json[0]["number"] == 18, rv.json  # number is doubled
+
+        # two values
+        rv = client.get(f"/setting_get_all?value=123&key={key}")
+        assert rv.status_code == HTTPStatus.OK, rv.data
+        assert len(rv.json) == 1
+        assert rv.json[0]["value"] == "123"
+
+        # no match
+        rv = client.get("/setting_get_all?value=nothing")
+        assert rv.status_code == HTTPStatus.OK
+        assert len(rv.json) == 0
+
+        # invalid field_name
+        rv = client.get("/setting_get_all?floogle=nothing")
+        assert rv.status_code == HTTPStatus.BAD_REQUEST
+
+        # type conversion
+        rv = client.get("/setting_get_all?number=18")
+        assert rv.status_code == HTTPStatus.OK
+        assert len(rv.json) == 1, rv.json
+
+    def test_filter_by_false(self, app, client):
+        # disable auto query
+        rv = client.post("/simple_add", data=dict(value=123))
+        assert rv.status_code == HTTPStatus.OK
+        rv = client.post("/simple_add", data=dict(value=456))
+        assert rv.status_code == HTTPStatus.OK
+        rv = client.post("/simple_add", data=dict(value="hello"))
+        assert rv.status_code == HTTPStatus.OK
+
+        rv = client.get("/simple")
+        assert rv.status_code == HTTPStatus.OK, rv.data
+        assert len(rv.json) == 3, len(rv.json)
+
+        rv = client.get("/simple?value=123")
+        assert rv.status_code == HTTPStatus.OK, rv.data
+        assert len(rv.json) == 3, len(rv.json)
+
     def test_get_user(self, app, client):
         key = random_string()
         # test add 2 settings
         client.post(
             "/setting_add", data=dict(setting_type="test", key=key, value="test-value")
         )
         test_user_name = random_string()
@@ -339,14 +392,25 @@
         assert rv.status_code == 302
         item = Setting.query.filter_by(key=key).first()
         assert item
         assert item.value == value
         rv = client.delete("/setting_delete/{}".format(item.id))
         assert rv.status_code == 400
         assert rv.data == b"Deletion not allowed.  Magic value!"
+        key = random_string()
+        value = "5678"
+        rv = client.post(
+            "/setting_add", data=dict(setting_type="test", key=key, value=value)
+        )
+        assert rv.status_code == 302
+        item = Setting.query.filter_by(key=key).first()
+        assert item
+        assert item.value == value
+        rv = client.delete("/setting_delete/{}".format(item.id))
+        assert rv.status_code == HTTPStatus.OK
 
     def test_column_conversion(self, app, client):
         # create
         key = random_string()
         value = "12.34"
         j_value = dict(a=123, b=True)
         rv = client.post(
@@ -484,14 +548,64 @@
             data=dict(setting_type="test", key=key, value=new_value, number=10),
         )
         assert rv.status_code == 200
         assert rv.json["message"] == "Updated"
         item = Setting.query.get_or_404(item.id)
         assert "n" == item.active
 
+    def test_fs_get_delete_put_post__fs_filter_by__(self, app, client):
+        key_test_value_1 = random_string()
+        # create using post
+        rv = client.post(
+            "/setting_post",
+            data=dict(
+                setting_type="test",
+                key=key_test_value_1,
+                value="test-value_1",
+                number=10,
+            ),
+        )
+        assert rv.status_code == 200
+        key_test_value_2 = random_string()
+        # create using post
+        rv = client.post(
+            "/setting_post",
+            data=dict(
+                setting_type="test",
+                key=key_test_value_2,
+                value="test-value_2",
+                number=10,
+            ),
+        )
+        assert rv.status_code == 200
+
+        items = client.get("/setting_get_all")
+        self.assertEqual(2, len(items.json))
+
+        rv = client.get("/setting_get_all?flog=blog")
+        assert rv.status_code == HTTPStatus.BAD_REQUEST
+
+        items = client.get("/setting_get_all?value=test-value_2")
+        self.assertEqual(1, len(items.json))
+        self.assertEqual(key_test_value_2, items.json[0]["key"])
+
+        items = client.get("/setting_get_all?value=test-value_3")
+        self.assertEqual(0, len(items.json))
+
+        item = client.post("/simple_add", data=dict(value=key_test_value_1))
+        assert item.status_code == HTTPStatus.OK
+        item = client.get("/simple")
+
+        assert item.status_code == HTTPStatus.OK
+        self.assertEqual(1, len(item.json))
+        # should not apply filter
+        item = client.get("/simple?value=wrong")
+        assert item.status_code == HTTPStatus.OK
+        self.assertEqual(1, len(item.json), item.data)
+
     def test_fs_get_delete_put_post(self, app, client):
         key = random_string()
         # create using post
         rv = client.post(
             "/setting_post",
             data=dict(setting_type="test", key=key, value="test-value", number=10),
         )
@@ -833,13 +947,21 @@
 
     def test_user(self, app, client):
         test_value = random_string()
         user_name = random_string()
         # test add user
         # get by id
         rv = client.post("/user", data={"name": user_name})
-        assert rv.json["name"] == user_name
+        assert rv.json["name"] == user_name, rv.json
         user_id = rv.json["id"]
         # add data
         rv = client.post(f"/user_add_data/{user_id}", data={"data": test_value})
         assert rv.json["name"] == user_name
         assert test_value in [item.get("value") for item in rv.json["data_items"]]
+
+
+class TestVersion(unittest.TestCase):
+    def test_version(self):
+        version_file = "../VERSION"
+        version = open(version_file).read().strip()
+
+        self.assertEqual(FlaskSerializeMixin.__fs_version__, version)
```

### Comparing `flask-serialize-2.1.3/test/test_flask_app.py` & `flask-serialize-2.2.0/test/test_flask_app.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from flask_serialize.flask_serialize import (
     FlaskSerialize,
     FlaskSerializeMixin,
 )
 from flask_serialize.form_page import FormPageMixin
 
-app = Flask("test_app")
+app: Flask = Flask("test_app")
 app.testing = True
 app.config["SQLALCHEMY_TRACK_MODIFICATIONS"] = False
 app.config["SQLALCHEMY_DATABASE_URI"] = os.environ.get(
     "SQLALCHEMY_DATABASE_URI", "sqlite:///:memory:"
 )
 db = SQLAlchemy(app)
 migrate = Migrate(app, db)
@@ -93,14 +93,15 @@
 @app.route("/sub_setting_delete/<int:item_id>", methods=["DELETE"])
 @app.route("/sub_setting_put/<int:item_id>", methods=["PUT", "POST"])
 @app.route("/sub_setting_get/<int:item_id>", methods=["GET"])
 def route_sub_setting_fs_get_delete_put_post(item_id=None, user="fake"):
     return SubSetting.fs_get_delete_put_post(item_id, user)
 
 
+@app.get("/simple")
 @app.route("/simple_add", methods=["POST"])
 @app.route("/simple_edit/<int:item_id>", methods=["PUT", "POST"])
 def route_simple_fs_get_delete_put_post(item_id=None, user=None):
     return SimpleModel.fs_get_delete_put_post(item_id, user)
 
 
 @app.route("/setting_get_json/<int:item_id>", methods=["GET"])
@@ -393,17 +394,17 @@
     __fs_update_properties__ = ["prop_test"]
     __fs_order_by_field__ = "value"
     # lob
     __fs_column_type_converters__ = {"LOB": lambda v: str(v)}
     # convert types
     __fs_scheduled_date_format__ = "%Y-%m-%d %H:%M:%S"
     __fs_convert_types__ = {
-        str(bool): lambda v: "y"
-        if (type(v) == bool and v) or str(v).lower() == "true"
-        else "n",
+        str(bool): lambda v: (
+            "y" if (type(v) == bool and v) or str(v).lower() == "true" else "n"
+        ),
         str(int): lambda n: int(n) * 2,
         str(datetime): lambda n: datetime.strptime(
             n, Setting.__fs_scheduled_date_format__
         ),
     }
     # form_page
     form_page_form = EditForm
@@ -505,14 +506,15 @@
     def __repr__(self):
         return "Setting {}".format(self.key)
 
 
 class SimpleModel(fs_mixin, db.Model):
     id = db.Column(db.Integer, primary_key=True)
     value = db.Column(db.String(30), default="")
+    __fs_filter_by__ = False
 
     @property
     def prop(self):
         return "prop:" + self.value
 
     def __repr__(self):
         return "<SimpleModel %r>" % (self.value)
```

