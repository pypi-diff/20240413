# Comparing `tmp/getlino-24.3.0.tar.gz` & `tmp/getlino-24.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getlino-24.3.0.tar", last modified: Fri Mar 15 12:34:28 2024, max compression
+gzip compressed data, was "getlino-24.4.0.tar", last modified: Fri Apr 12 23:15:52 2024, max compression
```

## Comparing `getlino-24.3.0.tar` & `getlino-24.4.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-15 12:34:28.151673 getlino-24.3.0/
--rw-rw-rw-   0 luc       (1000) www-data    (33)    34523 2021-04-07 12:56:36.000000 getlino-24.3.0/COPYING
--rw-rw-rw-   0 luc       (1000) www-data    (33)       59 2019-10-25 15:17:06.000000 getlino-24.3.0/MANIFEST.in
--rw-r--r--   0 luc       (1000) www-data    (33)     1559 2024-03-15 12:34:28.151673 getlino-24.3.0/PKG-INFO
--rw-rw-rw-   0 luc       (1000) www-data    (33)      692 2021-06-11 08:29:48.000000 getlino-24.3.0/README.rst
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-15 12:34:28.143673 getlino-24.3.0/getlino/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      322 2024-02-14 17:37:21.000000 getlino-24.3.0/getlino/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      816 2024-02-14 17:37:21.000000 getlino-24.3.0/getlino/cli.py
--rw-rw-r--   0 luc       (1000) www-data    (33)    20585 2024-02-14 17:37:21.000000 getlino-24.3.0/getlino/configure.py
--rw-rw-r--   0 luc       (1000) www-data    (33)     1094 2024-03-15 07:19:39.000000 getlino-24.3.0/getlino/list.py
--rw-rw-r--   0 luc       (1000) www-data    (33)     1788 2024-03-15 12:34:16.000000 getlino-24.3.0/getlino/setup_info.py
--rw-rw-r--   0 luc       (1000) www-data    (33)     7794 2024-03-11 13:29:19.000000 getlino-24.3.0/getlino/startproject.py
--rw-rw-r--   0 luc       (1000) www-data    (33)    25808 2024-03-15 10:49:00.000000 getlino-24.3.0/getlino/startsite.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-15 12:34:28.147673 getlino-24.3.0/getlino/templates/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      890 2021-02-12 13:40:30.000000 getlino-24.3.0/getlino/templates/apache.conf
--rw-rw-rw-   0 luc       (1000) www-data    (33)      214 2022-09-10 15:27:38.000000 getlino-24.3.0/getlino/templates/asgi.py
--rw-rw-r--   0 luc       (1000) www-data    (33)     1678 2024-02-22 15:57:56.000000 getlino-24.3.0/getlino/templates/daphne_supervisor.conf
--rw-rw-r--   0 luc       (1000) www-data    (33)      852 2023-01-01 07:07:06.000000 getlino-24.3.0/getlino/templates/django_settings.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      371 2023-07-01 18:31:56.000000 getlino-24.3.0/getlino/templates/healthcheck.sh
--rw-rw-r--   0 luc       (1000) www-data    (33)      308 2023-01-15 18:29:24.000000 getlino-24.3.0/getlino/templates/lino.ini
--rwxrwxr-x   0 luc       (1000) www-data    (33)     2074 2022-09-15 06:25:41.000000 getlino-24.3.0/getlino/templates/make_snapshot.sh
--rw-rw-r--   0 luc       (1000) www-data    (33)      329 2023-11-05 18:22:29.000000 getlino-24.3.0/getlino/templates/manage.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1671 2023-07-16 11:11:44.000000 getlino-24.3.0/getlino/templates/nginx.conf
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1543 2022-09-10 15:27:38.000000 getlino-24.3.0/getlino/templates/nginx_asgi.conf
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1558 2023-10-08 06:14:57.000000 getlino-24.3.0/getlino/templates/pull.sh
--rw-rw-r--   0 luc       (1000) www-data    (33)     1472 2023-11-14 01:23:35.000000 getlino-24.3.0/getlino/templates/settings.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1361 2021-02-10 17:53:35.000000 getlino-24.3.0/getlino/templates/uwsgi.ini
--rw-rw-rw-   0 luc       (1000) www-data    (33)      664 2019-10-25 14:15:15.000000 getlino-24.3.0/getlino/templates/uwsgi_params
--rw-rw-rw-   0 luc       (1000) www-data    (33)      251 2019-10-25 14:30:31.000000 getlino-24.3.0/getlino/templates/wsgi.py
--rw-rw-r--   0 luc       (1000) www-data    (33)    20790 2024-03-15 06:49:14.000000 getlino-24.3.0/getlino/utils.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-15 12:34:28.147673 getlino-24.3.0/getlino.egg-info/
--rw-r--r--   0 luc       (1000) www-data    (33)     1559 2024-03-15 12:34:28.000000 getlino-24.3.0/getlino.egg-info/PKG-INFO
--rw-rw-rw-   0 luc       (1000) www-data    (33)      983 2024-03-15 12:34:28.000000 getlino-24.3.0/getlino.egg-info/SOURCES.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2024-03-15 12:34:28.000000 getlino-24.3.0/getlino.egg-info/dependency_links.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)       45 2024-03-15 12:34:28.000000 getlino-24.3.0/getlino.egg-info/entry_points.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2019-06-20 10:29:13.000000 getlino-24.3.0/getlino.egg-info/not-zip-safe
--rw-rw-rw-   0 luc       (1000) www-data    (33)       56 2024-03-15 12:34:28.000000 getlino-24.3.0/getlino.egg-info/requires.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)        8 2024-03-15 12:34:28.000000 getlino-24.3.0/getlino.egg-info/top_level.txt
--rw-rw-r--   0 luc       (1000) www-data    (33)       38 2024-03-15 12:34:28.151673 getlino-24.3.0/setup.cfg
--rw-rw-rw-   0 luc       (1000) www-data    (33)      260 2020-07-10 08:02:46.000000 getlino-24.3.0/setup.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      313 2024-02-14 17:37:21.000000 getlino-24.3.0/tasks.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-15 12:34:28.147673 getlino-24.3.0/tests/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2021-03-02 11:04:28.000000 getlino-24.3.0/tests/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2106 2024-02-14 17:37:21.000000 getlino-24.3.0/tests/test_case.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)    10812 2024-02-14 17:37:21.000000 getlino-24.3.0/tests/test_docker.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      180 2024-02-14 17:37:21.000000 getlino-24.3.0/tests/test_docs.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      183 2024-02-14 17:37:21.000000 getlino-24.3.0/tests/test_packages.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-12 23:15:52.971992 getlino-24.4.0/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    34523 2021-04-07 12:56:36.000000 getlino-24.4.0/COPYING
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       59 2019-10-25 15:17:06.000000 getlino-24.4.0/MANIFEST.in
+-rw-r--r--   0 luc       (1000) www-data    (33)     1559 2024-04-12 23:15:52.971992 getlino-24.4.0/PKG-INFO
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      692 2021-06-11 08:29:48.000000 getlino-24.4.0/README.rst
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-12 23:15:52.967992 getlino-24.4.0/getlino/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      322 2024-02-14 17:37:21.000000 getlino-24.4.0/getlino/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      816 2024-02-14 17:37:21.000000 getlino-24.4.0/getlino/cli.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)    20445 2024-04-01 09:56:59.000000 getlino-24.4.0/getlino/configure.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)      971 2024-04-01 15:27:49.000000 getlino-24.4.0/getlino/list.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)     1788 2024-04-12 23:15:26.000000 getlino-24.4.0/getlino/setup_info.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)     7794 2024-03-11 13:29:19.000000 getlino-24.4.0/getlino/startproject.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)    25754 2024-04-01 09:53:27.000000 getlino-24.4.0/getlino/startsite.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-12 23:15:52.967992 getlino-24.4.0/getlino/templates/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      890 2021-02-12 13:40:30.000000 getlino-24.4.0/getlino/templates/apache.conf
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      214 2022-09-10 15:27:38.000000 getlino-24.4.0/getlino/templates/asgi.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)     1678 2024-02-22 15:57:56.000000 getlino-24.4.0/getlino/templates/daphne_supervisor.conf
+-rw-rw-r--   0 luc       (1000) www-data    (33)      852 2023-01-01 07:07:06.000000 getlino-24.4.0/getlino/templates/django_settings.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      371 2023-07-01 18:31:56.000000 getlino-24.4.0/getlino/templates/healthcheck.sh
+-rw-rw-r--   0 luc       (1000) www-data    (33)      308 2023-01-15 18:29:24.000000 getlino-24.4.0/getlino/templates/lino.ini
+-rwxrwxr-x   0 luc       (1000) www-data    (33)     2074 2022-09-15 06:25:41.000000 getlino-24.4.0/getlino/templates/make_snapshot.sh
+-rw-rw-r--   0 luc       (1000) www-data    (33)      329 2023-11-05 18:22:29.000000 getlino-24.4.0/getlino/templates/manage.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1671 2023-07-16 11:11:44.000000 getlino-24.4.0/getlino/templates/nginx.conf
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1543 2022-09-10 15:27:38.000000 getlino-24.4.0/getlino/templates/nginx_asgi.conf
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1558 2023-10-08 06:14:57.000000 getlino-24.4.0/getlino/templates/pull.sh
+-rw-rw-r--   0 luc       (1000) www-data    (33)     1472 2024-04-05 03:44:20.000000 getlino-24.4.0/getlino/templates/settings.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1361 2021-02-10 17:53:35.000000 getlino-24.4.0/getlino/templates/uwsgi.ini
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      664 2019-10-25 14:15:15.000000 getlino-24.4.0/getlino/templates/uwsgi_params
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      251 2019-10-25 14:30:31.000000 getlino-24.4.0/getlino/templates/wsgi.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)    20855 2024-03-30 09:04:06.000000 getlino-24.4.0/getlino/utils.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-12 23:15:52.971992 getlino-24.4.0/getlino.egg-info/
+-rw-r--r--   0 luc       (1000) www-data    (33)     1559 2024-04-12 23:15:52.000000 getlino-24.4.0/getlino.egg-info/PKG-INFO
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      983 2024-04-12 23:15:52.000000 getlino-24.4.0/getlino.egg-info/SOURCES.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2024-04-12 23:15:52.000000 getlino-24.4.0/getlino.egg-info/dependency_links.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       45 2024-04-12 23:15:52.000000 getlino-24.4.0/getlino.egg-info/entry_points.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2019-06-20 10:29:13.000000 getlino-24.4.0/getlino.egg-info/not-zip-safe
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       56 2024-04-12 23:15:52.000000 getlino-24.4.0/getlino.egg-info/requires.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        8 2024-04-12 23:15:52.000000 getlino-24.4.0/getlino.egg-info/top_level.txt
+-rw-rw-r--   0 luc       (1000) www-data    (33)       38 2024-04-12 23:15:52.971992 getlino-24.4.0/setup.cfg
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      260 2020-07-10 08:02:46.000000 getlino-24.4.0/setup.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      313 2024-02-14 17:37:21.000000 getlino-24.4.0/tasks.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-12 23:15:52.971992 getlino-24.4.0/tests/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2021-03-02 11:04:28.000000 getlino-24.4.0/tests/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2106 2024-02-14 17:37:21.000000 getlino-24.4.0/tests/test_case.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    10812 2024-02-14 17:37:21.000000 getlino-24.4.0/tests/test_docker.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      180 2024-02-14 17:37:21.000000 getlino-24.4.0/tests/test_docs.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      183 2024-02-14 17:37:21.000000 getlino-24.4.0/tests/test_packages.py
```

### Comparing `getlino-24.3.0/COPYING` & `getlino-24.4.0/COPYING`

 * *Files identical despite different names*

### Comparing `getlino-24.3.0/PKG-INFO` & `getlino-24.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getlino
-Version: 24.3.0
+Version: 24.4.0
 Summary: A command-line tool for installing Lino in different environments.
 Home-page: https://gitlab.com/lino-framework/getlino
 Author: Rumma & Ko Ltd
 Author-email: info@lino-framework.org
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `getlino-24.3.0/README.rst` & `getlino-24.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `getlino-24.3.0/getlino/cli.py` & `getlino-24.4.0/getlino/cli.py`

 * *Files identical despite different names*

### Comparing `getlino-24.3.0/getlino/configure.py` & `getlino-24.4.0/getlino/configure.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from os.path import join
 
 from .utils import CONFIG, CONF_FILES, DEFAULTSECTION
 from .utils import KNOWN_REPOS, DB_ENGINES, BATCH_HELP, FRONT_ENDS
 from .utils import Installer, ifroot, default_db_engine, resolve_db_engine
 from .utils import which_certbot
