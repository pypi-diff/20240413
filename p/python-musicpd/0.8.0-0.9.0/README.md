# Comparing `tmp/python-musicpd-0.8.0.tar.gz` & `tmp/python-musicpd-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-musicpd-0.8.0.tar", last modified: Sat May  7 16:50:27 2022, max compression
+gzip compressed data, was "python-musicpd-0.9.0.tar", last modified: Sat Apr 13 07:20:11 2024, max compression
```

## Comparing `python-musicpd-0.8.0.tar` & `python-musicpd-0.9.0.tar`

### file list

```diff
@@ -1,23 +1,32 @@
-drwxr-xr-x   0 gberret   (1000) gberret   (1000)        0 2022-05-07 16:50:27.378124 python-musicpd-0.8.0/
--rw-r--r--   0 gberret   (1000) gberret   (1000)     3344 2022-05-07 15:01:21.000000 python-musicpd-0.8.0/CHANGES.txt
--rw-r--r--   0 gberret   (1000) gberret   (1000)     7651 2017-02-13 09:25:48.000000 python-musicpd-0.8.0/LICENSE.txt
--rw-r--r--   0 gberret   (1000) gberret   (1000)       51 2020-12-30 10:08:36.000000 python-musicpd-0.8.0/MANIFEST.in
--rw-r--r--   0 gberret   (1000) gberret   (1000)     1339 2022-05-07 16:50:27.378124 python-musicpd-0.8.0/PKG-INFO
--rw-r--r--   0 gberret   (1000) gberret   (1000)      407 2022-02-08 15:29:57.000000 python-musicpd-0.8.0/README.rst
-drwxr-xr-x   0 gberret   (1000) gberret   (1000)        0 2022-05-07 16:50:27.378124 python-musicpd-0.8.0/doc/
-drwxr-xr-x   0 gberret   (1000) gberret   (1000)        0 2022-05-07 16:50:27.378124 python-musicpd-0.8.0/doc/source/
--rw-r--r--   0 gberret   (1000) gberret   (1000)      381 2022-05-07 15:01:21.000000 python-musicpd-0.8.0/doc/source/commands.rst
--rw-r--r--   0 gberret   (1000) gberret   (1000)     6871 2021-05-28 09:01:12.000000 python-musicpd-0.8.0/doc/source/commands.txt
--rw-r--r--   0 gberret   (1000) gberret   (1000)    12589 2022-05-07 15:01:21.000000 python-musicpd-0.8.0/doc/source/conf.py
--rw-r--r--   0 gberret   (1000) gberret   (1000)      987 2022-05-07 15:01:21.000000 python-musicpd-0.8.0/doc/source/contribute.rst
--rw-r--r--   0 gberret   (1000) gberret   (1000)      304 2022-05-07 15:01:21.000000 python-musicpd-0.8.0/doc/source/doc.rst
--rw-r--r--   0 gberret   (1000) gberret   (1000)     1841 2022-05-07 15:01:21.000000 python-musicpd-0.8.0/doc/source/index.rst
--rw-r--r--   0 gberret   (1000) gberret   (1000)    10113 2022-05-07 15:01:21.000000 python-musicpd-0.8.0/doc/source/use.rst
--rw-r--r--   0 gberret   (1000) gberret   (1000)    28302 2022-05-07 16:49:26.000000 python-musicpd-0.8.0/musicpd.py
-drwxr-xr-x   0 gberret   (1000) gberret   (1000)        0 2022-05-07 16:50:27.378124 python-musicpd-0.8.0/python_musicpd.egg-info/
--rw-r--r--   0 gberret   (1000) gberret   (1000)     1339 2022-05-07 16:50:27.000000 python-musicpd-0.8.0/python_musicpd.egg-info/PKG-INFO
--rw-r--r--   0 gberret   (1000) gberret   (1000)      380 2022-05-07 16:50:27.000000 python-musicpd-0.8.0/python_musicpd.egg-info/SOURCES.txt
--rw-r--r--   0 gberret   (1000) gberret   (1000)        1 2022-05-07 16:50:27.000000 python-musicpd-0.8.0/python_musicpd.egg-info/dependency_links.txt
--rw-r--r--   0 gberret   (1000) gberret   (1000)        8 2022-05-07 16:50:27.000000 python-musicpd-0.8.0/python_musicpd.egg-info/top_level.txt
--rw-r--r--   0 gberret   (1000) gberret   (1000)     1054 2022-05-07 16:50:27.378124 python-musicpd-0.8.0/setup.cfg
--rwxr-xr-x   0 gberret   (1000) gberret   (1000)      250 2022-05-07 15:01:21.000000 python-musicpd-0.8.0/setup.py
+drwxr-xr-x   0 kaliko    (1000) kaliko    (1000)        0 2024-04-13 07:20:11.803952 python-musicpd-0.9.0/
+-rw-r--r--   0 kaliko    (1000) kaliko    (1000)     3841 2024-04-13 07:19:50.000000 python-musicpd-0.9.0/CHANGES.txt
+-rw-r--r--   0 kaliko    (1000) kaliko    (1000)     7651 2024-04-13 07:19:50.000000 python-musicpd-0.9.0/LICENSE.txt
+-rw-r--r--   0 kaliko    (1000) kaliko    (1000)       70 2024-04-13 07:19:50.000000 python-musicpd-0.9.0/MANIFEST.in
+-rw-r--r--   0 kaliko    (1000) kaliko    (1000)    10206 2024-04-13 07:20:11.803952 python-musicpd-0.9.0/PKG-INFO
+-rw-r--r--   0 kaliko    (1000) kaliko    (1000)      396 2024-04-13 07:19:50.000000 python-musicpd-0.9.0/README.rst
+drwxr-xr-x   0 kaliko    (1000) kaliko    (1000)        0 2024-04-13 07:20:11.803952 python-musicpd-0.9.0/doc/
+drwxr-xr-x   0 kaliko    (1000) kaliko    (1000)        0 2024-04-13 07:20:11.803952 python-musicpd-0.9.0/doc/source/
+-rw-r--r--   0 kaliko    (1000) kaliko    (1000)      380 2024-04-13 07:19:50.000000 python-musicpd-0.9.0/doc/source/commands.rst
+-rw-r--r--   0 kaliko    (1000) kaliko    (1000)     7145 2024-04-13 07:19:50.000000 python-musicpd-0.9.0/doc/source/commands.txt
+-rw-r--r--   0 kaliko    (1000) kaliko    (1000)    12604 2024-04-13 07:19:50.000000 python-musicpd-0.9.0/doc/source/conf.py
+-rw-r--r--   0 kaliko    (1000) kaliko    (1000)      988 2024-04-13 07:19:50.000000 python-musicpd-0.9.0/doc/source/contribute.rst
+-rw-r--r--   0 kaliko    (1000) kaliko    (1000)      236 2024-04-13 07:19:50.000000 python-musicpd-0.9.0/doc/source/doc.rst
+drwxr-xr-x   0 kaliko    (1000) kaliko    (1000)        0 2024-04-13 07:20:11.803952 python-musicpd-0.9.0/doc/source/examples/
+-rw-r--r--   0 kaliko    (1000) kaliko    (1000)     2872 2024-04-13 07:19:50.000000 python-musicpd-0.9.0/doc/source/examples/client.py
+-rw-r--r--   0 kaliko    (1000) kaliko    (1000)      894 2024-04-13 07:19:50.000000 python-musicpd-0.9.0/doc/source/examples/connect.py
+-rw-r--r--   0 kaliko    (1000) kaliko    (1000)      378 2024-04-13 07:19:50.000000 python-musicpd-0.9.0/doc/source/examples/connect_host.py
+-rw-r--r--   0 kaliko    (1000) kaliko    (1000)     1574 2024-04-13 07:19:50.000000 python-musicpd-0.9.0/doc/source/examples/exceptions.py
+-rw-r--r--   0 kaliko    (1000) kaliko    (1000)      212 2024-04-13 07:19:50.000000 python-musicpd-0.9.0/doc/source/examples/findadd.py
+-rw-r--r--   0 kaliko    (1000) kaliko    (1000)      173 2024-04-13 07:19:50.000000 python-musicpd-0.9.0/doc/source/examples/playback.py
+-rw-r--r--   0 kaliko    (1000) kaliko    (1000)     1288 2024-04-13 07:19:50.000000 python-musicpd-0.9.0/doc/source/examples.rst
+-rw-r--r--   0 kaliko    (1000) kaliko    (1000)     1812 2024-04-13 07:19:50.000000 python-musicpd-0.9.0/doc/source/index.rst
+-rw-r--r--   0 kaliko    (1000) kaliko    (1000)    12552 2024-04-13 07:19:50.000000 python-musicpd-0.9.0/doc/source/use.rst
+-rw-r--r--   0 kaliko    (1000) kaliko    (1000)    30735 2024-04-13 07:19:50.000000 python-musicpd-0.9.0/musicpd.py
+-rw-r--r--   0 kaliko    (1000) kaliko    (1000)     1099 2024-04-13 07:19:50.000000 python-musicpd-0.9.0/pyproject.toml
+drwxr-xr-x   0 kaliko    (1000) kaliko    (1000)        0 2024-04-13 07:20:11.803952 python-musicpd-0.9.0/python_musicpd.egg-info/
+-rw-r--r--   0 kaliko    (1000) kaliko    (1000)    10206 2024-04-13 07:20:11.000000 python-musicpd-0.9.0/python_musicpd.egg-info/PKG-INFO
+-rw-r--r--   0 kaliko    (1000) kaliko    (1000)      631 2024-04-13 07:20:11.000000 python-musicpd-0.9.0/python_musicpd.egg-info/SOURCES.txt
+-rw-r--r--   0 kaliko    (1000) kaliko    (1000)        1 2024-04-13 07:20:11.000000 python-musicpd-0.9.0/python_musicpd.egg-info/dependency_links.txt
+-rw-r--r--   0 kaliko    (1000) kaliko    (1000)       24 2024-04-13 07:20:11.000000 python-musicpd-0.9.0/python_musicpd.egg-info/requires.txt
+-rw-r--r--   0 kaliko    (1000) kaliko    (1000)        8 2024-04-13 07:20:11.000000 python-musicpd-0.9.0/python_musicpd.egg-info/top_level.txt
+-rw-r--r--   0 kaliko    (1000) kaliko    (1000)       38 2024-04-13 07:20:11.803952 python-musicpd-0.9.0/setup.cfg
```

### Comparing `python-musicpd-0.8.0/CHANGES.txt` & `python-musicpd-0.9.0/CHANGES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,23 @@
 python-musicpd Changes List
 ===========================
 
