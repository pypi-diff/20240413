# Comparing `tmp/ownlib-0.0.1a4.tar.gz` & `tmp/ownlib-0.0.1b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ownlib-0.0.1a4.tar", max compression
+gzip compressed data, was "ownlib-0.0.1b4.tar", max compression
```

## Comparing `ownlib-0.0.1a4.tar` & `ownlib-0.0.1b4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    35149 2022-10-30 19:22:48.704414 ownlib-0.0.1a4/LICENSE
--rw-r--r--   0        0        0      140 2024-03-03 12:27:11.775267 ownlib-0.0.1a4/README.md
--rw-r--r--   0        0        0      580 2024-03-06 19:21:48.975829 ownlib-0.0.1a4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-03 12:27:11.775267 ownlib-0.0.1a4/src/ownlib/__init__.py
--rw-r--r--   0        0        0     2208 2024-03-03 19:47:57.101163 ownlib-0.0.1a4/src/ownlib/class_person.py
--rw-r--r--   0        0        0     4503 2024-03-04 18:43:34.567328 ownlib-0.0.1a4/src/ownlib/class_whatsapp_message.py
--rw-r--r--   0        0        0    13461 2024-03-04 18:43:34.555328 ownlib-0.0.1a4/src/ownlib/functions_whatsapp_refueling.py
--rw-r--r--   0        0        0     2074 2024-03-03 19:20:30.220277 ownlib-0.0.1a4/src/ownlib/months.py
--rw-r--r--   0        0        0     9806 2024-03-04 18:43:34.571328 ownlib-0.0.1a4/src/ownlib/my_datalib.py
--rw-r--r--   0        0        0      390 2024-03-03 19:53:59.412299 ownlib-0.0.1a4/src/ownlib/my_fileio.py
--rw-r--r--   0        0        0     9376 2024-03-03 17:56:39.624958 ownlib-0.0.1a4/src/ownlib/mytinylib.py
--rw-r--r--   0        0        0     1708 2024-03-03 12:27:11.779267 ownlib-0.0.1a4/src/ownlib/one_s_uat_lib.py
--rw-r--r--   0        0        0      164 2024-03-03 12:27:11.779267 ownlib-0.0.1a4/src/ownlib/platon_settings.py
--rw-r--r--   0        0        0     4907 2024-03-03 12:27:11.779267 ownlib-0.0.1a4/src/ownlib/txt_lib.py
--rw-r--r--   0        0        0     2138 2024-03-03 19:38:30.980129 ownlib-0.0.1a4/src/ownlib/whapp_funcs.py
--rw-r--r--   0        0        0      651 1970-01-01 00:00:00.000000 ownlib-0.0.1a4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-10-30 19:22:48.704414 ownlib-0.0.1b4/LICENSE
+-rw-r--r--   0        0        0      140 2024-03-03 12:27:11.775267 ownlib-0.0.1b4/README.md
+-rw-r--r--   0        0        0      638 2024-04-13 19:28:55.405393 ownlib-0.0.1b4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-03 12:27:11.775267 ownlib-0.0.1b4/src/ownlib/__init__.py
+-rw-r--r--   0        0        0     2213 2024-04-12 17:12:32.850420 ownlib-0.0.1b4/src/ownlib/class_person.py
+-rw-r--r--   0        0        0     4503 2024-04-12 17:12:32.850420 ownlib-0.0.1b4/src/ownlib/class_whatsapp_message.py
+-rw-r--r--   0        0        0    13461 2024-04-12 17:12:32.850420 ownlib-0.0.1b4/src/ownlib/functions_whatsapp_refueling.py
+-rw-r--r--   0        0        0     2074 2024-04-12 17:12:32.850420 ownlib-0.0.1b4/src/ownlib/months.py
+-rw-r--r--   0        0        0     9806 2024-04-12 17:12:32.850420 ownlib-0.0.1b4/src/ownlib/my_datalib.py
+-rw-r--r--   0        0        0      390 2024-04-12 17:12:32.850420 ownlib-0.0.1b4/src/ownlib/my_fileio.py
+-rw-r--r--   0        0        0     9512 2024-04-12 17:12:32.850420 ownlib-0.0.1b4/src/ownlib/mytinylib.py
+-rw-r--r--   0        0        0     1708 2024-03-03 12:27:11.779267 ownlib-0.0.1b4/src/ownlib/one_s_uat_lib.py
+-rw-r--r--   0        0        0      164 2024-03-03 12:27:11.779267 ownlib-0.0.1b4/src/ownlib/platon_settings.py
+-rw-r--r--   0        0        0     5257 2024-04-12 17:12:32.850420 ownlib-0.0.1b4/src/ownlib/txt_lib.py
+-rw-r--r--   0        0        0     2138 2024-04-12 17:12:32.850420 ownlib-0.0.1b4/src/ownlib/whapp_funcs.py
+-rw-r--r--   0        0        0      702 1970-01-01 00:00:00.000000 ownlib-0.0.1b4/PKG-INFO
```

### Comparing `ownlib-0.0.1a4/LICENSE` & `ownlib-0.0.1b4/LICENSE`

 * *Files identical despite different names*

### Comparing `ownlib-0.0.1a4/pyproject.toml` & `ownlib-0.0.1b4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ownlib"
-version = "0.0.1a4"
+version = "0.0.1b4"
 description = "Sample pypi project"
 authors = ["Андрей Мартынов <real.cloudhunter@gmail.com>"]
 license = "GNU"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
