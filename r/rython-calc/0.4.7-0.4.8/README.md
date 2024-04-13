# Comparing `tmp/rython_calc-0.4.7.tar.gz` & `tmp/rython_calc-0.4.8.tar.gz`

## Comparing `rython_calc-0.4.7.tar` & `rython_calc-0.4.8.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0      290 1970-01-01 00:00:00.000000 rython_calc-0.4.7/Cargo.toml
--rw-r--r--   0     1001      127      367 2024-04-07 13:39:04.000000 rython_calc-0.4.7/.github/dependabot.yml
--rw-r--r--   0     1001      127     4975 2024-04-07 13:39:04.000000 rython_calc-0.4.7/.github/workflows/CI.yml
--rw-r--r--   0     1001      127      686 2024-04-07 13:39:04.000000 rython_calc-0.4.7/.gitignore
--rw-r--r--   0     1001      127     1075 2024-04-07 13:39:04.000000 rython_calc-0.4.7/LICENSE
--rw-r--r--   0     1001      127      603 2024-04-07 13:39:04.000000 rython_calc-0.4.7/README.md
--rw-r--r--   0     1001      127    10298 2024-04-07 13:39:04.000000 rython_calc-0.4.7/poetry.lock
--rw-r--r--   0     1001      127        0 2024-04-07 13:39:04.000000 rython_calc-0.4.7/python/cli/__init__.py
--rw-r--r--   0     1001      127     1743 2024-04-07 13:39:04.000000 rython_calc-0.4.7/python/cli/main.py
--rw-r--r--   0     1001      127      443 2024-04-07 13:39:04.000000 rython_calc-0.4.7/python/cli/performance.txt
--rw-r--r--   0     1001      127        0 2024-04-07 13:39:04.000000 rython_calc-0.4.7/python/rython/__init__.py
--rw-r--r--   0     1001      127        0 2024-04-07 13:39:04.000000 rython_calc-0.4.7/python/rython/py.typed
--rw-r--r--   0     1001      127      666 2024-04-07 13:39:04.000000 rython_calc-0.4.7/python/rython/rython_calc.pyi
--rw-r--r--   0     1001      127     3030 2024-04-07 13:39:04.000000 rython_calc-0.4.7/src/lib.rs
--rw-r--r--   0     1001      127      347 2024-04-07 13:39:04.000000 rython_calc-0.4.7/test/rython/test_rython_calc.py
--rw-r--r--   0     1001      127     7857 2024-04-07 13:39:04.000000 rython_calc-0.4.7/Cargo.lock
--rw-r--r--   0     1001      127     1595 2024-04-07 13:39:04.000000 rython_calc-0.4.7/pyproject.toml
--rw-r--r--   0        0        0     1263 1970-01-01 00:00:00.000000 rython_calc-0.4.7/PKG-INFO
+-rw-r--r--   0        0        0      359 1970-01-01 00:00:00.000000 rython_calc-0.4.8/Cargo.toml
+-rw-r--r--   0     1001      127      367 2024-04-13 16:13:25.000000 rython_calc-0.4.8/.github/dependabot.yml
+-rw-r--r--   0     1001      127     4975 2024-04-13 16:13:25.000000 rython_calc-0.4.8/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127      686 2024-04-13 16:13:25.000000 rython_calc-0.4.8/.gitignore
+-rw-r--r--   0     1001      127      949 2024-04-13 16:13:25.000000 rython_calc-0.4.8/.pre-commit-config.yaml
+-rw-r--r--   0     1001      127     1075 2024-04-13 16:13:25.000000 rython_calc-0.4.8/LICENSE
+-rw-r--r--   0     1001      127      603 2024-04-13 16:13:25.000000 rython_calc-0.4.8/README.md
+-rw-r--r--   0     1001      127    29590 2024-04-13 16:13:25.000000 rython_calc-0.4.8/poetry.lock
+-rw-r--r--   0     1001      127        0 2024-04-13 16:13:25.000000 rython_calc-0.4.8/python/cli/__init__.py
+-rw-r--r--   0     1001      127     1744 2024-04-13 16:13:25.000000 rython_calc-0.4.8/python/cli/main.py
+-rw-r--r--   0     1001      127      443 2024-04-13 16:13:25.000000 rython_calc-0.4.8/python/cli/performance.txt
+-rw-r--r--   0     1001      127        0 2024-04-13 16:13:25.000000 rython_calc-0.4.8/python/rython/__init__.py
+-rw-r--r--   0     1001      127        0 2024-04-13 16:13:25.000000 rython_calc-0.4.8/python/rython/py.typed
+-rw-r--r--   0     1001      127      694 2024-04-13 16:13:25.000000 rython_calc-0.4.8/python/rython/rython_calc.pyi
+-rw-r--r--   0     1001      127     3030 2024-04-13 16:13:25.000000 rython_calc-0.4.8/src/lib.rs
+-rw-r--r--   0     1001      127      350 2024-04-13 16:13:25.000000 rython_calc-0.4.8/test/rython/test_rython_calc.py
+-rw-r--r--   0     1001      127    12301 2024-04-13 16:13:25.000000 rython_calc-0.4.8/Cargo.lock
+-rw-r--r--   0     1001      127     1685 2024-04-13 16:13:25.000000 rython_calc-0.4.8/pyproject.toml
+-rw-r--r--   0        0        0     1263 1970-01-01 00:00:00.000000 rython_calc-0.4.8/PKG-INFO
```

### Comparing `rython_calc-0.4.7/.github/workflows/CI.yml` & `rython_calc-0.4.8/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `rython_calc-0.4.7/.gitignore` & `rython_calc-0.4.8/.gitignore`

 * *Files identical despite different names*

