# Comparing `tmp/cosmix_launcher-1.0.3.tar.gz` & `tmp/cosmix_launcher-1.0.4.tar.gz`

## Comparing `cosmix_launcher-1.0.3.tar` & `cosmix_launcher-1.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.3/cosmix.bat
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.3/license.txt
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.3/requirements.txt
--rwxr-xr-x   0        0        0      130 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.3/scripts/publish.sh
--rwxr-xr-x   0        0        0      343 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.3/scripts/test.sh
--rw-r--r--   0        0        0     4807 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.3/src/cosmix/__main__.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.3/src/cosmix/api/__init__.py
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.3/src/cosmix/api/config.py
--rw-r--r--   0        0        0     5418 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.3/src/cosmix/api/instance.py
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.3/src/cosmix/api/logger.py
--rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.3/src/cosmix/api/maven.py
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.3/src/cosmix/api/mod.py
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.3/src/cosmix/api/net.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.3/src/cosmix/api/paths.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.3/src/cosmix/api/versions.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.3/.gitignore
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     3444 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.3/readme.md
--rw-r--r--   0        0        0     4097 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.4/cosmix.bat
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.4/license.txt
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.4/requirements.txt
+-rwxr-xr-x   0        0        0      130 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.4/scripts/publish.sh
+-rwxr-xr-x   0        0        0      343 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.4/scripts/test.sh
+-rw-r--r--   0        0        0     5117 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.4/src/cosmix/__main__.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.4/src/cosmix/api/__init__.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.4/src/cosmix/api/config.py
+-rw-r--r--   0        0        0     5418 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.4/src/cosmix/api/instance.py
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.4/src/cosmix/api/logger.py
+-rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.4/src/cosmix/api/maven.py
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.4/src/cosmix/api/mod.py
+-rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.4/src/cosmix/api/net.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.4/src/cosmix/api/paths.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.4/src/cosmix/api/versions.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.4/.gitignore
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     4112 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.4/readme.md
+-rw-r--r--   0        0        0     4765 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.4/PKG-INFO
```

### Comparing `cosmix_launcher-1.0.3/license.txt` & `cosmix_launcher-1.0.4/license.txt`

 * *Files identical despite different names*

### Comparing `cosmix_launcher-1.0.3/src/cosmix/__main__.py` & `cosmix_launcher-1.0.4/src/cosmix/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,22 +34,22 @@
     logger.info("Latest Available Versions: (these may take a second)")
     logger.info("  Cosmic Reach: " + versions.get_latest_of("reach"))
     logger.info("  Cosmic Quilt: " + versions.get_latest_of("quilt"))
 
 
 @cosmix.command()
 @click.option("--version", "-v", default="latest", type=str, help="The version of Cosmic Reach to use. Defaults to 'latest'")
-@click.option("--quilt-version", "-q", default="none", type=str, help="The Cosmic Quilt version to use.")
+@click.option("--quilt-version", "-q", default=None, type=str, help="The Cosmic Quilt version to use.")
 @click.option("--display-name", "-n", default=None, type=str, help="An optional display name to use for the instance.")
 @click.argument("name")
 def add(version: str, quilt_version: str, display_name: Optional[str], name: str):
     if Instance.exists(name):
         logger.error("Instance already exists.")
         exit(1)
-    instance = Instance.make_instance(name, version, None if quilt_version == "none" else quilt_version, display_name)
+    instance = Instance.make_instance(name, version, quilt_version, display_name)
     instance.download()
     logger.info("Made instance " + name)
 
 
 @cosmix.command()
 @click.option("--version", "-v", default="none", type=str, help="The version of Cosmic Reach to update to. Defaults to 'none'")
 @click.option("--quilt-version", "-q", default="none", type=str, help="The Cosmic Quilt version to update to. Defaults to 'none'")
@@ -93,14 +93,15 @@
 
 
 @cosmix.command()
 @click.argument("name")
 def trash(name: str):
     instance = Instance.get_or_throw(name)
     send2trash.send2trash(instance.path)
+    logger.info("Moved " + name + " to trash")
 
 
 @cosmix.command()
 @click.argument("name")
 def info(name: str):
     i = Instance.get_or_throw(name)
     print(i.display_name + ":")
@@ -127,23 +128,29 @@
 
     path = os.path.join(i.path, "mods")
     os.makedirs(path, exist_ok = True)
     shutil.copyfile(mod, os.path.join(path, os.path.split(mod)[-1]))
 
 
 @cosmix.command("add-crm1-mod")
+@click.option("--repo", "-r", default=None, type=str, help="Provide a CRM-1 repo to use to resolve the mod. Dependencies may still be found using default_repos.")
 @click.argument("name")
 @click.argument("mod")