+Changes in 0.9.0
+----------------
+
+ * Use right SPDX identifier for license headers
+ * mpd_version attribute init to empty string instead of None
+ * Fixed send_noidle (introduced with e8daa719)
+ * Improved Range object to deal with window parameter
+ * Add logging
+ * Switch to pyproject.toml (setuptools build system)
+ * The connect sequence raises ConnectionError only on error,
+   previously getaddrinfo or unix socket connection error raised an OSError
+ * Improved documentation, add examples
+
 Changes in 0.8.0
 ----------------
 
 * Need python 3.6 minimum (modernize code)
 * Add context management for MPDClient instance (Thanks Wonko der Verständige)
 * Switch to SPDX for license header
```

### Comparing `python-musicpd-0.8.0/LICENSE.txt` & `python-musicpd-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python-musicpd-0.8.0/doc/source/commands.txt` & `python-musicpd-0.9.0/doc/source/commands.txt`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 currentsong                                -> fetch_object
 idle               [<str>]                 -> fetch_list
 noidle                                     -> None
 status                                     -> fetch_object
 stats                                      -> fetch_object
 
 == Playback Option Commands
-consume            <bool>                  -> fetch_nothing
+consume            <str>                   -> fetch_nothing
 crossfade          <int>                   -> fetch_nothing
 mixrampdb          <str>                   -> fetch_nothing
 mixrampdelay       <int>                   -> fetch_nothing
 random             <bool>                  -> fetch_nothing
 repeat             <bool>                  -> fetch_nothing
 setvol             <int>                   -> fetch_nothing
 getvol                                     -> fetch_object
@@ -129,7 +129,14 @@
 
 == Reflection Commands
 config           -> fetch_object
 commands         -> fetch_list
 notcommands      -> fetch_list
 urlhandlers      -> fetch_list
 decoders         -> fetch_plugins
+
+== Client to Client
+subscribe      <str>       -> self._fetch_nothing,
+unsubscribe    <str>       -> self._fetch_nothing,
+channels                   -> self._fetch_list,
+readmessages               -> self._fetch_messages,
+sendmessage    <str> <str> -> self._fetch_nothing,
```

