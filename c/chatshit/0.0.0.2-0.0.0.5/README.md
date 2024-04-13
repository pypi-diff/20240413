# Comparing `tmp/chatshit-0.0.0.2.tar.gz` & `tmp/chatshit-0.0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatshit-0.0.0.2.tar", max compression
+gzip compressed data, was "chatshit-0.0.0.5.tar", max compression
```

## Comparing `chatshit-0.0.0.2.tar` & `chatshit-0.0.0.5.tar`

### file list

```diff
@@ -1,12 +1,22 @@
--rw-r--r--   0        0        0       22 2023-10-15 19:42:51.703549 chatshit-0.0.0.2/README.md
--rw-r--r--   0        0        0        0 2023-10-13 13:59:07.830949 chatshit-0.0.0.2/chatshit/__init__.py
--rw-r--r--   0        0        0      713 2023-10-15 19:34:04.686518 chatshit-0.0.0.2/chatshit/__main__.py
--rw-r--r--   0        0        0     1084 2023-10-16 16:14:53.689894 chatshit-0.0.0.2/chatshit/app.py
--rw-r--r--   0        0        0     2080 2023-10-16 16:48:06.973250 chatshit-0.0.0.2/chatshit/client.py
--rw-r--r--   0        0        0     1819 2023-10-16 16:48:14.121361 chatshit-0.0.0.2/chatshit/loginscreen.py
--rw-r--r--   0        0        0      670 2023-10-15 19:23:31.607795 chatshit-0.0.0.2/chatshit/mainscreen.py
--rw-r--r--   0        0        0      588 2023-10-15 18:46:38.254741 chatshit-0.0.0.2/chatshit/message_list.py
--rw-r--r--   0        0        0     4172 2023-10-15 19:26:48.174005 chatshit-0.0.0.2/chatshit/server.py
--rw-r--r--   0        0        0     1238 2023-10-15 19:22:42.271240 chatshit-0.0.0.2/chatshit/styles.css
--rw-r--r--   0        0        0      429 2023-10-16 16:50:13.627150 chatshit-0.0.0.2/pyproject.toml
--rw-r--r--   0        0        0      523 1970-01-01 00:00:00.000000 chatshit-0.0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       22 2023-10-15 19:42:51.703549 chatshit-0.0.0.5/README.md
+-rw-r--r--   0        0        0        0 2023-10-13 13:59:07.830949 chatshit-0.0.0.5/chatshit/__init__.py
+-rw-r--r--   0        0        0      982 2024-04-13 17:36:21.578298 chatshit-0.0.0.5/chatshit/__main__.py
+-rw-r--r--   0        0        0     4203 2024-04-13 17:36:21.578298 chatshit-0.0.0.5/chatshit/app.py
+-rw-r--r--   0        0        0     5685 2024-04-13 17:36:21.578298 chatshit-0.0.0.5/chatshit/network/chatroom_server.py
+-rw-r--r--   0        0        0     1414 2024-04-13 17:36:21.578298 chatshit-0.0.0.5/chatshit/network/client.py
+-rw-r--r--   0        0        0     2268 2024-04-13 17:28:56.061402 chatshit-0.0.0.5/chatshit/network/proto.py
+-rw-r--r--   0        0        0     2741 2024-04-13 17:36:21.578298 chatshit-0.0.0.5/chatshit/screens/chatroom_screen.py
+-rw-r--r--   0        0        0      482 2024-04-13 17:36:21.578298 chatshit-0.0.0.5/chatshit/screens/client_screen.py
+-rw-r--r--   0        0        0     1081 2024-04-13 17:36:21.582298 chatshit-0.0.0.5/chatshit/screens/confirmation_screen.py
+-rw-r--r--   0        0        0     1391 2024-04-13 17:36:21.582298 chatshit-0.0.0.5/chatshit/screens/create_server_screen.py
+-rw-r--r--   0        0        0     1400 2024-04-13 17:36:21.582298 chatshit-0.0.0.5/chatshit/screens/delete_message_screen.py
+-rw-r--r--   0        0        0     1713 2024-04-13 17:36:21.582298 chatshit-0.0.0.5/chatshit/screens/home_screen.py
+-rw-r--r--   0        0        0     2516 2024-04-13 17:36:21.582298 chatshit-0.0.0.5/chatshit/screens/login_screen.py
+-rw-r--r--   0        0        0     4911 2024-04-13 17:36:21.582298 chatshit-0.0.0.5/chatshit/styles.css
+-rw-r--r--   0        0        0     1767 2024-04-13 17:36:21.582298 chatshit-0.0.0.5/chatshit/widgets/chat_list.py
+-rw-r--r--   0        0        0     1195 2024-04-13 17:36:21.582298 chatshit-0.0.0.5/chatshit/widgets/member_list.py
+-rw-r--r--   0        0        0     2088 2024-04-13 17:36:21.582298 chatshit-0.0.0.5/chatshit/widgets/message_list.py
+-rw-r--r--   0        0        0     1766 2024-04-13 17:36:21.582298 chatshit-0.0.0.5/chatshit/widgets/server_list.py
+-rw-r--r--   0        0        0      448 2024-04-13 17:30:10.794205 chatshit-0.0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      809 1970-01-01 00:00:00.000000 chatshit-0.0.0.5/setup.py
+-rw-r--r--   0        0        0      373 1970-01-01 00:00:00.000000 chatshit-0.0.0.5/PKG-INFO
```

### Comparing `chatshit-0.0.0.2/chatshit/loginscreen.py` & `chatshit-0.0.0.5/chatshit/screens/login_screen.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,54 +1,75 @@
-from threading import Thread
-from time import sleep
-
 from socket import gaierror