-def add_crm1_mod(name: str, mod: str):
+def add_crm1_mod(repo: Optional[str], name: str, mod: str):
     i = Instance.get_or_throw(name)
 
     if not i.is_modded():
         logger.error("Instance is not modded")
         exit(1)
 
     path = os.path.join(i.path, "mods")
     os.makedirs(path, exist_ok = True)
-    net.download_crm1_mod(mod, path)
+
+    repos = config.get_config()["crm1"]["default_repos"]
+    if repo is not None:
+        repos.append(repo)
+
+    net.download_crm1_mod(mod, path, repos)
 
 
 if __name__ == "__main__":
     cosmix()
```

### Comparing `cosmix_launcher-1.0.3/src/cosmix/api/config.py` & `cosmix_launcher-1.0.4/src/cosmix/api/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,19 +23,20 @@
 
         # Colors!
         colored_logs: true
     }
 
     crm1: {
         # If JoJoJux's autorepo mapping should be used (https://crm-repo.jojojux.de/repo_mapping.json)
-        use_autorepo_mapping: true
+        use_autorepo_mapping: false
 
         # Default repos to apply
         default_repos: [
-            "https://crm-repo.jojojux.de/repo.json"
+            https://repo.crmodders.dev/repository.hjson
+            https://crm-repo.jojojux.de/repo.hjson
         ]
     }
 }"""
 _CACHED_CONFIG = None
 
 
 def get_config() -> dict:
```

### Comparing `cosmix_launcher-1.0.3/src/cosmix/api/instance.py` & `cosmix_launcher-1.0.4/src/cosmix/api/instance.py`

 * *Files identical despite different names*

### Comparing `cosmix_launcher-1.0.3/src/cosmix/api/logger.py` & `cosmix_launcher-1.0.4/src/cosmix/api/logger.py`

 * *Files identical despite different names*

### Comparing `cosmix_launcher-1.0.3/src/cosmix/api/maven.py` & `cosmix_launcher-1.0.4/src/cosmix/api/maven.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from . import logger
 import subprocess
 import os
 
 
 __all__ = (
     "QUILT_POM",
     "copy_deps",
@@ -68,14 +69,21 @@
 </project>
 """
 
 
 def copy_deps(of: str, dest: str):
     old = os.getcwd()
     os.chdir(of)
-    subprocess.run(["mvn", "dependency:copy-dependencies", "-DoutputDirectory=" + dest, "-Dsilent=true"])
+    try:
+        subprocess.run(["mvn", "dependency:copy-dependencies", "-DoutputDirectory=" + dest, "-Dsilent=true"])
+    except subprocess.CalledProcessError as error:
+        logger.error(f"Failed to run Maven goal ('{error.cmd}' with args {error.args}). Make sure that Maven is installed and in PATH.")
+        logger.error("Exit Code: " + error.returncode)
+        logger.error("Output: " + error.output)
+        logger.error("Stderr: " + error.stderr)
+        logger.error("Stdout: " + error.stdout)
     os.chdir(old)
 
 
 def make_pom(dest: str, quilt_version: str):
     with open(dest, "w") as f:
         f.write(QUILT_POM % quilt_version)
```

### Comparing `cosmix_launcher-1.0.3/src/cosmix/api/mod.py` & `cosmix_launcher-1.0.4/src/cosmix/api/mod.py`

 * *Files identical despite different names*

### Comparing `cosmix_launcher-1.0.3/src/cosmix/api/versions.py` & `cosmix_launcher-1.0.4/src/cosmix/api/versions.py`

 * *Files identical despite different names*

### Comparing `cosmix_launcher-1.0.3/pyproject.toml` & `cosmix_launcher-1.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "cosmix-launcher"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
     { name = "EmmaTheMartian", email="emmathemartian@gmail.com" },
 ]
 description = "A dead simple CLI-based launcher for Cosmic Reach and Cosmic Quilt"
 readme = "readme.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `cosmix_launcher-1.0.3/readme.md` & `cosmix_launcher-1.0.4/readme.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,43 +1,71 @@
 # Cosmix
 
 A dead simple CLI-based launcher for Cosmic Reach and Cosmic Quilt.
 
 ## Installation
 
 ```sh
-# Install from PyPI (recommended)
+# From PyPI (recommended)
 python3 -m pip install cosmix-launcher
 
-# Install from source
+# From source
 git clone https://codeberg.org/emmathemartian/cosmix && cd cosmix
 python3 -m pip install -r requirements.txt
 python3 -m build
 python3 -m pip install ./dist/*.whl
-
-# Test to make sure it's downloaded
-python3 -m cosmix version
 ```
 
