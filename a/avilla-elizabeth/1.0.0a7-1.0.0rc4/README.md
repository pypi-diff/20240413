# Comparing `tmp/avilla_elizabeth-1.0.0a7.tar.gz` & `tmp/avilla-elizabeth-1.0.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avilla_elizabeth-1.0.0a7.tar", last modified: Sat Sep  2 13:53:44 2023, max compression
+gzip compressed data, was "avilla-elizabeth-1.0.0rc4.tar", last modified: Wed Aug 31 04:41:00 2022, max compression
```

## Comparing `avilla_elizabeth-1.0.0a7.tar` & `avilla-elizabeth-1.0.0rc4.tar`

### file list

```diff
@@ -1,45 +1,23 @@
--rw-r--r--   0        0        0      525 2023-09-02 13:53:28.220868 avilla_elizabeth-1.0.0a7/.mina/elizabeth.toml
--rw-r--r--   0        0        0     1070 2023-09-02 13:53:28.224868 avilla_elizabeth-1.0.0a7/LICENSE
--rw-r--r--   0        0        0     8360 2023-09-02 13:53:28.224868 avilla_elizabeth-1.0.0a7/README.md
--rw-r--r--   0        0        0      118 2023-09-02 13:53:28.224868 avilla_elizabeth-1.0.0a7/avilla/elizabeth/__init__.py
--rw-r--r--   0        0        0      598 2023-09-02 13:53:28.224868 avilla_elizabeth-1.0.0a7/avilla/elizabeth/account.py
--rw-r--r--   0        0        0        0 2023-09-02 13:53:28.224868 avilla_elizabeth-1.0.0a7/avilla/elizabeth/collector/__init__.py
--rw-r--r--   0        0        0      948 2023-09-02 13:53:28.224868 avilla_elizabeth-1.0.0a7/avilla/elizabeth/collector/connection.py
--rw-r--r--   0        0        0        0 2023-09-02 13:53:28.224868 avilla_elizabeth-1.0.0a7/avilla/elizabeth/connection/__init__.py
--rw-r--r--   0        0        0     3941 2023-09-02 13:53:28.224868 avilla_elizabeth-1.0.0a7/avilla/elizabeth/connection/base.py
--rw-r--r--   0        0        0     2219 2023-09-02 13:53:28.224868 avilla_elizabeth-1.0.0a7/avilla/elizabeth/connection/util.py
--rw-r--r--   0        0        0     7807 2023-09-02 13:53:28.224868 avilla_elizabeth-1.0.0a7/avilla/elizabeth/connection/ws_client.py
--rw-r--r--   0        0        0      663 2023-09-02 13:53:28.224868 avilla_elizabeth-1.0.0a7/avilla/elizabeth/const.py
--rw-r--r--   0        0        0      898 2023-09-02 13:53:28.224868 avilla_elizabeth-1.0.0a7/avilla/elizabeth/exception.py
--rw-r--r--   0        0        0        0 2023-09-02 13:53:28.224868 avilla_elizabeth-1.0.0a7/avilla/elizabeth/perform/__init__.py
--rw-r--r--   0        0        0        0 2023-09-02 13:53:28.224868 avilla_elizabeth-1.0.0a7/avilla/elizabeth/perform/action/__init__.py
--rw-r--r--   0        0        0     1301 2023-09-02 13:53:28.224868 avilla_elizabeth-1.0.0a7/avilla/elizabeth/perform/action/activity.py
--rw-r--r--   0        0        0     4372 2023-09-02 13:53:28.224868 avilla_elizabeth-1.0.0a7/avilla/elizabeth/perform/action/announcement.py
--rw-r--r--   0        0        0     1242 2023-09-02 13:53:28.224868 avilla_elizabeth-1.0.0a7/avilla/elizabeth/perform/action/contact.py
--rw-r--r--   0        0        0     2351 2023-09-02 13:53:28.224868 avilla_elizabeth-1.0.0a7/avilla/elizabeth/perform/action/friend.py
--rw-r--r--   0        0        0     3863 2023-09-02 13:53:28.224868 avilla_elizabeth-1.0.0a7/avilla/elizabeth/perform/action/group.py
--rw-r--r--   0        0        0    12131 2023-09-02 13:53:28.224868 avilla_elizabeth-1.0.0a7/avilla/elizabeth/perform/action/group_member.py
--rw-r--r--   0        0        0     4638 2023-09-02 13:53:28.224868 avilla_elizabeth-1.0.0a7/avilla/elizabeth/perform/action/message.py
--rw-r--r--   0        0        0     4577 2023-09-02 13:53:28.224868 avilla_elizabeth-1.0.0a7/avilla/elizabeth/perform/action/request.py
--rw-r--r--   0        0        0     1572 2023-09-02 13:53:28.224868 avilla_elizabeth-1.0.0a7/avilla/elizabeth/perform/context.py
--rw-r--r--   0        0        0       99 2023-09-02 13:53:28.224868 avilla_elizabeth-1.0.0a7/avilla/elizabeth/perform/event/__init__.py
--rw-r--r--   0        0        0     1632 2023-09-02 13:53:28.224868 avilla_elizabeth-1.0.0a7/avilla/elizabeth/perform/event/activity.py
--rw-r--r--   0        0        0     2722 2023-09-02 13:53:28.224868 avilla_elizabeth-1.0.0a7/avilla/elizabeth/perform/event/friend.py
--rw-r--r--   0        0        0    13990 2023-09-02 13:53:28.224868 avilla_elizabeth-1.0.0a7/avilla/elizabeth/perform/event/group.py
--rw-r--r--   0        0        0    17690 2023-09-02 13:53:28.224868 avilla_elizabeth-1.0.0a7/avilla/elizabeth/perform/event/group_member.py
--rw-r--r--   0        0        0     7675 2023-09-02 13:53:28.224868 avilla_elizabeth-1.0.0a7/avilla/elizabeth/perform/event/message.py
--rw-r--r--   0        0        0    13972 2023-09-02 13:53:28.224868 avilla_elizabeth-1.0.0a7/avilla/elizabeth/perform/event/relationship.py
--rw-r--r--   0        0        0     3258 2023-09-02 13:53:28.228869 avilla_elizabeth-1.0.0a7/avilla/elizabeth/perform/event/request.py
--rw-r--r--   0        0        0     5586 2023-09-02 13:53:28.228869 avilla_elizabeth-1.0.0a7/avilla/elizabeth/perform/message/deserialize.py
--rw-r--r--   0        0        0     4815 2023-09-02 13:53:28.228869 avilla_elizabeth-1.0.0a7/avilla/elizabeth/perform/message/serialize.py
--rw-r--r--   0        0        0        0 2023-09-02 13:53:28.228869 avilla_elizabeth-1.0.0a7/avilla/elizabeth/perform/query/__init__.py
--rw-r--r--   0        0        0     1586 2023-09-02 13:53:28.228869 avilla_elizabeth-1.0.0a7/avilla/elizabeth/perform/query/announcement.py
--rw-r--r--   0        0        0     1057 2023-09-02 13:53:28.228869 avilla_elizabeth-1.0.0a7/avilla/elizabeth/perform/query/bot.py
--rw-r--r--   0        0        0     1394 2023-09-02 13:53:28.228869 avilla_elizabeth-1.0.0a7/avilla/elizabeth/perform/query/friend.py
--rw-r--r--   0        0        0     2396 2023-09-02 13:53:28.228869 avilla_elizabeth-1.0.0a7/avilla/elizabeth/perform/query/group.py
--rw-r--r--   0        0        0     1042 2023-09-02 13:53:28.228869 avilla_elizabeth-1.0.0a7/avilla/elizabeth/perform/resource_fetch.py
--rw-r--r--   0        0        0     3229 2023-09-02 13:53:28.228869 avilla_elizabeth-1.0.0a7/avilla/elizabeth/protocol.py
--rw-r--r--   0        0        0      930 2023-09-02 13:53:28.228869 avilla_elizabeth-1.0.0a7/avilla/elizabeth/resource.py
--rw-r--r--   0        0        0     1493 2023-09-02 13:53:28.228869 avilla_elizabeth-1.0.0a7/avilla/elizabeth/service.py
--rw-r--r--   0        0        0      956 2023-09-02 13:53:44.404952 avilla_elizabeth-1.0.0a7/pyproject.toml
--rw-r--r--   0        0        0     8755 1970-01-01 00:00:00.000000 avilla_elizabeth-1.0.0a7/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2022-08-31 04:32:04.327287 avilla-elizabeth-1.0.0rc4/avilla/elizabeth/__init__.py
+-rw-rw-rw-   0        0        0     1474 2022-08-31 04:32:04.328263 avilla-elizabeth-1.0.0rc4/avilla/elizabeth/_query.py
+-rw-rw-rw-   0        0        0     2164 2022-08-31 04:32:04.330401 avilla-elizabeth-1.0.0rc4/avilla/elizabeth/account.py
+-rw-rw-rw-   0        0        0     4206 2022-08-31 04:32:04.331330 avilla-elizabeth-1.0.0rc4/avilla/elizabeth/connection/__init__.py
+-rw-rw-rw-   0        0        0     2481 2022-08-31 04:32:04.333136 avilla-elizabeth-1.0.0rc4/avilla/elizabeth/connection/config.py
+-rw-rw-rw-   0        0        0     6231 2022-08-31 04:32:04.336566 avilla-elizabeth-1.0.0rc4/avilla/elizabeth/connection/http.py
+-rw-rw-rw-   0        0        0     2934 2022-08-31 04:32:04.337964 avilla-elizabeth-1.0.0rc4/avilla/elizabeth/connection/util.py
+-rw-rw-rw-   0        0        0     6998 2022-08-31 04:32:04.339974 avilla-elizabeth-1.0.0rc4/avilla/elizabeth/connection/ws.py
+-rw-rw-rw-   0        0        0      175 2022-08-31 04:32:04.341001 avilla-elizabeth-1.0.0rc4/avilla/elizabeth/element.py
+-rw-rw-rw-   0        0        0     5247 2022-08-31 04:32:04.342904 avilla-elizabeth-1.0.0rc4/avilla/elizabeth/event_parser.py
+-rw-rw-rw-   0        0        0      898 2022-08-31 04:32:04.343937 avilla-elizabeth-1.0.0rc4/avilla/elizabeth/exception.py
+-rw-rw-rw-   0        0        0     1208 2022-08-31 04:32:04.345888 avilla-elizabeth-1.0.0rc4/avilla/elizabeth/impl/__init__.py
+-rw-rw-rw-   0        0        0     1781 2022-08-31 04:34:09.980332 avilla-elizabeth-1.0.0rc4/avilla/elizabeth/impl/friend.py
+-rw-rw-rw-   0        0        0     9574 2022-08-31 04:34:09.989126 avilla-elizabeth-1.0.0rc4/avilla/elizabeth/impl/group.py
+-rw-rw-rw-   0        0        0     1867 2022-08-31 04:32:04.360005 avilla-elizabeth-1.0.0rc4/avilla/elizabeth/message_deserializer.py
+-rw-rw-rw-   0        0        0     1808 2022-08-31 04:32:04.361963 avilla-elizabeth-1.0.0rc4/avilla/elizabeth/message_serializer.py
+-rw-rw-rw-   0        0        0     2333 2022-08-31 04:34:09.996931 avilla-elizabeth-1.0.0rc4/avilla/elizabeth/protocol.py
+-rw-rw-rw-   0        0        0     1524 2022-08-31 04:32:04.363912 avilla-elizabeth-1.0.0rc4/avilla/elizabeth/resource.py
+-rw-rw-rw-   0        0        0     1988 2022-08-31 04:32:04.364894 avilla-elizabeth-1.0.0rc4/avilla/elizabeth/service.py
+-rw-rw-rw-   0        0        0     1091 2022-02-26 15:50:19.520302 avilla-elizabeth-1.0.0rc4/LICENSE
+-rw-rw-rw-   0        0        0     2051 2022-08-31 04:36:38.408969 avilla-elizabeth-1.0.0rc4/pyproject.toml
+-rw-rw-rw-   0        0        0     7166 2022-08-31 04:32:04.240367 avilla-elizabeth-1.0.0rc4/README.md
+-rw-rw-rw-   0        0        0     7371 2022-08-31 04:41:00.756210 avilla-elizabeth-1.0.0rc4/PKG-INFO
```

### Comparing `avilla_elizabeth-1.0.0a7/LICENSE` & `avilla-elizabeth-1.0.0rc4/LICENSE`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2021 Graia Project
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2021 Graia Project
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `avilla_elizabeth-1.0.0a7/avilla/elizabeth/exception.py` & `avilla-elizabeth-1.0.0rc4/avilla/elizabeth/exception.py`

 * *Files identical despite different names*

