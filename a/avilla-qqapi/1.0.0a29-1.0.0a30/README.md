# Comparing `tmp/avilla_qqapi-1.0.0a29.tar.gz` & `tmp/avilla_qqapi-1.0.0a30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avilla_qqapi-1.0.0a29.tar", last modified: Fri Apr 12 14:08:36 2024, max compression
+gzip compressed data, was "avilla_qqapi-1.0.0a30.tar", last modified: Sat Apr 13 16:16:18 2024, max compression
```

## Comparing `avilla_qqapi-1.0.0a29.tar` & `avilla_qqapi-1.0.0a30.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0      447 2024-04-12 14:08:23.843206 avilla_qqapi-1.0.0a29/.mina/qqapi.toml
--rw-r--r--   0        0        0     1070 2024-04-12 14:08:23.847206 avilla_qqapi-1.0.0a29/LICENSE
--rw-r--r--   0        0        0     8444 2024-04-12 14:08:23.847206 avilla_qqapi-1.0.0a29/README.md
--rw-r--r--   0        0        0      102 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/__init__.py
--rw-r--r--   0        0        0      699 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/account.py
--rw-r--r--   0        0        0      253 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/audit/__init__.py
--rw-r--r--   0        0        0      761 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/audit/event.py
--rw-r--r--   0        0        0      417 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/audit/metadata.py
--rw-r--r--   0        0        0      886 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/audit/store.py
--rw-r--r--   0        0        0     3230 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/capability.py
--rw-r--r--   0        0        0        0 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/collector/__init__.py
--rw-r--r--   0        0        0      924 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/collector/connection.py
--rw-r--r--   0        0        0        0 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/connection/__init__.py
--rw-r--r--   0        0        0     3244 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/connection/base.py
--rw-r--r--   0        0        0     1870 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/connection/util.py
--rw-r--r--   0        0        0    17347 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/connection/ws_client.py
--rw-r--r--   0        0        0      941 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/const.py
--rw-r--r--   0        0        0     2297 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/element.py
--rw-r--r--   0        0        0     2330 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/exception.py
--rw-r--r--   0        0        0        0 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/perform/__init__.py
--rw-r--r--   0        0        0        0 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/perform/action/__init__.py
--rw-r--r--   0        0        0     2911 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/perform/action/channel.py
--rw-r--r--   0        0        0     1404 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/perform/action/guild.py
--rw-r--r--   0        0        0     8439 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/perform/action/guild_member.py
--rw-r--r--   0        0        0    19240 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/perform/action/message.py
--rw-r--r--   0        0        0    12722 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/perform/action/role.py
--rw-r--r--   0        0        0     1216 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/perform/action/user.py
--rw-r--r--   0        0        0     4853 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/perform/context.py
--rw-r--r--   0        0        0        0 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/perform/event/__init__.py
--rw-r--r--   0        0        0     3056 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/perform/event/activity.py
--rw-r--r--   0        0        0     2525 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/perform/event/audit.py
--rw-r--r--   0        0        0    13955 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/perform/event/message.py
--rw-r--r--   0        0        0     2256 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/perform/event/metadata.py
--rw-r--r--   0        0        0     7676 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/perform/event/relationship.py
--rw-r--r--   0        0        0     5474 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/perform/message/deserialize.py
--rw-r--r--   0        0        0     6431 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/perform/message/serialize.py
--rw-r--r--   0        0        0     5463 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/perform/query.py
--rw-r--r--   0        0        0     1139 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/perform/resource_fetch.py
--rw-r--r--   0        0        0     5030 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/protocol.py
--rw-r--r--   0        0        0      986 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/resource.py
--rw-r--r--   0        0        0      247 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/role/__init__.py
--rw-r--r--   0        0        0     1087 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/role/capability.py
--rw-r--r--   0        0        0      304 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/role/metadata.py
--rw-r--r--   0        0        0     1530 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/service.py
--rw-r--r--   0        0        0     1614 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/utils.py
--rw-r--r--   0        0        0      963 2024-04-12 14:08:36.595352 avilla_qqapi-1.0.0a29/pyproject.toml
--rw-r--r--   0        0        0     8835 1970-01-01 00:00:00.000000 avilla_qqapi-1.0.0a29/PKG-INFO
+-rw-r--r--   0        0        0      447 2024-04-13 16:16:06.621938 avilla_qqapi-1.0.0a30/.mina/qqapi.toml
+-rw-r--r--   0        0        0     1070 2024-04-13 16:16:06.621938 avilla_qqapi-1.0.0a30/LICENSE
+-rw-r--r--   0        0        0     8444 2024-04-13 16:16:06.621938 avilla_qqapi-1.0.0a30/README.md
+-rw-r--r--   0        0        0      102 2024-04-13 16:16:06.633938 avilla_qqapi-1.0.0a30/avilla/qqapi/__init__.py
+-rw-r--r--   0        0        0      699 2024-04-13 16:16:06.633938 avilla_qqapi-1.0.0a30/avilla/qqapi/account.py
+-rw-r--r--   0        0        0      253 2024-04-13 16:16:06.633938 avilla_qqapi-1.0.0a30/avilla/qqapi/audit/__init__.py
+-rw-r--r--   0        0        0      761 2024-04-13 16:16:06.633938 avilla_qqapi-1.0.0a30/avilla/qqapi/audit/event.py
+-rw-r--r--   0        0        0      417 2024-04-13 16:16:06.633938 avilla_qqapi-1.0.0a30/avilla/qqapi/audit/metadata.py
+-rw-r--r--   0        0        0      886 2024-04-13 16:16:06.633938 avilla_qqapi-1.0.0a30/avilla/qqapi/audit/store.py
+-rw-r--r--   0        0        0     3230 2024-04-13 16:16:06.633938 avilla_qqapi-1.0.0a30/avilla/qqapi/capability.py
+-rw-r--r--   0        0        0        0 2024-04-13 16:16:06.633938 avilla_qqapi-1.0.0a30/avilla/qqapi/collector/__init__.py
+-rw-r--r--   0        0        0      924 2024-04-13 16:16:06.633938 avilla_qqapi-1.0.0a30/avilla/qqapi/collector/connection.py
+-rw-r--r--   0        0        0        0 2024-04-13 16:16:06.633938 avilla_qqapi-1.0.0a30/avilla/qqapi/connection/__init__.py
+-rw-r--r--   0        0        0     3244 2024-04-13 16:16:06.633938 avilla_qqapi-1.0.0a30/avilla/qqapi/connection/base.py
+-rw-r--r--   0        0        0     1870 2024-04-13 16:16:06.633938 avilla_qqapi-1.0.0a30/avilla/qqapi/connection/util.py
+-rw-r--r--   0        0        0    17347 2024-04-13 16:16:06.633938 avilla_qqapi-1.0.0a30/avilla/qqapi/connection/ws_client.py
+-rw-r--r--   0        0        0      941 2024-04-13 16:16:06.633938 avilla_qqapi-1.0.0a30/avilla/qqapi/const.py
+-rw-r--r--   0        0        0     2297 2024-04-13 16:16:06.633938 avilla_qqapi-1.0.0a30/avilla/qqapi/element.py
+-rw-r--r--   0        0        0     2330 2024-04-13 16:16:06.633938 avilla_qqapi-1.0.0a30/avilla/qqapi/exception.py
+-rw-r--r--   0        0        0        0 2024-04-13 16:16:06.633938 avilla_qqapi-1.0.0a30/avilla/qqapi/perform/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 16:16:06.633938 avilla_qqapi-1.0.0a30/avilla/qqapi/perform/action/__init__.py
+-rw-r--r--   0        0        0     2911 2024-04-13 16:16:06.633938 avilla_qqapi-1.0.0a30/avilla/qqapi/perform/action/channel.py
+-rw-r--r--   0        0        0     1404 2024-04-13 16:16:06.633938 avilla_qqapi-1.0.0a30/avilla/qqapi/perform/action/guild.py
+-rw-r--r--   0        0        0     7763 2024-04-13 16:16:06.633938 avilla_qqapi-1.0.0a30/avilla/qqapi/perform/action/guild_member.py
+-rw-r--r--   0        0        0    19240 2024-04-13 16:16:06.633938 avilla_qqapi-1.0.0a30/avilla/qqapi/perform/action/message.py
+-rw-r--r--   0        0        0    12722 2024-04-13 16:16:06.633938 avilla_qqapi-1.0.0a30/avilla/qqapi/perform/action/role.py
+-rw-r--r--   0        0        0     1216 2024-04-13 16:16:06.633938 avilla_qqapi-1.0.0a30/avilla/qqapi/perform/action/user.py
+-rw-r--r--   0        0        0     4853 2024-04-13 16:16:06.633938 avilla_qqapi-1.0.0a30/avilla/qqapi/perform/context.py
+-rw-r--r--   0        0        0        0 2024-04-13 16:16:06.633938 avilla_qqapi-1.0.0a30/avilla/qqapi/perform/event/__init__.py
+-rw-r--r--   0        0        0     3056 2024-04-13 16:16:06.633938 avilla_qqapi-1.0.0a30/avilla/qqapi/perform/event/activity.py
+-rw-r--r--   0        0        0     2525 2024-04-13 16:16:06.633938 avilla_qqapi-1.0.0a30/avilla/qqapi/perform/event/audit.py
+-rw-r--r--   0        0        0    13955 2024-04-13 16:16:06.633938 avilla_qqapi-1.0.0a30/avilla/qqapi/perform/event/message.py
+-rw-r--r--   0        0        0     2256 2024-04-13 16:16:06.633938 avilla_qqapi-1.0.0a30/avilla/qqapi/perform/event/metadata.py
+-rw-r--r--   0        0        0     7676 2024-04-13 16:16:06.633938 avilla_qqapi-1.0.0a30/avilla/qqapi/perform/event/relationship.py
+-rw-r--r--   0        0        0     5474 2024-04-13 16:16:06.633938 avilla_qqapi-1.0.0a30/avilla/qqapi/perform/message/deserialize.py
+-rw-r--r--   0        0        0     6431 2024-04-13 16:16:06.633938 avilla_qqapi-1.0.0a30/avilla/qqapi/perform/message/serialize.py
+-rw-r--r--   0        0        0     5463 2024-04-13 16:16:06.633938 avilla_qqapi-1.0.0a30/avilla/qqapi/perform/query.py
+-rw-r--r--   0        0        0     1139 2024-04-13 16:16:06.633938 avilla_qqapi-1.0.0a30/avilla/qqapi/perform/resource_fetch.py
+-rw-r--r--   0        0        0     5030 2024-04-13 16:16:06.633938 avilla_qqapi-1.0.0a30/avilla/qqapi/protocol.py
+-rw-r--r--   0        0        0      986 2024-04-13 16:16:06.633938 avilla_qqapi-1.0.0a30/avilla/qqapi/resource.py
+-rw-r--r--   0        0        0      247 2024-04-13 16:16:06.633938 avilla_qqapi-1.0.0a30/avilla/qqapi/role/__init__.py
+-rw-r--r--   0        0        0     1087 2024-04-13 16:16:06.633938 avilla_qqapi-1.0.0a30/avilla/qqapi/role/capability.py
+-rw-r--r--   0        0        0      304 2024-04-13 16:16:06.633938 avilla_qqapi-1.0.0a30/avilla/qqapi/role/metadata.py
+-rw-r--r--   0        0        0     1530 2024-04-13 16:16:06.633938 avilla_qqapi-1.0.0a30/avilla/qqapi/service.py
+-rw-r--r--   0        0        0     1614 2024-04-13 16:16:06.633938 avilla_qqapi-1.0.0a30/avilla/qqapi/utils.py
+-rw-r--r--   0        0        0      963 2024-04-13 16:16:18.521911 avilla_qqapi-1.0.0a30/pyproject.toml
+-rw-r--r--   0        0        0     8835 1970-01-01 00:00:00.000000 avilla_qqapi-1.0.0a30/PKG-INFO
```

### Comparing `avilla_qqapi-1.0.0a29/LICENSE` & `avilla_qqapi-1.0.0a30/LICENSE`

 * *Files identical despite different names*

### Comparing `avilla_qqapi-1.0.0a29/README.md` & `avilla_qqapi-1.0.0a30/README.md`

 * *Files identical despite different names*

### Comparing `avilla_qqapi-1.0.0a29/avilla/qqapi/account.py` & `avilla_qqapi-1.0.0a30/avilla/qqapi/account.py`

 * *Files identical despite different names*

### Comparing `avilla_qqapi-1.0.0a29/avilla/qqapi/audit/event.py` & `avilla_qqapi-1.0.0a30/avilla/qqapi/audit/event.py`

 * *Files identical despite different names*

### Comparing `avilla_qqapi-1.0.0a29/avilla/qqapi/audit/store.py` & `avilla_qqapi-1.0.0a30/avilla/qqapi/audit/store.py`

 * *Files identical despite different names*

### Comparing `avilla_qqapi-1.0.0a29/avilla/qqapi/capability.py` & `avilla_qqapi-1.0.0a30/avilla/qqapi/capability.py`

 * *Files identical despite different names*

### Comparing `avilla_qqapi-1.0.0a29/avilla/qqapi/collector/connection.py` & `avilla_qqapi-1.0.0a30/avilla/qqapi/collector/connection.py`

 * *Files identical despite different names*

### Comparing `avilla_qqapi-1.0.0a29/avilla/qqapi/connection/base.py` & `avilla_qqapi-1.0.0a30/avilla/qqapi/connection/base.py`

 * *Files identical despite different names*

### Comparing `avilla_qqapi-1.0.0a29/avilla/qqapi/connection/util.py` & `avilla_qqapi-1.0.0a30/avilla/qqapi/connection/util.py`

 * *Files identical despite different names*

### Comparing `avilla_qqapi-1.0.0a29/avilla/qqapi/connection/ws_client.py` & `avilla_qqapi-1.0.0a30/avilla/qqapi/connection/ws_client.py`

 * *Files identical despite different names*

### Comparing `avilla_qqapi-1.0.0a29/avilla/qqapi/const.py` & `avilla_qqapi-1.0.0a30/avilla/qqapi/const.py`

 * *Files identical despite different names*

### Comparing `avilla_qqapi-1.0.0a29/avilla/qqapi/element.py` & `avilla_qqapi-1.0.0a30/avilla/qqapi/element.py`

 * *Files identical despite different names*

### Comparing `avilla_qqapi-1.0.0a29/avilla/qqapi/exception.py` & `avilla_qqapi-1.0.0a30/avilla/qqapi/exception.py`

 * *Files identical despite different names*

### Comparing `avilla_qqapi-1.0.0a29/avilla/qqapi/perform/action/channel.py` & `avilla_qqapi-1.0.0a30/avilla/qqapi/perform/action/channel.py`

 * *Files identical despite different names*

### Comparing `avilla_qqapi-1.0.0a29/avilla/qqapi/perform/action/guild.py` & `avilla_qqapi-1.0.0a30/avilla/qqapi/perform/action/guild.py`

 * *Files identical despite different names*

### Comparing `avilla_qqapi-1.0.0a29/avilla/qqapi/perform/action/guild_member.py` & `avilla_qqapi-1.0.0a30/avilla/qqapi/perform/action/guild_member.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,27 +128,15 @@
             "put",
             f"channels/{target.pattern['channel']}/members/{target.pattern['member']}/permissions",
             {"add": 4, "remove": 0},
         )
 
     @SceneCapability.remove_member.collect(m, target="land.guild.member")
     @SceneCapability.remove_member.collect(m, target="land.guild.channel.member")