-I recommend making an alias to `python3 -m cosmix`. In Zsh you can do this by adding the following to your `.zshrc`:
+I highly recommend making an alias to Cosmix so that you do not have to repeatedly type `python3 -m cosmix`.
+
+**On Linux and MacOS:**
+
+In Zsh, just append this to `~/.zshrc`:
 ```zsh
 alias cosmix="python3 -m cosmix"
 ```
 
-On windows download the cosmix.bat file and put it in ```C:\Windows\System32```
+**On Windows:**
+
+On Windows download [cosmix.bat](./cosmix.bat) and put it in `C:\Windows\System32` or somewhere else where your shell can find it.
+
+### Updating
+
+```sh
+python3 -m pip install --upgrade cosmix-launcher
+```
+
+### Uninstallation
+
+```sh
+python3 -m pip uninstall cosmix-launcher
+```
+
+### Troubleshooting
 
 **Arch Linux:**
-> Arch Linux and it's derivatives may complain with this `error: externally-managed-environment`
->
-> To get around this, use the `--user --break-system-packages` options with `pip install`
->
+
+Arch Linux and its derivatives may complain with `error: externally-managed-environment`. To get around this, use the `--user --break-system-packages` options with `pip install`.
+
 > Obviously this has a chance of breaking something, but in my testing I have yet to have that happen. Though be aware and know that I am not responsible if you break your system.
 
+**Maven:**
+
 You may also need to install Maven. On Arch Linux this is just `pacman -S maven`.
 
+> Maven is used to download and resolve all of Cosmic Quilt's dependencies automatically, hence why it is required.
+
+### Dependencies
+
+> `hjson tqdm requests crm1 Send2Trash click java-manifest`
+
+To install and/or upgrade all of them at once, just run:
+
+`python3 -m pip install --upgrade hjson tqdm requests crm1 Send2Trash click java-manifest`
+
 ## Usage
 
 ```
 cosmix version
     prints the current installed cosmix version
 
 cosmix debug
@@ -74,33 +102,37 @@
 cosmix trash [instance]
     moves an instance to the system's trash folder
 ```
 
 **Examples**
 ```sh
 # Create an unmodded instance named `vanilla` on the latest CR version
-    cosmix add vanilla
+cosmix add vanilla
 # Create a Cosmic Quilt instance named `my-quilt` on the latest CR version with Cosmic Quilt 1.2.7
-    cosmix add my-quilt --quilt-version 1.2.7
+cosmix add my-quilt --quilt-version 1.2.7
 # Create a vanilla instance named `old-version` on CR 0.0.1
-    cosmix add old-version -v 0.0.1
+cosmix add old-version -v 0.0.1
 # Install the latest version of Flux API available on JoJoJux's autorepo to the instance `test`
-    cosmix add-crm1-mod test dev.crmodders.flux
+cosmix add-crm1-mod test dev.crmodders.flux
 # Update the `latest` instance to the latest available versions of Cosmic Reach and Cosmic Quilt
-    cosmix update latest -v latest -q latest
+cosmix update latest -v latest -q latest
 ```
 
-## Folder Structure
+## File Structure
 
-Cosmix stores all of its data in your `XDG_DATA_HOME` (typically `~/.local/share/`) on Linux and `%appdata%` on Windows and in the `cosmix` folder.
+Cosmix stores all of its data in your `$XDG_DATA_HOME` (typically `~/.local/share/`) on Linux and `%appdata%` on Windows and in the `cosmix` folder.
 
 This folder will contain the following extra folders:
 ```
 cosmix/
+    config.hjson - Configs for Cosmix
+
     deps/
         cosmic-reach/
             Contains JARs for each downloaded Cosmic Reach version.
+
     instances/
         example-instance/
-            config.json  - Configs for the instance.
-    config.hjson - Configs for Cosmix
+            config.hjson - Configs for the instance.
+            deps/
+                If the instance is modded, this folder is used to store Cosmic Quilt and its dependencies.
 ```
```

### Comparing `cosmix_launcher-1.0.3/PKG-INFO` & `cosmix_launcher-1.0.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: cosmix-launcher
-Version: 1.0.3
+Version: 1.0.4
 Summary: A dead simple CLI-based launcher for Cosmic Reach and Cosmic Quilt
 Project-URL: Homepage, https://codeberg.org/EmmaTheMartian/cosmix
 Project-URL: Issues, https://codeberg.org/EmmaTheMartian/cosmix/issues
 Author-email: EmmaTheMartian <emmathemartian@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