### Comparing `python-musicpd-0.8.0/doc/source/conf.py` & `python-musicpd-0.9.0/doc/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding: utf-8
 # SPDX-FileCopyrightText: 2018-2021  kaliko <kaliko@azylum.org>
-# SPDX-License-Identifier: GPL-3.0-or-later
+# SPDX-License-Identifier: LGPL-3.0-or-later
 #
 # Python MPD Module documentation build configuration file, created by
 # sphinx-quickstart on Mon Mar 12 14:37:32 2018.
 #
 # This file is execfile()d with the current directory set to its
 # containing dir.
 #
@@ -72,15 +72,15 @@
 release = VERSION
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+#language = None
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
 #
 # today = ''
 #
 # Else, today_fmt is used as the format for a strftime call.
@@ -434,11 +434,11 @@
 
 # If false, no index is generated.
 #
 # epub_use_index = True
 
 
 # Example configuration for intersphinx: refer to the Python standard library.
-intersphinx_mapping = {'https://docs.python.org/': None}
+intersphinx_mapping = {'python': ('https://docs.python.org/3', None)}
 
 # autodoc config
 autodoc_member_order = 'bysource'
```

### Comparing `python-musicpd-0.8.0/doc/source/contribute.rst` & `python-musicpd-0.9.0/doc/source/contribute.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .. SPDX-FileCopyrightText: 2018-2021  kaliko <kaliko@azylum.org>
-.. SPDX-License-Identifier: GPL-3.0-or-later
+.. SPDX-License-Identifier: LGPL-3.0-or-later
 
 Contributing
 =============
 
 Use git, `learn if needed`_.
 
 Git Workflow
```

### Comparing `python-musicpd-0.8.0/doc/source/index.rst` & `python-musicpd-0.9.0/doc/source/index.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-.. SPDX-FileCopyrightText: 2018-2021  kaliko <kaliko@azylum.org>
-.. SPDX-License-Identifier: GPL-3.0-or-later
+.. SPDX-FileCopyrightText: 2018-2023  kaliko <kaliko@azylum.org>
+.. SPDX-License-Identifier: LGPL-3.0-or-later
 
 .. include:: ../../README.rst
 
 Installation
 =============
 
 **Latest stable release** from `PyPi <https://pypi.org/project/python-musicpd/>`_:
@@ -16,15 +16,15 @@
 
 .. code:: bash
 
     pip install git+https://gitlab.com/kaliko/python-musicpd.git@dev
 
 
 Library overview
-----------------
+================
 Here is a snippet allowing to list the last modified artists in the media library:
 
 .. code:: python3
 
         #!/usr/bin/env python3
         # coding: utf-8
         import musicpd
@@ -42,38 +42,38 @@
 
         # Script starts here
         if __name__ == '__main__':
             main()
 
 
 Build documentation
---------------------
+===================
 
 .. code:: bash
 
     # Get the source
     git clone https://gitlab.com/kaliko/python-musicpd.git && cd python-musicpd
     # Installs sphinx if needed
     python3 -m venv venv && . ./venv/bin/activate
     pip install sphinx
-    # And build
-    python3 setup.py build_sphinx
-    # Or call sphinx
+    # Call sphinx
     sphinx-build -d ./doc/build/doctrees doc/source -b html ./doc/build/html
 
 
 Contents
 =========
 
 .. toctree::
    :maxdepth: 2
 
+   self
    use.rst
    doc.rst
    commands.rst
+   examples.rst
    contribute.rst
 
 
 Indices and tables
 ==================
 
 * :ref:`genindex`
```

### Comparing `python-musicpd-0.8.0/doc/source/use.rst` & `python-musicpd-0.9.0/doc/source/use.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-.. SPDX-FileCopyrightText: 2018-2021  kaliko <kaliko@azylum.org>
-.. SPDX-License-Identifier: GPL-3.0-or-later
+.. SPDX-FileCopyrightText: 2018-2023  kaliko <kaliko@azylum.org>
+.. SPDX-License-Identifier: LGPL-3.0-or-later
 
 Using the client library
 =========================
 
 Introduction
 ------------
 
@@ -12,51 +12,92 @@
 .. code-block:: python
 
     client = musicpd.MPDClient()       # create client object
     client.connect()                   # use MPD_HOST/MPD_PORT if set else
                                        #   test ${XDG_RUNTIME_DIR}/mpd/socket for existence
                                        #   fallback to localhost:6600
                                        # connect support host/port argument as well
