# Comparing `tmp/multi-agent-coordination-0.1.tar.gz` & `tmp/multi-agent-coordination-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\multi-agent-coordination-0.1.tar", last modified: Sun Mar  5 06:20:37 2023, max compression
+gzip compressed data, was "multi-agent-coordination-0.2.tar", last modified: Sat Apr 13 15:15:35 2024, max compression
```

## Comparing `multi-agent-coordination-0.1.tar` & `multi-agent-coordination-0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-03-05 06:20:37.000000 multi-agent-coordination-0.1/
--rw-rw-rw-   0        0        0     1089 2022-04-10 15:29:14.000000 multi-agent-coordination-0.1/LICENSE.txt
--rw-rw-rw-   0        0        0    14619 2023-03-05 06:20:37.000000 multi-agent-coordination-0.1/PKG-INFO
--rw-rw-rw-   0        0        0    13550 2023-03-05 05:39:18.000000 multi-agent-coordination-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-03-05 06:20:37.000000 multi-agent-coordination-0.1/multi_agent_coordination/
--rw-rw-rw-   0        0        0      147 2023-03-05 05:56:15.000000 multi-agent-coordination-0.1/multi_agent_coordination/__init__.py
--rw-rw-rw-   0        0        0    24596 2023-03-05 05:54:34.000000 multi-agent-coordination-0.1/multi_agent_coordination/simulation.py
-drwxrwxrwx   0        0        0        0 2023-03-05 06:20:37.000000 multi-agent-coordination-0.1/multi_agent_coordination.egg-info/
--rw-rw-rw-   0        0        0    14619 2023-03-05 06:20:29.000000 multi-agent-coordination-0.1/multi_agent_coordination.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      355 2023-03-05 06:20:29.000000 multi-agent-coordination-0.1/multi_agent_coordination.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-05 06:20:29.000000 multi-agent-coordination-0.1/multi_agent_coordination.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-03-05 06:20:29.000000 multi-agent-coordination-0.1/multi_agent_coordination.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-03-05 06:20:29.000000 multi-agent-coordination-0.1/multi_agent_coordination.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      115 2023-03-05 06:20:37.000000 multi-agent-coordination-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1450 2023-03-05 06:18:08.000000 multi-agent-coordination-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-13 15:15:35.707255 multi-agent-coordination-0.2/
+-rw-rw-rw-   0        0        0     1089 2022-04-10 15:29:14.000000 multi-agent-coordination-0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0    14620 2024-04-13 15:15:35.707255 multi-agent-coordination-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0    13550 2023-03-05 05:39:18.000000 multi-agent-coordination-0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-13 15:15:35.691676 multi-agent-coordination-0.2/multi_agent_coordination/
+-rw-rw-rw-   0        0        0      147 2023-03-05 05:56:15.000000 multi-agent-coordination-0.2/multi_agent_coordination/__init__.py
+-rw-rw-rw-   0        0        0    28705 2024-04-13 14:24:18.000000 multi-agent-coordination-0.2/multi_agent_coordination/simulation.py
+drwxrwxrwx   0        0        0        0 2024-04-13 15:15:35.707255 multi-agent-coordination-0.2/multi_agent_coordination.egg-info/
+-rw-rw-rw-   0        0        0    14620 2024-04-13 15:15:35.000000 multi-agent-coordination-0.2/multi_agent_coordination.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      355 2024-04-13 15:15:35.000000 multi-agent-coordination-0.2/multi_agent_coordination.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 15:15:35.000000 multi-agent-coordination-0.2/multi_agent_coordination.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2024-04-13 15:15:35.000000 multi-agent-coordination-0.2/multi_agent_coordination.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2024-04-13 15:15:35.000000 multi-agent-coordination-0.2/multi_agent_coordination.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      115 2024-04-13 15:15:35.707255 multi-agent-coordination-0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1486 2024-04-13 15:15:14.000000 multi-agent-coordination-0.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `multi-agent-coordination-0.1/LICENSE.txt` & `multi-agent-coordination-0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `multi-agent-coordination-0.1/PKG-INFO` & `multi-agent-coordination-0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: multi-agent-coordination
-Version: 0.1
+Version: 0.2
 Summary: Identification of strategic choices under multi-agent systems, coordination game and social networks
 Home-page: https://github.com/ankur-tutlani/multi-agent-coordination
