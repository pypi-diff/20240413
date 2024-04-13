# Comparing `tmp/reflex-chat-0.0.1a5.tar.gz` & `tmp/reflex-chat-0.0.1a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reflex-chat-0.0.1a5.tar", last modified: Fri Apr 12 01:10:48 2024, max compression
+gzip compressed data, was "reflex-chat-0.0.1a6.tar", last modified: Sat Apr 13 04:15:02 2024, max compression
```

## Comparing `reflex-chat-0.0.1a5.tar` & `reflex-chat-0.0.1a6.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2024-04-12 01:10:48.838246 reflex-chat-0.0.1a5/
--rw-r--r--   0 nikhil     (501) staff       (20)      672 2024-04-12 01:10:48.838040 reflex-chat-0.0.1a5/PKG-INFO
--rw-r--r--   0 nikhil     (501) staff       (20)       93 2024-03-07 21:28:46.000000 reflex-chat-0.0.1a5/README.md
-drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2024-04-12 01:10:48.836637 reflex-chat-0.0.1a5/custom_components/
-drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2024-04-12 01:10:48.837069 reflex-chat-0.0.1a5/custom_components/reflex_chat/
--rw-r--r--   0 nikhil     (501) staff       (20)       19 2024-04-05 22:25:08.000000 reflex-chat-0.0.1a5/custom_components/reflex_chat/__init__.py
--rw-r--r--   0 nikhil     (501) staff       (20)     4421 2024-04-12 01:08:21.000000 reflex-chat-0.0.1a5/custom_components/reflex_chat/chat.py
-drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2024-04-12 01:10:48.837762 reflex-chat-0.0.1a5/custom_components/reflex_chat.egg-info/
--rw-r--r--   0 nikhil     (501) staff       (20)      672 2024-04-12 01:10:48.000000 reflex-chat-0.0.1a5/custom_components/reflex_chat.egg-info/PKG-INFO
--rw-r--r--   0 nikhil     (501) staff       (20)      368 2024-04-12 01:10:48.000000 reflex-chat-0.0.1a5/custom_components/reflex_chat.egg-info/SOURCES.txt
--rw-r--r--   0 nikhil     (501) staff       (20)        1 2024-04-12 01:10:48.000000 reflex-chat-0.0.1a5/custom_components/reflex_chat.egg-info/dependency_links.txt
--rw-r--r--   0 nikhil     (501) staff       (20)       33 2024-04-12 01:10:48.000000 reflex-chat-0.0.1a5/custom_components/reflex_chat.egg-info/requires.txt
--rw-r--r--   0 nikhil     (501) staff       (20)       12 2024-04-12 01:10:48.000000 reflex-chat-0.0.1a5/custom_components/reflex_chat.egg-info/top_level.txt
--rw-r--r--   0 nikhil     (501) staff       (20)      762 2024-04-12 01:10:23.000000 reflex-chat-0.0.1a5/pyproject.toml
--rw-r--r--   0 nikhil     (501) staff       (20)       38 2024-04-12 01:10:48.838279 reflex-chat-0.0.1a5/setup.cfg
+drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2024-04-13 04:15:02.771173 reflex-chat-0.0.1a6/
+-rw-r--r--   0 nikhil     (501) staff       (20)     2646 2024-04-13 04:15:02.770977 reflex-chat-0.0.1a6/PKG-INFO
+-rw-r--r--   0 nikhil     (501) staff       (20)     2164 2024-04-13 00:01:45.000000 reflex-chat-0.0.1a6/README.md
+drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2024-04-13 04:15:02.768806 reflex-chat-0.0.1a6/custom_components/
+drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2024-04-13 04:15:02.769696 reflex-chat-0.0.1a6/custom_components/reflex_chat/
+-rw-r--r--   0 nikhil     (501) staff       (20)       19 2024-04-05 22:25:08.000000 reflex-chat-0.0.1a6/custom_components/reflex_chat/__init__.py
+-rw-r--r--   0 nikhil     (501) staff       (20)      929 2024-04-12 23:47:25.000000 reflex-chat-0.0.1a6/custom_components/reflex_chat/api.py
+-rw-r--r--   0 nikhil     (501) staff       (20)     5538 2024-04-13 00:14:04.000000 reflex-chat-0.0.1a6/custom_components/reflex_chat/chat.py
+drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2024-04-13 04:15:02.770702 reflex-chat-0.0.1a6/custom_components/reflex_chat.egg-info/
+-rw-r--r--   0 nikhil     (501) staff       (20)     2646 2024-04-13 04:15:02.000000 reflex-chat-0.0.1a6/custom_components/reflex_chat.egg-info/PKG-INFO
+-rw-r--r--   0 nikhil     (501) staff       (20)      405 2024-04-13 04:15:02.000000 reflex-chat-0.0.1a6/custom_components/reflex_chat.egg-info/SOURCES.txt
+-rw-r--r--   0 nikhil     (501) staff       (20)        1 2024-04-13 04:15:02.000000 reflex-chat-0.0.1a6/custom_components/reflex_chat.egg-info/dependency_links.txt
+-rw-r--r--   0 nikhil     (501) staff       (20)       33 2024-04-13 04:15:02.000000 reflex-chat-0.0.1a6/custom_components/reflex_chat.egg-info/requires.txt
+-rw-r--r--   0 nikhil     (501) staff       (20)       12 2024-04-13 04:15:02.000000 reflex-chat-0.0.1a6/custom_components/reflex_chat.egg-info/top_level.txt
+-rw-r--r--   0 nikhil     (501) staff       (20)      646 2024-04-13 04:14:55.000000 reflex-chat-0.0.1a6/pyproject.toml
+-rw-r--r--   0 nikhil     (501) staff       (20)       38 2024-04-13 04:15:02.771209 reflex-chat-0.0.1a6/setup.cfg
```

### Comparing `reflex-chat-0.0.1a5/custom_components/reflex_chat/chat.py` & `reflex-chat-0.0.1a6/custom_components/reflex_chat/chat.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,49 +1,62 @@
 """A custom component for a chat interface."""
 
