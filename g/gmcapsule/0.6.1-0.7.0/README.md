# Comparing `tmp/gmcapsule-0.6.1.tar.gz` & `tmp/gmcapsule-0.7.0.tar.gz`

## Comparing `gmcapsule-0.6.1.tar` & `gmcapsule-0.7.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 gmcapsule-0.6.1/example.ini
--rw-r--r--   0        0        0    21849 2020-02-02 00:00:00.000000 gmcapsule-0.6.1/gmcapsule/__init__.py
--rw-r--r--   0        0        0    33733 2020-02-02 00:00:00.000000 gmcapsule-0.6.1/gmcapsule/gemini.py
--rw-r--r--   0        0        0     4101 2020-02-02 00:00:00.000000 gmcapsule-0.6.1/gmcapsule/markdown.py
--rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 gmcapsule-0.6.1/gmcapsule/modules/10_rewrite.py
--rwxr-xr-x   0        0        0    18619 2020-02-02 00:00:00.000000 gmcapsule-0.6.1/gmcapsule/modules/80_gitview.py
--rw-r--r--   0        0        0     7076 2020-02-02 00:00:00.000000 gmcapsule-0.6.1/gmcapsule/modules/90_cgi.py
--rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 gmcapsule-0.6.1/gmcapsule/modules/99_static.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 gmcapsule-0.6.1/.gitignore
--rw-r--r--   0        0        0     4526 2020-02-02 00:00:00.000000 gmcapsule-0.6.1/README.md
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 gmcapsule-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     5439 2020-02-02 00:00:00.000000 gmcapsule-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 gmcapsule-0.7.0/example.ini
+-rw-r--r--   0        0        0    22038 2020-02-02 00:00:00.000000 gmcapsule-0.7.0/gmcapsule/__init__.py
+-rw-r--r--   0        0        0    34269 2020-02-02 00:00:00.000000 gmcapsule-0.7.0/gmcapsule/gemini.py
+-rw-r--r--   0        0        0     4101 2020-02-02 00:00:00.000000 gmcapsule-0.7.0/gmcapsule/markdown.py
+-rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 gmcapsule-0.7.0/gmcapsule/modules/10_rewrite.py
+-rwxr-xr-x   0        0        0    18619 2020-02-02 00:00:00.000000 gmcapsule-0.7.0/gmcapsule/modules/80_gitview.py
+-rw-r--r--   0        0        0     8017 2020-02-02 00:00:00.000000 gmcapsule-0.7.0/gmcapsule/modules/90_cgi.py
+-rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 gmcapsule-0.7.0/gmcapsule/modules/99_static.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 gmcapsule-0.7.0/.gitignore
+-rw-r--r--   0        0        0     5360 2020-02-02 00:00:00.000000 gmcapsule-0.7.0/README.md
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 gmcapsule-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     6273 2020-02-02 00:00:00.000000 gmcapsule-0.7.0/PKG-INFO
```

### Comparing `gmcapsule-0.6.1/example.ini` & `gmcapsule-0.7.0/example.ini`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ; By default, configuration is read from ~/.gmcapsulerc. Use the -c option
 ; to specify some other configuration file.
 
 [server]
-;host = localhost
+host = localhost 127.0.0.1
 ;address = 0.0.0.0
 ;port = 1965
 ;certs = .certs
 ;modules = 
 ;threads = 5
 ;processes = 2
 
@@ -22,15 +22,15 @@
 [cgi.booster]
 protocol        = titan
 host            = localhost
 path            = /gemlog/* /plan.gmi
 command         = /usr/bin/python3 ../booster/booster.py
 
 [cgi.printenv]
-path            = /cgienv
+path            = /cgienv*
 command         = printenv
 
 [rewrite.test]
 path = ^/altenv$
 status = 30 gemini://localhost/cgienv${QUERY_STRING}
 
 ;--------------------------------------------------------------------------
```

### Comparing `gmcapsule-0.6.1/gmcapsule/__init__.py` & `gmcapsule-0.7.0/gmcapsule/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 GmCapsule is an extensible Gemini/Titan server.
 
 Extensibility is achieved with Python modules that get loaded at launch
 from the configured directories. A set of built-in extension modules is
 provided for common functionality like CGI and for serving static files.
 