-Download-URL: https://github.com/ankur-tutlani/multi_agent_coordination/archive/refs/tags/v_01.tar.gz
+Download-URL: https://github.com/ankur-tutlani/multi_agent_coordination/archive/refs/tags/v_02.tar.gz
 Author: ankurtutlani
 Author-email: ankur.tutlani@gmail.com
 License: MIT
 Keywords: game theory,evolutionary game,social norms,multi-agent systems,evolution,social network,computational economics,simulation,agent-based modeling,computation
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 
 # Evolution of Strategic Choices under Coordination and Social Networks
 
 This library is used to understand how specific actions or choices can evolve as the dominant choices when agents donot have any specific choices to begin with and they form their opinions based upon their interactions with other agents repeatedly. Agents have incentives to coordinate with other agents and are connected with each other through a specific social network. The strategies or actions which satisfy the norm criteria are potential candidates for setting the norm. In simple terms, norm is something which is played by more number of agents and for a longer periods of time.
```

### Comparing `multi-agent-coordination-0.1/README.md` & `multi-agent-coordination-0.2/README.md`

 * *Files identical despite different names*

### Comparing `multi-agent-coordination-0.1/multi_agent_coordination/simulation.py` & `multi-agent-coordination-0.2/multi_agent_coordination/simulation.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 import pandas as pd
 import networkx as nx
 import matplotlib.pyplot as plt
 import datetime
 import random
 import string
 
-
-
 # 1.iteration_name: iteration name. String
 # 2.path_to_save_output: path to save output files. String 
 # 3.num_neighbors: number of neighbours. Integer
 # 4.num_agents: number of agents. Integer
 # 5.prob_edge_rewire: small world network parameter. Probability of rewiring each edge. Float
 # 6.grid_network_m:  2-dimensional grid network parameter. Number of nodes. Integer
 # 7.grid_network_n:  2-dimensional grid network parameter. Number of nodes. Integer
@@ -44,25 +42,23 @@
 # small_world2: Returns a Newman–Watts–Strogatz small-world graph. Here number of edges increased once we increase the prob_edge_rewire value. Would add more shortcut edges in addition to what already exist.
 # small_world3: Returns a connected Watts–Strogatz small-world graph.
 # complete: Returns the complete graph.
 # random: Compute a random graph by swapping edges of a given graph.
 # grid2d: Return the 2d grid graph of mxn nodes, each connected to its nearest neighbors.
 
 
-
-
 def perturbed_response1(AGENT_NO,data_to_look,perturb_ratio,name_len,prob_new_name):
 
     try:
         count_pd = data_to_look.loc[data_to_look["agent"]==AGENT_NO]["name_offered_by_opponent"].value_counts().reset_index()
-        count_pd["tot_sum"] = count_pd["name_offered_by_opponent"] / sum(count_pd["name_offered_by_opponent"])
-        best_response = count_pd.loc[count_pd["tot_sum"] == max(count_pd["tot_sum"])]['index'].tolist()
+        count_pd["tot_sum"] = count_pd["count"] / sum(count_pd["count"])
+        best_response = count_pd.loc[count_pd["tot_sum"] == max(count_pd["tot_sum"])]['name_offered_by_opponent'].tolist()
         draw1= random.choices(population=best_response,k=1)
 
-        Nonbest_response = count_pd.loc[count_pd["tot_sum"] != max(count_pd["tot_sum"])]['index'].tolist()
+        Nonbest_response = count_pd.loc[count_pd["tot_sum"] != max(count_pd["tot_sum"])]['name_offered_by_opponent'].tolist()
         if len(Nonbest_response) > 0:
             draw2= random.choices(population=Nonbest_response,k=1)
             best_response = random.choices(population=[draw1[0],draw2[0]],weights=[1-perturb_ratio,perturb_ratio],k=1)
             best_response = best_response[0]
         else:
             best_response = draw1[0]
 
@@ -77,20 +73,19 @@
 
     best_response3 = random.choices(population=[best_response,best_response2],weights=[1-prob_new_name,prob_new_name],k=1)[0]
 
     return best_response3
 
 
 