-from typing import ClassVar
-
 import reflex as rx
 
 
 class Chat(rx.ComponentState):
     """A chat component with state."""
 
-    # The full chat history.
-    messages: list[dict[str, str]] = [{
-        "role": "system",
-        "content": "You are a friendly chatbot named Reflex. Respond in markdown."
-    }]
+    # The full chat history, in the OpenAI format.
+    messages2: list[dict[str, str]] = [
+        {
+            "role": "system",
+            "content": "You are a friendly chatbot named Reflex. Respond in markdown.",
+        }
+    ]
 
-    # Whether we are processing the question.
+    # Whether we are processing a message.
     processing: bool = False
 
+    @rx.var
+    def messages(self) -> list[dict[str, str]]:
+        """Return the chat history including the last submitted user message.
+
+        Returns:
+            The chat history as a list of dictionaries.
+        """
+        # Convert to a list before sending.
+        return self.get_value(self.messages2)
+
     @classmethod
     def create(self, process, **props):
         component = super().create(**props)
         component.State.process = process
         return component
 
     @classmethod
+    def get_id(cls):
+        return f"chatbox-{cls.get_full_name()}"
+
+    @classmethod
     def get_component(cls, **props) -> rx.Component:
         return rx.vstack(
-            rx.flex(
+            rx.box(
                 rx.logo(),
+                justify="left",
                 background_color=rx.color("accent", 4),
-                border_bottom=f"1px solid {rx.color('accent', 6)}",
                 width="100%",
-                justify="start",
             ),
             rx.spacer(),
             rx.vstack(
                 rx.box(
                     rx.foreach(
                         cls.messages, lambda message, i: chat_bubble(message, i)
                     ),
-                    id=f"chatbox-{cls.__name__}",
+                    id=f"chatbox-{cls.get_full_name()}",
                     overflow="auto",
                     width="100%",
                     padding_bottom="2em",
                 ),
                 rx.spacer(),
                 action_bar(cls),
                 padding=props.pop("padding", "1em"),
@@ -52,76 +65,105 @@
                 height="100%",
                 width="100%",
                 **props,
             ),
             spacing="0",
             height="100%",
             width="100%",
+            align="start",
         )
 
     def scroll_to_bottom(self):
         return rx.call_script(
             f"""
-    var element = document.getElementById('chatbox-{type(self).__name__}');
+    var element = document.getElementById({f"chatbox-{self.get_full_name()}"}');
     element.scrollTop = element.scrollHeight;
 """
         )
 
-    async def process_question(self):
+    async def process_message(self):
         async for value in self.process():
             yield value
 
         self.processing = False
 
         # Scroll to the last message.
         yield self.scroll_to_bottom()
 
     def submit_message(self, form_data: dict[str, str]):
-        # Get the question from the form
-        question = form_data[self.__class__.__name__]
+        # Get the message from the form
+        message = form_data[self.__class__.__name__]
 
-        # Check if the question is empty
-        if question == "":
+        # Check if the message is empty
+        if message == "":
             return
 
-        # Add the question to the list of questions.
-        self.messages.append({"role": "user", "content": question})
-        self.messages.append({"role": "assistant", "content": ""})
+        # Add the message to the list of messages.
+        self.messages2.append({"role": "user", "content": message})
+        self.messages2.append({"role": "assistant", "content": ""})
         self.processing = True
         yield self.scroll_to_bottom()
-        yield type(self).process_question
+        yield type(self).process_message
+
+    @rx.var
+    def last_user_message(self) -> str:
+        """Return the last submitted user message.
+
+        Returns:
+            The last submitted user message.
+        """
+        for message in reversed(self.messages2):
+            if message["role"] == "user":
+                return message["content"]
+        return ""
+
+    def append_to_response(self, answer: str):
+        """Append to the last answer in the chat history.
+
+        Args:
+            answer: The answer to add to the chat history.
+        """
+        self.messages2[-1]["content"] += answer or ""
 
 
 def chat_bubble(message: str, idx: int = 0) -> rx.Component:
     """Display a single chat bubble.
 
     Args:
         message: The message to display.
 
     Returns:
-        A component displaying the question/answer pair.
+        A component displaying the message/answer pair.
     """
     return rx.cond(
         message["role"] == "system",
         rx.fragment(),
         rx.box(
             rx.markdown(
                 message["content"],
-                background_color=rx.cond(message["role"] == "user", rx.color("mauve", 4), rx.color("accent", 4)),
-                color=rx.cond(message["role"] == "user", rx.color("mauve", 12), rx.color("accent", 12)),
+                background_color=rx.cond(
+                    message["role"] == "user",
+                    rx.color("mauve", 4),
+                    rx.color("accent", 4),
+                ),
+                color=rx.cond(
+                    message["role"] == "user",
+                    rx.color("mauve", 12),
+                    rx.color("accent", 12),
+                ),
                 display="inline-block",
                 padding_x="1em",
                 border_radius="8px",
                 max_width=["30em", "30em", "50em", "50em", "50em", "50em"],
             ),
             id=f"message-{idx}",
             text_align=rx.cond(message["role"] == "user", "right", "left"),
             margin_top="1em",
             width="100%",
-        )
+        ),
     )
 
 
 def action_bar(State) -> rx.Component:
     """The action bar to send a new message."""
     return rx.form(
         rx.hstack(
@@ -141,8 +183,9 @@
             width="100%",
         ),
         width="100%",
         on_submit=State.submit_message,
         reset_on_submit=True,
     )
 
