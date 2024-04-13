# Comparing `tmp/mypy_baseline-0.6.1.tar.gz` & `tmp/mypy_baseline-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy_baseline-0.6.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "mypy_baseline-0.7.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `mypy_baseline-0.6.1.tar` & `mypy_baseline-0.7.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0      710 2023-06-14 09:11:46.439051 mypy_baseline-0.6.1/.github/workflows/main.yml
--rw-r--r--   0        0        0      140 2023-09-25 06:45:27.588929 mypy_baseline-0.6.1/.gitignore
--rw-r--r--   0        0        0      325 2023-02-24 08:10:15.428694 mypy_baseline-0.6.1/.markdownlint.yaml
--rw-r--r--   0        0        0     1048 2022-09-01 10:06:03.899566 mypy_baseline-0.6.1/LICENSE
--rw-r--r--   0        0        0     1964 2023-09-25 12:37:46.003628 mypy_baseline-0.6.1/README.md
--rw-r--r--   0        0        0     3448 2023-02-21 08:54:27.062504 mypy_baseline-0.6.1/Taskfile.yml
--rw-r--r--   0        0        0   127812 2022-09-28 08:10:05.956227 mypy_baseline-0.6.1/assets/example.png
--rw-r--r--   0        0        0   180974 2022-10-01 08:47:06.040486 mypy_baseline-0.6.1/assets/history.png
--rw-r--r--   0        0        0      326 2023-02-21 08:54:27.062504 mypy_baseline-0.6.1/docs/conf.py
--rw-r--r--   0        0        0      935 2023-09-25 12:37:46.003628 mypy_baseline-0.6.1/docs/config.md
--rw-r--r--   0        0        0      512 2023-04-14 07:08:04.277478 mypy_baseline-0.6.1/docs/filter.md
--rw-r--r--   0        0        0     4410 2023-02-27 13:02:41.839663 mypy_baseline-0.6.1/docs/follower.md
--rw-r--r--   0        0        0      852 2023-02-21 08:54:27.062504 mypy_baseline-0.6.1/docs/history.md
--rw-r--r--   0        0        0      486 2023-02-24 08:04:06.077059 mypy_baseline-0.6.1/docs/index.md
--rw-r--r--   0        0        0     4341 2023-02-21 08:54:27.062504 mypy_baseline-0.6.1/docs/leader.md
--rw-r--r--   0        0        0      377 2023-02-21 08:54:27.062504 mypy_baseline-0.6.1/docs/plot.md
--rw-r--r--   0        0        0     1297 2023-02-27 12:49:23.969584 mypy_baseline-0.6.1/docs/suggest.md
--rw-r--r--   0        0        0     1202 2023-04-14 07:15:00.364969 mypy_baseline-0.6.1/docs/sync.md
--rw-r--r--   0        0        0      540 2023-02-21 08:54:27.062504 mypy_baseline-0.6.1/docs/top-files.md
--rw-r--r--   0        0        0       74 2023-02-21 08:54:27.062504 mypy_baseline-0.6.1/docs/usage.md
--rw-r--r--   0        0        0      139 2023-12-02 07:39:52.494371 mypy_baseline-0.6.1/mypy_baseline/__init__.py
--rw-r--r--   0        0        0       44 2022-09-28 08:10:05.956227 mypy_baseline-0.6.1/mypy_baseline/__main__.py
--rw-r--r--   0        0        0      912 2022-09-28 08:10:05.956227 mypy_baseline-0.6.1/mypy_baseline/_cli.py
--rw-r--r--   0        0        0     2200 2022-10-08 07:27:10.462038 mypy_baseline-0.6.1/mypy_baseline/_colors.py
--rw-r--r--   0        0        0     4482 2023-09-25 12:37:46.007628 mypy_baseline-0.6.1/mypy_baseline/_config.py
--rw-r--r--   0        0        0     2525 2023-12-02 07:39:20.482759 mypy_baseline-0.6.1/mypy_baseline/_error.py
--rw-r--r--   0        0        0     2370 2022-10-08 07:27:10.462038 mypy_baseline-0.6.1/mypy_baseline/_git.py
--rw-r--r--   0        0        0      583 2023-02-24 08:04:06.077059 mypy_baseline-0.6.1/mypy_baseline/commands/__init__.py
--rw-r--r--   0        0        0      870 2022-10-26 09:21:57.066380 mypy_baseline-0.6.1/mypy_baseline/commands/_base.py
--rw-r--r--   0        0        0     3692 2023-09-25 12:37:46.007628 mypy_baseline-0.6.1/mypy_baseline/commands/_filter.py
--rw-r--r--   0        0        0     1219 2022-10-08 07:27:10.462038 mypy_baseline-0.6.1/mypy_baseline/commands/_history.py
--rw-r--r--   0        0        0     1514 2023-02-20 10:17:46.003690 mypy_baseline-0.6.1/mypy_baseline/commands/_plot.py
--rw-r--r--   0        0        0     7674 2023-03-10 09:22:19.906984 mypy_baseline-0.6.1/mypy_baseline/commands/_suggest.py
--rw-r--r--   0        0        0     2256 2023-09-25 12:37:46.007628 mypy_baseline-0.6.1/mypy_baseline/commands/_sync.py
--rw-r--r--   0        0        0     1508 2023-02-20 10:21:07.493456 mypy_baseline-0.6.1/mypy_baseline/commands/_top_files.py
--rw-r--r--   0        0        0      384 2022-09-28 08:10:05.960227 mypy_baseline-0.6.1/mypy_baseline/commands/_version.py
--rw-r--r--   0        0        0        0 2022-09-01 10:06:03.903566 mypy_baseline-0.6.1/mypy_baseline/py.typed
--rwxr-xr-x   0        0        0      147 2023-02-21 08:54:27.062504 mypy_baseline-0.6.1/netlify.sh
--rw-r--r--   0        0        0       95 2023-02-21 08:54:27.062504 mypy_baseline-0.6.1/netlify.toml
--rw-r--r--   0        0        0     1699 2023-09-25 12:37:46.007628 mypy_baseline-0.6.1/pyproject.toml
--rw-r--r--   0        0        0       66 2023-02-21 08:54:27.062504 mypy_baseline-0.6.1/setup.cfg
--rw-r--r--   0        0        0        0 2022-09-01 10:06:03.903566 mypy_baseline-0.6.1/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-02-24 08:04:06.077059 mypy_baseline-0.6.1/tests/test_commands/__init__.py
--rw-r--r--   0        0        0      989 2023-09-25 06:45:27.588929 mypy_baseline-0.6.1/tests/test_commands/helpers.py
--rw-r--r--   0        0        0     2081 2023-09-25 12:37:46.007628 mypy_baseline-0.6.1/tests/test_commands/test_filter.py
--rw-r--r--   0        0        0      385 2023-09-25 06:45:27.588929 mypy_baseline-0.6.1/tests/test_commands/test_history.py
--rw-r--r--   0        0        0     3453 2023-03-10 09:22:19.906984 mypy_baseline-0.6.1/tests/test_commands/test_suggest.py
--rw-r--r--   0        0        0     1235 2023-05-11 07:59:17.539586 mypy_baseline-0.6.1/tests/test_commands/test_sync.py
--rw-r--r--   0        0        0      637 2023-04-14 07:15:00.368969 mypy_baseline-0.6.1/tests/test_commands/test_top_files.py
--rw-r--r--   0        0        0      147 2023-02-24 08:04:06.081059 mypy_baseline-0.6.1/tests/test_commands/test_version.py
--rw-r--r--   0        0        0     2747 2023-12-02 07:39:20.486759 mypy_baseline-0.6.1/tests/test_error.py
--rw-r--r--   0        0        0     3078 1970-01-01 00:00:00.000000 mypy_baseline-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0      710 2023-06-14 09:11:46.439051 mypy_baseline-0.7.0/.github/workflows/main.yml
+-rw-r--r--   0        0        0      140 2023-09-25 06:45:27.588929 mypy_baseline-0.7.0/.gitignore
+-rw-r--r--   0        0        0      325 2023-02-24 08:10:15.428694 mypy_baseline-0.7.0/.markdownlint.yaml
+-rw-r--r--   0        0        0     1048 2022-09-01 10:06:03.899566 mypy_baseline-0.7.0/LICENSE
+-rw-r--r--   0        0        0     1964 2023-09-25 12:37:46.003628 mypy_baseline-0.7.0/README.md
+-rw-r--r--   0        0        0     3448 2023-02-21 08:54:27.062504 mypy_baseline-0.7.0/Taskfile.yml
+-rw-r--r--   0        0        0   127812 2022-09-28 08:10:05.956227 mypy_baseline-0.7.0/assets/example.png
+-rw-r--r--   0        0        0   180974 2022-10-01 08:47:06.040486 mypy_baseline-0.7.0/assets/history.png
+-rw-r--r--   0        0        0      326 2023-02-21 08:54:27.062504 mypy_baseline-0.7.0/docs/conf.py
+-rw-r--r--   0        0        0      935 2023-09-25 12:37:46.003628 mypy_baseline-0.7.0/docs/config.md
+-rw-r--r--   0        0        0      512 2023-04-14 07:08:04.277478 mypy_baseline-0.7.0/docs/filter.md
+-rw-r--r--   0        0        0     4410 2023-02-27 13:02:41.839663 mypy_baseline-0.7.0/docs/follower.md
+-rw-r--r--   0        0        0      852 2023-02-21 08:54:27.062504 mypy_baseline-0.7.0/docs/history.md
+-rw-r--r--   0        0        0      486 2023-02-24 08:04:06.077059 mypy_baseline-0.7.0/docs/index.md
+-rw-r--r--   0        0        0     4341 2023-02-21 08:54:27.062504 mypy_baseline-0.7.0/docs/leader.md
+-rw-r--r--   0        0        0      377 2023-02-21 08:54:27.062504 mypy_baseline-0.7.0/docs/plot.md
+-rw-r--r--   0        0        0     1297 2023-02-27 12:49:23.969584 mypy_baseline-0.7.0/docs/suggest.md
+-rw-r--r--   0        0        0     1202 2023-04-14 07:15:00.364969 mypy_baseline-0.7.0/docs/sync.md
+-rw-r--r--   0        0        0      540 2023-02-21 08:54:27.062504 mypy_baseline-0.7.0/docs/top-files.md
+-rw-r--r--   0        0        0       74 2023-02-21 08:54:27.062504 mypy_baseline-0.7.0/docs/usage.md
+-rw-r--r--   0        0        0      139 2024-04-13 15:26:36.750802 mypy_baseline-0.7.0/mypy_baseline/__init__.py
+-rw-r--r--   0        0        0       44 2022-09-28 08:10:05.956227 mypy_baseline-0.7.0/mypy_baseline/__main__.py
+-rw-r--r--   0        0        0      912 2022-09-28 08:10:05.956227 mypy_baseline-0.7.0/mypy_baseline/_cli.py
+-rw-r--r--   0        0        0     2200 2022-10-08 07:27:10.462038 mypy_baseline-0.7.0/mypy_baseline/_colors.py
+-rw-r--r--   0        0        0     4633 2024-04-13 15:25:53.995397 mypy_baseline-0.7.0/mypy_baseline/_config.py
+-rw-r--r--   0        0        0     2525 2023-12-02 07:39:20.482759 mypy_baseline-0.7.0/mypy_baseline/_error.py
+-rw-r--r--   0        0        0     2370 2022-10-08 07:27:10.462038 mypy_baseline-0.7.0/mypy_baseline/_git.py
+-rw-r--r--   0        0        0      583 2023-02-24 08:04:06.077059 mypy_baseline-0.7.0/mypy_baseline/commands/__init__.py
+-rw-r--r--   0        0        0      870 2022-10-26 09:21:57.066380 mypy_baseline-0.7.0/mypy_baseline/commands/_base.py
+-rw-r--r--   0        0        0     3692 2023-09-25 12:37:46.007628 mypy_baseline-0.7.0/mypy_baseline/commands/_filter.py
+-rw-r--r--   0        0        0     1219 2022-10-08 07:27:10.462038 mypy_baseline-0.7.0/mypy_baseline/commands/_history.py
+-rw-r--r--   0        0        0     1514 2023-02-20 10:17:46.003690 mypy_baseline-0.7.0/mypy_baseline/commands/_plot.py
+-rw-r--r--   0        0        0     7674 2023-03-10 09:22:19.906984 mypy_baseline-0.7.0/mypy_baseline/commands/_suggest.py
+-rw-r--r--   0        0        0     2492 2024-04-13 15:25:53.995397 mypy_baseline-0.7.0/mypy_baseline/commands/_sync.py
+-rw-r--r--   0        0        0     1508 2023-02-20 10:21:07.493456 mypy_baseline-0.7.0/mypy_baseline/commands/_top_files.py
+-rw-r--r--   0        0        0      384 2022-09-28 08:10:05.960227 mypy_baseline-0.7.0/mypy_baseline/commands/_version.py
+-rw-r--r--   0        0        0        0 2022-09-01 10:06:03.903566 mypy_baseline-0.7.0/mypy_baseline/py.typed
+-rwxr-xr-x   0        0        0      147 2023-02-21 08:54:27.062504 mypy_baseline-0.7.0/netlify.sh
+-rw-r--r--   0        0        0       95 2023-02-21 08:54:27.062504 mypy_baseline-0.7.0/netlify.toml
+-rw-r--r--   0        0        0     1699 2023-09-25 12:37:46.007628 mypy_baseline-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0       66 2023-02-21 08:54:27.062504 mypy_baseline-0.7.0/setup.cfg
+-rw-r--r--   0        0        0        0 2022-09-01 10:06:03.903566 mypy_baseline-0.7.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-24 08:04:06.077059 mypy_baseline-0.7.0/tests/test_commands/__init__.py
+-rw-r--r--   0        0        0      989 2023-09-25 06:45:27.588929 mypy_baseline-0.7.0/tests/test_commands/helpers.py
+-rw-r--r--   0        0        0     2081 2023-09-25 12:37:46.007628 mypy_baseline-0.7.0/tests/test_commands/test_filter.py
+-rw-r--r--   0        0        0      385 2023-09-25 06:45:27.588929 mypy_baseline-0.7.0/tests/test_commands/test_history.py
+-rw-r--r--   0        0        0     3453 2023-03-10 09:22:19.906984 mypy_baseline-0.7.0/tests/test_commands/test_suggest.py
+-rw-r--r--   0        0        0     1880 2024-04-13 15:25:53.995397 mypy_baseline-0.7.0/tests/test_commands/test_sync.py
+-rw-r--r--   0        0        0      637 2023-04-14 07:15:00.368969 mypy_baseline-0.7.0/tests/test_commands/test_top_files.py
+-rw-r--r--   0        0        0      147 2023-02-24 08:04:06.081059 mypy_baseline-0.7.0/tests/test_commands/test_version.py
+-rw-r--r--   0        0        0     2747 2023-12-02 07:39:20.486759 mypy_baseline-0.7.0/tests/test_error.py
+-rw-r--r--   0        0        0     3078 1970-01-01 00:00:00.000000 mypy_baseline-0.7.0/PKG-INFO
```

### Comparing `mypy_baseline-0.6.1/.github/workflows/main.yml` & `mypy_baseline-0.7.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.6.1/LICENSE` & `mypy_baseline-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.6.1/README.md` & `mypy_baseline-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.6.1/Taskfile.yml` & `mypy_baseline-0.7.0/Taskfile.yml`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.6.1/assets/example.png` & `mypy_baseline-0.7.0/assets/example.png`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.6.1/assets/history.png` & `mypy_baseline-0.7.0/assets/history.png`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.6.1/docs/config.md` & `mypy_baseline-0.7.0/docs/config.md`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.6.1/docs/filter.md` & `mypy_baseline-0.7.0/docs/filter.md`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.6.1/docs/follower.md` & `mypy_baseline-0.7.0/docs/follower.md`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.6.1/docs/history.md` & `mypy_baseline-0.7.0/docs/history.md`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.6.1/docs/leader.md` & `mypy_baseline-0.7.0/docs/leader.md`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.6.1/docs/suggest.md` & `mypy_baseline-0.7.0/docs/suggest.md`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.6.1/docs/sync.md` & `mypy_baseline-0.7.0/docs/sync.md`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.6.1/docs/top-files.md` & `mypy_baseline-0.7.0/docs/top-files.md`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.6.1/mypy_baseline/_cli.py` & `mypy_baseline-0.7.0/mypy_baseline/_cli.py`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.6.1/mypy_baseline/_colors.py` & `mypy_baseline-0.7.0/mypy_baseline/_colors.py`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.6.1/mypy_baseline/_config.py` & `mypy_baseline-0.7.0/mypy_baseline/_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 
 @dataclasses.dataclass
 class Config:
     baseline_path: Path = Path('mypy-baseline.txt')
     depth: int = 40
     allow_unsynced: bool = False
     preserve_position: bool = False
+    sort_baseline: bool = False
     hide_stats: bool = False
     no_colors: bool = bool(os.environ.get('NO_COLOR'))
     ignore: list[str] = dataclasses.field(default_factory=list)
     ignore_categories: list[str] = dataclasses.field(default_factory=list)
     default_branch: str = ''
 
     @classmethod
@@ -65,14 +66,18 @@
             help='do not fail for resolved violations.'
         )
         add(
             '--preserve-position', action='store_true',
             help='do not remove line number from the baseline.',
         )
         add(
+            '--sort-baseline', action='store_true',
+            help='sort the baseline file.',
+        )
+        add(
             '--hide-stats', action='store_true',
             help='do not show stats at the end.',
         )
         add(
             '--no-colors', action='store_true',
             help='disable colored output. Has no effect on the output of mypy.',
         )
```