-    print(client.mpd_version)          # print the mpd protocol version
-    print(client.cmd('foo', 42))       # print result of the request "cmd foo 42"
-                                       # (nb. for actual command, see link to the protocol below)
+    print(client.mpd_version)          # print the MPD protocol version
+    client.setvol('42')                # sets the volume
     client.disconnect()                # disconnect from the server
 
-In the example above `cmd` in not an actual MPD command, for a list of
-supported commands, their arguments (as MPD currently understands
-them), and the functions used to parse their responses see :ref:`commands`.
+The MPD command protocol exchanges line-based text records. The client emits a
+command with optional arguments. In the example above the client sends a
+`setvol` command with the string argument `42`.
+
+MPD commands are exposed as :py:class:`musicpd.MPDClient` methods. Methods
+**arguments are python strings**. Some commands are composed of more than one word
+(ie "**tagtypes [disable|enable|all]**"), for these use a `snake case`_ style to
+access the method. Then **"tagtypes enable"** command is called with
+**"tagtypes_enable"**.
+
+Remember MPD protocol is text based, then all MPD command arguments are UTF-8
+strings. In the example above, an integer can be used as argument for the
+`setvol` command, but it is then evaluated as a string when the command is
+written to the socket. To avoid confusion use regular string instead of relying
+on object string representation.
+
+:py:class:`musicpd.MPDClient` methods returns different kinds of objects
+depending on the command. Could be :py:obj:`None`, a single object as a
+:py:obj:`str` or a :py:obj:`dict`, a list of :py:obj:`dict`.
+
+Then :py:class:`musicpd.MPDClient` **methods signatures** are not hard coded
+within this module since the protocol is handled on the server side. Please
+refer to the protocol and MPD commands in `MPD protocol documentation`_ to
+learn how to call commands and what kind of arguments they expect.
 
-See the `MPD protocol documentation`_ for more details.
+Some examples are provided for the most common cases, see :ref:`examples`.
+
+For a list of currently supported commands in this python module see
+:ref:`commands`.
 
 .. _environment_variables:
 
 Environment variables
 ---------------------
 
-The client honors the following environment variables:
+:py:class:`musicpd.MPDClient` honors the following environment variables:
+
+.. envvar:: MPD_HOST
+
+   MPD host (:abbr:`FQDN (fully qualified domain name)`, IP, socket path or abstract socket) and password.
+
+    | To define a **password** set :envvar:`MPD_HOST` to "*password@host*" (password only "*password@*")
+    | For **abstract socket** use "@" as prefix : "*@socket*" and then with a password  "*pass@@socket*"
+    | Regular **unix socket** are set with an absolute path: "*/run/mpd/socket*"
+
+.. envvar:: MPD_PORT
+
+   MPD port, relevant for TCP socket only
+
+.. envvar:: MPD_TIMEOUT
+
+   socket timeout when connecting to MPD and waiting for MPD’s response (in seconds)
 
-  * ``MPD_HOST`` MPD host (:abbr:`FQDN (fully qualified domain name)`, socket path or abstract socket) and password.
+.. envvar:: XDG_RUNTIME_DIR
 
-    | To define a password set MPD_HOST to "`password@host`" (password only "`password@`")
-    | For abstract socket use "@" as prefix : "`@socket`" and then with a password  "`pass@@socket`"
-    | Regular unix socket are set with an absolute path: "`/run/mpd/socket`"
-  * ``MPD_PORT`` MPD port, relevant for TCP socket only, ie with :abbr:`FQDN (fully qualified domain name)` defined host
-  * ``MPD_TIMEOUT`` timeout for connecting to MPD and waiting for MPD’s response in seconds
-  * ``XDG_RUNTIME_DIR`` path to look for potential socket: ``${XDG_RUNTIME_DIR}/mpd/socket``
+   path to look for potential socket
 
 .. _default_settings:
 
 Default settings
 ----------------
 
-  * If ``MPD_HOST`` is not set, then look for a socket in ``${XDG_RUNTIME_DIR}/mpd/socket``
-  * If there is no socket use ``localhost``
-  * If ``MPD_PORT`` is not set, then use ``6600``
-  * If ``MPD_TIMEOUT`` is not set, then uses :py:obj:`musicpd.CONNECTION_TIMEOUT`
-
+Default host:
+ * use :envvar:`MPD_HOST` environment variable if set, extract password if present,
+ * else use :envvar:`XDG_RUNTIME_DIR` to looks for an existing file in ``${XDG_RUNTIME_DIR}/mpd/socket``, :envvar:`XDG_RUNTIME_DIR` defaults to ``/run`` if not set.
+ * else set host to ``localhost``
+
+Default port:
+ * use :envvar:`MPD_PORT` environment variable if set
+ * else use ``6600``
+
+Default timeout:
+ * use :envvar:`MPD_TIMEOUT` if set
+ * else use :py:obj:`musicpd.CONNECTION_TIMEOUT`
 
 Context manager
 ---------------
 
 Calling MPDClient in a context manager :py:obj:`musicpd.MPDClient.connect` is
 transparently called with :ref:`default setting<default_settings>` (use
 :ref:`environment variables<environment_variables>` to override defaults).
@@ -82,37 +123,42 @@
     client.update()                      # insert the update command into the list
     client.status()                      # insert the status command into the list
     results = client.command_list_end()  # results will be a list with the results
 
 Ranges
 ------
 
-Provide a 2-tuple as argument for command supporting ranges (cf. `MPD protocol documentation`_ for more details).
-Possible ranges are: "START:END", "START:" and ":" :
+Some commands (e.g. delete) allow specifying a range in the form `"START:END"` (cf. `MPD protocol documentation`_ for more details).
+
+Possible ranges are: `"START:END"`, `"START:"` and `":"` :
+
+Instead of giving the plain string as `"START:END"`, you **can** provide a :py:obj:`tuple` as `(START,END)`. The module is then ensuring the format is correct and raises an :py:obj:`musicpd.CommandError` exception otherwise. Empty start or end can be specified as en empty string ``''`` or :py:obj:`None`.
 
 .. code-block:: python
 
     # An intelligent clear
     # clears played track in the queue, currentsong included
     pos = client.currentsong().get('pos', 0)