-The supported protocols are `Gemini <https://gemini.circumlunar.space>`_ and
+The supported protocols are `Gemini <https://geminiprotocol.net>`_ and
 `Titan <https://transjovian.org/titan>`_. Both are accepted via the same
 TCP port.
 
 GmCapsule can be used in a few different ways:
 
 - You can run it as-is for serving static files.
 - You can use CGI programs to generate dynamic content and/or process
@@ -206,14 +206,18 @@
         bin_root = /home/user/gemini/cgi-bin
 
     An executable at `/home/user/gemini/cgi-bin/example.com/action` would then
     be visible at gemini://example.com/action. If the executable name ends
     with ``,titan`` (note: a comma), the entrypoint will use the Titan
     protocol instead of Gemini. The ``,titan`` suffix is omitted from the URL.
 
+    Executable files named `index.gmi` are assumed to be directory indices, so
+    a request for the directory `DIR` will check for `DIR/index.gmi` and use
+    it for generating the index page.
+
 
 cgi.*
 -----
 
 Each section whose name begins with ``cgi.`` is used for setting up CGI entry
 points for the `cgi` module. For example, this registers
 ``gemini://example.com/listing`` to show the output of ``/bin/ls -l``:
@@ -498,15 +502,15 @@
 import subprocess
 from pathlib import Path
 
 from .gemini import Server, Cache, Context, Identity
 from .markdown import to_gemtext as markdown_to_gemtext
 
 
-__version__ = '0.6.1'
+__version__ = '0.7.0'
 __all__ = [
     'Config', 'Cache', 'Context', 'Identity',
     'get_mime_type', 'markdown_to_gemtext'
 ]
 
 
 class Config:
```

### Comparing `gmcapsule-0.6.1/gmcapsule/gemini.py` & `gmcapsule-0.7.0/gmcapsule/gemini.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import fnmatch
 import hashlib
 import importlib
 import os.path
 import select
 import socket
+import ipaddress
 import multiprocessing as mp
 import subprocess
 import threading
 import queue
 import re
 import signal
 import time
@@ -377,20 +378,31 @@
         path = '/'
     hostname = url.hostname
 
     if url.port != None and url.port != worker.port:
         report_error(stream, 59, "Invalid port number")
         return
     if not stream.get_servername():