### Comparing `mypy_baseline-0.6.1/mypy_baseline/_error.py` & `mypy_baseline-0.7.0/mypy_baseline/_error.py`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.6.1/mypy_baseline/_git.py` & `mypy_baseline-0.7.0/mypy_baseline/_git.py`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.6.1/mypy_baseline/commands/__init__.py` & `mypy_baseline-0.7.0/mypy_baseline/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.6.1/mypy_baseline/commands/_base.py` & `mypy_baseline-0.7.0/mypy_baseline/commands/_base.py`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.6.1/mypy_baseline/commands/_filter.py` & `mypy_baseline-0.7.0/mypy_baseline/commands/_filter.py`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.6.1/mypy_baseline/commands/_history.py` & `mypy_baseline-0.7.0/mypy_baseline/commands/_history.py`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.6.1/mypy_baseline/commands/_plot.py` & `mypy_baseline-0.7.0/mypy_baseline/commands/_plot.py`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.6.1/mypy_baseline/commands/_suggest.py` & `mypy_baseline-0.7.0/mypy_baseline/commands/_suggest.py`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.6.1/mypy_baseline/commands/_sync.py` & `mypy_baseline-0.7.0/mypy_baseline/commands/_sync.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,14 +24,17 @@
             if self.config.is_ignored(error.message):
                 continue
             if self.config.is_ignored_category(error.category):
                 continue
             clean_line = error.get_clean_line(self.config)
             new_baseline.append(clean_line)
 
