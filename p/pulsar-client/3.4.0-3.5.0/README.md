# Comparing `tmp/pulsar_client-3.4.0-cp39-cp39-win_amd64.whl.zip` & `tmp/pulsar_client-3.5.0-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,27 @@
-Zip file size: 3425712 bytes, number of entries: 18
--rw-rw-rw-  2.0 fat  8604160 b- defN 23-Dec-26 04:23 _pulsar.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat      828 b- defN 23-Dec-26 04:21 pulsar/__about__.py
--rw-rw-rw-  2.0 fat    75082 b- defN 23-Dec-26 04:21 pulsar/__init__.py
--rw-rw-rw-  2.0 fat     1815 b- defN 23-Dec-26 04:21 pulsar/exceptions.py
--rw-rw-rw-  2.0 fat      836 b- defN 23-Dec-26 04:21 pulsar/functions/__init__.py
--rw-rw-rw-  2.0 fat     6469 b- defN 23-Dec-26 04:21 pulsar/functions/context.py
--rw-rw-rw-  2.0 fat     2115 b- defN 23-Dec-26 04:21 pulsar/functions/function.py
--rw-rw-rw-  2.0 fat     3237 b- defN 23-Dec-26 04:21 pulsar/functions/serde.py
--rw-rw-rw-  2.0 fat     1053 b- defN 23-Dec-26 04:21 pulsar/schema/__init__.py
--rw-rw-rw-  2.0 fat    16843 b- defN 23-Dec-26 04:21 pulsar/schema/definition.py
--rw-rw-rw-  2.0 fat     3729 b- defN 23-Dec-26 04:21 pulsar/schema/schema.py
--rw-rw-rw-  2.0 fat     5685 b- defN 23-Dec-26 04:21 pulsar/schema/schema_avro.py
--rw-rw-rw-  2.0 fat    11560 b- defN 23-Dec-26 04:23 pulsar_client-3.4.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1073 b- defN 23-Dec-26 04:23 pulsar_client-3.4.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      172 b- defN 23-Dec-26 04:23 pulsar_client-3.4.0.dist-info/NOTICE
--rw-rw-rw-  2.0 fat      100 b- defN 23-Dec-26 04:23 pulsar_client-3.4.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       15 b- defN 23-Dec-26 04:23 pulsar_client-3.4.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1491 b- defN 23-Dec-26 04:23 pulsar_client-3.4.0.dist-info/RECORD
-18 files, 8736263 bytes uncompressed, 3423284 bytes compressed:  60.8%
+Zip file size: 5189598 bytes, number of entries: 25
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-02 08:35 pulsar_client.libs/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-02 08:35 pulsar/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-02 08:35 pulsar_client-3.5.0.dist-info/
+-rw-r--r--  2.0 unx  1874729 b- defN 24-Apr-02 08:35 _pulsar.cpython-312-aarch64-linux-gnu.so
+-rwxr-xr-x  2.0 unx 14562345 b- defN 24-Apr-02 08:35 pulsar_client.libs/libpulsar-7cf2e558.so
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-02 08:35 pulsar/schema/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-02 08:35 pulsar/functions/
+-rw-r--r--  2.0 unx    75652 b- defN 24-Apr-02 08:35 pulsar/__init__.py
+-rw-r--r--  2.0 unx     4858 b- defN 24-Apr-02 08:35 pulsar/asyncio.py
+-rw-r--r--  2.0 unx      809 b- defN 24-Apr-02 08:35 pulsar/__about__.py
+-rw-r--r--  2.0 unx     1787 b- defN 24-Apr-02 08:35 pulsar/exceptions.py
+-rw-r--r--  2.0 unx     1029 b- defN 24-Apr-02 08:35 pulsar/schema/__init__.py
+-rw-r--r--  2.0 unx     3610 b- defN 24-Apr-02 08:35 pulsar/schema/schema.py
+-rw-r--r--  2.0 unx     5596 b- defN 24-Apr-02 08:35 pulsar/schema/schema_avro.py
+-rw-r--r--  2.0 unx    16314 b- defN 24-Apr-02 08:35 pulsar/schema/definition.py
+-rw-r--r--  2.0 unx      816 b- defN 24-Apr-02 08:35 pulsar/functions/__init__.py
+-rw-r--r--  2.0 unx     3143 b- defN 24-Apr-02 08:35 pulsar/functions/serde.py
+-rw-r--r--  2.0 unx     2060 b- defN 24-Apr-02 08:35 pulsar/functions/function.py
+-rw-r--r--  2.0 unx     6269 b- defN 24-Apr-02 08:35 pulsar/functions/context.py
+-rw-rw-r--  2.0 unx     1700 b- defN 24-Apr-02 08:35 pulsar_client-3.5.0.dist-info/RECORD
+-rw-r--r--  2.0 unx      167 b- defN 24-Apr-02 08:35 pulsar_client-3.5.0.dist-info/NOTICE
+-rw-r--r--  2.0 unx     1016 b- defN 24-Apr-02 08:35 pulsar_client-3.5.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      154 b- defN 24-Apr-02 08:35 pulsar_client-3.5.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 24-Apr-02 08:35 pulsar_client-3.5.0.dist-info/top_level.txt
+-rw-r--r--  2.0 unx    11358 b- defN 24-Apr-02 08:35 pulsar_client-3.5.0.dist-info/LICENSE
+25 files, 16573427 bytes uncompressed, 5186322 bytes compressed:  68.7%
```

## zipnote {}

```diff
@@ -1,55 +1,76 @@
-Filename: _pulsar.cp39-win_amd64.pyd
+Filename: pulsar_client.libs/
 Comment: 
 
-Filename: pulsar/__about__.py
+Filename: pulsar/
 Comment: 
 
-Filename: pulsar/__init__.py
+Filename: pulsar_client-3.5.0.dist-info/
 Comment: 
 
-Filename: pulsar/exceptions.py
+Filename: _pulsar.cpython-312-aarch64-linux-gnu.so
 Comment: 
 
-Filename: pulsar/functions/__init__.py
+Filename: pulsar_client.libs/libpulsar-7cf2e558.so
 Comment: 
 
-Filename: pulsar/functions/context.py
+Filename: pulsar/schema/
 Comment: 
 
-Filename: pulsar/functions/function.py
+Filename: pulsar/functions/
 Comment: 
 
-Filename: pulsar/functions/serde.py
+Filename: pulsar/__init__.py
 Comment: 
 
-Filename: pulsar/schema/__init__.py
+Filename: pulsar/asyncio.py
 Comment: 
 
-Filename: pulsar/schema/definition.py
+Filename: pulsar/__about__.py
+Comment: 
+
+Filename: pulsar/exceptions.py
+Comment: 
+
+Filename: pulsar/schema/__init__.py
 Comment: 
 
 Filename: pulsar/schema/schema.py
 Comment: 
 
 Filename: pulsar/schema/schema_avro.py
 Comment: 
 
-Filename: pulsar_client-3.4.0.dist-info/LICENSE
+Filename: pulsar/schema/definition.py
+Comment: 
+
+Filename: pulsar/functions/__init__.py
+Comment: 
+
+Filename: pulsar/functions/serde.py
+Comment: 
+
+Filename: pulsar/functions/function.py
+Comment: 
+
+Filename: pulsar/functions/context.py
+Comment: 
+
+Filename: pulsar_client-3.5.0.dist-info/RECORD
 Comment: 
 
-Filename: pulsar_client-3.4.0.dist-info/METADATA
+Filename: pulsar_client-3.5.0.dist-info/NOTICE
 Comment: 
 
-Filename: pulsar_client-3.4.0.dist-info/NOTICE
+Filename: pulsar_client-3.5.0.dist-info/METADATA
 Comment: 
 
-Filename: pulsar_client-3.4.0.dist-info/WHEEL
+Filename: pulsar_client-3.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: pulsar_client-3.4.0.dist-info/top_level.txt
+Filename: pulsar_client-3.5.0.dist-info/top_level.txt
 Comment: 
 
