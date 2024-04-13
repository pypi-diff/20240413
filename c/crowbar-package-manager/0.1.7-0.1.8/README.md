# Comparing `tmp/crowbar_package_manager-0.1.7.tar.gz` & `tmp/crowbar_package_manager-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crowbar_package_manager-0.1.7.tar", last modified: Wed Apr 10 00:16:14 2024, max compression
+gzip compressed data, was "crowbar_package_manager-0.1.8.tar", last modified: Sat Apr 13 00:20:41 2024, max compression
```

## Comparing `crowbar_package_manager-0.1.7.tar` & `crowbar_package_manager-0.1.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 coryfitz   (501) staff       (20)        0 2024-04-10 00:16:14.046063 crowbar_package_manager-0.1.7/
--rw-r--r--   0 coryfitz   (501) staff       (20)     1075 2024-04-10 00:16:14.045911 crowbar_package_manager-0.1.7/PKG-INFO
--rw-r--r--   0 coryfitz   (501) staff       (20)      896 2024-04-09 23:41:35.000000 crowbar_package_manager-0.1.7/README.md
-drwxr-xr-x   0 coryfitz   (501) staff       (20)        0 2024-04-10 00:16:14.044839 crowbar_package_manager-0.1.7/crowbar/
--rw-r--r--   0 coryfitz   (501) staff       (20)       25 2024-04-07 23:29:44.000000 crowbar_package_manager-0.1.7/crowbar/__init__.py
--rw-r--r--   0 coryfitz   (501) staff       (20)     7210 2024-04-09 23:19:15.000000 crowbar_package_manager-0.1.7/crowbar/crowbar.py
-drwxr-xr-x   0 coryfitz   (501) staff       (20)        0 2024-04-10 00:16:14.045693 crowbar_package_manager-0.1.7/crowbar_package_manager.egg-info/
--rw-r--r--   0 coryfitz   (501) staff       (20)     1075 2024-04-10 00:16:14.000000 crowbar_package_manager-0.1.7/crowbar_package_manager.egg-info/PKG-INFO
--rw-r--r--   0 coryfitz   (501) staff       (20)      295 2024-04-10 00:16:14.000000 crowbar_package_manager-0.1.7/crowbar_package_manager.egg-info/SOURCES.txt
--rw-r--r--   0 coryfitz   (501) staff       (20)        1 2024-04-10 00:16:14.000000 crowbar_package_manager-0.1.7/crowbar_package_manager.egg-info/dependency_links.txt
--rw-r--r--   0 coryfitz   (501) staff       (20)       59 2024-04-10 00:16:14.000000 crowbar_package_manager-0.1.7/crowbar_package_manager.egg-info/entry_points.txt
--rw-r--r--   0 coryfitz   (501) staff       (20)        8 2024-04-10 00:16:14.000000 crowbar_package_manager-0.1.7/crowbar_package_manager.egg-info/top_level.txt
--rw-r--r--   0 coryfitz   (501) staff       (20)       38 2024-04-10 00:16:14.046131 crowbar_package_manager-0.1.7/setup.cfg
--rw-r--r--   0 coryfitz   (501) staff       (20)      731 2024-04-10 00:16:05.000000 crowbar_package_manager-0.1.7/setup.py
+drwxr-xr-x   0 coryfitz   (501) staff       (20)        0 2024-04-13 00:20:41.260911 crowbar_package_manager-0.1.8/
+-rw-r--r--   0 coryfitz   (501) staff       (20)     1281 2024-04-13 00:20:41.260763 crowbar_package_manager-0.1.8/PKG-INFO
+-rw-r--r--   0 coryfitz   (501) staff       (20)     1102 2024-04-13 00:19:40.000000 crowbar_package_manager-0.1.8/README.md
+drwxr-xr-x   0 coryfitz   (501) staff       (20)        0 2024-04-13 00:20:41.259486 crowbar_package_manager-0.1.8/crowbar/
+-rw-r--r--   0 coryfitz   (501) staff       (20)       25 2024-04-07 23:29:44.000000 crowbar_package_manager-0.1.8/crowbar/__init__.py
+-rw-r--r--   0 coryfitz   (501) staff       (20)     8976 2024-04-13 00:14:00.000000 crowbar_package_manager-0.1.8/crowbar/crowbar.py
+drwxr-xr-x   0 coryfitz   (501) staff       (20)        0 2024-04-13 00:20:41.260520 crowbar_package_manager-0.1.8/crowbar_package_manager.egg-info/
+-rw-r--r--   0 coryfitz   (501) staff       (20)     1281 2024-04-13 00:20:41.000000 crowbar_package_manager-0.1.8/crowbar_package_manager.egg-info/PKG-INFO
+-rw-r--r--   0 coryfitz   (501) staff       (20)      295 2024-04-13 00:20:41.000000 crowbar_package_manager-0.1.8/crowbar_package_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 coryfitz   (501) staff       (20)        1 2024-04-13 00:20:41.000000 crowbar_package_manager-0.1.8/crowbar_package_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 coryfitz   (501) staff       (20)       59 2024-04-13 00:20:41.000000 crowbar_package_manager-0.1.8/crowbar_package_manager.egg-info/entry_points.txt
+-rw-r--r--   0 coryfitz   (501) staff       (20)        8 2024-04-13 00:20:41.000000 crowbar_package_manager-0.1.8/crowbar_package_manager.egg-info/top_level.txt
+-rw-r--r--   0 coryfitz   (501) staff       (20)       38 2024-04-13 00:20:41.260979 crowbar_package_manager-0.1.8/setup.cfg
+-rw-r--r--   0 coryfitz   (501) staff       (20)      653 2024-04-13 00:20:26.000000 crowbar_package_manager-0.1.8/setup.py
```

### Comparing `crowbar_package_manager-0.1.7/PKG-INFO` & `crowbar_package_manager-0.1.8/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,43 @@
-Metadata-Version: 2.1
-Name: crowbar_package_manager
-Version: 0.1.7
-Summary: a local-first tool for managing python dependencies with pip
-Description-Content-Type: text/markdown
-
 ## crowbar
 
 Note: any instance of ```crowbar``` can be replaced with ```cb```
 
 
 ```
-crowbar install <package_name>
+crowbar install <package_name> <package_name>
 ```
 -Creates a virtual environment called venv if it does not exist<br>