-    # the 2-tuple range object accepts str, no need to convert to int
+    # the range object accepts str, no need to convert to int
     client.delete((0, pos))
     # missing end interpreted as highest value possible, pay attention still need a tuple.
     client.delete((pos,))  # purge queue from current to the end
 
-A notable case is the `rangeid` command allowing an empty range specified
-as a single colon as argument (i.e. sending just ":"):
+A notable case is the *rangeid* command allowing an empty range specified
+as a single colon as argument (i.e. sending just ``":"``):
 
 .. code-block:: python
 
     # sending "rangeid :" to clear the range, play everything
     client.rangeid(())  # send an empty tuple
 
 Empty start in range (i.e. ":END") are not possible and will raise a CommandError.
 
+.. note:: Remember the use of a tuple is **optional**. Range can still be specified as a plain string ``"START:END"``.
+
 Iterators
 ----------
 
 Commands may also return iterators instead of lists if `iterate` is set to
 `True`:
 
 .. code-block:: python
@@ -168,15 +214,15 @@
     >>>         aart = cli.albumart(track, received)
     >>>         cover.write(aart.get('data'))
     >>>         received += int(aart.get('binary'))
     >>>     if received != size:
     >>>         print('something went wrong', file=sys.stderr)
     >>> cli.disconnect()
 
-A `CommandError` is raised if the album does not expose a cover.
+A :py:obj:`musicpd.CommandError` is raised if the album does not expose a cover.
 
 You can also use `readpicture` command to fetch embedded picture:
 
 .. code-block:: python
 
     >>> cli = musicpd.MPDClient()
     >>> cli.connect()
@@ -263,10 +309,24 @@
   * Nothing to read, cancel idle with ``noidle``
 
 All three commands in the while loop (send_idle, fetch_idle, noidle) are not
 triggering a socket timeout unless the connection is actually lost (actually it
 could also be that MPD took too much time to answer, but MPD taking more than a
 couple of seconds for these commands should never occur).
 
+.. _exceptions:
+
+Exceptions
+----------
+
+The :py:obj:`connect<musicpd.MPDClient.connect>` method raises
+:py:obj:`ConnectionError<musicpd.ConnectionError>` only (an :py:obj:`MPDError<musicpd.MPDError>` exception) but then, calling other MPD commands, the module can raise
+:py:obj:`MPDError<musicpd.MPDError>` or an :py:obj:`OSError` depending on the error and
+where it occurs.
+
+Then using musicpd module both :py:obj:`musicpd.MPDError` and :py:obj:`OSError`
+exceptions families are expected, see :ref:`examples<exceptions_example>` for a
+way to deal with this.
 
 .. _MPD protocol documentation: http://www.musicpd.org/doc/protocol/
+.. _snake case: https://en.wikipedia.org/wiki/Snake_case
 .. vim: spell spelllang=en
```

### Comparing `python-musicpd-0.8.0/musicpd.py` & `python-musicpd-0.9.0/musicpd.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,37 @@
-# SPDX-FileCopyrightText: 2012-2022  kaliko <kaliko@azylum.org>
+# -*- coding: utf-8 -*-
+# SPDX-FileCopyrightText: 2012-2024  kaliko <kaliko@azylum.org>
 # SPDX-FileCopyrightText: 2021       Wonko der Verständige <wonko@hanstool.org>
 # SPDX-FileCopyrightText: 2019       Naglis Jonaitis <naglis@mailbox.org>
 # SPDX-FileCopyrightText: 2019       Bart Van Loon <bbb@bbbart.be>
 # SPDX-FileCopyrightText: 2008-2010  J. Alexander Treuman <jat@spatialrift.net>
-# SPDX-License-Identifier: GPL-3.0-or-later
-"""python-musicpd: Python Music Player Daemon client library"""
+# SPDX-License-Identifier: LGPL-3.0-or-later
+"""Python Music Player Daemon client library"""
 
 
-import socket
+import logging
 import os
+import socket
 
 from functools import wraps
 
 HELLO_PREFIX = "OK MPD "
 ERROR_PREFIX = "ACK "
 SUCCESS = "OK"
 NEXT = "list_OK"
-VERSION = '0.8.0'
+#: Module version
+VERSION = '0.9.0'
 #: Seconds before a connection attempt times out
-#: (overriden by MPD_TIMEOUT env. var.)
+#: (overriden by :envvar:`MPD_TIMEOUT` env. var.)
 CONNECTION_TIMEOUT = 30
-#: Socket timeout in second (Default is None for no timeout)
+#: Socket timeout in second > 0 (Default is :py:obj:`None` for no timeout)
 SOCKET_TIMEOUT = None
 
+log = logging.getLogger(__name__)
+
 
 def iterator_wrapper(func):
     """Decorator handling iterate option"""
     @wraps(func)
     def decorated_function(instance, *args, **kwargs):
         generator = func(instance, *args, **kwargs)
         if not instance.iterate:
@@ -40,122 +45,148 @@
             finally:
                 instance._iterating = False
         return iterator(generator)
     return decorated_function
 
 
 class MPDError(Exception):
-    pass
+    """Main musicpd Exception"""
 
 
 class ConnectionError(MPDError):
-    pass
+    """Fatal Connection Error, cannot recover from it."""
 
 
 class ProtocolError(MPDError):
-    pass
+    """Fatal Protocol Error, cannot recover from it"""
 
 
 class CommandError(MPDError):