@@ -15,14 +15,18 @@
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.0.2"
 pylint = "^3.1.0"
 mypy = "^1.8.0"
 pandas-stubs = "^2.2.0.240218"
 flake8 = "^7.0.0"
 
+
+[tool.poetry.group.test.dependencies]
+pytest = "^8.1.1"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.mypy]
 python_version = 3.11
 follow_imports = "skip"
```

### Comparing `ownlib-0.0.1a4/src/ownlib/class_person.py` & `ownlib-0.0.1b4/src/ownlib/class_person.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from loguru import logger
 
 logger.disable(__name__)
 
 
 # noinspection SpellCheckingInspection
 @dataclass
-class PersonName:
+class PersonNames:
     """
     Object for storage and tiny manipulating person name`s data\n
     Set name, first, middlename, lastname attribs,\n
     TODO FIX unprocessing case with 'Doe J.J.' - like buffer!
     Strip extra spaces,\n
     Titling first characters,\n
     Set order in fullname via order (f-irst, m-iddlle, l-ast), default = 'lfm'.\n
@@ -52,12 +52,12 @@
                 _result = ''
             return _result
 
         self.initial_firstname = _get_initial(self.firstname)
         self.initial_middlename = _get_initial(self.middlename)
 
 
-class Person(PersonName):
+class Person(PersonNames):
     """
-    TODO FIX unprocessing case with 'Doe J.J.' - like buffer!
+    TODO FIX none processing case with 'Doe J.J.' - like buffer!
     """
     logger.debug(f"Some define log from Person")
```

### Comparing `ownlib-0.0.1a4/src/ownlib/class_whatsapp_message.py` & `ownlib-0.0.1b4/src/ownlib/class_whatsapp_message.py`

 * *Files identical despite different names*

### Comparing `ownlib-0.0.1a4/src/ownlib/functions_whatsapp_refueling.py` & `ownlib-0.0.1b4/src/ownlib/functions_whatsapp_refueling.py`

 * *Files identical despite different names*

### Comparing `ownlib-0.0.1a4/src/ownlib/months.py` & `ownlib-0.0.1b4/src/ownlib/months.py`

 * *Files identical despite different names*

### Comparing `ownlib-0.0.1a4/src/ownlib/my_datalib.py` & `ownlib-0.0.1b4/src/ownlib/my_datalib.py`

 * *Files identical despite different names*

### Comparing `ownlib-0.0.1a4/src/ownlib/mytinylib.py` & `ownlib-0.0.1b4/src/ownlib/mytinylib.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 """
 Short useful functions library
 """
 from typing import (Any,
-                    Tuple,
                     Union
-)
+                    )
 import os
 from glob import glob
 import pathlib
 from hashlib import md5
 
 from datetime import datetime
 import pandas
 from IPython.display import clear_output
 
 from loguru import logger
 
 from ownlib.txt_lib import (digit_only,
                             EMPTY_STR
-)
+                            )
 
 
 def non_filtering_mask(data_frame: pandas.DataFrame) -> pandas.DataFrame:
     """
     Prepare a non-filtering mask with a shape and columns similar to the tmp_df
     :param data_frame: Pandas.DataFrame, for which prep the mask
     :return: Non-filtering mask