### Comparing `rython_calc-0.4.7/LICENSE` & `rython_calc-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `rython_calc-0.4.7/README.md` & `rython_calc-0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `rython_calc-0.4.7/python/cli/main.py` & `rython_calc-0.4.8/python/cli/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from time import perf_counter
+
 from rython import rython_calc
 
 if __name__ == "__main__":
     NUMBER_OF_LOOPS = 3 * 10**7
 
     t1_start = perf_counter()
     new_int: rython_calc.NewInt = rython_calc.NewInt(1)
```

### Comparing `rython_calc-0.4.7/python/rython/rython_calc.pyi` & `rython_calc-0.4.8/python/rython/rython_calc.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 def sum_as_string(a: int, b: int) -> str: ...
 
 class NewInt:
     def __init__(self, number: int) -> None: ...
     def add(self, second_number: int) -> int: ...
     def mul(self, second_number: int) -> int: ...
-    def loop_add_mul_seq(self, number_of_loops: int, add_number: int, mul_number: int) -> int: ...
+    def loop_add_mul_seq(
+        self, number_of_loops: int, add_number: int, mul_number: int
+    ) -> int: ...
     def get_number(self) -> int: ...
 
 class NewFloat:
     def __init__(self, number: float) -> None: ...
     def add(self, second_number: float) -> float: ...
     def mul(self, second_number: float) -> float: ...
-    def loop_add_mul_seq(self, number_of_loops: int, add_number: float, mul_number: float) -> float: ...
+    def loop_add_mul_seq(
+        self, number_of_loops: int, add_number: float, mul_number: float
+    ) -> float: ...
     def get_number(self) -> float: ...