-    pass
+    """Malformed command, socket should be fine, can reuse it"""
 
 
 class CommandListError(MPDError):
-    pass
+    """"""
 
 
 class PendingCommandError(MPDError):
-    pass
+    """"""
 
 
 class IteratingError(MPDError):
-    pass
+    """"""
 
 
 class Range:
 
     def __init__(self, tpl):
         self.tpl = tpl
+        self.lower = ''
+        self.upper = ''
         self._check()
 
     def __str__(self):
-        if len(self.tpl) == 0:
-            return ':'
-        if len(self.tpl) == 1:
-            return '{0}:'.format(self.tpl[0])
-        return '{0[0]}:{0[1]}'.format(self.tpl)
+        return f'{self.lower}:{self.upper}'
 
     def __repr__(self):
-        return 'Range({0})'.format(self.tpl)
+        return f'Range({self.tpl})'
+
+    def _check_element(self, item):
+        if item is None or item == '':
+            return ''
+        try:
+            return str(int(item))
+        except (TypeError, ValueError) as err:
+            raise CommandError(f'Not an integer: "{item}"') from err
+        return item
 
     def _check(self):
         if not isinstance(self.tpl, tuple):
             raise CommandError('Wrong type, provide a tuple')
-        if len(self.tpl) not in [0, 1, 2]:
-            raise CommandError('length not in [0, 1, 2]')
-        for index in self.tpl:
-            try:
-                index = int(index)
-            except (TypeError, ValueError) as err:
-                raise CommandError('Not a tuple of int') from err
+        if len(self.tpl) == 0:
+            return
+        if len(self.tpl) == 1:
+            self.lower = self._check_element(self.tpl[0])
+            return
+        if len(self.tpl) != 2:
+            raise CommandError('Range wrong size (0, 1 or 2 allowed)')
+        self.lower = self._check_element(self.tpl[0])
+        self.upper = self._check_element(self.tpl[1])
+        if self.lower == '' and self.upper != '':
+            raise CommandError(f'Integer expected to start the range: {self.tpl}')
+        if self.upper.isdigit() and self.lower.isdigit():
+            if int(self.lower) > int(self.upper):
+                raise CommandError(f'Wrong range: {self.lower} > {self.upper}')
 
 
 class _NotConnected:
 
     def __getattr__(self, attr):
         return self._dummy
 
     def _dummy(self, *args):
         raise ConnectionError("Not connected")
 
 
 class MPDClient:
-    """MPDClient instance will look for ``MPD_HOST``/``MPD_PORT``/``XDG_RUNTIME_DIR`` environment
-    variables and set instance attribute ``host``, ``port`` and ``pwd``
-    accordingly. Regarding ``MPD_HOST`` format to expose password refer
-    MPD client manual :manpage:`mpc (1)`.
+    """MPDClient instance will look for :envvar:`MPD_HOST`/:envvar:`MPD_PORT`/:envvar:`XDG_RUNTIME_DIR` environment
+    variables and set instance attribute :py:attr:`host`, :py:attr:`port` and :py:obj:`pwd`
+    accordingly.
 
-    Then :py:obj:`musicpd.MPDClient.connect` will use ``host`` and ``port`` as defaults if not provided as args.
+    Then :py:obj:`musicpd.MPDClient.connect` will use :py:obj:`host` and
+    :py:obj:`port` as defaults if not provided as args.
 
-    Cf. :py:obj:`musicpd.MPDClient.connect` for details.
+    Regarding :envvar:`MPD_HOST` format to expose password refer this module
+    documentation or MPD client manual :manpage:`mpc (1)`.
 
     >>> from os import environ
     >>> environ['MPD_HOST'] = 'pass@mpdhost'
     >>> cli = musicpd.MPDClient()
     >>> cli.pwd == environ['MPD_HOST'].split('@')[0]
     True
     >>> cli.host == environ['MPD_HOST'].split('@')[1]
     True
     >>> cli.connect() # will use host/port as set in MPD_HOST/MPD_PORT
 
-    :ivar str host: host used with the current connection
-    :ivar str,int port: port used with the current connection
-    :ivar str pwd: password detected in ``MPD_HOST`` environment variable
-
-    .. warning:: Instance attribute host/port/pwd
-
-      While :py:attr:`musicpd.MPDClient().host` and
-      :py:attr:`musicpd.MPDClient().port` keep track of current connection
-      host and port, :py:attr:`musicpd.MPDClient().pwd` is set once with
+    .. note::
+
+      default host:
+       * use :envvar:`MPD_HOST` environment variable if set, extract password if present,
+       * else use :envvar:`XDG_RUNTIME_DIR` to looks for an existing file in ``${XDG_RUNTIME_DIR:-/run/}/mpd/socket``
+       * else set host to ``localhost``
+
+      default port:
+       * use :envvar:`MPD_PORT` environment variable is set
+       * else use ``6600``
+
+    .. warning:: **Instance attribute host/port/pwd**
+
+      While :py:attr:`musicpd.MPDClient.host` and
+      :py:attr:`musicpd.MPDClient.port` keep track of current connection
+      host and port, :py:attr:`musicpd.MPDClient.pwd` is set once with
       password extracted from environment variable.
-      Calling :py:meth:`musicpd.MPDClient().password()` with a new password
-      won't update :py:attr:`musicpd.MPDClient().pwd` value.
+      Calling MPS's password method with a new password
+      won't update :py:attr:`musicpd.MPDClient.pwd` value.
 
