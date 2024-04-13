# Comparing `tmp/baseweb-0.2.0.tar.gz` & `tmp/baseweb-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baseweb-0.2.0.tar", last modified: Wed Feb 28 20:29:02 2024, max compression
+gzip compressed data, was "baseweb-0.2.1.tar", last modified: Sat Apr 13 07:26:53 2024, max compression
```

## Comparing `baseweb-0.2.0.tar` & `baseweb-0.2.1.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-02-28 20:29:02.693119 baseweb-0.2.0/
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-02-28 20:29:02.679027 baseweb-0.2.0/.github/
--rw-r--r--   0 xtof       (501) staff       (20)      995 2024-02-18 12:58:44.000000 baseweb-0.2.0/.github/README.md
--rw-r--r--   0 xtof       (501) staff       (20)     1072 2024-01-17 08:54:40.000000 baseweb-0.2.0/LICENSE.txt
--rw-r--r--   0 xtof       (501) staff       (20)      189 2022-11-26 16:31:09.000000 baseweb-0.2.0/MANIFEST.in
--rw-r--r--   0 xtof       (501) staff       (20)     1933 2024-02-28 20:29:02.692876 baseweb-0.2.0/PKG-INFO
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-02-28 20:29:02.679876 baseweb-0.2.0/baseweb/
--rw-r--r--   0 xtof       (501) staff       (20)      232 2024-02-28 20:28:02.000000 baseweb-0.2.0/baseweb/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)     1455 2023-10-31 18:48:41.000000 baseweb-0.2.0/baseweb/config.py
--rw-r--r--   0 xtof       (501) staff       (20)     2006 2023-10-31 18:49:02.000000 baseweb-0.2.0/baseweb/interface.py
--rw-r--r--   0 xtof       (501) staff       (20)      331 2023-10-31 18:49:11.000000 baseweb-0.2.0/baseweb/rest.py
--rw-r--r--   0 xtof       (501) staff       (20)      841 2023-10-31 18:49:29.000000 baseweb-0.2.0/baseweb/security.py
--rw-r--r--   0 xtof       (501) staff       (20)      482 2023-10-31 18:49:59.000000 baseweb-0.2.0/baseweb/socketio.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-02-28 20:29:02.682590 baseweb-0.2.0/baseweb/static/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2022-08-27 14:55:53.000000 baseweb-0.2.0/baseweb/static/__init__.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-02-28 20:29:02.682895 baseweb-0.2.0/baseweb/static/css/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2022-08-27 14:55:53.000000 baseweb-0.2.0/baseweb/static/css/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)      287 2022-12-29 15:36:28.000000 baseweb-0.2.0/baseweb/static/css/main.css
--rw-rw-rw-   0 xtof       (501) staff       (20)     4773 2022-10-28 08:40:23.000000 baseweb-0.2.0/baseweb/static/css/process_diagram.css
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-02-28 20:29:02.683463 baseweb-0.2.0/baseweb/static/js/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2022-08-27 14:55:53.000000 baseweb-0.2.0/baseweb/static/js/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)      586 2023-05-03 12:25:47.000000 baseweb-0.2.0/baseweb/static/js/app.js
--rw-r--r--   0 xtof       (501) staff       (20)     1024 2024-02-28 19:30:19.000000 baseweb-0.2.0/baseweb/static/js/common.js
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-02-28 20:29:02.684430 baseweb-0.2.0/baseweb/static/js/components/
--rw-rw-rw-   0 xtof       (501) staff       (20)     8465 2023-01-12 13:14:07.000000 baseweb-0.2.0/baseweb/static/js/components/CollectionView.js
--rw-rw-rw-   0 xtof       (501) staff       (20)      730 2024-02-28 13:22:18.000000 baseweb-0.2.0/baseweb/static/js/components/LineChart.js
--rw-r--r--   0 xtof       (501) staff       (20)     4814 2022-12-29 15:51:31.000000 baseweb-0.2.0/baseweb/static/js/components/NavigationDrawer.js
--rw-r--r--   0 xtof       (501) staff       (20)      150 2024-02-17 17:20:33.000000 baseweb-0.2.0/baseweb/static/js/components/Page.js
--rw-r--r--   0 xtof       (501) staff       (20)      725 2024-02-17 17:25:08.000000 baseweb-0.2.0/baseweb/static/js/components/PageWithBanner.js
--rw-r--r--   0 xtof       (501) staff       (20)     1265 2024-02-17 17:29:54.000000 baseweb-0.2.0/baseweb/static/js/components/PageWithStatus.js
--rw-rw-rw-   0 xtof       (501) staff       (20)     1253 2024-02-28 20:13:23.000000 baseweb-0.2.0/baseweb/static/js/components/ProcessDiagram.js
--rw-r--r--   0 xtof       (501) staff       (20)        0 2022-08-27 14:55:53.000000 baseweb-0.2.0/baseweb/static/js/components/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)       88 2022-12-28 12:15:48.000000 baseweb-0.2.0/baseweb/static/js/router.js
--rw-r--r--   0 xtof       (501) staff       (20)      639 2024-02-28 19:00:45.000000 baseweb-0.2.0/baseweb/static/js/socketio.js
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-02-28 20:29:02.684523 baseweb-0.2.0/baseweb/static/vendor/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2022-08-27 14:55:53.000000 baseweb-0.2.0/baseweb/static/vendor/__init__.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-02-28 20:29:02.685395 baseweb-0.2.0/baseweb/static/vendor/css/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2022-08-27 14:55:53.000000 baseweb-0.2.0/baseweb/static/vendor/css/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)    13490 2022-08-27 14:55:53.000000 baseweb-0.2.0/baseweb/static/vendor/css/bootstrap-datetimepicker.css
--rw-r--r--   0 xtof       (501) staff       (20)     1571 2022-11-30 17:41:16.000000 baseweb-0.2.0/baseweb/static/vendor/css/highlight.js.github.css
--rw-r--r--   0 xtof       (501) staff       (20)     1363 2022-08-27 14:55:53.000000 baseweb-0.2.0/baseweb/static/vendor/css/roboto-material-icons.css
--rw-r--r--   0 xtof       (501) staff       (20)     9800 2022-08-27 14:55:53.000000 baseweb-0.2.0/baseweb/static/vendor/css/vfg.css
--rw-r--r--   0 xtof       (501) staff       (20)     7238 2022-08-27 14:55:53.000000 baseweb-0.2.0/baseweb/static/vendor/css/vue-multiselect.min.css
--rw-r--r--   0 xtof       (501) staff       (20)   210148 2022-12-25 18:19:16.000000 baseweb-0.2.0/baseweb/static/vendor/css/vuetify.min.css
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-02-28 20:29:02.686298 baseweb-0.2.0/baseweb/static/vendor/fonts/
--rw-r--r--   0 xtof       (501) staff       (20)    35588 2022-08-27 14:55:53.000000 baseweb-0.2.0/baseweb/static/vendor/fonts/KFOlCnqEu92Fr1MmEU9fBBc9.ttf
--rw-r--r--   0 xtof       (501) staff       (20)    35468 2022-12-28 19:16:33.000000 baseweb-0.2.0/baseweb/static/vendor/fonts/KFOlCnqEu92Fr1MmSU5fBBc9.ttf
--rw-r--r--   0 xtof       (501) staff       (20)    35236 2022-08-27 14:55:53.000000 baseweb-0.2.0/baseweb/static/vendor/fonts/KFOlCnqEu92Fr1MmWUlfBBc9.ttf
--rw-r--r--   0 xtof       (501) staff       (20)    35408 2022-08-27 14:55:53.000000 baseweb-0.2.0/baseweb/static/vendor/fonts/KFOmCnqEu92Fr1Mu4mxP.ttf
--rw-r--r--   0 xtof       (501) staff       (20)        0 2022-08-27 14:55:53.000000 baseweb-0.2.0/baseweb/static/vendor/fonts/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)    49168 2022-08-27 14:55:53.000000 baseweb-0.2.0/baseweb/static/vendor/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-02-28 20:29:02.691661 baseweb-0.2.0/baseweb/static/vendor/js/
--rw-r--r--   0 xtof       (501) staff       (20)   157843 2022-12-29 15:35:01.000000 baseweb-0.2.0/baseweb/static/vendor/js/Chart.min.js
--rw-r--r--   0 xtof       (501) staff       (20)        0 2022-08-27 14:55:53.000000 baseweb-0.2.0/baseweb/static/vendor/js/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)    39239 2022-08-27 14:55:53.000000 baseweb-0.2.0/baseweb/static/vendor/js/bootstrap-datetimepicker.min.js
--rwxr-xr-x   0 xtof       (501) staff       (20)    37045 2022-08-27 14:55:53.000000 baseweb-0.2.0/baseweb/static/vendor/js/bootstrap.min.js
--rw-r--r--   0 xtof       (501) staff       (20)   120762 2022-11-30 17:19:12.000000 baseweb-0.2.0/baseweb/static/vendor/js/highlight.min.js
--rw-r--r--   0 xtof       (501) staff       (20)     2730 2022-08-27 14:55:53.000000 baseweb-0.2.0/baseweb/static/vendor/js/html5shiv.min.js
--rw-r--r--   0 xtof       (501) staff       (20)    40413 2022-08-27 14:55:53.000000 baseweb-0.2.0/baseweb/static/vendor/js/index.js.map
--rwxr-xr-x   0 xtof       (501) staff       (20)    97163 2022-08-27 14:55:53.000000 baseweb-0.2.0/baseweb/static/vendor/js/jquery.min.js
--rw-r--r--   0 xtof       (501) staff       (20)    51465 2022-08-27 14:55:53.000000 baseweb-0.2.0/baseweb/static/vendor/js/moment.min.js
--rw-r--r--   0 xtof       (501) staff       (20)     4377 2022-08-27 14:55:53.000000 baseweb-0.2.0/baseweb/static/vendor/js/respond.min.js
--rw-r--r--   0 xtof       (501) staff       (20)   146329 2022-08-27 16:18:42.000000 baseweb-0.2.0/baseweb/static/vendor/js/socket.io.min.js.map
--rw-r--r--   0 xtof       (501) staff       (20)    43622 2022-08-27 16:18:54.000000 baseweb-0.2.0/baseweb/static/vendor/js/socket.io.slim.js
--rw-r--r--   0 xtof       (501) staff       (20)     3526 2022-08-27 14:55:54.000000 baseweb-0.2.0/baseweb/static/vendor/js/vue-chartjs.min.js
--rw-r--r--   0 xtof       (501) staff       (20)    24240 2022-08-27 14:55:54.000000 baseweb-0.2.0/baseweb/static/vendor/js/vue-chartjs.min.js.map
--rw-r--r--   0 xtof       (501) staff       (20)   115645 2022-08-27 14:55:54.000000 baseweb-0.2.0/baseweb/static/vendor/js/vue-form-generator.min.js
--rw-r--r--   0 xtof       (501) staff       (20)    43084 2022-08-27 14:55:54.000000 baseweb-0.2.0/baseweb/static/vendor/js/vue-multiselect.min.js
--rw-r--r--   0 xtof       (501) staff       (20)    30139 2022-08-27 14:55:54.000000 baseweb-0.2.0/baseweb/static/vendor/js/vue-notification.js
--rw-r--r--   0 xtof       (501) staff       (20)    65289 2022-11-26 16:27:44.000000 baseweb-0.2.0/baseweb/static/vendor/js/vue-router.js
--rw-r--r--   0 xtof       (501) staff       (20)   433738 2022-12-25 18:21:14.000000 baseweb-0.2.0/baseweb/static/vendor/js/vue.js
--rw-r--r--   0 xtof       (501) staff       (20)  1101513 2022-12-25 18:34:51.000000 baseweb-0.2.0/baseweb/static/vendor/js/vuetify.js
--rw-r--r--   0 xtof       (501) staff       (20)  1102711 2022-12-25 18:34:51.000000 baseweb-0.2.0/baseweb/static/vendor/js/vuetify.js.map
--rw-r--r--   0 xtof       (501) staff       (20)    25628 2022-11-26 16:27:44.000000 baseweb-0.2.0/baseweb/static/vendor/js/vuex.js
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-02-28 20:29:02.692400 baseweb-0.2.0/baseweb/templates/
--rw-r--r--   0 xtof       (501) staff       (20)      270 2022-08-27 14:55:54.000000 baseweb-0.2.0/baseweb/templates/404.html
--rw-r--r--   0 xtof       (501) staff       (20)        0 2022-08-27 14:55:54.000000 baseweb-0.2.0/baseweb/templates/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)     5798 2024-02-28 18:59:45.000000 baseweb-0.2.0/baseweb/templates/main.html
--rw-r--r--   0 xtof       (501) staff       (20)     1099 2022-12-28 10:02:38.000000 baseweb-0.2.0/baseweb/templates/manifest.json
--rw-r--r--   0 xtof       (501) staff       (20)      145 2022-12-28 11:17:50.000000 baseweb-0.2.0/baseweb/templates/store.js
--rw-r--r--   0 xtof       (501) staff       (20)      171 2023-10-31 18:50:47.000000 baseweb-0.2.0/baseweb/web.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-02-28 20:29:02.679995 baseweb-0.2.0/baseweb-demo/
--rw-r--r--   0 xtof       (501) staff       (20)     2110 2024-02-28 19:16:23.000000 baseweb-0.2.0/baseweb-demo/__init__.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-02-28 20:29:02.680114 baseweb-0.2.0/baseweb-demo/pages/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2022-11-26 16:32:12.000000 baseweb-0.2.0/baseweb-demo/pages/__init__.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-02-28 20:29:02.680206 baseweb-0.2.0/baseweb-demo/pages/components/
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-02-28 20:29:02.680310 baseweb-0.2.0/baseweb-demo/pages/components/CollectionView/
--rw-r--r--   0 xtof       (501) staff       (20)     1924 2024-02-18 13:05:47.000000 baseweb-0.2.0/baseweb-demo/pages/components/CollectionView/__init__.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-02-28 20:29:02.680465 baseweb-0.2.0/baseweb-demo/pages/components/LineChart/
--rw-r--r--   0 xtof       (501) staff       (20)      164 2024-02-18 16:47:27.000000 baseweb-0.2.0/baseweb-demo/pages/components/LineChart/__init__.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-02-28 20:29:02.680669 baseweb-0.2.0/baseweb-demo/pages/components/PageWithBanner/
--rw-r--r--   0 xtof       (501) staff       (20)      169 2022-12-28 10:58:50.000000 baseweb-0.2.0/baseweb-demo/pages/components/PageWithBanner/__init__.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-02-28 20:29:02.680816 baseweb-0.2.0/baseweb-demo/pages/components/PageWithStatus/
--rw-r--r--   0 xtof       (501) staff       (20)      169 2024-02-17 17:14:44.000000 baseweb-0.2.0/baseweb-demo/pages/components/PageWithStatus/__init__.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-02-28 20:29:02.680945 baseweb-0.2.0/baseweb-demo/pages/components/ProcessDiagram/
--rw-r--r--   0 xtof       (501) staff       (20)      244 2024-02-28 20:07:49.000000 baseweb-0.2.0/baseweb-demo/pages/components/ProcessDiagram/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)        0 2022-12-28 10:55:34.000000 baseweb-0.2.0/baseweb-demo/pages/components/__init__.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-02-28 20:29:02.681074 baseweb-0.2.0/baseweb-demo/pages/index/
--rw-r--r--   0 xtof       (501) staff       (20)     1313 2024-02-18 13:06:35.000000 baseweb-0.2.0/baseweb-demo/pages/index/__init__.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-02-28 20:29:02.681205 baseweb-0.2.0/baseweb-demo/pages/page1/
--rw-r--r--   0 xtof       (501) staff       (20)      160 2022-11-26 16:32:12.000000 baseweb-0.2.0/baseweb-demo/pages/page1/__init__.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-02-28 20:29:02.681329 baseweb-0.2.0/baseweb-demo/pages/page2/
--rw-r--r--   0 xtof       (501) staff       (20)      160 2022-11-26 16:32:12.000000 baseweb-0.2.0/baseweb-demo/pages/page2/__init__.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-02-28 20:29:02.681451 baseweb-0.2.0/baseweb-demo/pages/page3/
--rw-r--r--   0 xtof       (501) staff       (20)      311 2023-04-29 12:05:47.000000 baseweb-0.2.0/baseweb-demo/pages/page3/__init__.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-02-28 20:29:02.681572 baseweb-0.2.0/baseweb-demo/pages/page4/
--rw-r--r--   0 xtof       (501) staff       (20)      160 2022-12-28 13:04:06.000000 baseweb-0.2.0/baseweb-demo/pages/page4/__init__.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-02-28 20:29:02.681689 baseweb-0.2.0/baseweb-demo/pages/page5/
--rw-r--r--   0 xtof       (501) staff       (20)      160 2022-12-29 15:06:11.000000 baseweb-0.2.0/baseweb-demo/pages/page5/__init__.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-02-28 20:29:02.681809 baseweb-0.2.0/baseweb-demo/pages/protected_page/
--rw-r--r--   0 xtof       (501) staff       (20)     1227 2024-02-18 13:07:07.000000 baseweb-0.2.0/baseweb-demo/pages/protected_page/__init__.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-02-28 20:29:02.681933 baseweb-0.2.0/baseweb-demo/static/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2022-12-25 18:52:18.000000 baseweb-0.2.0/baseweb-demo/static/__init__.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-02-28 20:29:02.682479 baseweb-0.2.0/baseweb.egg-info/
--rw-r--r--   0 xtof       (501) staff       (20)     1933 2024-02-28 20:29:02.000000 baseweb-0.2.0/baseweb.egg-info/PKG-INFO
--rw-r--r--   0 xtof       (501) staff       (20)     3412 2024-02-28 20:29:02.000000 baseweb-0.2.0/baseweb.egg-info/SOURCES.txt
--rw-r--r--   0 xtof       (501) staff       (20)        1 2024-02-28 20:29:02.000000 baseweb-0.2.0/baseweb.egg-info/dependency_links.txt
--rw-r--r--   0 xtof       (501) staff       (20)      131 2024-02-28 20:29:02.000000 baseweb-0.2.0/baseweb.egg-info/requires.txt
--rw-r--r--   0 xtof       (501) staff       (20)       21 2024-02-28 20:29:02.000000 baseweb-0.2.0/baseweb.egg-info/top_level.txt
--rw-r--r--   0 xtof       (501) staff       (20)       38 2024-02-28 20:29:02.693166 baseweb-0.2.0/setup.cfg
--rw-r--r--   0 xtof       (501) staff       (20)     1724 2024-02-18 13:23:17.000000 baseweb-0.2.0/setup.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-02-28 20:29:02.692545 baseweb-0.2.0/tests/
--rw-r--r--   0 xtof       (501) staff       (20)       84 2023-10-31 18:51:49.000000 baseweb-0.2.0/tests/test_placeholder.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-13 07:26:52.999029 baseweb-0.2.1/
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-13 07:26:52.970221 baseweb-0.2.1/.github/
+-rw-r--r--   0 xtof       (501) staff       (20)      995 2024-02-18 12:58:44.000000 baseweb-0.2.1/.github/README.md
+-rw-r--r--   0 xtof       (501) staff       (20)     1072 2024-01-17 08:54:40.000000 baseweb-0.2.1/LICENSE.txt
+-rw-r--r--   0 xtof       (501) staff       (20)      189 2022-11-26 16:31:09.000000 baseweb-0.2.1/MANIFEST.in
+-rw-r--r--   0 xtof       (501) staff       (20)     1901 2024-04-13 07:26:52.998816 baseweb-0.2.1/PKG-INFO
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-13 07:26:52.971545 baseweb-0.2.1/baseweb/
+-rw-r--r--   0 xtof       (501) staff       (20)      232 2024-04-13 07:25:45.000000 baseweb-0.2.1/baseweb/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)     1455 2023-10-31 18:48:41.000000 baseweb-0.2.1/baseweb/config.py
+-rw-r--r--   0 xtof       (501) staff       (20)     2006 2023-10-31 18:49:02.000000 baseweb-0.2.1/baseweb/interface.py
+-rw-r--r--   0 xtof       (501) staff       (20)      331 2023-10-31 18:49:11.000000 baseweb-0.2.1/baseweb/rest.py
+-rw-r--r--   0 xtof       (501) staff       (20)      841 2023-10-31 18:49:29.000000 baseweb-0.2.1/baseweb/security.py
+-rw-r--r--   0 xtof       (501) staff       (20)      482 2023-10-31 18:49:59.000000 baseweb-0.2.1/baseweb/socketio.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-13 07:26:52.975781 baseweb-0.2.1/baseweb/static/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2022-08-27 14:55:53.000000 baseweb-0.2.1/baseweb/static/__init__.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-13 07:26:52.976270 baseweb-0.2.1/baseweb/static/css/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2022-08-27 14:55:53.000000 baseweb-0.2.1/baseweb/static/css/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)      287 2022-12-29 15:36:28.000000 baseweb-0.2.1/baseweb/static/css/main.css
+-rw-rw-rw-   0 xtof       (501) staff       (20)     4773 2022-10-28 08:40:23.000000 baseweb-0.2.1/baseweb/static/css/process_diagram.css
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-13 07:26:52.977448 baseweb-0.2.1/baseweb/static/js/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2022-08-27 14:55:53.000000 baseweb-0.2.1/baseweb/static/js/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)      586 2023-05-03 12:25:47.000000 baseweb-0.2.1/baseweb/static/js/app.js
+-rw-r--r--   0 xtof       (501) staff       (20)     1024 2024-02-28 19:30:19.000000 baseweb-0.2.1/baseweb/static/js/common.js
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-13 07:26:52.979745 baseweb-0.2.1/baseweb/static/js/components/
+-rw-rw-rw-   0 xtof       (501) staff       (20)     8465 2023-01-12 13:14:07.000000 baseweb-0.2.1/baseweb/static/js/components/CollectionView.js
+-rw-rw-rw-   0 xtof       (501) staff       (20)      730 2024-02-28 13:22:18.000000 baseweb-0.2.1/baseweb/static/js/components/LineChart.js
+-rw-r--r--   0 xtof       (501) staff       (20)     4814 2022-12-29 15:51:31.000000 baseweb-0.2.1/baseweb/static/js/components/NavigationDrawer.js
+-rw-r--r--   0 xtof       (501) staff       (20)      150 2024-02-17 17:20:33.000000 baseweb-0.2.1/baseweb/static/js/components/Page.js
+-rw-r--r--   0 xtof       (501) staff       (20)      725 2024-02-17 17:25:08.000000 baseweb-0.2.1/baseweb/static/js/components/PageWithBanner.js
+-rw-r--r--   0 xtof       (501) staff       (20)     1265 2024-02-17 17:29:54.000000 baseweb-0.2.1/baseweb/static/js/components/PageWithStatus.js
+-rw-rw-rw-   0 xtof       (501) staff       (20)     1253 2024-02-28 20:13:23.000000 baseweb-0.2.1/baseweb/static/js/components/ProcessDiagram.js
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2022-08-27 14:55:53.000000 baseweb-0.2.1/baseweb/static/js/components/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)       88 2022-12-28 12:15:48.000000 baseweb-0.2.1/baseweb/static/js/router.js
+-rw-r--r--   0 xtof       (501) staff       (20)      639 2024-02-28 19:00:45.000000 baseweb-0.2.1/baseweb/static/js/socketio.js
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-13 07:26:52.979867 baseweb-0.2.1/baseweb/static/vendor/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2022-08-27 14:55:53.000000 baseweb-0.2.1/baseweb/static/vendor/__init__.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-13 07:26:52.981379 baseweb-0.2.1/baseweb/static/vendor/css/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2022-08-27 14:55:53.000000 baseweb-0.2.1/baseweb/static/vendor/css/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)    13490 2022-08-27 14:55:53.000000 baseweb-0.2.1/baseweb/static/vendor/css/bootstrap-datetimepicker.css
+-rw-r--r--   0 xtof       (501) staff       (20)     1571 2022-11-30 17:41:16.000000 baseweb-0.2.1/baseweb/static/vendor/css/highlight.js.github.css
+-rw-r--r--   0 xtof       (501) staff       (20)     1363 2022-08-27 14:55:53.000000 baseweb-0.2.1/baseweb/static/vendor/css/roboto-material-icons.css
+-rw-r--r--   0 xtof       (501) staff       (20)     9800 2022-08-27 14:55:53.000000 baseweb-0.2.1/baseweb/static/vendor/css/vfg.css
+-rw-r--r--   0 xtof       (501) staff       (20)     7238 2022-08-27 14:55:53.000000 baseweb-0.2.1/baseweb/static/vendor/css/vue-multiselect.min.css
+-rw-r--r--   0 xtof       (501) staff       (20)   210148 2022-12-25 18:19:16.000000 baseweb-0.2.1/baseweb/static/vendor/css/vuetify.min.css
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-13 07:26:52.983751 baseweb-0.2.1/baseweb/static/vendor/fonts/
+-rw-r--r--   0 xtof       (501) staff       (20)    35588 2022-08-27 14:55:53.000000 baseweb-0.2.1/baseweb/static/vendor/fonts/KFOlCnqEu92Fr1MmEU9fBBc9.ttf
+-rw-r--r--   0 xtof       (501) staff       (20)    35468 2022-12-28 19:16:33.000000 baseweb-0.2.1/baseweb/static/vendor/fonts/KFOlCnqEu92Fr1MmSU5fBBc9.ttf
+-rw-r--r--   0 xtof       (501) staff       (20)    35236 2022-08-27 14:55:53.000000 baseweb-0.2.1/baseweb/static/vendor/fonts/KFOlCnqEu92Fr1MmWUlfBBc9.ttf
+-rw-r--r--   0 xtof       (501) staff       (20)    35408 2022-08-27 14:55:53.000000 baseweb-0.2.1/baseweb/static/vendor/fonts/KFOmCnqEu92Fr1Mu4mxP.ttf
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2022-08-27 14:55:53.000000 baseweb-0.2.1/baseweb/static/vendor/fonts/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)    49168 2022-08-27 14:55:53.000000 baseweb-0.2.1/baseweb/static/vendor/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-13 07:26:52.996333 baseweb-0.2.1/baseweb/static/vendor/js/
+-rw-r--r--   0 xtof       (501) staff       (20)   157843 2022-12-29 15:35:01.000000 baseweb-0.2.1/baseweb/static/vendor/js/Chart.min.js
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2022-08-27 14:55:53.000000 baseweb-0.2.1/baseweb/static/vendor/js/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)    39239 2022-08-27 14:55:53.000000 baseweb-0.2.1/baseweb/static/vendor/js/bootstrap-datetimepicker.min.js
+-rwxr-xr-x   0 xtof       (501) staff       (20)    37045 2022-08-27 14:55:53.000000 baseweb-0.2.1/baseweb/static/vendor/js/bootstrap.min.js
+-rw-r--r--   0 xtof       (501) staff       (20)   120762 2022-11-30 17:19:12.000000 baseweb-0.2.1/baseweb/static/vendor/js/highlight.min.js
+-rw-r--r--   0 xtof       (501) staff       (20)     2730 2022-08-27 14:55:53.000000 baseweb-0.2.1/baseweb/static/vendor/js/html5shiv.min.js
+-rw-r--r--   0 xtof       (501) staff       (20)    40413 2022-08-27 14:55:53.000000 baseweb-0.2.1/baseweb/static/vendor/js/index.js.map
+-rwxr-xr-x   0 xtof       (501) staff       (20)    97163 2022-08-27 14:55:53.000000 baseweb-0.2.1/baseweb/static/vendor/js/jquery.min.js
+-rw-r--r--   0 xtof       (501) staff       (20)    51465 2022-08-27 14:55:53.000000 baseweb-0.2.1/baseweb/static/vendor/js/moment.min.js
+-rw-r--r--   0 xtof       (501) staff       (20)     4377 2022-08-27 14:55:53.000000 baseweb-0.2.1/baseweb/static/vendor/js/respond.min.js
+-rw-r--r--   0 xtof       (501) staff       (20)   146329 2022-08-27 16:18:42.000000 baseweb-0.2.1/baseweb/static/vendor/js/socket.io.min.js.map
+-rw-r--r--   0 xtof       (501) staff       (20)    43622 2022-08-27 16:18:54.000000 baseweb-0.2.1/baseweb/static/vendor/js/socket.io.slim.js
+-rw-r--r--   0 xtof       (501) staff       (20)     3526 2022-08-27 14:55:54.000000 baseweb-0.2.1/baseweb/static/vendor/js/vue-chartjs.min.js
+-rw-r--r--   0 xtof       (501) staff       (20)    24240 2022-08-27 14:55:54.000000 baseweb-0.2.1/baseweb/static/vendor/js/vue-chartjs.min.js.map
+-rw-r--r--   0 xtof       (501) staff       (20)   115645 2022-08-27 14:55:54.000000 baseweb-0.2.1/baseweb/static/vendor/js/vue-form-generator.min.js
+-rw-r--r--   0 xtof       (501) staff       (20)    43084 2022-08-27 14:55:54.000000 baseweb-0.2.1/baseweb/static/vendor/js/vue-multiselect.min.js
+-rw-r--r--   0 xtof       (501) staff       (20)    30139 2022-08-27 14:55:54.000000 baseweb-0.2.1/baseweb/static/vendor/js/vue-notification.js
+-rw-r--r--   0 xtof       (501) staff       (20)    65289 2022-11-26 16:27:44.000000 baseweb-0.2.1/baseweb/static/vendor/js/vue-router.js
+-rw-r--r--   0 xtof       (501) staff       (20)   433738 2022-12-25 18:21:14.000000 baseweb-0.2.1/baseweb/static/vendor/js/vue.js
+-rw-r--r--   0 xtof       (501) staff       (20)  1101513 2022-12-25 18:34:51.000000 baseweb-0.2.1/baseweb/static/vendor/js/vuetify.js
+-rw-r--r--   0 xtof       (501) staff       (20)  1102711 2022-12-25 18:34:51.000000 baseweb-0.2.1/baseweb/static/vendor/js/vuetify.js.map
+-rw-r--r--   0 xtof       (501) staff       (20)    25628 2022-11-26 16:27:44.000000 baseweb-0.2.1/baseweb/static/vendor/js/vuex.js
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-13 07:26:52.998187 baseweb-0.2.1/baseweb/templates/
+-rw-r--r--   0 xtof       (501) staff       (20)      270 2022-08-27 14:55:54.000000 baseweb-0.2.1/baseweb/templates/404.html
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2022-08-27 14:55:54.000000 baseweb-0.2.1/baseweb/templates/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)     5798 2024-02-28 18:59:45.000000 baseweb-0.2.1/baseweb/templates/main.html
+-rw-r--r--   0 xtof       (501) staff       (20)     1099 2022-12-28 10:02:38.000000 baseweb-0.2.1/baseweb/templates/manifest.json
+-rw-r--r--   0 xtof       (501) staff       (20)      145 2022-12-28 11:17:50.000000 baseweb-0.2.1/baseweb/templates/store.js
+-rw-r--r--   0 xtof       (501) staff       (20)      171 2023-10-31 18:50:47.000000 baseweb-0.2.1/baseweb/web.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-13 07:26:52.971776 baseweb-0.2.1/baseweb-demo/
+-rw-r--r--   0 xtof       (501) staff       (20)     2110 2024-02-28 19:16:23.000000 baseweb-0.2.1/baseweb-demo/__init__.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-13 07:26:52.972012 baseweb-0.2.1/baseweb-demo/pages/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2022-11-26 16:32:12.000000 baseweb-0.2.1/baseweb-demo/pages/__init__.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-13 07:26:52.972110 baseweb-0.2.1/baseweb-demo/pages/components/
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-13 07:26:52.972208 baseweb-0.2.1/baseweb-demo/pages/components/CollectionView/
+-rw-r--r--   0 xtof       (501) staff       (20)     1924 2024-02-18 13:05:47.000000 baseweb-0.2.1/baseweb-demo/pages/components/CollectionView/__init__.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-13 07:26:52.972469 baseweb-0.2.1/baseweb-demo/pages/components/LineChart/
+-rw-r--r--   0 xtof       (501) staff       (20)      164 2024-02-18 16:47:27.000000 baseweb-0.2.1/baseweb-demo/pages/components/LineChart/__init__.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-13 07:26:52.972700 baseweb-0.2.1/baseweb-demo/pages/components/PageWithBanner/
+-rw-r--r--   0 xtof       (501) staff       (20)      169 2022-12-28 10:58:50.000000 baseweb-0.2.1/baseweb-demo/pages/components/PageWithBanner/__init__.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-13 07:26:52.972936 baseweb-0.2.1/baseweb-demo/pages/components/PageWithStatus/
+-rw-r--r--   0 xtof       (501) staff       (20)      169 2024-02-17 17:14:44.000000 baseweb-0.2.1/baseweb-demo/pages/components/PageWithStatus/__init__.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-13 07:26:52.973166 baseweb-0.2.1/baseweb-demo/pages/components/ProcessDiagram/
+-rw-r--r--   0 xtof       (501) staff       (20)      244 2024-02-28 20:07:49.000000 baseweb-0.2.1/baseweb-demo/pages/components/ProcessDiagram/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2022-12-28 10:55:34.000000 baseweb-0.2.1/baseweb-demo/pages/components/__init__.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-13 07:26:52.973424 baseweb-0.2.1/baseweb-demo/pages/index/
+-rw-r--r--   0 xtof       (501) staff       (20)     1313 2024-02-18 13:06:35.000000 baseweb-0.2.1/baseweb-demo/pages/index/__init__.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-13 07:26:52.973663 baseweb-0.2.1/baseweb-demo/pages/page1/
+-rw-r--r--   0 xtof       (501) staff       (20)      160 2022-11-26 16:32:12.000000 baseweb-0.2.1/baseweb-demo/pages/page1/__init__.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-13 07:26:52.973896 baseweb-0.2.1/baseweb-demo/pages/page2/
+-rw-r--r--   0 xtof       (501) staff       (20)      160 2022-11-26 16:32:12.000000 baseweb-0.2.1/baseweb-demo/pages/page2/__init__.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-13 07:26:52.974085 baseweb-0.2.1/baseweb-demo/pages/page3/
+-rw-r--r--   0 xtof       (501) staff       (20)      311 2023-04-29 12:05:47.000000 baseweb-0.2.1/baseweb-demo/pages/page3/__init__.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-13 07:26:52.974313 baseweb-0.2.1/baseweb-demo/pages/page4/
+-rw-r--r--   0 xtof       (501) staff       (20)      160 2022-12-28 13:04:06.000000 baseweb-0.2.1/baseweb-demo/pages/page4/__init__.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-13 07:26:52.974568 baseweb-0.2.1/baseweb-demo/pages/page5/
+-rw-r--r--   0 xtof       (501) staff       (20)      160 2022-12-29 15:06:11.000000 baseweb-0.2.1/baseweb-demo/pages/page5/__init__.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-13 07:26:52.974800 baseweb-0.2.1/baseweb-demo/pages/protected_page/
+-rw-r--r--   0 xtof       (501) staff       (20)     1227 2024-02-18 13:07:07.000000 baseweb-0.2.1/baseweb-demo/pages/protected_page/__init__.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-13 07:26:52.975042 baseweb-0.2.1/baseweb-demo/static/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2022-12-25 18:52:18.000000 baseweb-0.2.1/baseweb-demo/static/__init__.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-13 07:26:52.975654 baseweb-0.2.1/baseweb.egg-info/
+-rw-r--r--   0 xtof       (501) staff       (20)     1901 2024-04-13 07:26:52.000000 baseweb-0.2.1/baseweb.egg-info/PKG-INFO
+-rw-r--r--   0 xtof       (501) staff       (20)     3412 2024-04-13 07:26:52.000000 baseweb-0.2.1/baseweb.egg-info/SOURCES.txt
+-rw-r--r--   0 xtof       (501) staff       (20)        1 2024-04-13 07:26:52.000000 baseweb-0.2.1/baseweb.egg-info/dependency_links.txt
+-rw-r--r--   0 xtof       (501) staff       (20)      114 2024-04-13 07:26:52.000000 baseweb-0.2.1/baseweb.egg-info/requires.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       21 2024-04-13 07:26:52.000000 baseweb-0.2.1/baseweb.egg-info/top_level.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       38 2024-04-13 07:26:52.999069 baseweb-0.2.1/setup.cfg
+-rw-r--r--   0 xtof       (501) staff       (20)     1702 2024-04-13 07:23:18.000000 baseweb-0.2.1/setup.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-13 07:26:52.998422 baseweb-0.2.1/tests/
+-rw-r--r--   0 xtof       (501) staff       (20)       84 2023-10-31 18:51:49.000000 baseweb-0.2.1/tests/test_placeholder.py
```

### Comparing `baseweb-0.2.0/.github/README.md` & `baseweb-0.2.1/.github/README.md`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.0/LICENSE.txt` & `baseweb-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.0/PKG-INFO` & `baseweb-0.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baseweb
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Pythonic base for building interactive web applications
 Home-page: https://github.com/christophevg/baseweb
 Author: Christophe VG
 License: MIT
 Keywords: Flask Vue REST SocketIO
 Classifier: Environment :: Web Environment
 Classifier: Development Status :: 4 - Beta
@@ -20,15 +20,14 @@
 Requires-Dist: Flask-SocketIO
 Requires-Dist: python-dotenv
 Requires-Dist: websocket-client
 Requires-Dist: python-engineio
 Requires-Dist: python-socketio
 Requires-Dist: dotmap
 Requires-Dist: pyfiglet
-Requires-Dist: dnspython==2.5.0
 
 # baseweb
 
 > A Pythonic base for building interactive web applications
 
 [![Latest Version on PyPI](https://img.shields.io/pypi/v/baseweb.svg)](https://pypi.python.org/pypi/baseweb/)
 [![Supported Implementations](https://img.shields.io/pypi/pyversions/baseweb.svg)](https://pypi.python.org/pypi/baseweb/)
```

