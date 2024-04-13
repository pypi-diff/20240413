# Comparing `tmp/reset-tolkien-1.0.0.tar.gz` & `tmp/reset-tolkien-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reset-tolkien-1.0.0.tar", last modified: Fri Mar 29 17:02:15 2024, max compression
+gzip compressed data, was "reset-tolkien-1.1.0.tar", last modified: Sat Apr 13 07:59:38 2024, max compression
```

## Comparing `reset-tolkien-1.0.0.tar` & `reset-tolkien-1.1.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 aethlios  (1000) aethlios  (1000)        0 2024-03-29 17:02:15.346255 reset-tolkien-1.0.0/
--rw-r--r--   0 aethlios  (1000) aethlios  (1000)     1073 2024-03-29 16:44:20.000000 reset-tolkien-1.0.0/LICENSE
--rw-r--r--   0 aethlios  (1000) aethlios  (1000)    16208 2024-03-29 17:02:15.342255 reset-tolkien-1.0.0/PKG-INFO
--rw-r--r--   0 aethlios  (1000) aethlios  (1000)    13057 2024-03-29 17:00:18.000000 reset-tolkien-1.0.0/README.md
--rw-r--r--   0 aethlios  (1000) aethlios  (1000)     2004 2024-03-29 16:44:09.000000 reset-tolkien-1.0.0/pyproject.toml
--rw-r--r--   0 aethlios  (1000) aethlios  (1000)       38 2024-03-29 17:02:15.346255 reset-tolkien-1.0.0/setup.cfg
--rw-r--r--   0 aethlios  (1000) aethlios  (1000)       37 2024-03-29 16:43:47.000000 reset-tolkien-1.0.0/setup.py
-drwxr-xr-x   0 aethlios  (1000) aethlios  (1000)        0 2024-03-29 17:02:15.334255 reset-tolkien-1.0.0/src/
-drwxr-xr-x   0 aethlios  (1000) aethlios  (1000)        0 2024-03-29 17:02:15.338255 reset-tolkien-1.0.0/src/resetTolkien/
--rw-r--r--   0 aethlios  (1000) aethlios  (1000)      220 2024-03-29 16:43:15.000000 reset-tolkien-1.0.0/src/resetTolkien/__init__.py
--rw-r--r--   0 aethlios  (1000) aethlios  (1000)       72 2024-03-29 16:43:15.000000 reset-tolkien-1.0.0/src/resetTolkien/__main__.py
--rw-r--r--   0 aethlios  (1000) aethlios  (1000)    13573 2024-03-29 16:43:15.000000 reset-tolkien-1.0.0/src/resetTolkien/cli.py
--rw-r--r--   0 aethlios  (1000) aethlios  (1000)     2252 2024-03-29 16:43:15.000000 reset-tolkien-1.0.0/src/resetTolkien/constants.py
--rw-r--r--   0 aethlios  (1000) aethlios  (1000)    23876 2024-03-29 16:43:15.000000 reset-tolkien-1.0.0/src/resetTolkien/format.py
--rw-r--r--   0 aethlios  (1000) aethlios  (1000)     1525 2024-03-29 16:43:15.000000 reset-tolkien-1.0.0/src/resetTolkien/hashes.py
--rw-r--r--   0 aethlios  (1000) aethlios  (1000)    15955 2024-03-29 16:43:15.000000 reset-tolkien-1.0.0/src/resetTolkien/resetTolkien.py
--rw-r--r--   0 aethlios  (1000) aethlios  (1000)    15513 2024-03-29 16:43:15.000000 reset-tolkien-1.0.0/src/resetTolkien/utils.py
-drwxr-xr-x   0 aethlios  (1000) aethlios  (1000)        0 2024-03-29 17:02:15.342255 reset-tolkien-1.0.0/src/reset_tolkien.egg-info/
--rw-r--r--   0 aethlios  (1000) aethlios  (1000)    16208 2024-03-29 17:02:15.000000 reset-tolkien-1.0.0/src/reset_tolkien.egg-info/PKG-INFO
--rw-r--r--   0 aethlios  (1000) aethlios  (1000)      537 2024-03-29 17:02:15.000000 reset-tolkien-1.0.0/src/reset_tolkien.egg-info/SOURCES.txt
--rw-r--r--   0 aethlios  (1000) aethlios  (1000)        1 2024-03-29 17:02:15.000000 reset-tolkien-1.0.0/src/reset_tolkien.egg-info/dependency_links.txt
--rw-r--r--   0 aethlios  (1000) aethlios  (1000)       52 2024-03-29 17:02:15.000000 reset-tolkien-1.0.0/src/reset_tolkien.egg-info/entry_points.txt
--rw-r--r--   0 aethlios  (1000) aethlios  (1000)      249 2024-03-29 17:02:15.000000 reset-tolkien-1.0.0/src/reset_tolkien.egg-info/requires.txt
--rw-r--r--   0 aethlios  (1000) aethlios  (1000)       22 2024-03-29 17:02:15.000000 reset-tolkien-1.0.0/src/reset_tolkien.egg-info/top_level.txt
--rw-r--r--   0 aethlios  (1000) aethlios  (1000)       72 2024-03-29 16:56:55.000000 reset-tolkien-1.0.0/src/run.py
--rw-r--r--   0 aethlios  (1000) aethlios  (1000)    15201 2024-03-29 16:54:13.000000 reset-tolkien-1.0.0/src/test.py
+drwxr-xr-x   0 aethlios  (1000) aethlios  (1000)        0 2024-04-13 07:59:38.939850 reset-tolkien-1.1.0/
+-rw-r--r--   0 aethlios  (1000) aethlios  (1000)     1073 2024-03-29 16:44:20.000000 reset-tolkien-1.1.0/LICENSE
+-rw-r--r--   0 aethlios  (1000) aethlios  (1000)    16830 2024-04-13 07:59:38.939850 reset-tolkien-1.1.0/PKG-INFO
+-rw-r--r--   0 aethlios  (1000) aethlios  (1000)    13517 2024-04-06 18:13:01.000000 reset-tolkien-1.1.0/README.md
+-rw-r--r--   0 aethlios  (1000) aethlios  (1000)     2146 2024-04-13 07:53:32.000000 reset-tolkien-1.1.0/pyproject.toml
+-rw-r--r--   0 aethlios  (1000) aethlios  (1000)       38 2024-04-13 07:59:38.939850 reset-tolkien-1.1.0/setup.cfg
+-rw-r--r--   0 aethlios  (1000) aethlios  (1000)       37 2024-03-29 16:43:47.000000 reset-tolkien-1.1.0/setup.py
+drwxr-xr-x   0 aethlios  (1000) aethlios  (1000)        0 2024-04-13 07:59:38.927849 reset-tolkien-1.1.0/src/
+drwxr-xr-x   0 aethlios  (1000) aethlios  (1000)        0 2024-04-13 07:59:38.935850 reset-tolkien-1.1.0/src/resetTolkien/
+-rw-r--r--   0 aethlios  (1000) aethlios  (1000)      221 2024-04-06 17:47:14.000000 reset-tolkien-1.1.0/src/resetTolkien/__init__.py
+-rw-r--r--   0 aethlios  (1000) aethlios  (1000)       72 2024-03-29 16:43:15.000000 reset-tolkien-1.1.0/src/resetTolkien/__main__.py
+-rw-r--r--   0 aethlios  (1000) aethlios  (1000)    13573 2024-03-29 16:43:15.000000 reset-tolkien-1.1.0/src/resetTolkien/cli.py
+-rw-r--r--   0 aethlios  (1000) aethlios  (1000)     2278 2024-04-03 09:36:23.000000 reset-tolkien-1.1.0/src/resetTolkien/constants.py
+-rw-r--r--   0 aethlios  (1000) aethlios  (1000)    24743 2024-04-06 17:16:56.000000 reset-tolkien-1.1.0/src/resetTolkien/format.py
+-rw-r--r--   0 aethlios  (1000) aethlios  (1000)     1525 2024-03-29 16:43:15.000000 reset-tolkien-1.1.0/src/resetTolkien/hashes.py
+-rw-r--r--   0 aethlios  (1000) aethlios  (1000)    16200 2024-04-06 17:16:18.000000 reset-tolkien-1.1.0/src/resetTolkien/resetTolkien.py
+-rw-r--r--   0 aethlios  (1000) aethlios  (1000)    15513 2024-04-03 09:23:27.000000 reset-tolkien-1.1.0/src/resetTolkien/utils.py
+drwxr-xr-x   0 aethlios  (1000) aethlios  (1000)        0 2024-04-13 07:59:38.939850 reset-tolkien-1.1.0/src/reset_tolkien.egg-info/
+-rw-r--r--   0 aethlios  (1000) aethlios  (1000)    16830 2024-04-13 07:59:38.000000 reset-tolkien-1.1.0/src/reset_tolkien.egg-info/PKG-INFO
+-rw-r--r--   0 aethlios  (1000) aethlios  (1000)      537 2024-04-13 07:59:38.000000 reset-tolkien-1.1.0/src/reset_tolkien.egg-info/SOURCES.txt
+-rw-r--r--   0 aethlios  (1000) aethlios  (1000)        1 2024-04-13 07:59:38.000000 reset-tolkien-1.1.0/src/reset_tolkien.egg-info/dependency_links.txt
+-rw-r--r--   0 aethlios  (1000) aethlios  (1000)       52 2024-04-13 07:59:38.000000 reset-tolkien-1.1.0/src/reset_tolkien.egg-info/entry_points.txt
+-rw-r--r--   0 aethlios  (1000) aethlios  (1000)      249 2024-04-13 07:59:38.000000 reset-tolkien-1.1.0/src/reset_tolkien.egg-info/requires.txt
+-rw-r--r--   0 aethlios  (1000) aethlios  (1000)       22 2024-04-13 07:59:38.000000 reset-tolkien-1.1.0/src/reset_tolkien.egg-info/top_level.txt
+-rw-r--r--   0 aethlios  (1000) aethlios  (1000)       72 2024-03-29 16:56:55.000000 reset-tolkien-1.1.0/src/run.py
+-rw-r--r--   0 aethlios  (1000) aethlios  (1000)    15201 2024-03-29 16:54:13.000000 reset-tolkien-1.1.0/src/test.py
```

### Comparing `reset-tolkien-1.0.0/LICENSE` & `reset-tolkien-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `reset-tolkien-1.0.0/PKG-INFO` & `reset-tolkien-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reset-tolkien
-Version: 1.0.0
+Version: 1.1.0
 Summary: Unsecure time-based secret exploitation and Sandwich attack implementation.
 Author-email: Tom CHAMBARETAUD <tom.chambaretaud@protonmail.com>
 Maintainer-email: Tom CHAMBARETAUD <tom.chambaretaud@protonmail.com>
 License: MIT License
         
         Copyright (c) 2024 Tom Chambaretaud
         
@@ -22,16 +22,18 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: Repository, https://github.com/AethliosIK/resetTolkien
-Project-URL: Issues, https://github.com/AethliosIK/resetTolkien/issues
+Project-URL: Homepage, https://github.com/AethliosIK/reset-tolkien
+Project-URL: Repository, https://github.com/AethliosIK/reset-tolkien
+Project-URL: Issues, https://github.com/AethliosIK/reset-tolkien/issues
+Project-URL: Changelog, https://github.com/AethliosIK/reset-tolkien/blob/master/CHANGELOG.md
 Keywords: security,secret,reset,token,tolkien
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -85,14 +87,23 @@
 
 Install from [pip](https://pypi.org/project/reset-tolkien/):
 
 ```
 ▶ pip install reset-tolkien
 ```
 
+## Installation from Docker
+
+```
+▶ git clone https://github.com/AethliosIK/reset-tolkien.git
+▶ cd reset-tolkien
+▶ docker build -t reset-tolkien:latest . 
+▶ docker run --rm -it --net=host -v "$PWD:/reset-tolkien/" reset-tolkien:latest -h
+```
+
 ## Usage
 
 To detect whether a token is time-based, simply use this command:
 
 ```bash
 $ reset-tolkien detect 660430516ffcf -d "Wed, 27 Mar 2024 14:42:25 GMT" --prefixes "attacker@example.com" --suffixes "attacker@example.com" --timezone "-7"
 The token may be based on a timestamp: 1711550545.458703 (prefix: None / suffix: None)
