# Comparing `tmp/scramp-1.4.4.tar.gz` & `tmp/scramp-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scramp-1.4.4.tar", last modified: Tue Nov  1 17:17:53 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `scramp-1.4.4.tar` & `scramp-1.4.5.tar`

### file list

```diff
@@ -1,19 +1,11 @@
-drwxrwxr-x   0 tlocke    (1000) tlocke    (1000)        0 2022-11-01 17:17:53.270111 scramp-1.4.4/
--rw-rw-r--   0 tlocke    (1000) tlocke    (1000)      906 2022-10-22 13:23:38.000000 scramp-1.4.4/LICENSE
--rw-rw-r--   0 tlocke    (1000) tlocke    (1000)    19808 2022-11-01 17:17:53.270111 scramp-1.4.4/PKG-INFO
--rw-rw-r--   0 tlocke    (1000) tlocke    (1000)    18790 2022-11-01 17:14:55.000000 scramp-1.4.4/README.rst
--rw-rw-r--   0 tlocke    (1000) tlocke    (1000)     1533 2022-10-22 13:44:58.000000 scramp-1.4.4/pyproject.toml
-drwxrwxr-x   0 tlocke    (1000) tlocke    (1000)        0 2022-11-01 17:17:53.270111 scramp-1.4.4/scramp/
--rw-rw-r--   0 tlocke    (1000) tlocke    (1000)      335 2022-05-20 10:43:59.000000 scramp-1.4.4/scramp/__init__.py
--rw-rw-r--   0 tlocke    (1000) tlocke    (1000)    22503 2022-11-01 17:11:03.000000 scramp-1.4.4/scramp/core.py
--rw-rw-r--   0 tlocke    (1000) tlocke    (1000)      655 2021-07-26 09:16:41.000000 scramp-1.4.4/scramp/utils.py
-drwxrwxr-x   0 tlocke    (1000) tlocke    (1000)        0 2022-11-01 17:17:53.270111 scramp-1.4.4/scramp.egg-info/
--rw-rw-r--   0 tlocke    (1000) tlocke    (1000)    19808 2022-11-01 17:17:53.000000 scramp-1.4.4/scramp.egg-info/PKG-INFO
--rw-rw-r--   0 tlocke    (1000) tlocke    (1000)      282 2022-11-01 17:17:53.000000 scramp-1.4.4/scramp.egg-info/SOURCES.txt
--rw-rw-r--   0 tlocke    (1000) tlocke    (1000)        1 2022-11-01 17:17:53.000000 scramp-1.4.4/scramp.egg-info/dependency_links.txt
--rw-rw-r--   0 tlocke    (1000) tlocke    (1000)       69 2022-11-01 17:17:53.000000 scramp-1.4.4/scramp.egg-info/requires.txt
--rw-rw-r--   0 tlocke    (1000) tlocke    (1000)        7 2022-11-01 17:17:53.000000 scramp-1.4.4/scramp.egg-info/top_level.txt
--rw-rw-r--   0 tlocke    (1000) tlocke    (1000)      197 2022-11-01 17:17:53.270111 scramp-1.4.4/setup.cfg
-drwxrwxr-x   0 tlocke    (1000) tlocke    (1000)        0 2022-11-01 17:17:53.270111 scramp-1.4.4/test/
--rw-rw-r--   0 tlocke    (1000) tlocke    (1000)      222 2022-05-20 10:43:59.000000 scramp-1.4.4/test/test_readme.py
--rw-rw-r--   0 tlocke    (1000) tlocke    (1000)    18116 2022-11-01 17:11:03.000000 scramp-1.4.4/test/test_scramp.py
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 scramp-1.4.5/.github/workflows/test.yml
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 scramp-1.4.5/src/scramp/__init__.py
+-rw-r--r--   0        0        0    22501 2020-02-02 00:00:00.000000 scramp-1.4.5/src/scramp/core.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 scramp-1.4.5/src/scramp/utils.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 scramp-1.4.5/test/test_readme.py
+-rw-r--r--   0        0        0    18116 2020-02-02 00:00:00.000000 scramp-1.4.5/test/test_scramp.py
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 scramp-1.4.5/.gitignore
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 scramp-1.4.5/LICENSE
+-rw-r--r--   0        0        0    17940 2020-02-02 00:00:00.000000 scramp-1.4.5/README.md
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 scramp-1.4.5/pyproject.toml
+-rw-r--r--   0        0        0    19020 2020-02-02 00:00:00.000000 scramp-1.4.5/PKG-INFO
```

### Comparing `scramp-1.4.4/LICENSE` & `scramp-1.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `scramp-1.4.4/PKG-INFO` & `scramp-1.4.5/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,69 +1,38 @@
-Metadata-Version: 2.1
-Name: scramp
-Version: 1.4.4
-Summary: An implementation of the SCRAM protocol.
-License: MIT No Attribution
-Project-URL: Homepage, https://github.com/tlocke/scramp
-Keywords: SCRAM,authentication,SASL
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT No Attribution License (MIT-0)
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: Implementation
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
-======
-Scramp
-======
+# Scramp
 