-    async def remove_user(self, target: Selector, reason: str | None = None) -> None:
-        self_info = await self.account.connection.call_http(
-            "get", f"guilds/{target.pattern['guild']}/members/{self.account.route['account']}", {}
-        )
-        effective = bool({"2", "4", "5"} & set(self_info["roles"]))
-        if not effective:
-            raise PermissionError(permission_error_message(f"remove_member@{target.path}", "read", ["manage"]))
-        await self.account.connection.call_http(
-            "delete", f"guilds/{target.pattern['guild']}/members/{target.pattern['member']}", {}
-        )
-
-    @SceneCapability.remove_member.collect(m, target="land.guild.channel.member")
-    async def remove_member(self, target: Selector, reason: str | None = None) -> None:
+    async def remove_member(self, target: Selector, reason: str | None = None, permanent: bool = False) -> None:
         self_info = await self.account.connection.call_http(
             "get", f"guilds/{target.pattern['guild']}/members/{self.account.route['account']}", {}
         )
         effective = bool({"2", "4", "5"} & set(self_info["roles"]))
         if not effective:
             raise PermissionError(permission_error_message(f"remove_member@{target.path}", "read", ["manage"]))
         await self.account.connection.call_http(
```

### Comparing `avilla_qqapi-1.0.0a29/avilla/qqapi/perform/action/message.py` & `avilla_qqapi-1.0.0a30/avilla/qqapi/perform/action/message.py`

 * *Files identical despite different names*

### Comparing `avilla_qqapi-1.0.0a29/avilla/qqapi/perform/action/role.py` & `avilla_qqapi-1.0.0a30/avilla/qqapi/perform/action/role.py`

 * *Files identical despite different names*

### Comparing `avilla_qqapi-1.0.0a29/avilla/qqapi/perform/action/user.py` & `avilla_qqapi-1.0.0a30/avilla/qqapi/perform/action/user.py`

 * *Files identical despite different names*

### Comparing `avilla_qqapi-1.0.0a29/avilla/qqapi/perform/context.py` & `avilla_qqapi-1.0.0a30/avilla/qqapi/perform/context.py`

 * *Files identical despite different names*

### Comparing `avilla_qqapi-1.0.0a29/avilla/qqapi/perform/event/activity.py` & `avilla_qqapi-1.0.0a30/avilla/qqapi/perform/event/activity.py`

 * *Files identical despite different names*

### Comparing `avilla_qqapi-1.0.0a29/avilla/qqapi/perform/event/audit.py` & `avilla_qqapi-1.0.0a30/avilla/qqapi/perform/event/audit.py`

 * *Files identical despite different names*

### Comparing `avilla_qqapi-1.0.0a29/avilla/qqapi/perform/event/message.py` & `avilla_qqapi-1.0.0a30/avilla/qqapi/perform/event/message.py`

 * *Files identical despite different names*

### Comparing `avilla_qqapi-1.0.0a29/avilla/qqapi/perform/event/metadata.py` & `avilla_qqapi-1.0.0a30/avilla/qqapi/perform/event/metadata.py`

 * *Files identical despite different names*

### Comparing `avilla_qqapi-1.0.0a29/avilla/qqapi/perform/event/relationship.py` & `avilla_qqapi-1.0.0a30/avilla/qqapi/perform/event/relationship.py`

 * *Files identical despite different names*

### Comparing `avilla_qqapi-1.0.0a29/avilla/qqapi/perform/message/deserialize.py` & `avilla_qqapi-1.0.0a30/avilla/qqapi/perform/message/deserialize.py`

 * *Files identical despite different names*

### Comparing `avilla_qqapi-1.0.0a29/avilla/qqapi/perform/message/serialize.py` & `avilla_qqapi-1.0.0a30/avilla/qqapi/perform/message/serialize.py`

 * *Files identical despite different names*

### Comparing `avilla_qqapi-1.0.0a29/avilla/qqapi/perform/query.py` & `avilla_qqapi-1.0.0a30/avilla/qqapi/perform/query.py`

 * *Files identical despite different names*

### Comparing `avilla_qqapi-1.0.0a29/avilla/qqapi/perform/resource_fetch.py` & `avilla_qqapi-1.0.0a30/avilla/qqapi/perform/resource_fetch.py`

 * *Files identical despite different names*

### Comparing `avilla_qqapi-1.0.0a29/avilla/qqapi/protocol.py` & `avilla_qqapi-1.0.0a30/avilla/qqapi/protocol.py`

 * *Files identical despite different names*

### Comparing `avilla_qqapi-1.0.0a29/avilla/qqapi/resource.py` & `avilla_qqapi-1.0.0a30/avilla/qqapi/resource.py`

 * *Files identical despite different names*

### Comparing `avilla_qqapi-1.0.0a29/avilla/qqapi/role/capability.py` & `avilla_qqapi-1.0.0a30/avilla/qqapi/role/capability.py`

 * *Files identical despite different names*

### Comparing `avilla_qqapi-1.0.0a29/avilla/qqapi/service.py` & `avilla_qqapi-1.0.0a30/avilla/qqapi/service.py`

 * *Files identical despite different names*

### Comparing `avilla_qqapi-1.0.0a29/avilla/qqapi/utils.py` & `avilla_qqapi-1.0.0a30/avilla/qqapi/utils.py`

 * *Files identical despite different names*

### Comparing `avilla_qqapi-1.0.0a29/pyproject.toml` & `avilla_qqapi-1.0.0a30/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "avilla-qqapi"
-version = "1.0.0a29"
+version = "1.0.0a30"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "aiohttp>=3.8.1",
 ]
 description = ""
```

### Comparing `avilla_qqapi-1.0.0a29/PKG-INFO` & `avilla_qqapi-1.0.0a30/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avilla-qqapi
-Version: 1.0.0a29
+Version: 1.0.0a30
 Home-page: https://github.com/GraiaProject/Avilla
 Author-Email: RF-Tar-Railt <rf_tar_railt@qq.com>
 License: MIT
 Project-URL: Homepage, https://github.com/GraiaProject/Avilla
 Project-URL: Repository, https://github.com/GraiaProject/Avilla
 Requires-Python: >=3.9
 Requires-Dist: aiohttp>=3.8.1
```