@@ -20,43 +20,71 @@
 # Cosmix
 
 A dead simple CLI-based launcher for Cosmic Reach and Cosmic Quilt.
 
 ## Installation
 
 ```sh
-# Install from PyPI (recommended)
+# From PyPI (recommended)
 python3 -m pip install cosmix-launcher
 
-# Install from source
+# From source
 git clone https://codeberg.org/emmathemartian/cosmix && cd cosmix
 python3 -m pip install -r requirements.txt
 python3 -m build
 python3 -m pip install ./dist/*.whl
-
-# Test to make sure it's downloaded
-python3 -m cosmix version
 ```
 
-I recommend making an alias to `python3 -m cosmix`. In Zsh you can do this by adding the following to your `.zshrc`:
+I highly recommend making an alias to Cosmix so that you do not have to repeatedly type `python3 -m cosmix`.
+
+**On Linux and MacOS:**
+
+In Zsh, just append this to `~/.zshrc`:
 ```zsh
 alias cosmix="python3 -m cosmix"
 ```
 
-On windows download the cosmix.bat file and put it in ```C:\Windows\System32```
+**On Windows:**
+
+On Windows download [cosmix.bat](./cosmix.bat) and put it in `C:\Windows\System32` or somewhere else where your shell can find it.
+
+### Updating
+
+```sh
+python3 -m pip install --upgrade cosmix-launcher
+```
+
+### Uninstallation
+
+```sh
+python3 -m pip uninstall cosmix-launcher
+```
+
+### Troubleshooting
 
 **Arch Linux:**
-> Arch Linux and it's derivatives may complain with this `error: externally-managed-environment`
->
-> To get around this, use the `--user --break-system-packages` options with `pip install`
->
+
+Arch Linux and its derivatives may complain with `error: externally-managed-environment`. To get around this, use the `--user --break-system-packages` options with `pip install`.
+
 > Obviously this has a chance of breaking something, but in my testing I have yet to have that happen. Though be aware and know that I am not responsible if you break your system.
 
+**Maven:**
+
 You may also need to install Maven. On Arch Linux this is just `pacman -S maven`.
 
+> Maven is used to download and resolve all of Cosmic Quilt's dependencies automatically, hence why it is required.
+
+### Dependencies
+
+> `hjson tqdm requests crm1 Send2Trash click java-manifest`
+
+To install and/or upgrade all of them at once, just run:
+
+`python3 -m pip install --upgrade hjson tqdm requests crm1 Send2Trash click java-manifest`
+
 ## Usage
 
 ```
 cosmix version
     prints the current installed cosmix version
 
 cosmix debug
@@ -93,33 +121,37 @@
 cosmix trash [instance]
     moves an instance to the system's trash folder
 ```
 
 **Examples**
 ```sh
 # Create an unmodded instance named `vanilla` on the latest CR version
-    cosmix add vanilla
+cosmix add vanilla
 # Create a Cosmic Quilt instance named `my-quilt` on the latest CR version with Cosmic Quilt 1.2.7
-    cosmix add my-quilt --quilt-version 1.2.7
+cosmix add my-quilt --quilt-version 1.2.7
 # Create a vanilla instance named `old-version` on CR 0.0.1
-    cosmix add old-version -v 0.0.1
+cosmix add old-version -v 0.0.1
 # Install the latest version of Flux API available on JoJoJux's autorepo to the instance `test`
-    cosmix add-crm1-mod test dev.crmodders.flux
+cosmix add-crm1-mod test dev.crmodders.flux
 # Update the `latest` instance to the latest available versions of Cosmic Reach and Cosmic Quilt
-    cosmix update latest -v latest -q latest
+cosmix update latest -v latest -q latest
 ```
 
-## Folder Structure
+## File Structure
 
-Cosmix stores all of its data in your `XDG_DATA_HOME` (typically `~/.local/share/`) on Linux and `%appdata%` on Windows and in the `cosmix` folder.
+Cosmix stores all of its data in your `$XDG_DATA_HOME` (typically `~/.local/share/`) on Linux and `%appdata%` on Windows and in the `cosmix` folder.
 
 This folder will contain the following extra folders:
 ```
 cosmix/
+    config.hjson - Configs for Cosmix
+
     deps/
         cosmic-reach/
             Contains JARs for each downloaded Cosmic Reach version.
+
     instances/
         example-instance/
-            config.json  - Configs for the instance.
-    config.hjson - Configs for Cosmix
+            config.hjson - Configs for the instance.
+            deps/
+                If the instance is modded, this folder is used to store Cosmic Quilt and its dependencies.
 ```
```