-
 def perturbed_response2(AGENT_NO,data_to_look,name_len,prob_new_name):
     try:
         count_pd = data_to_look.loc[data_to_look["agent"]==AGENT_NO]["name_offered_by_opponent"].value_counts().reset_index()
-        count_pd["tot_sum"] = count_pd["name_offered_by_opponent"] / sum(count_pd["name_offered_by_opponent"])
-        names_list = count_pd['index'].tolist()
+        count_pd["tot_sum"] = count_pd["count"] / sum(count_pd["count"])
+        names_list = count_pd['name_offered_by_opponent'].tolist()
         share_list = count_pd['tot_sum'].tolist()
         draw1= random.choices(population=names_list,weights=share_list,k=1)
         best_response = draw1[0]
 
 
     except:
         best_response = [''.join(random.choices(string.ascii_uppercase+string.digits,k=name_len))]
@@ -102,23 +97,22 @@
     best_response3 = random.choices(population=[best_response,best_response2],weights=[1-prob_new_name,prob_new_name],k=1)[0]
 
 
     return best_response3
 
 
 
-
 def perturbed_response3(AGENT_NO,data_to_look,perturb_ratio,name_len,prob_new_name):
     try:
         count_pd = data_to_look.loc[data_to_look["agent"]==AGENT_NO]["name_offered_by_opponent"].value_counts().reset_index()
-        count_pd["tot_sum"] = count_pd["name_offered_by_opponent"] / sum(count_pd["name_offered_by_opponent"])
-        best_response = count_pd.loc[count_pd["tot_sum"] == max(count_pd["tot_sum"])]['index'].tolist()
+        count_pd["tot_sum"] = count_pd["count"] / sum(count_pd["count"])
+        best_response = count_pd.loc[count_pd["tot_sum"] == max(count_pd["tot_sum"])]['name_offered_by_opponent'].tolist()
         draw1= random.choices(population=best_response,k=1)
 
-        Nonbest_response = count_pd['index'].tolist()
+        Nonbest_response = count_pd['name_offered_by_opponent'].tolist()
         draw2= random.choices(population=Nonbest_response,k=1)
         best_response = random.choices(population=[draw1[0],draw2[0]],weights=[1-perturb_ratio,perturb_ratio],k=1)
         best_response = best_response[0]
 
     except:
         best_response = [''.join(random.choices(string.ascii_uppercase+string.digits,k=name_len))]
         best_response = best_response[0]
@@ -128,20 +122,19 @@
 
     best_response3 = random.choices(population=[best_response,best_response2],weights=[1-prob_new_name,prob_new_name],k=1)[0]
 
     return best_response3
 
 
 
-
 def perturbed_response4(AGENT_NO,data_to_look,name_len,prob_new_name):
     try:
         count_pd = data_to_look.loc[data_to_look["agent"]==AGENT_NO]["name_offered_by_opponent"].value_counts().reset_index()
-        count_pd["tot_sum"] = count_pd["name_offered_by_opponent"] / sum(count_pd["name_offered_by_opponent"])
-        best_response = count_pd.loc[count_pd["tot_sum"] == max(count_pd["tot_sum"])]['index'].tolist()
+        count_pd["tot_sum"] = count_pd["count"] / sum(count_pd["count"])
+        best_response = count_pd.loc[count_pd["tot_sum"] == max(count_pd["tot_sum"])]['name_offered_by_opponent'].tolist()
         draw1= random.choices(population=best_response,k=1)
         best_response = draw1[0]
 
     except:
         best_response = [''.join(random.choices(string.ascii_uppercase+string.digits,k=name_len))]
         best_response = best_response[0]
 
@@ -150,15 +143,14 @@
 
     best_response3 = random.choices(population=[best_response,best_response2],weights=[1-prob_new_name,prob_new_name],k=1)[0]
 
     return best_response3
 
 
 