-      Moreover, :py:attr:`musicpd.MPDClient().pwd` is only an helper attribute
-      exposing password extracted from ``MPD_HOST`` environment variable, it
-      will not be used as default value for the :py:meth:`password` method
+      Moreover, :py:attr:`musicpd.MPDClient.pwd` is only an helper attribute
+      exposing password extracted from :envvar:`MPD_HOST` environment variable, it
+      will not be used as default value for the MPD's password command.
     """
 
     def __init__(self):
         self.iterate = False
         #: Socket timeout value in seconds
         self._socket_timeout = SOCKET_TIMEOUT
         #: Current connection timeout value, defaults to
         #: :py:obj:`CONNECTION_TIMEOUT` or env. var. ``MPD_TIMEOUT`` if provided
         self.mpd_timeout = None
+        self.mpd_version = ''
+        """Protocol version as exposed by the server as a :py:obj:`str`
+
+        .. note:: This is the version of the protocol spoken, not the real version of the daemon."""
         self._reset()
         self._commands = {
             # Status Commands
             "clearerror":         self._fetch_nothing,
             "currentsong":        self._fetch_object,
             "idle":               self._fetch_list,
             #"noidle":             None,
@@ -280,55 +311,66 @@
             # Client to Client
             "subscribe":          self._fetch_nothing,
             "unsubscribe":        self._fetch_nothing,
             "channels":           self._fetch_list,
             "readmessages":       self._fetch_messages,
             "sendmessage":        self._fetch_nothing,
         }
+        #: host used with the current connection (:py:obj:`str`)
+        self.host = None
+        #: password detected in :envvar:`MPD_HOST` environment variable (:py:obj:`str`)
+        self.pwd = None
+        #: port used with the current connection (:py:obj:`int`, :py:obj:`str`)
+        self.port = None
         self._get_envvars()
 
     def _get_envvars(self):
         """
-        Retrieve MPD env. var. to overrides "localhost:6600"
-            Use MPD_HOST/MPD_PORT if set
-            else use MPD_HOST=${XDG_RUNTIME_DIR:-/run/}/mpd/socket if file exists
+        Retrieve MPD env. var. to overrides default "localhost:6600"
         """
+        # Set some defaults
         self.host = 'localhost'
-        self.pwd = None
         self.port = os.getenv('MPD_PORT', '6600')
-        if os.getenv('MPD_HOST'):
+        _host = os.getenv('MPD_HOST', '')
+        if _host:
             # If password is set: MPD_HOST=pass@host
-            if '@' in os.getenv('MPD_HOST'):
-                mpd_host_env = os.getenv('MPD_HOST').split('@', 1)
+            if '@' in _host:
+                mpd_host_env = _host.split('@', 1)
                 if mpd_host_env[0]:
                     # A password is actually set
+                    log.debug('password detected in MPD_HOST, set client pwd attribute')
                     self.pwd = mpd_host_env[0]
                     if mpd_host_env[1]:
                         self.host = mpd_host_env[1]
+                        log.debug('host detected in MPD_HOST: %s', self.host)
                 elif mpd_host_env[1]:
                     # No password set but leading @ is an abstract socket
                     self.host = '@'+mpd_host_env[1]
+                    log.debug('host detected in MPD_HOST: %s (abstract socket)', self.host)
             else:
                 # MPD_HOST is a plain host
-                self.host = os.getenv('MPD_HOST')
+                self.host = _host
+                log.debug('host detected in MPD_HOST: %s', self.host)
         else:
             # Is socket there
             xdg_runtime_dir = os.getenv('XDG_RUNTIME_DIR', '/run')
             rundir = os.path.join(xdg_runtime_dir, 'mpd/socket')
             if os.path.exists(rundir):
                 self.host = rundir
-        self.mpd_timeout = os.getenv('MPD_TIMEOUT')
-        if self.mpd_timeout and self.mpd_timeout.isdigit():
-            self.mpd_timeout = int(self.mpd_timeout)
+                log.debug('host detected in ${XDG_RUNTIME_DIR}/run: %s (unix socket)', self.host)
+        _mpd_timeout = os.getenv('MPD_TIMEOUT', '')
+        if _mpd_timeout.isdigit():
+            self.mpd_timeout = int(_mpd_timeout)
+            log.debug('timeout detected in MPD_TIMEOUT: %d', self.mpd_timeout)
         else:  # Use CONNECTION_TIMEOUT as default even if MPD_TIMEOUT carries gargage
             self.mpd_timeout = CONNECTION_TIMEOUT
 
     def __getattr__(self, attr):
         if attr == 'send_noidle':  # have send_noidle to cancel idle as well as noidle
-            return self.noidle()
+            return self.noidle
         if attr.startswith("send_"):
             command = attr.replace("send_", "", 1)
             wrapper = self._send
         elif attr.startswith("fetch_"):
             command = attr.replace("fetch_", "", 1)
             wrapper = self._fetch
         else:
@@ -390,17 +432,17 @@
 
     def _write_command(self, command, args=None):
         if args is None:
             args = []
         parts = [command]
         for arg in args:
             if isinstance(arg, tuple):
-                parts.append('{0!s}'.format(Range(arg)))
+                parts.append(f'{Range(arg)!s}')
             else:
-                parts.append('"%s"' % escape(str(arg)))
+                parts.append(f'"{escape(str(arg))}"')
         if '\n' in ' '.join(parts):
             raise CommandError('new line found in the command!')
         self._write_line(" ".join(parts))
 
     def _read_binary(self, amount):
         chunk = bytearray()
         while amount > 0:
@@ -581,130 +623,142 @@
             raise ConnectionError("Connection lost while reading MPD hello")
         line = line.rstrip("\n")
         if not line.startswith(HELLO_PREFIX):
             raise ProtocolError(f"Got invalid MPD hello: '{line}'")
         self.mpd_version = line[len(HELLO_PREFIX):].strip()
 
     def _reset(self):
-        self.mpd_version = None
+        self.mpd_version = ''
         self._iterating = False
         self._pending = []
         self._command_list = None
         self._sock = None
         self._rfile = _NotConnected()
         self._rbfile = _NotConnected()
         self._wfile = _NotConnected()
 
     def _connect_unix(self, path):
         if not hasattr(socket, "AF_UNIX"):
             raise ConnectionError("Unix domain sockets not supported on this platform")
         # abstract socket
         if path.startswith('@'):
             path = '\0'+path[1:]
-        sock = socket.socket(socket.AF_UNIX, socket.SOCK_STREAM)
-        sock.settimeout(self.mpd_timeout)
-        sock.connect(path)
-        sock.settimeout(self.socket_timeout)
+        try:
+            sock = socket.socket(socket.AF_UNIX, socket.SOCK_STREAM)
+            sock.settimeout(self.mpd_timeout)
+            sock.connect(path)
+            sock.settimeout(self.socket_timeout)
+        except socket.error as socket_err:
+            raise ConnectionError(socket_err) from socket_err
         return sock
 
     def _connect_tcp(self, host, port):
         try:
             flags = socket.AI_ADDRCONFIG
         except AttributeError:
             flags = 0
         err = None
-        for res in socket.getaddrinfo(host, port, socket.AF_UNSPEC,
-                                      socket.SOCK_STREAM, socket.IPPROTO_TCP,
-                                      flags):
+        try:
+            gai = socket.getaddrinfo(host, port, socket.AF_UNSPEC,
+                                     socket.SOCK_STREAM, socket.IPPROTO_TCP,
+                                     flags)
+        except socket.error as gaierr:
+            raise ConnectionError(gaierr) from gaierr
+        for res in gai:
             af, socktype, proto, _, sa = res
             sock = None
             try:
+                log.debug('opening socket %s', sa)
                 sock = socket.socket(af, socktype, proto)
                 sock.settimeout(self.mpd_timeout)
                 sock.connect(sa)
                 sock.settimeout(self.socket_timeout)
                 return sock
             except socket.error as socket_err:
+                log.debug('opening socket %s failed: %s', sa, socket_err)
                 err = socket_err
                 if sock is not None:
                     sock.close()
         if err is not None:
-            raise ConnectionError(str(err))
+            raise ConnectionError(err)
         raise ConnectionError("getaddrinfo returns an empty list")
 
     def noidle(self):
         # noidle's special case
         if not self._pending or self._pending[0] != 'idle':
             raise CommandError('cannot send noidle if send_idle was not called')
         del self._pending[0]
         self._write_command("noidle")
         return self._fetch_list()
 
     def connect(self, host=None, port=None):
         """Connects the MPD server
 
