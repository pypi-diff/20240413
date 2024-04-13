# Comparing `tmp/pycityagent-1.1.6.tar.gz` & `tmp/pycityagent-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycityagent-1.1.6.tar", last modified: Sat Apr 13 11:07:36 2024, max compression
+gzip compressed data, was "pycityagent-1.1.7.tar", last modified: Sat Apr 13 15:11:57 2024, max compression
```

## Comparing `pycityagent-1.1.6.tar` & `pycityagent-1.1.7.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 11:07:36.995474 pycityagent-1.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-13 11:07:32.000000 pycityagent-1.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7758 2024-04-13 11:07:36.995474 pycityagent-1.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-04-13 11:07:32.000000 pycityagent-1.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 11:07:36.987474 pycityagent-1.1.6/pycityagent/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 11:07:36.987474 pycityagent-1.1.6/pycityagent/ac/
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/ac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/ac/ac.py
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/ac/action.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/ac/action_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 11:07:36.987474 pycityagent-1.1.6/pycityagent/ac/citizen_actions/
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/ac/citizen_actions/controled.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/ac/citizen_actions/converse.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/ac/citizen_actions/idle.py
--rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/ac/citizen_actions/shop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/ac/citizen_actions/trip.py
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/ac/hub_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/ac/sim_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8767 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     5213 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/agent_citizen.py
--rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/agent_func.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 11:07:36.991474 pycityagent-1.1.6/pycityagent/brain/
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/brain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/brain/brain.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/brain/brainfc.py
--rw-r--r--   0 runner    (1001) docker     (127)    22067 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/brain/memory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 11:07:36.991474 pycityagent-1.1.6/pycityagent/brain/persistence/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/brain/persistence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/brain/persistence/social.py
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/brain/persistence/spatial.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 11:07:36.991474 pycityagent-1.1.6/pycityagent/brain/reason/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/brain/reason/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/brain/reason/shop.py
--rw-r--r--   0 runner    (1001) docker     (127)     6493 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/brain/reason/social.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/brain/reason/trip.py
--rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/brain/reason/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 11:07:36.991474 pycityagent-1.1.6/pycityagent/brain/retrive/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/brain/retrive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/brain/retrive/social.py
--rw-r--r--   0 runner    (1001) docker     (127)    18593 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/brain/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)    28724 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/brain/sence.py
--rw-r--r--   0 runner    (1001) docker     (127)    29101 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/brain/static.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 11:07:36.991474 pycityagent-1.1.6/pycityagent/cc/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/cc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/cc/cc.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/cc/conve.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/cc/idle.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/cc/shop.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/cc/trip.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/cc/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 11:07:36.991474 pycityagent-1.1.6/pycityagent/hubconnector/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/hubconnector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4908 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/hubconnector/hubconnector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 11:07:36.991474 pycityagent-1.1.6/pycityagent/image/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5501 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/image/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     5810 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/simulator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 11:07:36.995474 pycityagent-1.1.6/pycityagent/st/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/st/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5210 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/st/st.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 11:07:36.995474 pycityagent-1.1.6/pycityagent/urbanllm/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/urbanllm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5221 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/urbanllm/urbanllm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 11:07:36.995474 pycityagent-1.1.6/pycityagent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7758 2024-04-13 11:07:36.000000 pycityagent-1.1.6/pycityagent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-13 11:07:36.000000 pycityagent-1.1.6/pycityagent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 11:07:36.000000 pycityagent-1.1.6/pycityagent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-13 11:07:36.000000 pycityagent-1.1.6/pycityagent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-13 11:07:36.000000 pycityagent-1.1.6/pycityagent.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 11:07:36.995474 pycityagent-1.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:57.607262 pycityagent-1.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-13 15:11:51.000000 pycityagent-1.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7758 2024-04-13 15:11:57.607262 pycityagent-1.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-04-13 15:11:51.000000 pycityagent-1.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:57.599262 pycityagent-1.1.7/pycityagent/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-13 15:11:51.000000 pycityagent-1.1.7/pycityagent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:57.599262 pycityagent-1.1.7/pycityagent/ac/
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-13 15:11:51.000000 pycityagent-1.1.7/pycityagent/ac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-13 15:11:51.000000 pycityagent-1.1.7/pycityagent/ac/ac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-13 15:11:51.000000 pycityagent-1.1.7/pycityagent/ac/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-13 15:11:51.000000 pycityagent-1.1.7/pycityagent/ac/action_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:57.599262 pycityagent-1.1.7/pycityagent/ac/citizen_actions/
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-13 15:11:51.000000 pycityagent-1.1.7/pycityagent/ac/citizen_actions/controled.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-13 15:11:51.000000 pycityagent-1.1.7/pycityagent/ac/citizen_actions/converse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-13 15:11:51.000000 pycityagent-1.1.7/pycityagent/ac/citizen_actions/idle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-04-13 15:11:51.000000 pycityagent-1.1.7/pycityagent/ac/citizen_actions/shop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-13 15:11:51.000000 pycityagent-1.1.7/pycityagent/ac/citizen_actions/trip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-04-13 15:11:51.000000 pycityagent-1.1.7/pycityagent/ac/hub_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-04-13 15:11:51.000000 pycityagent-1.1.7/pycityagent/ac/sim_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8767 2024-04-13 15:11:51.000000 pycityagent-1.1.7/pycityagent/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5213 2024-04-13 15:11:51.000000 pycityagent-1.1.7/pycityagent/agent_citizen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-04-13 15:11:51.000000 pycityagent-1.1.7/pycityagent/agent_func.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:57.603262 pycityagent-1.1.7/pycityagent/brain/
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-13 15:11:51.000000 pycityagent-1.1.7/pycityagent/brain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-13 15:11:51.000000 pycityagent-1.1.7/pycityagent/brain/brain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-13 15:11:51.000000 pycityagent-1.1.7/pycityagent/brain/brainfc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22067 2024-04-13 15:11:51.000000 pycityagent-1.1.7/pycityagent/brain/memory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:57.603262 pycityagent-1.1.7/pycityagent/brain/persistence/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:51.000000 pycityagent-1.1.7/pycityagent/brain/persistence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-13 15:11:51.000000 pycityagent-1.1.7/pycityagent/brain/persistence/social.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-13 15:11:51.000000 pycityagent-1.1.7/pycityagent/brain/persistence/spatial.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:57.603262 pycityagent-1.1.7/pycityagent/brain/reason/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:51.000000 pycityagent-1.1.7/pycityagent/brain/reason/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-13 15:11:51.000000 pycityagent-1.1.7/pycityagent/brain/reason/shop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6493 2024-04-13 15:11:51.000000 pycityagent-1.1.7/pycityagent/brain/reason/social.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-13 15:11:51.000000 pycityagent-1.1.7/pycityagent/brain/reason/trip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-04-13 15:11:51.000000 pycityagent-1.1.7/pycityagent/brain/reason/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:57.603262 pycityagent-1.1.7/pycityagent/brain/retrive/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:51.000000 pycityagent-1.1.7/pycityagent/brain/retrive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-13 15:11:51.000000 pycityagent-1.1.7/pycityagent/brain/retrive/social.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18593 2024-04-13 15:11:51.000000 pycityagent-1.1.7/pycityagent/brain/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28861 2024-04-13 15:11:51.000000 pycityagent-1.1.7/pycityagent/brain/sence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29101 2024-04-13 15:11:51.000000 pycityagent-1.1.7/pycityagent/brain/static.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:57.603262 pycityagent-1.1.7/pycityagent/cc/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-13 15:11:51.000000 pycityagent-1.1.7/pycityagent/cc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-04-13 15:11:51.000000 pycityagent-1.1.7/pycityagent/cc/cc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-13 15:11:51.000000 pycityagent-1.1.7/pycityagent/cc/conve.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-13 15:11:51.000000 pycityagent-1.1.7/pycityagent/cc/idle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-13 15:11:51.000000 pycityagent-1.1.7/pycityagent/cc/shop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-13 15:11:51.000000 pycityagent-1.1.7/pycityagent/cc/trip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-13 15:11:51.000000 pycityagent-1.1.7/pycityagent/cc/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:57.603262 pycityagent-1.1.7/pycityagent/hubconnector/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-13 15:11:51.000000 pycityagent-1.1.7/pycityagent/hubconnector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4908 2024-04-13 15:11:51.000000 pycityagent-1.1.7/pycityagent/hubconnector/hubconnector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:57.607262 pycityagent-1.1.7/pycityagent/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-13 15:11:51.000000 pycityagent-1.1.7/pycityagent/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5501 2024-04-13 15:11:51.000000 pycityagent-1.1.7/pycityagent/image/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5810 2024-04-13 15:11:51.000000 pycityagent-1.1.7/pycityagent/simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:57.607262 pycityagent-1.1.7/pycityagent/st/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-13 15:11:51.000000 pycityagent-1.1.7/pycityagent/st/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5210 2024-04-13 15:11:51.000000 pycityagent-1.1.7/pycityagent/st/st.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:57.607262 pycityagent-1.1.7/pycityagent/urbanllm/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-13 15:11:51.000000 pycityagent-1.1.7/pycityagent/urbanllm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5221 2024-04-13 15:11:51.000000 pycityagent-1.1.7/pycityagent/urbanllm/urbanllm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:57.607262 pycityagent-1.1.7/pycityagent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7758 2024-04-13 15:11:57.000000 pycityagent-1.1.7/pycityagent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-13 15:11:57.000000 pycityagent-1.1.7/pycityagent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:11:57.000000 pycityagent-1.1.7/pycityagent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-13 15:11:57.000000 pycityagent-1.1.7/pycityagent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-13 15:11:57.000000 pycityagent-1.1.7/pycityagent.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-13 15:11:51.000000 pycityagent-1.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 15:11:57.607262 pycityagent-1.1.7/setup.cfg
```

### Comparing `pycityagent-1.1.6/LICENSE` & `pycityagent-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.6/PKG-INFO` & `pycityagent-1.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycityagent
-Version: 1.1.6
+Version: 1.1.7
 Summary: LLM-based城市模拟器agent构建库
 Author-email: Yuwei Yan <pinkgranite86@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 FIBLAB
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pycityagent-1.1.6/README.md` & `pycityagent-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.6/pycityagent/ac/ac.py` & `pycityagent-1.1.7/pycityagent/ac/ac.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.6/pycityagent/ac/action.py` & `pycityagent-1.1.7/pycityagent/ac/action.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.6/pycityagent/ac/action_stream.py` & `pycityagent-1.1.7/pycityagent/ac/action_stream.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.6/pycityagent/ac/citizen_actions/controled.py` & `pycityagent-1.1.7/pycityagent/ac/citizen_actions/controled.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.6/pycityagent/ac/citizen_actions/converse.py` & `pycityagent-1.1.7/pycityagent/ac/citizen_actions/converse.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.6/pycityagent/ac/citizen_actions/idle.py` & `pycityagent-1.1.7/pycityagent/ac/citizen_actions/idle.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.6/pycityagent/ac/citizen_actions/shop.py` & `pycityagent-1.1.7/pycityagent/ac/citizen_actions/shop.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.6/pycityagent/ac/citizen_actions/trip.py` & `pycityagent-1.1.7/pycityagent/ac/citizen_actions/trip.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.6/pycityagent/ac/hub_actions.py` & `pycityagent-1.1.7/pycityagent/ac/hub_actions.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.6/pycityagent/ac/sim_actions.py` & `pycityagent-1.1.7/pycityagent/ac/sim_actions.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.6/pycityagent/agent.py` & `pycityagent-1.1.7/pycityagent/agent.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.6/pycityagent/agent_citizen.py` & `pycityagent-1.1.7/pycityagent/agent_citizen.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.6/pycityagent/agent_func.py` & `pycityagent-1.1.7/pycityagent/agent_func.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.6/pycityagent/brain/brain.py` & `pycityagent-1.1.7/pycityagent/brain/brain.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.6/pycityagent/brain/memory.py` & `pycityagent-1.1.7/pycityagent/brain/memory.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.6/pycityagent/brain/persistence/spatial.py` & `pycityagent-1.1.7/pycityagent/brain/persistence/spatial.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.6/pycityagent/brain/reason/shop.py` & `pycityagent-1.1.7/pycityagent/brain/reason/shop.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.6/pycityagent/brain/reason/social.py` & `pycityagent-1.1.7/pycityagent/brain/reason/social.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.6/pycityagent/brain/reason/trip.py` & `pycityagent-1.1.7/pycityagent/brain/reason/trip.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.6/pycityagent/brain/reason/user.py` & `pycityagent-1.1.7/pycityagent/brain/reason/user.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.6/pycityagent/brain/scheduler.py` & `pycityagent-1.1.7/pycityagent/brain/scheduler.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.6/pycityagent/brain/sence.py` & `pycityagent-1.1.7/pycityagent/brain/sence.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,40 +56,42 @@
 def get_xy_in_lane(nodes, distance, direction:str='front'):
     temp_sum = 0
     remain_s = 0
     if direction == 'front':
         # 顺道路方向前进
         if distance == 0:
             return [nodes[0]['x'], nodes[0]['y']]