-
 def network_simulations(iteration_name,
                         path_to_save_output,
                         num_neighbors,
                         num_agents,
                         prob_edge_rewire,
                         grid_network_m,
                         grid_network_n,
@@ -233,14 +225,19 @@
     num_of_rounds = len(potential_edges)
     norms_db_to_fill = pd.DataFrame()
     norms_db_to_fill['name'] = ''
     norms_db_to_fill['percent_count'] = ''
     norms_db_to_fill['timeperiod'] = ''
     
     
+    agents_in_edges = list(set([i[0] for i in potential_edges]+[i[1] for i in potential_edges]))
+    agents_in_network = list(range(num_agents))
+    delta_agents_hardcoded = [i for i in agents_in_network if i not in agents_in_edges]
+    
+    
     for timeperiod in range(1,num_of_trials+1):
         empty_df_to_fill_temp = empty_df_to_fill_trial[0:0]
         for v in range(num_of_rounds):
             vcheck = potential_edges[v]
             agent1 = vcheck[0]
             agent2 = vcheck[1]
 
@@ -252,41 +249,41 @@
                 else:
                     name_to_fill1 = perturbed_response1(AGENT_NO = agent1,data_to_look = empty_df_to_fill_trial,perturb_ratio=perturb_ratio,name_len=name_len,prob_new_name=prob_new_name)
                     name_to_fill2 = perturbed_response1(AGENT_NO = agent2,data_to_look = empty_df_to_fill_trial,perturb_ratio=perturb_ratio,name_len=name_len,prob_new_name=prob_new_name)
 
             elif function_to_use == 'perturbed_response2':
                 if len(empty_df_to_fill_temp) > len(empty_df_to_fill_trial):
 
-                    name_to_fill1 = perturbed_response1(AGENT_NO = agent1,data_to_look = empty_df_to_fill_temp,perturb_ratio=perturb_ratio,name_len=name_len,prob_new_name=prob_new_name)
-                    name_to_fill2 = perturbed_response1(AGENT_NO = agent2,data_to_look = empty_df_to_fill_temp,perturb_ratio=perturb_ratio,name_len=name_len,prob_new_name=prob_new_name)
+                    name_to_fill1 = perturbed_response2(AGENT_NO = agent1,data_to_look = empty_df_to_fill_temp,perturb_ratio=perturb_ratio,name_len=name_len,prob_new_name=prob_new_name)
+                    name_to_fill2 = perturbed_response2(AGENT_NO = agent2,data_to_look = empty_df_to_fill_temp,perturb_ratio=perturb_ratio,name_len=name_len,prob_new_name=prob_new_name)
                 else:
-                    name_to_fill1 = perturbed_response1(AGENT_NO = agent1,data_to_look = empty_df_to_fill_trial,perturb_ratio=perturb_ratio,name_len=name_len,prob_new_name=prob_new_name)
-                    name_to_fill2 = perturbed_response1(AGENT_NO = agent2,data_to_look = empty_df_to_fill_trial,perturb_ratio=perturb_ratio,name_len=name_len,prob_new_name=prob_new_name)
+                    name_to_fill1 = perturbed_response2(AGENT_NO = agent1,data_to_look = empty_df_to_fill_trial,perturb_ratio=perturb_ratio,name_len=name_len,prob_new_name=prob_new_name)
+                    name_to_fill2 = perturbed_response2(AGENT_NO = agent2,data_to_look = empty_df_to_fill_trial,perturb_ratio=perturb_ratio,name_len=name_len,prob_new_name=prob_new_name)
 
 
 
             elif function_to_use == 'perturbed_response3':
                 if len(empty_df_to_fill_temp) > len(empty_df_to_fill_trial):
 
-                    name_to_fill1 = perturbed_response1(AGENT_NO = agent1,data_to_look = empty_df_to_fill_temp,perturb_ratio=perturb_ratio,name_len=name_len,prob_new_name=prob_new_name)
-                    name_to_fill2 = perturbed_response1(AGENT_NO = agent2,data_to_look = empty_df_to_fill_temp,perturb_ratio=perturb_ratio,name_len=name_len,prob_new_name=prob_new_name)
+                    name_to_fill1 = perturbed_response3(AGENT_NO = agent1,data_to_look = empty_df_to_fill_temp,perturb_ratio=perturb_ratio,name_len=name_len,prob_new_name=prob_new_name)
+                    name_to_fill2 = perturbed_response3(AGENT_NO = agent2,data_to_look = empty_df_to_fill_temp,perturb_ratio=perturb_ratio,name_len=name_len,prob_new_name=prob_new_name)
                 else:
-                    name_to_fill1 = perturbed_response1(AGENT_NO = agent1,data_to_look = empty_df_to_fill_trial,perturb_ratio=perturb_ratio,name_len=name_len,prob_new_name=prob_new_name)
-                    name_to_fill2 = perturbed_response1(AGENT_NO = agent2,data_to_look = empty_df_to_fill_trial,perturb_ratio=perturb_ratio,name_len=name_len,prob_new_name=prob_new_name)
+                    name_to_fill1 = perturbed_response3(AGENT_NO = agent1,data_to_look = empty_df_to_fill_trial,perturb_ratio=perturb_ratio,name_len=name_len,prob_new_name=prob_new_name)
+                    name_to_fill2 = perturbed_response3(AGENT_NO = agent2,data_to_look = empty_df_to_fill_trial,perturb_ratio=perturb_ratio,name_len=name_len,prob_new_name=prob_new_name)
 
 
 
             elif function_to_use == 'perturbed_response4':
                 if len(empty_df_to_fill_temp) > len(empty_df_to_fill_trial):
 
-                    name_to_fill1 = perturbed_response1(AGENT_NO = agent1,data_to_look = empty_df_to_fill_temp,perturb_ratio=perturb_ratio,name_len=name_len,prob_new_name=prob_new_name)
-                    name_to_fill2 = perturbed_response1(AGENT_NO = agent2,data_to_look = empty_df_to_fill_temp,perturb_ratio=perturb_ratio,name_len=name_len,prob_new_name=prob_new_name)
+                    name_to_fill1 = perturbed_response4(AGENT_NO = agent1,data_to_look = empty_df_to_fill_temp,perturb_ratio=perturb_ratio,name_len=name_len,prob_new_name=prob_new_name)
+                    name_to_fill2 = perturbed_response4(AGENT_NO = agent2,data_to_look = empty_df_to_fill_temp,perturb_ratio=perturb_ratio,name_len=name_len,prob_new_name=prob_new_name)
                 else:
-                    name_to_fill1 = perturbed_response1(AGENT_NO = agent1,data_to_look = empty_df_to_fill_trial,perturb_ratio=perturb_ratio,name_len=name_len,prob_new_name=prob_new_name)
-                    name_to_fill2 = perturbed_response1(AGENT_NO = agent2,data_to_look = empty_df_to_fill_trial,perturb_ratio=perturb_ratio,name_len=name_len,prob_new_name=prob_new_name)
+                    name_to_fill1 = perturbed_response4(AGENT_NO = agent1,data_to_look = empty_df_to_fill_trial,perturb_ratio=perturb_ratio,name_len=name_len,prob_new_name=prob_new_name)
+                    name_to_fill2 = perturbed_response4(AGENT_NO = agent2,data_to_look = empty_df_to_fill_trial,perturb_ratio=perturb_ratio,name_len=name_len,prob_new_name=prob_new_name)
 
 
 
             if (agent1 in fixed_agents or agent2 in fixed_agents) and len(fixed_values_to_use) < len(fixed_agents):
                 for jj in fixed_agents:
                     if jj not in list(fixed_values_to_use.keys()):
                         xx = empty_df_to_fill_temp.loc[empty_df_to_fill_temp["agent"]==jj].sort_values(["timeperiod"],ascending=True).head(1)
@@ -325,14 +322,64 @@
                                                'opponentagent':agent1,
                                                'pair':str(vcheck), 
                                                'timeperiod':timeperiod
                                                },index=[0])
 
 
             empty_df_to_fill_temp = pd.concat([empty_df_to_fill_temp,data_to_append,data_to_append2],ignore_index=True,sort=False)