-        :param str host: hostname, IP or FQDN (defaults to `localhost` or socket, see below for details)
-        :param port: port number (defaults to 6600)
+        :param str host: hostname, IP or FQDN (defaults to *localhost* or socket)
+        :param port: port number (defaults to *6600*)
         :type port: str or int
 
-        The connect method honors MPD_HOST/MPD_PORT environment variables.
+        If host/port are :py:obj:`None` the socket uses :py:attr:`host`/:py:attr:`port`
+        attributes as defaults. Cf. :py:obj:`MPDClient` for the logic behind default host/port.
 
-        The underlying socket also honors MPD_TIMEOUT environment variable
+        The underlying socket also honors :envvar:`MPD_TIMEOUT` environment variable
         and defaults to :py:obj:`musicpd.CONNECTION_TIMEOUT` (connect command only).
 
         If you want to have a timeout for each command once you got connected,
         set its value in :py:obj:`MPDClient.socket_timeout` (in second) or at
         module level in :py:obj:`musicpd.SOCKET_TIMEOUT`.
-
-        .. note:: Default host/port
-
-          If host evaluate to :py:obj:`False`
-           * use ``MPD_HOST`` environment variable if set, extract password if present,
-           * else looks for an existing file in ``${XDG_RUNTIME_DIR:-/run/}/mpd/socket``
-           * else set host to ``localhost``
-
-          If port evaluate to :py:obj:`False`
-           * if ``MPD_PORT`` environment variable is set, use it for port
-           * else use ``6600``
         """
         if not host:
             host = self.host
         else:
             self.host = host
         if not port:
             port = self.port
         else:
             self.port = port
         if self._sock is not None:
             raise ConnectionError("Already connected")
         if host[0] in ['/', '@']:
+            log.debug('Connecting unix socket %s', host)
             self._sock = self._connect_unix(host)
         else:
+            log.debug('Connecting tcp socket %s:%s (timeout: %ss)', host, port, self.mpd_timeout)
             self._sock = self._connect_tcp(host, port)
         self._rfile = self._sock.makefile("r", encoding='utf-8', errors='surrogateescape')
         self._rbfile = self._sock.makefile("rb")
         self._wfile = self._sock.makefile("w", encoding='utf-8')
         try:
             self._hello()
         except:
             self.disconnect()
             raise
+        log.debug('Connected')
 
     @property
     def socket_timeout(self):
         """Socket timeout in second (defaults to :py:obj:`SOCKET_TIMEOUT`).
-        Use None to disable socket timout."""
+        Use :py:obj:`None` to disable socket timout.
+
+        :setter: Set the socket timeout (integer > 0)
+        :type: int or None
+        """
         return self._socket_timeout
 
     @socket_timeout.setter
     def socket_timeout(self, timeout):
-        self._socket_timeout = timeout
+        if timeout is not None:
+            if int(timeout) <= 0:
+                raise ValueError('socket_timeout expects a non zero positive integer')
+            self._socket_timeout = int(timeout)
+        else:
+            self._socket_timeout = timeout
         if getattr(self._sock, 'settimeout', False):
             self._sock.settimeout(self._socket_timeout)
 
+
     def disconnect(self):
         """Closes the MPD connection.
         The client closes the actual socket, it does not use the
         'close' request from MPD protocol (as suggested in documentation).
         """
         if hasattr(self._rfile, 'close'):
             self._rfile.close()
```