-Filename: pulsar_client-3.4.0.dist-info/RECORD
+Filename: pulsar_client-3.5.0.dist-info/LICENSE
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v2.0 to extract, compression method=store
```

## pulsar/__about__.py

```diff
@@ -1,19 +1,19 @@
-#
-# Licensed to the Apache Software Foundation (ASF) under one
-# or more contributor license agreements.  See the NOTICE file
-# distributed with this work for additional information
-# regarding copyright ownership.  The ASF licenses this file
-# to you under the Apache License, Version 2.0 (the
-# "License"); you may not use this file except in compliance
-# with the License.  You may obtain a copy of the License at
-#
-#   http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing,
-# software distributed under the License is distributed on an
-# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
-# KIND, either express or implied.  See the License for the
-# specific language governing permissions and limitations
-# under the License.
-#
-__version__='3.4.0'
+#
+# Licensed to the Apache Software Foundation (ASF) under one
+# or more contributor license agreements.  See the NOTICE file
+# distributed with this work for additional information
+# regarding copyright ownership.  The ASF licenses this file
+# to you under the Apache License, Version 2.0 (the
+# "License"); you may not use this file except in compliance
+# with the License.  You may obtain a copy of the License at
+#
+#   http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing,
+# software distributed under the License is distributed on an
+# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
+# KIND, either express or implied.  See the License for the
+# specific language governing permissions and limitations
+# under the License.
+#
+__version__='3.5.0'
```

## pulsar/__init__.py

```diff
@@ -1,1790 +1,1831 @@
-#
-# Licensed to the Apache Software Foundation (ASF) under one
-# or more contributor license agreements.  See the NOTICE file
-# distributed with this work for additional information
-# regarding copyright ownership.  The ASF licenses this file
-# to you under the Apache License, Version 2.0 (the
-# "License"); you may not use this file except in compliance
-# with the License.  You may obtain a copy of the License at
-#
-#   http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing,
-# software distributed under the License is distributed on an
-# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
-# KIND, either express or implied.  See the License for the
-# specific language governing permissions and limitations
-# under the License.
-#
-
-"""
-The Pulsar Python client library is based on the existing C++ client library.
-All the same features are exposed through the Python interface.
-
-Currently, the supported Python versions are 3.7, 3.8, 3.9 and 3.10.
-
-=================
-Install from PyPI
-=================
-
-Download Python wheel binary files for macOS and Linux directly from
-the PyPI archive:
-
-.. code-block:: shell
-
-    sudo pip install pulsar-client
-
-========================
-Install from source code
-========================
-
-Read the instructions on `source code repository
-<https://github.com/apache/pulsar-client-python#install-the-python-wheel>`_.
-"""
-
-import logging
-from typing import List, Tuple, Optional
-
-import _pulsar
-
-from _pulsar import Result, CompressionType, ConsumerType, InitialPosition, PartitionsRoutingMode, BatchingType, \
-    LoggerLevel, BatchReceivePolicy, KeySharedPolicy, KeySharedMode, ProducerAccessMode, RegexSubscriptionMode, \
-    DeadLetterPolicyBuilder  # noqa: F401
-
-from pulsar.__about__ import __version__
-
-from pulsar.exceptions import *
-
-from pulsar.functions.function import Function
-from pulsar.functions.context import Context
-from pulsar.functions.serde import SerDe, IdentitySerDe, PickleSerDe
-from pulsar import schema
-_schema = schema
-
-import re
-_retype = type(re.compile('x'))
-
-from datetime import timedelta
-
-
-class MessageId:
-    """
-    Represents a message id.
-
-    Attributes
-    ----------
-
-    earliest:
-        Represents the earliest message stored in a topic
-    latest:
-        Represents the latest message published on a topic
-    """
-
-    def __init__(self, partition=-1, ledger_id=-1, entry_id=-1, batch_index=-1):
-        self._msg_id = _pulsar.MessageId(partition, ledger_id, entry_id, batch_index)
-
-    earliest = _pulsar.MessageId.earliest
-    latest = _pulsar.MessageId.latest
-
-    def ledger_id(self):
-        return self._msg_id.ledger_id()
-
-    def entry_id(self):
-        return self._msg_id.entry_id()
-
-    def batch_index(self):
-        return self._msg_id.batch_index()
-
-    def partition(self):
-        return self._msg_id.partition()
-
-    def serialize(self):
-        """
-        Returns a bytes representation of the message id.
-        This byte sequence can be stored and later deserialized.
-        """
-        return self._msg_id.serialize()
-
-    @staticmethod
-    def deserialize(message_id_bytes):
-        """
-        Deserialize a message id object from a previously
-        serialized bytes sequence.
-        """
-        return _pulsar.MessageId.deserialize(message_id_bytes)
-
-
-class Message:
-    """
-    Message objects are returned by a consumer, either by calling `receive` or
-    through a listener.
-    """
-
-    def data(self):
-        """
-        Returns object typed bytes with the payload of the message.
-        """
-        return self._message.data()
-
-    def value(self):
-        """
-        Returns object with the de-serialized version of the message content
-        """
-        return self._schema.decode_message(self._message)
-
-    def properties(self):
-        """
-        Return the properties attached to the message. Properties are
-        application-defined key/value pairs that will be attached to the
-        message.
-        """
-        return self._message.properties()
-
-    def partition_key(self):
-        """
-        Get the partitioning key for the message.
-        """
-        return self._message.partition_key()
-
-    def ordering_key(self):
-        """
-        Get the ordering key for the message.
-        """
-        return self._message.ordering_key()
-
-    def publish_timestamp(self):
-        """
-        Get the timestamp in milliseconds with the message publish time.
-        """
-        return self._message.publish_timestamp()
-
-    def event_timestamp(self):
-        """
-        Get the timestamp in milliseconds with the message event time.
-        """
-        return self._message.event_timestamp()
-
-    def message_id(self):
-        """
-        The message ID that can be used to refer to this particular message.
-        """
-        return self._message.message_id()
-
-    def topic_name(self):
-        """
-        Get the topic Name from which this message originated from
-        """
-        return self._message.topic_name()
-
-    def redelivery_count(self):
-        """
-        Get the redelivery count for this message
-        """
-        return self._message.redelivery_count()
-
-    def schema_version(self):
-        """
-        Get the schema version for this message
-        """
-        return self._message.schema_version()
-
-    @staticmethod
-    def _wrap(_message):
-        self = Message()
-        self._message = _message
-        return self
-
-
-class MessageBatch:
-
-    def __init__(self):
-        self._msg_batch = _pulsar.MessageBatch()
-
-    def with_message_id(self, msg_id):
-        if not isinstance(msg_id, _pulsar.MessageId):
-            if isinstance(msg_id, MessageId):
-                msg_id = msg_id._msg_id
-            else:
-                raise TypeError("unknown message id type")
-        self._msg_batch.with_message_id(msg_id)
-        return self
-
-    def parse_from(self, data, size):
-        self._msg_batch.parse_from(data, size)
-        _msgs = self._msg_batch.messages()
-        return list(map(Message._wrap, _msgs))
-
-
-class Authentication:
-    """
-    Authentication provider object. Used to load authentication from an external
-    shared library.
-    """
-    def __init__(self, dynamicLibPath, authParamsString):
-        """
-        Create the authentication provider instance.
-
-        Parameters
-        ----------
-
-        dynamicLibPath: str
-            Path to the authentication provider shared library (such as ``tls.so``)
-        authParamsString: str
-            Comma-separated list of provider-specific configuration params
-        """
-        _check_type(str, dynamicLibPath, 'dynamicLibPath')
-        _check_type(str, authParamsString, 'authParamsString')
-        self.auth = _pulsar.Authentication.create(dynamicLibPath, authParamsString)
-
-
-class AuthenticationTLS(Authentication):
-    """
-    TLS Authentication implementation
-    """
-    def __init__(self, certificate_path, private_key_path):
-        """
-        Create the TLS authentication provider instance.
-
-        Parameters
-        ----------
-
-        certificate_path: str
-            Path to the public certificate
-        private_key_path: str
-            Path to private TLS key
-        """
-        _check_type(str, certificate_path, 'certificate_path')
-        _check_type(str, private_key_path, 'private_key_path')
-        self.auth = _pulsar.AuthenticationTLS.create(certificate_path, private_key_path)
-
-
-class AuthenticationToken(Authentication):
-    """
-    Token based authentication implementation
-    """
-    def __init__(self, token):
-        """
-        Create the token authentication provider instance.
-
-        Parameters
-        ----------
-
-        token
-            A string containing the token or a functions that provides a string with the token
-        """
-        if not (isinstance(token, str) or callable(token)):
-            raise ValueError("Argument token is expected to be of type 'str' or a function returning 'str'")
-        self.auth = _pulsar.AuthenticationToken.create(token)
-
-
-class AuthenticationAthenz(Authentication):
-    """
-    Athenz Authentication implementation
-    """
-    def __init__(self, auth_params_string):
-        """
-        Create the Athenz authentication provider instance.
-
-        Parameters
-        ----------
-
-        auth_params_string: str
-            JSON encoded configuration for Athenz client
-        """
-        _check_type(str, auth_params_string, 'auth_params_string')
-        self.auth = _pulsar.AuthenticationAthenz.create(auth_params_string)
-
-class AuthenticationOauth2(Authentication):
-    """
-    Oauth2 Authentication implementation
-    """
-    def __init__(self, auth_params_string: str):
-        """
-        Create the Oauth2 authentication provider instance.
-
-        You can create the instance by setting the necessary fields in the JSON string.
-
-        .. code-block:: python
-
-            auth = AuthenticationOauth2('{"issuer_url": "xxx", "private_key": "yyy"}')
-
-        The valid JSON fields are:
-
-        * issuer_url (required)
-            The URL of the authentication provider which allows the Pulsar client to obtain an
-            access token.
-        * private_key (required)
-            The URL to the JSON credentials file. It supports the following pattern formats:
-
-            * ``/path/to/file``
-            * ``file:///path/to/file``
-            * ``file:/path/to/file``
-            * ``data:application/json;base64,<base64-encoded-value>``
-
-            The file content or the based64 encoded value is the encoded JSON string that contains
-            the following fields:
-
-            * ``client_id``
-            * ``client_secret``
-        * audience
-            The OAuth 2.0 "resource server" identifier for a Pulsar cluster.
-        * scope
-            The scope of an access request.
-
-        Parameters
-        ----------
-        auth_params_string : str
-            JSON encoded configuration for Oauth2 client
-
-        """
-        _check_type(str, auth_params_string, 'auth_params_string')
-        self.auth = _pulsar.AuthenticationOauth2.create(auth_params_string)
-
-class AuthenticationBasic(Authentication):
-    """
-    Basic Authentication implementation
-    """
-    def __init__(self, username=None, password=None, method='basic', auth_params_string=None):
-        """
-        Create the Basic authentication provider instance.
-
-        For example, if you want to create a basic authentication instance whose
-        username is "my-user" and password is "my-pass", there are two ways:
-
-        .. code-block:: python
-
-            auth = AuthenticationBasic('my-user', 'my-pass')
-            auth = AuthenticationBasic(auth_params_string='{"username": "my-user", "password": "my-pass"}')
-
-
-        Parameters
-        ----------
-        username : str, optional
-        password : str, optional
-        method : str, default='basic'
-            The authentication method name
-        auth_params_string : str, optional
-            The JSON presentation of all fields above. If it's not None, the other parameters will be ignored.
-            Here is an example JSON presentation:
-
-                {"username": "my-user", "password": "my-pass", "method": "oms3.0"}
-
-            The ``username`` and ``password`` fields are required. If the "method" field is not set, it will be
-            "basic" by default.
-        """
-        if auth_params_string is not None:
-            _check_type(str, auth_params_string, 'auth_params_string')
-            self.auth = _pulsar.AuthenticationBasic.create(auth_params_string)
-        else:
-            _check_type(str, username, 'username')
-            _check_type(str, password, 'password')
-            _check_type(str, method, 'method')
-            self.auth = _pulsar.AuthenticationBasic.create(username, password, method)
-
-class ConsumerDeadLetterPolicy:
-    """
-    Configuration for the "dead letter queue" feature in consumer.
-    """
-    def __init__(self,
-                 max_redeliver_count: int,
-                 dead_letter_topic: str = None,
-                 initial_subscription_name: str = None):
-        """
-        Wrapper DeadLetterPolicy.
-
-        Parameters
-        ----------
-        max_redeliver_count: Maximum number of times that a message is redelivered before being sent to the dead letter queue.
-            - The maxRedeliverCount must be greater than 0.
-        dead_letter_topic: Name of the dead topic where the failing messages are sent.
-            The default value is: sourceTopicName + "-" + subscriptionName + "-DLQ"
-        initial_subscription_name: Name of the initial subscription name of the dead letter topic.
-            If this field is not set, the initial subscription for the dead letter topic is not created.
-            If this field is set but the broker's `allowAutoSubscriptionCreation` is disabled, the DLQ producer
-            fails to be created.
-        """
-        builder = DeadLetterPolicyBuilder()
-        if max_redeliver_count is None or max_redeliver_count < 1:
-            raise ValueError("max_redeliver_count must be greater than 0")
-        builder.maxRedeliverCount(max_redeliver_count)
-        if dead_letter_topic is not None:
-            builder.deadLetterTopic(dead_letter_topic)
-        if initial_subscription_name is not None:
-            builder.initialSubscriptionName(initial_subscription_name)
-        self._policy = builder.build()
-
-    @property
-    def dead_letter_topic(self) -> str:
-        """
-        Return the dead letter topic for dead letter policy.
-        """
-        return self._policy.getDeadLetterTopic()
-
-    @property
-    def max_redeliver_count(self) -> int:
-        """
-        Return the max redeliver count for dead letter policy.
-        """
-        return self._policy.getMaxRedeliverCount()
-
-    @property
-    def initial_subscription_name(self) -> str:
-        """
-        Return the initial subscription name for dead letter policy.
-        """
-        return self._policy.getInitialSubscriptionName()
-
-    def policy(self):
-        """
-        Returns the actual one DeadLetterPolicy.
-        """
-        return self._policy
-
-class CryptoKeyReader:
-    """
-    Default crypto key reader implementation
-    """
-    def __init__(self, public_key_path, private_key_path):
-        """
-        Create crypto key reader.
-
-        Parameters
-        ----------
-
-        public_key_path: str
-            Path to the public key
-        private_key_path: str
-            Path to private key
-        """
-        _check_type(str, public_key_path, 'public_key_path')
-        _check_type(str, private_key_path, 'private_key_path')
-        self.cryptoKeyReader = _pulsar.CryptoKeyReader(public_key_path, private_key_path)
-
-class Client:
-    """
-    The Pulsar client. A single client instance can be used to create producers
-    and consumers on multiple topics.
-
-    The client will share the same connection pool and threads across all
-    producers and consumers.
-    """
-
-    def __init__(self, service_url,
-                 authentication=None,
-                 operation_timeout_seconds=30,
-                 io_threads=1,
-                 message_listener_threads=1,
-                 concurrent_lookup_requests=50000,
-                 log_conf_file_path=None,
-                 use_tls=False,
-                 tls_trust_certs_file_path=None,
-                 tls_allow_insecure_connection=False,
-                 tls_validate_hostname=False,
-                 logger=None,
-                 connection_timeout_ms=10000,
-                 listener_name=None
-                 ):
-        """
-        Create a new Pulsar client instance.
-
-        Parameters
-        ----------
-
-        service_url: str
-            The Pulsar service url eg: pulsar://my-broker.com:6650/
-        authentication: Authentication, optional
-            Set the authentication provider to be used with the broker. Supported methods:
-
-            * `AuthenticationTLS`
-            * `AuthenticationToken`
-            * `AuthenticationAthenz`
-            * `AuthenticationOauth2`
-        operation_timeout_seconds: int, default=30
-            Set timeout on client operations (subscribe, create producer, close, unsubscribe).
-        io_threads: int, default=1
-            Set the number of IO threads to be used by the Pulsar client.
-        message_listener_threads: int, default=1
-            Set the number of threads to be used by the Pulsar client when delivering messages through
-            message listener. The default is 1 thread per Pulsar client. If using more than 1 thread,
-            messages for distinct ``message_listener``s will be delivered in different threads, however a
-            single ``MessageListener`` will always be assigned to the same thread.
-        concurrent_lookup_requests: int, default=50000
-            Number of concurrent lookup-requests allowed on each broker connection to prevent overload
-            on the broker.
-        log_conf_file_path: str, optional
-            This parameter is deprecated and makes no effect. It's retained only for compatibility.
-            Use `logger` to customize a logger.
-        use_tls: bool, default=False
-            Configure whether to use TLS encryption on the connection. This setting is deprecated.
-            TLS will be automatically enabled if the ``serviceUrl`` is set to ``pulsar+ssl://`` or ``https://``
-        tls_trust_certs_file_path: str, optional
-            Set the path to the trusted TLS certificate file. If empty defaults to certifi.
-        tls_allow_insecure_connection: bool, default=False
-            Configure whether the Pulsar client accepts untrusted TLS certificates from the broker.
-        tls_validate_hostname: bool, default=False
-            Configure whether the Pulsar client validates that the hostname of the endpoint,
-            matches the common name on the TLS certificate presented by the endpoint.
-        logger: optional
-            Set a Python logger for this Pulsar client. Should be an instance of `logging.Logger`.
-        connection_timeout_ms: int, default=10000
-            Set timeout in milliseconds on TCP connections.
-        listener_name: str, optional
-            Listener name for lookup. Clients can use listenerName to choose one of the listeners as
-            the service URL to create a connection to the broker as long as the network is accessible.
-            ``advertisedListeners`` must be enabled in broker side.
-        """
-        _check_type(str, service_url, 'service_url')
-        _check_type_or_none(Authentication, authentication, 'authentication')
-        _check_type(int, operation_timeout_seconds, 'operation_timeout_seconds')
-        _check_type(int, connection_timeout_ms, 'connection_timeout_ms')
-        _check_type(int, io_threads, 'io_threads')
-        _check_type(int, message_listener_threads, 'message_listener_threads')
-        _check_type(int, concurrent_lookup_requests, 'concurrent_lookup_requests')
-        _check_type_or_none(str, log_conf_file_path, 'log_conf_file_path')
-        _check_type(bool, use_tls, 'use_tls')
-        _check_type_or_none(str, tls_trust_certs_file_path, 'tls_trust_certs_file_path')
-        _check_type(bool, tls_allow_insecure_connection, 'tls_allow_insecure_connection')
-        _check_type(bool, tls_validate_hostname, 'tls_validate_hostname')
-        _check_type_or_none(str, listener_name, 'listener_name')
-
-        conf = _pulsar.ClientConfiguration()
-        if authentication:
-            conf.authentication(authentication.auth)
-        conf.operation_timeout_seconds(operation_timeout_seconds)
-        conf.connection_timeout(connection_timeout_ms)
-        conf.io_threads(io_threads)
-        conf.message_listener_threads(message_listener_threads)
-        conf.concurrent_lookup_requests(concurrent_lookup_requests)
-
-        if isinstance(logger, logging.Logger):
-            conf.set_logger(self._prepare_logger(logger))
-        elif isinstance(logger, ConsoleLogger):
-            conf.set_console_logger(logger.log_level)
-        elif isinstance(logger, FileLogger):
-            conf.set_file_logger(logger.log_level, logger.log_file)
-        elif logger is not None:
-            raise ValueError("Logger is expected to be either None, logger.Logger, pulsar.ConsoleLogger or pulsar.FileLogger")
-
-        if listener_name:
-            conf.listener_name(listener_name)
-        if use_tls or service_url.startswith('pulsar+ssl://') or service_url.startswith('https://'):
-            conf.use_tls(True)
-        if tls_trust_certs_file_path:
-            conf.tls_trust_certs_file_path(tls_trust_certs_file_path)
-        else:
-            import certifi
-            conf.tls_trust_certs_file_path(certifi.where())
-        conf.tls_allow_insecure_connection(tls_allow_insecure_connection)
-        conf.tls_validate_hostname(tls_validate_hostname)
-        self._client = _pulsar.Client(service_url, conf)
-        self._consumers = []
-
-    @staticmethod
-    def _prepare_logger(logger):
-        import logging
-        def log(level, message):
-            old_threads = logging.logThreads
-            logging.logThreads = False
-            logger.log(logging.getLevelName(level), message)
-            logging.logThreads = old_threads
-        return log
-
-    def create_producer(self, topic,
-                        producer_name=None,
-                        schema=schema.BytesSchema(),
-                        initial_sequence_id=None,
-                        send_timeout_millis=30000,
-                        compression_type: CompressionType = CompressionType.NONE,
-                        max_pending_messages=1000,
-                        max_pending_messages_across_partitions=50000,
-                        block_if_queue_full=False,
-                        batching_enabled=False,
-                        batching_max_messages=1000,
-                        batching_max_allowed_size_in_bytes=128*1024,
-                        batching_max_publish_delay_ms=10,
-                        chunking_enabled=False,
-                        message_routing_mode: PartitionsRoutingMode = PartitionsRoutingMode.RoundRobinDistribution,
-                        lazy_start_partitioned_producers=False,
-                        properties=None,
-                        batching_type: BatchingType = BatchingType.Default,
-                        encryption_key=None,
-                        crypto_key_reader: CryptoKeyReader = None,
-                        access_mode: ProducerAccessMode = ProducerAccessMode.Shared,
-                        ):
-        """
-        Create a new producer on a given topic.
-
-        Parameters
-        ----------
-
-        topic: str
-            The topic name
-        producer_name: str, optional
-            Specify a name for the producer. If not assigned, the system will generate a globally unique name
-            which can be accessed with `Producer.producer_name()`. When specifying a name, it is app to the user
-            to ensure that, for a given topic, the producer name is unique across all Pulsar's clusters.
-        schema: pulsar.schema.Schema, default=pulsar.schema.BytesSchema
-            Define the schema of the data that will be published by this producer, e.g,
-            ``schema=JsonSchema(MyRecordClass)``.
-
-            The schema will be used for two purposes:
-                * Validate the data format against the topic defined schema
-                * Perform serialization/deserialization between data and objects
-        initial_sequence_id: int, optional
-            Set the baseline for the sequence ids for messages published by the producer. First message will be
-            using ``(initialSequenceId + 1)`` as its sequence id and subsequent messages will be assigned
-            incremental sequence ids, if not otherwise specified.
-        send_timeout_millis: int, default=30000
-            If a message is not acknowledged by the server before the ``send_timeout`` expires, an error will be reported.
-        compression_type: CompressionType, default=CompressionType.NONE
-            Set the compression type for the producer. By default, message payloads are not compressed.
-
-            Supported compression types:
-
-            * CompressionType.LZ4
-            * CompressionType.ZLib
-            * CompressionType.ZSTD
-            * CompressionType.SNAPPY
-
-            ZSTD is supported since Pulsar 2.3. Consumers will need to be at least at that release in order to
-            be able to receive messages compressed with ZSTD.
-
-            SNAPPY is supported since Pulsar 2.4. Consumers will need to be at least at that release in order to
-            be able to receive messages compressed with SNAPPY.
-        max_pending_messages: int, default=1000
-            Set the max size of the queue holding the messages pending to receive an acknowledgment from the broker.
-        max_pending_messages_across_partitions: int, default=50000
-            Set the max size of the queue holding the messages pending to receive an acknowledgment across partitions
-            from the broker.
-        block_if_queue_full: bool, default=False
-            Set whether `send_async` operations should block when the outgoing message queue is full.
-        message_routing_mode: PartitionsRoutingMode, default=PartitionsRoutingMode.RoundRobinDistribution
-            Set the message routing mode for the partitioned producer.
-
-            Supported modes:
-
-            * ``PartitionsRoutingMode.RoundRobinDistribution``
-            * ``PartitionsRoutingMode.UseSinglePartition``
-        lazy_start_partitioned_producers: bool, default=False
-            This config affects producers of partitioned topics only. It controls whether producers register
-            and connect immediately to the owner broker of each partition or start lazily on demand. The internal
-            producer of one partition is always started eagerly, chosen by the routing policy, but the internal
-            producers of any additional partitions are started on demand, upon receiving their first message.
-
-            Using this mode can reduce the strain on brokers for topics with large numbers of partitions and when
-            the SinglePartition routing policy is used without keyed messages. Because producer connection can be
-            on demand, this can produce extra send latency for the first messages of a given partition.
-        properties: dict, optional
-            Sets the properties for the producer. The properties associated with a producer can be used for identify
-            a producer at broker side.
-        batching_type: BatchingType, default=BatchingType.Default
-            Sets the batching type for the producer.
-
-            There are two batching type: DefaultBatching and KeyBasedBatching.
-
-            DefaultBatching will batch single messages:
-                (k1, v1), (k2, v1), (k3, v1), (k1, v2), (k2, v2), (k3, v2), (k1, v3), (k2, v3), (k3, v3)
-            ... into single batch message:
-                [(k1, v1), (k2, v1), (k3, v1), (k1, v2), (k2, v2), (k3, v2), (k1, v3), (k2, v3), (k3, v3)]
-
-            KeyBasedBatching will batch incoming single messages:
-                (k1, v1), (k2, v1), (k3, v1), (k1, v2), (k2, v2), (k3, v2), (k1, v3), (k2, v3), (k3, v3)
-            ... into single batch message:
-                [(k1, v1), (k1, v2), (k1, v3)], [(k2, v1), (k2, v2), (k2, v3)], [(k3, v1), (k3, v2), (k3, v3)]
-        chunking_enabled: bool, default=False
-            If message size is higher than allowed max publish-payload size by broker then chunking_enabled helps
-            producer to split message into multiple chunks and publish them to broker separately and in order.
-            So, it allows client to successfully publish large size of messages in pulsar.
-        encryption_key: str, optional
-            The key used for symmetric encryption, configured on the producer side
-        crypto_key_reader: CryptoKeyReader, optional
-            Symmetric encryption class implementation, configuring public key encryption messages for the producer
-            and private key decryption messages for the consumer
-        access_mode: ProducerAccessMode, optional
-            Set the type of access mode that the producer requires on the topic.
-
-            Supported modes:
-
-            * Shared: By default multiple producers can publish on a topic.
-            * Exclusive: Require exclusive access for producer.
-                         Fail immediately if there's already a producer connected.
-            * WaitForExclusive: Producer creation is pending until it can acquire exclusive access.
-            * ExclusiveWithFencing: Acquire exclusive access for the producer.
-                                    Any existing producer will be removed and invalidated immediately.
-        """
-        _check_type(str, topic, 'topic')
-        _check_type_or_none(str, producer_name, 'producer_name')
-        _check_type(_schema.Schema, schema, 'schema')
-        _check_type_or_none(int, initial_sequence_id, 'initial_sequence_id')
-        _check_type(int, send_timeout_millis, 'send_timeout_millis')
-        _check_type(CompressionType, compression_type, 'compression_type')
-        _check_type(int, max_pending_messages, 'max_pending_messages')
-        _check_type(int, max_pending_messages_across_partitions, 'max_pending_messages_across_partitions')
-        _check_type(bool, block_if_queue_full, 'block_if_queue_full')
-        _check_type(bool, batching_enabled, 'batching_enabled')
-        _check_type(int, batching_max_messages, 'batching_max_messages')
-        _check_type(int, batching_max_allowed_size_in_bytes, 'batching_max_allowed_size_in_bytes')
-        _check_type(int, batching_max_publish_delay_ms, 'batching_max_publish_delay_ms')
-        _check_type(bool, chunking_enabled, 'chunking_enabled')
-        _check_type_or_none(dict, properties, 'properties')
-        _check_type(BatchingType, batching_type, 'batching_type')
-        _check_type_or_none(str, encryption_key, 'encryption_key')
-        _check_type_or_none(CryptoKeyReader, crypto_key_reader, 'crypto_key_reader')
-        _check_type(bool, lazy_start_partitioned_producers, 'lazy_start_partitioned_producers')
-        _check_type(ProducerAccessMode, access_mode, 'access_mode')
-
-        conf = _pulsar.ProducerConfiguration()
-        conf.send_timeout_millis(send_timeout_millis)
-        conf.compression_type(compression_type)
-        conf.max_pending_messages(max_pending_messages)
-        conf.max_pending_messages_across_partitions(max_pending_messages_across_partitions)
-        conf.block_if_queue_full(block_if_queue_full)
-        conf.batching_enabled(batching_enabled)
-        conf.batching_max_messages(batching_max_messages)
-        conf.batching_max_allowed_size_in_bytes(batching_max_allowed_size_in_bytes)
-        conf.batching_max_publish_delay_ms(batching_max_publish_delay_ms)
-        conf.partitions_routing_mode(message_routing_mode)
-        conf.batching_type(batching_type)
-        conf.chunking_enabled(chunking_enabled)
-        conf.lazy_start_partitioned_producers(lazy_start_partitioned_producers)
-        conf.access_mode(access_mode)
-        if producer_name:
-            conf.producer_name(producer_name)
-        if initial_sequence_id:
-            conf.initial_sequence_id(initial_sequence_id)
-        if properties:
-            for k, v in properties.items():
-                conf.property(k, v)
-
-        conf.schema(schema.schema_info())
-        if encryption_key:
-            conf.encryption_key(encryption_key)
-        if crypto_key_reader:
-            conf.crypto_key_reader(crypto_key_reader.cryptoKeyReader)
-
-        if batching_enabled and chunking_enabled:
-            raise ValueError("Batching and chunking of messages can't be enabled together.")
-
-        p = Producer()
-        p._producer = self._client.create_producer(topic, conf)
-        p._schema = schema
-        p._client = self._client
-        return p
-
-    def subscribe(self, topic, subscription_name,
-                  consumer_type: ConsumerType = ConsumerType.Exclusive,
-                  schema=schema.BytesSchema(),
-                  message_listener=None,
-                  receiver_queue_size=1000,
-                  max_total_receiver_queue_size_across_partitions=50000,
-                  consumer_name=None,
-                  unacked_messages_timeout_ms=None,
-                  broker_consumer_stats_cache_time_ms=30000,
-                  negative_ack_redelivery_delay_ms=60000,
-                  is_read_compacted=False,
-                  properties=None,
-                  pattern_auto_discovery_period=60,
-                  initial_position: InitialPosition = InitialPosition.Latest,
-                  crypto_key_reader: CryptoKeyReader = None,
-                  replicate_subscription_state_enabled=False,
-                  max_pending_chunked_message=10,
-                  auto_ack_oldest_chunked_message_on_queue_full=False,
-                  start_message_id_inclusive=False,
-                  batch_receive_policy=None,
-                  key_shared_policy=None,
-                  batch_index_ack_enabled=False,
-                  regex_subscription_mode: RegexSubscriptionMode = RegexSubscriptionMode.PersistentOnly,
-                  dead_letter_policy: ConsumerDeadLetterPolicy = None,
-                  ):
-        """
-        Subscribe to the given topic and subscription combination.
-
-        Parameters
-        ----------
-
-        topic:
-            The name of the topic, list of topics or regex pattern. This method will accept these forms:
-            * ``topic='my-topic'``
-            * ``topic=['topic-1', 'topic-2', 'topic-3']``
-            * ``topic=re.compile('persistent://public/default/topic-*')``
-        subscription_name: str
-            The name of the subscription.
-        consumer_type: ConsumerType, default=ConsumerType.Exclusive
-            Select the subscription type to be used when subscribing to the topic.
-        schema: pulsar.schema.Schema, default=pulsar.schema.BytesSchema
-            Define the schema of the data that will be received by this consumer.
-        message_listener: optional
-            Sets a message listener for the consumer. When the listener is set, the application will
-            receive messages through it. Calls to ``consumer.receive()`` will not be allowed.
-            The listener function needs to accept (consumer, message), for example:
-
-            .. code-block:: python
-
-                def my_listener(consumer, message):
-                    # process message
-                    consumer.acknowledge(message)
-        receiver_queue_size: int, default=1000
-            Sets the size of the consumer receive queue. The consumer receive queue controls how many messages can be
-            accumulated by the consumer before the application calls `receive()`. Using a higher value could potentially
-            increase the consumer throughput at the expense of higher memory utilization. Setting the consumer queue
-            size to zero decreases the throughput of the consumer by disabling pre-fetching of messages.
-
-            This approach improves the message distribution on shared subscription by pushing messages only to those
-            consumers that are ready to process them. Neither receive with timeout nor partitioned topics can be used
-            if the consumer queue size is zero. The `receive()` function call should not be interrupted when the
-            consumer queue size is zero. The default value is 1000 messages and should work well for most use cases.
-        max_total_receiver_queue_size_across_partitions: int, default=50000
-            Set the max total receiver queue size across partitions. This setting will be used to reduce the
-            receiver queue size for individual partitions
-        consumer_name: str, optional
-            Sets the consumer name.
-        unacked_messages_timeout_ms: int, optional
-            Sets the timeout in milliseconds for unacknowledged messages. The timeout needs to be greater than
-            10 seconds. An exception is thrown if the given value is less than 10 seconds. If a successful
-            acknowledgement is not sent within the timeout, all the unacknowledged messages are redelivered.
-        negative_ack_redelivery_delay_ms: int, default=60000
-            The delay after which to redeliver the messages that failed to be processed
-            (with the ``consumer.negative_acknowledge()``)
-        broker_consumer_stats_cache_time_ms: int, default=30000
-            Sets the time duration for which the broker-side consumer stats will be cached in the client.
-        is_read_compacted: bool, default=False
-            Selects whether to read the compacted version of the topic
-        properties: dict, optional
-            Sets the properties for the consumer. The properties associated with a consumer can be used for
-            identify a consumer at broker side.
-        pattern_auto_discovery_period: int, default=60
-            Periods of seconds for consumer to auto discover match topics.
-        initial_position: InitialPosition, default=InitialPosition.Latest
-          Set the initial position of a consumer when subscribing to the topic.
-          It could be either: ``InitialPosition.Earliest`` or ``InitialPosition.Latest``.
-        crypto_key_reader: CryptoKeyReader, optional
-            Symmetric encryption class implementation, configuring public key encryption messages for the producer
-            and private key decryption messages for the consumer
-        replicate_subscription_state_enabled: bool, default=False
-            Set whether the subscription status should be replicated.
-        max_pending_chunked_message: int, default=10
-          Consumer buffers chunk messages into memory until it receives all the chunks of the original message.
-          While consuming chunk-messages, chunks from same message might not be contiguous in the stream, and they
-          might be mixed with other messages' chunks. so, consumer has to maintain multiple buffers to manage
-          chunks coming from different messages. This mainly happens when multiple publishers are publishing
-          messages on the topic concurrently or publisher failed to publish all chunks of the messages.
-
-          If it's zero, the pending chunked messages will not be limited.
-        auto_ack_oldest_chunked_message_on_queue_full: bool, default=False
-          Buffering large number of outstanding uncompleted chunked messages can create memory pressure, and it
-          can be guarded by providing the maxPendingChunkedMessage threshold. See setMaxPendingChunkedMessage.
-          Once, consumer reaches this threshold, it drops the outstanding unchunked-messages by silently acking
-          if autoAckOldestChunkedMessageOnQueueFull is true else it marks them for redelivery.
-        start_message_id_inclusive: bool, default=False
-          Set the consumer to include the given position of any reset operation like Consumer::seek.
-        batch_receive_policy: class ConsumerBatchReceivePolicy
-          Set the batch collection policy for batch receiving.
-        key_shared_policy: class ConsumerKeySharedPolicy
-            Set the key shared policy for use when the ConsumerType is KeyShared.
-        batch_index_ack_enabled: Enable the batch index acknowledgement.
-            It should be noted that this option can only work when the broker side also enables the batch index
-            acknowledgement. See the `acknowledgmentAtBatchIndexLevelEnabled` config in `broker.conf`.
-        regex_subscription_mode: RegexSubscriptionMode, optional
-            Set the regex subscription mode for use when the topic is a regex pattern.
-
-            Supported modes:
-
-            * PersistentOnly: By default only subscribe to persistent topics.
-            * NonPersistentOnly: Only subscribe to non-persistent topics.
-            * AllTopics: Subscribe to both persistent and non-persistent topics.
-        dead_letter_policy: class ConsumerDeadLetterPolicy
-          Set dead letter policy for consumer.
-          By default, some messages are redelivered many times, even to the extent that they can never be
-          stopped. By using the dead letter mechanism, messages have the max redelivery count, when they're
-          exceeding the maximum number of redeliveries. Messages are sent to dead letter topics and acknowledged
-          automatically.
-        """
-        _check_type(str, subscription_name, 'subscription_name')
-        _check_type(ConsumerType, consumer_type, 'consumer_type')
-        _check_type(_schema.Schema, schema, 'schema')
-        _check_type(int, receiver_queue_size, 'receiver_queue_size')
-        _check_type(int, max_total_receiver_queue_size_across_partitions,
-                    'max_total_receiver_queue_size_across_partitions')
-        _check_type_or_none(str, consumer_name, 'consumer_name')
-        _check_type_or_none(int, unacked_messages_timeout_ms, 'unacked_messages_timeout_ms')
-        _check_type(int, broker_consumer_stats_cache_time_ms, 'broker_consumer_stats_cache_time_ms')
-        _check_type(int, negative_ack_redelivery_delay_ms, 'negative_ack_redelivery_delay_ms')
-        _check_type(int, pattern_auto_discovery_period, 'pattern_auto_discovery_period')
-        _check_type(bool, is_read_compacted, 'is_read_compacted')
-        _check_type_or_none(dict, properties, 'properties')
-        _check_type(InitialPosition, initial_position, 'initial_position')
-        _check_type_or_none(CryptoKeyReader, crypto_key_reader, 'crypto_key_reader')
-        _check_type(int, max_pending_chunked_message, 'max_pending_chunked_message')
-        _check_type(bool, auto_ack_oldest_chunked_message_on_queue_full, 'auto_ack_oldest_chunked_message_on_queue_full')
-        _check_type(bool, start_message_id_inclusive, 'start_message_id_inclusive')
-        _check_type_or_none(ConsumerBatchReceivePolicy, batch_receive_policy, 'batch_receive_policy')
-        _check_type_or_none(ConsumerKeySharedPolicy, key_shared_policy, 'key_shared_policy')
-        _check_type(bool, batch_index_ack_enabled, 'batch_index_ack_enabled')
-        _check_type(RegexSubscriptionMode, regex_subscription_mode, 'regex_subscription_mode')
-
-        conf = _pulsar.ConsumerConfiguration()
-        conf.consumer_type(consumer_type)
-        conf.regex_subscription_mode(regex_subscription_mode)
-        conf.read_compacted(is_read_compacted)
-        if message_listener:
-            conf.message_listener(_listener_wrapper(message_listener, schema))
-        conf.receiver_queue_size(receiver_queue_size)
-        conf.max_total_receiver_queue_size_across_partitions(max_total_receiver_queue_size_across_partitions)
-        if consumer_name:
-            conf.consumer_name(consumer_name)
-        if unacked_messages_timeout_ms:
-            conf.unacked_messages_timeout_ms(unacked_messages_timeout_ms)
-
-        conf.negative_ack_redelivery_delay_ms(negative_ack_redelivery_delay_ms)
-        conf.broker_consumer_stats_cache_time_ms(broker_consumer_stats_cache_time_ms)
-        if properties:
-            for k, v in properties.items():
-                conf.property(k, v)
-        conf.subscription_initial_position(initial_position)
-
-        conf.schema(schema.schema_info())
-
-        if crypto_key_reader:
-            conf.crypto_key_reader(crypto_key_reader.cryptoKeyReader)
-
-        conf.replicate_subscription_state_enabled(replicate_subscription_state_enabled)
-        conf.max_pending_chunked_message(max_pending_chunked_message)
-        conf.auto_ack_oldest_chunked_message_on_queue_full(auto_ack_oldest_chunked_message_on_queue_full)
-        conf.start_message_id_inclusive(start_message_id_inclusive)
-        if batch_receive_policy:
-            conf.batch_receive_policy(batch_receive_policy.policy())
-
-        if key_shared_policy:
-            conf.key_shared_policy(key_shared_policy.policy())
-        conf.batch_index_ack_enabled(batch_index_ack_enabled)
-        if dead_letter_policy:
-            conf.dead_letter_policy(dead_letter_policy.policy())
-
-        c = Consumer()
-        if isinstance(topic, str):
-            # Single topic
-            c._consumer = self._client.subscribe(topic, subscription_name, conf)
-        elif isinstance(topic, list):
-            # List of topics
-            c._consumer = self._client.subscribe_topics(topic, subscription_name, conf)
-        elif isinstance(topic, _retype):
-            # Regex pattern
-            c._consumer = self._client.subscribe_pattern(topic.pattern, subscription_name, conf)
-        else:
-            raise ValueError("Argument 'topic' is expected to be of a type between (str, list, re.pattern)")
-
-        c._client = self
-        c._schema = schema
-        c._schema.attach_client(self._client)
-        self._consumers.append(c)
-        return c
-
-    def create_reader(self, topic, start_message_id,
-                      schema=schema.BytesSchema(),
-                      reader_listener=None,
-                      receiver_queue_size=1000,
-                      reader_name=None,
-                      subscription_role_prefix=None,
-                      is_read_compacted=False,
-                      crypto_key_reader: CryptoKeyReader = None,
-                      start_message_id_inclusive=False
-                      ):
-        """
-        Create a reader on a particular topic
-
-        Parameters
-        ----------
-
-        topic:
-            The name of the topic.
-        start_message_id:
-            The initial reader positioning is done by specifying a message id. The options are:
-
-            * ``MessageId.earliest``:
-
-            Start reading from the earliest message available in the topic
-
-            * ``MessageId.latest``:
-
-            Start reading from the end topic, only getting messages published after the reader was created
-
-            * ``MessageId``:
-
-            When passing a particular message id, the reader will position itself on that specific position.
-            The first message to be read will be the message next to the specified messageId.
-            Message id can be serialized into a string and deserialized back into a `MessageId` object:
-
-               .. code-block:: python
-
-                   # Serialize to string
-                   s = msg.message_id().serialize()
-
-                   # Deserialize from string
-                   msg_id = MessageId.deserialize(s)
-        schema: pulsar.schema.Schema, default=pulsar.schema.BytesSchema
-            Define the schema of the data that will be received by this reader.
-        reader_listener: optional
-            Sets a message listener for the reader. When the listener is set, the application will receive messages
-            through it. Calls to ``reader.read_next()`` will not be allowed. The listener function needs to accept
-            (reader, message), for example:
-
-            .. code-block:: python
-
-                def my_listener(reader, message):
-                    # process message
-                    pass
-        receiver_queue_size: int, default=1000
-            Sets the size of the reader receive queue. The reader receive queue controls how many messages can be
-            accumulated by the reader before the application calls `read_next()`. Using a higher value could
-            potentially increase the reader throughput at the expense of higher memory utilization.
-        reader_name: str, optional
-            Sets the reader name.
-        subscription_role_prefix: str, optional
-            Sets the subscription role prefix.
-        is_read_compacted: bool, default=False
-            Selects whether to read the compacted version of the topic
-        crypto_key_reader: CryptoKeyReader, optional
-            Symmetric encryption class implementation, configuring public key encryption messages for the producer
-            and private key decryption messages for the consumer
-        start_message_id_inclusive: bool, default=False
-            Set the reader to include the startMessageId or given position of any reset operation like Reader.seek
-        """
-
-        # If a pulsar.MessageId object is passed, access the _pulsar.MessageId object
-        if isinstance(start_message_id, MessageId):
-            start_message_id = start_message_id._msg_id
-
-        _check_type(str, topic, 'topic')
-        _check_type(_pulsar.MessageId, start_message_id, 'start_message_id')
-        _check_type(_schema.Schema, schema, 'schema')
-        _check_type(int, receiver_queue_size, 'receiver_queue_size')
-        _check_type_or_none(str, reader_name, 'reader_name')
-        _check_type_or_none(str, subscription_role_prefix, 'subscription_role_prefix')
-        _check_type(bool, is_read_compacted, 'is_read_compacted')
-        _check_type_or_none(CryptoKeyReader, crypto_key_reader, 'crypto_key_reader')
-        _check_type(bool, start_message_id_inclusive, 'start_message_id_inclusive')
-
-        conf = _pulsar.ReaderConfiguration()
-        if reader_listener:
-            conf.reader_listener(_listener_wrapper(reader_listener, schema))
-        conf.receiver_queue_size(receiver_queue_size)
-        if reader_name:
-            conf.reader_name(reader_name)
-        if subscription_role_prefix:
-            conf.subscription_role_prefix(subscription_role_prefix)
-        conf.schema(schema.schema_info())
-        conf.read_compacted(is_read_compacted)
-        if crypto_key_reader:
-            conf.crypto_key_reader(crypto_key_reader.cryptoKeyReader)
-        conf.start_message_id_inclusive(start_message_id_inclusive)
-
-        c = Reader()
-        c._reader = self._client.create_reader(topic, start_message_id, conf)
-        c._client = self
-        c._schema = schema
-        c._schema.attach_client(self._client)
-        self._consumers.append(c)
-        return c
-
-    def get_topic_partitions(self, topic):
-        """
-        Get the list of partitions for a given topic.
-
-        If the topic is partitioned, this will return a list of partition names. If the topic is not
-        partitioned, the returned list will contain the topic name itself.
-
-        This can be used to discover the partitions and create Reader, Consumer or Producer
-        instances directly on a particular partition.
-
-        Parameters
-        ----------
-
-        topic: str
-            the topic name to lookup
-
-        Returns
-        -------
-        list
-            a list of partition name
-        """
-        _check_type(str, topic, 'topic')
-        return self._client.get_topic_partitions(topic)
-
-    def shutdown(self):
-        """
-        Perform immediate shutdown of Pulsar client.
-
-        Release all resources and close all producer, consumer, and readers without waiting
-        for ongoing operations to complete.
-        """
-        self._client.shutdown()
-
-    def close(self):
-        """
-        Close the client and all the associated producers and consumers
-        """
-        self._client.close()
-
-
-class Producer:
-    """
-    The Pulsar message producer, used to publish messages on a topic.
-
-    Examples
-    --------
-
-    .. code-block:: python
-
-        import pulsar
-
-        client = pulsar.Client('pulsar://localhost:6650')
-        producer = client.create_producer('my-topic')
-        for i in range(10):
-            producer.send(('Hello-%d' % i).encode('utf-8'))
-        client.close()
-    """
-
-    def topic(self):
-        """
-        Return the topic which producer is publishing to
-        """
-        return self._producer.topic()
-
-    def producer_name(self):
-        """
-        Return the producer name which could have been assigned by the
-        system or specified by the client
-        """
-        return self._producer.producer_name()
-
-    def last_sequence_id(self):
-        """
-        Get the last sequence id that was published by this producer.
-
-        This represents either the automatically assigned or custom sequence id
-        (set on the ``MessageBuilder``) that was published and acknowledged by the broker.
-
-        After recreating a producer with the same producer name, this will return the
-        last message that was published in the previous producer session, or -1 if
-        there was no message ever published.
-        """
-        return self._producer.last_sequence_id()
-
-    def send(self, content,
-             properties=None,
-             partition_key=None,
-             ordering_key=None,
-             sequence_id=None,
-             replication_clusters=None,
-             disable_replication=False,
-             event_timestamp=None,
-             deliver_at=None,
-             deliver_after=None,
-             ):
-        """
-        Publish a message on the topic. Blocks until the message is acknowledged
-
-        Returns a `MessageId` object that represents where the message is persisted.
-
-        Parameters
-        ----------
-
-        content:
-            A ``bytes`` object with the message payload.
-        properties: optional
-            A dict of application-defined string properties.
-        partition_key: optional
-            Sets the partition key for message routing. A hash of this key is used
-            to determine the message's topic partition.
-        ordering_key: optional
-            Sets the ordering key for message routing.
-        sequence_id:  optional
-            Specify a custom sequence id for the message being published.
-        replication_clusters:  optional
-          Override namespace replication clusters. Note that it is the caller's responsibility to provide valid
-          cluster names and that all clusters have been previously configured as topics. Given an empty list,
-          the message will replicate according to the namespace configuration.
-        disable_replication: bool, default=False
-            Do not replicate this message.
-        event_timestamp: optional
-            Timestamp in millis of the timestamp of event creation
-        deliver_at: optional
-            Specify the message should not be delivered earlier than the specified timestamp.
-            The timestamp is milliseconds and based on UTC
-        deliver_after: optional
-            Specify a delay in timedelta for the delivery of the messages.
-        """
-        msg = self._build_msg(content, properties, partition_key, ordering_key, sequence_id,
-                              replication_clusters, disable_replication, event_timestamp,
-                              deliver_at, deliver_after)
-        return self._producer.send(msg)
-
-    def send_async(self, content, callback,
-                   properties=None,
-                   partition_key=None,
-                   ordering_key=None,
-                   sequence_id=None,
-                   replication_clusters=None,
-                   disable_replication=False,
-                   event_timestamp=None,
-                   deliver_at=None,
-                   deliver_after=None,
-                   ):
-        """
-        Send a message asynchronously.
-
-        Examples
-        --------
-
-        The ``callback`` will be invoked once the message has been acknowledged by the broker.
-
-        .. code-block:: python
-
-            import pulsar
-
-            client = pulsar.Client('pulsar://localhost:6650')
-            producer = client.create_producer(
-                            'my-topic',
-                            block_if_queue_full=True,
-                            batching_enabled=True,
-                            batching_max_publish_delay_ms=10)
-
-            def callback(res, msg_id):
-                print('Message published res=%s', res)
-
-            while True:
-                producer.send_async(('Hello-%d' % i).encode('utf-8'), callback)
-
-            client.close()
-
-
-        When the producer queue is full, by default the message will be rejected
-        and the callback invoked with an error code.
-
-
-        Parameters
-        ----------
-
-        content
-            A `bytes` object with the message payload.
-        callback
-            A callback that is invoked once the message has been acknowledged by the broker.
-        properties: optional
-            A dict of application0-defined string properties.
-        partition_key: optional
-            Sets the partition key for the message routing. A hash of this key is
-            used to determine the message's topic partition.
-        ordering_key: optional
-            Sets the ordering key for the message routing.
-        sequence_id: optional
-            Specify a custom sequence id for the message being published.
-        replication_clusters: optional
-            Override namespace replication clusters. Note that it is the caller's responsibility
-            to provide valid cluster names and that all clusters have been previously configured
-            as topics. Given an empty list, the message will replicate per the namespace configuration.
-        disable_replication: optional
-            Do not replicate this message.
-        event_timestamp: optional
-            Timestamp in millis of the timestamp of event creation
-        deliver_at: optional
-            Specify the message should not be delivered earlier than the specified timestamp.
-        deliver_after: optional
-            Specify a delay in timedelta for the delivery of the messages.
-        """
-        msg = self._build_msg(content, properties, partition_key, ordering_key, sequence_id,
-                              replication_clusters, disable_replication, event_timestamp,
-                              deliver_at, deliver_after)
-        self._producer.send_async(msg, callback)
-
-
-    def flush(self):
-        """
-        Flush all the messages buffered in the client and wait until all messages have been
-        successfully persisted
-        """
-        self._producer.flush()
-
-
-    def close(self):
-        """
-        Close the producer.
-        """
-        self._producer.close()
-
-    def _build_msg(self, content, properties, partition_key, ordering_key, sequence_id,
-                   replication_clusters, disable_replication, event_timestamp,
-                   deliver_at, deliver_after):
-        data = self._schema.encode(content)
-
-        _check_type(bytes, data, 'data')
-        _check_type_or_none(dict, properties, 'properties')
-        _check_type_or_none(str, partition_key, 'partition_key')
-        _check_type_or_none(str, ordering_key, 'ordering_key')
-        _check_type_or_none(int, sequence_id, 'sequence_id')
-        _check_type_or_none(list, replication_clusters, 'replication_clusters')
-        _check_type(bool, disable_replication, 'disable_replication')
-        _check_type_or_none(int, event_timestamp, 'event_timestamp')
-        _check_type_or_none(int, deliver_at, 'deliver_at')
-        _check_type_or_none(timedelta, deliver_after, 'deliver_after')
-
-        mb = _pulsar.MessageBuilder()
-        mb.content(data)
-        if properties:
-            for k, v in properties.items():
-                mb.property(k, v)
-        if partition_key:
-            mb.partition_key(partition_key)
-        if ordering_key:
-            mb.ordering_key(ordering_key)
-        if sequence_id:
-            mb.sequence_id(sequence_id)
-        if replication_clusters:
-            mb.replication_clusters(replication_clusters)
-        if disable_replication:
-            mb.disable_replication(disable_replication)
-        if event_timestamp:
-            mb.event_timestamp(event_timestamp)
-        if deliver_at:
-            mb.deliver_at(deliver_at)
-        if deliver_after:
-            mb.deliver_after(deliver_after)
-
-        return mb.build()
-
-    def is_connected(self):
-        """
-        Check if the producer is connected or not.
-        """
-        return self._producer.is_connected()
-
-
-class Consumer:
-    """
-    Pulsar consumer.
-
-    Examples
-    --------
-
-    .. code-block:: python
-
-        import pulsar
-
-        client = pulsar.Client('pulsar://localhost:6650')
-        consumer = client.subscribe('my-topic', 'my-subscription')
-        while True:
-            msg = consumer.receive()
-            try:
-                print("Received message '{}' id='{}'".format(msg.data(), msg.message_id()))
-                consumer.acknowledge(msg)
-            except Exception:
-                consumer.negative_acknowledge(msg)
-        client.close()
-    """
-
-    def topic(self):
-        """
-        Return the topic this consumer is subscribed to.
-        """
-        return self._consumer.topic()
-
-    def subscription_name(self):
-        """
-        Return the subscription name.
-        """
-        return self._consumer.subscription_name()
-
-    def unsubscribe(self):
-        """
-        Unsubscribe the current consumer from the topic.
-
-        This method will block until the operation is completed. Once the
-        consumer is unsubscribed, no more messages will be received and
-        subsequent new messages will not be retained for this consumer.
-
-        This consumer object cannot be reused.
-        """
-        return self._consumer.unsubscribe()
-
-    def receive(self, timeout_millis=None):
-        """
-        Receive a single message.
-
-        If a message is not immediately available, this method will block until
-        a new message is available.
-
-        Parameters
-        ----------
-
-        timeout_millis: int, optional
-            If specified, the receiver will raise an exception if a message is not available within the timeout.
-        """
-        if timeout_millis is None:
-            msg = self._consumer.receive()
-        else:
-            _check_type(int, timeout_millis, 'timeout_millis')
-            msg = self._consumer.receive(timeout_millis)
-
-        m = Message()
-        m._message = msg
-        m._schema = self._schema
-        return m
-
-    def batch_receive(self):
-        """
-        Batch receiving messages.
-
-        This calls blocks until has enough messages or wait timeout, more details to see {@link BatchReceivePolicy}.
-        """
-        messages = []
-        msgs = self._consumer.batch_receive()
-        for msg in msgs:
-            m = Message()
-            m._message = msg
-            messages.append(m)
-        return messages
-
-    def acknowledge(self, message):
-        """
-        Acknowledge the reception of a single message.
-
-        This method will block until an acknowledgement is sent to the broker.
-        After that, the message will not be re-delivered to this consumer.
-
-        Parameters
-        ----------
-        message : Message, _pulsar.Message, _pulsar.MessageId
-            The received message or message id.
-
-        Raises
-        ------
-        OperationNotSupported
-             if ``message`` is not allowed to acknowledge
-        """
-        if isinstance(message, Message):
-            self._consumer.acknowledge(message._message)
-        else:
-            self._consumer.acknowledge(message)
-
-    def acknowledge_cumulative(self, message):
-        """
-        Acknowledge the reception of all the messages in the stream up to (and
-        including) the provided message.
-
-        This method will block until an acknowledgement is sent to the broker.
-        After that, the messages will not be re-delivered to this consumer.
-
-        Parameters
-        ----------
-
-        message:
-            The received message or message id.
-
-        Raises
-        ------
-        CumulativeAcknowledgementNotAllowedError
-            if the consumer type is ConsumerType.KeyShared or ConsumerType.Shared
-        """
-        if isinstance(message, Message):
-            self._consumer.acknowledge_cumulative(message._message)
-        else:
-            self._consumer.acknowledge_cumulative(message)
-
-    def negative_acknowledge(self, message):
-        """
-        Acknowledge the failure to process a single message.
-
-        When a message is "negatively acked" it will be marked for redelivery after
-        some fixed delay. The delay is configurable when constructing the consumer
-        with {@link ConsumerConfiguration#setNegativeAckRedeliveryDelayMs}.
-
-        This call is not blocking.
-
-        Parameters
-        ----------
-
-        message:
-            The received message or message id.
-        """
-        if isinstance(message, Message):
-            self._consumer.negative_acknowledge(message._message)
-        else:
-            self._consumer.negative_acknowledge(message)
-
-    def pause_message_listener(self):
-        """
-        Pause receiving messages via the ``message_listener`` until `resume_message_listener()` is called.
-        """
-        self._consumer.pause_message_listener()
-
-    def resume_message_listener(self):
-        """
-        Resume receiving the messages via the message listener.
-        Asynchronously receive all the messages enqueued from the time
-        `pause_message_listener()` was called.
-        """
-        self._consumer.resume_message_listener()
-
-    def redeliver_unacknowledged_messages(self):
-        """
-        Redelivers all the unacknowledged messages. In failover mode, the
-        request is ignored if the consumer is not active for the given topic. In
-        shared mode, the consumer's messages to be redelivered are distributed
-        across all the connected consumers. This is a non-blocking call and
-        doesn't throw an exception. In case the connection breaks, the messages
-        are redelivered after reconnect.
-        """
-        self._consumer.redeliver_unacknowledged_messages()
-
-    def seek(self, messageid):
-        """
-        Reset the subscription associated with this consumer to a specific message id or publish timestamp.
-        The message id can either be a specific message or represent the first or last messages in the topic.
-        Note: this operation can only be done on non-partitioned topics. For these, one can rather perform the
-        seek() on the individual partitions.
-
-        Parameters
-        ----------
-
-        messageid:
-            The message id for seek, OR an integer event time to seek to
-        """
-        self._consumer.seek(messageid)
-
-    def close(self):
-        """
-        Close the consumer.
-        """
-        self._consumer.close()
-        self._client._consumers.remove(self)
-
-    def is_connected(self):
-        """
-        Check if the consumer is connected or not.
-        """
-        return self._consumer.is_connected()
-
-    def get_last_message_id(self):
-        """
-        Get the last message id.
-        """
-        return self._consumer.get_last_message_id()
-
-class ConsumerBatchReceivePolicy:
-    """
-    Batch receive policy can limit the number and bytes of messages in a single batch,
-    and can specify a timeout for waiting for enough messages for this batch.
-
-    A batch receive action is completed as long as any one of the conditions (the batch has enough number
-    or size of messages, or the waiting timeout is passed) are met.
-    """
-    def __init__(self, max_num_message, max_num_bytes, timeout_ms):
-        """
-        Wrapper BatchReceivePolicy.
-
-        Parameters
-        ----------
-
-        max_num_message: Max num message, if less than 0, it means no limit. default: -1
-        max_num_bytes: Max num bytes, if less than 0, it means no limit. default: 10 * 1024 * 1024
-        timeout_ms: If less than 0, it means no limit. default: 100
-        """
-        self._policy = BatchReceivePolicy(max_num_message, max_num_bytes, timeout_ms)
-
-    def policy(self):
-        """
-        Returns the actual one BatchReceivePolicy.
-        """
-        return self._policy
-
-class ConsumerKeySharedPolicy:
-    """
-    Consumer key shared policy is used to configure the consumer behaviour when the ConsumerType is KeyShared.
-    """
-    def __init__(
-            self,
-            key_shared_mode: KeySharedMode = KeySharedMode.AutoSplit,
-            allow_out_of_order_delivery: bool = False,
-            sticky_ranges: Optional[List[Tuple[int, int]]] = None,
-    ):
-        """
-        Wrapper KeySharedPolicy.
-
-        Parameters
-        ----------
-
-        key_shared_mode: KeySharedMode, optional
-            Set the key shared mode. eg: KeySharedMode.Sticky or KeysharedMode.AutoSplit
-
-        allow_out_of_order_delivery: bool, optional
-            Set whether to allow for out of order delivery
-            If it is enabled, it relaxes the ordering requirement and allows the broker to send out-of-order
-            messages in case of failures. This makes it faster for new consumers to join without being stalled by
-            an existing slow consumer.
-
-            If this is True, a single consumer still receives all keys, but they may come in different orders.
-
-        sticky_ranges: List[Tuple[int, int]], optional
-            Set the ranges used with sticky mode. The integers can be from 0 to 2^16 (0 <= val < 65,536)
-        """
-        if key_shared_mode == KeySharedMode.Sticky and sticky_ranges is None:
-            raise ValueError("When using key_shared_mode = KeySharedMode.Sticky you must also provide sticky_ranges")
-
-        self._policy = KeySharedPolicy()
-        self._policy.set_key_shared_mode(key_shared_mode)
-        self._policy.set_allow_out_of_order_delivery(allow_out_of_order_delivery)
-
-        if sticky_ranges is not None:
-            self._policy.set_sticky_ranges(sticky_ranges)
-
-    @property
-    def key_shared_mode(self) -> KeySharedMode:
-        """
-        Returns the key shared mode
-        """
-        return self._policy.get_key_shared_mode()
-
-    @property
-    def allow_out_of_order_delivery(self) -> bool:
-        """
-        Returns whether out of order delivery is enabled
-        """
-        return self._policy.is_allow_out_of_order_delivery()
-
-    @property
-    def sticky_ranges(self) -> List[Tuple[int, int]]:
-        """
-        Returns the actual sticky ranges
-        """
-        return self._policy.get_sticky_ranges()
-
-    def policy(self):
-        """
-        Returns the actual KeySharedPolicy.
-        """
-        return self._policy
-
-class Reader:
-    """
-    Pulsar topic reader.
-    """
-
-    def topic(self):
-        """
-        Return the topic this reader is reading from.
-        """
-        return self._reader.topic()
-
-    def read_next(self, timeout_millis=None):
-        """
-        Read a single message.
-
-        If a message is not immediately available, this method will block until
-        a new message is available.
-
-        Parameters
-        ----------
-
-        timeout_millis: int, optional
-            If specified, the receiver will raise an exception if a message is not available within the timeout.
-        """
-        if timeout_millis is None:
-            msg = self._reader.read_next()
-        else:
-            _check_type(int, timeout_millis, 'timeout_millis')
-            msg = self._reader.read_next(timeout_millis)
-
-        m = Message()
-        m._message = msg
-        m._schema = self._schema
-        return m
-
-    def has_message_available(self):
-        """
-        Check if there is any message available to read from the current position.
-        """
-        return self._reader.has_message_available();
-
-    def seek(self, messageid):
-        """
-        Reset this reader to a specific message id or publish timestamp.
-        The message id can either be a specific message or represent the first or last messages in the topic.
-        Note: this operation can only be done on non-partitioned topics. For these, one can rather perform the
-        seek() on the individual partitions.
-
-        Parameters
-        ----------
-
-        messageid:
-            The message id for seek, OR an integer event time to seek to
-        """
-        self._reader.seek(messageid)
-
-    def close(self):
-        """
-        Close the reader.
-        """
-        self._reader.close()
-        self._client._consumers.remove(self)
-
-    def is_connected(self):
-        """
-        Check if the reader is connected or not.
-        """
-        return self._reader.is_connected()
-
-
-class ConsoleLogger:
-    """
-    Logger that writes on standard output
-
-    Attributes
-    ----------
-
-    log_level:
-        The logging level, eg: ``pulsar.LoggerLevel.Info``
-    """
-    def __init__(self, log_level=_pulsar.LoggerLevel.Info):
-        _check_type(_pulsar.LoggerLevel, log_level, 'log_level')
-        self.log_level = log_level
-
-
-class FileLogger:
-    """
-    Logger that writes into a file
-
-    Attributes
-    ----------
-
-    log_level:
-        The logging level, eg: ``pulsar.LoggerLevel.Info``
-    log_file:
-        The file where to write the logs
-    """
-    def __init__(self, log_level, log_file):
-        _check_type(_pulsar.LoggerLevel, log_level, 'log_level')
-        _check_type(str, log_file, 'log_file')
-        self.log_level = log_level
-        self.log_file = log_file
-
-
-def _check_type(var_type, var, name):
-    if not isinstance(var, var_type):
-        raise ValueError("Argument %s is expected to be of type '%s' and not '%s'"
-                         % (name, var_type.__name__, type(var).__name__))
-
-
-def _check_type_or_none(var_type, var, name):
-    if var is not None and not isinstance(var, var_type):
-        raise ValueError("Argument %s is expected to be either None or of type '%s'"
-                         % (name, var_type.__name__))
-
-
-def _listener_wrapper(listener, schema):
-    def wrapper(consumer, msg):
-        c = Consumer()
-        c._consumer = consumer
-        m = Message()
-        m._message = msg
-        m._schema = schema
-        listener(c, m)
-    return wrapper
+#
+# Licensed to the Apache Software Foundation (ASF) under one
+# or more contributor license agreements.  See the NOTICE file
+# distributed with this work for additional information
+# regarding copyright ownership.  The ASF licenses this file
+# to you under the Apache License, Version 2.0 (the
+# "License"); you may not use this file except in compliance
+# with the License.  You may obtain a copy of the License at
+#
+#   http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing,
+# software distributed under the License is distributed on an
+# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
+# KIND, either express or implied.  See the License for the
+# specific language governing permissions and limitations
+# under the License.
+#
+
+"""
+The Pulsar Python client library is based on the existing C++ client library.
+All the same features are exposed through the Python interface.
+
+Currently, the supported Python versions are 3.7, 3.8, 3.9 and 3.10.
+
+=================
+Install from PyPI
+=================
+
+Download Python wheel binary files for macOS and Linux directly from
+the PyPI archive:
+
+.. code-block:: shell
+
+    sudo pip install pulsar-client
+
+========================
+Install from source code
+========================
+
+Read the instructions on `source code repository
+<https://github.com/apache/pulsar-client-python#install-the-python-wheel>`_.
+"""
+
+import logging
+from typing import List, Tuple, Optional, Union
+
+import _pulsar
+
+from _pulsar import Result, CompressionType, ConsumerType, InitialPosition, PartitionsRoutingMode, BatchingType, \
+    LoggerLevel, BatchReceivePolicy, KeySharedPolicy, KeySharedMode, ProducerAccessMode, RegexSubscriptionMode, \
+    DeadLetterPolicyBuilder  # noqa: F401
+
+from pulsar.__about__ import __version__
+
+from pulsar.exceptions import *
+
+from pulsar.functions.function import Function
+from pulsar.functions.context import Context
+from pulsar.functions.serde import SerDe, IdentitySerDe, PickleSerDe
+from pulsar import schema
+_schema = schema
+
+import re
+_retype = type(re.compile('x'))
+
+from datetime import timedelta
+
+
+class MessageId:
+    """
+    Represents a message id.
+
+    Attributes
+    ----------
+
+    earliest:
+        Represents the earliest message stored in a topic
+    latest:
+        Represents the latest message published on a topic
+    """
+
+    def __init__(self, partition=-1, ledger_id=-1, entry_id=-1, batch_index=-1):
+        self._msg_id = _pulsar.MessageId(partition, ledger_id, entry_id, batch_index)
+
+    earliest = _pulsar.MessageId.earliest
+    latest = _pulsar.MessageId.latest
+
+    def ledger_id(self):
+        return self._msg_id.ledger_id()
+
+    def entry_id(self):
+        return self._msg_id.entry_id()
+
+    def batch_index(self):
+        return self._msg_id.batch_index()
+
+    def partition(self):
+        return self._msg_id.partition()
+
+    def serialize(self):
+        """
+        Returns a bytes representation of the message id.
+        This byte sequence can be stored and later deserialized.
+        """
+        return self._msg_id.serialize()
+
+    def __str__(self) -> str:
+        """
+        Returns the string representation of the message id.
+        """
+        return str(self._msg_id)
+
+    @staticmethod
+    def deserialize(message_id_bytes):
+        """
+        Deserialize a message id object from a previously
+        serialized bytes sequence.
+        """
+        return _pulsar.MessageId.deserialize(message_id_bytes)
+
+
+class Message:
+    """
+    Message objects are returned by a consumer, either by calling `receive` or
+    through a listener.
+    """
+
+    def data(self):
+        """
+        Returns object typed bytes with the payload of the message.
+        """
+        return self._message.data()
+
+    def value(self):
+        """
+        Returns object with the de-serialized version of the message content
+        """
+        return self._schema.decode_message(self._message)
+
+    def properties(self):
+        """
+        Return the properties attached to the message. Properties are
+        application-defined key/value pairs that will be attached to the
+        message.
+        """
+        return self._message.properties()
+
+    def partition_key(self):
+        """
+        Get the partitioning key for the message.
+        """
+        return self._message.partition_key()
+
+    def ordering_key(self):
+        """
+        Get the ordering key for the message.
+        """
+        return self._message.ordering_key()
+
+    def publish_timestamp(self):
+        """
+        Get the timestamp in milliseconds with the message publish time.
+        """
+        return self._message.publish_timestamp()
+
+    def event_timestamp(self):
+        """
+        Get the timestamp in milliseconds with the message event time.
+        """
+        return self._message.event_timestamp()
+
+    def message_id(self):
+        """
+        The message ID that can be used to refer to this particular message.
+        """
+        return self._message.message_id()
+
+    def topic_name(self):
+        """
+        Get the topic Name from which this message originated from
+        """
+        return self._message.topic_name()
+
+    def redelivery_count(self):
+        """
+        Get the redelivery count for this message
+        """
+        return self._message.redelivery_count()
+
+    def schema_version(self):
+        """
+        Get the schema version for this message
+        """
+        return self._message.schema_version()
+
+    @staticmethod
+    def _wrap(_message):
+        self = Message()
+        self._message = _message
+        return self
+
+
+class MessageBatch:
+
+    def __init__(self):
+        self._msg_batch = _pulsar.MessageBatch()
+
+    def with_message_id(self, msg_id):
+        if not isinstance(msg_id, _pulsar.MessageId):
+            if isinstance(msg_id, MessageId):
+                msg_id = msg_id._msg_id
+            else:
+                raise TypeError("unknown message id type")
+        self._msg_batch.with_message_id(msg_id)
+        return self
+
+    def parse_from(self, data, size):
+        self._msg_batch.parse_from(data, size)
+        _msgs = self._msg_batch.messages()
+        return list(map(Message._wrap, _msgs))
+
+
+class Authentication:
+    """
+    Authentication provider object. Used to load authentication from an external
+    shared library.
+    """
+    def __init__(self, dynamicLibPath, authParamsString):
+        """
+        Create the authentication provider instance.
+
+        Parameters
+        ----------
+
+        dynamicLibPath: str
+            Path to the authentication provider shared library (such as ``tls.so``)
+        authParamsString: str
+            Comma-separated list of provider-specific configuration params
+        """
+        _check_type(str, dynamicLibPath, 'dynamicLibPath')
+        _check_type(str, authParamsString, 'authParamsString')
+        self.auth = _pulsar.Authentication.create(dynamicLibPath, authParamsString)
+
+
+class AuthenticationTLS(Authentication):
+    """
+    TLS Authentication implementation
+    """
+    def __init__(self, certificate_path, private_key_path):
+        """
+        Create the TLS authentication provider instance.
+
+        Parameters
+        ----------
+
+        certificate_path: str
+            Path to the public certificate
+        private_key_path: str
+            Path to private TLS key
+        """
+        _check_type(str, certificate_path, 'certificate_path')
+        _check_type(str, private_key_path, 'private_key_path')
+        self.auth = _pulsar.AuthenticationTLS.create(certificate_path, private_key_path)
+
+
+class AuthenticationToken(Authentication):
+    """
+    Token based authentication implementation
+    """
+    def __init__(self, token):
+        """
+        Create the token authentication provider instance.
+
+        Parameters
+        ----------
+
+        token
+            A string containing the token or a functions that provides a string with the token
+        """
+        if not (isinstance(token, str) or callable(token)):
+            raise ValueError("Argument token is expected to be of type 'str' or a function returning 'str'")
+        self.auth = _pulsar.AuthenticationToken.create(token)
+
+
+class AuthenticationAthenz(Authentication):
+    """
+    Athenz Authentication implementation
+    """
+    def __init__(self, auth_params_string):
+        """
+        Create the Athenz authentication provider instance.
+
+        Parameters
+        ----------
+
+        auth_params_string: str
+            JSON encoded configuration for Athenz client
+        """
+        _check_type(str, auth_params_string, 'auth_params_string')
+        self.auth = _pulsar.AuthenticationAthenz.create(auth_params_string)
+
+class AuthenticationOauth2(Authentication):
+    """
+    Oauth2 Authentication implementation
+    """
+    def __init__(self, auth_params_string: str):
+        """
+        Create the Oauth2 authentication provider instance.
+
+        You can create the instance by setting the necessary fields in the JSON string.
+
+        .. code-block:: python
+
+            auth = AuthenticationOauth2('{"issuer_url": "xxx", "private_key": "yyy"}')
+
+        The valid JSON fields are:
+
+        * issuer_url (required)
+            The URL of the authentication provider which allows the Pulsar client to obtain an
+            access token.
+        * private_key (required)
+            The URL to the JSON credentials file. It supports the following pattern formats:
+
+            * ``/path/to/file``
+            * ``file:///path/to/file``
+            * ``file:/path/to/file``
+            * ``data:application/json;base64,<base64-encoded-value>``
+
+            The file content or the based64 encoded value is the encoded JSON string that contains
+            the following fields:
+
+            * ``client_id``
+            * ``client_secret``
+        * audience
+            The OAuth 2.0 "resource server" identifier for a Pulsar cluster.
+        * scope
+            The scope of an access request.
+
+        Parameters
+        ----------
+        auth_params_string : str
+            JSON encoded configuration for Oauth2 client
+
+        """
+        _check_type(str, auth_params_string, 'auth_params_string')
+        self.auth = _pulsar.AuthenticationOauth2.create(auth_params_string)
+
+class AuthenticationBasic(Authentication):
+    """
+    Basic Authentication implementation
+    """
+    def __init__(self, username=None, password=None, method='basic', auth_params_string=None):
+        """
+        Create the Basic authentication provider instance.
+
+        For example, if you want to create a basic authentication instance whose
+        username is "my-user" and password is "my-pass", there are two ways:
+
+        .. code-block:: python
+
+            auth = AuthenticationBasic('my-user', 'my-pass')
+            auth = AuthenticationBasic(auth_params_string='{"username": "my-user", "password": "my-pass"}')
+
+
+        Parameters
+        ----------
+        username : str, optional
+        password : str, optional
+        method : str, default='basic'
+            The authentication method name
+        auth_params_string : str, optional
+            The JSON presentation of all fields above. If it's not None, the other parameters will be ignored.
+            Here is an example JSON presentation:
+
+                {"username": "my-user", "password": "my-pass", "method": "oms3.0"}
+
+            The ``username`` and ``password`` fields are required. If the "method" field is not set, it will be
+            "basic" by default.
+        """
+        if auth_params_string is not None:
+            _check_type(str, auth_params_string, 'auth_params_string')
+            self.auth = _pulsar.AuthenticationBasic.create(auth_params_string)
+        else:
+            _check_type(str, username, 'username')
+            _check_type(str, password, 'password')
+            _check_type(str, method, 'method')
+            self.auth = _pulsar.AuthenticationBasic.create(username, password, method)
+
+class ConsumerDeadLetterPolicy:
+    """
+    Configuration for the "dead letter queue" feature in consumer.
+    """
+    def __init__(self,
+                 max_redeliver_count: int,
+                 dead_letter_topic: str = None,
+                 initial_subscription_name: str = None):
+        """
+        Wrapper DeadLetterPolicy.
+
+        Parameters
+        ----------
+        max_redeliver_count: Maximum number of times that a message is redelivered before being sent to the dead letter queue.
+            - The maxRedeliverCount must be greater than 0.
+        dead_letter_topic: Name of the dead topic where the failing messages are sent.
+            The default value is: sourceTopicName + "-" + subscriptionName + "-DLQ"
+        initial_subscription_name: Name of the initial subscription name of the dead letter topic.
+            If this field is not set, the initial subscription for the dead letter topic is not created.
+            If this field is set but the broker's `allowAutoSubscriptionCreation` is disabled, the DLQ producer
+            fails to be created.
+        """
+        builder = DeadLetterPolicyBuilder()
+        if max_redeliver_count is None or max_redeliver_count < 1:
+            raise ValueError("max_redeliver_count must be greater than 0")
+        builder.maxRedeliverCount(max_redeliver_count)
+        if dead_letter_topic is not None:
+            builder.deadLetterTopic(dead_letter_topic)
+        if initial_subscription_name is not None:
+            builder.initialSubscriptionName(initial_subscription_name)
+        self._policy = builder.build()
+
+    @property
+    def dead_letter_topic(self) -> str:
+        """
+        Return the dead letter topic for dead letter policy.
+        """
+        return self._policy.getDeadLetterTopic()
+
+    @property
+    def max_redeliver_count(self) -> int:
+        """
+        Return the max redeliver count for dead letter policy.
+        """
+        return self._policy.getMaxRedeliverCount()
+
+    @property
+    def initial_subscription_name(self) -> str:
+        """
+        Return the initial subscription name for dead letter policy.
+        """
+        return self._policy.getInitialSubscriptionName()
+
+    def policy(self):
+        """
+        Returns the actual one DeadLetterPolicy.
+        """
+        return self._policy
+
+class CryptoKeyReader:
+    """
+    Default crypto key reader implementation
+    """
+    def __init__(self, public_key_path, private_key_path):
+        """
+        Create crypto key reader.
+
+        Parameters
+        ----------
+
+        public_key_path: str
+            Path to the public key
+        private_key_path: str
+            Path to private key
+        """
+        _check_type(str, public_key_path, 'public_key_path')
+        _check_type(str, private_key_path, 'private_key_path')
+        self.cryptoKeyReader = _pulsar.CryptoKeyReader(public_key_path, private_key_path)
+
+class Client:
+    """
+    The Pulsar client. A single client instance can be used to create producers
+    and consumers on multiple topics.
+
+    The client will share the same connection pool and threads across all
+    producers and consumers.
+    """
+
+    def __init__(self, service_url,
+                 authentication=None,
+                 operation_timeout_seconds=30,
+                 io_threads=1,
+                 message_listener_threads=1,
+                 concurrent_lookup_requests=50000,
+                 log_conf_file_path=None,
+                 use_tls=False,
+                 tls_trust_certs_file_path=None,
+                 tls_allow_insecure_connection=False,
+                 tls_validate_hostname=False,
+                 logger=None,
+                 connection_timeout_ms=10000,
+                 listener_name=None
+                 ):
+        """
+        Create a new Pulsar client instance.
+
+        Parameters
+        ----------
+
+        service_url: str
+            The Pulsar service url eg: pulsar://my-broker.com:6650/
+        authentication: Authentication, optional
+            Set the authentication provider to be used with the broker. Supported methods:
+
+            * `AuthenticationTLS`
+            * `AuthenticationToken`
+            * `AuthenticationAthenz`
+            * `AuthenticationOauth2`
+        operation_timeout_seconds: int, default=30
+            Set timeout on client operations (subscribe, create producer, close, unsubscribe).
+        io_threads: int, default=1
+            Set the number of IO threads to be used by the Pulsar client.
+        message_listener_threads: int, default=1
+            Set the number of threads to be used by the Pulsar client when delivering messages through
+            message listener. The default is 1 thread per Pulsar client. If using more than 1 thread,
+            messages for distinct ``message_listener``s will be delivered in different threads, however a
+            single ``MessageListener`` will always be assigned to the same thread.
+        concurrent_lookup_requests: int, default=50000
+            Number of concurrent lookup-requests allowed on each broker connection to prevent overload
+            on the broker.
+        log_conf_file_path: str, optional
+            This parameter is deprecated and makes no effect. It's retained only for compatibility.
+            Use `logger` to customize a logger.
+        use_tls: bool, default=False
+            Configure whether to use TLS encryption on the connection. This setting is deprecated.
+            TLS will be automatically enabled if the ``serviceUrl`` is set to ``pulsar+ssl://`` or ``https://``
+        tls_trust_certs_file_path: str, optional
+            Set the path to the trusted TLS certificate file. If empty defaults to certifi.
+        tls_allow_insecure_connection: bool, default=False
+            Configure whether the Pulsar client accepts untrusted TLS certificates from the broker.
+        tls_validate_hostname: bool, default=False
+            Configure whether the Pulsar client validates that the hostname of the endpoint,
+            matches the common name on the TLS certificate presented by the endpoint.
+        logger: optional
+            Set a Python logger for this Pulsar client. Should be an instance of `logging.Logger`.
+            It should be noted that if the Python logger is configured, during the termination of the Python
+            interpreter, the Python logger will be unavailable and the default logger will be used for logging.
+            To avoid strange behavior, you'd better delete all instances explicitly before exiting.
+
+            .. code-block:: python
+
+                import logging
+                client = Client(service_url, logger=logging.getLogger('pulsar'))
+                producer = client.create_producer(topic)
+                # ...
+                del producer
+                del client
+
+        connection_timeout_ms: int, default=10000
+            Set timeout in milliseconds on TCP connections.
+        listener_name: str, optional
+            Listener name for lookup. Clients can use listenerName to choose one of the listeners as
+            the service URL to create a connection to the broker as long as the network is accessible.
+            ``advertisedListeners`` must be enabled in broker side.
+        """
+        _check_type(str, service_url, 'service_url')
+        _check_type_or_none(Authentication, authentication, 'authentication')
+        _check_type(int, operation_timeout_seconds, 'operation_timeout_seconds')
+        _check_type(int, connection_timeout_ms, 'connection_timeout_ms')
+        _check_type(int, io_threads, 'io_threads')
+        _check_type(int, message_listener_threads, 'message_listener_threads')
+        _check_type(int, concurrent_lookup_requests, 'concurrent_lookup_requests')
+        _check_type_or_none(str, log_conf_file_path, 'log_conf_file_path')
+        _check_type(bool, use_tls, 'use_tls')
+        _check_type_or_none(str, tls_trust_certs_file_path, 'tls_trust_certs_file_path')
+        _check_type(bool, tls_allow_insecure_connection, 'tls_allow_insecure_connection')
+        _check_type(bool, tls_validate_hostname, 'tls_validate_hostname')
+        _check_type_or_none(str, listener_name, 'listener_name')
+
+        conf = _pulsar.ClientConfiguration()
+        if authentication:
+            conf.authentication(authentication.auth)
+        conf.operation_timeout_seconds(operation_timeout_seconds)
+        conf.connection_timeout(connection_timeout_ms)
+        conf.io_threads(io_threads)
+        conf.message_listener_threads(message_listener_threads)
+        conf.concurrent_lookup_requests(concurrent_lookup_requests)
+
+        if isinstance(logger, logging.Logger):
+            conf.set_logger(self._prepare_logger(logger))
+        elif isinstance(logger, ConsoleLogger):
+            conf.set_console_logger(logger.log_level)
+        elif isinstance(logger, FileLogger):
+            conf.set_file_logger(logger.log_level, logger.log_file)
+        elif logger is not None:
+            raise ValueError("Logger is expected to be either None, logger.Logger, pulsar.ConsoleLogger or pulsar.FileLogger")
+
+        if listener_name:
+            conf.listener_name(listener_name)
+        if use_tls or service_url.startswith('pulsar+ssl://') or service_url.startswith('https://'):
+            conf.use_tls(True)
+        if tls_trust_certs_file_path:
+            conf.tls_trust_certs_file_path(tls_trust_certs_file_path)
+        else:
+            import certifi
+            conf.tls_trust_certs_file_path(certifi.where())
+        conf.tls_allow_insecure_connection(tls_allow_insecure_connection)
+        conf.tls_validate_hostname(tls_validate_hostname)
+        self._client = _pulsar.Client(service_url, conf)
+        self._consumers = []
+
+    @staticmethod
+    def _prepare_logger(logger):
+        import logging
+        def log(level, message):
+            old_threads = logging.logThreads
+            logging.logThreads = False
+            logger.log(logging.getLevelName(level), message)
+            logging.logThreads = old_threads
+        return log
+
+    def create_producer(self, topic,
+                        producer_name=None,
+                        schema=schema.BytesSchema(),
+                        initial_sequence_id=None,
+                        send_timeout_millis=30000,
+                        compression_type: CompressionType = CompressionType.NONE,
+                        max_pending_messages=1000,
+                        max_pending_messages_across_partitions=50000,
+                        block_if_queue_full=False,
+                        batching_enabled=False,
+                        batching_max_messages=1000,
+                        batching_max_allowed_size_in_bytes=128*1024,
+                        batching_max_publish_delay_ms=10,
+                        chunking_enabled=False,
+                        message_routing_mode: PartitionsRoutingMode = PartitionsRoutingMode.RoundRobinDistribution,
+                        lazy_start_partitioned_producers=False,
+                        properties=None,
+                        batching_type: BatchingType = BatchingType.Default,
+                        encryption_key=None,
+                        crypto_key_reader: Union[None, CryptoKeyReader] = None,
+                        access_mode: ProducerAccessMode = ProducerAccessMode.Shared,
+                        ):
+        """
+        Create a new producer on a given topic.
+
+        Parameters
+        ----------
+
+        topic: str
+            The topic name
+        producer_name: str, optional
+            Specify a name for the producer. If not assigned, the system will generate a globally unique name
+            which can be accessed with `Producer.producer_name()`. When specifying a name, it is app to the user
+            to ensure that, for a given topic, the producer name is unique across all Pulsar's clusters.
+        schema: pulsar.schema.Schema, default=pulsar.schema.BytesSchema
+            Define the schema of the data that will be published by this producer, e.g,
+            ``schema=JsonSchema(MyRecordClass)``.
+
+            The schema will be used for two purposes:
+                * Validate the data format against the topic defined schema
+                * Perform serialization/deserialization between data and objects
+        initial_sequence_id: int, optional
+            Set the baseline for the sequence ids for messages published by the producer. First message will be
+            using ``(initialSequenceId + 1)`` as its sequence id and subsequent messages will be assigned
+            incremental sequence ids, if not otherwise specified.
+        send_timeout_millis: int, default=30000
+            If a message is not acknowledged by the server before the ``send_timeout`` expires, an error will be reported.
+        compression_type: CompressionType, default=CompressionType.NONE
+            Set the compression type for the producer. By default, message payloads are not compressed.
+
+            Supported compression types:
+
+            * CompressionType.LZ4
+            * CompressionType.ZLib
+            * CompressionType.ZSTD
+            * CompressionType.SNAPPY
+
+            ZSTD is supported since Pulsar 2.3. Consumers will need to be at least at that release in order to
+            be able to receive messages compressed with ZSTD.
+
+            SNAPPY is supported since Pulsar 2.4. Consumers will need to be at least at that release in order to
+            be able to receive messages compressed with SNAPPY.
+        batching_enabled: bool, default=False
+            When automatic batching is enabled, multiple calls to `send` can result in a single batch to be sent to the
+            broker, leading to better throughput, especially when publishing small messages.
+            All messages in a batch will be published as a single batched message. The consumer will be delivered
+            individual messages in the batch in the same order they were enqueued.
+        batching_max_messages: int, default=1000
+            When you set this option to a value greater than 1, messages are queued until this threshold or
+            `batching_max_allowed_size_in_bytes` is reached or batch interval has elapsed.
+        batching_max_allowed_size_in_bytes: int, default=128*1024
+            When you set this option to a value greater than 1, messages are queued until this threshold or
+            `batching_max_messages` is reached or batch interval has elapsed.
+        batching_max_publish_delay_ms: int, default=10
+            The batch interval in milliseconds. Queued messages will be sent in batch after this interval even if both
+            the threshold of `batching_max_messages` and `batching_max_allowed_size_in_bytes` are not reached.
+        max_pending_messages: int, default=1000
+            Set the max size of the queue holding the messages pending to receive an acknowledgment from the broker.
+        max_pending_messages_across_partitions: int, default=50000
+            Set the max size of the queue holding the messages pending to receive an acknowledgment across partitions
+            from the broker.
+        block_if_queue_full: bool, default=False
+            Set whether `send_async` operations should block when the outgoing message queue is full.
+        message_routing_mode: PartitionsRoutingMode, default=PartitionsRoutingMode.RoundRobinDistribution
+            Set the message routing mode for the partitioned producer.
+
+            Supported modes:
+
+            * ``PartitionsRoutingMode.RoundRobinDistribution``
+            * ``PartitionsRoutingMode.UseSinglePartition``
+        lazy_start_partitioned_producers: bool, default=False
+            This config affects producers of partitioned topics only. It controls whether producers register
+            and connect immediately to the owner broker of each partition or start lazily on demand. The internal
+            producer of one partition is always started eagerly, chosen by the routing policy, but the internal
+            producers of any additional partitions are started on demand, upon receiving their first message.
+
+            Using this mode can reduce the strain on brokers for topics with large numbers of partitions and when
+            the SinglePartition routing policy is used without keyed messages. Because producer connection can be
+            on demand, this can produce extra send latency for the first messages of a given partition.
+        properties: dict, optional
+            Sets the properties for the producer. The properties associated with a producer can be used for identify
+            a producer at broker side.
+        batching_type: BatchingType, default=BatchingType.Default
+            Sets the batching type for the producer.
+
+            There are two batching type: DefaultBatching and KeyBasedBatching.
+
+            DefaultBatching will batch single messages:
+                (k1, v1), (k2, v1), (k3, v1), (k1, v2), (k2, v2), (k3, v2), (k1, v3), (k2, v3), (k3, v3)
+            ... into single batch message:
+                [(k1, v1), (k2, v1), (k3, v1), (k1, v2), (k2, v2), (k3, v2), (k1, v3), (k2, v3), (k3, v3)]
+
+            KeyBasedBatching will batch incoming single messages:
+                (k1, v1), (k2, v1), (k3, v1), (k1, v2), (k2, v2), (k3, v2), (k1, v3), (k2, v3), (k3, v3)
+            ... into single batch message:
+                [(k1, v1), (k1, v2), (k1, v3)], [(k2, v1), (k2, v2), (k2, v3)], [(k3, v1), (k3, v2), (k3, v3)]
+        chunking_enabled: bool, default=False
+            If message size is higher than allowed max publish-payload size by broker then chunking_enabled helps
+            producer to split message into multiple chunks and publish them to broker separately and in order.
+            So, it allows client to successfully publish large size of messages in pulsar.
+        encryption_key: str, optional
+            The key used for symmetric encryption, configured on the producer side
+        crypto_key_reader: CryptoKeyReader, optional
+            Symmetric encryption class implementation, configuring public key encryption messages for the producer
+            and private key decryption messages for the consumer
+        access_mode: ProducerAccessMode, optional
+            Set the type of access mode that the producer requires on the topic.
+
+            Supported modes:
+
+            * Shared: By default multiple producers can publish on a topic.
+            * Exclusive: Require exclusive access for producer.
+                         Fail immediately if there's already a producer connected.
+            * WaitForExclusive: Producer creation is pending until it can acquire exclusive access.
+            * ExclusiveWithFencing: Acquire exclusive access for the producer.
+                                    Any existing producer will be removed and invalidated immediately.
+        """
+        _check_type(str, topic, 'topic')
+        _check_type_or_none(str, producer_name, 'producer_name')
+        _check_type(_schema.Schema, schema, 'schema')
+        _check_type_or_none(int, initial_sequence_id, 'initial_sequence_id')
+        _check_type(int, send_timeout_millis, 'send_timeout_millis')
+        _check_type(CompressionType, compression_type, 'compression_type')
+        _check_type(int, max_pending_messages, 'max_pending_messages')
+        _check_type(int, max_pending_messages_across_partitions, 'max_pending_messages_across_partitions')
+        _check_type(bool, block_if_queue_full, 'block_if_queue_full')
+        _check_type(bool, batching_enabled, 'batching_enabled')
+        _check_type(int, batching_max_messages, 'batching_max_messages')
+        _check_type(int, batching_max_allowed_size_in_bytes, 'batching_max_allowed_size_in_bytes')
+        _check_type(int, batching_max_publish_delay_ms, 'batching_max_publish_delay_ms')
+        _check_type(bool, chunking_enabled, 'chunking_enabled')
+        _check_type_or_none(dict, properties, 'properties')
+        _check_type(BatchingType, batching_type, 'batching_type')
+        _check_type_or_none(str, encryption_key, 'encryption_key')
+        _check_type_or_none(CryptoKeyReader, crypto_key_reader, 'crypto_key_reader')
+        _check_type(bool, lazy_start_partitioned_producers, 'lazy_start_partitioned_producers')
+        _check_type(ProducerAccessMode, access_mode, 'access_mode')
+
+        conf = _pulsar.ProducerConfiguration()
+        conf.send_timeout_millis(send_timeout_millis)
+        conf.compression_type(compression_type)
+        conf.max_pending_messages(max_pending_messages)
+        conf.max_pending_messages_across_partitions(max_pending_messages_across_partitions)
+        conf.block_if_queue_full(block_if_queue_full)
+        conf.batching_enabled(batching_enabled)
+        conf.batching_max_messages(batching_max_messages)
+        conf.batching_max_allowed_size_in_bytes(batching_max_allowed_size_in_bytes)
+        conf.batching_max_publish_delay_ms(batching_max_publish_delay_ms)
+        conf.partitions_routing_mode(message_routing_mode)
+        conf.batching_type(batching_type)
+        conf.chunking_enabled(chunking_enabled)
+        conf.lazy_start_partitioned_producers(lazy_start_partitioned_producers)
+        conf.access_mode(access_mode)
+        if producer_name:
+            conf.producer_name(producer_name)
+        if initial_sequence_id:
+            conf.initial_sequence_id(initial_sequence_id)
+        if properties:
+            for k, v in properties.items():
+                conf.property(k, v)
+
+        conf.schema(schema.schema_info())
+        if encryption_key:
+            conf.encryption_key(encryption_key)
+        if crypto_key_reader:
+            conf.crypto_key_reader(crypto_key_reader.cryptoKeyReader)
+
+        if batching_enabled and chunking_enabled:
+            raise ValueError("Batching and chunking of messages can't be enabled together.")
+
+        p = Producer()
+        p._producer = self._client.create_producer(topic, conf)
+        p._schema = schema
+        p._client = self._client
+        return p
+
+    def subscribe(self, topic, subscription_name,
+                  consumer_type: ConsumerType = ConsumerType.Exclusive,
+                  schema=schema.BytesSchema(),
+                  message_listener=None,
+                  receiver_queue_size=1000,
+                  max_total_receiver_queue_size_across_partitions=50000,
+                  consumer_name=None,
+                  unacked_messages_timeout_ms=None,
+                  broker_consumer_stats_cache_time_ms=30000,
+                  negative_ack_redelivery_delay_ms=60000,
+                  is_read_compacted=False,
+                  properties=None,
+                  pattern_auto_discovery_period=60,
+                  initial_position: InitialPosition = InitialPosition.Latest,
+                  crypto_key_reader: Union[None, CryptoKeyReader] = None,
+                  replicate_subscription_state_enabled=False,
+                  max_pending_chunked_message=10,
+                  auto_ack_oldest_chunked_message_on_queue_full=False,
+                  start_message_id_inclusive=False,
+                  batch_receive_policy=None,
+                  key_shared_policy=None,
+                  batch_index_ack_enabled=False,
+                  regex_subscription_mode: RegexSubscriptionMode = RegexSubscriptionMode.PersistentOnly,
+                  dead_letter_policy: Union[None, ConsumerDeadLetterPolicy] = None,
+                  ):
+        """
+        Subscribe to the given topic and subscription combination.
+
+        Parameters
+        ----------
+
+        topic:
+            The name of the topic, list of topics or regex pattern. This method will accept these forms:
+            * ``topic='my-topic'``
+            * ``topic=['topic-1', 'topic-2', 'topic-3']``
+            * ``topic=re.compile('persistent://public/default/topic-*')``
+        subscription_name: str
+            The name of the subscription.
+        consumer_type: ConsumerType, default=ConsumerType.Exclusive
+            Select the subscription type to be used when subscribing to the topic.
+        schema: pulsar.schema.Schema, default=pulsar.schema.BytesSchema
+            Define the schema of the data that will be received by this consumer.
+        message_listener: optional
+            Sets a message listener for the consumer. When the listener is set, the application will
+            receive messages through it. Calls to ``consumer.receive()`` will not be allowed.
+            The listener function needs to accept (consumer, message), for example:
+
+            .. code-block:: python
+
+                def my_listener(consumer, message):
+                    # process message
+                    consumer.acknowledge(message)
+        receiver_queue_size: int, default=1000
+            Sets the size of the consumer receive queue. The consumer receive queue controls how many messages can be
+            accumulated by the consumer before the application calls `receive()`. Using a higher value could potentially
+            increase the consumer throughput at the expense of higher memory utilization. Setting the consumer queue
+            size to zero decreases the throughput of the consumer by disabling pre-fetching of messages.
+
+            This approach improves the message distribution on shared subscription by pushing messages only to those
+            consumers that are ready to process them. Neither receive with timeout nor partitioned topics can be used
+            if the consumer queue size is zero. The `receive()` function call should not be interrupted when the
+            consumer queue size is zero. The default value is 1000 messages and should work well for most use cases.
+        max_total_receiver_queue_size_across_partitions: int, default=50000
+            Set the max total receiver queue size across partitions. This setting will be used to reduce the
+            receiver queue size for individual partitions
+        consumer_name: str, optional
+            Sets the consumer name.
+        unacked_messages_timeout_ms: int, optional
+            Sets the timeout in milliseconds for unacknowledged messages. The timeout needs to be greater than
+            10 seconds. An exception is thrown if the given value is less than 10 seconds. If a successful
+            acknowledgement is not sent within the timeout, all the unacknowledged messages are redelivered.
+        negative_ack_redelivery_delay_ms: int, default=60000
+            The delay after which to redeliver the messages that failed to be processed
+            (with the ``consumer.negative_acknowledge()``)
+        broker_consumer_stats_cache_time_ms: int, default=30000
+            Sets the time duration for which the broker-side consumer stats will be cached in the client.
+        is_read_compacted: bool, default=False
+            Selects whether to read the compacted version of the topic
+        properties: dict, optional
+            Sets the properties for the consumer. The properties associated with a consumer can be used for
+            identify a consumer at broker side.
+        pattern_auto_discovery_period: int, default=60
+            Periods of seconds for consumer to auto discover match topics.
+        initial_position: InitialPosition, default=InitialPosition.Latest
+          Set the initial position of a consumer when subscribing to the topic.
+          It could be either: ``InitialPosition.Earliest`` or ``InitialPosition.Latest``.
+        crypto_key_reader: CryptoKeyReader, optional
+            Symmetric encryption class implementation, configuring public key encryption messages for the producer
+            and private key decryption messages for the consumer
+        replicate_subscription_state_enabled: bool, default=False
+            Set whether the subscription status should be replicated.
+        max_pending_chunked_message: int, default=10
+          Consumer buffers chunk messages into memory until it receives all the chunks of the original message.
+          While consuming chunk-messages, chunks from same message might not be contiguous in the stream, and they
+          might be mixed with other messages' chunks. so, consumer has to maintain multiple buffers to manage
+          chunks coming from different messages. This mainly happens when multiple publishers are publishing
+          messages on the topic concurrently or publisher failed to publish all chunks of the messages.
+
+          If it's zero, the pending chunked messages will not be limited.
+        auto_ack_oldest_chunked_message_on_queue_full: bool, default=False
+          Buffering large number of outstanding uncompleted chunked messages can create memory pressure, and it
+          can be guarded by providing the maxPendingChunkedMessage threshold. See setMaxPendingChunkedMessage.
+          Once, consumer reaches this threshold, it drops the outstanding unchunked-messages by silently acking
+          if autoAckOldestChunkedMessageOnQueueFull is true else it marks them for redelivery.
+        start_message_id_inclusive: bool, default=False
+          Set the consumer to include the given position of any reset operation like Consumer::seek.
+        batch_receive_policy: class ConsumerBatchReceivePolicy
+          Set the batch collection policy for batch receiving.
+        key_shared_policy: class ConsumerKeySharedPolicy
+            Set the key shared policy for use when the ConsumerType is KeyShared.
+        batch_index_ack_enabled: Enable the batch index acknowledgement.
+            It should be noted that this option can only work when the broker side also enables the batch index
+            acknowledgement. See the `acknowledgmentAtBatchIndexLevelEnabled` config in `broker.conf`.
+        regex_subscription_mode: RegexSubscriptionMode, optional
+            Set the regex subscription mode for use when the topic is a regex pattern.
+
+            Supported modes:
+
+            * PersistentOnly: By default only subscribe to persistent topics.
+            * NonPersistentOnly: Only subscribe to non-persistent topics.
+            * AllTopics: Subscribe to both persistent and non-persistent topics.
+        dead_letter_policy: class ConsumerDeadLetterPolicy
+          Set dead letter policy for consumer.
+          By default, some messages are redelivered many times, even to the extent that they can never be
+          stopped. By using the dead letter mechanism, messages have the max redelivery count, when they're
+          exceeding the maximum number of redeliveries. Messages are sent to dead letter topics and acknowledged
+          automatically.
+        """
+        _check_type(str, subscription_name, 'subscription_name')
+        _check_type(ConsumerType, consumer_type, 'consumer_type')
+        _check_type(_schema.Schema, schema, 'schema')
+        _check_type(int, receiver_queue_size, 'receiver_queue_size')
+        _check_type(int, max_total_receiver_queue_size_across_partitions,
+                    'max_total_receiver_queue_size_across_partitions')
+        _check_type_or_none(str, consumer_name, 'consumer_name')
+        _check_type_or_none(int, unacked_messages_timeout_ms, 'unacked_messages_timeout_ms')
+        _check_type(int, broker_consumer_stats_cache_time_ms, 'broker_consumer_stats_cache_time_ms')
+        _check_type(int, negative_ack_redelivery_delay_ms, 'negative_ack_redelivery_delay_ms')
+        _check_type(int, pattern_auto_discovery_period, 'pattern_auto_discovery_period')
+        _check_type(bool, is_read_compacted, 'is_read_compacted')
+        _check_type_or_none(dict, properties, 'properties')
+        _check_type(InitialPosition, initial_position, 'initial_position')
+        _check_type_or_none(CryptoKeyReader, crypto_key_reader, 'crypto_key_reader')
+        _check_type(int, max_pending_chunked_message, 'max_pending_chunked_message')
+        _check_type(bool, auto_ack_oldest_chunked_message_on_queue_full, 'auto_ack_oldest_chunked_message_on_queue_full')
+        _check_type(bool, start_message_id_inclusive, 'start_message_id_inclusive')
+        _check_type_or_none(ConsumerBatchReceivePolicy, batch_receive_policy, 'batch_receive_policy')
+        _check_type_or_none(ConsumerKeySharedPolicy, key_shared_policy, 'key_shared_policy')
+        _check_type(bool, batch_index_ack_enabled, 'batch_index_ack_enabled')
+        _check_type(RegexSubscriptionMode, regex_subscription_mode, 'regex_subscription_mode')
+
+        conf = _pulsar.ConsumerConfiguration()
+        conf.consumer_type(consumer_type)
+        conf.regex_subscription_mode(regex_subscription_mode)
+        conf.read_compacted(is_read_compacted)
+        if message_listener:
+            conf.message_listener(_listener_wrapper(message_listener, schema))
+        conf.receiver_queue_size(receiver_queue_size)
+        conf.max_total_receiver_queue_size_across_partitions(max_total_receiver_queue_size_across_partitions)
+        if consumer_name:
+            conf.consumer_name(consumer_name)
+        if unacked_messages_timeout_ms:
+            conf.unacked_messages_timeout_ms(unacked_messages_timeout_ms)
+
+        conf.negative_ack_redelivery_delay_ms(negative_ack_redelivery_delay_ms)
+        conf.broker_consumer_stats_cache_time_ms(broker_consumer_stats_cache_time_ms)
+        if properties:
+            for k, v in properties.items():
+                conf.property(k, v)
+        conf.subscription_initial_position(initial_position)
+
+        conf.schema(schema.schema_info())
+
+        if crypto_key_reader:
+            conf.crypto_key_reader(crypto_key_reader.cryptoKeyReader)
+
+        conf.replicate_subscription_state_enabled(replicate_subscription_state_enabled)
+        conf.max_pending_chunked_message(max_pending_chunked_message)
+        conf.auto_ack_oldest_chunked_message_on_queue_full(auto_ack_oldest_chunked_message_on_queue_full)
+        conf.start_message_id_inclusive(start_message_id_inclusive)
+        if batch_receive_policy:
+            conf.batch_receive_policy(batch_receive_policy.policy())
+
+        if key_shared_policy:
+            conf.key_shared_policy(key_shared_policy.policy())
+        conf.batch_index_ack_enabled(batch_index_ack_enabled)
+        if dead_letter_policy:
+            conf.dead_letter_policy(dead_letter_policy.policy())
+
+        c = Consumer()
+        if isinstance(topic, str):
+            # Single topic
+            c._consumer = self._client.subscribe(topic, subscription_name, conf)
+        elif isinstance(topic, list):
+            # List of topics
+            c._consumer = self._client.subscribe_topics(topic, subscription_name, conf)
+        elif isinstance(topic, _retype):
+            # Regex pattern
+            c._consumer = self._client.subscribe_pattern(topic.pattern, subscription_name, conf)
+        else:
+            raise ValueError("Argument 'topic' is expected to be of a type between (str, list, re.pattern)")
+
+        c._client = self
+        c._schema = schema
+        c._schema.attach_client(self._client)
+        self._consumers.append(c)
+        return c
+
+    def create_reader(self, topic, start_message_id,
+                      schema=schema.BytesSchema(),
+                      reader_listener=None,
+                      receiver_queue_size=1000,
+                      reader_name=None,
+                      subscription_role_prefix=None,
+                      is_read_compacted=False,
+                      crypto_key_reader: Union[None, CryptoKeyReader] = None,
+                      start_message_id_inclusive=False
+                      ):
+        """
+        Create a reader on a particular topic
+
+        Parameters
+        ----------
+
+        topic:
+            The name of the topic.
+        start_message_id:
+            The initial reader positioning is done by specifying a message id. The options are:
+
+            * ``MessageId.earliest``:
+
+            Start reading from the earliest message available in the topic
+
+            * ``MessageId.latest``:
+
+            Start reading from the end topic, only getting messages published after the reader was created
+
+            * ``MessageId``:
+
+            When passing a particular message id, the reader will position itself on that specific position.
+            The first message to be read will be the message next to the specified messageId.
+            Message id can be serialized into a string and deserialized back into a `MessageId` object:
+
+               .. code-block:: python
+
+                   # Serialize to string
+                   s = msg.message_id().serialize()
+
+                   # Deserialize from string
+                   msg_id = MessageId.deserialize(s)
+        schema: pulsar.schema.Schema, default=pulsar.schema.BytesSchema
+            Define the schema of the data that will be received by this reader.
+        reader_listener: optional
+            Sets a message listener for the reader. When the listener is set, the application will receive messages
+            through it. Calls to ``reader.read_next()`` will not be allowed. The listener function needs to accept
+            (reader, message), for example:
+
+            .. code-block:: python
+
+                def my_listener(reader, message):
+                    # process message
+                    pass
+        receiver_queue_size: int, default=1000
+            Sets the size of the reader receive queue. The reader receive queue controls how many messages can be
+            accumulated by the reader before the application calls `read_next()`. Using a higher value could
+            potentially increase the reader throughput at the expense of higher memory utilization.
+        reader_name: str, optional
+            Sets the reader name.
+        subscription_role_prefix: str, optional
+            Sets the subscription role prefix.
+        is_read_compacted: bool, default=False
+            Selects whether to read the compacted version of the topic
+        crypto_key_reader: CryptoKeyReader, optional
+            Symmetric encryption class implementation, configuring public key encryption messages for the producer
+            and private key decryption messages for the consumer
+        start_message_id_inclusive: bool, default=False
+            Set the reader to include the startMessageId or given position of any reset operation like Reader.seek
+        """
+
+        # If a pulsar.MessageId object is passed, access the _pulsar.MessageId object
+        if isinstance(start_message_id, MessageId):
+            start_message_id = start_message_id._msg_id
+
+        _check_type(str, topic, 'topic')
+        _check_type(_pulsar.MessageId, start_message_id, 'start_message_id')
+        _check_type(_schema.Schema, schema, 'schema')
+        _check_type(int, receiver_queue_size, 'receiver_queue_size')
+        _check_type_or_none(str, reader_name, 'reader_name')
+        _check_type_or_none(str, subscription_role_prefix, 'subscription_role_prefix')
+        _check_type(bool, is_read_compacted, 'is_read_compacted')
+        _check_type_or_none(CryptoKeyReader, crypto_key_reader, 'crypto_key_reader')
+        _check_type(bool, start_message_id_inclusive, 'start_message_id_inclusive')
+
+        conf = _pulsar.ReaderConfiguration()
+        if reader_listener:
+            conf.reader_listener(_listener_wrapper(reader_listener, schema))
+        conf.receiver_queue_size(receiver_queue_size)
+        if reader_name:
+            conf.reader_name(reader_name)
+        if subscription_role_prefix:
+            conf.subscription_role_prefix(subscription_role_prefix)
+        conf.schema(schema.schema_info())
+        conf.read_compacted(is_read_compacted)
+        if crypto_key_reader:
+            conf.crypto_key_reader(crypto_key_reader.cryptoKeyReader)
+        conf.start_message_id_inclusive(start_message_id_inclusive)
+
+        c = Reader()
+        c._reader = self._client.create_reader(topic, start_message_id, conf)
+        c._client = self
+        c._schema = schema
+        c._schema.attach_client(self._client)
+        self._consumers.append(c)
+        return c
+
+    def get_topic_partitions(self, topic):
+        """
+        Get the list of partitions for a given topic.
+
+        If the topic is partitioned, this will return a list of partition names. If the topic is not
+        partitioned, the returned list will contain the topic name itself.
+
+        This can be used to discover the partitions and create Reader, Consumer or Producer
+        instances directly on a particular partition.
+
+        Parameters
+        ----------
+
+        topic: str
+            the topic name to lookup
+
+        Returns
+        -------
+        list
+            a list of partition name
+        """
+        _check_type(str, topic, 'topic')
+        return self._client.get_topic_partitions(topic)
+
+    def shutdown(self):
+        """
+        Perform immediate shutdown of Pulsar client.
+
+        Release all resources and close all producer, consumer, and readers without waiting
+        for ongoing operations to complete.
+        """
+        self._client.shutdown()
+
+    def close(self):
+        """
+        Close the client and all the associated producers and consumers
+        """
+        self._client.close()
+
+
+class Producer:
+    """
+    The Pulsar message producer, used to publish messages on a topic.
+
+    Examples
+    --------
+
+    .. code-block:: python
+
+        import pulsar
+
+        client = pulsar.Client('pulsar://localhost:6650')
+        producer = client.create_producer('my-topic')
+        for i in range(10):
+            producer.send(('Hello-%d' % i).encode('utf-8'))
+        client.close()
+    """
+
+    def topic(self):
+        """
+        Return the topic which producer is publishing to
+        """
+        return self._producer.topic()
+
+    def producer_name(self):
+        """
+        Return the producer name which could have been assigned by the
+        system or specified by the client
+        """
+        return self._producer.producer_name()
+
+    def last_sequence_id(self):
+        """
+        Get the last sequence id that was published by this producer.
+
+        This represents either the automatically assigned or custom sequence id
+        (set on the ``MessageBuilder``) that was published and acknowledged by the broker.
+
+        After recreating a producer with the same producer name, this will return the
+        last message that was published in the previous producer session, or -1 if
+        there was no message ever published.
+        """
+        return self._producer.last_sequence_id()
+
+    def send(self, content,
+             properties=None,
+             partition_key=None,
+             ordering_key=None,
+             sequence_id=None,
+             replication_clusters=None,
+             disable_replication=False,
+             event_timestamp=None,
+             deliver_at=None,
+             deliver_after=None,
+             ):
+        """
+        Publish a message on the topic. Blocks until the message is acknowledged
+
+        Returns a `MessageId` object that represents where the message is persisted.
+
+        Parameters
+        ----------
+
+        content:
+            A ``bytes`` object with the message payload.
+        properties: optional
+            A dict of application-defined string properties.
+        partition_key: optional
+            Sets the partition key for message routing. A hash of this key is used
+            to determine the message's topic partition.
+        ordering_key: optional
+            Sets the ordering key for message routing.
+        sequence_id:  optional
+            Specify a custom sequence id for the message being published.
+        replication_clusters:  optional
+          Override namespace replication clusters. Note that it is the caller's responsibility to provide valid
+          cluster names and that all clusters have been previously configured as topics. Given an empty list,
+          the message will replicate according to the namespace configuration.
+        disable_replication: bool, default=False
+            Do not replicate this message.
+        event_timestamp: optional
+            Timestamp in millis of the timestamp of event creation
+        deliver_at: optional
+            Specify the message should not be delivered earlier than the specified timestamp.
+            The timestamp is milliseconds and based on UTC
+        deliver_after: optional
+            Specify a delay in timedelta for the delivery of the messages.
+        """
+        msg = self._build_msg(content, properties, partition_key, ordering_key, sequence_id,
+                              replication_clusters, disable_replication, event_timestamp,
+                              deliver_at, deliver_after)
+        return self._producer.send(msg)
+
+    def send_async(self, content, callback,
+                   properties=None,
+                   partition_key=None,
+                   ordering_key=None,
+                   sequence_id=None,
+                   replication_clusters=None,
+                   disable_replication=False,
+                   event_timestamp=None,
+                   deliver_at=None,
+                   deliver_after=None,
+                   ):
+        """
+        Send a message asynchronously.
+
+        Examples
+        --------
+
+        The ``callback`` will be invoked once the message has been acknowledged by the broker.
+        Users are responsible to handle the exception inside the callback. If any exception was
+        thrown from the callback, the process would terminate immediately.
+
+        .. code-block:: python
+
+            import pulsar
+
+            client = pulsar.Client('pulsar://localhost:6650')
+            producer = client.create_producer(
+                            'my-topic',
+                            block_if_queue_full=True,
+                            batching_enabled=True,
+                            batching_max_publish_delay_ms=10)
+
+            def callback(res, msg_id):
+                print('Message published res=%s', res)
+
+            while True:
+                producer.send_async(('Hello-%d' % i).encode('utf-8'), callback)
+
+            client.close()
+
+
+        When the producer queue is full, by default the message will be rejected
+        and the callback invoked with an error code.
+
+
+        Parameters
+        ----------
+
+        content
+            A `bytes` object with the message payload.
+        callback
+            A callback that is invoked once the message has been acknowledged by the broker.
+        properties: optional
+            A dict of application0-defined string properties.
+        partition_key: optional
+            Sets the partition key for the message routing. A hash of this key is
+            used to determine the message's topic partition.
+        ordering_key: optional
+            Sets the ordering key for the message routing.
+        sequence_id: optional
+            Specify a custom sequence id for the message being published.
+        replication_clusters: optional
+            Override namespace replication clusters. Note that it is the caller's responsibility
+            to provide valid cluster names and that all clusters have been previously configured
+            as topics. Given an empty list, the message will replicate per the namespace configuration.
+        disable_replication: optional
+            Do not replicate this message.
+        event_timestamp: optional
+            Timestamp in millis of the timestamp of event creation
+        deliver_at: optional
+            Specify the message should not be delivered earlier than the specified timestamp.
+        deliver_after: optional
+            Specify a delay in timedelta for the delivery of the messages.
+        """
+        msg = self._build_msg(content, properties, partition_key, ordering_key, sequence_id,
+                              replication_clusters, disable_replication, event_timestamp,
+                              deliver_at, deliver_after)
+        self._producer.send_async(msg, callback)
+
+
+    def flush(self):
+        """
+        Flush all the messages buffered in the client and wait until all messages have been
+        successfully persisted
+        """
+        self._producer.flush()
+
+
+    def close(self):
+        """
+        Close the producer.
+        """
+        self._producer.close()
+
+    def _build_msg(self, content, properties, partition_key, ordering_key, sequence_id,
+                   replication_clusters, disable_replication, event_timestamp,
+                   deliver_at, deliver_after):
+        data = self._schema.encode(content)
+
+        _check_type(bytes, data, 'data')
+        _check_type_or_none(dict, properties, 'properties')
+        _check_type_or_none(str, partition_key, 'partition_key')
+        _check_type_or_none(str, ordering_key, 'ordering_key')
+        _check_type_or_none(int, sequence_id, 'sequence_id')
+        _check_type_or_none(list, replication_clusters, 'replication_clusters')
+        _check_type(bool, disable_replication, 'disable_replication')
+        _check_type_or_none(int, event_timestamp, 'event_timestamp')
+        _check_type_or_none(int, deliver_at, 'deliver_at')
+        _check_type_or_none(timedelta, deliver_after, 'deliver_after')
+
+        mb = _pulsar.MessageBuilder()
+        mb.content(data)
+        if properties:
+            for k, v in properties.items():
+                mb.property(k, v)
+        if partition_key:
+            mb.partition_key(partition_key)
+        if ordering_key:
+            mb.ordering_key(ordering_key)
+        if sequence_id:
+            mb.sequence_id(sequence_id)
+        if replication_clusters:
+            mb.replication_clusters(replication_clusters)
+        if disable_replication:
+            mb.disable_replication(disable_replication)
+        if event_timestamp:
+            mb.event_timestamp(event_timestamp)
+        if deliver_at:
+            mb.deliver_at(deliver_at)
+        if deliver_after:
+            mb.deliver_after(deliver_after)
+
+        return mb.build()
+
+    def is_connected(self):
+        """
+        Check if the producer is connected or not.
+        """
+        return self._producer.is_connected()
+
+
+class Consumer:
+    """
+    Pulsar consumer.
+
+    Examples
+    --------
+
+    .. code-block:: python
+
+        import pulsar
+
+        client = pulsar.Client('pulsar://localhost:6650')
+        consumer = client.subscribe('my-topic', 'my-subscription')
+        while True:
+            msg = consumer.receive()
+            try:
+                print("Received message '{}' id='{}'".format(msg.data(), msg.message_id()))
+                consumer.acknowledge(msg)
+            except Exception:
+                consumer.negative_acknowledge(msg)
+        client.close()
+    """
+
+    def topic(self):
+        """
+        Return the topic this consumer is subscribed to.
+        """
+        return self._consumer.topic()
+
+    def subscription_name(self):
+        """
+        Return the subscription name.
+        """
+        return self._consumer.subscription_name()
+
+    def consumer_name(self):
+        """
+        Return the consumer name.
+        """
+        return self._consumer.consumer_name()
+
+    def unsubscribe(self):
+        """
+        Unsubscribe the current consumer from the topic.
+
+        This method will block until the operation is completed. Once the
+        consumer is unsubscribed, no more messages will be received and
+        subsequent new messages will not be retained for this consumer.
+
+        This consumer object cannot be reused.
+        """
+        return self._consumer.unsubscribe()
+
+    def receive(self, timeout_millis=None):
+        """
+        Receive a single message.
+
+        If a message is not immediately available, this method will block until
+        a new message is available.
+
+        Parameters
+        ----------
+
+        timeout_millis: int, optional
+            If specified, the receiver will raise an exception if a message is not available within the timeout.
+        """
+        if timeout_millis is None:
+            msg = self._consumer.receive()
+        else:
+            _check_type(int, timeout_millis, 'timeout_millis')
+            msg = self._consumer.receive(timeout_millis)
+
+        m = Message()
+        m._message = msg
+        m._schema = self._schema
+        return m
+
+    def batch_receive(self):
+        """
+        Batch receiving messages.
+
+        This calls blocks until has enough messages or wait timeout, more details to see {@link BatchReceivePolicy}.
+        """
+        messages = []
+        msgs = self._consumer.batch_receive()
+        for msg in msgs:
+            m = Message()
+            m._message = msg
+            messages.append(m)
+        return messages
+
+    def acknowledge(self, message):
+        """
+        Acknowledge the reception of a single message.
+
+        This method will block until an acknowledgement is sent to the broker.
+        After that, the message will not be re-delivered to this consumer.
+
+        Parameters
+        ----------
+        message : Message, _pulsar.Message, _pulsar.MessageId
+            The received message or message id.
+
+        Raises
+        ------
+        OperationNotSupported
+             if ``message`` is not allowed to acknowledge
+        """
+        if isinstance(message, Message):
+            self._consumer.acknowledge(message._message)
+        else:
+            self._consumer.acknowledge(message)
+
+    def acknowledge_cumulative(self, message):
+        """
+        Acknowledge the reception of all the messages in the stream up to (and
+        including) the provided message.
+
+        This method will block until an acknowledgement is sent to the broker.
+        After that, the messages will not be re-delivered to this consumer.
+
+        Parameters
+        ----------
+
+        message:
+            The received message or message id.
+
+        Raises
+        ------
+        CumulativeAcknowledgementNotAllowedError
+            if the consumer type is ConsumerType.KeyShared or ConsumerType.Shared
+        """
+        if isinstance(message, Message):
+            self._consumer.acknowledge_cumulative(message._message)
+        else:
+            self._consumer.acknowledge_cumulative(message)
+
+    def negative_acknowledge(self, message):
+        """
+        Acknowledge the failure to process a single message.
+
+        When a message is "negatively acked" it will be marked for redelivery after
+        some fixed delay. The delay is configurable when constructing the consumer
+        with {@link ConsumerConfiguration#setNegativeAckRedeliveryDelayMs}.
+
+        This call is not blocking.
+
+        Parameters
+        ----------
+
+        message:
+            The received message or message id.
+        """
+        if isinstance(message, Message):
+            self._consumer.negative_acknowledge(message._message)
+        else:
+            self._consumer.negative_acknowledge(message)
+
+    def pause_message_listener(self):
+        """
+        Pause receiving messages via the ``message_listener`` until `resume_message_listener()` is called.
+        """
+        self._consumer.pause_message_listener()
+
+    def resume_message_listener(self):
+        """
+        Resume receiving the messages via the message listener.
+        Asynchronously receive all the messages enqueued from the time
+        `pause_message_listener()` was called.
+        """
+        self._consumer.resume_message_listener()
+
+    def redeliver_unacknowledged_messages(self):
+        """
+        Redelivers all the unacknowledged messages. In failover mode, the
+        request is ignored if the consumer is not active for the given topic. In
+        shared mode, the consumer's messages to be redelivered are distributed
+        across all the connected consumers. This is a non-blocking call and
+        doesn't throw an exception. In case the connection breaks, the messages
+        are redelivered after reconnect.
+        """
+        self._consumer.redeliver_unacknowledged_messages()
+
+    def seek(self, messageid):
+        """
+        Reset the subscription associated with this consumer to a specific message id or publish timestamp.
+        The message id can either be a specific message or represent the first or last messages in the topic.
+        Note: this operation can only be done on non-partitioned topics. For these, one can rather perform the
+        seek() on the individual partitions.
+
+        Parameters
+        ----------
+
+        messageid:
+            The message id for seek, OR an integer event time to seek to
+        """
+        self._consumer.seek(messageid)
+
+    def close(self):
+        """
+        Close the consumer.
+        """
+        self._consumer.close()
+        self._client._consumers.remove(self)
+
+    def is_connected(self):
+        """
+        Check if the consumer is connected or not.
+        """
+        return self._consumer.is_connected()
+
+    def get_last_message_id(self):
+        """
+        Get the last message id.
+        """
+        return self._consumer.get_last_message_id()
+
+class ConsumerBatchReceivePolicy:
+    """
+    Batch receive policy can limit the number and bytes of messages in a single batch,
+    and can specify a timeout for waiting for enough messages for this batch.
+
+    A batch receive action is completed as long as any one of the conditions (the batch has enough number
+    or size of messages, or the waiting timeout is passed) are met.
+    """
+    def __init__(self, max_num_message, max_num_bytes, timeout_ms):
+        """
+        Wrapper BatchReceivePolicy.
+
+        Parameters
+        ----------
+
+        max_num_message: Max num message, if less than 0, it means no limit. default: -1
+        max_num_bytes: Max num bytes, if less than 0, it means no limit. default: 10 * 1024 * 1024
+        timeout_ms: If less than 0, it means no limit. default: 100
+        """
+        self._policy = BatchReceivePolicy(max_num_message, max_num_bytes, timeout_ms)
+
+    def policy(self):
+        """
+        Returns the actual one BatchReceivePolicy.
+        """
+        return self._policy
+
+class ConsumerKeySharedPolicy:
+    """
+    Consumer key shared policy is used to configure the consumer behaviour when the ConsumerType is KeyShared.
+    """
+    def __init__(
+            self,
+            key_shared_mode: KeySharedMode = KeySharedMode.AutoSplit,
+            allow_out_of_order_delivery: bool = False,
+            sticky_ranges: Optional[List[Tuple[int, int]]] = None,
+    ):
+        """
+        Wrapper KeySharedPolicy.
+
+        Parameters
+        ----------
+
+        key_shared_mode: KeySharedMode, optional
+            Set the key shared mode. eg: KeySharedMode.Sticky or KeysharedMode.AutoSplit
+
+        allow_out_of_order_delivery: bool, optional
+            Set whether to allow for out of order delivery
+            If it is enabled, it relaxes the ordering requirement and allows the broker to send out-of-order
+            messages in case of failures. This makes it faster for new consumers to join without being stalled by
+            an existing slow consumer.
+
+            If this is True, a single consumer still receives all keys, but they may come in different orders.
+
+        sticky_ranges: List[Tuple[int, int]], optional
+            Set the ranges used with sticky mode. The integers can be from 0 to 2^16 (0 <= val < 65,536)
+        """
+        if key_shared_mode == KeySharedMode.Sticky and sticky_ranges is None:
+            raise ValueError("When using key_shared_mode = KeySharedMode.Sticky you must also provide sticky_ranges")
+
+        self._policy = KeySharedPolicy()
+        self._policy.set_key_shared_mode(key_shared_mode)
+        self._policy.set_allow_out_of_order_delivery(allow_out_of_order_delivery)
+
+        if sticky_ranges is not None:
+            self._policy.set_sticky_ranges(sticky_ranges)
+
+    @property
+    def key_shared_mode(self) -> KeySharedMode:
+        """
+        Returns the key shared mode
+        """
+        return self._policy.get_key_shared_mode()
+
+    @property
+    def allow_out_of_order_delivery(self) -> bool:
+        """
+        Returns whether out of order delivery is enabled
+        """
+        return self._policy.is_allow_out_of_order_delivery()
+
+    @property
+    def sticky_ranges(self) -> List[Tuple[int, int]]:
+        """
+        Returns the actual sticky ranges
+        """
+        return self._policy.get_sticky_ranges()
+
+    def policy(self):
+        """
+        Returns the actual KeySharedPolicy.
+        """
+        return self._policy
+
+class Reader:
+    """
+    Pulsar topic reader.
+    """
+
+    def topic(self):
+        """
+        Return the topic this reader is reading from.
+        """
+        return self._reader.topic()
+
+    def read_next(self, timeout_millis=None):
+        """
+        Read a single message.
+
+        If a message is not immediately available, this method will block until
+        a new message is available.
+
+        Parameters
+        ----------
+
+        timeout_millis: int, optional
+            If specified, the receiver will raise an exception if a message is not available within the timeout.
+        """
+        if timeout_millis is None:
+            msg = self._reader.read_next()
+        else:
+            _check_type(int, timeout_millis, 'timeout_millis')
+            msg = self._reader.read_next(timeout_millis)
+
+        m = Message()
+        m._message = msg
+        m._schema = self._schema
+        return m
+
+    def has_message_available(self):
+        """
+        Check if there is any message available to read from the current position.
+        """
+        return self._reader.has_message_available();
+
+    def seek(self, messageid):
+        """
+        Reset this reader to a specific message id or publish timestamp.
+        The message id can either be a specific message or represent the first or last messages in the topic.
+        Note: this operation can only be done on non-partitioned topics. For these, one can rather perform the
+        seek() on the individual partitions.
+
+        Parameters
+        ----------
+
+        messageid:
+            The message id for seek, OR an integer event time to seek to
+        """
+        self._reader.seek(messageid)
+
+    def close(self):
+        """
+        Close the reader.
+        """
+        self._reader.close()
+        self._client._consumers.remove(self)
+
+    def is_connected(self):
+        """
+        Check if the reader is connected or not.
+        """
+        return self._reader.is_connected()
+
+
+class ConsoleLogger:
+    """
+    Logger that writes on standard output
+
+    Attributes
+    ----------
+
+    log_level:
+        The logging level, eg: ``pulsar.LoggerLevel.Info``
+    """
+    def __init__(self, log_level=_pulsar.LoggerLevel.Info):
+        _check_type(_pulsar.LoggerLevel, log_level, 'log_level')
+        self.log_level = log_level
+
+
+class FileLogger:
+    """
+    Logger that writes into a file
+
+    Attributes
+    ----------
+
+    log_level:
+        The logging level, eg: ``pulsar.LoggerLevel.Info``
+    log_file:
+        The file where to write the logs
+    """
+    def __init__(self, log_level, log_file):
+        _check_type(_pulsar.LoggerLevel, log_level, 'log_level')
+        _check_type(str, log_file, 'log_file')
+        self.log_level = log_level
+        self.log_file = log_file
+
+
+def _check_type(var_type, var, name):
+    if not isinstance(var, var_type):
+        raise ValueError("Argument %s is expected to be of type '%s' and not '%s'"
+                         % (name, var_type.__name__, type(var).__name__))
+
+
+def _check_type_or_none(var_type, var, name):
+    if var is not None and not isinstance(var, var_type):
+        raise ValueError("Argument %s is expected to be either None or of type '%s'"
+                         % (name, var_type.__name__))
+
+
+def _listener_wrapper(listener, schema):
+    def wrapper(consumer, msg):
+        c = Consumer()
+        c._consumer = consumer
+        m = Message()
+        m._message = msg
+        m._schema = schema
+        listener(c, m)
+    return wrapper
```

## pulsar/exceptions.py

 * *Ordering differences only*

```diff
@@ -1,28 +1,28 @@
-#
-# Licensed to the Apache Software Foundation (ASF) under one
-# or more contributor license agreements.  See the NOTICE file
-# distributed with this work for additional information
-# regarding copyright ownership.  The ASF licenses this file
-# to you under the Apache License, Version 2.0 (the
-# "License"); you may not use this file except in compliance
-# with the License.  You may obtain a copy of the License at
-#
-#   http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing,
-# software distributed under the License is distributed on an
-# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
-# KIND, either express or implied.  See the License for the
-# specific language governing permissions and limitations
-# under the License.
-#
-
-from _pulsar import PulsarException, UnknownError, InvalidConfiguration, Timeout, LookupError, ConnectError, \
-    ReadError, AuthenticationError, AuthorizationError, ErrorGettingAuthenticationData, BrokerMetadataError, \
-    BrokerPersistenceError, ChecksumError, ConsumerBusy, NotConnected, AlreadyClosed, InvalidMessage, \
-    ConsumerNotInitialized, ProducerNotInitialized, ProducerBusy, TooManyLookupRequestException, InvalidTopicName, \
-    InvalidUrl, ServiceUnitNotReady, OperationNotSupported, ProducerBlockedQuotaExceededError, \
-    ProducerBlockedQuotaExceededException, ProducerQueueIsFull, MessageTooBig, TopicNotFound, SubscriptionNotFound, \
-    ConsumerNotFound, UnsupportedVersionError, TopicTerminated, CryptoError, IncompatibleSchema, ConsumerAssignError, \
-    CumulativeAcknowledgementNotAllowedError, TransactionCoordinatorNotFoundError, InvalidTxnStatusError, \
-    NotAllowedError, TransactionConflict, TransactionNotFound, ProducerFenced, MemoryBufferIsFull, Interrupted
+#
+# Licensed to the Apache Software Foundation (ASF) under one
+# or more contributor license agreements.  See the NOTICE file
+# distributed with this work for additional information
+# regarding copyright ownership.  The ASF licenses this file
+# to you under the Apache License, Version 2.0 (the
+# "License"); you may not use this file except in compliance
+# with the License.  You may obtain a copy of the License at
+#
+#   http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing,
+# software distributed under the License is distributed on an
+# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
+# KIND, either express or implied.  See the License for the
+# specific language governing permissions and limitations
+# under the License.
+#
+
+from _pulsar import PulsarException, UnknownError, InvalidConfiguration, Timeout, LookupError, ConnectError, \
+    ReadError, AuthenticationError, AuthorizationError, ErrorGettingAuthenticationData, BrokerMetadataError, \
+    BrokerPersistenceError, ChecksumError, ConsumerBusy, NotConnected, AlreadyClosed, InvalidMessage, \
+    ConsumerNotInitialized, ProducerNotInitialized, ProducerBusy, TooManyLookupRequestException, InvalidTopicName, \
+    InvalidUrl, ServiceUnitNotReady, OperationNotSupported, ProducerBlockedQuotaExceededError, \
+    ProducerBlockedQuotaExceededException, ProducerQueueIsFull, MessageTooBig, TopicNotFound, SubscriptionNotFound, \
+    ConsumerNotFound, UnsupportedVersionError, TopicTerminated, CryptoError, IncompatibleSchema, ConsumerAssignError, \
+    CumulativeAcknowledgementNotAllowedError, TransactionCoordinatorNotFoundError, InvalidTxnStatusError, \
+    NotAllowedError, TransactionConflict, TransactionNotFound, ProducerFenced, MemoryBufferIsFull, Interrupted
```

## pulsar/functions/__init__.py

 * *Ordering differences only*

```diff
@@ -1,20 +1,20 @@
-#
-# Licensed to the Apache Software Foundation (ASF) under one
-# or more contributor license agreements.  See the NOTICE file
-# distributed with this work for additional information
-# regarding copyright ownership.  The ASF licenses this file
-# to you under the Apache License, Version 2.0 (the
-# "License"); you may not use this file except in compliance
-# with the License.  You may obtain a copy of the License at
-#
-#   http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing,
-# software distributed under the License is distributed on an
-# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
-# KIND, either express or implied.  See the License for the
-# specific language governing permissions and limitations
-# under the License.
-#
-
-# -*- encoding: utf-8 -*-
+#
+# Licensed to the Apache Software Foundation (ASF) under one
+# or more contributor license agreements.  See the NOTICE file
+# distributed with this work for additional information
+# regarding copyright ownership.  The ASF licenses this file
+# to you under the Apache License, Version 2.0 (the
+# "License"); you may not use this file except in compliance
+# with the License.  You may obtain a copy of the License at
+#
+#   http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing,
+# software distributed under the License is distributed on an
+# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
+# KIND, either express or implied.  See the License for the
+# specific language governing permissions and limitations
+# under the License.
+#
+
+# -*- encoding: utf-8 -*-
```

## pulsar/functions/context.py

 * *Ordering differences only*

```diff
@@ -1,200 +1,200 @@
-#
-# Licensed to the Apache Software Foundation (ASF) under one
-# or more contributor license agreements.  See the NOTICE file
-# distributed with this work for additional information
-# regarding copyright ownership.  The ASF licenses this file
-# to you under the Apache License, Version 2.0 (the
-# "License"); you may not use this file except in compliance
-# with the License.  You may obtain a copy of the License at
-#
-#   http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing,
-# software distributed under the License is distributed on an
-# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
-# KIND, either express or implied.  See the License for the
-# specific language governing permissions and limitations
-# under the License.
-#
-
-# -*- encoding: utf-8 -*-
-
-# Licensed to the Apache Software Foundation (ASF) under one
-# or more contributor license agreements.  See the NOTICE file
-# distributed with this work for additional information
-# regarding copyright ownership.  The ASF licenses this file
-# to you under the Apache License, Version 2.0 (the
-# "License"); you may not use this file except in compliance
-# with the License.  You may obtain a copy of the License at
-#
-#   http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing,
-# software distributed under the License is distributed on an
-# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
-# KIND, either express or implied.  See the License for the
-# specific language governing permissions and limitations
-# under the License.
-#
-"""
-Context defines context information available during processing of a request.
-"""
-from abc import abstractmethod
-
-
-class Context(object):
-    """Interface defining information available at process time"""
-
-    @abstractmethod
-    def get_message_id(self):
-        """Return the messageid of the current message that we are processing"""
-        pass
-
-    @abstractmethod
-    def get_message_key(self):
-        """Return the key of the current message that we are processing"""
-        pass
-
-    @abstractmethod
-    def get_message_eventtime(self):
-        """Return the event time of the current message that we are processing"""
-        pass
-
-    @abstractmethod
-    def get_message_properties(self):
-        """Return the message properties kv map of the current message that we are processing"""
-        pass
-
-    @abstractmethod
-    def get_current_message_topic_name(self):
-        """Returns the topic name of the message that we are processing"""
-        pass
-
-    @abstractmethod
-    def get_function_tenant(self):
-        """Returns the tenant of the message that's being processed"""
-        pass
-
-    @abstractmethod
-    def get_function_namespace(self):
-        """Returns the namespace of the message that's being processed"""
-
-    @abstractmethod
-    def get_function_name(self):
-        """Returns the function name that we are a part of"""
-        pass
-
-    @abstractmethod
-    def get_function_id(self):
-        """Returns the function id that we are a part of"""
-        pass
-
-    @abstractmethod
-    def get_instance_id(self):
-        """Returns the instance id that is executing the function"""
-        pass
-
-    @abstractmethod
-    def get_function_version(self):
-        """Returns the version of function that we are executing"""
-        pass
-
-    @abstractmethod
-    def get_logger(self):
-        """Returns the logger object that can be used to do logging"""
-        pass
-
-    @abstractmethod
-    def get_user_config_value(self, key):
-        """Returns the value of the user-defined config. If the key doesn't exist, None is returned"""
-        pass
-
-    @abstractmethod
-    def get_user_config_map(self):
-        """Returns the entire user-defined config as a dict
-        (the dict will be empty if no user-defined config is supplied)"""
-        pass
-
-    @abstractmethod
-    def get_secret(self, secret_name):
-        """Returns the secret value associated with the name. None if nothing was found"""
-        pass
-
-    @abstractmethod
-    def get_partition_key(self):
-        """Returns partition key of the input message is one exists"""
-        pass
-
-    @abstractmethod
-    def get_ordering_key(self):
-        """Returns ordering key of the input message, if one exists"""
-        pass
-
-    @abstractmethod
-    def record_metric(self, metric_name, metric_value):
-        """Records the metric_value. metric_value has to satisfy isinstance(metric_value, numbers.Number)"""
-        pass
-
-    @abstractmethod
-    def publish(self, topic_name, message, serde_class_name="serde.IdentitySerDe", properties=None,
-                compression_type=None, callback=None, message_conf=None):
-        """Publishes message to topic_name by first serializing the message using serde_class_name serde
-        The message will have properties specified if any
-
-        The available options for message_conf:
-
-          properties,
-          partition_key,
-          ordering_key,
-          sequence_id,
-          replication_clusters,
-          disable_replication,
-          event_timestamp
-
-        """
-        pass
-
-    @abstractmethod
-    def get_input_topics(self):
-        """Returns the input topics of function"""
-        pass
-
-    @abstractmethod
-    def get_output_topic(self):
-        """Returns the output topic of function"""
-        pass
-
-    @abstractmethod
-    def get_output_serde_class_name(self):
-        """return output Serde class"""
-        pass
-
-    @abstractmethod
-    def ack(self, msgid, topic):
-        """ack this message id"""
-        pass
-
-    @abstractmethod
-    def incr_counter(self, key, amount):
-        """incr the counter of a given key in the managed state"""
-        pass
-
-    @abstractmethod
-    def get_counter(self, key):
-        """get the counter of a given key in the managed state"""
-        pass
-
-    @abstractmethod
-    def del_counter(self, key):
-        """delete the counter of a given key in the managed state"""
-        pass
-
-    @abstractmethod
-    def put_state(self, key, value):
-        """update the value of a given key in the managed state"""
-        pass
-
-    @abstractmethod
-    def get_state(self, key):
-        """get the value of a given key in the managed state"""
-        pass
+#
+# Licensed to the Apache Software Foundation (ASF) under one
+# or more contributor license agreements.  See the NOTICE file
+# distributed with this work for additional information
+# regarding copyright ownership.  The ASF licenses this file
+# to you under the Apache License, Version 2.0 (the
+# "License"); you may not use this file except in compliance
+# with the License.  You may obtain a copy of the License at
+#
+#   http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing,
+# software distributed under the License is distributed on an
+# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
+# KIND, either express or implied.  See the License for the
+# specific language governing permissions and limitations
+# under the License.
+#
+
+# -*- encoding: utf-8 -*-
+
+# Licensed to the Apache Software Foundation (ASF) under one
+# or more contributor license agreements.  See the NOTICE file
+# distributed with this work for additional information
+# regarding copyright ownership.  The ASF licenses this file
+# to you under the Apache License, Version 2.0 (the
+# "License"); you may not use this file except in compliance
+# with the License.  You may obtain a copy of the License at
+#
+#   http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing,
+# software distributed under the License is distributed on an
+# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
+# KIND, either express or implied.  See the License for the
+# specific language governing permissions and limitations
+# under the License.
+#
+"""
+Context defines context information available during processing of a request.
+"""
+from abc import abstractmethod
+
+
+class Context(object):
+    """Interface defining information available at process time"""
+
+    @abstractmethod
+    def get_message_id(self):
+        """Return the messageid of the current message that we are processing"""
+        pass
+
+    @abstractmethod
+    def get_message_key(self):
+        """Return the key of the current message that we are processing"""
+        pass
+
+    @abstractmethod
+    def get_message_eventtime(self):
+        """Return the event time of the current message that we are processing"""
+        pass
+
+    @abstractmethod
+    def get_message_properties(self):
+        """Return the message properties kv map of the current message that we are processing"""
+        pass
+
+    @abstractmethod
+    def get_current_message_topic_name(self):
+        """Returns the topic name of the message that we are processing"""
+        pass
+
+    @abstractmethod
+    def get_function_tenant(self):
+        """Returns the tenant of the message that's being processed"""
+        pass
+
+    @abstractmethod
+    def get_function_namespace(self):
+        """Returns the namespace of the message that's being processed"""
+
+    @abstractmethod
+    def get_function_name(self):
+        """Returns the function name that we are a part of"""
+        pass
+
+    @abstractmethod
+    def get_function_id(self):
+        """Returns the function id that we are a part of"""
+        pass
+
+    @abstractmethod
+    def get_instance_id(self):
+        """Returns the instance id that is executing the function"""
+        pass
+
+    @abstractmethod
+    def get_function_version(self):
+        """Returns the version of function that we are executing"""
+        pass
+
+    @abstractmethod
+    def get_logger(self):
+        """Returns the logger object that can be used to do logging"""
+        pass
+
+    @abstractmethod
+    def get_user_config_value(self, key):
+        """Returns the value of the user-defined config. If the key doesn't exist, None is returned"""
+        pass
+
+    @abstractmethod
+    def get_user_config_map(self):
+        """Returns the entire user-defined config as a dict
+        (the dict will be empty if no user-defined config is supplied)"""
+        pass
+
+    @abstractmethod
+    def get_secret(self, secret_name):
+        """Returns the secret value associated with the name. None if nothing was found"""
+        pass
+
+    @abstractmethod
+    def get_partition_key(self):
+        """Returns partition key of the input message is one exists"""
+        pass
+
+    @abstractmethod
+    def get_ordering_key(self):
+        """Returns ordering key of the input message, if one exists"""
+        pass
+
+    @abstractmethod
+    def record_metric(self, metric_name, metric_value):
+        """Records the metric_value. metric_value has to satisfy isinstance(metric_value, numbers.Number)"""
+        pass
+
+    @abstractmethod
+    def publish(self, topic_name, message, serde_class_name="serde.IdentitySerDe", properties=None,
+                compression_type=None, callback=None, message_conf=None):
+        """Publishes message to topic_name by first serializing the message using serde_class_name serde
+        The message will have properties specified if any
+
+        The available options for message_conf:
+
+          properties,
+          partition_key,
+          ordering_key,
+          sequence_id,
+          replication_clusters,
+          disable_replication,
+          event_timestamp
+
+        """
+        pass
+
+    @abstractmethod
+    def get_input_topics(self):
+        """Returns the input topics of function"""
+        pass
+
+    @abstractmethod
+    def get_output_topic(self):
+        """Returns the output topic of function"""
+        pass
+
+    @abstractmethod
+    def get_output_serde_class_name(self):
+        """return output Serde class"""
+        pass
+
+    @abstractmethod
+    def ack(self, msgid, topic):
+        """ack this message id"""
+        pass
+
+    @abstractmethod
+    def incr_counter(self, key, amount):
+        """incr the counter of a given key in the managed state"""
+        pass
+
+    @abstractmethod
+    def get_counter(self, key):
+        """get the counter of a given key in the managed state"""
+        pass
+
+    @abstractmethod
+    def del_counter(self, key):
+        """delete the counter of a given key in the managed state"""
+        pass
+
+    @abstractmethod
+    def put_state(self, key, value):
+        """update the value of a given key in the managed state"""
+        pass
+
+    @abstractmethod
+    def get_state(self, key):
+        """get the value of a given key in the managed state"""
+        pass
```

## pulsar/functions/function.py

 * *Ordering differences only*

```diff
@@ -1,55 +1,55 @@
-#
-# Licensed to the Apache Software Foundation (ASF) under one
-# or more contributor license agreements.  See the NOTICE file
-# distributed with this work for additional information
-# regarding copyright ownership.  The ASF licenses this file
-# to you under the Apache License, Version 2.0 (the
-# "License"); you may not use this file except in compliance
-# with the License.  You may obtain a copy of the License at
-#
-#   http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing,
-# software distributed under the License is distributed on an
-# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
-# KIND, either express or implied.  See the License for the
-# specific language governing permissions and limitations
-# under the License.
-#
-
-# -*- encoding: utf-8 -*-
-
-# Licensed to the Apache Software Foundation (ASF) under one
-# or more contributor license agreements.  See the NOTICE file
-# distributed with this work for additional information
-# regarding copyright ownership.  The ASF licenses this file
-# to you under the Apache License, Version 2.0 (the
-# "License"); you may not use this file except in compliance
-# with the License.  You may obtain a copy of the License at
-#
-#   http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing,
-# software distributed under the License is distributed on an
-# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
-# KIND, either express or implied.  See the License for the
-# specific language governing permissions and limitations
-# under the License.
-#
-"""
-This is the core interface of the function api.
-
-The process method is called for every message of the input topic of the
-function. The incoming input bytes are deserialized using the serde.
-The process function can optionally emit an output
-"""
-from abc import abstractmethod
-
-
-class Function(object):
-    """Interface for Pulsar Function"""
-
-    @abstractmethod
-    def process(self, input, context):
-        """Process input message"""
-        pass
+#
+# Licensed to the Apache Software Foundation (ASF) under one
+# or more contributor license agreements.  See the NOTICE file
+# distributed with this work for additional information
+# regarding copyright ownership.  The ASF licenses this file
+# to you under the Apache License, Version 2.0 (the
+# "License"); you may not use this file except in compliance
+# with the License.  You may obtain a copy of the License at
+#
+#   http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing,
+# software distributed under the License is distributed on an
+# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
+# KIND, either express or implied.  See the License for the
+# specific language governing permissions and limitations
+# under the License.
+#
+
+# -*- encoding: utf-8 -*-
+
+# Licensed to the Apache Software Foundation (ASF) under one
+# or more contributor license agreements.  See the NOTICE file
+# distributed with this work for additional information
+# regarding copyright ownership.  The ASF licenses this file
+# to you under the Apache License, Version 2.0 (the
+# "License"); you may not use this file except in compliance
+# with the License.  You may obtain a copy of the License at
+#
+#   http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing,
+# software distributed under the License is distributed on an
+# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
+# KIND, either express or implied.  See the License for the
+# specific language governing permissions and limitations
+# under the License.
+#
+"""
+This is the core interface of the function api.
+
+The process method is called for every message of the input topic of the
+function. The incoming input bytes are deserialized using the serde.
+The process function can optionally emit an output
+"""
+from abc import abstractmethod
+
+
+class Function(object):
+    """Interface for Pulsar Function"""
+
+    @abstractmethod
+    def process(self, input, context):
+        """Process input message"""
+        pass
```

## pulsar/functions/serde.py

 * *Ordering differences only*

```diff
@@ -1,94 +1,94 @@
-#
-# Licensed to the Apache Software Foundation (ASF) under one
-# or more contributor license agreements.  See the NOTICE file
-# distributed with this work for additional information
-# regarding copyright ownership.  The ASF licenses this file
-# to you under the Apache License, Version 2.0 (the
-# "License"); you may not use this file except in compliance
-# with the License.  You may obtain a copy of the License at
-#
-#   http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing,
-# software distributed under the License is distributed on an
-# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
-# KIND, either express or implied.  See the License for the
-# specific language governing permissions and limitations
-# under the License.
-#
-
-# -*- encoding: utf-8 -*-
-
-# Licensed to the Apache Software Foundation (ASF) under one
-# or more contributor license agreements.  See the NOTICE file
-# distributed with this work for additional information
-# regarding copyright ownership.  The ASF licenses this file
-# to you under the Apache License, Version 2.0 (the
-# "License"); you may not use this file except in compliance
-# with the License.  You may obtain a copy of the License at
-#
-#   http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing,
-# software distributed under the License is distributed on an
-# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
-# KIND, either express or implied.  See the License for the
-# specific language governing permissions and limitations
-# under the License.
-#
-"""
-SerDe defines the interface for serialization/deserialization.
-
-Everytime a message is read from pulsar topic, the serde is invoked to
-serialize the bytes into an object before invoking the process method.
-Anytime a python object needs to be written back to pulsar, it is
-serialized into bytes before writing.
-"""
-import pickle
-from abc import abstractmethod
-
-
-class SerDe(object):
-    """Interface for Serialization/Deserialization"""
-
-    @abstractmethod
-    def serialize(self, input):
-        """Serialize input message into bytes"""
-        pass
-
-    @abstractmethod
-    def deserialize(self, input_bytes):
-        """Serialize input_bytes into an object"""
-        pass
-
-
-class PickleSerDe(SerDe):
-    """Pickle based serializer"""
-
-    def serialize(self, input):
-        return pickle.dumps(input)
-
-    def deserialize(self, input_bytes):
-        return pickle.loads(input_bytes)
-
-
-class IdentitySerDe(SerDe):
-    """Simple Serde that just conversion to string and back"""
-
-    def __init__(self):
-        self._types = [int, float, complex, str]
-
-    def serialize(self, input):
-        if type(input) in self._types:
-            return str(input).encode('utf-8')
-        if type(input) == bytes:
-            return input
-        raise TypeError("IdentitySerde cannot serialize object of type %s" % type(input))
-
-    def deserialize(self, input_bytes):
-        for typ in self._types:
-            try:
-                return typ(input_bytes.decode('utf-8'))
-            except:
-                pass
-        return input_bytes
+#
+# Licensed to the Apache Software Foundation (ASF) under one
+# or more contributor license agreements.  See the NOTICE file
+# distributed with this work for additional information
+# regarding copyright ownership.  The ASF licenses this file
+# to you under the Apache License, Version 2.0 (the
+# "License"); you may not use this file except in compliance
+# with the License.  You may obtain a copy of the License at
+#
+#   http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing,
+# software distributed under the License is distributed on an
+# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
+# KIND, either express or implied.  See the License for the
+# specific language governing permissions and limitations
+# under the License.
+#
+
+# -*- encoding: utf-8 -*-
+
+# Licensed to the Apache Software Foundation (ASF) under one
+# or more contributor license agreements.  See the NOTICE file
+# distributed with this work for additional information
+# regarding copyright ownership.  The ASF licenses this file
+# to you under the Apache License, Version 2.0 (the
+# "License"); you may not use this file except in compliance
+# with the License.  You may obtain a copy of the License at
+#
+#   http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing,
+# software distributed under the License is distributed on an
+# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
+# KIND, either express or implied.  See the License for the
+# specific language governing permissions and limitations
+# under the License.
+#
+"""
+SerDe defines the interface for serialization/deserialization.
+
+Everytime a message is read from pulsar topic, the serde is invoked to
+serialize the bytes into an object before invoking the process method.
+Anytime a python object needs to be written back to pulsar, it is
+serialized into bytes before writing.
+"""
+import pickle
+from abc import abstractmethod
+
+
+class SerDe(object):
+    """Interface for Serialization/Deserialization"""
+
+    @abstractmethod
+    def serialize(self, input):
+        """Serialize input message into bytes"""
+        pass
+
+    @abstractmethod
+    def deserialize(self, input_bytes):
+        """Serialize input_bytes into an object"""
+        pass
+
+
+class PickleSerDe(SerDe):
+    """Pickle based serializer"""
+
+    def serialize(self, input):
+        return pickle.dumps(input)
+
+    def deserialize(self, input_bytes):
+        return pickle.loads(input_bytes)
+
+
+class IdentitySerDe(SerDe):
+    """Simple Serde that just conversion to string and back"""
+
+    def __init__(self):
+        self._types = [int, float, complex, str]
+
+    def serialize(self, input):
+        if type(input) in self._types:
+            return str(input).encode('utf-8')
+        if type(input) == bytes:
+            return input
+        raise TypeError("IdentitySerde cannot serialize object of type %s" % type(input))
+
+    def deserialize(self, input_bytes):
+        for typ in self._types:
+            try:
+                return typ(input_bytes.decode('utf-8'))
+            except:
+                pass
+        return input_bytes
```

## pulsar/schema/__init__.py

 * *Ordering differences only*

```diff
@@ -1,24 +1,24 @@
-#
-# Licensed to the Apache Software Foundation (ASF) under one
-# or more contributor license agreements.  See the NOTICE file
-# distributed with this work for additional information
-# regarding copyright ownership.  The ASF licenses this file
-# to you under the Apache License, Version 2.0 (the
-# "License"); you may not use this file except in compliance
-# with the License.  You may obtain a copy of the License at
-#
-#   http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing,
-# software distributed under the License is distributed on an
-# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
-# KIND, either express or implied.  See the License for the
-# specific language governing permissions and limitations
-# under the License.
-#
-
-from .definition import Record, Field, Null, Boolean, Integer, Long, \
-            Float, Double, Bytes, String, Array, Map, CustomEnum
-
-from .schema import Schema, BytesSchema, StringSchema, JsonSchema
-from .schema_avro import AvroSchema
+#
+# Licensed to the Apache Software Foundation (ASF) under one
+# or more contributor license agreements.  See the NOTICE file
+# distributed with this work for additional information
+# regarding copyright ownership.  The ASF licenses this file
+# to you under the Apache License, Version 2.0 (the
+# "License"); you may not use this file except in compliance
+# with the License.  You may obtain a copy of the License at
+#
+#   http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing,
+# software distributed under the License is distributed on an
+# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
+# KIND, either express or implied.  See the License for the
+# specific language governing permissions and limitations
+# under the License.
+#
+
+from .definition import Record, Field, Null, Boolean, Integer, Long, \
+            Float, Double, Bytes, String, Array, Map, CustomEnum
+
+from .schema import Schema, BytesSchema, StringSchema, JsonSchema
+from .schema_avro import AvroSchema
```

## pulsar/schema/definition.py

 * *Ordering differences only*

```diff
@@ -1,529 +1,529 @@
-#
-# Licensed to the Apache Software Foundation (ASF) under one
-# or more contributor license agreements.  See the NOTICE file
-# distributed with this work for additional information
-# regarding copyright ownership.  The ASF licenses this file
-# to you under the Apache License, Version 2.0 (the
-# "License"); you may not use this file except in compliance
-# with the License.  You may obtain a copy of the License at
-#
-#   http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing,
-# software distributed under the License is distributed on an
-# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
-# KIND, either express or implied.  See the License for the
-# specific language governing permissions and limitations
-# under the License.
-#
-
-import copy
-from abc import abstractmethod
-from collections import OrderedDict
-from enum import Enum, EnumMeta
-
-
-def _string_representation(x):
-    if hasattr(x, "__name__"):
-        return x.__name__
-    else:
-        return str(x)
-
-
-def _check_record_or_field(x):
-    if (type(x) is type and not issubclass(x, Record)) \
-            and not isinstance(x, Field):
-        raise Exception('Argument ' + _string_representation(x) + ' is not a Record or a Field')
-
-
-class RecordMeta(type):
-    def __new__(metacls, name, parents, dct):
-        if name != 'Record':
-            # Do not apply this logic to the base class itself
-            dct['_fields'] = RecordMeta._get_fields(dct)
-            dct['_required'] = False
-        return type.__new__(metacls, name, parents, dct)
-
-    @classmethod
-    def _get_fields(cls, dct):
-        # Build a set of valid fields for this record
-        fields = OrderedDict()
-        for name, value in dct.items():
-            if issubclass(type(value), EnumMeta):
-                value = CustomEnum(value)
-            elif type(value) == RecordMeta:
-                # We expect an instance of a record rather than the class itself
-                value = value()
-
-            if isinstance(value, Record) or isinstance(value, Field):
-                fields[name] = value
-        return fields
-
-
-class Record(metaclass=RecordMeta):
-
-    # This field is used to set namespace for Avro Record schema.
-    _avro_namespace = None
-
-    # Generate a schema where fields are sorted alphabetically
-    _sorted_fields = False
-
-    def __init__(self, default=None, required_default=False, required=False, *args, **kwargs):
-        self._required_default = required_default
-        self._default = default
-        self._required = required
-
-        for k, value in self._fields.items():
-            if k in kwargs:
-                if isinstance(value, Record) and isinstance(kwargs[k], dict):
-                    # Use dict init Record object
-                    copied = copy.copy(value)
-                    copied.__init__(**kwargs[k])
-                    self.__setattr__(k, copied)
-                elif isinstance(value, Array) and isinstance(kwargs[k], list) and len(kwargs[k]) > 0 \
-                        and isinstance(value.array_type, Record) and isinstance(kwargs[k][0], dict):
-                    arr = []
-                    for item in kwargs[k]:
-                        copied = copy.copy(value.array_type)
-                        copied.__init__(**item)
-                        arr.append(copied)
-                    self.__setattr__(k, arr)
-                elif isinstance(value, Map) and isinstance(kwargs[k], dict) and len(kwargs[k]) > 0 \
-                    and isinstance(value.value_type, Record) and isinstance(list(kwargs[k].values())[0], dict):
-                    dic = {}
-                    for mapKey, mapValue in kwargs[k].items():
-                        copied = copy.copy(value.value_type)
-                        copied.__init__(**mapValue)
-                        dic[mapKey] = copied
-                    self.__setattr__(k, dic)
-                else:
-                    # Value was overridden at constructor
-                    self.__setattr__(k, kwargs[k])
-            elif isinstance(value, Record):
-                # Value is a subrecord
-                self.__setattr__(k, value)
-            else:
-                # Set field to default value, without revalidating the default value type
-                super(Record, self).__setattr__(k, value.default())
-
-    @classmethod
-    def schema(cls):
-        return cls.schema_info(set())
-
-    @classmethod
-    def schema_info(cls, defined_names):
-        namespace_prefix = ''
-        if cls._avro_namespace is not None:
-            namespace_prefix = cls._avro_namespace + '.'
-        namespace_name = namespace_prefix + cls.__name__
-
-        if namespace_name in defined_names:
-            return namespace_name
-
-        defined_names.add(namespace_name)
-
-        schema = {
-            'type': 'record',
-            'name': str(cls.__name__)
-        }
-        if cls._avro_namespace is not None:
-            schema['namespace'] = cls._avro_namespace
-        schema['fields'] = []
-
-        def get_filed_default_value(value):
-            if isinstance(value, Enum):
-                return value.name
-            else:
-                return value
-
-        if cls._sorted_fields:
-            fields = sorted(cls._fields.keys())
-        else:
-            fields = cls._fields.keys()
-        for name in fields:
-            field = cls._fields[name]
-            field_type = field.schema_info(defined_names) \
-                if field._required else ['null', field.schema_info(defined_names)]
-            schema['fields'].append({
-                'name': name,
-                'default': get_filed_default_value(field.default()),
-                'type': field_type
-            }) if field.required_default() else schema['fields'].append({
-                'name': name,
-                'type': field_type,
-            })
-
-        return schema
-
-    def __setattr__(self, key, value):
-        if key == '_default':
-            super(Record, self).__setattr__(key, value)
-        elif key == '_required_default':
-            super(Record, self).__setattr__(key, value)
-        elif key == '_required':
-            super(Record, self).__setattr__(key, value)
-        else:
-            if key not in self._fields:
-                raise AttributeError('Cannot set undeclared field ' + key + ' on record')
-
-            # Check that type of value matches the field type
-            field = self._fields[key]
-            value = field.validate_type(key, value)
-            super(Record, self).__setattr__(key, value)
-
-    def __eq__(self, other):
-        for field in self._fields:
-            if self.__getattribute__(field) != other.__getattribute__(field):
-                return False
-        return True
-
-    def __ne__(self, other):
-        return not self.__eq__(other)
-
-    def __str__(self):
-        return str(self.__dict__)
-
-    def type(self):
-        return str(self.__class__.__name__)
-
-    def python_type(self):
-        return self.__class__
-
-    def validate_type(self, name, val):
-        if val is None and not self._required:
-            return self.default()
-
-        if not isinstance(val, self.__class__):
-            raise TypeError("Invalid type '%s' for sub-record field '%s'. Expected: %s" % (
-                type(val), name, _string_representation(self.__class__)))
-        return val
-
-    def default(self):
-        if self._default is not None:
-            return self._default
-        else:
-            return None
-
-    def required_default(self):
-        return self._required_default
-
-
-class Field(object):
-    def __init__(self, default=None, required=False, required_default=False):
-        if default is not None:
-            default = self.validate_type('default', default)
-        self._default = default
-        self._required_default = required_default
-        self._required = required
-
-    @abstractmethod
-    def type(self):
-        pass
-
-    @abstractmethod
-    def python_type(self):
-        pass
-
-    def validate_type(self, name, val):
-        if val is None and not self._required:
-            return self.default()
-
-        if not isinstance(val, self.python_type()):
-            raise TypeError("Invalid type '%s' for field '%s'. Expected: %s" % (type(val), name, _string_representation(self.python_type())))
-        return val
-
-    def schema(self):
-        # For primitive types, the schema would just be the type itself
-        return self.type()
-
-    def schema_info(self, defined_names):
-        return self.type()
-
-    def default(self):
-        return self._default
-
-    def required_default(self):
-        return self._required_default
-
-
-# All types
-
-
-class Null(Field):
-    def type(self):
-        return 'null'
-
-    def python_type(self):
-        return type(None)
-
-    def validate_type(self, name, val):
-        if val is not None:
-            raise TypeError('Field ' + name + ' is set to be None')
-        return val
-
-
-class Boolean(Field):
-    def type(self):
-        return 'boolean'
-
-    def python_type(self):
-        return bool
-
-    def default(self):
-        if self._default is not None:
-            return self._default
-        else:
-            return False
-
-
-class Integer(Field):
-    def type(self):
-        return 'int'
-
-    def python_type(self):
-        return int
-
-    def default(self):
-        if self._default is not None:
-            return self._default
-        else:
-            return None
-
-
-class Long(Field):
-    def type(self):
-        return 'long'
-
-    def python_type(self):
-        return int
-
-    def default(self):
-        if self._default is not None:
-            return self._default
-        else:
-            return None
-
-
-class Float(Field):
-    def type(self):
-        return 'float'
-
-    def python_type(self):
-        return float, int
-
-    def default(self):
-        if self._default is not None:
-            return self._default
-        else:
-            return None
-
-
-class Double(Field):
-    def type(self):
-        return 'double'
-
-    def python_type(self):
-        return float, int
-
-    def default(self):
-        if self._default is not None:
-            return self._default
-        else:
-            return None
-
-
-class Bytes(Field):
-    def type(self):
-        return 'bytes'
-
-    def python_type(self):
-        return bytes, str
-
-    def default(self):
-        if self._default is not None:
-            return self._default
-        else:
-            return None
-
-    def validate_type(self, name, val):
-        if isinstance(val, str):
-            return val.encode()
-        return val
-
-
-class String(Field):
-    def type(self):
-        return 'string'
-
-    def python_type(self):
-        return str, bytes
-
-    def validate_type(self, name, val):
-        t = type(val)
-
-        if val is None and not self._required:
-            return self.default()
-
-        if not (isinstance(val, (str, bytes)) or t.__name__ == 'unicode'):
-            raise TypeError("Invalid type '%s' for field '%s'. Expected a string" % (t, name))
-        if isinstance(val, bytes):
-            return val.decode()
-        return val
-
-    def default(self):
-        if self._default is not None:
-            return self._default
-        else:
-            return None
-
-# Complex types
-
-
-class CustomEnum(Field):
-    def __init__(self, enum_type, default=None, required=False, required_default=False):
-        if not issubclass(enum_type, Enum):
-            raise Exception(_string_representation(enum_type) + " is not a valid Enum type")
-        self.enum_type = enum_type
-        self.values = {}
-        for x in enum_type.__members__.values():
-            self.values[x.value] = x
-        super(CustomEnum, self).__init__(default, required, required_default)
-
-    def type(self):
-        return 'enum'
-
-    def python_type(self):
-        return self.enum_type
-
-    def validate_type(self, name, val):
-        if val is None:
-            return None
-
-        if type(val) is str:
-            # The enum was passed as a string, we need to check it against the possible values
-            if val in self.enum_type.__members__:
-                return self.enum_type.__members__[val]
-            else:
-                raise TypeError(
-                    "Invalid enum value '%s' for field '%s'. Expected: %s" % (val, name, self.enum_type.__members__.keys()))
-        elif type(val) is int:
-            # The enum was passed as an int, we need to check it against the possible values
-            if val in self.values:
-                return self.values[val]
-            else:
-                raise TypeError(
-                    "Invalid enum value '%s' for field '%s'. Expected: %s" % (val, name, self.values.keys()))
-        elif not isinstance(val, self.python_type()):
-            raise TypeError("Invalid type '%s' for field '%s'. Expected: %s" % (type(val), name, _string_representation(self.python_type())))
-        else:
-            return val
-
-    def schema(self):
-        return self.schema_info(set())
-
-    def schema_info(self, defined_names):
-        if self.enum_type.__name__ in defined_names:
-            return self.enum_type.__name__
-        defined_names.add(self.enum_type.__name__)
-        return {
-            'type': self.type(),
-            'name': self.enum_type.__name__,
-            'symbols': [x.name for x in self.enum_type]
-        }
-
-    def default(self):
-        if self._default is not None:
-            return self._default
-        else:
-            return None
-
-
-class Array(Field):
-    def __init__(self, array_type, default=None, required=False, required_default=False):
-        _check_record_or_field(array_type)
-        self.array_type = array_type
-        super(Array, self).__init__(default=default, required=required, required_default=required_default)
-
-    def type(self):
-        return 'array'
-
-    def python_type(self):
-        return list
-
-    def validate_type(self, name, val):
-        if val is None:
-            return None
-
-        super(Array, self).validate_type(name, val)
-
-        for x in val:
-            if not isinstance(x, self.array_type.python_type()):
-                raise TypeError('Array field ' + name + ' items should all be of type ' +
-                                _string_representation(self.array_type.type()))
-        return val
-
-    def schema(self):
-        return self.schema_info(set())
-
-    def schema_info(self, defined_names):
-        return {
-            'type': self.type(),
-            'items': self.array_type.schema_info(defined_names) if isinstance(self.array_type, (Array, Map, Record))
-                else self.array_type.type()
-        }
-
-    def default(self):
-        if self._default is not None:
-            return self._default
-        else:
-            return None
-
-
-class Map(Field):
-    def __init__(self, value_type, default=None, required=False, required_default=False):
-        _check_record_or_field(value_type)
-        self.value_type = value_type
-        super(Map, self).__init__(default=default, required=required, required_default=required_default)
-
-    def type(self):
-        return 'map'
-
-    def python_type(self):
-        return dict
-
-    def validate_type(self, name, val):
-        if val is None:
-            return None
-
-        super(Map, self).validate_type(name, val)
-
-        for k, v in val.items():
-            if type(k) != str and not is_unicode(k):
-                raise TypeError('Map keys for field ' + name + '  should all be strings')
-            if not isinstance(v, self.value_type.python_type()):
-                raise TypeError('Map values for field ' + name + ' should all be of type '
-                                + _string_representation(self.value_type.python_type()))
-
-        return val
-
-    def schema(self):
-        return self.schema_info(set())
-
-    def schema_info(self, defined_names):
-        return {
-            'type': self.type(),
-            'values': self.value_type.schema_info(defined_names) if isinstance(self.value_type, (Array, Map, Record))
-                else self.value_type.type()
-        }
-
-    def default(self):
-        if self._default is not None:
-            return self._default
-        else:
-            return None
-
-
-# Python3 has no `unicode` type, so here we use a tricky way to check if the type of `x` is `unicode` in Python2
-# and also make it work well with Python3.
-def is_unicode(x):
-    return 'encode' in dir(x) and type(x.encode()) == str
+#
+# Licensed to the Apache Software Foundation (ASF) under one
+# or more contributor license agreements.  See the NOTICE file
+# distributed with this work for additional information
+# regarding copyright ownership.  The ASF licenses this file
+# to you under the Apache License, Version 2.0 (the
+# "License"); you may not use this file except in compliance
+# with the License.  You may obtain a copy of the License at
+#
+#   http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing,
+# software distributed under the License is distributed on an
+# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
+# KIND, either express or implied.  See the License for the
+# specific language governing permissions and limitations
+# under the License.
+#
+
+import copy
+from abc import abstractmethod
+from collections import OrderedDict
+from enum import Enum, EnumMeta
+
+
+def _string_representation(x):
+    if hasattr(x, "__name__"):
+        return x.__name__
+    else:
+        return str(x)
+
+
+def _check_record_or_field(x):
+    if (type(x) is type and not issubclass(x, Record)) \
+            and not isinstance(x, Field):
+        raise Exception('Argument ' + _string_representation(x) + ' is not a Record or a Field')
+
+
+class RecordMeta(type):
+    def __new__(metacls, name, parents, dct):
+        if name != 'Record':
+            # Do not apply this logic to the base class itself
+            dct['_fields'] = RecordMeta._get_fields(dct)
+            dct['_required'] = False
+        return type.__new__(metacls, name, parents, dct)
+
+    @classmethod
+    def _get_fields(cls, dct):
+        # Build a set of valid fields for this record
+        fields = OrderedDict()
+        for name, value in dct.items():
+            if issubclass(type(value), EnumMeta):
+                value = CustomEnum(value)
+            elif type(value) == RecordMeta:
+                # We expect an instance of a record rather than the class itself
+                value = value()
+
+            if isinstance(value, Record) or isinstance(value, Field):
+                fields[name] = value
+        return fields
+
+
+class Record(metaclass=RecordMeta):
+
+    # This field is used to set namespace for Avro Record schema.
+    _avro_namespace = None
+
+    # Generate a schema where fields are sorted alphabetically
+    _sorted_fields = False
+
+    def __init__(self, default=None, required_default=False, required=False, *args, **kwargs):
+        self._required_default = required_default
+        self._default = default
+        self._required = required
+
+        for k, value in self._fields.items():
+            if k in kwargs:
+                if isinstance(value, Record) and isinstance(kwargs[k], dict):
+                    # Use dict init Record object
+                    copied = copy.copy(value)
+                    copied.__init__(**kwargs[k])
+                    self.__setattr__(k, copied)
+                elif isinstance(value, Array) and isinstance(kwargs[k], list) and len(kwargs[k]) > 0 \
+                        and isinstance(value.array_type, Record) and isinstance(kwargs[k][0], dict):
+                    arr = []
+                    for item in kwargs[k]:
+                        copied = copy.copy(value.array_type)
+                        copied.__init__(**item)
+                        arr.append(copied)
+                    self.__setattr__(k, arr)
+                elif isinstance(value, Map) and isinstance(kwargs[k], dict) and len(kwargs[k]) > 0 \
+                    and isinstance(value.value_type, Record) and isinstance(list(kwargs[k].values())[0], dict):
+                    dic = {}
+                    for mapKey, mapValue in kwargs[k].items():
+                        copied = copy.copy(value.value_type)
+                        copied.__init__(**mapValue)
+                        dic[mapKey] = copied
+                    self.__setattr__(k, dic)
+                else:
+                    # Value was overridden at constructor
+                    self.__setattr__(k, kwargs[k])
+            elif isinstance(value, Record):
+                # Value is a subrecord
+                self.__setattr__(k, value)
+            else:
+                # Set field to default value, without revalidating the default value type
+                super(Record, self).__setattr__(k, value.default())
+
+    @classmethod
+    def schema(cls):
+        return cls.schema_info(set())
+
+    @classmethod
+    def schema_info(cls, defined_names):
+        namespace_prefix = ''
+        if cls._avro_namespace is not None:
+            namespace_prefix = cls._avro_namespace + '.'
+        namespace_name = namespace_prefix + cls.__name__
+
+        if namespace_name in defined_names:
+            return namespace_name
+
+        defined_names.add(namespace_name)
+
+        schema = {
+            'type': 'record',
+            'name': str(cls.__name__)
+        }
+        if cls._avro_namespace is not None:
+            schema['namespace'] = cls._avro_namespace
+        schema['fields'] = []
+
+        def get_filed_default_value(value):
+            if isinstance(value, Enum):
+                return value.name
+            else:
+                return value
+
+        if cls._sorted_fields:
+            fields = sorted(cls._fields.keys())
+        else:
+            fields = cls._fields.keys()
+        for name in fields:
+            field = cls._fields[name]
+            field_type = field.schema_info(defined_names) \
+                if field._required else ['null', field.schema_info(defined_names)]
+            schema['fields'].append({
+                'name': name,
+                'default': get_filed_default_value(field.default()),
+                'type': field_type
+            }) if field.required_default() else schema['fields'].append({
+                'name': name,
+                'type': field_type,
+            })
+
+        return schema
+
+    def __setattr__(self, key, value):
+        if key == '_default':
+            super(Record, self).__setattr__(key, value)
+        elif key == '_required_default':
+            super(Record, self).__setattr__(key, value)
+        elif key == '_required':
+            super(Record, self).__setattr__(key, value)
+        else:
+            if key not in self._fields:
+                raise AttributeError('Cannot set undeclared field ' + key + ' on record')
+
+            # Check that type of value matches the field type
+            field = self._fields[key]
+            value = field.validate_type(key, value)
+            super(Record, self).__setattr__(key, value)
+
+    def __eq__(self, other):
+        for field in self._fields:
+            if self.__getattribute__(field) != other.__getattribute__(field):
+                return False
+        return True
+
+    def __ne__(self, other):
+        return not self.__eq__(other)
+
+    def __str__(self):
+        return str(self.__dict__)
+
+    def type(self):
+        return str(self.__class__.__name__)
+
+    def python_type(self):
+        return self.__class__
+
+    def validate_type(self, name, val):
+        if val is None and not self._required:
+            return self.default()
+
+        if not isinstance(val, self.__class__):
+            raise TypeError("Invalid type '%s' for sub-record field '%s'. Expected: %s" % (
+                type(val), name, _string_representation(self.__class__)))
+        return val
+
+    def default(self):
+        if self._default is not None:
+            return self._default
+        else:
+            return None
+
+    def required_default(self):
+        return self._required_default
+
+
+class Field(object):
+    def __init__(self, default=None, required=False, required_default=False):
+        if default is not None:
+            default = self.validate_type('default', default)
+        self._default = default
+        self._required_default = required_default
+        self._required = required
+
+    @abstractmethod
+    def type(self):
+        pass
+
+    @abstractmethod
+    def python_type(self):
+        pass
+
+    def validate_type(self, name, val):
+        if val is None and not self._required:
+            return self.default()
+
+        if not isinstance(val, self.python_type()):
+            raise TypeError("Invalid type '%s' for field '%s'. Expected: %s" % (type(val), name, _string_representation(self.python_type())))
+        return val
+
+    def schema(self):
+        # For primitive types, the schema would just be the type itself
+        return self.type()
+
+    def schema_info(self, defined_names):
+        return self.type()
+
+    def default(self):
+        return self._default
+
+    def required_default(self):
+        return self._required_default
+
+
+# All types
+
+
+class Null(Field):
+    def type(self):
+        return 'null'
+
+    def python_type(self):
+        return type(None)
+
+    def validate_type(self, name, val):
+        if val is not None:
+            raise TypeError('Field ' + name + ' is set to be None')
+        return val
+
+
+class Boolean(Field):
+    def type(self):
+        return 'boolean'
+
+    def python_type(self):
+        return bool
+
+    def default(self):
+        if self._default is not None:
+            return self._default
+        else:
+            return False
+
+
+class Integer(Field):
+    def type(self):
+        return 'int'
+
+    def python_type(self):
+        return int
+
+    def default(self):
+        if self._default is not None:
+            return self._default
+        else:
+            return None
+
+
+class Long(Field):
+    def type(self):
+        return 'long'
+
+    def python_type(self):
+        return int
+
+    def default(self):
+        if self._default is not None:
+            return self._default
+        else:
+            return None
+
+
+class Float(Field):
+    def type(self):
+        return 'float'
+
+    def python_type(self):
+        return float, int
+
+    def default(self):
+        if self._default is not None:
+            return self._default
+        else:
+            return None
+
+
+class Double(Field):
+    def type(self):
+        return 'double'
+
+    def python_type(self):
+        return float, int
+
+    def default(self):
+        if self._default is not None:
+            return self._default
+        else:
+            return None
+
+
+class Bytes(Field):
+    def type(self):
+        return 'bytes'
+
+    def python_type(self):
+        return bytes, str
+
+    def default(self):
+        if self._default is not None:
+            return self._default
+        else:
+            return None
+
+    def validate_type(self, name, val):
+        if isinstance(val, str):
+            return val.encode()
+        return val
+
+
+class String(Field):
+    def type(self):
+        return 'string'
+
+    def python_type(self):
+        return str, bytes
+
+    def validate_type(self, name, val):
+        t = type(val)
+
+        if val is None and not self._required:
+            return self.default()
+
+        if not (isinstance(val, (str, bytes)) or t.__name__ == 'unicode'):
+            raise TypeError("Invalid type '%s' for field '%s'. Expected a string" % (t, name))
+        if isinstance(val, bytes):
+            return val.decode()
+        return val
+
+    def default(self):
+        if self._default is not None:
+            return self._default
+        else:
+            return None
+
+# Complex types
+
+
+class CustomEnum(Field):
+    def __init__(self, enum_type, default=None, required=False, required_default=False):
+        if not issubclass(enum_type, Enum):
+            raise Exception(_string_representation(enum_type) + " is not a valid Enum type")
+        self.enum_type = enum_type
+        self.values = {}
+        for x in enum_type.__members__.values():
+            self.values[x.value] = x
+        super(CustomEnum, self).__init__(default, required, required_default)
+
+    def type(self):
+        return 'enum'
+
+    def python_type(self):
+        return self.enum_type
+
+    def validate_type(self, name, val):
+        if val is None:
+            return None
+
+        if type(val) is str:
+            # The enum was passed as a string, we need to check it against the possible values
+            if val in self.enum_type.__members__:
+                return self.enum_type.__members__[val]
+            else:
+                raise TypeError(
+                    "Invalid enum value '%s' for field '%s'. Expected: %s" % (val, name, self.enum_type.__members__.keys()))
+        elif type(val) is int:
+            # The enum was passed as an int, we need to check it against the possible values
+            if val in self.values:
+                return self.values[val]
+            else:
+                raise TypeError(
+                    "Invalid enum value '%s' for field '%s'. Expected: %s" % (val, name, self.values.keys()))
+        elif not isinstance(val, self.python_type()):
+            raise TypeError("Invalid type '%s' for field '%s'. Expected: %s" % (type(val), name, _string_representation(self.python_type())))
+        else:
+            return val
+
+    def schema(self):
+        return self.schema_info(set())
+
+    def schema_info(self, defined_names):
+        if self.enum_type.__name__ in defined_names:
+            return self.enum_type.__name__
+        defined_names.add(self.enum_type.__name__)
+        return {
+            'type': self.type(),
+            'name': self.enum_type.__name__,
+            'symbols': [x.name for x in self.enum_type]
+        }
+
+    def default(self):
+        if self._default is not None:
+            return self._default
+        else:
+            return None
+
+
+class Array(Field):
+    def __init__(self, array_type, default=None, required=False, required_default=False):
+        _check_record_or_field(array_type)
+        self.array_type = array_type
+        super(Array, self).__init__(default=default, required=required, required_default=required_default)
+
+    def type(self):
+        return 'array'
+
+    def python_type(self):
+        return list
+
+    def validate_type(self, name, val):
+        if val is None:
+            return None
+
+        super(Array, self).validate_type(name, val)
+
+        for x in val:
+            if not isinstance(x, self.array_type.python_type()):
+                raise TypeError('Array field ' + name + ' items should all be of type ' +
+                                _string_representation(self.array_type.type()))
+        return val
+
+    def schema(self):
+        return self.schema_info(set())
+
+    def schema_info(self, defined_names):
+        return {
+            'type': self.type(),
+            'items': self.array_type.schema_info(defined_names) if isinstance(self.array_type, (Array, Map, Record))
+                else self.array_type.type()
+        }
+
+    def default(self):
+        if self._default is not None:
+            return self._default
+        else:
+            return None
+
+
+class Map(Field):
+    def __init__(self, value_type, default=None, required=False, required_default=False):
+        _check_record_or_field(value_type)
+        self.value_type = value_type
+        super(Map, self).__init__(default=default, required=required, required_default=required_default)
+
+    def type(self):
+        return 'map'
+
+    def python_type(self):
+        return dict
+
+    def validate_type(self, name, val):
+        if val is None:
+            return None
+
+        super(Map, self).validate_type(name, val)
+
+        for k, v in val.items():
+            if type(k) != str and not is_unicode(k):
+                raise TypeError('Map keys for field ' + name + '  should all be strings')
+            if not isinstance(v, self.value_type.python_type()):
+                raise TypeError('Map values for field ' + name + ' should all be of type '
+                                + _string_representation(self.value_type.python_type()))
+
+        return val
+
+    def schema(self):
+        return self.schema_info(set())
+
+    def schema_info(self, defined_names):
+        return {
+            'type': self.type(),
+            'values': self.value_type.schema_info(defined_names) if isinstance(self.value_type, (Array, Map, Record))
+                else self.value_type.type()
+        }
+
+    def default(self):
+        if self._default is not None:
+            return self._default
+        else:
+            return None
+
+
+# Python3 has no `unicode` type, so here we use a tricky way to check if the type of `x` is `unicode` in Python2
+# and also make it work well with Python3.
+def is_unicode(x):
+    return 'encode' in dir(x) and type(x.encode()) == str
```

## pulsar/schema/schema.py

 * *Ordering differences only*

```diff
@@ -1,119 +1,119 @@
-#
-# Licensed to the Apache Software Foundation (ASF) under one
-# or more contributor license agreements.  See the NOTICE file
-# distributed with this work for additional information
-# regarding copyright ownership.  The ASF licenses this file
-# to you under the Apache License, Version 2.0 (the
-# "License"); you may not use this file except in compliance
-# with the License.  You may obtain a copy of the License at
-#
-#   http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing,
-# software distributed under the License is distributed on an
-# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
-# KIND, either express or implied.  See the License for the
-# specific language governing permissions and limitations
-# under the License.
-#
-
-
-from abc import abstractmethod
-import json
-import _pulsar
-import enum
-
-
-class Schema(object):
-    def __init__(self, record_cls, schema_type, schema_definition, schema_name):
-        self._record_cls = record_cls
-        self._schema_info = _pulsar.SchemaInfo(schema_type, schema_name,
-                                               json.dumps(schema_definition, indent=True))
-
-    @abstractmethod
-    def encode(self, obj):
-        pass
-
-    @abstractmethod
-    def decode(self, data):
-        pass
-
-    def decode_message(self, msg: _pulsar.Message):
-        return self.decode(msg.data())
-
-    def schema_info(self):
-        return self._schema_info
-
-    def attach_client(self, client: _pulsar.Client):
-        self._client = client
-
-    def _validate_object_type(self, obj):
-        if not isinstance(obj, self._record_cls):
-            raise TypeError('Invalid record obj of type ' + str(type(obj))
-                            + ' - expected type is ' + str(self._record_cls))
-
-
-class BytesSchema(Schema):
-    def __init__(self):
-        super(BytesSchema, self).__init__(bytes, _pulsar.SchemaType.BYTES, None, 'BYTES')
-
-    def encode(self, data):
-        self._validate_object_type(data)
-        return data
-
-    def decode(self, data):
-        return data
-
-    def __str__(self):
-        return 'BytesSchema'
-
-
-class StringSchema(Schema):
-    def __init__(self):
-        super(StringSchema, self).__init__(str, _pulsar.SchemaType.STRING, None, 'STRING')
-
-    def encode(self, obj):
-        self._validate_object_type(obj)
-        return obj.encode('utf-8')
-
-    def decode(self, data):
-        return data.decode('utf-8')
-
-    def __str__(self):
-        return 'StringSchema'
-
-
-def remove_reserved_key(data):
-    if '_default' in data:
-        del data['_default']
-    if '_required' in data:
-        del data['_required']
-    if '_required_default' in data:
-        del data['_required_default']
-
-
-class JsonSchema(Schema):
-
-    def __init__(self, record_cls):
-        super(JsonSchema, self).__init__(record_cls, _pulsar.SchemaType.JSON,
-                                         record_cls.schema(), 'JSON')
-
-    def _get_serialized_value(self, o):
-        if isinstance(o, enum.Enum):
-            return o.value
-        elif isinstance(o, bytes):
-            return o.decode()
-        else:
-            data = o.__dict__.copy()
-            remove_reserved_key(data)
-            return data
-
-    def encode(self, obj):
-        self._validate_object_type(obj)
-        # Copy the dict of the object as to not modify the provided object via the reference provided
-        data = obj.__dict__.copy()
-        remove_reserved_key(data)
-        return json.dumps(data, default=self._get_serialized_value, indent=True).encode('utf-8')
-
-    def decode(self, data):
-        return self._record_cls(**json.loads(data))
+#
+# Licensed to the Apache Software Foundation (ASF) under one
+# or more contributor license agreements.  See the NOTICE file
+# distributed with this work for additional information
+# regarding copyright ownership.  The ASF licenses this file
+# to you under the Apache License, Version 2.0 (the
+# "License"); you may not use this file except in compliance
+# with the License.  You may obtain a copy of the License at
+#
+#   http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing,
+# software distributed under the License is distributed on an
+# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
+# KIND, either express or implied.  See the License for the
+# specific language governing permissions and limitations
+# under the License.
+#
+
+
+from abc import abstractmethod
+import json
+import _pulsar
+import enum
+
+
+class Schema(object):
+    def __init__(self, record_cls, schema_type, schema_definition, schema_name):
+        self._record_cls = record_cls
+        self._schema_info = _pulsar.SchemaInfo(schema_type, schema_name,
+                                               json.dumps(schema_definition, indent=True))
+
+    @abstractmethod
+    def encode(self, obj):
+        pass
+
+    @abstractmethod
+    def decode(self, data):
+        pass
+
+    def decode_message(self, msg: _pulsar.Message):
+        return self.decode(msg.data())
+
+    def schema_info(self):
+        return self._schema_info
+
+    def attach_client(self, client: _pulsar.Client):
+        self._client = client
+
+    def _validate_object_type(self, obj):
+        if not isinstance(obj, self._record_cls):
+            raise TypeError('Invalid record obj of type ' + str(type(obj))
+                            + ' - expected type is ' + str(self._record_cls))
+
+
+class BytesSchema(Schema):
+    def __init__(self):
+        super(BytesSchema, self).__init__(bytes, _pulsar.SchemaType.BYTES, None, 'BYTES')
+
+    def encode(self, data):
+        self._validate_object_type(data)
+        return data
+
+    def decode(self, data):
+        return data
+
+    def __str__(self):
+        return 'BytesSchema'
+
+
+class StringSchema(Schema):
+    def __init__(self):
+        super(StringSchema, self).__init__(str, _pulsar.SchemaType.STRING, None, 'STRING')
+
+    def encode(self, obj):
+        self._validate_object_type(obj)
+        return obj.encode('utf-8')
+
+    def decode(self, data):
+        return data.decode('utf-8')
+
+    def __str__(self):
+        return 'StringSchema'
+
+
+def remove_reserved_key(data):
+    if '_default' in data:
+        del data['_default']
+    if '_required' in data:
+        del data['_required']
+    if '_required_default' in data:
+        del data['_required_default']
+
+
+class JsonSchema(Schema):
+
+    def __init__(self, record_cls):
+        super(JsonSchema, self).__init__(record_cls, _pulsar.SchemaType.JSON,
+                                         record_cls.schema(), 'JSON')
+
+    def _get_serialized_value(self, o):
+        if isinstance(o, enum.Enum):
+            return o.value
+        elif isinstance(o, bytes):
+            return o.decode()
+        else:
+            data = o.__dict__.copy()
+            remove_reserved_key(data)
+            return data
+
+    def encode(self, obj):
+        self._validate_object_type(obj)
+        # Copy the dict of the object as to not modify the provided object via the reference provided
+        data = obj.__dict__.copy()
+        remove_reserved_key(data)
+        return json.dumps(data, default=self._get_serialized_value, indent=True).encode('utf-8')
+
+    def decode(self, data):
+        return self._record_cls(**json.loads(data))
```

## pulsar/schema/schema_avro.py

```diff
@@ -1,139 +1,140 @@
-#
-# Licensed to the Apache Software Foundation (ASF) under one
-# or more contributor license agreements.  See the NOTICE file
-# distributed with this work for additional information
-# regarding copyright ownership.  The ASF licenses this file
-# to you under the Apache License, Version 2.0 (the
-# "License"); you may not use this file except in compliance
-# with the License.  You may obtain a copy of the License at
-#
-#   http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing,
-# software distributed under the License is distributed on an
-# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
-# KIND, either express or implied.  See the License for the
-# specific language governing permissions and limitations
-# under the License.
-#
-
-import _pulsar
-import io
-import json
-import logging
-import enum
-
-from . import Record
-from .schema import Schema
-
-try:
-    import fastavro
-    HAS_AVRO = True
-except ImportError:
-    HAS_AVRO = False
-
-if HAS_AVRO:
-    class AvroSchema(Schema):
-        def __init__(self, record_cls, schema_definition=None):
-            if record_cls is None and schema_definition is None:
-                raise AssertionError("The param record_cls and schema_definition shouldn't be both None.")
-
-            if record_cls is not None:
-                self._schema = record_cls.schema()
-            else:
-                self._schema = schema_definition
-            self._writer_schemas = dict()
-            self._logger = logging.getLogger()
-            super(AvroSchema, self).__init__(record_cls, _pulsar.SchemaType.AVRO, self._schema, 'AVRO')
-
-        def _get_serialized_value(self, x):
-            if isinstance(x, enum.Enum):
-                return x.name
-            elif isinstance(x, Record):
-                return self.encode_dict(x.__dict__)
-            elif isinstance(x, list):
-                arr = []
-                for item in x:
-                    arr.append(self._get_serialized_value(item))
-                return arr
-            elif isinstance(x, dict):
-                return self.encode_dict(x)
-            else:
-                return x
-
-        def encode(self, obj):
-            buffer = io.BytesIO()
-            m = obj
-            if self._record_cls is not None:
-                self._validate_object_type(obj)
-                m = self.encode_dict(obj.__dict__)
-            elif not isinstance(obj, dict):
-                raise ValueError('If using the custom schema, the record data should be dict type.')
-
-            fastavro.schemaless_writer(buffer, self._schema, m)
-            return buffer.getvalue()
-
-        def encode_dict(self, d):
-            obj = {}
-            for k, v in d.items():
-                obj[k] = self._get_serialized_value(v)
-            return obj
-
-        def decode(self, data):
-            return self._decode_bytes(data, self._schema)
-
-        def decode_message(self, msg: _pulsar.Message):
-            if self._client is None:
-                return self.decode(msg.data())
-            topic = msg.topic_name()
-            version = msg.int_schema_version()
-            try:
-                writer_schema = self._get_writer_schema(topic, version)
-                return self._decode_bytes(msg.data(), writer_schema)
-            except Exception as e:
-                self._logger.error(f'Failed to get schema info of {topic} version {version}: {e}')
-                return self._decode_bytes(msg.data(), self._schema)
-
-        def _get_writer_schema(self, topic: str, version: int) -> 'dict':
-            if self._writer_schemas.get(topic) is None:
-                self._writer_schemas[topic] = dict()
-            writer_schema = self._writer_schemas[topic].get(version)
-            if writer_schema is not None:
-                return writer_schema
-            if self._client is None:
-                return self._schema
-
-            self._logger.info('Downloading schema of %s version %d...', topic, version)
-            info = self._client.get_schema_info(topic, version)
-            self._logger.info('Downloaded schema of %s version %d', topic, version)
-            if info.schema_type() != _pulsar.SchemaType.AVRO:
-                raise RuntimeError(f'The schema type of topic "{topic}" and version {version}'
-                                   f' is {info.schema_type()}')
-            writer_schema = json.loads(info.schema())
-            self._writer_schemas[topic][version] = writer_schema
-            return writer_schema
-
-        def _decode_bytes(self, data: bytes, writer_schema: dict):
-            buffer = io.BytesIO(data)
-            # If the record names are different between the writer schema and the reader schema,
-            # schemaless_reader will fail with fastavro._read_common.SchemaResolutionError.
-            # So we make the record name fields consistent here.
-            reader_schema: dict = self._schema
-            writer_schema['name'] = reader_schema['name']
-            d = fastavro.schemaless_reader(buffer, writer_schema, reader_schema)
-            if self._record_cls is not None:
-                return self._record_cls(**d)
-            else:
-                return d
-
-else:
-    class AvroSchema(Schema):
-        def __init__(self, _record_cls, _schema_definition=None):
-            raise Exception("Avro library support was not found. Make sure to install Pulsar client " +
-                            "with Avro support: pip3 install 'pulsar-client[avro]'")
-
-        def encode(self, obj):
-            pass
-
-        def decode(self, data):
-            pass
+#
+# Licensed to the Apache Software Foundation (ASF) under one
+# or more contributor license agreements.  See the NOTICE file
+# distributed with this work for additional information
+# regarding copyright ownership.  The ASF licenses this file
+# to you under the Apache License, Version 2.0 (the
+# "License"); you may not use this file except in compliance
+# with the License.  You may obtain a copy of the License at
+#
+#   http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing,
+# software distributed under the License is distributed on an
+# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
+# KIND, either express or implied.  See the License for the
+# specific language governing permissions and limitations
+# under the License.
+#
+
+import _pulsar
+import io
+import json
+import logging
+import enum
+
+from . import Record
+from .schema import Schema
+
+try:
+    import fastavro
+    HAS_AVRO = True
+except ImportError:
+    HAS_AVRO = False
+
+if HAS_AVRO:
+    class AvroSchema(Schema):
+        def __init__(self, record_cls, schema_definition=None):
+            if record_cls is None and schema_definition is None:
+                raise AssertionError("The param record_cls and schema_definition shouldn't be both None.")
+
+            if record_cls is not None:
+                self._schema = record_cls.schema()
+            else:
+                self._schema = schema_definition
+            self._writer_schemas = dict()
+            self._logger = logging.getLogger()
+            super(AvroSchema, self).__init__(record_cls, _pulsar.SchemaType.AVRO, self._schema, 'AVRO')
+
+        def _get_serialized_value(self, x):
+            if isinstance(x, enum.Enum):
+                return x.name
+            elif isinstance(x, Record):
+                return self.encode_dict(x.__dict__)
+            elif isinstance(x, list):
+                arr = []
+                for item in x:
+                    arr.append(self._get_serialized_value(item))
+                return arr
+            elif isinstance(x, dict):
+                return self.encode_dict(x)
+            else:
+                return x
+
+        def encode(self, obj):
+            buffer = io.BytesIO()
+            m = obj
+            if self._record_cls is not None:
+                self._validate_object_type(obj)
+                m = self.encode_dict(obj.__dict__)
+            elif not isinstance(obj, dict):
+                raise ValueError('If using the custom schema, the record data should be dict type.')
+
+            fastavro.schemaless_writer(buffer, self._schema, m)
+            return buffer.getvalue()
+
+        def encode_dict(self, d):
+            obj = {}
+            for k, v in d.items():
+                obj[k] = self._get_serialized_value(v)
+            return obj
+
+        def decode(self, data):
+            return self._decode_bytes(data, self._schema)
+
+        def decode_message(self, msg: _pulsar.Message):
+            if self._client is None:
+                return self.decode(msg.data())
+            topic = msg.topic_name()
+            version = msg.int_schema_version()
+            try:
+                writer_schema = self._get_writer_schema(topic, version)
+                return self._decode_bytes(msg.data(), writer_schema)
+            except Exception as e:
+                msg_id = msg.message_id()
+                self._logger.warn(f'Failed to decode {msg_id} with schema {topic} version {version}: {e}')
+                return self._decode_bytes(msg.data(), self._schema)
+
+        def _get_writer_schema(self, topic: str, version: int) -> 'dict':
+            if self._writer_schemas.get(topic) is None:
+                self._writer_schemas[topic] = dict()
+            writer_schema = self._writer_schemas[topic].get(version)
+            if writer_schema is not None:
+                return writer_schema
+            if self._client is None:
+                return self._schema
+
+            self._logger.info('Downloading schema of %s version %d...', topic, version)
+            info = self._client.get_schema_info(topic, version)
+            self._logger.info('Downloaded schema of %s version %d', topic, version)
+            if info.schema_type() != _pulsar.SchemaType.AVRO:
+                raise RuntimeError(f'The schema type of topic "{topic}" and version {version}'
+                                   f' is {info.schema_type()}')
+            writer_schema = json.loads(info.schema())
+            self._writer_schemas[topic][version] = writer_schema
+            return writer_schema
+
+        def _decode_bytes(self, data: bytes, writer_schema: dict):
+            buffer = io.BytesIO(data)
+            # If the record names are different between the writer schema and the reader schema,
+            # schemaless_reader will fail with fastavro._read_common.SchemaResolutionError.
+            # So we make the record name fields consistent here.
+            reader_schema: dict = self._schema
+            writer_schema['name'] = reader_schema['name']
+            d = fastavro.schemaless_reader(buffer, writer_schema, reader_schema)
+            if self._record_cls is not None:
+                return self._record_cls(**d)
+            else:
+                return d
+
+else:
+    class AvroSchema(Schema):
+        def __init__(self, _record_cls, _schema_definition=None):
+            raise Exception("Avro library support was not found. Make sure to install Pulsar client " +
+                            "with Avro support: pip3 install 'pulsar-client[avro]'")
+
+        def encode(self, obj):
+            pass
+
+        def decode(self, data):
+            pass
```

## Comparing `pulsar_client-3.4.0.dist-info/LICENSE` & `pulsar_client-3.5.0.dist-info/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,202 +1,202 @@
-
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