@@ -56,18 +55,18 @@
                     string_pattern: str = '*',
                     postfix: str = EMPTY_STR,
                     drop_last_insert: bool = True) -> str:
     """
     Make repeated patterns string
 
     :param repeat_num: int, num of repeating
-    :param string_pattern: str, repeated pattern (default = '*')
-    :param postfix: str, pattern, inserting between two char_pattern
-    :param drop_last_insert: bool, drop last insert_pattern if True (default)
-    :returns: str, like (char_pattern + insert_pattern) * repeat_num
+    :param string_pattern: str - repeated pattern, default = '*'
+    :param postfix: str - pattern, inserting between two char_pattern
+    :param drop_last_insert: bool - drop last insert_pattern if True (default)
+    :returns: str - like (char_pattern + insert_pattern) * repeat_num
     """
     hyper_pattern = string_pattern + postfix
     got_string = hyper_pattern * repeat_num
     if drop_last_insert:
         got_string = got_string[:len(got_string) - len(postfix)]
 
     return got_string
@@ -85,15 +84,16 @@
 
         print(div_line)
         for i, item in enumerate(choices):
             print(f"{i}: {item}")
         print(div_line)
     # TODO THOUGHT ABOUT THIS CASE NECESSARY
     elif axe == 'h':
-        choices_in_line = '  '.join(f"{i}:{variant}" for i, variant in enumerate(choices))
+        choices_in_line = '  '.join(f"{i}:{variant}" for i, variant in
+                                    enumerate(choices))
         div_line = repeated_string(len(choices_in_line))
         print(div_line)
         print(choices_in_line)
         print(div_line)
     else:
         logger.error(f"[!] Unknown {axe=}")
 
@@ -103,42 +103,44 @@
     Show warning message
     :param message:
     :return: None
     """
     print(f"[!] Wrong input value: {message}")
 
 
-def last_index(iterator: list) -> int:
+def last_index(sequence: Union[str, list, tuple, set]) -> int:
     """
     Return last iterator index\n
-    :param iterator: - list for example
+    :param sequence: - data sequence for example
     :return: last index in iterator
     """
-    return len(iterator) - 1
+    return len(sequence) - 1
 
 
-def get_choice_position(choices: list, axe: str = 'v') -> Union[int, None]:
+def get_choice_position(choices: list[str], axe: str = 'v') -> int | None:
     """
     Type choices list and request choice position from user.\n
     In case incorrect choice position - clear output and start again.\n
     :param choices: list: list of choices (filenames for example)