-from .utils import WEB_SERVERS, resolve_web_server
+from .utils import WEB_SERVERS, resolve_web_server, GITLAB_CI
 
 HEALTHCHECK_NAME = '/usr/local/bin/healthcheck.sh'
 
 CERTBOT_AUTO_RENEW = """\
 # generated by getlino
 0 0,12 * * * root python -c 'import random; import time; time.sleep(random.random() * 3600)' && {} renew
 """
@@ -81,15 +81,15 @@
     return -1
 }}
 """
 
 BASH_ALIASES_DEV = """
 alias pp='per_project'
 alias ci='inv ci'
-alias dt=doctest
+alias dt='doctest'
 """
 
 # The configure command will be decorated below. We cannot use decorators
 # because we define the list of options in CONFIGURE_OPTIONS because we need
 # that list also for asking questions using the help text.
 
 CONFIGURE_OPTIONS = []
@@ -200,15 +200,15 @@
 add('--admin-name', 'Joe Dow', "The full name of the server administrator")
 add('--admin-email', 'joe@example.com',
     "The email address of the server administrator")
 add('--time-zone', 'Europe/Brussels', "The TIME_ZONE to set on new sites")
 add('--linod/--no-linod', True, "Whether new sites use linod", root_only=True)
 add('--languages', 'en', "The languages to set on new sites")
 add('--front-end', 'lino_react.react', "The front end to use on new sites",
-    click.Choice([r.front_end for r in FRONT_ENDS]))
+    click.Choice(FRONT_ENDS.keys()))
 
 
 def configure(ctx, batch, sites_base, local_prefix, shared_env, repos_base,
               clone, webdav, backups_base, log_base, usergroup, supervisor_dir,
               env_link, repos_link, appy, redis, devtools, server_domain,
               https, ldap, monit, db_engine, db_port, db_host, db_user,
               db_password, admin_name, admin_email, time_zone, linod,
@@ -337,25 +337,25 @@
 
     if DEFAULTSECTION.getboolean('devtools'):
         i.apt_install("subversion graphviz sqlite3")
 
     if DEFAULTSECTION.getboolean('monit'):
         i.apt_install("monit")
 
-    if DEFAULTSECTION.getboolean('redis') and not int(
-            os.environ.get('GITLAB_CI', '0')):
+    if DEFAULTSECTION.getboolean('redis') and not GITLAB_CI:
         i.apt_install("redis-server")
         i.must_restart('redis')
 
-    if not int(os.environ.get('GITLAB_CI', '0')):
+    if not GITLAB_CI:
         i.apt_install(db_engine.apt_packages)
+
     if web_server:
         i.apt_install(web_server.apt_packages)
 
-    if db_engine.service and not int(os.environ.get("GITLAB_CI", "0")):
+    if db_engine.service and not GITLAB_CI:
         i.must_restart(db_engine.service)
 
     if appy:
         i.apt_install("libreoffice-common python3-uno")
         i.apt_install("tidy")
 
     if DEFAULTSECTION.getboolean('ldap'):
@@ -394,16 +394,15 @@
                     i.write_file(pth, content)
                     # i.runcmd('printf "%s\\n" "deb http://ftp.de.debian.org/debian buster-backports main" | sudo tee /etc/apt/sources.list.d/buster-backports.list')
                     # i.runcmd('echo "deb http://ftp.de.debian.org/debian buster-backports main" >> /etc/apt/sources.list.d/buster-backports.list')
 
     i.run_apt_install()
     i.restart_services()
 
-    if DEFAULTSECTION.get('db_user') and not int(
-            os.environ.get('GITLAB_CI', '0')):
+    if DEFAULTSECTION.get('db_user') and not GITLAB_CI:
         db_engine.setup_user(i, context)
 
     go_bases = []
 
     if clone:
         click.echo("Installing repositories for shared-env...")
         if not shared_env:
```

### Comparing `getlino-24.3.0/getlino/setup_info.py` & `getlino-24.4.0/getlino/setup_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 SETUP_INFO = dict(
     name='getlino',
-    version='24.3.0',
+    version='24.4.0',
     install_requires=[
         'click', 'virtualenv', 'jinja2', 'distro', 'synodal',
         'GitPython', 'rstgen'
     ],
     # tests_require=['docker', 'atelier'],
     # test_suite='tests',
     description=
```

### Comparing `getlino-24.3.0/getlino/startproject.py` & `getlino-24.4.0/getlino/startproject.py`

 * *Files identical despite different names*

### Comparing `getlino-24.3.0/getlino/startsite.py` & `getlino-24.4.0/getlino/startsite.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,20 +9,22 @@
 from logging import getLogger
 from urllib.parse import urlparse
 
 logger = getLogger(__file__)
 
 from os.path import join
 
+from synodal import REPOS_DICT, KNOWN_REPOS, FRONT_ENDS
 from .utils import KNOWN_REPOS, DEFAULTSECTION
-from .utils import DB_ENGINES, BATCH_HELP, REPOS_DICT, KNOWN_REPOS
+from .utils import DB_ENGINES, BATCH_HELP
 from .utils import Installer, ifroot, has_usergroup
 from .utils import default_db_engine, resolve_db_engine
 from .utils import which_certbot, resolve_web_server
 from .utils import JINJA_ENV
+from .utils import GITLAB_CI
 
 from configparser import NoOptionError, NoSectionError
 from rstgen.confparser import ConfigParser
 
 APPNAMES = [a.nickname for a in KNOWN_REPOS if a.settings_module]
 
 UWSGI_SUPERVISOR_CONF = """\