## Comparing `pulsar_client-3.4.0.dist-info/METADATA` & `pulsar_client-3.5.0.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,27 @@
-Metadata-Version: 2.1
-Name: pulsar-client
-Version: 3.4.0
-Summary: Apache Pulsar Python client library
-Home-page: https://pulsar.apache.org/
-Author: Pulsar Devs
-Author-email: dev@pulsar.apache.org
-License: Apache License v2.0
-Platform: UNKNOWN
-License-File: LICENSE
-License-File: NOTICE
-Requires-Dist: certifi
-Provides-Extra: all
-Requires-Dist: apache-bookkeeper-client >=4.16.1 ; extra == 'all'
-Requires-Dist: fastavro >=1.9.2 ; extra == 'all'
-Requires-Dist: grpcio >=1.60.0 ; extra == 'all'
-Requires-Dist: prometheus-client ; extra == 'all'
-Requires-Dist: protobuf <=3.20.3,>=3.6.1 ; extra == 'all'
-Requires-Dist: ratelimit ; extra == 'all'
-Provides-Extra: avro
-Requires-Dist: fastavro >=1.9.2 ; extra == 'avro'
-Provides-Extra: functions
-Requires-Dist: apache-bookkeeper-client >=4.16.1 ; extra == 'functions'
-Requires-Dist: grpcio >=1.60.0 ; extra == 'functions'
-Requires-Dist: prometheus-client ; extra == 'functions'
-Requires-Dist: protobuf <=3.20.3,>=3.6.1 ; extra == 'functions'
-Requires-Dist: ratelimit ; extra == 'functions'
-
-UNKNOWN
-
+Metadata-Version: 2.1
+Name: pulsar-client
+Version: 3.5.0
+Summary: Apache Pulsar Python client library
+Home-page: https://pulsar.apache.org/
+Author: Pulsar Devs
+Author-email: dev@pulsar.apache.org
+License: Apache License v2.0
+License-File: LICENSE
+License-File: NOTICE
+Requires-Dist: certifi
+Provides-Extra: all
+Requires-Dist: apache-bookkeeper-client >=4.16.1 ; extra == 'all'
+Requires-Dist: fastavro >=1.9.2 ; extra == 'all'
+Requires-Dist: grpcio >=1.60.0 ; extra == 'all'
+Requires-Dist: prometheus-client ; extra == 'all'
+Requires-Dist: protobuf <=3.20.3,>=3.6.1 ; extra == 'all'
+Requires-Dist: ratelimit ; extra == 'all'
+Provides-Extra: avro
+Requires-Dist: fastavro >=1.9.2 ; extra == 'avro'
+Provides-Extra: functions
+Requires-Dist: apache-bookkeeper-client >=4.16.1 ; extra == 'functions'
+Requires-Dist: grpcio >=1.60.0 ; extra == 'functions'
+Requires-Dist: prometheus-client ; extra == 'functions'
+Requires-Dist: protobuf <=3.20.3,>=3.6.1 ; extra == 'functions'
+Requires-Dist: ratelimit ; extra == 'functions'
+
```