@@ -332,11 +343,18 @@
 
 Among the points that would be very useful:
 - **Format management via [Abstract syntax tree](https://docs.python.org/3/library/ast.html)**: the tool currently only manages formats applied in a linear way, so a simple format like `md5(timestamp()+1)` won't be supported. By configuring formats as a tree, this type of format can be supported by the tool.
 - **Better application of user-specific information**: when detecting a token format, it is possible to define user-specific information as prefixes or suffixes of the token generation date. Many other configurations could be possible.
 - **Management of other dynamic variables**: the tool detects formats and allows attacks based on the only variable supported: time. However, some formats can have several variables that evolve.
 - **Addition of new supported formats**: the tool only supports the time-based functions found during my research, but many other formats should still exist and could also be supported by the tool.
 
+## Changelog
+
+You could retrieve changes for each version from [CHANGELOG.md](CHANGELOG.md).
 
 ## Licensing
 
 This project is licensed under the [MIT license](LICENSE).
+
+## Credit
+
+- Main illustration: service provided by [@valentin.froute](https://www.instagram.com/valentin.froute/).
```

### Comparing `reset-tolkien-1.0.0/README.md` & `reset-tolkien-1.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,23 @@
 
 Install from [pip](https://pypi.org/project/reset-tolkien/):
 
 ```
 ▶ pip install reset-tolkien
 ```
 
+## Installation from Docker
+
+```
+▶ git clone https://github.com/AethliosIK/reset-tolkien.git
+▶ cd reset-tolkien
+▶ docker build -t reset-tolkien:latest . 
+▶ docker run --rm -it --net=host -v "$PWD:/reset-tolkien/" reset-tolkien:latest -h
+```
+
 ## Usage
 
 To detect whether a token is time-based, simply use this command:
 
 ```bash
 $ reset-tolkien detect 660430516ffcf -d "Wed, 27 Mar 2024 14:42:25 GMT" --prefixes "attacker@example.com" --suffixes "attacker@example.com" --timezone "-7"
 The token may be based on a timestamp: 1711550545.458703 (prefix: None / suffix: None)
@@ -264,11 +273,18 @@
 
 Among the points that would be very useful:
 - **Format management via [Abstract syntax tree](https://docs.python.org/3/library/ast.html)**: the tool currently only manages formats applied in a linear way, so a simple format like `md5(timestamp()+1)` won't be supported. By configuring formats as a tree, this type of format can be supported by the tool.
 - **Better application of user-specific information**: when detecting a token format, it is possible to define user-specific information as prefixes or suffixes of the token generation date. Many other configurations could be possible.
 - **Management of other dynamic variables**: the tool detects formats and allows attacks based on the only variable supported: time. However, some formats can have several variables that evolve.
 - **Addition of new supported formats**: the tool only supports the time-based functions found during my research, but many other formats should still exist and could also be supported by the tool.
 
+## Changelog
+
+You could retrieve changes for each version from [CHANGELOG.md](CHANGELOG.md).
 
 ## Licensing
 
 This project is licensed under the [MIT license](LICENSE).
+
+## Credit
+
+- Main illustration: service provided by [@valentin.froute](https://www.instagram.com/valentin.froute/).
```

### Comparing `reset-tolkien-1.0.0/pyproject.toml` & `reset-tolkien-1.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -47,16 +47,18 @@
     "shortuuid == 1.0.11",
     "six == 1.16.0",
     "typing_extensions == 4.10.0",
     "tzlocal == 5.2",
 ]
 
 [project.urls]
-Repository = "https://github.com/AethliosIK/resetTolkien"
-Issues = "https://github.com/AethliosIK/resetTolkien/issues"
+Homepage = "https://github.com/AethliosIK/reset-tolkien"
+Repository = "https://github.com/AethliosIK/reset-tolkien"
+Issues = "https://github.com/AethliosIK/reset-tolkien/issues"
+Changelog = "https://github.com/AethliosIK/reset-tolkien/blob/master/CHANGELOG.md"
 
 [tool.setuptools.dynamic]
 version = {attr = "resetTolkien.__version__"}
 
 [project.optional-dependencies]
 dev = [
     "setuptools == 68.2.0",
```

### Comparing `reset-tolkien-1.0.0/src/resetTolkien/cli.py` & `reset-tolkien-1.1.0/src/resetTolkien/cli.py`

 * *Files identical despite different names*

### Comparing `reset-tolkien-1.0.0/src/resetTolkien/constants.py` & `reset-tolkien-1.1.0/src/resetTolkien/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     },
 }
 
 PROG_DESCRIPTION = "Reset Tolkien can be used to find out whether a provided token is based on a timestamp, from a timestamp corresponding to the period in which it was generated."
 
 NB_DAYS_LIMIT = 365 * 1
 TIMESTAMP_HEX_LENGTH = 8
+TIMESTAMP_STR_LENGTH = 10
 DEFAULT_DECIMAL_LENGTH = 7
 UUID_DECIMAL_LENGTH = 7
 DEFAULT_TIMERANGE_FOR_INT_TIMESTAMP = 60
 DEFAULT_TIMERANGE_FOR_FLOAT_TIMESTAMP = 2
 MIN_LENGTH_OF_FLOATING_TIMESTAMP_HEX = 8
 MAX_LENGTH_OF_FLOATING_TIMESTAMP_HEX = 13
```

### Comparing `reset-tolkien-1.0.0/src/resetTolkien/format.py` & `reset-tolkien-1.1.0/src/resetTolkien/format.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 from resetTolkien.constants import (
     DEFAULT_THREAD_NUMBER,
     DATE_SLASH_REGEX,
     DATE_DASH_REGEX,
     TIME_REGEX,
     MONTH_REGEX,
     PARTIAL_FUNC_NAME_REGEX,
+    TIMESTAMP_STR_LENGTH,
 )
 from resetTolkien.hashes import Hashes
 
 
 class Formatter:
     """Class for encoding, hashing and decrypting a timestamp-based value"""
 
@@ -97,17 +98,40 @@
             return True
         except (ValueError, OverflowError, TypeError):
             return False
 
     def getNumbers(self, token: str) -> list[str]:
         """Extracts numeric values from the string value."""
 
-        matches = re.findall(r"(\d+)", str(token))
+        matches = re.findall(r"([0-9]+\.?[0-9]*)", str(token))
         return [match for match in matches if self.isLiteralIntegerOrFloat(match)]
 
+    def searchTimestamps(self, numbers: list[str]) -> list[float]:
+        """Extracts nearby timestamp values from numerical values."""
+
+        matches: list[float] = []
+        for number in numbers:
+            if self.isLiteralIntegerOrFloat(number):
+                if "." in number:
+                    n = float(number)
+                elif len(number) > TIMESTAMP_STR_LENGTH:
+                    n = float(
+                        number[:TIMESTAMP_STR_LENGTH]
+                        + "."
+                        + number[TIMESTAMP_STR_LENGTH:]
+                    )
+                else:
+                    n = int(number)
+                try:
+                    from_microsecond_timestamp(n)
+                except ValueError:
+                    continue
+                matches.append(n)
+        return matches
+
     def isDatetime(self, token: str) -> bool:
         """Confirms that the value is datetime format."""
 
         return (
             re.search(DATE_SLASH_REGEX, token) != None
             or re.search(DATE_DASH_REGEX, token) != None
             or re.search(TIME_REGEX, token) != None
```

### Comparing `reset-tolkien-1.0.0/src/resetTolkien/hashes.py` & `reset-tolkien-1.1.0/src/resetTolkien/hashes.py`

 * *Files identical despite different names*

### Comparing `reset-tolkien-1.0.0/src/resetTolkien/resetTolkien.py` & `reset-tolkien-1.1.0/src/resetTolkien/resetTolkien.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     NotAHash,
     GeneratorLen,
     AlternativeGen,
     TimestampGenerator,
     TimestampHashFormat,
     import_from_yaml,
     possible_date_format_of_token,
-    CustomFloat
+    CustomFloat,
 )
 from resetTolkien.constants import (
     DEFAULT_TIMERANGE_FOR_INT_TIMESTAMP,
     DEFAULT_TIMERANGE_FOR_FLOAT_TIMESTAMP,
     MAX_DEPTH_LEVEL,
     DEFAULT_THREAD_NUMBER,
     DEFAULT_CONFIG_FILE,
@@ -48,17 +48,15 @@
         formats: Optional[list[str]] = None,
     ) -> None:
         """Initialization function of ResetTolkien."""
 
         self.formatter = Formatter()
         self.token = token
         self.decimal_length = (
-            decimal_length
-            if decimal_length
-            else DEFAULT_DECIMAL_LENGTH
+            decimal_length if decimal_length else DEFAULT_DECIMAL_LENGTH
         )
         self.int_range_limit = (
             int_range_limit * 2
             if int_range_limit
             else DEFAULT_TIMERANGE_FOR_INT_TIMESTAMP * 2
         )
         self.float_range_limit = (
@@ -216,17 +214,20 @@
         timestamp: Optional[float] = None,
     ) -> list[tuple[tuple[str, Optional[str], Optional[str]], list[FormatType], bool]]:
         """Recursive function - Determines a function
         corresponding to the format of an input token."""
 
         formats = [] if formats is None else formats
 
-        if self.verbosity >= 1:
-            numbers = self.formatter.getNumbers(token)
+        numbers = self.formatter.getNumbers(token)
+        if self.verbosity >= 1 and len(numbers) > 0:
             print(f"Integer value detected : {numbers}")
+        possibleTimestamp = self.formatter.searchTimestamps(numbers)
+        if len(possibleTimestamp) > 0:
+            print(f"Possible timestamp detected! {possibleTimestamp} from \"{token}\"")
 
         if self.formatter.isLiteralIntegerOrFloat(token):
             new_token, _ = self.detectOneEncoding(token, self.formatter.timestamp)
             if new_token:
                 if self.verbosity >= 1:
                     print(
                         f"Format detected and stored : {self.formatter.export_formats(formats)}"
@@ -286,15 +287,17 @@
             hashes = self.formatter.availableHashingDict(token)
             if len(hashes) > 0:
                 if self.verbosity >= 1:
                     print(f"Hash format detected : {list(hashes.keys())} : {token}")
 
                 if token.lower() != token:
                     if self.verbosity >= 1:
-                        print(f"Hash with uppercase detected : {token} -> {token.lower()}")
+                        print(
+                            f"Hash with uppercase detected : {token} -> {token.lower()}"
+                        )
                     token = token.lower()
 
                 for timestampFormat in self.timestamp_hash_formats:
                     if self.verbosity >= 1:
                         print(
                             f"Check hash with {timestampFormat.description} ({timestampFormat.range_limit} tokens)"
                         )
@@ -367,15 +370,15 @@
         if isinstance(init, int):
             if not range_limit:
                 range_limit = self.int_range_limit
         else:
             if not range_limit:
                 range_limit = self.float_range_limit
 
-        for i in AlternativeGen(range_limit): # type: ignore
+        for i in AlternativeGen(range_limit):  # type: ignore
             timestamp = str(init + i)
             if not isinstance(init, int):
                 t = CustomFloat(init, self.decimal_length)
                 t.value = t.value + i
                 timestamp = str(t)
             if prefix:
                 timestamp = f"{prefix}{timestamp}"
```

### Comparing `reset-tolkien-1.0.0/src/resetTolkien/utils.py` & `reset-tolkien-1.1.0/src/resetTolkien/utils.py`

 * *Files identical despite different names*

### Comparing `reset-tolkien-1.0.0/src/reset_tolkien.egg-info/PKG-INFO` & `reset-tolkien-1.1.0/src/reset_tolkien.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reset-tolkien
-Version: 1.0.0
+Version: 1.1.0
 Summary: Unsecure time-based secret exploitation and Sandwich attack implementation.
 Author-email: Tom CHAMBARETAUD <tom.chambaretaud@protonmail.com>
 Maintainer-email: Tom CHAMBARETAUD <tom.chambaretaud@protonmail.com>
 License: MIT License
         
         Copyright (c) 2024 Tom Chambaretaud
         
@@ -22,16 +22,18 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: Repository, https://github.com/AethliosIK/resetTolkien
-Project-URL: Issues, https://github.com/AethliosIK/resetTolkien/issues
+Project-URL: Homepage, https://github.com/AethliosIK/reset-tolkien
+Project-URL: Repository, https://github.com/AethliosIK/reset-tolkien
+Project-URL: Issues, https://github.com/AethliosIK/reset-tolkien/issues
+Project-URL: Changelog, https://github.com/AethliosIK/reset-tolkien/blob/master/CHANGELOG.md
 Keywords: security,secret,reset,token,tolkien
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -85,14 +87,23 @@
 
 Install from [pip](https://pypi.org/project/reset-tolkien/):
 
 ```
 ▶ pip install reset-tolkien
 ```
 
+## Installation from Docker
+
+```
+▶ git clone https://github.com/AethliosIK/reset-tolkien.git
+▶ cd reset-tolkien
+▶ docker build -t reset-tolkien:latest . 
+▶ docker run --rm -it --net=host -v "$PWD:/reset-tolkien/" reset-tolkien:latest -h
+```
+
 ## Usage
 
 To detect whether a token is time-based, simply use this command:
 
 ```bash
 $ reset-tolkien detect 660430516ffcf -d "Wed, 27 Mar 2024 14:42:25 GMT" --prefixes "attacker@example.com" --suffixes "attacker@example.com" --timezone "-7"
 The token may be based on a timestamp: 1711550545.458703 (prefix: None / suffix: None)
@@ -332,11 +343,18 @@
 
 Among the points that would be very useful:
 - **Format management via [Abstract syntax tree](https://docs.python.org/3/library/ast.html)**: the tool currently only manages formats applied in a linear way, so a simple format like `md5(timestamp()+1)` won't be supported. By configuring formats as a tree, this type of format can be supported by the tool.
 - **Better application of user-specific information**: when detecting a token format, it is possible to define user-specific information as prefixes or suffixes of the token generation date. Many other configurations could be possible.
 - **Management of other dynamic variables**: the tool detects formats and allows attacks based on the only variable supported: time. However, some formats can have several variables that evolve.
 - **Addition of new supported formats**: the tool only supports the time-based functions found during my research, but many other formats should still exist and could also be supported by the tool.
 
+## Changelog
+
+You could retrieve changes for each version from [CHANGELOG.md](CHANGELOG.md).
 
 ## Licensing
 
 This project is licensed under the [MIT license](LICENSE).
+
+## Credit
+
+- Main illustration: service provided by [@valentin.froute](https://www.instagram.com/valentin.froute/).
```

### Comparing `reset-tolkien-1.0.0/src/reset_tolkien.egg-info/SOURCES.txt` & `reset-tolkien-1.1.0/src/reset_tolkien.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reset-tolkien-1.0.0/src/test.py` & `reset-tolkien-1.1.0/src/test.py`

 * *Files identical despite different names*