-    :param axe: str: 'v'(default) - vertical or 'h' - horizontal data print mode
-    :return: int: choice position in the list or Null if empty / wrong user input
+    :param axe: str: 'v'(default) - vertical or 'h' - horizontal \
+    data print mode
+    :return: int: choice position in the list or Null if empty / \
+    wrong user input
     """
     logger.disable(__name__)
     choices = choices.copy()
     choices.append('Exit')
     index_range = range(len(choices))
     choice_position = max_index = last_index(choices)
 
     while choice_position in index_range:
         print("Select choices:")
         show_choices(choices, axe)
-        choice_position = input(f"\nEnter choice position < from 0 to {max_index} >, "
-                                f"empty input for quit:")
+        choice_position = input(f"\nEnter choice position < from 0 to "
+                                f"{max_index} >, empty input for quit:")
         logger.debug(f"{choice_position=}")
         if choice_position == '' or choice_position == str(max_index):
             choice_position = None
             break
         try:
             choice_position = int(choice_position)
         except ValueError:
@@ -181,29 +183,30 @@
         create_date = datetime.fromtimestamp(f_name.stat().st_mtime)
         files_info.append({"name": filename, "date": create_date})
 
     names = [note['name'] for note in files_info]
     dates = [note['date'] for note in files_info]
     if mask_by == 'recently':
         recently = max(dates)
-        recent_filename = [name for name, date in zip(names, dates) if date == recently]
+        recent_filename = [name for name, date in zip(names, dates)
+                           if date == recently]
         ordered_filename = recent_filename
 
     return files_info, ordered_filename
 
 
 def edit_df_row(original_df: pandas.DataFrame,
-                row_arg = EMPTY_STR) -> Tuple[pandas.DataFrame, int]:
+                row_arg: str = EMPTY_STR) -> tuple[pandas.DataFrame, int]:
     """
     Maybe need atomizing (too large)?
     TODO Fill function description text
     TODO: Though about using get_choice_position() here
     :param original_df: pandas.DataFrame - source Pandas DataFrame
     :param row_arg: str - user`s input
-    :return: Tuple[pandas.DataFrame, int] - result (DataFrame, edited row index)
+    :return: tuple[pandas.DataFrame, int] - result (DataFrame, edited row index)
     """
     edited_df = original_df.copy()
     row_arg = str(row_arg)
     editing_row_index = None
     while row_arg.lower() != 'exit':
         if row_arg == EMPTY_STR or not digit_only(row_arg):
             row_arg = input('\n' + '[?] Enter index row to edit (integer):')
@@ -253,17 +256,18 @@
         raise
     function_result = md5(data_for_md5).hexdigest()
     logger.debug(f"{args=}" + 'n' + f"{function_result}")
 
     return function_result
 
 
-def chosen_filename(file_mask: str = '*.*') -> Union[str, None]:
+def chosen_filename(file_mask: str = '*.*') -> str | None:
     """
-    Request user and return name of chosen file or None in case empty or last point user input
+    Request user and return name of chosen file or None in case empty \
+    or last point user input
 
     :param file_mask:
     :return: str: filename [!] ONLY. \
     Without previously parts of path ([any/.../]filename) or None when Exit
     """
     ls_list = get_file_name(file_mask)[0]
     files_list = [note['name'] for note in ls_list]
```

### Comparing `ownlib-0.0.1a4/src/ownlib/one_s_uat_lib.py` & `ownlib-0.0.1b4/src/ownlib/one_s_uat_lib.py`

 * *Files identical despite different names*

### Comparing `ownlib-0.0.1a4/src/ownlib/txt_lib.py` & `ownlib-0.0.1b4/src/ownlib/txt_lib.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """
 Short useful text functions library
 """
 import re
-from typing import Union
+from typing import (Optional,
+                    Union
+                    )
 from loguru import logger
 
 from ownlib.months import months_df
 
 SPACE_CHAR: str = ' '
 TAB_CHAR = '\t'
 NEW_LINE = '\n'
@@ -14,39 +16,42 @@
 
 complete_rules = {'\xa0': EMPTY_STR,
                   '\n': SPACE_CHAR
                   }
 # noAutoStringLength = 10
 
 
-def nominative_month(month_mame: str) -> str:
+def nominative_month(month_mame: str) -> str | None:
     """
     TODO Add some description
     """
     return (month_mame[:-1] + 'й' if month_mame.lower() == 'мая'
             else month_mame[:-1] + 'ь' if month_mame[-1:] == 'я'
             else month_mame[:-1] if month_mame[-1:] == 'а'
-            else -1
+            else None
             )
 
 
-def translated_month(month: str) -> Union[str, None]:
+def translated_month(month: str) -> str | None:
     """
     TODO Add some description
     """
-    # TODO make mirroring language functionality (ru->lat, lat->ru) (?) auto lang recognition
+    # TODO make mirroring language functionality (ru->lat, lat->ru) \
+    #  (?) auto lang recognition
     try:
-        translated = months_df[months_df['russian'] == month]['english'].values[0]
-    except IndexError:
+        translated = months_df[months_df['russian']
+                               == month]['english'].values[0]
+    except IndexError as ie_ex:
         logger.exception('Wrong argument: ', month)
-        translated = None
+        raise ie_ex
+
     return translated
 
 
-def get_month_number(month: str) -> Union[int, None]:
+def get_month_number(month: str) -> int | None:
     """
     TODO Add some description
     """
     try:
         month_number = months_df[months_df['english'] == month]['number'].values[0]
     except IndexError:
         logger.exception('Wrong argument: ', month)
@@ -106,73 +111,84 @@
 
 
 def get_month(month_field: str) -> str:
     """
     TODO Add some description
     """
     if cyrillic_only(month_field):
+        # FIXME Понять как обрабатывать ошибку аргумента
         month_field = nominative_month(month_field).title()
         month_field = translated_month(month_field)
     elif not lat_only(month_field):
         month_field = 'MonthParsingError'
-    else:
-        pass
+
     return month_field
 
 
-def string_transform(manipulated_string: str, change_rules=None):
+def string_transform(manipulated_string: str,
+                     rules: dict[str, str] | None = None) -> str | None:
     """Change change_rules.key => change_rules.value in manipulated_string
 
     :param manipulated_string: str - source string on which we could change a symbols
