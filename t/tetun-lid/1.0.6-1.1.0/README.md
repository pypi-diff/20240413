# Comparing `tmp/tetun_lid-1.0.6.tar.gz` & `tmp/tetun_lid-1.1.0.tar.gz`

## Comparing `tetun_lid-1.0.6.tar` & `tetun_lid-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,795 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tetun_lid-1.0.6/.DS_Store
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 tetun_lid-1.0.6/Pipfile
--rw-r--r--   0        0        0     8238 2020-02-02 00:00:00.000000 tetun_lid-1.0.6/Pipfile.lock
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 tetun_lid-1.0.6/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tetun_lid-1.0.6/tetunlid/__init__.py
--rw-r--r--   0        0        0     2803 2020-02-02 00:00:00.000000 tetun_lid-1.0.6/tetunlid/lid.py
--rw-r--r--   0        0        0 16769278 2020-02-02 00:00:00.000000 tetun_lid-1.0.6/tetunlid/model/tetun_lid_model.pkl
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 tetun_lid-1.0.6/LICENSE
--rw-r--r--   0        0        0     6433 2020-02-02 00:00:00.000000 tetun_lid-1.0.6/README.md
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 tetun_lid-1.0.6/pyproject.toml
--rw-r--r--   0        0        0     6896 2020-02-02 00:00:00.000000 tetun_lid-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/pyvenv.cfg
+-rw-r--r--   0        0        0     8834 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/bin/Activate.ps1
+-rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/bin/activate
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/bin/activate.csh
+-rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/bin/activate.fish
+-rwxr-xr-x   0        0        0      279 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/bin/pip
+-rwxr-xr-x   0        0        0      279 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/bin/pip3
+-rwxr-xr-x   0        0        0      279 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/bin/pip3.10
+-rwxr-xr-x   0        0        0      279 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/bin/pip3.9
+-rwxr-xr-x   0        0        0      283 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/bin/pyproject-build
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/bin/python -> /Users/gabrieldejesus/opt/anaconda3/bin/python
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/bin/python3 -> python
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/bin/python3.9 -> python
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/distutils-precedence.pth
+-rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/_distutils_hack/__init__.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/_distutils_hack/override.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/build/__init__.py
+-rw-r--r--   0        0        0    14227 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/build/__main__.py
+-rw-r--r--   0        0        0    13393 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/build/_builder.py
+-rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/build/_ctx.py
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/build/_exceptions.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/build/_types.py
+-rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/build/_util.py
+-rw-r--r--   0        0        0    13473 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/build/env.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/build/py.typed
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/build/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/build/_compat/__init__.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/build/_compat/importlib.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/build/_compat/tarfile.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/build/_compat/tomllib.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/build-1.2.1.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/build-1.2.1.dist-info/LICENSE
+-rw-r--r--   0        0        0     4324 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/build-1.2.1.dist-info/METADATA
+-rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/build-1.2.1.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/build-1.2.1.dist-info/REQUESTED
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/build-1.2.1.dist-info/WHEEL
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/build-1.2.1.dist-info/entry_points.txt
+-rw-r--r--   0        0        0    34302 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/importlib_metadata/__init__.py
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/importlib_metadata/_adapters.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/importlib_metadata/_collections.py
+-rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/importlib_metadata/_compat.py
+-rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/importlib_metadata/_functools.py
+-rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/importlib_metadata/_itertools.py
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/importlib_metadata/_meta.py
+-rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/importlib_metadata/_text.py
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/importlib_metadata/diagnose.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/importlib_metadata/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/importlib_metadata/compat/__init__.py
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/importlib_metadata/compat/py39.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/importlib_metadata-7.1.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/importlib_metadata-7.1.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/importlib_metadata-7.1.0.dist-info/METADATA
+-rw-r--r--   0        0        0     2254 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/importlib_metadata-7.1.0.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/importlib_metadata-7.1.0.dist-info/WHEEL
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/importlib_metadata-7.1.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/packaging/__init__.py
+-rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/packaging/_elffile.py
+-rw-r--r--   0        0        0     9590 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/packaging/_manylinux.py
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/packaging/_musllinux.py
+-rw-r--r--   0        0        0    10347 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/packaging/_parser.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/packaging/_structures.py
+-rw-r--r--   0        0        0     5292 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/packaging/_tokenizer.py
+-rw-r--r--   0        0        0     8208 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/packaging/markers.py
+-rw-r--r--   0        0        0    33036 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/packaging/metadata.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/packaging/py.typed
+-rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/packaging/requirements.py
+-rw-r--r--   0        0        0    39784 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/packaging/specifiers.py
+-rw-r--r--   0        0        0    18950 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/packaging/tags.py
+-rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/packaging/utils.py
+-rw-r--r--   0        0        0    16236 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/packaging/version.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/packaging-24.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/packaging-24.0.dist-info/LICENSE
+-rw-r--r--   0        0        0    10174 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/packaging-24.0.dist-info/LICENSE.APACHE
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/packaging-24.0.dist-info/LICENSE.BSD
+-rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/packaging-24.0.dist-info/METADATA
+-rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/packaging-24.0.dist-info/RECORD
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/packaging-24.0.dist-info/WHEEL
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/__init__.py
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/__main__.py
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/__pip-runner__.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/py.typed
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/__init__.py
+-rw-r--r--   0        0        0    10243 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/build_env.py
+-rw-r--r--   0        0        0    10370 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/cache.py
+-rw-r--r--   0        0        0    14006 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/configuration.py
+-rw-r--r--   0        0        0    23634 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/exceptions.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/main.py
+-rw-r--r--   0        0        0     7152 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/pyproject.py
+-rw-r--r--   0        0        0     8378 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/self_outdated_check.py
+-rw-r--r--   0        0        0    11801 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/wheel_builder.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/cli/__init__.py
+-rw-r--r--   0        0        0     6690 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/cli/autocompletion.py
+-rw-r--r--   0        0        0     8733 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/cli/base_command.py
+-rw-r--r--   0        0        0    30064 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/cli/cmdoptions.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/cli/command_context.py
+-rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/cli/main.py
+-rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/cli/main_parser.py
+-rw-r--r--   0        0        0    10781 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/cli/parser.py
+-rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/cli/progress_bars.py
+-rw-r--r--   0        0        0    18369 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/cli/req_command.py
+-rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/cli/spinners.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/cli/status_codes.py
+-rw-r--r--   0        0        0     3882 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/commands/__init__.py
+-rw-r--r--   0        0        0     7944 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/commands/cache.py
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/commands/check.py
+-rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/commands/completion.py
+-rw-r--r--   0        0        0     9766 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/commands/configuration.py
+-rw-r--r--   0        0        0     6777 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/commands/debug.py
+-rw-r--r--   0        0        0     5335 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/commands/download.py
+-rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/commands/freeze.py
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/commands/hash.py
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/commands/help.py
+-rw-r--r--   0        0        0     4775 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/commands/index.py
+-rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/commands/inspect.py
+-rw-r--r--   0        0        0    28782 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/commands/install.py
+-rw-r--r--   0        0        0    12450 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/commands/list.py
+-rw-r--r--   0        0        0     5697 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/commands/search.py
+-rw-r--r--   0        0        0     6419 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/commands/show.py
+-rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/commands/uninstall.py
+-rw-r--r--   0        0        0     6476 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/commands/wheel.py
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/distributions/__init__.py
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/distributions/base.py
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/distributions/installed.py
+-rw-r--r--   0        0        0     6709 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/distributions/sdist.py
+-rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/distributions/wheel.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/index/__init__.py
+-rw-r--r--   0        0        0    16590 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/index/collector.py
+-rw-r--r--   0        0        0    37843 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/index/package_finder.py
+-rw-r--r--   0        0        0     8688 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/index/sources.py
+-rw-r--r--   0        0        0    15365 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/locations/__init__.py
+-rw-r--r--   0        0        0     6009 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/locations/_distutils.py
+-rw-r--r--   0        0        0     7680 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/locations/_sysconfig.py
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/locations/base.py
+-rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/metadata/__init__.py
+-rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/metadata/_json.py
+-rw-r--r--   0        0        0    25907 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/metadata/base.py
+-rw-r--r--   0        0        0    10035 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/metadata/pkg_resources.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/metadata/importlib/__init__.py
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/metadata/importlib/_compat.py
+-rw-r--r--   0        0        0     8297 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/metadata/importlib/_dists.py
+-rw-r--r--   0        0        0     7456 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/metadata/importlib/_envs.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/models/__init__.py
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/models/candidate.py
+-rw-r--r--   0        0        0     6889 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/models/direct_url.py
+-rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/models/format_control.py
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/models/index.py
+-rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/models/installation_report.py
+-rw-r--r--   0        0        0    20777 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/models/link.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/models/scheme.py
+-rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/models/search_scope.py
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/models/selection_prefs.py
+-rw-r--r--   0        0        0     4272 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/models/target_python.py
+-rw-r--r--   0        0        0     3600 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/models/wheel.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/network/__init__.py
+-rw-r--r--   0        0        0    20541 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/network/auth.py
+-rw-r--r--   0        0        0     3935 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/network/cache.py
+-rw-r--r--   0        0        0     6086 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/network/download.py
+-rw-r--r--   0        0        0     7638 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/network/lazy_wheel.py
+-rw-r--r--   0        0        0    18698 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/network/session.py
+-rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/network/utils.py
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/network/xmlrpc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/operations/__init__.py
+-rw-r--r--   0        0        0     6806 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/operations/check.py
+-rw-r--r--   0        0        0     9816 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/operations/freeze.py
+-rw-r--r--   0        0        0    28128 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/operations/prepare.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/operations/build/__init__.py
+-rw-r--r--   0        0        0     4832 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/operations/build/build_tracker.py
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/operations/build/metadata.py
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/operations/build/metadata_editable.py
+-rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/operations/build/metadata_legacy.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/operations/build/wheel.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/operations/build/wheel_editable.py
+-rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/operations/build/wheel_legacy.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/operations/install/__init__.py
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/operations/install/editable_legacy.py
+-rw-r--r--   0        0        0    27311 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/operations/install/wheel.py
+-rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/req/__init__.py
+-rw-r--r--   0        0        0    19018 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/req/constructors.py
+-rw-r--r--   0        0        0    17790 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/req/req_file.py
+-rw-r--r--   0        0        0    35460 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/req/req_install.py
+-rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/req/req_set.py
+-rw-r--r--   0        0        0    24551 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/req/req_uninstall.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/resolution/__init__.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/resolution/base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/resolution/legacy/__init__.py
+-rw-r--r--   0        0        0    24025 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/resolution/legacy/resolver.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/resolution/resolvelib/__init__.py
+-rw-r--r--   0        0        0     5173 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/resolution/resolvelib/base.py
+-rw-r--r--   0        0        0    21052 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/resolution/resolvelib/candidates.py
+-rw-r--r--   0        0        0    32292 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/resolution/resolvelib/factory.py
+-rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
+-rw-r--r--   0        0        0     9824 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/resolution/resolvelib/provider.py
+-rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/resolution/resolvelib/reporter.py
+-rw-r--r--   0        0        0     5696 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/resolution/resolvelib/requirements.py
+-rw-r--r--   0        0        0    12592 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/resolution/resolvelib/resolver.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/utils/__init__.py
+-rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/utils/_jaraco_text.py
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/utils/_log.py
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/utils/appdirs.py
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/utils/compat.py
+-rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/utils/compatibility_tags.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/utils/datetime.py
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/utils/deprecation.py
+-rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/utils/direct_url_helpers.py
+-rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/utils/egg_link.py
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/utils/encoding.py
+-rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/utils/entrypoints.py
+-rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/utils/filesystem.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/utils/filetypes.py
+-rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/utils/glibc.py
+-rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/utils/hashes.py
+-rw-r--r--   0        0        0    11603 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/utils/logging.py
+-rw-r--r--   0        0        0    23623 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/utils/misc.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/utils/models.py
+-rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/utils/packaging.py
+-rw-r--r--   0        0        0     4435 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/utils/setuptools_build.py
+-rw-r--r--   0        0        0     9207 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/utils/subprocess.py
+-rw-r--r--   0        0        0     9312 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/utils/temp_dir.py
+-rw-r--r--   0        0        0     8821 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/utils/unpacking.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/utils/urls.py
+-rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/utils/virtualenv.py
+-rw-r--r--   0        0        0     4499 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/utils/wheel.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/vcs/__init__.py
+-rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/vcs/bazaar.py
+-rw-r--r--   0        0        0    18121 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/vcs/git.py
+-rw-r--r--   0        0        0     5249 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/vcs/mercurial.py
+-rw-r--r--   0        0        0    11729 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/vcs/subversion.py
+-rw-r--r--   0        0        0    22787 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_internal/vcs/versioncontrol.py
+-rw-r--r--   0        0        0     4993 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/__init__.py
+-rw-r--r--   0        0        0    34549 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/six.py
+-rw-r--r--   0        0        0   111130 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/typing_extensions.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/vendor.txt
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/cachecontrol/__init__.py
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/cachecontrol/_cmd.py
+-rw-r--r--   0        0        0     6392 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/cachecontrol/adapter.py
+-rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/cachecontrol/cache.py
+-rw-r--r--   0        0        0    18384 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/cachecontrol/controller.py
+-rw-r--r--   0        0        0     4292 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/cachecontrol/filewrapper.py
+-rw-r--r--   0        0        0     4828 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/cachecontrol/heuristics.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/cachecontrol/py.typed
+-rw-r--r--   0        0        0     7173 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/cachecontrol/serialize.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/cachecontrol/wrapper.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
+-rw-r--r--   0        0        0     5352 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/certifi/__init__.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/certifi/__main__.py
+-rw-r--r--   0        0        0   281617 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/certifi/cacert.pem
+-rw-r--r--   0        0        0     4279 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/certifi/core.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/certifi/py.typed
+-rw-r--r--   0        0        0     4797 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/chardet/__init__.py
+-rw-r--r--   0        0        0    31274 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/chardet/big5freq.py
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/chardet/big5prober.py
+-rw-r--r--   0        0        0    10032 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/chardet/chardistribution.py
+-rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/chardet/charsetgroupprober.py
+-rw-r--r--   0        0        0     5420 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/chardet/charsetprober.py
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/chardet/codingstatemachine.py
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/chardet/codingstatemachinedict.py
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/chardet/cp949prober.py
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/chardet/enums.py
+-rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/chardet/escprober.py
+-rw-r--r--   0        0        0    12176 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/chardet/escsm.py
+-rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/chardet/eucjpprober.py
+-rw-r--r--   0        0        0    13566 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/chardet/euckrfreq.py
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/chardet/euckrprober.py
+-rw-r--r--   0        0        0    36913 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/chardet/euctwfreq.py
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/chardet/euctwprober.py
+-rw-r--r--   0        0        0    20735 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/chardet/gb2312freq.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/chardet/gb2312prober.py
+-rw-r--r--   0        0        0    14537 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/chardet/hebrewprober.py
+-rw-r--r--   0        0        0    25796 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/chardet/jisfreq.py
+-rw-r--r--   0        0        0    42498 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/chardet/johabfreq.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/chardet/johabprober.py
+-rw-r--r--   0        0        0    27055 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/chardet/jpcntx.py
+-rw-r--r--   0        0        0   104562 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
+-rw-r--r--   0        0        0    98484 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/chardet/langgreekmodel.py
+-rw-r--r--   0        0        0    98196 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/chardet/langhebrewmodel.py
+-rw-r--r--   0        0        0   101363 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/chardet/langhungarianmodel.py
+-rw-r--r--   0        0        0   128035 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/chardet/langrussianmodel.py
+-rw-r--r--   0        0        0   102774 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/chardet/langthaimodel.py
+-rw-r--r--   0        0        0    95372 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/chardet/langturkishmodel.py
+-rw-r--r--   0        0        0     5380 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/chardet/latin1prober.py
+-rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/chardet/macromanprober.py
+-rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/chardet/mbcharsetprober.py
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
+-rw-r--r--   0        0        0    30391 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/chardet/mbcssm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/chardet/py.typed
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/chardet/resultdict.py
+-rw-r--r--   0        0        0     6400 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/chardet/sbcharsetprober.py
+-rw-r--r--   0        0        0     4137 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
+-rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/chardet/sjisprober.py
+-rw-r--r--   0        0        0    14848 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/chardet/universaldetector.py
+-rw-r--r--   0        0        0     8505 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/chardet/utf1632prober.py
+-rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/chardet/utf8prober.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/chardet/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/chardet/cli/__init__.py
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/chardet/cli/chardetect.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/chardet/metadata/__init__.py
+-rw-r--r--   0        0        0    13560 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/chardet/metadata/languages.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/colorama/__init__.py
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/colorama/ansi.py
+-rw-r--r--   0        0        0    11128 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/colorama/ansitowin32.py
+-rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/colorama/initialise.py
+-rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/colorama/win32.py
+-rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/colorama/winterm.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/colorama/tests/__init__.py
+-rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/colorama/tests/ansi_test.py
+-rw-r--r--   0        0        0    10678 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py
+-rw-r--r--   0        0        0     6741 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/colorama/tests/initialise_test.py
+-rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/colorama/tests/isatty_test.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/colorama/tests/utils.py
+-rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/colorama/tests/winterm_test.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/distlib/__init__.py
+-rw-r--r--   0        0        0    41487 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/distlib/compat.py
+-rw-r--r--   0        0        0    51965 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/distlib/database.py
+-rw-r--r--   0        0        0    20797 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/distlib/index.py
+-rw-r--r--   0        0        0    51767 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/distlib/locators.py
+-rw-r--r--   0        0        0    14168 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/distlib/manifest.py
+-rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/distlib/markers.py
+-rw-r--r--   0        0        0    39693 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/distlib/metadata.py
+-rw-r--r--   0        0        0    10820 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/distlib/resources.py
+-rw-r--r--   0        0        0    18315 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/distlib/scripts.py
+-rw-r--r--   0        0        0    97792 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/distlib/t32.exe
+-rw-r--r--   0        0        0   182784 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/distlib/t64-arm.exe
+-rw-r--r--   0        0        0   108032 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/distlib/t64.exe
+-rw-r--r--   0        0        0    67530 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/distlib/util.py
+-rw-r--r--   0        0        0    23747 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/distlib/version.py
+-rw-r--r--   0        0        0    91648 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/distlib/w32.exe
+-rw-r--r--   0        0        0   168448 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/distlib/w64-arm.exe
+-rw-r--r--   0        0        0   101888 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/distlib/w64.exe
+-rw-r--r--   0        0        0    43958 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/distlib/wheel.py
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/distro/__init__.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/distro/__main__.py
+-rw-r--r--   0        0        0    49330 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/distro/distro.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/distro/py.typed
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/idna/__init__.py
+-rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/idna/codec.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/idna/compat.py
+-rw-r--r--   0        0        0    12950 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/idna/core.py
+-rw-r--r--   0        0        0    44375 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/idna/idnadata.py
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/idna/intranges.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/idna/package_data.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/idna/py.typed
+-rw-r--r--   0        0        0   206539 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/idna/uts46data.py
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/msgpack/__init__.py
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/msgpack/exceptions.py
+-rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/msgpack/ext.py
+-rw-r--r--   0        0        0    34544 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/msgpack/fallback.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/packaging/__about__.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/packaging/__init__.py
+-rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/packaging/_manylinux.py
+-rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/packaging/_musllinux.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/packaging/_structures.py
+-rw-r--r--   0        0        0     8487 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/packaging/markers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/packaging/py.typed
+-rw-r--r--   0        0        0     4676 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/packaging/requirements.py
+-rw-r--r--   0        0        0    30110 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/packaging/specifiers.py
+-rw-r--r--   0        0        0    15699 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/packaging/tags.py
+-rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/packaging/utils.py
+-rw-r--r--   0        0        0    14665 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/packaging/version.py
+-rw-r--r--   0        0        0   109364 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/pkg_resources/__init__.py
+-rw-r--r--   0        0        0    20155 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/platformdirs/__init__.py
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/platformdirs/__main__.py
+-rw-r--r--   0        0        0     7211 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/platformdirs/android.py
+-rw-r--r--   0        0        0     7132 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/platformdirs/api.py
+-rw-r--r--   0        0        0     3678 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/platformdirs/macos.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/platformdirs/py.typed
+-rw-r--r--   0        0        0     8809 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/platformdirs/unix.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/platformdirs/version.py
+-rw-r--r--   0        0        0     9573 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/platformdirs/windows.py
+-rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/pygments/__init__.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/pygments/__main__.py
+-rw-r--r--   0        0        0    23685 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/pygments/cmdline.py
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/pygments/console.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/pygments/filter.py
+-rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/pygments/formatter.py
+-rw-r--r--   0        0        0    34618 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/pygments/lexer.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/pygments/modeline.py
+-rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/pygments/plugin.py
+-rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/pygments/regexopt.py
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/pygments/scanner.py
+-rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/pygments/sphinxext.py
+-rw-r--r--   0        0        0     6257 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/pygments/style.py
+-rw-r--r--   0        0        0     6184 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/pygments/token.py
+-rw-r--r--   0        0        0    63223 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/pygments/unistring.py
+-rw-r--r--   0        0        0    10230 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/pygments/util.py
+-rw-r--r--   0        0        0    40386 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/pygments/filters/__init__.py
+-rw-r--r--   0        0        0     5424 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/pygments/formatters/__init__.py
+-rw-r--r--   0        0        0     4176 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/pygments/formatters/_mapping.py
+-rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/pygments/formatters/bbcode.py
+-rw-r--r--   0        0        0     5094 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/pygments/formatters/groff.py
+-rw-r--r--   0        0        0    35610 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/pygments/formatters/html.py
+-rw-r--r--   0        0        0    21938 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/pygments/formatters/img.py
+-rw-r--r--   0        0        0     4981 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/pygments/formatters/irc.py
+-rw-r--r--   0        0        0    19351 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/pygments/formatters/latex.py
+-rw-r--r--   0        0        0     5073 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/pygments/formatters/other.py
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
+-rw-r--r--   0        0        0     5014 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/pygments/formatters/rtf.py
+-rw-r--r--   0        0        0     7335 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/pygments/formatters/svg.py
+-rw-r--r--   0        0        0     4674 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/pygments/formatters/terminal.py
+-rw-r--r--   0        0        0    11753 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/pygments/formatters/terminal256.py
+-rw-r--r--   0        0        0    12130 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/pygments/lexers/__init__.py
+-rw-r--r--   0        0        0    72281 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/pygments/lexers/_mapping.py
+-rw-r--r--   0        0        0    53424 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/pygments/lexers/python.py
+-rw-r--r--   0        0        0     3700 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/pygments/styles/__init__.py
+-rw-r--r--   0        0        0     9116 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/pyparsing/__init__.py
+-rw-r--r--   0        0        0     6567 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/pyparsing/actions.py
+-rw-r--r--   0        0        0    13387 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/pyparsing/common.py
+-rw-r--r--   0        0        0   224445 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/pyparsing/core.py
+-rw-r--r--   0        0        0     9523 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/pyparsing/exceptions.py
+-rw-r--r--   0        0        0    38646 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/pyparsing/helpers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/pyparsing/py.typed
+-rw-r--r--   0        0        0    26692 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/pyparsing/results.py
+-rw-r--r--   0        0        0    13488 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/pyparsing/testing.py
+-rw-r--r--   0        0        0    10646 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/pyparsing/unicode.py
+-rw-r--r--   0        0        0     8670 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/pyparsing/util.py
+-rw-r--r--   0        0        0    24215 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/pyproject_hooks/__init__.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/pyproject_hooks/_compat.py
+-rw-r--r--   0        0        0    11920 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/pyproject_hooks/_impl.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py
+-rw-r--r--   0        0        0    10927 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py
+-rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/requests/__init__.py
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/requests/__version__.py
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/requests/_internal_utils.py
+-rw-r--r--   0        0        0    19697 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/requests/adapters.py
+-rw-r--r--   0        0        0     6449 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/requests/api.py
+-rw-r--r--   0        0        0    10187 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/requests/auth.py
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/requests/certs.py
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/requests/compat.py
+-rw-r--r--   0        0        0    18560 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/requests/cookies.py
+-rw-r--r--   0        0        0     3823 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/requests/exceptions.py
+-rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/requests/help.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/requests/hooks.py
+-rw-r--r--   0        0        0    35288 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/requests/models.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/requests/packages.py
+-rw-r--r--   0        0        0    30373 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/requests/sessions.py
+-rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/requests/status_codes.py
+-rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/requests/structures.py
+-rw-r--r--   0        0        0    33460 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/requests/utils.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/resolvelib/__init__.py
+-rw-r--r--   0        0        0     5871 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/resolvelib/providers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/resolvelib/py.typed
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/resolvelib/reporters.py
+-rw-r--r--   0        0        0    20511 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/resolvelib/resolvers.py
+-rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/resolvelib/structs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/resolvelib/compat/__init__.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
+-rw-r--r--   0        0        0     6090 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/__init__.py
+-rw-r--r--   0        0        0     8478 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/__main__.py
+-rw-r--r--   0        0        0    10096 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/_cell_widths.py
+-rw-r--r--   0        0        0   140235 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/_emoji_codes.py
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/_emoji_replace.py
+-rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/_export_format.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/_extension.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/_fileno.py
+-rw-r--r--   0        0        0     9695 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/_inspect.py
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/_log_render.py
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/_loop.py
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/_null_file.py
+-rw-r--r--   0        0        0     7063 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/_palettes.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/_pick.py
+-rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/_ratio.py
+-rw-r--r--   0        0        0    19919 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/_spinners.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/_stack.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/_timer.py
+-rw-r--r--   0        0        0    22820 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/_win32_console.py
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/_windows.py
+-rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/_windows_renderer.py
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/_wrap.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/abc.py
+-rw-r--r--   0        0        0    10368 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/align.py
+-rw-r--r--   0        0        0     6906 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/ansi.py
+-rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/bar.py
+-rw-r--r--   0        0        0     9842 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/box.py
+-rw-r--r--   0        0        0     4509 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/cells.py
+-rw-r--r--   0        0        0    18224 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/color.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/color_triplet.py
+-rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/columns.py
+-rw-r--r--   0        0        0    99218 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/console.py
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/constrain.py
+-rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/containers.py
+-rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/control.py
+-rw-r--r--   0        0        0     8082 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/default_styles.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/diagnose.py
+-rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/emoji.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/errors.py
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/file_proxy.py
+-rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/filesize.py
+-rw-r--r--   0        0        0     9584 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/highlighter.py
+-rw-r--r--   0        0        0     5032 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/json.py
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/jupyter.py
+-rw-r--r--   0        0        0    14007 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/layout.py
+-rw-r--r--   0        0        0    14273 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/live.py
+-rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/live_render.py
+-rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/logging.py
+-rw-r--r--   0        0        0     8198 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/markup.py
+-rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/measure.py
+-rw-r--r--   0        0        0     4970 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/padding.py
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/pager.py
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/palette.py
+-rw-r--r--   0        0        0    10574 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/panel.py
+-rw-r--r--   0        0        0    35852 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/pretty.py
+-rw-r--r--   0        0        0    59706 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/progress.py
+-rw-r--r--   0        0        0     8165 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/progress_bar.py
+-rw-r--r--   0        0        0    11303 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/prompt.py
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/protocol.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/py.typed
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/region.py
+-rw-r--r--   0        0        0     4431 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/repr.py
+-rw-r--r--   0        0        0     4602 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/rule.py
+-rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/scope.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/screen.py
+-rw-r--r--   0        0        0    24247 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/segment.py
+-rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/spinner.py
+-rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/status.py
+-rw-r--r--   0        0        0    27073 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/style.py
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/styled.py
+-rw-r--r--   0        0        0    35173 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/syntax.py
+-rw-r--r--   0        0        0    39684 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/table.py
+-rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/terminal_theme.py
+-rw-r--r--   0        0        0    45525 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/text.py
+-rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/theme.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/themes.py
+-rw-r--r--   0        0        0    29604 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/traceback.py
+-rw-r--r--   0        0        0     9169 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/rich/tree.py
+-rw-r--r--   0        0        0    20493 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/tenacity/__init__.py
+-rw-r--r--   0        0        0     3551 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/tenacity/_asyncio.py
+-rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/tenacity/_utils.py
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/tenacity/after.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/tenacity/before.py
+-rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/tenacity/before_sleep.py
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/tenacity/nap.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/tenacity/py.typed
+-rw-r--r--   0        0        0     8746 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/tenacity/retry.py
+-rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/tenacity/stop.py
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/tenacity/tornadoweb.py
+-rw-r--r--   0        0        0     8024 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/tenacity/wait.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/tomli/__init__.py
+-rw-r--r--   0        0        0    22633 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/tomli/_parser.py
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/tomli/_re.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/tomli/_types.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/tomli/py.typed
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/truststore/__init__.py
+-rw-r--r--   0        0        0     9893 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/truststore/_api.py
+-rw-r--r--   0        0        0    17694 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/truststore/_macos.py
+-rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/truststore/_openssl.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/truststore/_ssl_constants.py
+-rw-r--r--   0        0        0    17468 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/truststore/_windows.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/truststore/py.typed
+-rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/urllib3/__init__.py
+-rw-r--r--   0        0        0    10811 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/urllib3/_collections.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/urllib3/_version.py
+-rw-r--r--   0        0        0    20300 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/urllib3/connection.py
+-rw-r--r--   0        0        0    39990 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/urllib3/connectionpool.py
+-rw-r--r--   0        0        0     8217 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/urllib3/exceptions.py
+-rw-r--r--   0        0        0     8579 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/urllib3/fields.py
+-rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/urllib3/filepost.py
+-rw-r--r--   0        0        0    19752 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/urllib3/poolmanager.py
+-rw-r--r--   0        0        0     6691 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/urllib3/request.py
+-rw-r--r--   0        0        0    30641 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/urllib3/response.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/urllib3/contrib/__init__.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
+-rw-r--r--   0        0        0    11036 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/urllib3/contrib/appengine.py
+-rw-r--r--   0        0        0     4528 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
+-rw-r--r--   0        0        0    17081 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
+-rw-r--r--   0        0        0    34448 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
+-rw-r--r--   0        0        0     7097 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/urllib3/contrib/socks.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
+-rw-r--r--   0        0        0    17632 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
+-rw-r--r--   0        0        0    13922 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/urllib3/packages/__init__.py
+-rw-r--r--   0        0        0    34665 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/urllib3/packages/six.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
+-rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/urllib3/packages/backports/weakref_finalize.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/urllib3/util/__init__.py
+-rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/urllib3/util/connection.py
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/urllib3/util/proxy.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/urllib3/util/queue.py
+-rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/urllib3/util/request.py
+-rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/urllib3/util/response.py
+-rw-r--r--   0        0        0    22013 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/urllib3/util/retry.py
+-rw-r--r--   0        0        0    17177 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/urllib3/util/ssl_.py
+-rw-r--r--   0        0        0     5758 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
+-rw-r--r--   0        0        0     6895 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/urllib3/util/ssltransport.py
+-rw-r--r--   0        0        0    10168 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/urllib3/util/timeout.py
+-rw-r--r--   0        0        0    14296 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/urllib3/util/url.py
+-rw-r--r--   0        0        0     5403 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/urllib3/util/wait.py
+-rw-r--r--   0        0        0    10579 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/webencodings/__init__.py
+-rw-r--r--   0        0        0     8979 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/webencodings/labels.py
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/webencodings/mklabels.py
+-rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/webencodings/tests.py
+-rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip/_vendor/webencodings/x_user_defined.py
+-rw-r--r--   0        0        0    10388 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip-24.0.dist-info/AUTHORS.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip-24.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip-24.0.dist-info/LICENSE.txt
+-rw-r--r--   0        0        0     3581 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip-24.0.dist-info/METADATA
+-rw-r--r--   0        0        0    78517 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip-24.0.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip-24.0.dist-info/REQUESTED
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip-24.0.dist-info/WHEEL
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip-24.0.dist-info/entry_points.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pip-24.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0   108202 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pkg_resources/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pkg_resources/_vendor/__init__.py
+-rw-r--r--   0        0        0    24701 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pkg_resources/_vendor/appdirs.py
+-rw-r--r--   0        0        0   232056 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pkg_resources/_vendor/pyparsing.py
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pkg_resources/_vendor/packaging/__about__.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pkg_resources/_vendor/packaging/__init__.py
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pkg_resources/_vendor/packaging/_compat.py
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pkg_resources/_vendor/packaging/_structures.py
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pkg_resources/_vendor/packaging/_typing.py
+-rw-r--r--   0        0        0     9518 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pkg_resources/_vendor/packaging/markers.py
+-rw-r--r--   0        0        0     4929 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pkg_resources/_vendor/packaging/requirements.py
+-rw-r--r--   0        0        0    31944 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pkg_resources/_vendor/packaging/specifiers.py
+-rw-r--r--   0        0        0    24067 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pkg_resources/_vendor/packaging/tags.py
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pkg_resources/_vendor/packaging/utils.py
+-rw-r--r--   0        0        0    15470 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pkg_resources/_vendor/packaging/version.py
+-rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pkg_resources/extern/__init__.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pkg_resources/tests/data/my-test-package-source/setup.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pyproject_hooks/__init__.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pyproject_hooks/_compat.py
+-rw-r--r--   0        0        0    11920 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pyproject_hooks/_impl.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pyproject_hooks/_in_process/__init__.py
+-rw-r--r--   0        0        0    10927 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pyproject_hooks/_in_process/_in_process.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pyproject_hooks-1.0.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pyproject_hooks-1.0.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pyproject_hooks-1.0.0.dist-info/METADATA
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pyproject_hooks-1.0.0.dist-info/RECORD
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/pyproject_hooks-1.0.0.dist-info/WHEEL
+-rw-r--r--   0        0        0     7681 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/__init__.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_deprecation_warning.py
+-rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_imp.py
+-rw-r--r--   0        0        0     7077 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/archive_util.py
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/build_meta.py
+-rw-r--r--   0        0        0    65536 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/cli-32.exe
+-rw-r--r--   0        0        0    74752 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/cli-64.exe
+-rw-r--r--   0        0        0    65536 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/cli.exe
+-rw-r--r--   0        0        0    22279 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/config.py
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/dep_util.py
+-rw-r--r--   0        0        0     5474 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/depends.py
+-rw-r--r--   0        0        0    42591 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/dist.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/errors.py
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/extension.py
+-rw-r--r--   0        0        0     4873 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/glob.py
+-rw-r--r--   0        0        0    65536 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/gui-32.exe
+-rw-r--r--   0        0        0    75264 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/gui-64.exe
+-rw-r--r--   0        0        0    65536 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/gui.exe
+-rw-r--r--   0        0        0     3567 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/installer.py
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/launch.py
+-rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/lib2to3_ex.py
+-rw-r--r--   0        0        0     5217 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/monkey.py
+-rw-r--r--   0        0        0    50561 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/msvc.py
+-rw-r--r--   0        0        0     3093 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/namespaces.py
+-rw-r--r--   0        0        0    39886 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/package_index.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/py34compat.py
+-rw-r--r--   0        0        0    14151 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/sandbox.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/script (dev).tmpl
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/script.tmpl
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/unicode_utils.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/version.py
+-rw-r--r--   0        0        0     8288 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/wheel.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/windows_support.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_distutils/__init__.py
+-rw-r--r--   0        0        0    20813 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_distutils/_msvccompiler.py
+-rw-r--r--   0        0        0     8572 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_distutils/archive_util.py
+-rw-r--r--   0        0        0    14894 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_distutils/bcppcompiler.py
+-rw-r--r--   0        0        0    47607 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_distutils/ccompiler.py
+-rw-r--r--   0        0        0    18079 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_distutils/cmd.py
+-rw-r--r--   0        0        0     4827 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_distutils/config.py
+-rw-r--r--   0        0        0     8876 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_distutils/core.py
+-rw-r--r--   0        0        0    16938 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_distutils/cygwinccompiler.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_distutils/debug.py
+-rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_distutils/dep_util.py
+-rw-r--r--   0        0        0     7778 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_distutils/dir_util.py
+-rw-r--r--   0        0        0    50421 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_distutils/dist.py
+-rw-r--r--   0        0        0     3577 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_distutils/errors.py
+-rw-r--r--   0        0        0    10515 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_distutils/extension.py
+-rw-r--r--   0        0        0    17784 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_distutils/fancy_getopt.py
+-rw-r--r--   0        0        0     8148 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_distutils/file_util.py
+-rw-r--r--   0        0        0    13407 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_distutils/filelist.py
+-rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_distutils/log.py
+-rw-r--r--   0        0        0    30453 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_distutils/msvc9compiler.py
+-rw-r--r--   0        0        0    23540 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_distutils/msvccompiler.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_distutils/py35compat.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_distutils/py38compat.py
+-rw-r--r--   0        0        0     3498 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_distutils/spawn.py
+-rw-r--r--   0        0        0    21349 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_distutils/sysconfig.py
+-rw-r--r--   0        0        0    12483 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_distutils/text_file.py
+-rw-r--r--   0        0        0    14957 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_distutils/unixccompiler.py
+-rw-r--r--   0        0        0    23185 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_distutils/util.py
+-rw-r--r--   0        0        0    12514 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_distutils/version.py
+-rw-r--r--   0        0        0     5133 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_distutils/versionpredicate.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_distutils/command/__init__.py
+-rw-r--r--   0        0        0     5562 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_distutils/command/bdist.py
+-rw-r--r--   0        0        0     4913 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_distutils/command/bdist_dumb.py
+-rw-r--r--   0        0        0    35579 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_distutils/command/bdist_msi.py
+-rw-r--r--   0        0        0    21537 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_distutils/command/bdist_rpm.py
+-rw-r--r--   0        0        0    16030 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_distutils/command/bdist_wininst.py
+-rw-r--r--   0        0        0     5773 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_distutils/command/build.py
+-rw-r--r--   0        0        0     8022 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_distutils/command/build_clib.py
+-rw-r--r--   0        0        0    31720 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_distutils/command/build_ext.py
+-rw-r--r--   0        0        0    17190 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_distutils/command/build_py.py
+-rw-r--r--   0        0        0     6232 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_distutils/command/build_scripts.py
+-rw-r--r--   0        0        0     5637 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_distutils/command/check.py
+-rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_distutils/command/clean.py
+-rw-r--r--   0        0        0    13117 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_distutils/command/config.py
+-rw-r--r--   0        0        0    27488 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_distutils/command/install.py
+-rw-r--r--   0        0        0     2822 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_distutils/command/install_data.py
+-rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_distutils/command/install_egg_info.py
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_distutils/command/install_headers.py
+-rw-r--r--   0        0        0     8397 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_distutils/command/install_lib.py
+-rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_distutils/command/install_scripts.py
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_distutils/command/py37compat.py
+-rw-r--r--   0        0        0    11712 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_distutils/command/register.py
+-rw-r--r--   0        0        0    19005 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_distutils/command/sdist.py
+-rw-r--r--   0        0        0     7597 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_distutils/command/upload.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_vendor/__init__.py
+-rw-r--r--   0        0        0    15130 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_vendor/ordered_set.py
+-rw-r--r--   0        0        0   232056 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_vendor/pyparsing.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_vendor/more_itertools/__init__.py
+-rw-r--r--   0        0        0   117968 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_vendor/more_itertools/more.py
+-rw-r--r--   0        0        0    16256 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_vendor/more_itertools/recipes.py
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_vendor/packaging/__about__.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_vendor/packaging/__init__.py
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_vendor/packaging/_compat.py
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_vendor/packaging/_structures.py
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_vendor/packaging/_typing.py
+-rw-r--r--   0        0        0     9509 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_vendor/packaging/markers.py
+-rw-r--r--   0        0        0     4917 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_vendor/packaging/requirements.py
+-rw-r--r--   0        0        0    31944 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_vendor/packaging/specifiers.py
+-rw-r--r--   0        0        0    24067 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_vendor/packaging/tags.py
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_vendor/packaging/utils.py
+-rw-r--r--   0        0        0    15470 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/_vendor/packaging/version.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/command/__init__.py
+-rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/command/alias.py
+-rw-r--r--   0        0        0    16604 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/command/bdist_egg.py
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/command/bdist_rpm.py
+-rw-r--r--   0        0        0     4415 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/command/build_clib.py
+-rw-r--r--   0        0        0    13212 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/command/build_ext.py
+-rw-r--r--   0        0        0     8930 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/command/build_py.py
+-rw-r--r--   0        0        0     8045 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/command/develop.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/command/dist_info.py
+-rw-r--r--   0        0        0    85308 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/command/easy_install.py
+-rw-r--r--   0        0        0    25335 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/command/egg_info.py
+-rw-r--r--   0        0        0     4705 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/command/install.py
+-rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/command/install_egg_info.py
+-rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/command/install_lib.py
+-rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/command/install_scripts.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/command/launcher manifest.xml
+-rw-r--r--   0        0        0     4946 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/command/py36compat.py
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/command/register.py
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/command/rotate.py
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/command/saveopts.py
+-rw-r--r--   0        0        0     5967 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/command/sdist.py
+-rw-r--r--   0        0        0     5051 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/command/setopt.py
+-rw-r--r--   0        0        0     9490 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/command/test.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/command/upload.py
+-rw-r--r--   0        0        0     7218 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/command/upload_docs.py
+-rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools/extern/__init__.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools-57.4.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools-57.4.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     4908 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools-57.4.0.dist-info/METADATA
+-rw-r--r--   0        0        0    23074 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools-57.4.0.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools-57.4.0.dist-info/REQUESTED
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools-57.4.0.dist-info/WHEEL
+-rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools-57.4.0.dist-info/entry_points.txt
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/setuptools-57.4.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/tomli/__init__.py
+-rw-r--r--   0        0        0    22633 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/tomli/_parser.py
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/tomli/_re.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/tomli/_types.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/tomli/py.typed
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/tomli-2.0.1.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/tomli-2.0.1.dist-info/LICENSE
+-rw-r--r--   0        0        0     8875 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/tomli-2.0.1.dist-info/METADATA
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/tomli-2.0.1.dist-info/RECORD
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/tomli-2.0.1.dist-info/WHEEL
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/zipp/__init__.py
+-rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/zipp/glob.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/zipp/compat/__init__.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/zipp/compat/py310.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/zipp-3.18.1.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/zipp-3.18.1.dist-info/LICENSE
+-rw-r--r--   0        0        0     3461 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/zipp-3.18.1.dist-info/METADATA
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/zipp-3.18.1.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/zipp-3.18.1.dist-info/WHEEL
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/.tetunlidnew/lib/python3.9/site-packages/zipp-3.18.1.dist-info/top_level.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/tetunlid/__init__.py
+-rw-r--r--   0        0        0     2803 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/tetunlid/lid.py
+-rw-r--r--   0        0        0 16769278 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/tetunlid/model/tetun_lid_model.pkl
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/LICENSE
+-rw-r--r--   0        0        0     6433 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/README.md
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6896 2020-02-02 00:00:00.000000 tetun_lid-1.1.0/PKG-INFO
```

### Comparing `tetun_lid-1.0.6/tetunlid/lid.py` & `tetun_lid-1.1.0/tetunlid/lid.py`

 * *Files identical despite different names*

### Comparing `tetun_lid-1.0.6/tetunlid/model/tetun_lid_model.pkl` & `tetun_lid-1.1.0/tetunlid/model/tetun_lid_model.pkl`

 * *Files identical despite different names*

### Comparing `tetun_lid-1.0.6/LICENSE` & `tetun_lid-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tetun_lid-1.0.6/README.md` & `tetun_lid-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `tetun_lid-1.0.6/pyproject.toml` & `tetun_lid-1.1.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tetun_lid"
-version = "1.0.6"
+version = "1.1.0"
 
 authors = [
   { name="Gabriel de Jesus", email="gabriel.dejesus@timornews.tl" },
 ]
 description = "Tetun Language Identification Model"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [tool.hatch.build.targets.wheel]
-packages = ["src/tetun_lid"]
+packages = ["tetunlid"]
 
 [project.urls]
 repository= "https://github.com/gabriel-de-jesus/tetun-lid"
```

### Comparing `tetun_lid-1.0.6/PKG-INFO` & `tetun_lid-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: tetun_lid
-Version: 1.0.6
+Version: 1.1.0
 Summary: Tetun Language Identification Model
 Project-URL: repository, https://github.com/gabriel-de-jesus/tetun-lid
 Author-email: Gabriel de Jesus <gabriel.dejesus@timornews.tl>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 ### Tetun LID
 Tetun Language Identification (Tetun LID) model is a machine learning model that automatically identifies the language of a given text. It was specifically designed to recognize four languages commonly spoken in Timor-Leste: Tetun, Portuguese, English, and Indonesian.
 
 ### Installation
```