+            
+        if len(delta_agents_hardcoded) > 0:
+            for agent1 in delta_agents_hardcoded:
+                
+                if function_to_use == 'perturbed_response1':
+                    if len(empty_df_to_fill_temp) > len(empty_df_to_fill_trial):
+                        name_to_fill1 = perturbed_response1(AGENT_NO = agent1,data_to_look = empty_df_to_fill_temp,perturb_ratio=perturb_ratio,name_len=name_len,prob_new_name=prob_new_name)
+                    else:
+                        name_to_fill1 = perturbed_response1(AGENT_NO = agent1,data_to_look = empty_df_to_fill_trial,perturb_ratio=perturb_ratio,name_len=name_len,prob_new_name=prob_new_name)
+
+                elif function_to_use == 'perturbed_response2':
+                    if len(empty_df_to_fill_temp) > len(empty_df_to_fill_trial):
+                        name_to_fill1 = perturbed_response2(AGENT_NO = agent1,data_to_look = empty_df_to_fill_temp,perturb_ratio=perturb_ratio,name_len=name_len,prob_new_name=prob_new_name)
+                    else:
+                        name_to_fill1 = perturbed_response2(AGENT_NO = agent1,data_to_look = empty_df_to_fill_trial,perturb_ratio=perturb_ratio,name_len=name_len,prob_new_name=prob_new_name)
+
+                elif function_to_use == 'perturbed_response3':
+                    if len(empty_df_to_fill_temp) > len(empty_df_to_fill_trial):
+                        name_to_fill1 = perturbed_response3(AGENT_NO = agent1,data_to_look = empty_df_to_fill_temp,perturb_ratio=perturb_ratio,name_len=name_len,prob_new_name=prob_new_name)
+                    else:
+                        name_to_fill1 = perturbed_response3(AGENT_NO = agent1,data_to_look = empty_df_to_fill_trial,perturb_ratio=perturb_ratio,name_len=name_len,prob_new_name=prob_new_name)
+                
+                elif function_to_use == 'perturbed_response4':
+                    if len(empty_df_to_fill_temp) > len(empty_df_to_fill_trial):
+                        name_to_fill1 = perturbed_response4(AGENT_NO = agent1,data_to_look = empty_df_to_fill_temp,perturb_ratio=perturb_ratio,name_len=name_len,prob_new_name=prob_new_name)
+                    else:
+                        name_to_fill1 = perturbed_response4(AGENT_NO = agent1,data_to_look = empty_df_to_fill_trial,perturb_ratio=perturb_ratio,name_len=name_len,prob_new_name=prob_new_name)
+
+                if (agent1 in fixed_agents) and len(fixed_values_to_use) < len(fixed_agents):
+                    for jj in fixed_agents:
+                        if jj not in list(fixed_values_to_use.keys()):
+                            xx = empty_df_to_fill_temp.loc[empty_df_to_fill_temp["agent"]==jj].sort_values(["timeperiod"],ascending=True).head(1)
+                            if len(xx) > 0:
+                                fixed_values_to_use[xx["agent"].values[0]]=xx["name_offered"].values[0]
+                                
+                if agent1 in fixed_agents:
+                    try:
+                        name_offered = fixed_values_to_use[agent1]
+                    except:
+                        name_offered = name_to_fill1
+                else:
+                    name_offered = name_to_fill1
+                    
+                
+                data_to_append = pd.DataFrame({'agent':agent1,
+                                               'name_offered':name_offered,
+                                               'timeperiod':timeperiod
+                                               },index=[0])
+                
+                empty_df_to_fill_temp = pd.concat([empty_df_to_fill_temp,data_to_append],ignore_index=True,sort=False)
 
 
         empty_df_to_fill_trial = pd.concat([empty_df_to_fill_trial,empty_df_to_fill_temp],ignore_index=True,sort=False)
         footemp = empty_df_to_fill_temp['name_offered'].value_counts(normalize=True).to_frame()
         footemp.columns = ['percent_count']
         footemp['name'] = footemp.index.values
         footemp=footemp[['name','percent_count']].reset_index(drop=True)
