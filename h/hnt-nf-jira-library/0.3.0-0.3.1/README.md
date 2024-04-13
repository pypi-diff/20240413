# Comparing `tmp/hnt_nf_jira_library-0.3.0.tar.gz` & `tmp/hnt_nf_jira_library-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hnt_nf_jira_library-0.3.0.tar", last modified: Fri Apr 12 20:11:51 2024, max compression
+gzip compressed data, was "hnt_nf_jira_library-0.3.1.tar", last modified: Fri Apr 12 21:52:20 2024, max compression
```

## Comparing `hnt_nf_jira_library-0.3.0.tar` & `hnt_nf_jira_library-0.3.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 20:11:51.344657 hnt_nf_jira_library-0.3.0/
--rw-rw-rw-   0        0        0      286 2024-04-12 20:11:51.344657 hnt_nf_jira_library-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0      381 2024-02-22 17:33:05.000000 hnt_nf_jira_library-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-12 20:11:51.343196 hnt_nf_jira_library-0.3.0/hnt_nf_jira_library.egg-info/
--rw-rw-rw-   0        0        0      286 2024-04-12 20:11:51.000000 hnt_nf_jira_library-0.3.0/hnt_nf_jira_library.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1065 2024-04-12 20:11:51.000000 hnt_nf_jira_library-0.3.0/hnt_nf_jira_library.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 20:11:51.000000 hnt_nf_jira_library-0.3.0/hnt_nf_jira_library.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-04-12 20:11:51.000000 hnt_nf_jira_library-0.3.0/hnt_nf_jira_library.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-12 20:11:51.000000 hnt_nf_jira_library-0.3.0/hnt_nf_jira_library.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-12 20:11:51.264292 hnt_nf_jira_library-0.3.0/nf_jira/
--rw-rw-rw-   0        0        0       30 2024-04-04 19:57:31.000000 hnt_nf_jira_library-0.3.0/nf_jira/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 20:11:51.317672 hnt_nf_jira_library-0.3.0/nf_jira/entities/
--rw-rw-rw-   0        0        0       92 2024-02-22 18:39:39.000000 hnt_nf_jira_library-0.3.0/nf_jira/entities/anexo.py
--rw-rw-rw-   0        0        0      110 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.3.0/nf_jira/entities/chave_acesso.py
-drwxrwxrwx   0        0        0        0 2024-04-12 20:11:51.332775 hnt_nf_jira_library-0.3.0/nf_jira/entities/classes/
--rw-rw-rw-   0        0        0     4819 2024-04-12 19:57:34.000000 hnt_nf_jira_library-0.3.0/nf_jira/entities/classes/form_jira.py
--rw-rw-rw-   0        0        0     2011 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.0/nf_jira/entities/classes/helper.py
--rw-rw-rw-   0        0        0     2019 2024-04-11 13:23:35.000000 hnt_nf_jira_library-0.3.0/nf_jira/entities/classes/issue_fields.py
--rw-rw-rw-   0        0        0     3049 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.0/nf_jira/entities/classes/issue_jira.py
--rw-rw-rw-   0        0        0     1695 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.0/nf_jira/entities/classes/n8n_domain.py
--rw-rw-rw-   0        0        0     2956 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.0/nf_jira/entities/constants.py
--rw-rw-rw-   0        0        0      331 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.0/nf_jira/entities/dados_basicos_fatura.py
--rw-rw-rw-   0        0        0      145 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.0/nf_jira/entities/dados_basicos_miro.py
--rw-rw-rw-   0        0        0      198 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.3.0/nf_jira/entities/dados_nfe.py
--rw-rw-rw-   0        0        0       76 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.3.0/nf_jira/entities/detalhe.py
--rw-rw-rw-   0        0        0      201 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.0/nf_jira/entities/fatura.py
--rw-rw-rw-   0        0        0      140 2024-04-11 13:23:35.000000 hnt_nf_jira_library-0.3.0/nf_jira/entities/item.py
--rw-rw-rw-   0        0        0      224 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.0/nf_jira/entities/itens_fatura.py
--rw-rw-rw-   0        0        0       97 2024-04-11 13:23:35.000000 hnt_nf_jira_library-0.3.0/nf_jira/entities/jira_info.py
--rw-rw-rw-   0        0        0      402 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.0/nf_jira/entities/miro copy.py
--rw-rw-rw-   0        0        0      402 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.0/nf_jira/entities/miro.py
--rw-rw-rw-   0        0        0      127 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.3.0/nf_jira/entities/nfe_sefaz.py
--rw-rw-rw-   0        0        0      379 2024-04-11 13:23:35.000000 hnt_nf_jira_library-0.3.0/nf_jira/entities/nota_pedido.py
--rw-rw-rw-   0        0        0      169 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.0/nf_jira/entities/pagamento.py
--rw-rw-rw-   0        0        0       92 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.3.0/nf_jira/entities/referencia_pedido.py
--rw-rw-rw-   0        0        0      173 2024-02-26 13:33:35.000000 hnt_nf_jira_library-0.3.0/nf_jira/entities/sintese_itens.py
--rw-rw-rw-   0        0        0       78 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.3.0/nf_jira/entities/sintese_miro.py
--rw-rw-rw-   0        0        0    20872 2024-04-12 19:50:36.000000 hnt_nf_jira_library-0.3.0/nf_jira/wrapper_nf_jira.py
--rw-rw-rw-   0        0        0       42 2024-04-12 20:11:51.344657 hnt_nf_jira_library-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0      510 2024-04-12 20:11:05.000000 hnt_nf_jira_library-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 21:52:20.538409 hnt_nf_jira_library-0.3.1/
+-rw-rw-rw-   0        0        0      286 2024-04-12 21:52:20.534408 hnt_nf_jira_library-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2024-02-22 17:33:05.000000 hnt_nf_jira_library-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-12 21:52:20.531405 hnt_nf_jira_library-0.3.1/hnt_nf_jira_library.egg-info/
+-rw-rw-rw-   0        0        0      286 2024-04-12 21:52:20.000000 hnt_nf_jira_library-0.3.1/hnt_nf_jira_library.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1065 2024-04-12 21:52:20.000000 hnt_nf_jira_library-0.3.1/hnt_nf_jira_library.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 21:52:20.000000 hnt_nf_jira_library-0.3.1/hnt_nf_jira_library.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-04-12 21:52:20.000000 hnt_nf_jira_library-0.3.1/hnt_nf_jira_library.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-12 21:52:20.000000 hnt_nf_jira_library-0.3.1/hnt_nf_jira_library.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-12 21:52:20.457397 hnt_nf_jira_library-0.3.1/nf_jira/
+-rw-rw-rw-   0        0        0       30 2024-04-04 19:57:31.000000 hnt_nf_jira_library-0.3.1/nf_jira/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 21:52:20.511405 hnt_nf_jira_library-0.3.1/nf_jira/entities/
+-rw-rw-rw-   0        0        0       92 2024-02-22 18:39:39.000000 hnt_nf_jira_library-0.3.1/nf_jira/entities/anexo.py
+-rw-rw-rw-   0        0        0      110 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.3.1/nf_jira/entities/chave_acesso.py
+drwxrwxrwx   0        0        0        0 2024-04-12 21:52:20.528405 hnt_nf_jira_library-0.3.1/nf_jira/entities/classes/
+-rw-rw-rw-   0        0        0     4819 2024-04-12 19:57:34.000000 hnt_nf_jira_library-0.3.1/nf_jira/entities/classes/form_jira.py
+-rw-rw-rw-   0        0        0     2011 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.1/nf_jira/entities/classes/helper.py
+-rw-rw-rw-   0        0        0     2019 2024-04-11 13:23:35.000000 hnt_nf_jira_library-0.3.1/nf_jira/entities/classes/issue_fields.py
+-rw-rw-rw-   0        0        0     3049 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.1/nf_jira/entities/classes/issue_jira.py
+-rw-rw-rw-   0        0        0     1695 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.1/nf_jira/entities/classes/n8n_domain.py
+-rw-rw-rw-   0        0        0     2956 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.1/nf_jira/entities/constants.py
+-rw-rw-rw-   0        0        0      331 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.1/nf_jira/entities/dados_basicos_fatura.py
+-rw-rw-rw-   0        0        0      145 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.1/nf_jira/entities/dados_basicos_miro.py
+-rw-rw-rw-   0        0        0      198 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.3.1/nf_jira/entities/dados_nfe.py
+-rw-rw-rw-   0        0        0       76 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.3.1/nf_jira/entities/detalhe.py
+-rw-rw-rw-   0        0        0      259 2024-04-12 21:48:41.000000 hnt_nf_jira_library-0.3.1/nf_jira/entities/fatura.py
+-rw-rw-rw-   0        0        0      140 2024-04-11 13:23:35.000000 hnt_nf_jira_library-0.3.1/nf_jira/entities/item.py
+-rw-rw-rw-   0        0        0      224 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.1/nf_jira/entities/itens_fatura.py
+-rw-rw-rw-   0        0        0       97 2024-04-11 13:23:35.000000 hnt_nf_jira_library-0.3.1/nf_jira/entities/jira_info.py
+-rw-rw-rw-   0        0        0      402 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.1/nf_jira/entities/miro copy.py
+-rw-rw-rw-   0        0        0      402 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.1/nf_jira/entities/miro.py
+-rw-rw-rw-   0        0        0      127 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.3.1/nf_jira/entities/nfe_sefaz.py
+-rw-rw-rw-   0        0        0      379 2024-04-11 13:23:35.000000 hnt_nf_jira_library-0.3.1/nf_jira/entities/nota_pedido.py
+-rw-rw-rw-   0        0        0      169 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.1/nf_jira/entities/pagamento.py
+-rw-rw-rw-   0        0        0       92 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.3.1/nf_jira/entities/referencia_pedido.py
+-rw-rw-rw-   0        0        0      173 2024-02-26 13:33:35.000000 hnt_nf_jira_library-0.3.1/nf_jira/entities/sintese_itens.py
+-rw-rw-rw-   0        0        0       78 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.3.1/nf_jira/entities/sintese_miro.py
+-rw-rw-rw-   0        0        0    20919 2024-04-12 21:46:51.000000 hnt_nf_jira_library-0.3.1/nf_jira/wrapper_nf_jira.py
+-rw-rw-rw-   0        0        0       42 2024-04-12 21:52:20.538409 hnt_nf_jira_library-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      510 2024-04-12 21:52:13.000000 hnt_nf_jira_library-0.3.1/setup.py
```

### Comparing `hnt_nf_jira_library-0.3.0/hnt_nf_jira_library.egg-info/SOURCES.txt` & `hnt_nf_jira_library-0.3.1/hnt_nf_jira_library.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.3.0/nf_jira/entities/classes/form_jira.py` & `hnt_nf_jira_library-0.3.1/nf_jira/entities/classes/form_jira.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.3.0/nf_jira/entities/classes/helper.py` & `hnt_nf_jira_library-0.3.1/nf_jira/entities/classes/helper.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.3.0/nf_jira/entities/classes/issue_fields.py` & `hnt_nf_jira_library-0.3.1/nf_jira/entities/classes/issue_fields.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.3.0/nf_jira/entities/classes/issue_jira.py` & `hnt_nf_jira_library-0.3.1/nf_jira/entities/classes/issue_jira.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.3.0/nf_jira/entities/classes/n8n_domain.py` & `hnt_nf_jira_library-0.3.1/nf_jira/entities/classes/n8n_domain.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.3.0/nf_jira/entities/constants.py` & `hnt_nf_jira_library-0.3.1/nf_jira/entities/constants.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.3.0/nf_jira/wrapper_nf_jira.py` & `hnt_nf_jira_library-0.3.1/nf_jira/wrapper_nf_jira.py`

 * *Files 0% similar despite different names*

```diff
@@ -294,15 +294,16 @@
         pagamento = {
             "data_basica": datetime.now().strftime("%d.%m.%Y"),
             "cond_pgto": "0000" #CONSTANTE 
         }
 
         fatura_model = {
             "dados_basicos": dados_basicos,
-            "pagamento":pagamento
+            "pagamento":pagamento,
+            "jira_info": issue["jira_info"],
         }
 
         return fatura_model
 
     def _get_nf_issue_context(self, issue_id: str):
         try:
```