### Comparing `baseweb-0.2.0/baseweb/config.py` & `baseweb-0.2.1/baseweb/config.py`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.0/baseweb/interface.py` & `baseweb-0.2.1/baseweb/interface.py`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.0/baseweb/security.py` & `baseweb-0.2.1/baseweb/security.py`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.0/baseweb/static/css/process_diagram.css` & `baseweb-0.2.1/baseweb/static/css/process_diagram.css`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.0/baseweb/static/js/app.js` & `baseweb-0.2.1/baseweb/static/js/app.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.0/baseweb/static/js/common.js` & `baseweb-0.2.1/baseweb/static/js/common.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.0/baseweb/static/js/components/CollectionView.js` & `baseweb-0.2.1/baseweb/static/js/components/CollectionView.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.0/baseweb/static/js/components/LineChart.js` & `baseweb-0.2.1/baseweb/static/js/components/LineChart.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.0/baseweb/static/js/components/NavigationDrawer.js` & `baseweb-0.2.1/baseweb/static/js/components/NavigationDrawer.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.0/baseweb/static/js/components/PageWithBanner.js` & `baseweb-0.2.1/baseweb/static/js/components/PageWithBanner.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.0/baseweb/static/js/components/PageWithStatus.js` & `baseweb-0.2.1/baseweb/static/js/components/PageWithStatus.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.0/baseweb/static/js/components/ProcessDiagram.js` & `baseweb-0.2.1/baseweb/static/js/components/ProcessDiagram.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.0/baseweb/static/js/socketio.js` & `baseweb-0.2.1/baseweb/static/js/socketio.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.0/baseweb/static/vendor/css/bootstrap-datetimepicker.css` & `baseweb-0.2.1/baseweb/static/vendor/css/bootstrap-datetimepicker.css`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.0/baseweb/static/vendor/css/highlight.js.github.css` & `baseweb-0.2.1/baseweb/static/vendor/css/highlight.js.github.css`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.0/baseweb/static/vendor/css/roboto-material-icons.css` & `baseweb-0.2.1/baseweb/static/vendor/css/roboto-material-icons.css`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.0/baseweb/static/vendor/css/vfg.css` & `baseweb-0.2.1/baseweb/static/vendor/css/vfg.css`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.0/baseweb/static/vendor/css/vue-multiselect.min.css` & `baseweb-0.2.1/baseweb/static/vendor/css/vue-multiselect.min.css`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.0/baseweb/static/vendor/css/vuetify.min.css` & `baseweb-0.2.1/baseweb/static/vendor/css/vuetify.min.css`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.0/baseweb/static/vendor/fonts/KFOlCnqEu92Fr1MmEU9fBBc9.ttf` & `baseweb-0.2.1/baseweb/static/vendor/fonts/KFOlCnqEu92Fr1MmEU9fBBc9.ttf`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.0/baseweb/static/vendor/fonts/KFOlCnqEu92Fr1MmSU5fBBc9.ttf` & `baseweb-0.2.1/baseweb/static/vendor/fonts/KFOlCnqEu92Fr1MmSU5fBBc9.ttf`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.0/baseweb/static/vendor/fonts/KFOlCnqEu92Fr1MmWUlfBBc9.ttf` & `baseweb-0.2.1/baseweb/static/vendor/fonts/KFOlCnqEu92Fr1MmWUlfBBc9.ttf`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.0/baseweb/static/vendor/fonts/KFOmCnqEu92Fr1Mu4mxP.ttf` & `baseweb-0.2.1/baseweb/static/vendor/fonts/KFOmCnqEu92Fr1Mu4mxP.ttf`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.0/baseweb/static/vendor/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2` & `baseweb-0.2.1/baseweb/static/vendor/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.0/baseweb/static/vendor/js/Chart.min.js` & `baseweb-0.2.1/baseweb/static/vendor/js/Chart.min.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.0/baseweb/static/vendor/js/bootstrap-datetimepicker.min.js` & `baseweb-0.2.1/baseweb/static/vendor/js/bootstrap-datetimepicker.min.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.0/baseweb/static/vendor/js/bootstrap.min.js` & `baseweb-0.2.1/baseweb/static/vendor/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.0/baseweb/static/vendor/js/highlight.min.js` & `baseweb-0.2.1/baseweb/static/vendor/js/highlight.min.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.0/baseweb/static/vendor/js/html5shiv.min.js` & `baseweb-0.2.1/baseweb/static/vendor/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.0/baseweb/static/vendor/js/index.js.map` & `baseweb-0.2.1/baseweb/static/vendor/js/index.js.map`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.0/baseweb/static/vendor/js/jquery.min.js` & `baseweb-0.2.1/baseweb/static/vendor/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.0/baseweb/static/vendor/js/moment.min.js` & `baseweb-0.2.1/baseweb/static/vendor/js/moment.min.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.0/baseweb/static/vendor/js/respond.min.js` & `baseweb-0.2.1/baseweb/static/vendor/js/respond.min.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.0/baseweb/static/vendor/js/socket.io.min.js.map` & `baseweb-0.2.1/baseweb/static/vendor/js/socket.io.min.js.map`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.0/baseweb/static/vendor/js/socket.io.slim.js` & `baseweb-0.2.1/baseweb/static/vendor/js/socket.io.slim.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.0/baseweb/static/vendor/js/vue-chartjs.min.js` & `baseweb-0.2.1/baseweb/static/vendor/js/vue-chartjs.min.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.0/baseweb/static/vendor/js/vue-chartjs.min.js.map` & `baseweb-0.2.1/baseweb/static/vendor/js/vue-chartjs.min.js.map`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.0/baseweb/static/vendor/js/vue-form-generator.min.js` & `baseweb-0.2.1/baseweb/static/vendor/js/vue-form-generator.min.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.0/baseweb/static/vendor/js/vue-multiselect.min.js` & `baseweb-0.2.1/baseweb/static/vendor/js/vue-multiselect.min.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.0/baseweb/static/vendor/js/vue-notification.js` & `baseweb-0.2.1/baseweb/static/vendor/js/vue-notification.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.0/baseweb/static/vendor/js/vue-router.js` & `baseweb-0.2.1/baseweb/static/vendor/js/vue-router.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.0/baseweb/static/vendor/js/vue.js` & `baseweb-0.2.1/baseweb/static/vendor/js/vue.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.0/baseweb/static/vendor/js/vuetify.js` & `baseweb-0.2.1/baseweb/static/vendor/js/vuetify.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.0/baseweb/static/vendor/js/vuetify.js.map` & `baseweb-0.2.1/baseweb/static/vendor/js/vuetify.js.map`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.0/baseweb/static/vendor/js/vuex.js` & `baseweb-0.2.1/baseweb/static/vendor/js/vuex.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.0/baseweb/templates/main.html` & `baseweb-0.2.1/baseweb/templates/main.html`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.0/baseweb/templates/manifest.json` & `baseweb-0.2.1/baseweb/templates/manifest.json`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.0/baseweb-demo/__init__.py` & `baseweb-0.2.1/baseweb-demo/__init__.py`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.0/baseweb-demo/pages/components/CollectionView/__init__.py` & `baseweb-0.2.1/baseweb-demo/pages/components/CollectionView/__init__.py`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.0/baseweb-demo/pages/index/__init__.py` & `baseweb-0.2.1/baseweb-demo/pages/index/__init__.py`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.0/baseweb-demo/pages/protected_page/__init__.py` & `baseweb-0.2.1/baseweb-demo/pages/protected_page/__init__.py`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.0/baseweb.egg-info/PKG-INFO` & `baseweb-0.2.1/baseweb.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baseweb
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Pythonic base for building interactive web applications
 Home-page: https://github.com/christophevg/baseweb
 Author: Christophe VG
 License: MIT
 Keywords: Flask Vue REST SocketIO
 Classifier: Environment :: Web Environment
 Classifier: Development Status :: 4 - Beta
@@ -20,15 +20,14 @@
 Requires-Dist: Flask-SocketIO
 Requires-Dist: python-dotenv
 Requires-Dist: websocket-client
 Requires-Dist: python-engineio
 Requires-Dist: python-socketio
 Requires-Dist: dotmap
 Requires-Dist: pyfiglet
-Requires-Dist: dnspython==2.5.0
 
 # baseweb
 
 > A Pythonic base for building interactive web applications
 
 [![Latest Version on PyPI](https://img.shields.io/pypi/v/baseweb.svg)](https://pypi.python.org/pypi/baseweb/)
 [![Supported Implementations](https://img.shields.io/pypi/pyversions/baseweb.svg)](https://pypi.python.org/pypi/baseweb/)
```

### Comparing `baseweb-0.2.0/baseweb.egg-info/SOURCES.txt` & `baseweb-0.2.1/baseweb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.0/setup.py` & `baseweb-0.2.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,14 @@
   "Flask-SocketIO",
   "python-dotenv",
   "websocket-client",
   "python-engineio",
   "python-socketio",
   "dotmap",
   "pyfiglet",
-  "dnspython==2.5.0",
   
 ]
 ENTRY_POINTS = {
   
 }
 SCRIPTS = [
```