@@ -426,17 +473,27 @@
     selected_norms = list(set(list_to_fill_for_labels_2))
     
     fig,ax = plt.subplots()
     data_for_trend_plot = norms_db_to_fill.loc[norms_db_to_fill['name'].isin(selected_norms)]
     data_for_trend_plot = data_for_trend_plot.reset_index(drop=True)
     for label,grp in data_for_trend_plot.groupby('name'):
         grp.plot(x='timeperiod',y='percent_count',ax=ax,label=label)
+    
+    
+    x_values11 = data_for_trend_plot['timeperiod'].unique()
+    total_periods11 = len(x_values11)
+    max_display_labels = 5  
+    interval11 = max(1, total_periods11 // max_display_labels)  
+
+    ax.set_xticks(np.arange(len(x_values11))[::interval11])
+    ax.set_xticklabels(x_values11[::interval11])
+
+
     ax.set_xlabel('Timeperiod')
     ax.set_ylabel('Count %')
-    # plt.show()
     plt.savefig(path_to_save_output+"top_names_"+iteration_name+"_"+today+".png")
     plt.clf()
     
     names_to_check = list(np.unique(empty_df_to_fill_trial['name_offered']))
     get_colors = lambda n: list(map(lambda i: "#" + "%06x" % random.randint(0, 0xFFFFFF),range(n)))
     list_of_colors = get_colors(len(names_to_check))
     
@@ -473,8 +530,9 @@
                   'function_to_use':function_to_use,'norms_agents_frequency':norms_agents_frequency,
                    'norms_time_frequency':norms_time_frequency}]).T
     parameters_pd.columns=["parameter_values"]
     parameters_pd["parameter"]=parameters_pd.index
     parameters_pd[["parameter","parameter_values"]].to_excel(path_to_save_output+"parameters_"+iteration_name+"_"+today+".xlsx",index=None)
 
 