+
 chat = Chat.create
```

### Comparing `reflex-chat-0.0.1a5/pyproject.toml` & `reflex-chat-0.0.1a6/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,26 @@
 [build-system]
-requires = [
-    "setuptools",
-    "wheel",
-]
+requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "reflex-chat"
-version = "0.0.1a5"
-description = "A chat component that can be hooked up to any LLM."
+version = "0.0.1a6"
+description = "Reflex custom component chat"
 readme = "README.md"
 license = { text = "Apache-2.0" }
 requires-python = ">=3.8"
-authors = [{ name = "Nikhil Rao", email = "nikhil@reflex.dev" }]
-keywords = [
-    "reflex",
-    "reflex-custom-components"]
-
-dependencies = [
-    "reflex>=0.4.2"
-]
-
-classifiers = [
-  "Development Status :: 4 - Beta",
-]
+authors = [{ name = "", email = "nikhil@reflex.dev" }]
+keywords = ["reflex","reflex-custom-components"]
+
+dependencies = ["reflex>=0.4.7"]
+
+classifiers = ["Development Status :: 4 - Beta"]
 
 [project.urls]
-homepage = "https://github.com/picklelo/reflex-chat"
-source = "https://github.com/picklelo/reflex-chat"
+Homepage = "https://github.com/picklelo/reflex-chat"
 
 [project.optional-dependencies]
 dev = ["build", "twine"]
 
-
 [tool.setuptools.packages.find]
 where = ["custom_components"]
```