@@ -288,15 +290,15 @@
             raise click.ClickException(
                 "Invalid application nickname '{}'".format(appname))
         settings_module = app.settings_module
         if not settings_module:
             raise click.ClickException(
                 "{} is a library, not an application".format(appname))
 
-        front_end = REPOS_DICT.get(DEFAULTSECTION.get('front_end'), None)
+        front_end = FRONT_ENDS.get(DEFAULTSECTION.get('front_end'), None)
         if front_end is None:
             raise click.ClickException(
                 "Invalid front_end name '{}''".format(front_end))
 
         if dev_repos:
             for k in dev_repos.split():
                 repo = REPOS_DICT.get(k, None)
@@ -451,15 +453,15 @@
 
         if create_db and not batch:
             click.echo(
                 "User credentials (for {db_engine} on {db_host}:{db_port}):".
                 format(**context))
             db_user = click.prompt("- user name", default=db_user)
             db_password = click.prompt("- user password", default=db_password)
-            if not int(os.environ.get('GITLAB_CI', '0')):
+            if not GITLAB_CI:
                 db_port = click.prompt("- port", default=db_port)
             db_host = click.prompt("- host name", default=db_host)
 
         if not batch:
             secret_key = click.prompt("Site's secret key", default=secret_key)
 
         context.update({
@@ -621,19 +623,18 @@
 
         if i.jinja_write(avpth, conf_tpl, **context):
             with i.override_batch(True):
                 if i.check_overwrite(enpth):
                     os.symlink(avpth, enpth)
         i.must_restart(web_server.service)
 
-    if create_db and db_engine.needs_user:
-        if not shared_user and not int(os.environ.get('GITLAB_CI', '0')):
+    if create_db and db_engine.needs_user and not GITLAB_CI:
+        if not shared_user:
             db_engine.setup_user(i, context)
-        if not int(os.environ.get('GITLAB_CI', '0')):
-            db_engine.setup_database(i, prjname, db_user, db_host)
+        db_engine.setup_database(i, prjname, db_user, db_host)
 
     os.chdir(project_dir)
     i.run_in_env(envdir, "python manage.py install --noinput")
 
     if linod and not asgi_server and ifroot():
         i.write_file(join(project_dir, 'linod.sh'), LINOD_SH.format(**context))
         i.check_permissions(executable=True, writeable=False)
```

### Comparing `getlino-24.3.0/getlino/templates/apache.conf` & `getlino-24.4.0/getlino/templates/apache.conf`

 * *Files identical despite different names*

### Comparing `getlino-24.3.0/getlino/templates/daphne_supervisor.conf` & `getlino-24.4.0/getlino/templates/daphne_supervisor.conf`

 * *Files identical despite different names*

### Comparing `getlino-24.3.0/getlino/templates/django_settings.py` & `getlino-24.4.0/getlino/templates/django_settings.py`

 * *Files identical despite different names*

### Comparing `getlino-24.3.0/getlino/templates/make_snapshot.sh` & `getlino-24.4.0/getlino/templates/make_snapshot.sh`

 * *Files identical despite different names*

### Comparing `getlino-24.3.0/getlino/templates/nginx.conf` & `getlino-24.4.0/getlino/templates/nginx.conf`

 * *Files identical despite different names*

### Comparing `getlino-24.3.0/getlino/templates/nginx_asgi.conf` & `getlino-24.4.0/getlino/templates/nginx_asgi.conf`

 * *Files identical despite different names*

### Comparing `getlino-24.3.0/getlino/templates/pull.sh` & `getlino-24.4.0/getlino/templates/pull.sh`

 * *Files identical despite different names*

### Comparing `getlino-24.3.0/getlino/templates/settings.py` & `getlino-24.4.0/getlino/templates/settings.py`

 * *Files identical despite different names*

### Comparing `getlino-24.3.0/getlino/templates/uwsgi.ini` & `getlino-24.4.0/getlino/templates/uwsgi.ini`

 * *Files identical despite different names*

### Comparing `getlino-24.3.0/getlino/templates/uwsgi_params` & `getlino-24.4.0/getlino/templates/uwsgi_params`

 * *Files identical despite different names*

### Comparing `getlino-24.3.0/getlino/utils.py` & `getlino-24.4.0/getlino/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 import virtualenv
 from jinja2 import Environment, PackageLoader
 from synodal import REPOS_DICT, KNOWN_REPOS, FRONT_ENDS
 from .setup_info import SETUP_INFO
 
 JINJA_ENV = Environment(loader=PackageLoader('getlino', 'templates'))
 
+GITLAB_CI = os.environ.get("GITLAB_CI", "false") == "true"
+
 # currently getlino supports only nginx, maybe we might add other web servers
 # USE_NGINX = True
 
 BATCH_HELP = "Whether to run in batch mode, i.e. without asking any questions.  "\
              "Don't use this on a machine that is already being used."
 
 # note that we double curly braces because we will run format() on this string:
@@ -175,33 +177,33 @@
 class MySQL(DbEngine):
     name = 'mysql'
     service = 'mysql'
     # service = '/lib/systemd/system/mysql.service'
     default_port = "3306"
     if distro.id() == "debian":
         apt_packages = "mariadb-server libmariadb-dev-compat libmariadb-dev "\
-        "python-dev libffi-dev libssl-dev pkgconf"
+        "python3-dev libffi-dev libssl-dev pkgconf"
     else:
         apt_packages = "mysql-server mysql-client libmysqlclient-dev pkgconf"
     # apt_packages = "default-mysql-server default-libmysqlclient-dev"
     python_packages = "mysqlclient"
     needs_root = True
     needs_user = True
 
     # def __init__(self):
     #     super().__init__()
     #     # apt_packages = "mysql-server libmysqlclient-dev"
     #     # TODO: support different platforms (Debian, Ubuntu, Elementary, ...)
-    #     # apt_packages += " python-dev libffi-dev libssl-dev python-mysqldb"
+    #     # apt_packages += " python3-dev libffi-dev libssl-dev python-mysqldb"
     #     if distro.id() == "debian":
     #         # package name is mariadb but service name remains mysql
     #         # self.service = 'mariadb'
     #         self.apt_packages = "mariadb-server libmariadb-dev-compat libmariadb-dev "\
-    #             "python-dev libffi-dev libssl-dev"
-    #             # "python-dev libffi-dev libssl-dev python-mysqldb"
+    #             "python3-dev libffi-dev libssl-dev"
+    #             # "python3-dev libffi-dev libssl-dev python-mysqldb"
 
     def run(self, i, sqlcmd):
         # options = "" if i.batch else "-p"
         # return i.runcmd('sudo mysql -u root {} -e "{};"'.format(options, sqlcmd))
         return i.runcmd('mysql -e "{};"'.format(sqlcmd))
 
     def setup_user(self, i, context):
@@ -216,15 +218,15 @@
             i, "grant all PRIVILEGES on {database}.* to '{user}'@'{db_host}'".
             format(**locals()))
 
 
 class PostgreSQL(DbEngine):
     name = 'postgresql'
     service = 'postgresql'
-    apt_packages = "postgresql postgresql-contrib libpq-dev python-dev"
+    apt_packages = "postgresql postgresql-contrib libpq-dev python3-dev"
     python_packages = "psycopg2"
     # python_packages = "psycopg2-binary"
     default_port = "5432"
     needs_root = True
     needs_user = True
 
     def run(self, i, cmd):
```

### Comparing `getlino-24.3.0/getlino.egg-info/PKG-INFO` & `getlino-24.4.0/getlino.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getlino
-Version: 24.3.0
+Version: 24.4.0
 Summary: A command-line tool for installing Lino in different environments.
 Home-page: https://gitlab.com/lino-framework/getlino
 Author: Rumma & Ko Ltd
 Author-email: info@lino-framework.org
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `getlino-24.3.0/getlino.egg-info/SOURCES.txt` & `getlino-24.4.0/getlino.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `getlino-24.3.0/tests/test_case.py` & `getlino-24.4.0/tests/test_case.py`

 * *Files identical despite different names*

### Comparing `getlino-24.3.0/tests/test_docker.py` & `getlino-24.4.0/tests/test_docker.py`

 * *Files identical despite different names*