-    return(print("done"))
+    return(print("done"))
+
```

### Comparing `multi-agent-coordination-0.1/multi_agent_coordination.egg-info/PKG-INFO` & `multi-agent-coordination-0.2/multi_agent_coordination.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: multi-agent-coordination
-Version: 0.1
+Version: 0.2
 Summary: Identification of strategic choices under multi-agent systems, coordination game and social networks
 Home-page: https://github.com/ankur-tutlani/multi-agent-coordination
-Download-URL: https://github.com/ankur-tutlani/multi_agent_coordination/archive/refs/tags/v_01.tar.gz
+Download-URL: https://github.com/ankur-tutlani/multi_agent_coordination/archive/refs/tags/v_02.tar.gz
 Author: ankurtutlani
 Author-email: ankur.tutlani@gmail.com
 License: MIT
 Keywords: game theory,evolutionary game,social norms,multi-agent systems,evolution,social network,computational economics,simulation,agent-based modeling,computation
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 
 # Evolution of Strategic Choices under Coordination and Social Networks
 
 This library is used to understand how specific actions or choices can evolve as the dominant choices when agents donot have any specific choices to begin with and they form their opinions based upon their interactions with other agents repeatedly. Agents have incentives to coordinate with other agents and are connected with each other through a specific social network. The strategies or actions which satisfy the norm criteria are potential candidates for setting the norm. In simple terms, norm is something which is played by more number of agents and for a longer periods of time.
```

### Comparing `multi-agent-coordination-0.1/setup.py` & `multi-agent-coordination-0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,35 +4,35 @@
 def read_file(filename):
     with open(os.path.join(os.path.dirname(__file__), filename)) as file:
         return file.read()
 
 setup(
   name = 'multi-agent-coordination',         
   packages = ['multi_agent_coordination'],   
-  version = '0.1',      
+  version = '0.2',      
   license='MIT',        
   description = 'Identification of strategic choices under multi-agent systems, coordination game and social networks',  
   long_description=read_file('README.md'),
   long_description_content_type='text/markdown',  
   author = 'ankurtutlani',                   
   author_email = 'ankur.tutlani@gmail.com',      
   url = 'https://github.com/ankur-tutlani/multi-agent-coordination',   
-  download_url = 'https://github.com/ankur-tutlani/multi_agent_coordination/archive/refs/tags/v_01.tar.gz',    
+  download_url = 'https://github.com/ankur-tutlani/multi_agent_coordination/archive/refs/tags/v_02.tar.gz',    
   keywords = ['game theory', 'evolutionary game', 'social norms','multi-agent systems','evolution','social network','computational economics','simulation','agent-based modeling','computation'],   
   install_requires=[            
-          'numpy',
-		  'pandas',
-		  'networkx',
-		  'matplotlib',
-		  'setuptools'
+          'numpy>=1.24.3',
+		  'pandas>=2.0.3',
+		  'networkx>=3.1',
+		  'matplotlib>=3.7.2',
+		  'setuptools>=68.0.0'
 		  
 		  
       ],
   classifiers=[
     'Development Status :: 3 - Alpha',      
     'Intended Audience :: Developers',      
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',   
 												
-	'Programming Language :: Python :: 3.7',
+	'Programming Language :: Python :: 3.11',
   ],
 )
```