--Installs a package from pypi into venv<br>
+-Installs a package (or packages) from pypi into venv<br>
 -Updates requirements.txt and creates one if it does not exist
 
 ```
-crowbar uninstall <package_name>
+crowbar uninstall <package_name> <package_name>
 ```
--Uninstalls a package from venv
+-Uninstalls a package (or packages) from venv
 -Updates requirements.txt
 
 ```
 crowbar install
 ```
 -Installs all packages listed in requirements.txt
 
 ```
 crowbar run <file_name>.py
 ```
 -Runs a python file using the contents of the local venv
 
 Warning – you may have pip muscle memory which may cause you to accidentally install globally. Use crowbar/cb and not pip if you are not in an active virtual environment.
 
+### global flag
+
+```
+crowbar --global install <package_name>
+```
+```
+cb -g uninstall <package_name>
+```
+-installs or uninstalls a package globally
+
 ### conda support
 
-Crowbar supports python and will create an environment called conda_env instead of venv if it detects that it is within a conda environment.
+Crowbar supports python and will create an environment called conda_env instead of venv if it detects that it is within a conda environment.
```

### Comparing `crowbar_package_manager-0.1.7/README.md` & `crowbar_package_manager-0.1.8/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,49 @@
+Metadata-Version: 2.1
+Name: crowbar_package_manager
+Version: 0.1.8
+Summary: a local-first tool for managing python dependencies with pip
+Description-Content-Type: text/markdown
+
 ## crowbar
 
 Note: any instance of ```crowbar``` can be replaced with ```cb```
 
 
 ```
-crowbar install <package_name>
+crowbar install <package_name> <package_name>
 ```
 -Creates a virtual environment called venv if it does not exist<br>
--Installs a package from pypi into venv<br>
+-Installs a package (or packages) from pypi into venv<br>
 -Updates requirements.txt and creates one if it does not exist
 
 ```
-crowbar uninstall <package_name>
+crowbar uninstall <package_name> <package_name>
 ```
--Uninstalls a package from venv
+-Uninstalls a package (or packages) from venv
 -Updates requirements.txt
 
 ```
 crowbar install
 ```
 -Installs all packages listed in requirements.txt
 
 ```
 crowbar run <file_name>.py
 ```
 -Runs a python file using the contents of the local venv
 
 Warning – you may have pip muscle memory which may cause you to accidentally install globally. Use crowbar/cb and not pip if you are not in an active virtual environment.
 
+### global flag
+
+```
+crowbar --global install <package_name>
+```
+```
+cb -g uninstall <package_name>
+```
+-installs or uninstalls a package globally
+
 ### conda support
 