-    :param change_rules: dict - {symbol_from_change : symbol_to_change}
+    :param rules: dict - {symbol_from_change : symbol_to_change}
     :return: result string: str
     Example rules: rules = {'\xa0' : EMPTY_STR\n' : ' '}
     """
-    if change_rules is None:
-        change_rules = {'\xa0': EMPTY_STR}
-    for ch_from in change_rules.keys():
-        try:
-            manipulated_string = manipulated_string.replace(ch_from, change_rules[ch_from])
-        except IndexError:
-            logger.exception(f"[!] Unknown error in manipulation with {manipulated_string=}, "
-                         f"{change_rules=}")
+    result_string = ''
+    rules = rules if rules else {'\xa0': EMPTY_STR}
 
-    return manipulated_string
+    for char in manipulated_string:
+        result_string += rules[char] \
+            if char in rules else char
+    return result_string
 
 
-def list_transform(manipulated_list: str, change_rules=None):
+def list_transform(manipulated_list: list[str],
+                   change_rules: Optional[dict[str, str]] = None):
     """
     Change change_rules.key => change_rules.value in manipulated_list
     
     :param manipulated_list: list - source list on which we could change a symbols
     :param change_rules: dict - {symbol_from_change : symbol_to_change} \
     Example: {'\xa0':'', '\n':' '}
     :return: result list: list
     """
+    # TODO Though about union both of this functions ^
     if change_rules is None:
         change_rules = {'\xa0': EMPTY_STR}
     return [string_transform(string, change_rules) for string in manipulated_list]
 
 
-def txt2float(arg: str) -> float:
+def txt2float(arg: str) -> float | None:
     """
     Convert  str -> float. Change ',' -> '.', '\xa0' -> ''
     
     :param arg: str - string via digits
     :return: float(arg)
     """
     arg = arg.replace(',', '.')
     arg = arg.replace("\xa0", EMPTY_STR)
-    arg = float(arg)
-    return arg
 
+    try:
+        float_arg = float(arg)
+    except ValueError:
+        logger.exception('Wrong argument format', arg)
+        float_arg = None
+
+    return float_arg
 
-def items_in_string(analysing_string: str, parent_list: list) -> list:
+
+def items_in_string(analysing_string: str,
+                    parent_list: list[str]) -> list[str]:
     """
-    Return the ordered list of words from analysing string, which have equals in the predefined list
+    Return the ordered list of words from analysing string,
+    which have equals in the predefined list
 
     :param analysing_string: str - Analysing string
-    :param parent_list: list - Predefined list
-    :return: list - An ordered list of words equals the same ones in parent_list
-    """
-    return [item[0] for item in [[value for value in parent_list if value == word]
-                                 for word in analysing_string.split()] if item]
+    :param parent_list: list[str] - Predefined list
+    :return: list[str] - An ordered list of words equals the same
+    ones in parent_list
+    """
+    return [item[0] for item in [[value for value in parent_list
+                                  if value == word]
+                                 for word in analysing_string.split()]
+            if item]
```

### Comparing `ownlib-0.0.1a4/src/ownlib/whapp_funcs.py` & `ownlib-0.0.1b4/src/ownlib/whapp_funcs.py`

 * *Files identical despite different names*

### Comparing `ownlib-0.0.1a4/PKG-INFO` & `ownlib-0.0.1b4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: ownlib
-Version: 0.0.1a4
+Version: 0.0.1b4
 Summary: Sample pypi project
 License: GNU
 Author: Андрей Мартынов
 Author-email: real.cloudhunter@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: ipython (>=8.22.1,<9.0.0)
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
 Requires-Dist: pandas (>=2.2.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # ownlib
 My own code
```