-        key_index = 0
+        key_index = 0  # first node
         for i in range(1, len(nodes)):
             x1, y1 = nodes[i-1]['x'], nodes[i-1]['y']
             x2, y2 = nodes[i]['x'], nodes[i]['y']
             temp_sum += math.sqrt((x2 - x1)**2 + (y2-y1)**2)
             if temp_sum > distance:
                 remain_s = distance - (temp_sum - math.sqrt((x2 - x1)**2 + (y2-y1)**2))
                 break;
             key_index += 1
         if remain_s < 0.5:
-            return [nodes[-1]['x'], nodes[-1]['y']]
+            return [nodes[key_index]['x'], nodes[key_index]['y']]
         longlat = point_on_line_given_distance(nodes[key_index], nodes[key_index+1], remain_s)
         return longlat
     else:
         # 逆道路方向前进
-        key_index = len(nodes)
+        if distance == 0:
+            return [nodes[-1]['x'], nodes[-1]['y']]
+        key_index = len(nodes)-1  # last node
         for i in range(len(nodes)-1, 0, -1):
             x1, y1 = nodes[i]['x'], nodes[i]['y']
             x2, y2 = nodes[i-1]['x'], nodes[i-1]['y']
             temp_sum += math.sqrt((x2 - x1)**2 + (y2-y1)**2)
             if temp_sum > distance:
                 remain_s = distance - (temp_sum - math.sqrt((x2 - x1)**2 + (y2-y1)**2))
                 break;
             key_index -= 1
         if remain_s < 0.5:
-            return [nodes[0]['x'], nodes[0]['y']]
+            return [nodes[key_index]['x'], nodes[key_index]['y']]
         longlat = point_on_line_given_distance(nodes[key_index], nodes[key_index-1], remain_s)
         return longlat
 
 class SencePlug:
     """
     感知模块插件
     Plugin of Sence Module
@@ -403,26 +405,26 @@
             else:
                 # 非端点位置
                 neg_s = agent_s - radius_
                 neg_s = neg_s if neg_s >= 0 else 0
                 x, y = get_xy_in_lane(nodes, neg_s, 'back')
                 longlat = self._agent._simulator.map.xy2lnglat(x=x, y=y)
                 type = self._lane_type_mapping.get(lane['type'], 'unspecified')
-                positions += [{'lans_id': lane_id, 
+                positions += [{'lane_id': lane_id, 
                                's': neg_s, 
                                'xy': (x, y),
                                'longlat': longlat, 
                                'type': type}]
 
                 pos_s = agent_s + radius_
                 pos_s = pos_s if pos_s <= lane['length'] else lane['length']
                 x, y = get_xy_in_lane(nodes, pos_s)
                 longlat = self._agent._simulator.map.xy2lnglat(x=x, y=y)
                 type = self._lane_type_mapping.get(lane['type'], 'unspecified')
-                positions += [{'lans_id': lane_id, 
+                positions += [{'lane_id': lane_id, 
                                's': neg_s, 
                                'xy': (x, y),
                                'longlat': longlat, 
                                'type': type}]
         return positions
 
     async def PerceivePoi(self, radius:int=None, category:str=None):
```

### Comparing `pycityagent-1.1.6/pycityagent/brain/static.py` & `pycityagent-1.1.7/pycityagent/brain/static.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.6/pycityagent/cc/cc.py` & `pycityagent-1.1.7/pycityagent/cc/cc.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.6/pycityagent/hubconnector/hubconnector.py` & `pycityagent-1.1.7/pycityagent/hubconnector/hubconnector.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.6/pycityagent/image/image.py` & `pycityagent-1.1.7/pycityagent/image/image.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.6/pycityagent/simulator.py` & `pycityagent-1.1.7/pycityagent/simulator.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.6/pycityagent/st/st.py` & `pycityagent-1.1.7/pycityagent/st/st.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.6/pycityagent/urbanllm/urbanllm.py` & `pycityagent-1.1.7/pycityagent/urbanllm/urbanllm.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.6/pycityagent.egg-info/PKG-INFO` & `pycityagent-1.1.7/pycityagent.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycityagent
-Version: 1.1.6
+Version: 1.1.7
 Summary: LLM-based城市模拟器agent构建库
 Author-email: Yuwei Yan <pinkgranite86@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 FIBLAB
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pycityagent-1.1.6/pycityagent.egg-info/SOURCES.txt` & `pycityagent-1.1.7/pycityagent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.6/pyproject.toml` & `pycityagent-1.1.7/pyproject.toml`

 * *Files identical despite different names*