-A Python implementation of the `SCRAM authentication protocol
-<https://en.wikipedia.org/wiki/Salted_Challenge_Response_Authentication_Mechanism>`_.
+A Python implementation of the [SCRAM authentication protocol](
+https://en.wikipedia.org/wiki/Salted_Challenge_Response_Authentication_Mechanism>).
 Scramp supports the following mechanisms:
 
 - SCRAM-SHA-1
 - SCRAM-SHA-1-PLUS
 - SCRAM-SHA-256
 - SCRAM-SHA-256-PLUS
 - SCRAM-SHA-512
 - SCRAM-SHA-512-PLUS
 - SCRAM-SHA3-512
 - SCRAM-SHA3-512-PLUS
 
-.. contents:: Table of Contents
-   :depth: 2
-   :local:
 
-Installation
-------------
+## Installation
 
-- Create a virtual environment: ``python3 -m venv venv``
-- Activate the virtual environment: ``source venv/bin/activate``
-- Install: ``pip install scramp``
+- Create a virtual environment: `python3 -m venv venv`
+- Activate the virtual environment: `source venv/bin/activate`
+- Install: `pip install scramp`
 
 
-Examples
---------
+## Examples
 
-Client and Server
-`````````````````
+### Client and Server
 
 Here's an example using both the client and the server. It's a bit contrived as normally
 you'd be using either the client or server on its own.
 
+```python
 >>> from scramp import ScramClient, ScramMechanism
 >>>
 >>> USERNAME = 'user'
 >>> PASSWORD = 'pencil'
 >>> MECHANISMS = ['SCRAM-SHA-256']
 >>>
 >>>
@@ -100,23 +69,24 @@
 >>> s.set_client_final(cfinal)
 >>> sfinal = s.get_server_final()
 >>>
 >>> c.set_server_final(sfinal)
 >>>
 >>> # If it all runs through without raising an exception, the authentication
 >>> # has succeeded
+```
 
 
-Client only
-```````````
+### Client only
 
 Here's an example using just the client. The client nonce is specified in order to give
-a reproducible example, but in production you'd omit the ``c_nonce`` parameter and let
-``ScramClient`` generate a client nonce:
+a reproducible example, but in production you'd omit the `c_nonce` parameter and let
+`ScramClient` generate a client nonce:
 
+```python
 >>> from scramp import ScramClient
 >>>
 >>> USERNAME = 'user'
 >>> PASSWORD = 'pencil'
 >>> C_NONCE = 'rOprNGfwEbeRWgbNEkqO'
 >>> MECHANISMS = ['SCRAM-SHA-256']
 >>>
@@ -141,23 +111,24 @@
 c=biws,r=rOprNGfwEbeRWgbNEkqO%hvYDpWUa2RaTCAfuxFIlj)hNlF$k0,p=dHzbZapWIk4jUhN+Ute9ytag9zjfMHgsqmmiz7AndVQ=
 >>>
 >>> # Set the final message from the server
 >>> c.set_server_final('v=6rriTRBi23WpRR/wtup+mMhUZUn/dB5nLTJRsjl95G4=')
 >>>
 >>> # If it all runs through without raising an exception, the authentication
 >>> # has succeeded
+```
 
 
-Server only
-```````````
+### Server only
 
 Here's an example using just the server. The server nonce and salt is specified in order
-to give a reproducible example, but in production you'd omit the ``s_nonce`` and
-``salt`` parameters and let Scramp generate them:
+to give a reproducible example, but in production you'd omit the `s_nonce` and `salt`
+parameters and let Scramp generate them:
 
+```python
 >>> from scramp import ScramMechanism
 >>>
 >>> USERNAME = 'user'
 >>> PASSWORD = 'pencil'
 >>> S_NONCE = '%hvYDpWUa2RaTCAfuxFIlj)hNlF$k0'
 >>> SALT = b'[m\x99h\x9d\x125\x8e\xec\xa0K\x14\x126\xfa\x81'
 >>>
@@ -195,24 +166,25 @@
 >>> # Get the final server message and send it to the client
 >>> sfinal = s.get_server_final()
 >>> print(sfinal)
 v=6rriTRBi23WpRR/wtup+mMhUZUn/dB5nLTJRsjl95G4=
 >>>
 >>> # If it all runs through without raising an exception, the authentication
 >>> # has succeeded
+```
 
 
-Server only with passlib
-````````````````````````
+### Server only with passlib
 
-Here's an example using just the server and using the `passlib hashing library
-<https://passlib.readthedocs.io/en/stable/index.html>`_. The server nonce and salt is
+Here's an example using just the server and using the [passlib hashing library](
+https://passlib.readthedocs.io/en/stable/index.html). The server nonce and salt is
 specified in order to give a reproducible example, but in production you'd omit the
-``s_nonce`` and ``salt`` parameters and let Scramp generate them:
+`s_nonce` and `salt` parameters and let Scramp generate them:
 
+```python
 >>> from scramp import ScramMechanism
 >>> from passlib.hash import scram
 >>>
 >>> USERNAME = 'user'
 >>> PASSWORD = 'pencil'
 >>> S_NONCE = '%hvYDpWUa2RaTCAfuxFIlj)hNlF$k0'
 >>> SALT = b'[m\x99h\x9d\x125\x8e\xec\xa0K\x14\x126\xfa\x81'
@@ -253,23 +225,24 @@
 >>> # Get the final server message and send it to the client
 >>> sfinal = s.get_server_final()
 >>> print(sfinal)
 v=6rriTRBi23WpRR/wtup+mMhUZUn/dB5nLTJRsjl95G4=
 >>>
 >>> # If it all runs through without raising an exception, the authentication
 >>> # has succeeded
+```
 
 
-Server Error
-````````````
+### Server Error
 
 Here's an example of when setting a message from the client causes an error. The server
 nonce and salt is specified in order to give a reproducible example, but in production
-you'd omit the ``s_nonce`` and ``salt`` parameters and let Scramp generate them:
+you'd omit the `s_nonce` and `salt` parameters and let Scramp generate them:
 
+```python
 >>> from scramp import ScramException, ScramMechanism
 >>>
 >>> USERNAME = 'user'
 >>> PASSWORD = 'pencil'
 >>> S_NONCE = '%hvYDpWUa2RaTCAfuxFIlj)hNlF$k0'
 >>> SALT = b'[m\x99h\x9d\x125\x8e\xec\xa0K\x14\x126\xfa\x81'
 >>>
@@ -298,311 +271,187 @@
 ...     print(e)
 ...     # Get the final server message and send it to the client
 ...     sfinal = s.get_server_final()
 ...     print(sfinal)
 Received GS2 flag 'p' which indicates that the client requires channel binding, but the server does not: channel-binding-not-supported
 e=channel-binding-not-supported
 
+```
 
-Standards
----------
 
-`RFC 5802 <https://tools.ietf.org/html/rfc5802>`_
-  Describes SCRAM.
-`RFC 7677 <https://datatracker.ietf.org/doc/html/rfc7677>`_
-  Registers SCRAM-SHA-256 and SCRAM-SHA-256-PLUS.
-`draft-melnikov-scram-sha-512-02 <https://datatracker.ietf.org/doc/html/draft-melnikov-scram-sha-512>`_
-  Registers SCRAM-SHA-512 and SCRAM-SHA-512-PLUS.
-`draft-melnikov-scram-sha3-512 <https://datatracker.ietf.org/doc/html/draft-melnikov-scram-sha3-512>`_
-  Registers SCRAM-SHA3-512 and SCRAM-SHA3-512-PLUS.
-`RFC 5929 <https://datatracker.ietf.org/doc/html/rfc5929>`_
-  Channel Bindings for TLS.
-`draft-ietf-kitten-tls-channel-bindings-for-tls13 <https://datatracker.ietf.org/doc/html/draft-ietf-kitten-tls-channel-bindings-for-tls13>`_
-  Defines the ``tls-exporter`` channel binding, which is `not yet supported by Scramp
-  <https://github.com/tlocke/scramp/issues/9>`_.
+### Standards
 
+- [RFC 5802](https://tools.ietf.org/html/rfc5802>) Describes SCRAM.
+- [RFC 7677](https://datatracker.ietf.org/doc/html/rfc7677>) Registers SCRAM-SHA-256 and SCRAM-SHA-256-PLUS.
+- [draft-melnikov-scram-sha-512-02](https://datatracker.ietf.org/doc/html/draft-melnikov-scram-sha-512) Registers SCRAM-SHA-512 and SCRAM-SHA-512-PLUS.
+- [draft-melnikov-scram-sha3-512](https://datatracker.ietf.org/doc/html/draft-melnikov-scram-sha3-512) Registers SCRAM-SHA3-512 and SCRAM-SHA3-512-PLUS.
+- [RFC 5929](https://datatracker.ietf.org/doc/html/rfc5929) Channel Bindings for TLS.
+- [draft-ietf-kitten-tls-channel-bindings-for-tls13](https://datatracker.ietf.org/doc/html/draft-ietf-kitten-tls-channel-bindings-for-tls13>) Defines the `tls-exporter` channel binding, which is [not yet supported by Scramp](https://github.com/tlocke/scramp/issues/9).
 
-API Docs
---------
 
+## API Docs
 
-scramp.MECHANISMS
-`````````````````
 
-A tuple of the supported mechanism names.
-
-
-scramp.ScramClient
-``````````````````
-
-``ScramClient(mechanisms, username, password, channel_binding=None, c_nonce=None)``
-  Constructor of the ``ScramClient`` class, with the following parameters:
-
-  ``mechanisms``
-    A list or tuple of mechanism names. ScramClient will choose the most secure. If
-    ``cbind_data`` is ``None``, the '-PLUS' variants will be filtered out first. The
-    chosen mechanism is available as the property ``mechanism_name``.
-
-  ``username``
-
-  ``password``
-
-  ``channel_binding``
-    Providing a value for this parameter allows channel binding to be used (ie. it lets
-    you use mechanisms ending in '-PLUS'). The value for ``channel_binding`` is a tuple
-    consisting of the channel binding name and the channel binding data. For example, if
-    the channel binding name is ``tls-unique``, the ``channel_binding`` parameter would
-    be ``('tls-unique', data)``, where ``data`` is obtained by calling
-    `SSLSocket.get_channel_binding()
-    <https://docs.python.org/3/library/ssl.html#ssl.SSLSocket.get_channel_binding>`_.
-    The convenience function ``scramp.make_channel_binding()`` can be used to create a
-    channel binding tuple.
-
-  ``c_nonce``
-    The client nonce. It's sometimes useful to set this when testing / debugging, but in
-    production this should be omitted, in which case ``ScramClient`` will generate a
-    client nonce.
+### scramp.MECHANISMS
 
-The ``ScramClient`` object has the following methods and properties:
-
-``get_client_first()``
-  Get the client first message.
-``set_server_first(message)``
-    Set the first message from the server.
-``get_client_final()``
-  Get the final client message.
-``set_server_final(message)``
-  Set the final message from the server.
-``mechanism_name``
-  The mechanism chosen from the list given in the constructor.
-
-
-scramp.ScramMechanism
-`````````````````````
-
-``ScramMechanism(mechanism='SCRAM-SHA-256')``
-  Constructor of the ``ScramMechanism`` class, with the following parameter:
+A tuple of the supported mechanism names.
 
-  ``mechanism``
-    The SCRAM mechanism to use.
 
-The ``ScramMechanism`` object has the following methods and properties:
+### scramp.ScramClient
 
-``make_auth_info(password, iteration_count=None, salt=None)``
-  returns the tuple ``(salt, stored_key, server_key, iteration_count)`` which is stored
-  in the authentication database on the server side. It has the following parameters:
+`ScramClient(mechanisms, username, password, channel_binding=None, c_nonce=None)`
 
-  ``password``
-    The user's password as a ``str``.
+Constructor of the `scramp.ScramClient` class, with the following parameters:
 
-  ``iteration_count``
-    The rounds as an ``int``. If ``None`` then use the minimum associated with the
-    mechanism.
-  ``salt``
-    It's sometimes useful to set this binary parameter when testing / debugging, but in
-    production this should be omitted, in which case a salt will be generated.
+- `mechanisms` - A list or tuple of mechanism names. ScramClient will choose the most secure. If `cbind_data` is `None`, the '-PLUS' variants will be filtered out first. The chosen mechanism is available as the property `mechanism_name`.
+- `username`
+- `password`
+- `channel_binding` - Providing a value for this parameter allows channel binding to be used (ie. it lets you use mechanisms ending in '-PLUS'). The value for `channel_binding` is a tuple consisting of the channel binding name and the channel binding data. For example, if the channel binding name is `tls-unique`, the `channel_binding` parameter would be `('tls-unique', data)`, where `data` is obtained by calling [SSLSocket.get\_channel\_binding()](https://docs.python.org/3/library/ssl.html#ssl.SSLSocket.get_channel_binding). The convenience function `scramp.make_channel_binding()` can be used to create a channel binding tuple.
+- `c_nonce` - The client nonce. It's sometimes useful to set this when testing / debugging, but in production this should be omitted, in which case `ScramClient` will generate a client nonce.
 
-``make_server(auth_fn, channel_binding=None, s_nonce=None)``
-    returns a ``ScramServer`` object. It takes the following parameters:
+The `ScramClient` object has the following methods and properties:
 
-  ``auth_fn``
-    This is a function provided by the programmer that has one parameter, a username of
-    type ``str`` and returns returns the tuple ``(salt, stored_key, server_key,
-    iteration_count)``. Where ``salt``, ``stored_key`` and ``server_key`` are of a
-    binary type, and ``iteration_count`` is an ``int``.
+- `get_client_first()` - Get the client first message.
+- `set_server_first(message)` - Set the first message from the server.
+- `get_client_final()` - Get the final client message.
+- `set_server_final(message)` - Set the final message from the server.
+- `mechanism_name` - The mechanism chosen from the list given in the constructor.
 
-  ``channel_binding``
-    Providing a value for this parameter allows channel binding to be used (ie.  it lets
-    you use mechanisms ending in ``-PLUS``). The value for ``channel_binding`` is a
-    tuple consisting of the channel binding name and the channel binding data. For
-    example, if the channel binding name is 'tls-unique', the ``channel_binding``
-    parameter would be ``('tls-unique', data)``, where ``data`` is obtained by calling
-    `SSLSocket.get_channel_binding()
-    <https://docs.python.org/3/library/ssl.html#ssl.SSLSocket.get_channel_binding>`_.
-    The convenience function ``scramp.make_channel_binding()`` can be used to create a
-    channel binding tuple. If ``channel_binding`` is provided and the mechanism isn't a
-    ``-PLUS`` variant, then the server will negotiate with the client to use the
-    ``-PLUS`` variant if the client supports it, or otherwise to use the mechanism
-    without channel binding.
 
-  ``s_nonce``
-    The server nonce as a ``str``. It's sometimes useful to set this when testing /
-    debugging, but in production this should be omitted, in which case ``ScramServer``
-    will generate a server nonce.
+### scramp.ScramMechanism
 
-``make_stored_server_keys(salted_password)``
-    returns ``(stored_key, server_key)`` tuple of ``bytes`` objects given a salted
-    password. This is useful if you want to use a separate hashing implementation from
-    the one provided by Scramp. It takes the following parameter:
+`ScramMechanism(mechanism='SCRAM-SHA-256')`
 
-  ``salted_password``
-    A binary object representing the hashed password.
+Constructor of the `ScramMechanism` class, with the following parameter:
 
-``iteration_count``
-    The minimum iteration count recommended for this mechanism.
+- `mechanism` - The SCRAM mechanism to use.
 
+The `ScramMechanism` object has the following methods and properties:
 
-scramp.ScramServer
-``````````````````
+- `make_auth_info(password, iteration_count=None, salt=None)` - Returns the tuple `(salt, stored_key, server_key, iteration_count)` which is stored in the authentication database on the server side. It has the following parameters:
+  - `password` - The user's password as a `str`.
+  - `iteration_count` - The rounds as an `int`. If `None` then use the minimum associated with the mechanism.
+  - `salt` - It's sometimes useful to set this binary parameter when testing / debugging, but in production this should be omitted, in which case a salt will be generated.
+- `make_server(auth_fn, channel_binding=None, s_nonce=None)` - returns a `ScramServer` object. It takes the following parameters:
+  - `auth_fn` This is a function provided by the programmer that has one parameter, a username of type `str` and returns returns the tuple `(salt, stored_key, server_key, iteration_count)`. Where `salt`, `stored_key` and `server_key` are of a binary type, and `iteration_count` is an `int`.
+  - `channel_binding` - Providing a value for this parameter allows channel binding to be used (ie.  it lets you use mechanisms ending in `-PLUS`). The value for `channel_binding` is a tuple consisting of the channel binding name and the channel binding data. For example, if the channel binding name is 'tls-unique', the `channel_binding` parameter would be `('tls-unique', data)`, where `data` is obtained by calling [SSLSocket.get\_channel\_binding()](https://docs.python.org/3/library/ssl.html#ssl.SSLSocket.get_channel_binding>). The convenience function `scramp.make_channel_binding()` can be used to create a channel binding tuple. If `channel_binding` is provided and the mechanism isn't a `-PLUS` variant, then the server will negotiate with the client to use the `-PLUS` variant if the client supports it, or otherwise to use the mechanism without channel binding.
+  - `s_nonce` - The server nonce as a `str`. It's sometimes useful to set this when testing / debugging, but in production this should be omitted, in which case `ScramServer` will generate a server nonce.
+- `make_stored_server_keys(salted_password)` - Returns `(stored_key, server_key)` tuple of `bytes` objects given a salted password. This is useful if you want to use a separate hashing implementation from the one provided by Scramp. It takes the following parameter:
+  - `salted_password` - A binary object representing the hashed password.
+- `iteration_count` - The minimum iteration count recommended for this mechanism.
 
-The ``ScramServer`` object has the following methods:
 
-``set_client_first(message)``
-  Set the first message from the client.
+### scramp.ScramServer
 
-``get_server_first()``
-  Get the server first message.
+The `ScramServer` object has the following methods:
 
-``set_client_final(message)``
-  Set the final client message.
+- `set_client_first(message)` - Set the first message from the client.
+- `get_server_first()` - Get the server first message.
+- `set_client_final(message)` - Set the final client message.
+- `get_server_final()` - Get the server final message.
 
-``get_server_final()``
-  Get the server final message.
 
+### scramp.make\_channel\_binding(name, ssl\_socket)
 
-scramp.make_channel_binding()
-`````````````````````````````
+A helper function that makes a `channel_binding` tuple when given a channel binding name and an SSL socket. The parameters are:
+- `name` - A channel binding name such as 'tls-unique' or 'tls-server-end-point'.
+- `ssl_socket` - An instance of [ssl.SSLSocket](https://docs.python.org/3/library/ssl.html#ssl.SSLSocket).
 
-``make_channel_binding(name, ssl_socket)``
-  A helper function that makes a ``channel_binding`` tuple when given a channel binding
-  name and an SSL socket. The parameters are:
 
-  ``name``
-    A channel binding name such as 'tls-unique' or 'tls-server-end-point'.
+## Testing
 
-  ``ssl_socket``
-    An instance of `ssl.SSLSocket
-    <https://docs.python.org/3/library/ssl.html#ssl.SSLSocket>`_.
+- Activate the virtual environment: `source venv/bin/activate`
+- Install `tox`: `pip install tox`
+- Run `tox`: `tox`
 
 
-README.rst
-----------
+## OpenSSF Scorecard
 
-This file is written in the `reStructuredText
-<https://docutils.sourceforge.io/docs/user/rst/quickref.html>`_ format. To generate an
-HTML page from it, do:
+It might be worth running the [OpenSSF Scorecard](https://securityscorecards.dev/):
 
-- Activate the virtual environment: ``source venv/bin/activate``
-- Install ``Sphinx``: ``pip install Sphinx``
-- Run ``rst2html.py``: ``rst2html.py README.rst README.html``
+`sudo docker run -e GITHUB_AUTH_TOKEN=<auth_token> gcr.io/openssf/scorecard:stable --repo=github.com/tlocke/scramp`
 
 
-Testing
--------
+## Doing A Release Of Scramp
 
-- Activate the virtual environment: ``source venv/bin/activate``
-- Install ``tox``: ``pip install tox``
-- Run ``tox``: ``tox``
+Run `tox` to make sure all tests pass, then update the release notes, then do:
 
+- `git tag -a x.y.z -m "version x.y.z"`
+- `rm -r dist`
+- `python -m build`
+- `twine upload dist/*`
 
-Doing A Release Of Scramp
--------------------------
 
-Run ``tox`` to make sure all tests pass, then update the release notes, then do::
+## Release Notes
 
-  git tag -a x.y.z -m "version x.y.z"
-  rm -r dist
-  python -m build
-  twine upload --sign dist/*
+### Version 1.4.5, 2024-04-13
 
+- Drop support for Python 3.7, which means we're not dependent on `importlib-metadata` anymore.
+- Various changes to build system, docs and automated testing.
 
-Release Notes
--------------
 
-Version 1.4.4, 2022-11-01
-`````````````````````````
+### Version 1.4.4, 2022-11-01
 
-- Tighten up parsing of messages to make sure that a ``ScramException`` is raised if a
-  message is malformed.
+- Tighten up parsing of messages to make sure that a `ScramException` is raised if a message is malformed.
 
 
-Version 1.4.3, 2022-10-26
-`````````````````````````
+### Version 1.4.3, 2022-10-26
 
-- The client now sends a gs2-cbind-flag of 'y' if the client supports channel
-  binding, but thinks the server does not.
+- The client now sends a gs2-cbind-flag of 'y' if the client supports channel binding, but thinks the server does not.
 
 
-Version 1.4.2, 2022-10-22
-`````````````````````````
+### Version 1.4.2, 2022-10-22
 
 - Switch to using the MIT-0 licence https://choosealicense.com/licenses/mit-0/
-
-- When creating a ScramClient, allow non ``-PLUS`` variants, even if a
-  ``channel_binding`` parameter is provided. Previously this would raise and
-  exception.
+- When creating a ScramClient, allow non ``-PLUS`` variants, even if a `channel_binding` parameter is provided. Previously this would raise and exception.
 
 
-Version 1.4.1, 2021-08-25
-`````````````````````````
+### Version 1.4.1, 2021-08-25
 
-- When using ``make_channel_binding()`` to create a tls-server-end-point channel
-  binding, support certificates with hash algorithm of sha512.
+- When using `make_channel_binding()` to create a tls-server-end-point channel binding, support certificates with hash algorithm of sha512.
 
 
-Version 1.4.0, 2021-03-28
-`````````````````````````
+### Version 1.4.0, 2021-03-28
 
 - Raise an exception if the client receives an error from the server.
 
 
-Version 1.3.0, 2021-03-28
-`````````````````````````
+### Version 1.3.0, 2021-03-28
 
-- As the specification allows, server errors are now sent to the client in the
-  ``server_final`` message, an exception is still thrown as before.
+- As the specification allows, server errors are now sent to the client in the `server_final` message, an exception is still thrown as before.
 
 
-Version 1.2.2, 2021-02-13
-`````````````````````````
+### Version 1.2.2, 2021-02-13
 
-- Fix bug in generating the AuthMessage. It was incorrect when channel binding
-  was used. So now Scramp supports channel binding.
+- Fix bug in generating the AuthMessage. It was incorrect when channel binding was used. So now Scramp supports channel binding.
 
 
-Version 1.2.1, 2021-02-07
-`````````````````````````
+### Version 1.2.1, 2021-02-07
 
 - Add support for channel binding.
+- Add support for SCRAM-SHA-512 and SCRAM-SHA3-512 and their channel binding variants.
 
-- Add support for SCRAM-SHA-512 and SCRAM-SHA3-512 and their channel binding
-  variants.
-
-
-Version 1.2.0, 2020-05-30
-`````````````````````````
 
-- This is a backwardly incompatible change on the server side, the client side will
-  work as before. The idea of this change is to make it possible to have an
-  authentication database. That is, the authentication information can be stored, and
-  then retrieved when needed to authenticate the user.
+### Version 1.2.0, 2020-05-30
 
-- In addition, it's now possible on the server side to use a third party hashing library
-  such as passlib as the hashing implementation.
+- This is a backwardly incompatible change on the server side, the client side will work as before. The idea of this change is to make it possible to have an authentication database. That is, the authentication information can be stored, and then retrieved when needed to authenticate the user.
+- In addition, it's now possible on the server side to use a third party hashing library such as passlib as the hashing implementation.
 
 
-Version 1.1.1, 2020-03-28
-`````````````````````````
+### Version 1.1.1, 2020-03-28
 
 - Add the README and LICENCE to the distribution.
 
 
-Version 1.1.0, 2019-02-24
-`````````````````````````
+### Version 1.1.0, 2019-02-24
 
 - Add support for the SCRAM-SHA-1 mechanism.
 
 
-Version 1.0.0, 2019-02-17
-`````````````````````````
+### Version 1.0.0, 2019-02-17
 
 - Implement the server side as well as the client side.
 
 
-Version 0.0.0, 2019-02-10
-`````````````````````````
+### Version 0.0.0, 2019-02-10
 
-- Copied SCRAM implementation from `pg8000 <https://github.com/tlocke/pg8000>`_. The
-  idea is to make it a general SCRAM implemtation. Credit to the `Scrampy
-  <https://github.com/cagdass/scrampy>`_ project which I read through to help with this
-  project. Also credit to the `passlib <https://github.com/efficks/passlib>`_ project
-  from which I copied the ``saslprep`` function.
+- Copied SCRAM implementation from [pg8000](https://github.com/tlocke/pg8000). The idea is to make it a general SCRAM implemtation. Credit to the [Scrampy](https://github.com/cagdass/scrampy) project which I read through to help with this project. Also credit to the [passlib](https://github.com/efficks/passlib) project from which I copied the `saslprep` function.
```

### Comparing `scramp-1.4.4/pyproject.toml` & `scramp-1.4.5/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,63 +1,77 @@
 [build-system]
-requires = [
-    "setuptools>=61",
-    "versioningit >= 2.0.1",
-]
-build-backend = "setuptools.build_meta"
+requires = ["hatchling", "versioningit"]
+build-backend = "hatchling.build"
 
 [project]
 name = "scramp"
+authors = [{name = "The Contributors"}]
 description = "An implementation of the SCRAM protocol."
-readme = "README.rst"
-requires-python = ">=3.7"
+readme = "README.md"
+requires-python = ">=3.8"
 keywords = ["SCRAM", "authentication", "SASL"]
 license = {text = "MIT No Attribution"}
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT No Attribution License (MIT-0)",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "asn1crypto >= 1.5.1",
-    'importlib-metadata >= 1.0 ; python_version < "3.8"',
 ]
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://github.com/tlocke/scramp"
 
+[tool.hatch.version]
+source = "versioningit"
+
 [tool.versioningit]
 
 [tool.versioningit.vcs]
 method = "git"
 default-tag = "0.0.0"
 
+[tool.flake8]
+application-names = ["scramp"]
+ignore = ["E203", "W503"]
+max-line-length = 88
+exclude = [".git", "__pycache__", "build", "dist", "venv", ".tox"]
+application-import-names = ["scramp"]
+
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 isolated_build = True
 envlist = py
 
 [testenv]
+allowlist_externals=/usr/bin/rm
 commands =
     black --check .
     flake8 .
     pytest -v -x -W error test
+    rm -rf dist
+    python -m build
+    twine check dist/*
 deps =
+    build
     pytest
     pytest-mock
     black
     flake8
+    Flake8-pyproject
     flake8-alphabetize
     passlib
+    twine
 """
```

### Comparing `scramp-1.4.4/scramp/core.py` & `scramp-1.4.5/src/scramp/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -277,15 +277,14 @@
             raise e
 
     return wrapper
 
 
 class ScramServer:
     def __init__(self, mechanism, auth_fn, channel_binding=None, s_nonce=None):
-
         _validate_channel_binding(channel_binding)
 
         self.channel_binding = channel_binding
         self.s_nonce = _make_nonce() if s_nonce is None else s_nonce
         self.auth_fn = auth_fn
         self.stage = None
         self.server_signature = None
@@ -592,15 +591,14 @@
     stored_key,
     server_key,
     client_first_bare,
     server_first,
     channel_binding,
     use_binding,
 ):
-
     msg = _parse_message(client_final, "client final", "crp")
     chan_binding = msg["c"]
 
     nonce = msg["r"]
     proof = msg["p"]
     if use_binding and b64dec(chan_binding) != _make_cbind_input(
         channel_binding, use_binding
```

### Comparing `scramp-1.4.4/scramp/utils.py` & `scramp-1.4.5/src/scramp/utils.py`

 * *Files identical despite different names*

### Comparing `scramp-1.4.4/scramp.egg-info/PKG-INFO` & `scramp-1.4.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,69 +1,64 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: scramp
-Version: 1.4.4
+Version: 1.4.5
 Summary: An implementation of the SCRAM protocol.
-License: MIT No Attribution
 Project-URL: Homepage, https://github.com/tlocke/scramp
-Keywords: SCRAM,authentication,SASL
+Author: The Contributors
+License: MIT No Attribution
+License-File: LICENSE
+Keywords: SASL,SCRAM,authentication
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT No Attribution License (MIT-0)
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-License-File: LICENSE
+Requires-Python: >=3.8
+Requires-Dist: asn1crypto>=1.5.1
+Description-Content-Type: text/markdown
 
-======
-Scramp
-======
+# Scramp
 
-A Python implementation of the `SCRAM authentication protocol
-<https://en.wikipedia.org/wiki/Salted_Challenge_Response_Authentication_Mechanism>`_.
+A Python implementation of the [SCRAM authentication protocol](
+https://en.wikipedia.org/wiki/Salted_Challenge_Response_Authentication_Mechanism>).
 Scramp supports the following mechanisms:
 
 - SCRAM-SHA-1
 - SCRAM-SHA-1-PLUS
 - SCRAM-SHA-256
 - SCRAM-SHA-256-PLUS
 - SCRAM-SHA-512
 - SCRAM-SHA-512-PLUS
 - SCRAM-SHA3-512
 - SCRAM-SHA3-512-PLUS
 
-.. contents:: Table of Contents
-   :depth: 2
-   :local:
 
-Installation
-------------
+## Installation
 
-- Create a virtual environment: ``python3 -m venv venv``
-- Activate the virtual environment: ``source venv/bin/activate``
-- Install: ``pip install scramp``
+- Create a virtual environment: `python3 -m venv venv`
+- Activate the virtual environment: `source venv/bin/activate`
+- Install: `pip install scramp`
 
 
-Examples
---------
+## Examples
 
-Client and Server
-`````````````````
+### Client and Server
 
 Here's an example using both the client and the server. It's a bit contrived as normally
 you'd be using either the client or server on its own.
 
+```python
 >>> from scramp import ScramClient, ScramMechanism
 >>>
 >>> USERNAME = 'user'
 >>> PASSWORD = 'pencil'
 >>> MECHANISMS = ['SCRAM-SHA-256']
 >>>
 >>>
@@ -100,23 +95,24 @@
 >>> s.set_client_final(cfinal)
 >>> sfinal = s.get_server_final()
 >>>
 >>> c.set_server_final(sfinal)
 >>>
 >>> # If it all runs through without raising an exception, the authentication
 >>> # has succeeded
+```
 
 
-Client only
-```````````
+### Client only
 
 Here's an example using just the client. The client nonce is specified in order to give
-a reproducible example, but in production you'd omit the ``c_nonce`` parameter and let
-``ScramClient`` generate a client nonce:
+a reproducible example, but in production you'd omit the `c_nonce` parameter and let
+`ScramClient` generate a client nonce:
 
+```python
 >>> from scramp import ScramClient
 >>>
 >>> USERNAME = 'user'
 >>> PASSWORD = 'pencil'
 >>> C_NONCE = 'rOprNGfwEbeRWgbNEkqO'
 >>> MECHANISMS = ['SCRAM-SHA-256']
 >>>
@@ -141,23 +137,24 @@
 c=biws,r=rOprNGfwEbeRWgbNEkqO%hvYDpWUa2RaTCAfuxFIlj)hNlF$k0,p=dHzbZapWIk4jUhN+Ute9ytag9zjfMHgsqmmiz7AndVQ=
 >>>
 >>> # Set the final message from the server
 >>> c.set_server_final('v=6rriTRBi23WpRR/wtup+mMhUZUn/dB5nLTJRsjl95G4=')
 >>>
 >>> # If it all runs through without raising an exception, the authentication
 >>> # has succeeded
+```
 
 
-Server only
-```````````
+### Server only
 
 Here's an example using just the server. The server nonce and salt is specified in order
-to give a reproducible example, but in production you'd omit the ``s_nonce`` and
-``salt`` parameters and let Scramp generate them:
+to give a reproducible example, but in production you'd omit the `s_nonce` and `salt`
+parameters and let Scramp generate them:
 
+```python
 >>> from scramp import ScramMechanism
 >>>
 >>> USERNAME = 'user'
 >>> PASSWORD = 'pencil'
 >>> S_NONCE = '%hvYDpWUa2RaTCAfuxFIlj)hNlF$k0'
 >>> SALT = b'[m\x99h\x9d\x125\x8e\xec\xa0K\x14\x126\xfa\x81'
 >>>
@@ -195,24 +192,25 @@
 >>> # Get the final server message and send it to the client
 >>> sfinal = s.get_server_final()
 >>> print(sfinal)
 v=6rriTRBi23WpRR/wtup+mMhUZUn/dB5nLTJRsjl95G4=
 >>>
 >>> # If it all runs through without raising an exception, the authentication
 >>> # has succeeded
+```
 
 
-Server only with passlib
-````````````````````````
+### Server only with passlib
 
-Here's an example using just the server and using the `passlib hashing library
-<https://passlib.readthedocs.io/en/stable/index.html>`_. The server nonce and salt is
+Here's an example using just the server and using the [passlib hashing library](
+https://passlib.readthedocs.io/en/stable/index.html). The server nonce and salt is
 specified in order to give a reproducible example, but in production you'd omit the
-``s_nonce`` and ``salt`` parameters and let Scramp generate them:
+`s_nonce` and `salt` parameters and let Scramp generate them:
 
+```python
 >>> from scramp import ScramMechanism
 >>> from passlib.hash import scram
 >>>
 >>> USERNAME = 'user'
 >>> PASSWORD = 'pencil'
 >>> S_NONCE = '%hvYDpWUa2RaTCAfuxFIlj)hNlF$k0'
 >>> SALT = b'[m\x99h\x9d\x125\x8e\xec\xa0K\x14\x126\xfa\x81'
@@ -253,23 +251,24 @@
 >>> # Get the final server message and send it to the client
 >>> sfinal = s.get_server_final()
 >>> print(sfinal)
 v=6rriTRBi23WpRR/wtup+mMhUZUn/dB5nLTJRsjl95G4=
 >>>
 >>> # If it all runs through without raising an exception, the authentication
 >>> # has succeeded
+```
 
 
-Server Error
-````````````
+### Server Error
 
 Here's an example of when setting a message from the client causes an error. The server
 nonce and salt is specified in order to give a reproducible example, but in production
-you'd omit the ``s_nonce`` and ``salt`` parameters and let Scramp generate them:
+you'd omit the `s_nonce` and `salt` parameters and let Scramp generate them:
 
+```python
 >>> from scramp import ScramException, ScramMechanism
 >>>
 >>> USERNAME = 'user'
 >>> PASSWORD = 'pencil'
 >>> S_NONCE = '%hvYDpWUa2RaTCAfuxFIlj)hNlF$k0'
 >>> SALT = b'[m\x99h\x9d\x125\x8e\xec\xa0K\x14\x126\xfa\x81'
 >>>
@@ -298,311 +297,187 @@
 ...     print(e)
 ...     # Get the final server message and send it to the client
 ...     sfinal = s.get_server_final()
 ...     print(sfinal)
 Received GS2 flag 'p' which indicates that the client requires channel binding, but the server does not: channel-binding-not-supported
 e=channel-binding-not-supported
 
+```
 
-Standards
----------
 
-`RFC 5802 <https://tools.ietf.org/html/rfc5802>`_
-  Describes SCRAM.
-`RFC 7677 <https://datatracker.ietf.org/doc/html/rfc7677>`_
-  Registers SCRAM-SHA-256 and SCRAM-SHA-256-PLUS.
-`draft-melnikov-scram-sha-512-02 <https://datatracker.ietf.org/doc/html/draft-melnikov-scram-sha-512>`_
-  Registers SCRAM-SHA-512 and SCRAM-SHA-512-PLUS.
-`draft-melnikov-scram-sha3-512 <https://datatracker.ietf.org/doc/html/draft-melnikov-scram-sha3-512>`_
-  Registers SCRAM-SHA3-512 and SCRAM-SHA3-512-PLUS.
-`RFC 5929 <https://datatracker.ietf.org/doc/html/rfc5929>`_
-  Channel Bindings for TLS.
-`draft-ietf-kitten-tls-channel-bindings-for-tls13 <https://datatracker.ietf.org/doc/html/draft-ietf-kitten-tls-channel-bindings-for-tls13>`_
-  Defines the ``tls-exporter`` channel binding, which is `not yet supported by Scramp
-  <https://github.com/tlocke/scramp/issues/9>`_.
-
-
-API Docs
---------
-
-
-scramp.MECHANISMS
-`````````````````
-
-A tuple of the supported mechanism names.
+### Standards
 
+- [RFC 5802](https://tools.ietf.org/html/rfc5802>) Describes SCRAM.
+- [RFC 7677](https://datatracker.ietf.org/doc/html/rfc7677>) Registers SCRAM-SHA-256 and SCRAM-SHA-256-PLUS.
+- [draft-melnikov-scram-sha-512-02](https://datatracker.ietf.org/doc/html/draft-melnikov-scram-sha-512) Registers SCRAM-SHA-512 and SCRAM-SHA-512-PLUS.
+- [draft-melnikov-scram-sha3-512](https://datatracker.ietf.org/doc/html/draft-melnikov-scram-sha3-512) Registers SCRAM-SHA3-512 and SCRAM-SHA3-512-PLUS.
+- [RFC 5929](https://datatracker.ietf.org/doc/html/rfc5929) Channel Bindings for TLS.
+- [draft-ietf-kitten-tls-channel-bindings-for-tls13](https://datatracker.ietf.org/doc/html/draft-ietf-kitten-tls-channel-bindings-for-tls13>) Defines the `tls-exporter` channel binding, which is [not yet supported by Scramp](https://github.com/tlocke/scramp/issues/9).
 
-scramp.ScramClient
-``````````````````
 
-``ScramClient(mechanisms, username, password, channel_binding=None, c_nonce=None)``
-  Constructor of the ``ScramClient`` class, with the following parameters:
+## API Docs
 
-  ``mechanisms``
-    A list or tuple of mechanism names. ScramClient will choose the most secure. If
-    ``cbind_data`` is ``None``, the '-PLUS' variants will be filtered out first. The
-    chosen mechanism is available as the property ``mechanism_name``.
 
-  ``username``
+### scramp.MECHANISMS
 
-  ``password``
-
-  ``channel_binding``
-    Providing a value for this parameter allows channel binding to be used (ie. it lets
-    you use mechanisms ending in '-PLUS'). The value for ``channel_binding`` is a tuple
-    consisting of the channel binding name and the channel binding data. For example, if
-    the channel binding name is ``tls-unique``, the ``channel_binding`` parameter would
-    be ``('tls-unique', data)``, where ``data`` is obtained by calling
-    `SSLSocket.get_channel_binding()
-    <https://docs.python.org/3/library/ssl.html#ssl.SSLSocket.get_channel_binding>`_.
-    The convenience function ``scramp.make_channel_binding()`` can be used to create a
-    channel binding tuple.
-
-  ``c_nonce``
-    The client nonce. It's sometimes useful to set this when testing / debugging, but in
-    production this should be omitted, in which case ``ScramClient`` will generate a
-    client nonce.
-
-The ``ScramClient`` object has the following methods and properties:
-
-``get_client_first()``
-  Get the client first message.
-``set_server_first(message)``
-    Set the first message from the server.
-``get_client_final()``
-  Get the final client message.
-``set_server_final(message)``
-  Set the final message from the server.
-``mechanism_name``
-  The mechanism chosen from the list given in the constructor.
-
-
-scramp.ScramMechanism
-`````````````````````
-
-``ScramMechanism(mechanism='SCRAM-SHA-256')``
-  Constructor of the ``ScramMechanism`` class, with the following parameter:
+A tuple of the supported mechanism names.
 
-  ``mechanism``
-    The SCRAM mechanism to use.
 
-The ``ScramMechanism`` object has the following methods and properties:
+### scramp.ScramClient
 
-``make_auth_info(password, iteration_count=None, salt=None)``
-  returns the tuple ``(salt, stored_key, server_key, iteration_count)`` which is stored
-  in the authentication database on the server side. It has the following parameters:
+`ScramClient(mechanisms, username, password, channel_binding=None, c_nonce=None)`
 
-  ``password``
-    The user's password as a ``str``.
+Constructor of the `scramp.ScramClient` class, with the following parameters:
 
-  ``iteration_count``
-    The rounds as an ``int``. If ``None`` then use the minimum associated with the
-    mechanism.
-  ``salt``
-    It's sometimes useful to set this binary parameter when testing / debugging, but in
-    production this should be omitted, in which case a salt will be generated.
+- `mechanisms` - A list or tuple of mechanism names. ScramClient will choose the most secure. If `cbind_data` is `None`, the '-PLUS' variants will be filtered out first. The chosen mechanism is available as the property `mechanism_name`.
+- `username`
+- `password`
+- `channel_binding` - Providing a value for this parameter allows channel binding to be used (ie. it lets you use mechanisms ending in '-PLUS'). The value for `channel_binding` is a tuple consisting of the channel binding name and the channel binding data. For example, if the channel binding name is `tls-unique`, the `channel_binding` parameter would be `('tls-unique', data)`, where `data` is obtained by calling [SSLSocket.get\_channel\_binding()](https://docs.python.org/3/library/ssl.html#ssl.SSLSocket.get_channel_binding). The convenience function `scramp.make_channel_binding()` can be used to create a channel binding tuple.
+- `c_nonce` - The client nonce. It's sometimes useful to set this when testing / debugging, but in production this should be omitted, in which case `ScramClient` will generate a client nonce.
 
-``make_server(auth_fn, channel_binding=None, s_nonce=None)``
-    returns a ``ScramServer`` object. It takes the following parameters:
+The `ScramClient` object has the following methods and properties:
 
-  ``auth_fn``
-    This is a function provided by the programmer that has one parameter, a username of
-    type ``str`` and returns returns the tuple ``(salt, stored_key, server_key,
-    iteration_count)``. Where ``salt``, ``stored_key`` and ``server_key`` are of a
-    binary type, and ``iteration_count`` is an ``int``.
+- `get_client_first()` - Get the client first message.
+- `set_server_first(message)` - Set the first message from the server.
+- `get_client_final()` - Get the final client message.
+- `set_server_final(message)` - Set the final message from the server.
+- `mechanism_name` - The mechanism chosen from the list given in the constructor.
 
-  ``channel_binding``
-    Providing a value for this parameter allows channel binding to be used (ie.  it lets
-    you use mechanisms ending in ``-PLUS``). The value for ``channel_binding`` is a
-    tuple consisting of the channel binding name and the channel binding data. For
-    example, if the channel binding name is 'tls-unique', the ``channel_binding``
-    parameter would be ``('tls-unique', data)``, where ``data`` is obtained by calling
-    `SSLSocket.get_channel_binding()
-    <https://docs.python.org/3/library/ssl.html#ssl.SSLSocket.get_channel_binding>`_.
-    The convenience function ``scramp.make_channel_binding()`` can be used to create a
-    channel binding tuple. If ``channel_binding`` is provided and the mechanism isn't a
-    ``-PLUS`` variant, then the server will negotiate with the client to use the
-    ``-PLUS`` variant if the client supports it, or otherwise to use the mechanism
-    without channel binding.
 
-  ``s_nonce``
-    The server nonce as a ``str``. It's sometimes useful to set this when testing /
-    debugging, but in production this should be omitted, in which case ``ScramServer``
-    will generate a server nonce.
+### scramp.ScramMechanism
 
-``make_stored_server_keys(salted_password)``
-    returns ``(stored_key, server_key)`` tuple of ``bytes`` objects given a salted
-    password. This is useful if you want to use a separate hashing implementation from
-    the one provided by Scramp. It takes the following parameter:
+`ScramMechanism(mechanism='SCRAM-SHA-256')`
 
-  ``salted_password``
-    A binary object representing the hashed password.
+Constructor of the `ScramMechanism` class, with the following parameter:
 
-``iteration_count``
-    The minimum iteration count recommended for this mechanism.
+- `mechanism` - The SCRAM mechanism to use.
 
+The `ScramMechanism` object has the following methods and properties:
 
-scramp.ScramServer
-``````````````````
+- `make_auth_info(password, iteration_count=None, salt=None)` - Returns the tuple `(salt, stored_key, server_key, iteration_count)` which is stored in the authentication database on the server side. It has the following parameters:
+  - `password` - The user's password as a `str`.
+  - `iteration_count` - The rounds as an `int`. If `None` then use the minimum associated with the mechanism.
+  - `salt` - It's sometimes useful to set this binary parameter when testing / debugging, but in production this should be omitted, in which case a salt will be generated.
+- `make_server(auth_fn, channel_binding=None, s_nonce=None)` - returns a `ScramServer` object. It takes the following parameters:
+  - `auth_fn` This is a function provided by the programmer that has one parameter, a username of type `str` and returns returns the tuple `(salt, stored_key, server_key, iteration_count)`. Where `salt`, `stored_key` and `server_key` are of a binary type, and `iteration_count` is an `int`.
+  - `channel_binding` - Providing a value for this parameter allows channel binding to be used (ie.  it lets you use mechanisms ending in `-PLUS`). The value for `channel_binding` is a tuple consisting of the channel binding name and the channel binding data. For example, if the channel binding name is 'tls-unique', the `channel_binding` parameter would be `('tls-unique', data)`, where `data` is obtained by calling [SSLSocket.get\_channel\_binding()](https://docs.python.org/3/library/ssl.html#ssl.SSLSocket.get_channel_binding>). The convenience function `scramp.make_channel_binding()` can be used to create a channel binding tuple. If `channel_binding` is provided and the mechanism isn't a `-PLUS` variant, then the server will negotiate with the client to use the `-PLUS` variant if the client supports it, or otherwise to use the mechanism without channel binding.
+  - `s_nonce` - The server nonce as a `str`. It's sometimes useful to set this when testing / debugging, but in production this should be omitted, in which case `ScramServer` will generate a server nonce.
+- `make_stored_server_keys(salted_password)` - Returns `(stored_key, server_key)` tuple of `bytes` objects given a salted password. This is useful if you want to use a separate hashing implementation from the one provided by Scramp. It takes the following parameter:
+  - `salted_password` - A binary object representing the hashed password.
+- `iteration_count` - The minimum iteration count recommended for this mechanism.
 
-The ``ScramServer`` object has the following methods:
 
-``set_client_first(message)``
-  Set the first message from the client.
+### scramp.ScramServer
 
-``get_server_first()``
-  Get the server first message.
+The `ScramServer` object has the following methods:
 
-``set_client_final(message)``
-  Set the final client message.
+- `set_client_first(message)` - Set the first message from the client.
+- `get_server_first()` - Get the server first message.
+- `set_client_final(message)` - Set the final client message.
+- `get_server_final()` - Get the server final message.
 
-``get_server_final()``
-  Get the server final message.
 
+### scramp.make\_channel\_binding(name, ssl\_socket)
 
-scramp.make_channel_binding()
-`````````````````````````````
+A helper function that makes a `channel_binding` tuple when given a channel binding name and an SSL socket. The parameters are:
+- `name` - A channel binding name such as 'tls-unique' or 'tls-server-end-point'.
+- `ssl_socket` - An instance of [ssl.SSLSocket](https://docs.python.org/3/library/ssl.html#ssl.SSLSocket).
 
-``make_channel_binding(name, ssl_socket)``
-  A helper function that makes a ``channel_binding`` tuple when given a channel binding
-  name and an SSL socket. The parameters are:
 
-  ``name``
-    A channel binding name such as 'tls-unique' or 'tls-server-end-point'.
+## Testing
 
-  ``ssl_socket``
-    An instance of `ssl.SSLSocket
-    <https://docs.python.org/3/library/ssl.html#ssl.SSLSocket>`_.
+- Activate the virtual environment: `source venv/bin/activate`
+- Install `tox`: `pip install tox`
+- Run `tox`: `tox`
 
 
-README.rst
-----------
+## OpenSSF Scorecard
 
-This file is written in the `reStructuredText
-<https://docutils.sourceforge.io/docs/user/rst/quickref.html>`_ format. To generate an
-HTML page from it, do:
+It might be worth running the [OpenSSF Scorecard](https://securityscorecards.dev/):
 
-- Activate the virtual environment: ``source venv/bin/activate``
-- Install ``Sphinx``: ``pip install Sphinx``
-- Run ``rst2html.py``: ``rst2html.py README.rst README.html``
+`sudo docker run -e GITHUB_AUTH_TOKEN=<auth_token> gcr.io/openssf/scorecard:stable --repo=github.com/tlocke/scramp`
 
 
-Testing
--------
+## Doing A Release Of Scramp
 
-- Activate the virtual environment: ``source venv/bin/activate``
-- Install ``tox``: ``pip install tox``
-- Run ``tox``: ``tox``
+Run `tox` to make sure all tests pass, then update the release notes, then do:
 
+- `git tag -a x.y.z -m "version x.y.z"`
+- `rm -r dist`
+- `python -m build`
+- `twine upload dist/*`
 
-Doing A Release Of Scramp
--------------------------
 
-Run ``tox`` to make sure all tests pass, then update the release notes, then do::
+## Release Notes
 
-  git tag -a x.y.z -m "version x.y.z"
-  rm -r dist
-  python -m build
-  twine upload --sign dist/*
+### Version 1.4.5, 2024-04-13
 
+- Drop support for Python 3.7, which means we're not dependent on `importlib-metadata` anymore.
+- Various changes to build system, docs and automated testing.
 
-Release Notes
--------------
 
-Version 1.4.4, 2022-11-01
-`````````````````````````
+### Version 1.4.4, 2022-11-01
 
-- Tighten up parsing of messages to make sure that a ``ScramException`` is raised if a
-  message is malformed.
+- Tighten up parsing of messages to make sure that a `ScramException` is raised if a message is malformed.
 
 
-Version 1.4.3, 2022-10-26
-`````````````````````````
+### Version 1.4.3, 2022-10-26
 
-- The client now sends a gs2-cbind-flag of 'y' if the client supports channel
-  binding, but thinks the server does not.
+- The client now sends a gs2-cbind-flag of 'y' if the client supports channel binding, but thinks the server does not.
 
 
-Version 1.4.2, 2022-10-22
-`````````````````````````
+### Version 1.4.2, 2022-10-22
 
 - Switch to using the MIT-0 licence https://choosealicense.com/licenses/mit-0/
-
-- When creating a ScramClient, allow non ``-PLUS`` variants, even if a
-  ``channel_binding`` parameter is provided. Previously this would raise and
-  exception.
+- When creating a ScramClient, allow non ``-PLUS`` variants, even if a `channel_binding` parameter is provided. Previously this would raise and exception.
 
 
-Version 1.4.1, 2021-08-25
-`````````````````````````
+### Version 1.4.1, 2021-08-25
 
-- When using ``make_channel_binding()`` to create a tls-server-end-point channel
-  binding, support certificates with hash algorithm of sha512.
+- When using `make_channel_binding()` to create a tls-server-end-point channel binding, support certificates with hash algorithm of sha512.
 
 
-Version 1.4.0, 2021-03-28
-`````````````````````````
+### Version 1.4.0, 2021-03-28
 
 - Raise an exception if the client receives an error from the server.
 
 
-Version 1.3.0, 2021-03-28
-`````````````````````````
+### Version 1.3.0, 2021-03-28
 
-- As the specification allows, server errors are now sent to the client in the
-  ``server_final`` message, an exception is still thrown as before.
+- As the specification allows, server errors are now sent to the client in the `server_final` message, an exception is still thrown as before.
 
 
-Version 1.2.2, 2021-02-13
-`````````````````````````
+### Version 1.2.2, 2021-02-13
 
-- Fix bug in generating the AuthMessage. It was incorrect when channel binding
-  was used. So now Scramp supports channel binding.
+- Fix bug in generating the AuthMessage. It was incorrect when channel binding was used. So now Scramp supports channel binding.
 
 
-Version 1.2.1, 2021-02-07
-`````````````````````````
+### Version 1.2.1, 2021-02-07
 
 - Add support for channel binding.
+- Add support for SCRAM-SHA-512 and SCRAM-SHA3-512 and their channel binding variants.
 
-- Add support for SCRAM-SHA-512 and SCRAM-SHA3-512 and their channel binding
-  variants.
-
-
-Version 1.2.0, 2020-05-30
-`````````````````````````
 
-- This is a backwardly incompatible change on the server side, the client side will
-  work as before. The idea of this change is to make it possible to have an
-  authentication database. That is, the authentication information can be stored, and
-  then retrieved when needed to authenticate the user.
+### Version 1.2.0, 2020-05-30
 
-- In addition, it's now possible on the server side to use a third party hashing library
-  such as passlib as the hashing implementation.
+- This is a backwardly incompatible change on the server side, the client side will work as before. The idea of this change is to make it possible to have an authentication database. That is, the authentication information can be stored, and then retrieved when needed to authenticate the user.
+- In addition, it's now possible on the server side to use a third party hashing library such as passlib as the hashing implementation.
 
 
-Version 1.1.1, 2020-03-28
-`````````````````````````
+### Version 1.1.1, 2020-03-28
 
 - Add the README and LICENCE to the distribution.
 
 
-Version 1.1.0, 2019-02-24
-`````````````````````````
+### Version 1.1.0, 2019-02-24
 
 - Add support for the SCRAM-SHA-1 mechanism.
 
 
-Version 1.0.0, 2019-02-17
-`````````````````````````
+### Version 1.0.0, 2019-02-17
 
 - Implement the server side as well as the client side.
 
 
-Version 0.0.0, 2019-02-10
-`````````````````````````
+### Version 0.0.0, 2019-02-10
 
-- Copied SCRAM implementation from `pg8000 <https://github.com/tlocke/pg8000>`_. The
-  idea is to make it a general SCRAM implemtation. Credit to the `Scrampy
-  <https://github.com/cagdass/scrampy>`_ project which I read through to help with this
-  project. Also credit to the `passlib <https://github.com/efficks/passlib>`_ project
-  from which I copied the ``saslprep`` function.
+- Copied SCRAM implementation from [pg8000](https://github.com/tlocke/pg8000). The idea is to make it a general SCRAM implemtation. Credit to the [Scrampy](https://github.com/cagdass/scrampy) project which I read through to help with this project. Also credit to the [passlib](https://github.com/efficks/passlib) project from which I copied the `saslprep` function.
```

### Comparing `scramp-1.4.4/test/test_scramp.py` & `scramp-1.4.5/test/test_scramp.py`

 * *Files identical despite different names*