+        if self.config.sort_baseline:
+            new_baseline.sort()
+
         synced = False
         if old_baseline:
             synced = self._stable_sync(old_baseline, new_baseline)
         if not synced:
             self._write_baseline(new_baseline)
         return 0
 
@@ -40,17 +43,21 @@
 
         We do that to avoid lines jumping around that happens because of not ordered
         output from mypy.
 
         Currently, we can do a stable sync only when there are no new lines added.
         It's hard to insert new lines in the correct positions, and adding them
         at the end of the file will cause merge conflicts.
-        Sorting lines alphabetically would solve the issue, but I want to keep
-        backward compatibility.
+        Sorting lines solves the issue, so we don't use stable sync when the output
+        is sorted.
+        However, sorting is not enabled by default because I want to keep backward
+        compatibility.
         """
+        if not self.config.sort_baseline:
+            return False
         old_set = set(old_bline)
         new_set = set(new_bline)
         removed = old_set - new_set
         added = new_set - old_set
         if added:
             return False
         result = [line for line in old_bline if line not in removed]
```

### Comparing `mypy_baseline-0.6.1/mypy_baseline/commands/_top_files.py` & `mypy_baseline-0.7.0/mypy_baseline/commands/_top_files.py`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.6.1/pyproject.toml` & `mypy_baseline-0.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.6.1/tests/test_commands/helpers.py` & `mypy_baseline-0.7.0/tests/test_commands/helpers.py`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.6.1/tests/test_commands/test_filter.py` & `mypy_baseline-0.7.0/tests/test_commands/test_filter.py`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.6.1/tests/test_commands/test_suggest.py` & `mypy_baseline-0.7.0/tests/test_commands/test_suggest.py`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.6.1/tests/test_commands/test_sync.py` & `mypy_baseline-0.7.0/tests/test_commands/test_sync.py`

 * *Files 22% similar despite different names*

```diff
@@ -30,7 +30,23 @@
     stdin.write(NOTEBOOK_LINE1)
     stdin.seek(0)
     code = main(['sync', '--baseline-path', str(blpath)], stdin, StringIO())
     assert code == 0
     actual = blpath.read_text()
     line1 = actual.splitlines()[0]
     assert line1 == 'fail.ipynb:cell_1:0: error: Incompatible return value type (got "int", expected "str")  [return-value]'  # noqa: E501
+
+
+def test_sync_sorted(tmp_path: Path):
+    blpath = tmp_path / 'bline.txt'
+    stdin = StringIO()
+    stdin.write(LINE1)
+    stdin.write(LINE2)
+    stdin.write(LINE3)
+    stdin.seek(0)
+    code = main(['sync', '--sort-baseline', '--baseline-path', str(blpath)], stdin, StringIO())  # noqa: E501
+    assert code == 0
+    actual = blpath.read_text()
+    line1, line2, line3 = actual.splitlines()
+    assert line1 == 'python/utils.py:0: error: Second argument of Enum() must be string  [misc]'  # noqa: E501s
+    assert line2 == 'settings.py:0: error: How are you?  [union-attr]'
+    assert line3 == 'views.py:0: error: Hello world  [assignment]'
```

### Comparing `mypy_baseline-0.6.1/tests/test_commands/test_top_files.py` & `mypy_baseline-0.7.0/tests/test_commands/test_top_files.py`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.6.1/tests/test_error.py` & `mypy_baseline-0.7.0/tests/test_error.py`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.6.1/PKG-INFO` & `mypy_baseline-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mypy_baseline
-Version: 0.6.1
+Version: 0.7.0
 Summary: Integrate mypy with existing codebase.
 Keywords: mypy,typing,annotations,type annotations
 Author-email: Gram <git@orsinium.dev>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