-Crowbar supports python and will create an environment called conda_env instead of venv if it detects that it is within a conda environment.
+Crowbar supports python and will create an environment called conda_env instead of venv if it detects that it is within a conda environment.
```

### Comparing `crowbar_package_manager-0.1.7/crowbar/crowbar.py` & `crowbar_package_manager-0.1.8/crowbar/crowbar.py`

 * *Files 27% similar despite different names*

```diff
@@ -15,31 +15,38 @@
     elif 'CONDA_PREFIX' in os.environ:
         # Construct a path to conda based on the active environment
         conda_executable = os.path.join(os.environ['CONDA_PREFIX'], 'condabin', 'conda')
     return conda_executable
 
 def parse_arguments():
     parser = argparse.ArgumentParser(description='Crowbar Package Manager')
+    
+    # Define the global option at the main parser level
+    parser.add_argument('-g', '--global', action='store_true', help='Operate on the global Python environment instead of a virtual environment')
+
     subparsers = parser.add_subparsers(dest='command', required=True)
 
     # Parser for the install command
     install_parser = subparsers.add_parser('install', help='Install packages')
-    # Make package_name optional for the install command
-    install_parser.add_argument('package_name', nargs='?', default=None, help='Name of the package to install (optional). If omitted, installs from requirements.txt')
+    # Allow multiple package names, including zero for installing from requirements.txt
+    install_parser.add_argument('packages', nargs='*', help='Name(s) of package(s) to install (optional). If omitted, installs from requirements.txt')
 
     # Parser for the uninstall command
-    uninstall_parser = subparsers.add_parser('uninstall', help='Uninstall a package')
-    uninstall_parser.add_argument('package_name', help='Name of the package to uninstall')
+    uninstall_parser = subparsers.add_parser('uninstall', help='Uninstall packages')
+    # Allow multiple package names
+    uninstall_parser.add_argument('packages', nargs='+', help='Name(s) of package(s) to uninstall')
+
 
     # Parser for the run command
     run_parser = subparsers.add_parser('run', help='Run a Python script')
     run_parser.add_argument('file_name', help='Name of the Python file to run')
 
     return parser.parse_args()
 
+
 def create_conda_environment(env_name):
         conda_prefix = os.environ['CONDA_PREFIX']
         # Construct the command to create a new Conda environment
         command = f"{os.path.join(conda_prefix, 'condabin', 'conda')} create --name {env_name} --yes"
         subprocess.run(command, shell=True)
 
 def create_env_if_not_exists():
@@ -48,36 +55,41 @@
     if is_conda_environment():
         # Check if the Conda environment already exists
         conda_executable = get_conda_executable()
         check_env = subprocess.run([conda_executable, 'env', 'list'], capture_output=True, text=True)
         if env_name not in check_env.stdout:
             print(f"Creating Conda environment named {env_name}...")
             subprocess.run([conda_executable, 'create', '--name', env_name, '--yes'], check=True)
-        else:
-            print(f"Conda environment named {env_name} already exists.")
     else:
         if not os.path.isdir(env_name):
             print(f"Creating environment named {env_name}...")
             subprocess.run([sys.executable, '-m', 'venv', env_name], check=True)
-        else:
-            print(f"Environment named {env_name} already exists.")
     
     return env_name
 
-def uninstall_package(env_name, package_name):
-    if is_conda_environment():
-        conda_executable = get_conda_executable()
-        # Uninstall a package with Conda
-        print(f"Uninstalling {package_name} from Conda environment {env_name}...")
-        subprocess.run([conda_executable, 'remove', '--name', env_name, package_name, '--yes'], check=True)
+def uninstall_package(env_name, packages, global_uninstall=False):
+    if global_uninstall:
+        pip_path = 'pip'  # Use the globally available pip command
+        for package_name in packages:
+            print(f"Uninstalling {package_name} globally...")
+            subprocess.run([pip_path, 'uninstall', package_name, '-y'], check=True)
     else:
-        pip_path = os.path.join(env_name, 'Scripts', 'pip') if os.name == 'nt' else os.path.join(env_name, 'bin', 'pip')
-        # Uninstall a package with pip
-        print(f"Uninstalling {package_name} from environment {env_name}...")
-        subprocess.run([pip_path, 'uninstall', package_name, '-y'], check=True)  # The '-y' flag auto-confirms uninstallation
+        if is_conda_environment():
+            conda_executable = get_conda_executable()
+            for package_name in packages:
+                # Uninstall a package with Conda
+                print(f"Uninstalling {package_name} from Conda environment {env_name}...")
+                subprocess.run([conda_executable, 'remove', '--name', env_name, package_name, '--yes'], check=True)
+        else:
+            pip_path = os.path.join(env_name, 'Scripts' if os.name == 'nt' else 'bin', 'pip')
+            for package_name in packages:
+                # Uninstall a package with pip
+                print(f"Uninstalling {package_name} from environment {env_name}...")
+                subprocess.run([pip_path, 'uninstall', package_name, '-y'], check=True)  # The '-y' flag auto-confirms uninstallation
+
 
 def run_python_script(env_name, script_name):
     if not os.path.isfile(script_name):
         print(f"Error: The file {script_name} does not exist.")
         sys.exit(1)
     
     # Determine the correct path for the Python executable
@@ -91,65 +103,89 @@
     if not os.path.exists(python_executable):
         print(f"Error: Python executable not found at {python_executable}.")
         sys.exit(1)
     
     print(f"Running {script_name} using {python_executable}...")
     subprocess.run([python_executable, script_name])
 
-def install_packages(env_name, package_name=None):
-    if is_conda_environment():
-        conda_executable = get_conda_executable()
-        if package_name:
-            subprocess.run([conda_executable, 'install', '--name', env_name, package_name, '--yes'], check=True)
+def install_packages(env_name, packages=None, global_install=False):
+    if global_install:
+        pip_path = 'pip'  # Use the globally available pip command
+        if packages:
+            subprocess.run([pip_path, 'install'] + packages, check=True)
         else:
-            requirements_path = os.path.join(os.getcwd(), 'requirements.txt')
-            if os.path.exists(requirements_path):
-                subprocess.run([conda_executable, 'install', '--name', env_name, '--file', requirements_path, '--yes'], check=True)
-            else:
-                print("requirements.txt not found.")
+            print("No packages to install globally.")
     else:
-        pip_path = os.path.join(env_name, 'Scripts', 'pip') if os.name == 'nt' else os.path.join(env_name, 'bin', 'pip')
-        if package_name:
-            subprocess.run([pip_path, 'install', package_name], check=True)
+        if is_conda_environment():
+            conda_executable = get_conda_executable()
+            if packages:
+                # Install multiple specified packages with Conda
+                subprocess.run([conda_executable, 'install', '--name', env_name] + packages + ['--yes'], check=True)
+            else:
+                # Install all packages from requirements.txt with Conda
+                requirements_path = os.path.join(os.getcwd(), 'requirements.txt')
+                if os.path.exists(requirements_path):
+                    subprocess.run([conda_executable, 'install', '--name', env_name, '--file', requirements_path, '--yes'], check=True)
+                else:
+                    print("requirements.txt not found.")
         else:
-            requirements_path = os.path.join(os.getcwd(), 'requirements.txt')
-            if os.path.exists(requirements_path):
-                subprocess.run([pip_path, 'install', '-r', requirements_path], check=True)
+            pip_path = os.path.join(env_name, 'Scripts' if os.name == 'nt' else 'bin', 'pip')
+            if packages:
+                # Install multiple specified packages with pip
+                subprocess.run([pip_path, 'install'] + packages, check=True)
             else:
-                print("requirements.txt not found.")
+                # Install all packages from requirements.txt with pip
+                requirements_path = os.path.join(os.getcwd(), 'requirements.txt')
+                if os.path.exists(requirements_path):
+                    subprocess.run([pip_path, 'install', '-r', requirements_path], check=True)
+                else:
+                    print("requirements.txt not found.")
+
 
 def update_requirements(env_name):
     if is_conda_environment():
         conda_executable = get_conda_executable()
         # Using conda list to export the package list, which is not directly equivalent to pip freeze
         subprocess.run([conda_executable, 'list', '--name', env_name, '--export'], stdout=open('requirements.txt', 'w'), check=True)
     else:
         pip_path = os.path.join(env_name, 'Scripts', 'pip') if os.name == 'nt' else os.path.join(env_name, 'bin', 'pip')
         subprocess.run([pip_path, 'freeze'], stdout=open('requirements.txt', 'w'), check=True)
 
 def main():
     args = parse_arguments()
     