-        # Server name indication is required.
-        report_error(stream, 59, "Missing TLS server name indication")
-        return
-    if stream.get_servername().decode() != hostname:
-        report_error(stream, 53, "Proxy request refused")
-        return
+        # The hostname may be a literal IPv4/IPv6 address.
+        try:
+            ipaddress.ip_address(hostname)
+            # No error during parsing, looks like a literal address.
+        except ValueError:
+            # Server name indication is required.
+            report_error(stream, 59, "Missing TLS server name indication")
+            return
+    else:
+        sni_name = stream.get_servername().decode()
+        if sni_name != hostname:
+            # SNI servername does not match the hostname in the URL. Misbehaving client?
+            report_error(stream, 53, "Proxy request refused")
+            return
+        if sni_name not in worker.cfg.hostnames():
+            report_error(stream, 53, f"Proxy request refused (domain \"{sni_name}\")")
+            return
 
     try:
         status, meta, body, from_cache = worker.context.call_entrypoint(Request(
             identity,
             remote_address=from_addr,
             scheme=url.scheme,
             hostname=hostname,
```

### Comparing `gmcapsule-0.6.1/gmcapsule/markdown.py` & `gmcapsule-0.7.0/gmcapsule/markdown.py`

 * *Files identical despite different names*

### Comparing `gmcapsule-0.6.1/gmcapsule/modules/10_rewrite.py` & `gmcapsule-0.7.0/gmcapsule/modules/10_rewrite.py`

 * *Files identical despite different names*

### Comparing `gmcapsule-0.6.1/gmcapsule/modules/80_gitview.py` & `gmcapsule-0.7.0/gmcapsule/modules/80_gitview.py`

 * *Files identical despite different names*

### Comparing `gmcapsule-0.6.1/gmcapsule/modules/90_cgi.py` & `gmcapsule-0.7.0/gmcapsule/modules/90_cgi.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,29 +13,33 @@
 
 
 class CgiContext:
     def __init__(self, port, url_path, args, work_dir=None, is_streaming=False):
         self.port = port
         self.args = args
         self.base_path = url_path
-        if self.base_path.endswith('/*'):
-            self.base_path = self.base_path[:-2]
+        if self.base_path.endswith('*'):
+            self.base_path = self.base_path[:-1]
         self.work_dir = work_dir
         self.is_streaming = is_streaming
 
     def __call__(self, req):
         try:
             env_vars = dict(os.environ)
 
             # Standard CGI variables.
             env_vars['GATEWAY_INTERFACE'] = 'CGI/1.1'
             env_vars['REMOTE_ADDR'] = '%s:%d' % req.remote_address
             if req.query != None:
                 env_vars['QUERY_STRING'] = req.query
-            env_vars['PATH_INFO'] = req.path
+            # PATH_INFO contains any additional subdirectories deeper than the script location.
+            path_info = urllib.parse.unquote(req.path)
+            if path_info.startswith(self.base_path):
+                path_info = path_info[len(self.base_path):]
+            env_vars['PATH_INFO'] = path_info
             env_vars['SCRIPT_NAME'] = self.base_path
             env_vars['SERVER_SOFTWARE'] = 'GmCapsule/' + gmcapsule.__version__
             env_vars['SERVER_PROTOCOL'] = req.scheme.upper()
             env_vars['SERVER_NAME'] = req.hostname
             env_vars['SERVER_PORT'] = str(self.port)
             env_vars[req.scheme.upper() + '_URL'] = f"{req.scheme}://{req.hostname}{req.path}" + (
                 '?' + req.query if req.query != None else '')
@@ -106,21 +110,33 @@
         self.host = host
         self.port = port
         self.root_dir = pathlib.Path(root_dir)
 
     def __call__(self, url_path):
         # Check if url_path is a valid CGI entrypoint and return
         # a CgiContext for it.
-        fn = str(self.root_dir) + url_path
+        root_dir = str(self.root_dir)
+        fn = root_dir + url_path
         if self.protocol == 'titan':
             fn += ',titan'
-        if os.path.isdir(fn):
-            return None
-        if os.access(fn, os.X_OK):
-            return CgiContext(self.port, url_path, [fn], work_dir=os.path.dirname(fn))
+        # Look for an executable up the path.
+        par_path = fn
+        par_url = url_path
+        while len(par_path) > len(root_dir):
+            # An executable 'index.gmi' is used for generating the index page.
+            if os.path.isdir(par_path):
+                if os.access(os.path.join(par_path, 'index.gmi'), os.X_OK):
+                    return CgiContext(self.port, par_url + '*', [os.path.join(par_path, 'index.gmi')],
+                                                                 work_dir=par_path)
+                else:
+                    return None
+            if os.access(par_path, os.X_OK):
+                return CgiContext(self.port, par_url + '*', [par_path], work_dir=os.path.dirname(par_path))
+            par_path = os.path.dirname(par_path)
+            par_url = os.path.dirname(par_url)
         return None
 
 
 # # NOTE: This require restarting the server when binaries are added/removed.
 # def add_cgibin_entrypoints_recursively(context, host, base, cur_dir=None):
 #     if cur_dir is None:
 #         cur_dir = base
```

### Comparing `gmcapsule-0.6.1/gmcapsule/modules/99_static.py` & `gmcapsule-0.7.0/gmcapsule/modules/99_static.py`

 * *Files identical despite different names*

### Comparing `gmcapsule-0.6.1/README.md` & `gmcapsule-0.7.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -43,19 +43,32 @@
 
 The log can be viewed via journalctl (or syslog):
 
     journalctl -xe --user-unit=gmcapsule
 
 ## Change log
 
+### v0.7
+
+* CGI: Fixed contents of `PATH_INFO`: it is now URL-decoded and the script path is removed so only the part following the script path is included in the environment variable (RFC 3875, section 4.1.5).
+* CGI: `bin_root` applies a wildcard to all found CGI executables so `PATH_INFO` can be used.
+* CGI: `bin_root` looks for executable "index.gmi" files in requested directories to provide the directory index.
+* Skip the TLS SNI check when request hostname has a literal IP address. (SNI is not supposed to be used with literal addresses.)
+* Respond with status 53 if an unknown hostname is requested. This helps reveal configuration errors where the correct hostnames are not specified.
+
 ### v0.6
 
 * Added `stream` to the `[cgi.*]` section to enable streaming output mode where the output of the CGI child process is immediately sent to the client without any buffering. Streaming is not supported if the server is using multiple processes.
 * Markdown: Fixed handling of alt text in preformatted blocks (patch by Mike Cifelli).
 
+v0.6.1:
+
+* Static: Fixed unquoting URL paths when looking up files.
+* Added example of printing Gemini meta line in CGI documentation.
+
 ### v0.5
 
 * Added `processes` to the `[server]` section to configure how many request handler processes are started.
 * Extension modules can register new protocols in addition to the built-in Gemini and Titan.
 * SIGHUP causes the configuration file to be reloaded and workers to be restarted. The listening socket remains open, so the socket and TLS parameters cannot be changed.
 * API change: Extension modules get initialized separately in each worker thread. Instead of a `Capsule`, the extension module `init` method is passed a `Context`. `Capsule` is no longer available as global state.
 * API change: `Identity` no longer contains OpenSSL objects for the certificate and public key. Instead, they are provided as serialized in DER format.
```

### Comparing `gmcapsule-0.6.1/pyproject.toml` & `gmcapsule-0.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gmcapsule-0.6.1/PKG-INFO` & `gmcapsule-0.7.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmcapsule
-Version: 0.6.1
+Version: 0.7.0
 Summary: Extensible Gemini/Titan server
 Project-URL: Home-page, https://geminispace.org/gmcapsule/
 Project-URL: Documentation, https://geminispace.org/gmcapsule/gmcapsule.html
 Project-URL: Source, https://codeberg.org/skyjake/gmcapsule
 Project-URL: Issues, https://codeberg.org/skyjake/gmcapsule/issues
 Author-email: Jaakko Keränen <jaakko.keranen@iki.fi>
 Keywords: gemini,internet,server,titan
@@ -65,19 +65,32 @@
 
 The log can be viewed via journalctl (or syslog):
 
     journalctl -xe --user-unit=gmcapsule
 
 ## Change log
 
+### v0.7
+
+* CGI: Fixed contents of `PATH_INFO`: it is now URL-decoded and the script path is removed so only the part following the script path is included in the environment variable (RFC 3875, section 4.1.5).
+* CGI: `bin_root` applies a wildcard to all found CGI executables so `PATH_INFO` can be used.
+* CGI: `bin_root` looks for executable "index.gmi" files in requested directories to provide the directory index.
+* Skip the TLS SNI check when request hostname has a literal IP address. (SNI is not supposed to be used with literal addresses.)
+* Respond with status 53 if an unknown hostname is requested. This helps reveal configuration errors where the correct hostnames are not specified.
+
 ### v0.6
 
 * Added `stream` to the `[cgi.*]` section to enable streaming output mode where the output of the CGI child process is immediately sent to the client without any buffering. Streaming is not supported if the server is using multiple processes.
 * Markdown: Fixed handling of alt text in preformatted blocks (patch by Mike Cifelli).
 
+v0.6.1:
+
+* Static: Fixed unquoting URL paths when looking up files.
+* Added example of printing Gemini meta line in CGI documentation.
+
 ### v0.5
 
 * Added `processes` to the `[server]` section to configure how many request handler processes are started.
 * Extension modules can register new protocols in addition to the built-in Gemini and Titan.
 * SIGHUP causes the configuration file to be reloaded and workers to be restarted. The listening socket remains open, so the socket and TLS parameters cannot be changed.
 * API change: Extension modules get initialized separately in each worker thread. Instead of a `Capsule`, the extension module `init` method is passed a `Context`. `Capsule` is no longer available as global state.
 * API change: `Identity` no longer contains OpenSSL objects for the certificate and public key. Instead, they are provided as serialized in DER format.
```