```

### Comparing `rython_calc-0.4.7/src/lib.rs` & `rython_calc-0.4.8/src/lib.rs`

 * *Files identical despite different names*

### Comparing `rython_calc-0.4.7/Cargo.lock` & `rython_calc-0.4.8/Cargo.lock`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,120 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
+name = "arrayref"
+version = "0.3.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6b4930d2cb77ce62f89ee5d5289b4ac049559b1c45539271f5ed4fdc7db34545"
+
+[[package]]
+name = "arrayvec"
+version = "0.5.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "23b62fc65de8e4e7f52534fb52b0f3ed04746ae267519eef2a83941e8085068b"
+
+[[package]]
 name = "autocfg"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
 
 [[package]]
+name = "base64"
+version = "0.13.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9e1b586273c5702936fe7b7d6896644d8be71e6314cfe09d3167c95f712589e8"
+
+[[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
+name = "blake2b_simd"
+version = "0.5.11"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "afa748e348ad3be8263be728124b24a24f268266f6f5d58af9d75f6a40b5c587"
+dependencies = [
+ "arrayref",
+ "arrayvec",
+ "constant_time_eq",
+]
+
+[[package]]
+name = "byteorder"
+version = "1.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1fd0f2584146f6f2ef48085050886acf353beff7305ebd1ae69500e27c67f64b"
+
+[[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
+name = "check"
+version = "1.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "89beada3dfaf43501b20ab69f1d1dd2d43b4a600eb16ca05ea0e093a100634b1"
+
+[[package]]
+name = "clippy"
+version = "0.0.302"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d911ee15579a3f50880d8c1d59ef6e79f9533127a3bd342462f5d584f5e8c294"
+dependencies = [
+ "term",
+]
+
+[[package]]
+name = "constant_time_eq"
+version = "0.1.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "245097e9a4535ee1e3e3931fcfcd55a796a44c643e8596ff6566d68f09b87bbc"
+
+[[package]]
+name = "crossbeam-utils"
+version = "0.8.19"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "248e3bacc7dc6baa3b21e405ee045c3047101a49145e7e9eca583ab4c2ca5345"
+
+[[package]]
+name = "dirs"
+version = "1.0.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3fd78930633bd1c6e35c4b42b1df7b0cbc6bc191146e512bb3bedf243fcc3901"
+dependencies = [
+ "libc",
+ "redox_users",
+ "winapi",
+]
+
+[[package]]
+name = "fmt"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "09904adae26440d46daeacb5ed7922fee69d43ebf84d31e078cd49652cecd718"
+
+[[package]]
+name = "getrandom"
+version = "0.1.16"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8fc3cb4d91f53b50155bdcfd23f6a4c39ae1969c2ae85982b135750cccaf5fce"
+dependencies = [
+ "cfg-if",
+ "libc",
+ "wasi",
+]
+
+[[package]]
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
 [[package]]
 name = "indoc"
@@ -77,15 +167,15 @@
 name = "parking_lot_core"
 version = "0.9.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4c42a9226546d68acdd9c0a280d17ce19bfe27a46bf68784e4066115788d008e"
 dependencies = [
  "cfg-if",
  "libc",
- "redox_syscall",
+ "redox_syscall 0.4.1",
  "smallvec",
  "windows-targets",
 ]
 
 [[package]]
 name = "portable-atomic"
 version = "1.6.0"
@@ -171,25 +261,57 @@
 checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "redox_syscall"
+version = "0.1.57"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "41cc0f7e4d5d4544e8861606a285bb08d3e70712ccc7d2b84d7c0ccfaf4b05ce"
+
+[[package]]
+name = "redox_syscall"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
+name = "redox_users"
+version = "0.3.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "de0737333e7a9502c789a36d7c7fa6092a49895d4faa31ca5df163857ded2e9d"
+dependencies = [
+ "getrandom",
+ "redox_syscall 0.1.57",
+ "rust-argon2",
+]
+
+[[package]]
+name = "rust-argon2"
+version = "0.8.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4b18820d944b33caa75a71378964ac46f58517c92b6ae5f762636247c09e78fb"
+dependencies = [
+ "base64",
+ "blake2b_simd",
+ "constant_time_eq",
+ "crossbeam-utils",
+]
+
+[[package]]
 name = "rython"
-version = "0.4.7"
+version = "0.4.8"
 dependencies = [
+ "check",
+ "clippy",
+ "fmt",
  "pyo3",
 ]
 
 [[package]]
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -215,26 +337,65 @@
 [[package]]
 name = "target-lexicon"
 version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
+name = "term"
+version = "0.5.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "edd106a334b7657c10b7c540a0106114feadeb4dc314513e97df481d5d966f42"
+dependencies = [
+ "byteorder",
+ "dirs",
+ "winapi",
+]
+
+[[package]]
 name = "unicode-ident"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3354b9ac3fae1ff6755cb6db53683adb661634f67557942dea4facebec0fee4b"
 
 [[package]]
 name = "unindent"
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c7de7d73e1754487cb58364ee906a499937a0dfabd86bcb980fa99ec8c8fa2ce"
 
 [[package]]
+name = "wasi"
+version = "0.9.0+wasi-snapshot-preview1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "cccddf32554fecc6acb585f82a32a72e28b48f8c4c1883ddfeeeaa96f7d8e519"
+
+[[package]]
+name = "winapi"
+version = "0.3.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5c839a674fcd7a98952e593242ea400abe93992746761e38641405d28b00f419"
+dependencies = [
+ "winapi-i686-pc-windows-gnu",
+ "winapi-x86_64-pc-windows-gnu",
+]
+
+[[package]]
+name = "winapi-i686-pc-windows-gnu"
+version = "0.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ac3b87c63620426dd9b991e5ce0329eff545bccbbb34f3be09ff6fb6ab51b7b6"
+
+[[package]]
+name = "winapi-x86_64-pc-windows-gnu"
+version = "0.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
+
+[[package]]
 name = "windows-targets"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
 dependencies = [
  "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
```

### Comparing `rython_calc-0.4.7/pyproject.toml` & `rython_calc-0.4.8/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["maturin>=1.5,<2.0"]
 build-backend = "maturin"
 
 [project]
 name = "rython_calc"
 requires-python = ">=3.12"
-version = "0.4.7"
+version = "0.4.8"
 description = "Small project developed by me to learn PyO3 library."
 authors = [
     {name = "Krystian Krakowski", email = "kkrakowski22@gmail.com"}
 ]
 maintainers = [
     {name = "Krystian Krakowski", email = "kkrakowski22@gmail.com"}
 ]
@@ -31,15 +31,15 @@
 python-source = "python"
 bindings = "pyo3"
 module-name = "rython.rython_calc"
 strip = true
 
 [tool.poetry]
 name = "rython_calc"
-version = "0.4.7"
+version = "0.4.8"
 description = "Small project developed by me to learn PyO3 library."
 authors = ["Krystian Krakowski <kkrakowski22@gmail.com>"]
 maintainers = ["Krystian Krakowski <kkrakowski22@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 classifiers = [
     "Development Status :: 1 - Planning",
@@ -51,7 +51,13 @@
 [tool.poetry.dependencies]
 python = "^3.12"
 
 [tool.poetry.group.dev.dependencies]
 maturin = "^1.5.1"
 pytest = "^8.1.1"
 mypy = "^1.9.0"
+isort = "^5.13.2"
+black = "^24.4.0"
+pre-commit = "^3.7.0"
+
+[tool.isort]
+profile = "black"
```

### Comparing `rython_calc-0.4.7/PKG-INFO` & `rython_calc-0.4.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: rython_calc
-Version: 0.4.7
+Version: 0.4.8
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Small project developed by me to learn PyO3 library.
 Author-email: Krystian Krakowski <kkrakowski22@gmail.com>
```