-    venv_path = create_env_if_not_exists()
-    
-    if args.command == 'install':
-        if args.package_name:
-            print(f"Installing {args.package_name}...")
-            install_packages(venv_path, args.package_name)
-            update_requirements(venv_path)  # Update requirements after installing a specific package
+    global_operation = getattr(args, 'global', False)  # Safe way to get 'global' attribute with a default value
+    if global_operation:
+        # Handle global installation or uninstallation
+        if args.command == 'install':
+            print(f"Installing packages globally: {' '.join(args.packages)}")
+            install_packages(None, args.packages, global_install=True)
+        elif args.command == 'uninstall':
+            print(f"Uninstalling packages globally: {' '.join(args.packages)}")
+            uninstall_package(None, args.packages, global_uninstall=True)
         else:
-            print("Installing packages from requirements.txt...")
-            install_packages(venv_path)
-            # No call to update_requirements here, as we're installing from it
-    elif args.command == 'uninstall':
-        print(f"Uninstalling {args.package_name}...")
-        uninstall_package(venv_path, args.package_name)
-        update_requirements(venv_path)  # Update requirements after uninstallation
-    elif args.command == 'run':
-        print(f"Running {args.file_name}...")
-        run_python_script(venv_path, args.file_name)
+            print("Unknown command.")
+            sys.exit(1)
     else:
-        print("Unknown command.")
-        sys.exit(1)
+    
+        venv_path = create_env_if_not_exists()
+        
+        if args.command == 'install':
+            if args.packages:
+                print(f"Installing packages: {' '.join(args.packages)}")
+                install_packages(venv_path, args.packages)
+                update_requirements(venv_path)  # This will overwrite requirements.txt with the new environment state
+            else:
+                print("Installing packages from requirements.txt...")
+                install_packages(venv_path)
+        if args.command == 'uninstall':
+            print(f"Uninstalling packages: {' '.join(args.packages)}")
+            uninstall_package(venv_path, args.packages)
+            update_requirements(venv_path)  # Update requirements after uninstallation
+        elif args.command == 'run':
+            print(f"Running {args.file_name}...")
+            run_python_script(venv_path, args.file_name)
+        else:
+            sys.exit(1)
 
 if __name__ == "__main__":
     main()
```

### Comparing `crowbar_package_manager-0.1.7/crowbar_package_manager.egg-info/PKG-INFO` & `crowbar_package_manager-0.1.8/crowbar_package_manager.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,49 @@
 Metadata-Version: 2.1
 Name: crowbar-package-manager
-Version: 0.1.7
+Version: 0.1.8
 Summary: a local-first tool for managing python dependencies with pip
 Description-Content-Type: text/markdown
 
 ## crowbar
 
 Note: any instance of ```crowbar``` can be replaced with ```cb```
 
 
 ```
-crowbar install <package_name>
+crowbar install <package_name> <package_name>
 ```
 -Creates a virtual environment called venv if it does not exist<br>
--Installs a package from pypi into venv<br>
+-Installs a package (or packages) from pypi into venv<br>
 -Updates requirements.txt and creates one if it does not exist
 
 ```
-crowbar uninstall <package_name>
+crowbar uninstall <package_name> <package_name>
 ```
--Uninstalls a package from venv
+-Uninstalls a package (or packages) from venv
 -Updates requirements.txt
 
 ```
 crowbar install
 ```
 -Installs all packages listed in requirements.txt
 
 ```
 crowbar run <file_name>.py
 ```
 -Runs a python file using the contents of the local venv
 
 Warning – you may have pip muscle memory which may cause you to accidentally install globally. Use crowbar/cb and not pip if you are not in an active virtual environment.
 
+### global flag
+
+```
+crowbar --global install <package_name>
+```
+```
+cb -g uninstall <package_name>
+```
+-installs or uninstalls a package globally
+
 ### conda support
 
 Crowbar supports python and will create an environment called conda_env instead of venv if it detects that it is within a conda environment.
```

### Comparing `crowbar_package_manager-0.1.7/setup.py` & `crowbar_package_manager-0.1.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,21 +2,20 @@
 
 # Read the contents of your README file
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='crowbar_package_manager',
-    version='0.1.7',
+    version='0.1.8',
     packages=find_packages(),
     install_requires=[],
     entry_points={
         'console_scripts': [
             'crowbar=crowbar:main',
             'cb=crowbar:main',
         ],
     },
-    summary = 'a local-first tool for managing python dependencies with pip',
     description = 'a local-first tool for managing python dependencies with pip',
     long_description=long_description,
     long_description_content_type='text/markdown',  # This line is important for Markdown rendering on PyPI
 )
```