-from textual.app import ComposeResult
-from textual.containers import Container
+from textual.app import ComposeResult, events
+from textual.containers import ScrollableContainer
 from textual.screen import Screen
 from textual.widgets import Button, Input, Static
 
+from chatshit.network.client import Client
+
 
 class LoginScreen(Screen):
+
+    class Result:
+        def __init__(self, client: Client, name: str):
+            self.client = client
+            self.name = name
+
+    def __init__(
+        self,
+        host: str | None = None,
+        port: int | None = None,
+        classes: str | None = None,
+    ):
+        super().__init__(classes=classes)
+        self._host = host
+        self._port = port
+
     def compose(self) -> ComposeResult:
-        with Container(id="input-form"):
+        with ScrollableContainer(id="input-form"):
             self.info = Static("", id="connecting-error")
-            self.ip = Input(id="ip")
-            self.port = Input(id="port")
-            self.nickname = Input(id="nickname")
+            self.name_field = Input(id="name")
+            self.ip_field = Input(id="ip")
+            self.port_field = Input(id="port")
+            self.username_field = Input(id="username")
             self.button = Button("Connect", id="connect")
             yield self.info
-            yield self.ip
-            yield self.port
-            yield self.nickname
+            yield self.ip_field
+            yield self.port_field
+            yield self.username_field
+            yield self.name_field
             yield self.button
 
-    def on_mount(self) -> None:
-        self.ip.border_title = "IP"
-        self.port.border_title = "PORT"
-        self.nickname.border_title = "Nickname"
+    def on_mount(self):
+        self.ip_field.border_title = "IP"
+        self.port_field.border_title = "PORT"
+        self.username_field.border_title = "Username"
+        self.name_field.border_title = "Name (optional)"
+        self.ip_field.focus()
+        if self._host and self._port:
+            self.ip_field.value = self._host
+            self.port_field.value = str(self._port)
+            self.username_field.focus()
+
+    def on_key(self, event: events.Key):
+        if event.key == "escape":
+            event.stop()
+            self.dismiss(None)
 
-    def on_button_pressed(self) -> None:
+    def on_button_pressed(self):
         try:
-            self.connect_to_server()
+            self._client = Client(
+                self.ip_field.value, int(self.port_field.value), self.username_field.value
+            )
+            self._client.connect()
         except ValueError:
             self.info.update("Port is a number")
         except gaierror:
             self.info.update("Wrong address")
         except ConnectionRefusedError:
             self.info.update("No server on this port")
+        except OverflowError:
+            self.info.update("Port must be 0-65535.")
+        except TimeoutError:
+            self.info.update("Timeout")
         else:
-            if not self.app.client.connection_closed:
-                self.dismiss()
-            else:
-                self.info.update("Can't reach the server. Try again.")
-
-    def connect_to_server(self):
-        self.app.client.set_address(self.ip.value, int(self.port.value))
-        self.app.client.set_nickname(self.nickname.value)
-        conn_t = Thread(target=self.app.client.connect)
-        conn_t.daemon = True
-        conn_t.start()
-        for _ in range(10):
-            if not self.app.client.connection_closed:
-                break
-            sleep(0.5)
+            self.dismiss(self.Result(self._client, self.name_field.value))
```

