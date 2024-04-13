# Comparing `tmp/sortinghat-1.0.0rc2.tar.gz` & `tmp/sortinghat-1.0.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sortinghat-1.0.0rc2.tar", max compression
+gzip compressed data, was "sortinghat-1.0.0rc3.tar", max compression
```

## Comparing `sortinghat-1.0.0rc2.tar` & `sortinghat-1.0.0rc3.tar`

### file list

```diff
@@ -1,205 +1,205 @@
--rw-r--r--   0        0        0      431 2024-04-11 10:44:11.130280 sortinghat-1.0.0rc2/AUTHORS
--rw-r--r--   0        0        0    35147 2024-04-11 10:44:11.130280 sortinghat-1.0.0rc2/LICENSE
--rw-r--r--   0        0        0    27792 2024-04-11 10:44:11.130280 sortinghat-1.0.0rc2/NEWS
--rw-r--r--   0        0        0     9626 2024-04-11 10:44:11.134280 sortinghat-1.0.0rc2/README.md
--rw-r--r--   0        0        0     2149 2024-04-11 10:44:11.134280 sortinghat-1.0.0rc2/pyproject.toml
--rw-r--r--   0        0        0       91 2024-04-11 10:44:11.134280 sortinghat-1.0.0rc2/sortinghat/_version.py
--rw-r--r--   0        0        0        0 2024-04-11 10:44:11.134280 sortinghat-1.0.0rc2/sortinghat/app/__init__.py
--rw-r--r--   0        0        0     1250 2024-04-11 10:44:11.134280 sortinghat-1.0.0rc2/sortinghat/app/schema.py
--rw-r--r--   0        0        0      647 2024-04-11 10:44:11.134280 sortinghat-1.0.0rc2/sortinghat/app/urls.py
--rw-r--r--   0        0        0      196 2024-04-11 10:44:11.134280 sortinghat-1.0.0rc2/sortinghat/app/wsgi.py
--rw-r--r--   0        0        0        0 2024-04-11 10:44:11.134280 sortinghat-1.0.0rc2/sortinghat/cli/__init__.py
--rw-r--r--   0        0        0      977 2024-04-11 10:44:11.134280 sortinghat-1.0.0rc2/sortinghat/cli/client/__init__.py
--rw-r--r--   0        0        0     5411 2024-04-11 10:44:11.134280 sortinghat-1.0.0rc2/sortinghat/cli/client/client.py
--rw-r--r--   0        0        0    43408 2024-04-11 10:44:11.134280 sortinghat-1.0.0rc2/sortinghat/cli/client/schema.py
--rw-r--r--   0        0        0        0 2024-04-11 10:44:11.138280 sortinghat-1.0.0rc2/sortinghat/cli/cmds/__init__.py
--rw-r--r--   0        0        0     3072 2024-04-11 10:44:11.138280 sortinghat-1.0.0rc2/sortinghat/cli/cmds/add.py
--rw-r--r--   0        0        0     6145 2024-04-11 10:44:11.138280 sortinghat-1.0.0rc2/sortinghat/cli/cmds/config.py
--rw-r--r--   0        0        0     3219 2024-04-11 10:44:11.138280 sortinghat-1.0.0rc2/sortinghat/cli/cmds/countries.py
--rw-r--r--   0        0        0     3462 2024-04-11 10:44:11.138280 sortinghat-1.0.0rc2/sortinghat/cli/cmds/enroll.py
--rw-r--r--   0        0        0     2860 2024-04-11 10:44:11.138280 sortinghat-1.0.0rc2/sortinghat/cli/cmds/lock.py
--rw-r--r--   0        0        0     2342 2024-04-11 10:44:11.138280 sortinghat-1.0.0rc2/sortinghat/cli/cmds/merge.py
--rw-r--r--   0        0        0     2352 2024-04-11 10:44:11.138280 sortinghat-1.0.0rc2/sortinghat/cli/cmds/mv.py
--rw-r--r--   0        0        0     7466 2024-04-11 10:44:11.138280 sortinghat-1.0.0rc2/sortinghat/cli/cmds/orgs.py
--rw-r--r--   0        0        0     2934 2024-04-11 10:44:11.138280 sortinghat-1.0.0rc2/sortinghat/cli/cmds/profile.py
--rw-r--r--   0        0        0     1992 2024-04-11 10:44:11.138280 sortinghat-1.0.0rc2/sortinghat/cli/cmds/rm.py
--rw-r--r--   0        0        0     2909 2024-04-11 10:44:11.138280 sortinghat-1.0.0rc2/sortinghat/cli/cmds/show.py
--rw-r--r--   0        0        0     2365 2024-04-11 10:44:11.138280 sortinghat-1.0.0rc2/sortinghat/cli/cmds/split.py
--rw-r--r--   0        0        0     3364 2024-04-11 10:44:11.138280 sortinghat-1.0.0rc2/sortinghat/cli/cmds/withdraw.py
--rwxr-xr-x   0        0        0     2857 2024-04-11 10:44:11.138280 sortinghat-1.0.0rc2/sortinghat/cli/sortinghat.py
--rw-r--r--   0        0        0       43 2024-04-11 10:44:11.138280 sortinghat-1.0.0rc2/sortinghat/cli/templates/add.tmpl
--rw-r--r--   0        0        0       23 2024-04-11 10:44:11.138280 sortinghat-1.0.0rc2/sortinghat/cli/templates/config.tmpl
--rw-r--r--   0        0        0       83 2024-04-11 10:44:11.138280 sortinghat-1.0.0rc2/sortinghat/cli/templates/countries.tmpl
--rw-r--r--   0        0        0       54 2024-04-11 10:44:11.138280 sortinghat-1.0.0rc2/sortinghat/cli/templates/lock.tmpl
--rw-r--r--   0        0        0      169 2024-04-11 10:44:11.138280 sortinghat-1.0.0rc2/sortinghat/cli/templates/mv.tmpl
--rw-r--r--   0        0        0      208 2024-04-11 10:44:11.138280 sortinghat-1.0.0rc2/sortinghat/cli/templates/organizations.tmpl
--rw-r--r--   0        0        0      375 2024-04-11 10:44:11.138280 sortinghat-1.0.0rc2/sortinghat/cli/templates/profile.tmpl
--rw-r--r--   0        0        0      106 2024-04-11 10:44:11.138280 sortinghat-1.0.0rc2/sortinghat/cli/templates/rm.tmpl
--rw-r--r--   0        0        0     1016 2024-04-11 10:44:11.138280 sortinghat-1.0.0rc2/sortinghat/cli/templates/show.tmpl
--rw-r--r--   0        0        0       69 2024-04-11 10:44:11.138280 sortinghat-1.0.0rc2/sortinghat/cli/templates/split.tmpl
--rw-r--r--   0        0        0     4856 2024-04-11 10:44:11.138280 sortinghat-1.0.0rc2/sortinghat/cli/utils.py
--rw-r--r--   0        0        0        0 2024-04-11 10:44:11.138280 sortinghat-1.0.0rc2/sortinghat/config/__init__.py
--rw-r--r--   0        0        0    10027 2024-04-11 10:44:11.138280 sortinghat-1.0.0rc2/sortinghat/config/settings.py
--rw-r--r--   0        0        0       20 2024-04-11 10:44:11.138280 sortinghat-1.0.0rc2/sortinghat/config/tenants.json
--rw-r--r--   0        0        0     1544 2024-04-11 10:44:11.138280 sortinghat-1.0.0rc2/sortinghat/core/admin.py
--rw-r--r--   0        0        0    58676 2024-04-11 10:44:11.138280 sortinghat-1.0.0rc2/sortinghat/core/api.py
--rw-r--r--   0        0        0      926 2024-04-11 10:44:11.138280 sortinghat-1.0.0rc2/sortinghat/core/apps.py
--rw-r--r--   0        0        0     5169 2024-04-11 10:44:11.138280 sortinghat-1.0.0rc2/sortinghat/core/aux.py
--rw-r--r--   0        0        0      997 2024-04-11 10:44:11.138280 sortinghat-1.0.0rc2/sortinghat/core/context.py
--rw-r--r--   0        0        0    43214 2024-04-11 10:44:11.138280 sortinghat-1.0.0rc2/sortinghat/core/db.py
--rw-r--r--   0        0        0     4700 2024-04-11 10:44:11.138280 sortinghat-1.0.0rc2/sortinghat/core/decorators.py
--rw-r--r--   0        0        0     4006 2024-04-11 10:44:11.138280 sortinghat-1.0.0rc2/sortinghat/core/errors.py
--rw-r--r--   0        0        0    41236 2024-04-11 10:44:11.138280 sortinghat-1.0.0rc2/sortinghat/core/fixtures/countries.json
--rw-r--r--   0        0        0     7820 2024-04-11 10:44:11.138280 sortinghat-1.0.0rc2/sortinghat/core/importer/backend.py
--rw-r--r--   0        0        0    13977 2024-04-11 10:44:11.138280 sortinghat-1.0.0rc2/sortinghat/core/importer/backends/gitdm.py
--rw-r--r--   0        0        0     7136 2024-04-11 10:44:11.138280 sortinghat-1.0.0rc2/sortinghat/core/importer/backends/mailmap.py
--rw-r--r--   0        0        0     3628 2024-04-11 10:44:11.138280 sortinghat-1.0.0rc2/sortinghat/core/importer/base.py
--rw-r--r--   0        0        0     2143 2024-04-11 10:44:11.138280 sortinghat-1.0.0rc2/sortinghat/core/importer/models.py
--rw-r--r--   0        0        0     2059 2024-04-11 10:44:11.138280 sortinghat-1.0.0rc2/sortinghat/core/importer/utils.py
--rw-r--r--   0        0        0    33234 2024-04-11 10:44:11.138280 sortinghat-1.0.0rc2/sortinghat/core/jobs.py
--rw-r--r--   0        0        0     7298 2024-04-11 10:44:11.138280 sortinghat-1.0.0rc2/sortinghat/core/log.py
--rw-r--r--   0        0        0        0 2024-04-11 10:44:11.138280 sortinghat-1.0.0rc2/sortinghat/core/management/__init__.py
--rw-r--r--   0        0        0        0 2024-04-11 10:44:11.138280 sortinghat-1.0.0rc2/sortinghat/core/management/commands/__init__.py
--rw-r--r--   0        0        0     4155 2024-04-11 10:44:11.138280 sortinghat-1.0.0rc2/sortinghat/core/management/commands/create_groups.py
--rw-r--r--   0        0        0     4372 2024-04-11 10:44:11.138280 sortinghat-1.0.0rc2/sortinghat/core/middleware.py
--rw-r--r--   0        0        0    14035 2024-04-11 10:44:11.138280 sortinghat-1.0.0rc2/sortinghat/core/migrations/0001_sortinghat.py
--rw-r--r--   0        0        0     1717 2024-04-11 10:44:11.138280 sortinghat-1.0.0rc2/sortinghat/core/migrations/0002_importidentitiestask.py
--rw-r--r--   0        0        0     1502 2024-04-11 10:44:11.138280 sortinghat-1.0.0rc2/sortinghat/core/migrations/0003_multi_tenancy.py
--rw-r--r--   0        0        0      582 2024-04-11 10:44:11.138280 sortinghat-1.0.0rc2/sortinghat/core/migrations/0004_tenant_using_header.py
--rw-r--r--   0        0        0     1597 2024-04-11 10:44:11.138280 sortinghat-1.0.0rc2/sortinghat/core/migrations/0005_scheduledtask.py
--rw-r--r--   0        0        0     1117 2024-04-11 10:44:11.138280 sortinghat-1.0.0rc2/sortinghat/core/migrations/0006_unify_scheduled_tasks.py
--rw-r--r--   0        0        0      310 2024-04-11 10:44:11.138280 sortinghat-1.0.0rc2/sortinghat/core/migrations/0007_delete_importidentitiestask.py
--rw-r--r--   0        0        0     1245 2024-04-11 10:44:11.138280 sortinghat-1.0.0rc2/sortinghat/core/migrations/0008_alias.py
--rw-r--r--   0        0        0        0 2024-04-11 10:44:11.138280 sortinghat-1.0.0rc2/sortinghat/core/migrations/__init__.py
--rw-r--r--   0        0        0    12140 2024-04-11 10:44:11.138280 sortinghat-1.0.0rc2/sortinghat/core/models.py
--rw-r--r--   0        0        0      839 2024-04-11 10:44:11.138280 sortinghat-1.0.0rc2/sortinghat/core/recommendations/__init__.py
--rw-r--r--   0        0        0     5219 2024-04-11 10:44:11.138280 sortinghat-1.0.0rc2/sortinghat/core/recommendations/affiliation.py
--rw-r--r--   0        0        0     3151 2024-04-11 10:44:11.138280 sortinghat-1.0.0rc2/sortinghat/core/recommendations/engine.py
--rw-r--r--   0        0        0     5313 2024-04-11 10:44:11.138280 sortinghat-1.0.0rc2/sortinghat/core/recommendations/exclusion.py
--rw-r--r--   0        0        0     5657 2024-04-11 10:44:11.138280 sortinghat-1.0.0rc2/sortinghat/core/recommendations/gender.py
--rw-r--r--   0        0        0     9792 2024-04-11 10:44:11.138280 sortinghat-1.0.0rc2/sortinghat/core/recommendations/matching.py
--rw-r--r--   0        0        0    80905 2024-04-11 10:44:11.138280 sortinghat-1.0.0rc2/sortinghat/core/schema.py
--rw-r--r--   0        0        0      893 2024-04-11 10:45:13.614500 sortinghat-1.0.0rc2/sortinghat/core/static/css/105.858cd75e.css
--rw-r--r--   0        0        0    16227 2024-04-11 10:45:13.606500 sortinghat-1.0.0rc2/sortinghat/core/static/css/119.87ef3a04.css
--rw-r--r--   0        0        0    16726 2024-04-11 10:45:13.626500 sortinghat-1.0.0rc2/sortinghat/core/static/css/206.7bb5d056.css
--rw-r--r--   0        0        0       71 2024-04-11 10:45:13.614500 sortinghat-1.0.0rc2/sortinghat/core/static/css/253.193dbe55.css
--rw-r--r--   0        0        0     6900 2024-04-11 10:45:13.614500 sortinghat-1.0.0rc2/sortinghat/core/static/css/488.19ce97b1.css
--rw-r--r--   0        0        0     5954 2024-04-11 10:45:13.614500 sortinghat-1.0.0rc2/sortinghat/core/static/css/546.696b6ba4.css
--rw-r--r--   0        0        0    10467 2024-04-11 10:45:13.614500 sortinghat-1.0.0rc2/sortinghat/core/static/css/764.ddc4524e.css
--rw-r--r--   0        0        0     6252 2024-04-11 10:45:13.606500 sortinghat-1.0.0rc2/sortinghat/core/static/css/812.39b5238d.css
--rw-r--r--   0        0        0    25071 2024-04-11 10:45:13.626500 sortinghat-1.0.0rc2/sortinghat/core/static/css/912.a5e49ce0.css
--rw-r--r--   0        0        0     5368 2024-04-11 10:45:13.606500 sortinghat-1.0.0rc2/sortinghat/core/static/css/app.1adeaa19.css
--rw-r--r--   0        0        0   698806 2024-04-11 10:45:13.614500 sortinghat-1.0.0rc2/sortinghat/core/static/css/chunk-vendors.42fea764.css
--rw-r--r--   0        0        0    15086 2024-04-11 10:45:13.626500 sortinghat-1.0.0rc2/sortinghat/core/static/favicon-grimoirelab.ico
--rw-r--r--   0        0        0    99428 2024-04-11 10:45:13.590500 sortinghat-1.0.0rc2/sortinghat/core/static/fonts/Roboto-Italic.76b8308b.woff
--rw-r--r--   0        0        0   173516 2024-04-11 10:45:13.590500 sortinghat-1.0.0rc2/sortinghat/core/static/fonts/Roboto-Italic.991def81.ttf
--rw-r--r--   0        0        0    30612 2024-04-11 10:45:13.590500 sortinghat-1.0.0rc2/sortinghat/core/static/fonts/Roboto-Italic.ca10c790.woff2
--rw-r--r--   0        0        0    93472 2024-04-11 10:45:13.590500 sortinghat-1.0.0rc2/sortinghat/core/static/fonts/Roboto-Light.2d3c72a3.woff
--rw-r--r--   0        0        0    65564 2024-04-11 10:45:13.590500 sortinghat-1.0.0rc2/sortinghat/core/static/fonts/Roboto-Light.41cb61ed.woff2
--rw-r--r--   0        0        0   170012 2024-04-11 10:45:13.590500 sortinghat-1.0.0rc2/sortinghat/core/static/fonts/Roboto-Light.f2e7274e.ttf
--rw-r--r--   0        0        0    72036 2024-04-11 10:45:13.590500 sortinghat-1.0.0rc2/sortinghat/core/static/fonts/Roboto-LightItalic.07369d23.woff2
--rw-r--r--   0        0        0   101120 2024-04-11 10:45:13.590500 sortinghat-1.0.0rc2/sortinghat/core/static/fonts/Roboto-LightItalic.45582c0c.woff
--rw-r--r--   0        0        0   176184 2024-04-11 10:45:13.590500 sortinghat-1.0.0rc2/sortinghat/core/static/fonts/Roboto-LightItalic.b694f0fe.ttf
--rw-r--r--   0        0        0    50224 2024-04-11 10:45:13.590500 sortinghat-1.0.0rc2/sortinghat/core/static/fonts/Roboto-Medium.0519ad6f.woff2
--rw-r--r--   0        0        0    94364 2024-04-11 10:45:13.590500 sortinghat-1.0.0rc2/sortinghat/core/static/fonts/Roboto-Medium.483a3bd1.woff
--rw-r--r--   0        0        0   171656 2024-04-11 10:45:13.602500 sortinghat-1.0.0rc2/sortinghat/core/static/fonts/Roboto-Medium.af9d0139.ttf
--rw-r--r--   0        0        0   176428 2024-04-11 10:45:13.602500 sortinghat-1.0.0rc2/sortinghat/core/static/fonts/Roboto-MediumItalic.3723a2e7.ttf
--rw-r--r--   0        0        0   101008 2024-04-11 10:45:13.602500 sortinghat-1.0.0rc2/sortinghat/core/static/fonts/Roboto-MediumItalic.8b19cc18.woff
--rw-r--r--   0        0        0   139529 2024-04-11 10:45:13.602500 sortinghat-1.0.0rc2/sortinghat/core/static/fonts/Roboto-MediumItalic.b35d3641.woff2
--rw-r--r--   0        0        0    93784 2024-04-11 10:45:13.590500 sortinghat-1.0.0rc2/sortinghat/core/static/fonts/Roboto-Regular.36d4503d.woff
--rw-r--r--   0        0        0   171272 2024-04-11 10:45:13.590500 sortinghat-1.0.0rc2/sortinghat/core/static/fonts/Roboto-Regular.ae3a8db9.ttf
--rw-r--r--   0        0        0    66012 2024-04-11 10:45:13.590500 sortinghat-1.0.0rc2/sortinghat/core/static/fonts/Roboto-Regular.e0553e00.woff2
--rw-r--r--   0        0        0  1026176 2024-04-11 10:45:13.606500 sortinghat-1.0.0rc2/sortinghat/core/static/fonts/materialdesignicons-webfont.21f691f0.ttf
--rw-r--r--   0        0        0   325244 2024-04-11 10:45:13.602500 sortinghat-1.0.0rc2/sortinghat/core/static/fonts/materialdesignicons-webfont.54b0f60d.woff2
--rw-r--r--   0        0        0  1026396 2024-04-11 10:45:13.602500 sortinghat-1.0.0rc2/sortinghat/core/static/fonts/materialdesignicons-webfont.5d875350.eot
--rw-r--r--   0        0        0   465188 2024-04-11 10:45:13.606500 sortinghat-1.0.0rc2/sortinghat/core/static/fonts/materialdesignicons-webfont.d671cbf6.woff
--rw-r--r--   0        0        0    13357 2024-04-11 10:45:13.614500 sortinghat-1.0.0rc2/sortinghat/core/static/js/105.2c5bfa40.js
--rw-r--r--   0        0        0    30516 2024-04-11 10:45:13.626500 sortinghat-1.0.0rc2/sortinghat/core/static/js/105.2c5bfa40.js.map
--rw-r--r--   0        0        0    66424 2024-04-11 10:45:13.606500 sortinghat-1.0.0rc2/sortinghat/core/static/js/119.6bdc5ff2.js
--rw-r--r--   0        0        0   154025 2024-04-11 10:45:13.626500 sortinghat-1.0.0rc2/sortinghat/core/static/js/119.6bdc5ff2.js.map
--rw-r--r--   0        0        0    54509 2024-04-11 10:45:13.626500 sortinghat-1.0.0rc2/sortinghat/core/static/js/206.75232ba8.js
--rw-r--r--   0        0        0   131975 2024-04-11 10:45:13.674500 sortinghat-1.0.0rc2/sortinghat/core/static/js/206.75232ba8.js.map
--rw-r--r--   0        0        0     3737 2024-04-11 10:45:13.606500 sortinghat-1.0.0rc2/sortinghat/core/static/js/208.91e4b79e.js
--rw-r--r--   0        0        0     7875 2024-04-11 10:45:13.626500 sortinghat-1.0.0rc2/sortinghat/core/static/js/208.91e4b79e.js.map
--rw-r--r--   0        0        0     1900 2024-04-11 10:45:13.614500 sortinghat-1.0.0rc2/sortinghat/core/static/js/253.61ce8eec.js
--rw-r--r--   0        0        0     4676 2024-04-11 10:45:13.626500 sortinghat-1.0.0rc2/sortinghat/core/static/js/253.61ce8eec.js.map
--rw-r--r--   0        0        0     2783 2024-04-11 10:45:13.606500 sortinghat-1.0.0rc2/sortinghat/core/static/js/414.13cae85b.js
--rw-r--r--   0        0        0     6249 2024-04-11 10:45:13.626500 sortinghat-1.0.0rc2/sortinghat/core/static/js/414.13cae85b.js.map
--rw-r--r--   0        0        0    23895 2024-04-11 10:45:13.614500 sortinghat-1.0.0rc2/sortinghat/core/static/js/488.0a0d2dda.js
--rw-r--r--   0        0        0    59037 2024-04-11 10:45:13.626500 sortinghat-1.0.0rc2/sortinghat/core/static/js/488.0a0d2dda.js.map
--rw-r--r--   0        0        0     7069 2024-04-11 10:45:13.614500 sortinghat-1.0.0rc2/sortinghat/core/static/js/544.b1834368.js
--rw-r--r--   0        0        0    13923 2024-04-11 10:45:13.626500 sortinghat-1.0.0rc2/sortinghat/core/static/js/544.b1834368.js.map
--rw-r--r--   0        0        0    12841 2024-04-11 10:45:13.614500 sortinghat-1.0.0rc2/sortinghat/core/static/js/546.718bab60.js
--rw-r--r--   0        0        0    29507 2024-04-11 10:45:13.626500 sortinghat-1.0.0rc2/sortinghat/core/static/js/546.718bab60.js.map
--rw-r--r--   0        0        0    50765 2024-04-11 10:45:13.614500 sortinghat-1.0.0rc2/sortinghat/core/static/js/689.e598fac2.js
--rw-r--r--   0        0        0   167791 2024-04-11 10:45:13.674500 sortinghat-1.0.0rc2/sortinghat/core/static/js/689.e598fac2.js.map
--rw-r--r--   0        0        0    14356 2024-04-11 10:45:13.614500 sortinghat-1.0.0rc2/sortinghat/core/static/js/764.5fe45faf.js
--rw-r--r--   0        0        0    31925 2024-04-11 10:45:13.666500 sortinghat-1.0.0rc2/sortinghat/core/static/js/764.5fe45faf.js.map
--rw-r--r--   0        0        0    23708 2024-04-11 10:45:13.606500 sortinghat-1.0.0rc2/sortinghat/core/static/js/812.711cab61.js
--rw-r--r--   0        0        0    54522 2024-04-11 10:45:13.626500 sortinghat-1.0.0rc2/sortinghat/core/static/js/812.711cab61.js.map
--rw-r--r--   0        0        0    58642 2024-04-11 10:45:13.626500 sortinghat-1.0.0rc2/sortinghat/core/static/js/912.ddb83f31.js
--rw-r--r--   0        0        0   156277 2024-04-11 10:45:13.674500 sortinghat-1.0.0rc2/sortinghat/core/static/js/912.ddb83f31.js.map
--rw-r--r--   0        0        0    14541 2024-04-11 10:45:13.606500 sortinghat-1.0.0rc2/sortinghat/core/static/js/app.ba14e94f.js
--rw-r--r--   0        0        0    47793 2024-04-11 10:45:13.626500 sortinghat-1.0.0rc2/sortinghat/core/static/js/app.ba14e94f.js.map
--rw-r--r--   0        0        0   922197 2024-04-11 10:45:13.614500 sortinghat-1.0.0rc2/sortinghat/core/static/js/chunk-vendors.dba6d507.js
--rw-r--r--   0        0        0  4116361 2024-04-11 10:45:13.666500 sortinghat-1.0.0rc2/sortinghat/core/static/js/chunk-vendors.dba6d507.js.map
--rw-r--r--   0        0        0      867 2024-04-11 10:45:13.674500 sortinghat-1.0.0rc2/sortinghat/core/templates/index.html
--rw-r--r--   0        0        0     2436 2024-04-11 10:44:11.142280 sortinghat-1.0.0rc2/sortinghat/core/tenant.py
--rw-r--r--   0        0        0     3881 2024-04-11 10:44:11.142280 sortinghat-1.0.0rc2/sortinghat/core/views.py
--rw-r--r--   0        0        0        0 2024-04-11 10:44:11.142280 sortinghat-1.0.0rc2/sortinghat/server/__init__.py
--rw-r--r--   0        0        0    13717 2024-04-11 10:44:11.142280 sortinghat-1.0.0rc2/sortinghat/server/sortinghat_admin.py
--rw-r--r--   0        0        0     3062 2024-04-11 10:44:11.142280 sortinghat-1.0.0rc2/sortinghat/server/sortinghatd.py
--rw-r--r--   0        0        0     2365 2024-04-11 10:44:11.142280 sortinghat-1.0.0rc2/sortinghat/server/sortinghatw.py
--rwxr-xr-x   0        0        0     9218 2024-04-11 10:44:11.142280 sortinghat-1.0.0rc2/sortinghat/server/utils/create_sh_0_7_fixture.py
--rw-r--r--   0        0        0     3485 2024-04-11 10:44:11.142280 sortinghat-1.0.0rc2/sortinghat/utils/__init__.py
--rw-r--r--   0        0        0        0 2024-04-11 10:44:11.142280 sortinghat-1.0.0rc2/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-04-11 10:44:11.142280 sortinghat-1.0.0rc2/tests/cli/__init__.py
--rw-r--r--   0        0        0       57 2024-04-11 10:44:11.142280 sortinghat-1.0.0rc2/tests/cli/config_file.cfg
--rw-r--r--   0        0        0     7601 2024-04-11 10:44:11.142280 sortinghat-1.0.0rc2/tests/cli/test_cmd_add.py
--rw-r--r--   0        0        0    17698 2024-04-11 10:44:11.142280 sortinghat-1.0.0rc2/tests/cli/test_cmd_config.py
--rw-r--r--   0        0        0    10234 2024-04-11 10:44:11.142280 sortinghat-1.0.0rc2/tests/cli/test_cmd_countries.py
--rw-r--r--   0        0        0     7597 2024-04-11 10:44:11.142280 sortinghat-1.0.0rc2/tests/cli/test_cmd_enroll.py
--rw-r--r--   0        0        0     5397 2024-04-11 10:44:11.142280 sortinghat-1.0.0rc2/tests/cli/test_cmd_lock.py
--rw-r--r--   0        0        0     3851 2024-04-11 10:44:11.142280 sortinghat-1.0.0rc2/tests/cli/test_cmd_merge.py
--rw-r--r--   0        0        0     5041 2024-04-11 10:44:11.142280 sortinghat-1.0.0rc2/tests/cli/test_cmd_mv.py
--rw-r--r--   0        0        0    13658 2024-04-11 10:44:11.142280 sortinghat-1.0.0rc2/tests/cli/test_cmd_orgs.py
--rw-r--r--   0        0        0     9117 2024-04-11 10:44:11.142280 sortinghat-1.0.0rc2/tests/cli/test_cmd_profile.py
--rw-r--r--   0        0        0     4599 2024-04-11 10:44:11.142280 sortinghat-1.0.0rc2/tests/cli/test_cmd_rm.py
--rw-r--r--   0        0        0    10993 2024-04-11 10:44:11.142280 sortinghat-1.0.0rc2/tests/cli/test_cmd_show.py
--rw-r--r--   0        0        0     5280 2024-04-11 10:44:11.142280 sortinghat-1.0.0rc2/tests/cli/test_cmd_split.py
--rw-r--r--   0        0        0     6294 2024-04-11 10:44:11.142280 sortinghat-1.0.0rc2/tests/cli/test_cmd_withdraw.py
--rw-r--r--   0        0        0        0 2024-04-11 10:44:11.142280 sortinghat-1.0.0rc2/tests/importer/__init__.py
--rw-r--r--   0        0        0      159 2024-04-11 10:44:11.142280 sortinghat-1.0.0rc2/tests/importer/data/gitdm/gitdm_email_aliases_valid.txt
--rw-r--r--   0        0        0      244 2024-04-11 10:44:11.142280 sortinghat-1.0.0rc2/tests/importer/data/gitdm/gitdm_email_to_employer_invalid.txt
--rw-r--r--   0        0        0      249 2024-04-11 10:44:11.142280 sortinghat-1.0.0rc2/tests/importer/data/gitdm/gitdm_email_to_employer_valid.txt
--rw-r--r--   0        0        0        0 2024-04-11 10:44:11.142280 sortinghat-1.0.0rc2/tests/importer/mocked_package/__init__.py
--rw-r--r--   0        0        0     1055 2024-04-11 10:44:11.142280 sortinghat-1.0.0rc2/tests/importer/mocked_package/backend_a.py
--rw-r--r--   0        0        0        0 2024-04-11 10:44:11.142280 sortinghat-1.0.0rc2/tests/importer/mocked_package/nested_package/__init__.py
--rw-r--r--   0        0        0      950 2024-04-11 10:44:11.142280 sortinghat-1.0.0rc2/tests/importer/mocked_package/nested_package/nested_backend_b.py
--rw-r--r--   0        0        0     1050 2024-04-11 10:44:11.142280 sortinghat-1.0.0rc2/tests/importer/mocked_package/nested_package/nested_backend_c.py
--rw-r--r--   0        0        0      865 2024-04-11 10:44:11.142280 sortinghat-1.0.0rc2/tests/importer/mocked_package/nested_package/nested_not_backend.py
--rw-r--r--   0        0        0     4797 2024-04-11 10:44:11.142280 sortinghat-1.0.0rc2/tests/importer/test_backend.py
--rw-r--r--   0        0        0    25058 2024-04-11 10:44:11.142280 sortinghat-1.0.0rc2/tests/importer/test_gitdm.py
--rw-r--r--   0        0        0     2416 2024-04-11 10:44:11.142280 sortinghat-1.0.0rc2/tests/importer/test_utils.py
--rw-r--r--   0        0        0        0 2024-04-11 10:44:11.142280 sortinghat-1.0.0rc2/tests/rec/__init__.py
--rw-r--r--   0        0        0    10028 2024-04-11 10:44:11.142280 sortinghat-1.0.0rc2/tests/rec/test_affiliations.py
--rw-r--r--   0        0        0     2925 2024-04-11 10:44:11.142280 sortinghat-1.0.0rc2/tests/rec/test_engine.py
--rw-r--r--   0        0        0     3937 2024-04-11 10:44:11.142280 sortinghat-1.0.0rc2/tests/rec/test_exclusion.py
--rw-r--r--   0        0        0     9040 2024-04-11 10:44:11.142280 sortinghat-1.0.0rc2/tests/rec/test_gender.py
--rw-r--r--   0        0        0    21600 2024-04-11 10:44:11.142280 sortinghat-1.0.0rc2/tests/rec/test_matches.py
--rw-r--r--   0        0        0      825 2024-04-11 10:44:11.142280 sortinghat-1.0.0rc2/tests/runners.py
--rw-r--r--   0        0        0        0 2024-04-11 10:44:11.142280 sortinghat-1.0.0rc2/tests/tenants/__init__.py
--rw-r--r--   0        0        0     7235 2024-04-11 10:44:11.142280 sortinghat-1.0.0rc2/tests/tenants/test_jobs.py
--rw-r--r--   0        0        0     2277 2024-04-11 10:44:11.142280 sortinghat-1.0.0rc2/tests/tenants/test_middleware.py
--rw-r--r--   0        0        0     5872 2024-04-11 10:44:11.142280 sortinghat-1.0.0rc2/tests/tenants/test_schema.py
--rw-r--r--   0        0        0   287020 2024-04-11 10:44:11.142280 sortinghat-1.0.0rc2/tests/test_api.py
--rw-r--r--   0        0        0    18365 2024-04-11 10:44:11.142280 sortinghat-1.0.0rc2/tests/test_aux.py
--rw-r--r--   0        0        0     9779 2024-04-11 10:44:11.142280 sortinghat-1.0.0rc2/tests/test_client.py
--rw-r--r--   0        0        0   135031 2024-04-11 10:44:11.146280 sortinghat-1.0.0rc2/tests/test_db.py
--rw-r--r--   0        0        0     9785 2024-04-11 10:44:11.146280 sortinghat-1.0.0rc2/tests/test_errors.py
--rw-r--r--   0        0        0    72127 2024-04-11 10:44:11.146280 sortinghat-1.0.0rc2/tests/test_jobs.py
--rw-r--r--   0        0        0    14074 2024-04-11 10:44:11.146280 sortinghat-1.0.0rc2/tests/test_log.py
--rw-r--r--   0        0        0    48532 2024-04-11 10:44:11.146280 sortinghat-1.0.0rc2/tests/test_model.py
--rw-r--r--   0        0        0   430566 2024-04-11 10:44:11.146280 sortinghat-1.0.0rc2/tests/test_schema.py
--rw-r--r--   0        0        0     6316 2024-04-11 10:44:11.146280 sortinghat-1.0.0rc2/tests/test_utils.py
--rw-r--r--   0        0        0    11505 1970-01-01 00:00:00.000000 sortinghat-1.0.0rc2/PKG-INFO
+-rw-r--r--   0        0        0      431 2024-04-12 14:43:30.535004 sortinghat-1.0.0rc3/AUTHORS
+-rw-r--r--   0        0        0    35147 2024-04-12 14:43:30.535004 sortinghat-1.0.0rc3/LICENSE
+-rw-r--r--   0        0        0    27792 2024-04-12 14:43:30.535004 sortinghat-1.0.0rc3/NEWS
+-rw-r--r--   0        0        0     9640 2024-04-12 14:43:30.535004 sortinghat-1.0.0rc3/README.md
+-rw-r--r--   0        0        0     2149 2024-04-12 14:43:30.539003 sortinghat-1.0.0rc3/pyproject.toml
+-rw-r--r--   0        0        0       91 2024-04-12 14:43:30.539003 sortinghat-1.0.0rc3/sortinghat/_version.py
+-rw-r--r--   0        0        0        0 2024-04-12 14:43:30.539003 sortinghat-1.0.0rc3/sortinghat/app/__init__.py
+-rw-r--r--   0        0        0     1250 2024-04-12 14:43:30.539003 sortinghat-1.0.0rc3/sortinghat/app/schema.py
+-rw-r--r--   0        0        0      647 2024-04-12 14:43:30.539003 sortinghat-1.0.0rc3/sortinghat/app/urls.py
+-rw-r--r--   0        0        0      196 2024-04-12 14:43:30.539003 sortinghat-1.0.0rc3/sortinghat/app/wsgi.py
+-rw-r--r--   0        0        0        0 2024-04-12 14:43:30.539003 sortinghat-1.0.0rc3/sortinghat/cli/__init__.py
+-rw-r--r--   0        0        0      977 2024-04-12 14:43:30.539003 sortinghat-1.0.0rc3/sortinghat/cli/client/__init__.py
+-rw-r--r--   0        0        0     5411 2024-04-12 14:43:30.539003 sortinghat-1.0.0rc3/sortinghat/cli/client/client.py
+-rw-r--r--   0        0        0    43408 2024-04-12 14:43:30.539003 sortinghat-1.0.0rc3/sortinghat/cli/client/schema.py
+-rw-r--r--   0        0        0        0 2024-04-12 14:43:30.539003 sortinghat-1.0.0rc3/sortinghat/cli/cmds/__init__.py
+-rw-r--r--   0        0        0     3072 2024-04-12 14:43:30.539003 sortinghat-1.0.0rc3/sortinghat/cli/cmds/add.py
+-rw-r--r--   0        0        0     6145 2024-04-12 14:43:30.539003 sortinghat-1.0.0rc3/sortinghat/cli/cmds/config.py
+-rw-r--r--   0        0        0     3219 2024-04-12 14:43:30.539003 sortinghat-1.0.0rc3/sortinghat/cli/cmds/countries.py
+-rw-r--r--   0        0        0     3462 2024-04-12 14:43:30.539003 sortinghat-1.0.0rc3/sortinghat/cli/cmds/enroll.py
+-rw-r--r--   0        0        0     2860 2024-04-12 14:43:30.539003 sortinghat-1.0.0rc3/sortinghat/cli/cmds/lock.py
+-rw-r--r--   0        0        0     2342 2024-04-12 14:43:30.539003 sortinghat-1.0.0rc3/sortinghat/cli/cmds/merge.py
+-rw-r--r--   0        0        0     2352 2024-04-12 14:43:30.539003 sortinghat-1.0.0rc3/sortinghat/cli/cmds/mv.py
+-rw-r--r--   0        0        0     7466 2024-04-12 14:43:30.539003 sortinghat-1.0.0rc3/sortinghat/cli/cmds/orgs.py
+-rw-r--r--   0        0        0     2934 2024-04-12 14:43:30.539003 sortinghat-1.0.0rc3/sortinghat/cli/cmds/profile.py
+-rw-r--r--   0        0        0     1992 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/cli/cmds/rm.py
+-rw-r--r--   0        0        0     2909 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/cli/cmds/show.py
+-rw-r--r--   0        0        0     2365 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/cli/cmds/split.py
+-rw-r--r--   0        0        0     3364 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/cli/cmds/withdraw.py
+-rwxr-xr-x   0        0        0     2857 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/cli/sortinghat.py
+-rw-r--r--   0        0        0       43 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/cli/templates/add.tmpl
+-rw-r--r--   0        0        0       23 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/cli/templates/config.tmpl
+-rw-r--r--   0        0        0       83 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/cli/templates/countries.tmpl
+-rw-r--r--   0        0        0       54 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/cli/templates/lock.tmpl
+-rw-r--r--   0        0        0      169 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/cli/templates/mv.tmpl
+-rw-r--r--   0        0        0      208 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/cli/templates/organizations.tmpl
+-rw-r--r--   0        0        0      375 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/cli/templates/profile.tmpl
+-rw-r--r--   0        0        0      106 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/cli/templates/rm.tmpl
+-rw-r--r--   0        0        0     1016 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/cli/templates/show.tmpl
+-rw-r--r--   0        0        0       69 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/cli/templates/split.tmpl
+-rw-r--r--   0        0        0     4856 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/cli/utils.py
+-rw-r--r--   0        0        0        0 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/config/__init__.py
+-rw-r--r--   0        0        0    10011 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/config/settings.py
+-rw-r--r--   0        0        0       20 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/config/tenants.json
+-rw-r--r--   0        0        0     1544 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/admin.py
+-rw-r--r--   0        0        0    58676 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/api.py
+-rw-r--r--   0        0        0      926 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/apps.py
+-rw-r--r--   0        0        0     5169 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/aux.py
+-rw-r--r--   0        0        0      997 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/context.py
+-rw-r--r--   0        0        0    43214 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/db.py
+-rw-r--r--   0        0        0     4700 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/decorators.py
+-rw-r--r--   0        0        0     4006 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/errors.py
+-rw-r--r--   0        0        0    41236 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/fixtures/countries.json
+-rw-r--r--   0        0        0     7820 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/importer/backend.py
+-rw-r--r--   0        0        0    13977 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/importer/backends/gitdm.py
+-rw-r--r--   0        0        0     7136 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/importer/backends/mailmap.py
+-rw-r--r--   0        0        0     3628 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/importer/base.py
+-rw-r--r--   0        0        0     2143 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/importer/models.py
+-rw-r--r--   0        0        0     2059 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/importer/utils.py
+-rw-r--r--   0        0        0    33234 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/jobs.py
+-rw-r--r--   0        0        0     7298 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/log.py
+-rw-r--r--   0        0        0        0 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/management/commands/__init__.py
+-rw-r--r--   0        0        0     4155 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/management/commands/create_groups.py
+-rw-r--r--   0        0        0     4372 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/middleware.py
+-rw-r--r--   0        0        0    14033 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/migrations/0001_sortinghat.py
+-rw-r--r--   0        0        0     1717 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/migrations/0002_importidentitiestask.py
+-rw-r--r--   0        0        0     1502 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/migrations/0003_multi_tenancy.py
+-rw-r--r--   0        0        0      582 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/migrations/0004_tenant_using_header.py
+-rw-r--r--   0        0        0     1597 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/migrations/0005_scheduledtask.py
+-rw-r--r--   0        0        0     1117 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/migrations/0006_unify_scheduled_tasks.py
+-rw-r--r--   0        0        0      310 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/migrations/0007_delete_importidentitiestask.py
+-rw-r--r--   0        0        0     1245 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/migrations/0008_alias.py
+-rw-r--r--   0        0        0        0 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/migrations/__init__.py
+-rw-r--r--   0        0        0    12140 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/models.py
+-rw-r--r--   0        0        0      839 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/recommendations/__init__.py
+-rw-r--r--   0        0        0     5219 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/recommendations/affiliation.py
+-rw-r--r--   0        0        0     3151 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/recommendations/engine.py
+-rw-r--r--   0        0        0     5313 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/recommendations/exclusion.py
+-rw-r--r--   0        0        0     5657 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/recommendations/gender.py
+-rw-r--r--   0        0        0     9792 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/recommendations/matching.py
+-rw-r--r--   0        0        0    80917 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/schema.py
+-rw-r--r--   0        0        0      893 2024-04-12 14:44:35.507217 sortinghat-1.0.0rc3/sortinghat/core/static/css/105.858cd75e.css
+-rw-r--r--   0        0        0    16227 2024-04-12 14:44:35.495217 sortinghat-1.0.0rc3/sortinghat/core/static/css/119.87ef3a04.css
+-rw-r--r--   0        0        0    16726 2024-04-12 14:44:35.515217 sortinghat-1.0.0rc3/sortinghat/core/static/css/206.7bb5d056.css
+-rw-r--r--   0        0        0       71 2024-04-12 14:44:35.507217 sortinghat-1.0.0rc3/sortinghat/core/static/css/253.193dbe55.css
+-rw-r--r--   0        0        0     6900 2024-04-12 14:44:35.507217 sortinghat-1.0.0rc3/sortinghat/core/static/css/488.19ce97b1.css
+-rw-r--r--   0        0        0     5954 2024-04-12 14:44:35.507217 sortinghat-1.0.0rc3/sortinghat/core/static/css/546.696b6ba4.css
+-rw-r--r--   0        0        0    10467 2024-04-12 14:44:35.507217 sortinghat-1.0.0rc3/sortinghat/core/static/css/764.ddc4524e.css
+-rw-r--r--   0        0        0     6252 2024-04-12 14:44:35.495217 sortinghat-1.0.0rc3/sortinghat/core/static/css/812.39b5238d.css
+-rw-r--r--   0        0        0    25071 2024-04-12 14:44:35.507217 sortinghat-1.0.0rc3/sortinghat/core/static/css/912.a5e49ce0.css
+-rw-r--r--   0        0        0     5368 2024-04-12 14:44:35.495217 sortinghat-1.0.0rc3/sortinghat/core/static/css/app.1adeaa19.css
+-rw-r--r--   0        0        0   698806 2024-04-12 14:44:35.507217 sortinghat-1.0.0rc3/sortinghat/core/static/css/chunk-vendors.42fea764.css
+-rw-r--r--   0        0        0    15086 2024-04-12 14:44:35.511217 sortinghat-1.0.0rc3/sortinghat/core/static/favicon-grimoirelab.ico
+-rw-r--r--   0        0        0    99428 2024-04-12 14:44:35.487217 sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-Italic.76b8308b.woff
+-rw-r--r--   0        0        0   173516 2024-04-12 14:44:35.487217 sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-Italic.991def81.ttf
+-rw-r--r--   0        0        0    30612 2024-04-12 14:44:35.487217 sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-Italic.ca10c790.woff2
+-rw-r--r--   0        0        0    93472 2024-04-12 14:44:35.483217 sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-Light.2d3c72a3.woff
+-rw-r--r--   0        0        0    65564 2024-04-12 14:44:35.483217 sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-Light.41cb61ed.woff2
+-rw-r--r--   0        0        0   170012 2024-04-12 14:44:35.483217 sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-Light.f2e7274e.ttf
+-rw-r--r--   0        0        0    72036 2024-04-12 14:44:35.483217 sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-LightItalic.07369d23.woff2
+-rw-r--r--   0        0        0   101120 2024-04-12 14:44:35.483217 sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-LightItalic.45582c0c.woff
+-rw-r--r--   0        0        0   176184 2024-04-12 14:44:35.483217 sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-LightItalic.b694f0fe.ttf
+-rw-r--r--   0        0        0    50224 2024-04-12 14:44:35.487217 sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-Medium.0519ad6f.woff2
+-rw-r--r--   0        0        0    94364 2024-04-12 14:44:35.487217 sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-Medium.483a3bd1.woff
+-rw-r--r--   0        0        0   171656 2024-04-12 14:44:35.487217 sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-Medium.af9d0139.ttf
+-rw-r--r--   0        0        0   176428 2024-04-12 14:44:35.491217 sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-MediumItalic.3723a2e7.ttf
+-rw-r--r--   0        0        0   101008 2024-04-12 14:44:35.491217 sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-MediumItalic.8b19cc18.woff
+-rw-r--r--   0        0        0   139529 2024-04-12 14:44:35.491217 sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-MediumItalic.b35d3641.woff2
+-rw-r--r--   0        0        0    93784 2024-04-12 14:44:35.487217 sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-Regular.36d4503d.woff
+-rw-r--r--   0        0        0   171272 2024-04-12 14:44:35.487217 sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-Regular.ae3a8db9.ttf
+-rw-r--r--   0        0        0    66012 2024-04-12 14:44:35.483217 sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-Regular.e0553e00.woff2
+-rw-r--r--   0        0        0  1026176 2024-04-12 14:44:35.495217 sortinghat-1.0.0rc3/sortinghat/core/static/fonts/materialdesignicons-webfont.21f691f0.ttf
+-rw-r--r--   0        0        0   325244 2024-04-12 14:44:35.495217 sortinghat-1.0.0rc3/sortinghat/core/static/fonts/materialdesignicons-webfont.54b0f60d.woff2
+-rw-r--r--   0        0        0  1026396 2024-04-12 14:44:35.491217 sortinghat-1.0.0rc3/sortinghat/core/static/fonts/materialdesignicons-webfont.5d875350.eot
+-rw-r--r--   0        0        0   465188 2024-04-12 14:44:35.495217 sortinghat-1.0.0rc3/sortinghat/core/static/fonts/materialdesignicons-webfont.d671cbf6.woff
+-rw-r--r--   0        0        0    13357 2024-04-12 14:44:35.507217 sortinghat-1.0.0rc3/sortinghat/core/static/js/105.2c5bfa40.js
+-rw-r--r--   0        0        0    30516 2024-04-12 14:44:35.515217 sortinghat-1.0.0rc3/sortinghat/core/static/js/105.2c5bfa40.js.map
+-rw-r--r--   0        0        0    66424 2024-04-12 14:44:35.495217 sortinghat-1.0.0rc3/sortinghat/core/static/js/119.6bdc5ff2.js
+-rw-r--r--   0        0        0   154025 2024-04-12 14:44:35.515217 sortinghat-1.0.0rc3/sortinghat/core/static/js/119.6bdc5ff2.js.map
+-rw-r--r--   0        0        0    54509 2024-04-12 14:44:35.515217 sortinghat-1.0.0rc3/sortinghat/core/static/js/206.75232ba8.js
+-rw-r--r--   0        0        0   131975 2024-04-12 14:44:35.543217 sortinghat-1.0.0rc3/sortinghat/core/static/js/206.75232ba8.js.map
+-rw-r--r--   0        0        0     1900 2024-04-12 14:44:35.507217 sortinghat-1.0.0rc3/sortinghat/core/static/js/253.61ce8eec.js
+-rw-r--r--   0        0        0     4676 2024-04-12 14:44:35.515217 sortinghat-1.0.0rc3/sortinghat/core/static/js/253.61ce8eec.js.map
+-rw-r--r--   0        0        0     2783 2024-04-12 14:44:35.495217 sortinghat-1.0.0rc3/sortinghat/core/static/js/414.13cae85b.js
+-rw-r--r--   0        0        0     6249 2024-04-12 14:44:35.515217 sortinghat-1.0.0rc3/sortinghat/core/static/js/414.13cae85b.js.map
+-rw-r--r--   0        0        0    23895 2024-04-12 14:44:35.507217 sortinghat-1.0.0rc3/sortinghat/core/static/js/488.0a0d2dda.js
+-rw-r--r--   0        0        0    59037 2024-04-12 14:44:35.515217 sortinghat-1.0.0rc3/sortinghat/core/static/js/488.0a0d2dda.js.map
+-rw-r--r--   0        0        0     7069 2024-04-12 14:44:35.507217 sortinghat-1.0.0rc3/sortinghat/core/static/js/544.b1834368.js
+-rw-r--r--   0        0        0    13923 2024-04-12 14:44:35.515217 sortinghat-1.0.0rc3/sortinghat/core/static/js/544.b1834368.js.map
+-rw-r--r--   0        0        0    12841 2024-04-12 14:44:35.507217 sortinghat-1.0.0rc3/sortinghat/core/static/js/546.718bab60.js
+-rw-r--r--   0        0        0    29507 2024-04-12 14:44:35.515217 sortinghat-1.0.0rc3/sortinghat/core/static/js/546.718bab60.js.map
+-rw-r--r--   0        0        0    50765 2024-04-12 14:44:35.507217 sortinghat-1.0.0rc3/sortinghat/core/static/js/689.e598fac2.js
+-rw-r--r--   0        0        0   167791 2024-04-12 14:44:35.543217 sortinghat-1.0.0rc3/sortinghat/core/static/js/689.e598fac2.js.map
+-rw-r--r--   0        0        0    14356 2024-04-12 14:44:35.507217 sortinghat-1.0.0rc3/sortinghat/core/static/js/764.5fe45faf.js
+-rw-r--r--   0        0        0    31925 2024-04-12 14:44:35.515217 sortinghat-1.0.0rc3/sortinghat/core/static/js/764.5fe45faf.js.map
+-rw-r--r--   0        0        0    23708 2024-04-12 14:44:35.495217 sortinghat-1.0.0rc3/sortinghat/core/static/js/812.711cab61.js
+-rw-r--r--   0        0        0    54522 2024-04-12 14:44:35.515217 sortinghat-1.0.0rc3/sortinghat/core/static/js/812.711cab61.js.map
+-rw-r--r--   0        0        0     3680 2024-04-12 14:44:35.495217 sortinghat-1.0.0rc3/sortinghat/core/static/js/858.8246391b.js
+-rw-r--r--   0        0        0     7696 2024-04-12 14:44:35.515217 sortinghat-1.0.0rc3/sortinghat/core/static/js/858.8246391b.js.map
+-rw-r--r--   0        0        0    58642 2024-04-12 14:44:35.515217 sortinghat-1.0.0rc3/sortinghat/core/static/js/912.ddb83f31.js
+-rw-r--r--   0        0        0   156277 2024-04-12 14:44:35.543217 sortinghat-1.0.0rc3/sortinghat/core/static/js/912.ddb83f31.js.map
+-rw-r--r--   0        0        0    14541 2024-04-12 14:44:35.495217 sortinghat-1.0.0rc3/sortinghat/core/static/js/app.014c6257.js
+-rw-r--r--   0        0        0    47793 2024-04-12 14:44:35.515217 sortinghat-1.0.0rc3/sortinghat/core/static/js/app.014c6257.js.map
+-rw-r--r--   0        0        0   922197 2024-04-12 14:44:35.507217 sortinghat-1.0.0rc3/sortinghat/core/static/js/chunk-vendors.dba6d507.js
+-rw-r--r--   0        0        0  4116361 2024-04-12 14:44:35.535217 sortinghat-1.0.0rc3/sortinghat/core/static/js/chunk-vendors.dba6d507.js.map
+-rw-r--r--   0        0        0      867 2024-04-12 14:44:35.543217 sortinghat-1.0.0rc3/sortinghat/core/templates/index.html
+-rw-r--r--   0        0        0     2436 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/tenant.py
+-rw-r--r--   0        0        0     3881 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/views.py
+-rw-r--r--   0        0        0        0 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/server/__init__.py
+-rw-r--r--   0        0        0    13717 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/server/sortinghat_admin.py
+-rw-r--r--   0        0        0     3062 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/server/sortinghatd.py
+-rw-r--r--   0        0        0     2365 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/server/sortinghatw.py
+-rwxr-xr-x   0        0        0     9218 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/server/utils/create_sh_0_7_fixture.py
+-rw-r--r--   0        0        0     3485 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/sortinghat/utils/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/cli/__init__.py
+-rw-r--r--   0        0        0       57 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/cli/config_file.cfg
+-rw-r--r--   0        0        0     7601 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/cli/test_cmd_add.py
+-rw-r--r--   0        0        0    17698 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/cli/test_cmd_config.py
+-rw-r--r--   0        0        0    10234 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/cli/test_cmd_countries.py
+-rw-r--r--   0        0        0     7597 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/cli/test_cmd_enroll.py
+-rw-r--r--   0        0        0     5397 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/cli/test_cmd_lock.py
+-rw-r--r--   0        0        0     3851 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/cli/test_cmd_merge.py
+-rw-r--r--   0        0        0     5041 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/cli/test_cmd_mv.py
+-rw-r--r--   0        0        0    13658 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/cli/test_cmd_orgs.py
+-rw-r--r--   0        0        0     9117 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/cli/test_cmd_profile.py
+-rw-r--r--   0        0        0     4599 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/cli/test_cmd_rm.py
+-rw-r--r--   0        0        0    10993 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/cli/test_cmd_show.py
+-rw-r--r--   0        0        0     5280 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/cli/test_cmd_split.py
+-rw-r--r--   0        0        0     6294 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/cli/test_cmd_withdraw.py
+-rw-r--r--   0        0        0        0 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/importer/__init__.py
+-rw-r--r--   0        0        0      159 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/importer/data/gitdm/gitdm_email_aliases_valid.txt
+-rw-r--r--   0        0        0      244 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/importer/data/gitdm/gitdm_email_to_employer_invalid.txt
+-rw-r--r--   0        0        0      249 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/importer/data/gitdm/gitdm_email_to_employer_valid.txt
+-rw-r--r--   0        0        0        0 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/importer/mocked_package/__init__.py
+-rw-r--r--   0        0        0     1055 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/importer/mocked_package/backend_a.py
+-rw-r--r--   0        0        0        0 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/importer/mocked_package/nested_package/__init__.py
+-rw-r--r--   0        0        0      950 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/importer/mocked_package/nested_package/nested_backend_b.py
+-rw-r--r--   0        0        0     1050 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/importer/mocked_package/nested_package/nested_backend_c.py
+-rw-r--r--   0        0        0      865 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/importer/mocked_package/nested_package/nested_not_backend.py
+-rw-r--r--   0        0        0     4797 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/importer/test_backend.py
+-rw-r--r--   0        0        0    25058 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/importer/test_gitdm.py
+-rw-r--r--   0        0        0     2416 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/importer/test_utils.py
+-rw-r--r--   0        0        0        0 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/rec/__init__.py
+-rw-r--r--   0        0        0    10028 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/rec/test_affiliations.py
+-rw-r--r--   0        0        0     2925 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/rec/test_engine.py
+-rw-r--r--   0        0        0     3937 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/rec/test_exclusion.py
+-rw-r--r--   0        0        0     9040 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/rec/test_gender.py
+-rw-r--r--   0        0        0    21600 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/rec/test_matches.py
+-rw-r--r--   0        0        0      825 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/runners.py
+-rw-r--r--   0        0        0        0 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/tenants/__init__.py
+-rw-r--r--   0        0        0     7242 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/tenants/test_jobs.py
+-rw-r--r--   0        0        0     2277 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/tenants/test_middleware.py
+-rw-r--r--   0        0        0     5872 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/tenants/test_schema.py
+-rw-r--r--   0        0        0   287020 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/test_api.py
+-rw-r--r--   0        0        0    18365 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/test_aux.py
+-rw-r--r--   0        0        0     9779 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/test_client.py
+-rw-r--r--   0        0        0   135031 2024-04-12 14:43:30.551004 sortinghat-1.0.0rc3/tests/test_db.py
+-rw-r--r--   0        0        0     9785 2024-04-12 14:43:30.551004 sortinghat-1.0.0rc3/tests/test_errors.py
+-rw-r--r--   0        0        0    72127 2024-04-12 14:43:30.551004 sortinghat-1.0.0rc3/tests/test_jobs.py
+-rw-r--r--   0        0        0    14074 2024-04-12 14:43:30.551004 sortinghat-1.0.0rc3/tests/test_log.py
+-rw-r--r--   0        0        0    48532 2024-04-12 14:43:30.551004 sortinghat-1.0.0rc3/tests/test_model.py
+-rw-r--r--   0        0        0   430482 2024-04-12 14:43:30.551004 sortinghat-1.0.0rc3/tests/test_schema.py
+-rw-r--r--   0        0        0     6316 2024-04-12 14:43:30.551004 sortinghat-1.0.0rc3/tests/test_utils.py
+-rw-r--r--   0        0        0    11519 1970-01-01 00:00:00.000000 sortinghat-1.0.0rc3/PKG-INFO
```

### Comparing `sortinghat-1.0.0rc2/LICENSE` & `sortinghat-1.0.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/NEWS` & `sortinghat-1.0.0rc3/NEWS`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/README.md` & `sortinghat-1.0.0rc3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 ## Requirements
 
 * Python >= 3.8
 * Poetry >= 1.1.0
 * MySQL >= 5.7 or MariaDB 10.0
-* Django = 3.2
+* Django = 4.2
 * Graphene-Django >= 2.0
 * uWSGI >= 2.0
 
 You will also need some other libraries for running the tool, you can find the
 whole list of dependencies in [pyproject.toml](pyproject.toml) file.
 
 
@@ -66,15 +66,15 @@
 ```
 
 #### Installation and configuration
 
 **Note**: these examples use `sortinghat.config.settings` configuration file.
 In order to use that configuration you need to define the environment variable
 `SORTINGHAT_SECRET_KEY` with a secret. More info here:
-https://docs.djangoproject.com/en/3.2/ref/settings/#std:setting-SECRET_KEY
+https://docs.djangoproject.com/en/4.2/ref/settings/#std:setting-SECRET_KEY
 
 
 Install the required dependencies (this will also create a virtual environment).
 ```
 $ poetry install
 ```
 
@@ -281,16 +281,16 @@
 ## Running tests
 
 SortingHat comes with a comprehensive list of unit tests for both 
 frontend and backend.
 
 #### Backend test suite
 ```
-(.venv)$ ./manage.py test --settings=config.settings.testing
-(.venv)$ ./manage.py test --settings=config.settings.testing_tenant
+(.venv)$ ./manage.py test --settings=config.settings.config_testing
+(.venv)$ ./manage.py test --settings=config.settings.config_testing_tenant
 ```
 
 #### Frontend test suite
 ```
 $ cd ui/
 $ yarn test:unit
 ```
```

### Comparing `sortinghat-1.0.0rc2/pyproject.toml` & `sortinghat-1.0.0rc3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sortinghat"
-version = "1.0.0-rc.2"
+version = "1.0.0-rc.3"
 description = "A tool to manage identities."
 authors = [
     "GrimoireLab Developers"
 ]
 license = "GPL-3.0+"
 
 readme = "README.md"
@@ -48,15 +48,15 @@
 sortinghatw = "sortinghat.server.sortinghatw:sortinghatw"
 sortinghat-admin = "sortinghat.server.sortinghat_admin:sortinghat_admin"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 
 click = "7.1.1"
-Django = "^3.2"
+Django = "^4.2"
 django-graphql-jwt = "^0.3.0"
 graphene-django = "^2.15"
 sgqlc = "^16.1"
 mysqlclient = "2.0.3"
 python-dateutil = "^2.8.2"
 requests = "^2.7.0"
 Jinja2 = "^3.1.1"
```

### Comparing `sortinghat-1.0.0rc2/sortinghat/app/schema.py` & `sortinghat-1.0.0rc3/sortinghat/app/schema.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/app/urls.py` & `sortinghat-1.0.0rc3/sortinghat/app/urls.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/cli/client/__init__.py` & `sortinghat-1.0.0rc3/sortinghat/cli/client/__init__.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/cli/client/client.py` & `sortinghat-1.0.0rc3/sortinghat/cli/client/client.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/cli/client/schema.py` & `sortinghat-1.0.0rc3/sortinghat/cli/client/schema.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/cli/cmds/add.py` & `sortinghat-1.0.0rc3/sortinghat/cli/cmds/add.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/cli/cmds/config.py` & `sortinghat-1.0.0rc3/sortinghat/cli/cmds/config.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/cli/cmds/countries.py` & `sortinghat-1.0.0rc3/sortinghat/cli/cmds/countries.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/cli/cmds/enroll.py` & `sortinghat-1.0.0rc3/sortinghat/cli/cmds/enroll.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/cli/cmds/lock.py` & `sortinghat-1.0.0rc3/sortinghat/cli/cmds/lock.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/cli/cmds/merge.py` & `sortinghat-1.0.0rc3/sortinghat/cli/cmds/merge.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/cli/cmds/mv.py` & `sortinghat-1.0.0rc3/sortinghat/cli/cmds/mv.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/cli/cmds/orgs.py` & `sortinghat-1.0.0rc3/sortinghat/cli/cmds/orgs.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/cli/cmds/profile.py` & `sortinghat-1.0.0rc3/sortinghat/cli/cmds/profile.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/cli/cmds/rm.py` & `sortinghat-1.0.0rc3/sortinghat/cli/cmds/rm.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/cli/cmds/show.py` & `sortinghat-1.0.0rc3/sortinghat/cli/cmds/show.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/cli/cmds/split.py` & `sortinghat-1.0.0rc3/sortinghat/cli/cmds/split.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/cli/cmds/withdraw.py` & `sortinghat-1.0.0rc3/sortinghat/cli/cmds/withdraw.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/cli/sortinghat.py` & `sortinghat-1.0.0rc3/sortinghat/cli/sortinghat.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/cli/templates/show.tmpl` & `sortinghat-1.0.0rc3/sortinghat/cli/templates/show.tmpl`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/cli/utils.py` & `sortinghat-1.0.0rc3/sortinghat/cli/utils.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/config/settings.py` & `sortinghat-1.0.0rc3/sortinghat/config/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,15 +170,15 @@
     ]
 
 CORS_ALLOW_CREDENTIALS = True
 
 #
 # Static files (CSS, JavaScript, Images)
 #
-# https://docs.djangoproject.com/en/3.2/howto/static-files/
+# https://docs.djangoproject.com/en/4.2/howto/static-files/
 #
 
 STATIC_URL = '/'
 
 # Use this variable to upload static files to a cloud storage.
 # Current supported cloud platforms are: GCP
 if 'SORTINGHAT_STATICFILES_STORAGE' in os.environ:
@@ -205,15 +205,14 @@
 #
 # https://docs.djangoproject.com/en/3.1/topics/i18n/
 #
 #
 
 LANGUAGE_CODE = 'en-us'
 USE_I18N = True
-USE_L10N = True
 
 #
 # Time Zone
 #
 
 USE_TZ = True
 TIME_ZONE = 'UTC'
```

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/admin.py` & `sortinghat-1.0.0rc3/sortinghat/core/admin.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/api.py` & `sortinghat-1.0.0rc3/sortinghat/core/api.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/apps.py` & `sortinghat-1.0.0rc3/sortinghat/core/apps.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/aux.py` & `sortinghat-1.0.0rc3/sortinghat/core/aux.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/context.py` & `sortinghat-1.0.0rc3/sortinghat/core/context.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/db.py` & `sortinghat-1.0.0rc3/sortinghat/core/db.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/decorators.py` & `sortinghat-1.0.0rc3/sortinghat/core/decorators.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/errors.py` & `sortinghat-1.0.0rc3/sortinghat/core/errors.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/fixtures/countries.json` & `sortinghat-1.0.0rc3/sortinghat/core/fixtures/countries.json`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/importer/backend.py` & `sortinghat-1.0.0rc3/sortinghat/core/importer/backend.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/importer/backends/gitdm.py` & `sortinghat-1.0.0rc3/sortinghat/core/importer/backends/gitdm.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/importer/backends/mailmap.py` & `sortinghat-1.0.0rc3/sortinghat/core/importer/backends/mailmap.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/importer/base.py` & `sortinghat-1.0.0rc3/sortinghat/core/importer/base.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/importer/models.py` & `sortinghat-1.0.0rc3/sortinghat/core/importer/models.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/importer/utils.py` & `sortinghat-1.0.0rc3/sortinghat/core/importer/utils.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/jobs.py` & `sortinghat-1.0.0rc3/sortinghat/core/jobs.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/log.py` & `sortinghat-1.0.0rc3/sortinghat/core/log.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/management/commands/create_groups.py` & `sortinghat-1.0.0rc3/sortinghat/core/management/commands/create_groups.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/middleware.py` & `sortinghat-1.0.0rc3/sortinghat/core/middleware.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/migrations/0001_sortinghat.py` & `sortinghat-1.0.0rc3/sortinghat/core/migrations/0001_sortinghat.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # Generated by Django 3.2.16 on 2023-01-09 10:44
 
 import datetime
 from django.db import migrations, models
 import django.db.models.deletion
-from django.utils.timezone import utc
 import grimoirelab_toolkit.datetime
 import sortinghat.core.models
 
 
 class Migration(migrations.Migration):
 
     initial = True
@@ -206,16 +205,16 @@
         ),
         migrations.CreateModel(
             name='Enrollment',
             fields=[
                 ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('created_at', sortinghat.core.models.CreationDateTimeField(default=grimoirelab_toolkit.datetime.datetime_utcnow, editable=False)),
                 ('last_modified', sortinghat.core.models.LastModificationDateTimeField(default=grimoirelab_toolkit.datetime.datetime_utcnow, editable=False)),
-                ('start', models.DateTimeField(default=datetime.datetime(1900, 1, 1, 0, 0, tzinfo=utc))),
-                ('end', models.DateTimeField(default=datetime.datetime(2100, 1, 1, 0, 0, tzinfo=utc))),
+                ('start', models.DateTimeField(default=datetime.datetime(1900, 1, 1, 0, 0, tzinfo=datetime.timezone.utc))),
+                ('end', models.DateTimeField(default=datetime.datetime(2100, 1, 1, 0, 0, tzinfo=datetime.timezone.utc))),
                 ('group', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='enrollments', to='core.group')),
                 ('individual', models.ForeignKey(db_column='mk', on_delete=django.db.models.deletion.CASCADE, related_name='enrollments', to='core.individual')),
             ],
             options={
                 'db_table': 'enrollments',
                 'ordering': ('start', 'end'),
                 'unique_together': {('individual', 'group', 'start', 'end')},
```

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/migrations/0002_importidentitiestask.py` & `sortinghat-1.0.0rc3/sortinghat/core/migrations/0002_importidentitiestask.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/migrations/0003_multi_tenancy.py` & `sortinghat-1.0.0rc3/sortinghat/core/migrations/0003_multi_tenancy.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/migrations/0004_tenant_using_header.py` & `sortinghat-1.0.0rc3/sortinghat/core/migrations/0004_tenant_using_header.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/migrations/0005_scheduledtask.py` & `sortinghat-1.0.0rc3/sortinghat/core/migrations/0005_scheduledtask.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/migrations/0006_unify_scheduled_tasks.py` & `sortinghat-1.0.0rc3/sortinghat/core/migrations/0006_unify_scheduled_tasks.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/migrations/0008_alias.py` & `sortinghat-1.0.0rc3/sortinghat/core/migrations/0008_alias.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/models.py` & `sortinghat-1.0.0rc3/sortinghat/core/models.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/recommendations/__init__.py` & `sortinghat-1.0.0rc3/sortinghat/core/recommendations/__init__.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/recommendations/affiliation.py` & `sortinghat-1.0.0rc3/sortinghat/core/recommendations/affiliation.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/recommendations/engine.py` & `sortinghat-1.0.0rc3/sortinghat/core/recommendations/engine.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/recommendations/exclusion.py` & `sortinghat-1.0.0rc3/sortinghat/core/recommendations/exclusion.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/recommendations/gender.py` & `sortinghat-1.0.0rc3/sortinghat/core/recommendations/gender.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/recommendations/matching.py` & `sortinghat-1.0.0rc3/sortinghat/core/recommendations/matching.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/schema.py` & `sortinghat-1.0.0rc3/sortinghat/core/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1096,15 +1096,15 @@
     class Arguments:
         uuids = graphene.List(graphene.String,
                               required=False)
         last_modified = graphene.DateTime(required=False)
 
     job_id = graphene.Field(lambda: graphene.String)
 
-    @check_permissions('core.execute_job')
+    @check_permissions(['core.execute_job'])
     @check_auth
     def mutate(self, info, uuids=None, last_modified=MIN_PERIOD_DATE):
         user = info.context.user
         tenant = get_db_tenant()
         ctx = SortingHatContext(user=user, tenant=tenant)
 
         job = get_tenant_queue(tenant).enqueue(recommend_affiliations,
@@ -1127,15 +1127,15 @@
         exclude = graphene.Boolean(required=False)
         strict = graphene.Boolean(required=False)
         match_source = graphene.Boolean(required=False)
         last_modified = graphene.DateTime(required=False)
 
     job_id = graphene.Field(lambda: graphene.String)
 
-    @check_permissions('core.execute_job')
+    @check_permissions(['core.execute_job'])
     @check_auth
     def mutate(self, info, criteria,
                source_uuids=None, target_uuids=None,
                exclude=True, verbose=False, strict=True,
                match_source=False, last_modified=MIN_PERIOD_DATE):
         user = info.context.user
         tenant = get_db_tenant()
@@ -1162,15 +1162,15 @@
     class Arguments:
         uuids = graphene.List(graphene.String)
         exclude = graphene.Boolean(required=False)
         no_strict_matching = graphene.Boolean(required=False)
 
     job_id = graphene.Field(lambda: graphene.String)
 
-    @check_permissions('core.execute_job')
+    @check_permissions(['core.execute_job'])
     @check_auth
     def mutate(self, info, uuids=None, exclude=True, no_strict_matching=False):
         user = info.context.user
         tenant = get_db_tenant()
         ctx = SortingHatContext(user=user, tenant=tenant)
 
         job = get_tenant_queue(tenant).enqueue(recommend_gender,
@@ -1187,15 +1187,15 @@
     class Arguments:
         uuids = graphene.List(graphene.String,
                               required=False)
         last_modified = graphene.DateTime(required=False)
 
     job_id = graphene.Field(lambda: graphene.String)
 
-    @check_permissions('core.execute_job')
+    @check_permissions(['core.execute_job'])
     @check_auth
     def mutate(self, info, uuids=None, last_modified=MIN_PERIOD_DATE):
         user = info.context.user
         tenant = get_db_tenant()
         ctx = SortingHatContext(user=user, tenant=tenant)
 
         job = get_tenant_queue(tenant).enqueue(affiliate, ctx, uuids,
@@ -1217,15 +1217,15 @@
         exclude = graphene.Boolean(required=False)
         strict = graphene.Boolean(required=False)
         match_source = graphene.Boolean(required=False)
         last_modified = graphene.DateTime(required=False)
 
     job_id = graphene.Field(lambda: graphene.String)
 
-    @check_permissions('core.execute_job')
+    @check_permissions(['core.execute_job'])
     @check_auth
     def mutate(self, info, criteria,
                source_uuids=None, target_uuids=None,
                exclude=True, strict=True,
                match_source=False,
                last_modified=MIN_PERIOD_DATE):
         user = info.context.user
@@ -1252,15 +1252,15 @@
     class Arguments:
         uuids = graphene.List(graphene.String)
         exclude = graphene.Boolean(required=False)
         no_strict_matching = graphene.Boolean(required=False)
 
     job_id = graphene.Field(lambda: graphene.String)
 
-    @check_permissions('core.execute_job')
+    @check_permissions(['core.execute_job'])
     @check_auth
     def mutate(self, info, uuids=None, exclude=True, no_strict_matching=False):
         user = info.context.user
         tenant = get_db_tenant()
         ctx = SortingHatContext(user=user, tenant=tenant)
 
         job = get_tenant_queue(tenant).enqueue(genderize, ctx, uuids,
```

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/static/css/105.858cd75e.css` & `sortinghat-1.0.0rc3/sortinghat/core/static/css/105.858cd75e.css`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/static/css/119.87ef3a04.css` & `sortinghat-1.0.0rc3/sortinghat/core/static/css/119.87ef3a04.css`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/static/css/206.7bb5d056.css` & `sortinghat-1.0.0rc3/sortinghat/core/static/css/206.7bb5d056.css`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/static/css/488.19ce97b1.css` & `sortinghat-1.0.0rc3/sortinghat/core/static/css/488.19ce97b1.css`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/static/css/546.696b6ba4.css` & `sortinghat-1.0.0rc3/sortinghat/core/static/css/546.696b6ba4.css`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/static/css/764.ddc4524e.css` & `sortinghat-1.0.0rc3/sortinghat/core/static/css/764.ddc4524e.css`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/static/css/812.39b5238d.css` & `sortinghat-1.0.0rc3/sortinghat/core/static/css/812.39b5238d.css`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/static/css/912.a5e49ce0.css` & `sortinghat-1.0.0rc3/sortinghat/core/static/css/912.a5e49ce0.css`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/static/css/app.1adeaa19.css` & `sortinghat-1.0.0rc3/sortinghat/core/static/css/app.1adeaa19.css`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/static/css/chunk-vendors.42fea764.css` & `sortinghat-1.0.0rc3/sortinghat/core/static/css/chunk-vendors.42fea764.css`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/static/favicon-grimoirelab.ico` & `sortinghat-1.0.0rc3/sortinghat/core/static/favicon-grimoirelab.ico`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/static/fonts/Roboto-Italic.76b8308b.woff` & `sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-Italic.76b8308b.woff`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/static/fonts/Roboto-Italic.991def81.ttf` & `sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-Italic.991def81.ttf`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/static/fonts/Roboto-Italic.ca10c790.woff2` & `sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-Italic.ca10c790.woff2`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/static/fonts/Roboto-Light.2d3c72a3.woff` & `sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-Light.2d3c72a3.woff`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/static/fonts/Roboto-Light.41cb61ed.woff2` & `sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-Light.41cb61ed.woff2`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/static/fonts/Roboto-Light.f2e7274e.ttf` & `sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-Light.f2e7274e.ttf`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/static/fonts/Roboto-LightItalic.07369d23.woff2` & `sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-LightItalic.07369d23.woff2`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/static/fonts/Roboto-LightItalic.45582c0c.woff` & `sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-LightItalic.45582c0c.woff`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/static/fonts/Roboto-LightItalic.b694f0fe.ttf` & `sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-LightItalic.b694f0fe.ttf`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/static/fonts/Roboto-Medium.0519ad6f.woff2` & `sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-Medium.0519ad6f.woff2`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/static/fonts/Roboto-Medium.483a3bd1.woff` & `sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-Medium.483a3bd1.woff`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/static/fonts/Roboto-Medium.af9d0139.ttf` & `sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-Medium.af9d0139.ttf`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/static/fonts/Roboto-MediumItalic.3723a2e7.ttf` & `sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-MediumItalic.3723a2e7.ttf`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/static/fonts/Roboto-MediumItalic.8b19cc18.woff` & `sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-MediumItalic.8b19cc18.woff`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/static/fonts/Roboto-MediumItalic.b35d3641.woff2` & `sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-MediumItalic.b35d3641.woff2`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/static/fonts/Roboto-Regular.36d4503d.woff` & `sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-Regular.36d4503d.woff`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/static/fonts/Roboto-Regular.ae3a8db9.ttf` & `sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-Regular.ae3a8db9.ttf`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/static/fonts/Roboto-Regular.e0553e00.woff2` & `sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-Regular.e0553e00.woff2`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/static/fonts/materialdesignicons-webfont.21f691f0.ttf` & `sortinghat-1.0.0rc3/sortinghat/core/static/fonts/materialdesignicons-webfont.21f691f0.ttf`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/static/fonts/materialdesignicons-webfont.54b0f60d.woff2` & `sortinghat-1.0.0rc3/sortinghat/core/static/fonts/materialdesignicons-webfont.54b0f60d.woff2`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/static/fonts/materialdesignicons-webfont.5d875350.eot` & `sortinghat-1.0.0rc3/sortinghat/core/static/fonts/materialdesignicons-webfont.5d875350.eot`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/static/fonts/materialdesignicons-webfont.d671cbf6.woff` & `sortinghat-1.0.0rc3/sortinghat/core/static/fonts/materialdesignicons-webfont.d671cbf6.woff`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/static/js/105.2c5bfa40.js` & `sortinghat-1.0.0rc3/sortinghat/core/static/js/105.2c5bfa40.js`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/static/js/105.2c5bfa40.js.map` & `sortinghat-1.0.0rc3/sortinghat/core/static/js/105.2c5bfa40.js.map`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/static/js/119.6bdc5ff2.js` & `sortinghat-1.0.0rc3/sortinghat/core/static/js/119.6bdc5ff2.js`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/static/js/119.6bdc5ff2.js.map` & `sortinghat-1.0.0rc3/sortinghat/core/static/js/119.6bdc5ff2.js.map`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/static/js/206.75232ba8.js` & `sortinghat-1.0.0rc3/sortinghat/core/static/js/206.75232ba8.js`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/static/js/206.75232ba8.js.map` & `sortinghat-1.0.0rc3/sortinghat/core/static/js/206.75232ba8.js.map`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/static/js/208.91e4b79e.js` & `sortinghat-1.0.0rc3/sortinghat/core/static/js/858.8246391b.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 "use strict";
 (self["webpackChunksortinghat_ui"] = self["webpackChunksortinghat_ui"] || []).push([
-    [208], {
-        80208: (e, r, s) => {
+    [858], {
+        44858: (e, r, s) => {
             s.r(r), s.d(r, {
                 default: () => k
             });
             s(62062);
             var o = s(20641),
                 n = s(53751),
                 a = s(31969),
@@ -151,20 +151,18 @@
                         }.VUE_APP_API_URL && (r = new URL({
                             NODE_ENV: "production",
                             BASE_URL: "/identities/"
                         }.VUE_APP_API_URL).origin.replace(/\/$/, "")), "".concat(r).concat(e)
                     },
                     headers: function() {
                         var e = f().get("csrftoken"),
-                            r = f().get("sh_authtoken"),
-                            s = {
-                                "X-CSRFToken": e,
-                                Authorization: "JWT ".concat(r)
+                            r = {
+                                "X-CSRFToken": e
                             };
-                        return s
+                        return r
                     }
                 },
                 methods: {
                     onSubmit: function() {
                         var e = this,
                             r = this.$refs.form_change_password.$el,
                             s = new FormData(r);
@@ -185,8 +183,8 @@
             const b = (0, g.A)(h, [
                     ["render", m]
                 ]),
                 k = b
         }
     }
 ]);
-//# sourceMappingURL=208.91e4b79e.js.map
+//# sourceMappingURL=858.8246391b.js.map
```

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/static/js/208.91e4b79e.js.map` & `sortinghat-1.0.0rc3/sortinghat/core/static/js/858.8246391b.js.map`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7837837837837839%*

 * *Differences: {"'file'": "'js/858.8246391b.js'",*

 * * "'mappings'": "'oRAK2BA,MAAM,Q,0CAJ/BC,EAAAA,EAAAA,IAqESC,EAAAA,EAAA,M,kBApEP,iBAmES,EAnETC,EAAAA,EAAAA,IAmESC,EAAAA,EAAA,CAnEDJ,MAAM,uBAAuB,YAAU,MAAMK,UAAU,IAAIC,SAAA,I,mBACjE,iBAA2D,EAA3DH,EAAAA,EAAAA,IAA2DI,EAAAA,EAAA,CAA7CP,MAAM,UAAQ,C,kBAAC,iBAAe,UAAf,mB,WAC7BG,EAAAA,EAAAA,IAgEcK,EAAAA,EAAA,CAhEDR,MAAM,QAAM,C,kBACvB,iBAGI,CAHKS,EAAAC,WAAQ,WAAjBC,EAAAA,EAAAA,IAGI,IAHJC,EAAgC,+IAGhC,eACcH,EAAAC,WAAQ,WAAtBT,EAAAA,EAAAA,IAuDSY,EAAAA,EAAA,C,MAvDeC,IAAI,wB,mBAC1B,iBAcE,EAd […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "js/208.91e4b79e.js",
-    "mappings": "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",
+    "file": "js/858.8246391b.js",
+    "mappings": "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",
     "names": [
         "class",
         "_createBlock",
         "_component_v_main",
         "_createVNode",
         "_component_v_card",
         "elevation",
@@ -50,16 +50,14 @@
         "replace",
         "VUE_APP_API_URL",
         "URL",
         "concat",
         "headers",
         "csrftoken",
         "Cookies",
-        "authtoken",
-        "Authorization",
         "methods",
         "_this",
         "HTMLForm",
         "this",
         "$refs",
         "form_change_password",
         "$el",
@@ -79,12 +77,12 @@
     ],
     "sourceRoot": "",
     "sources": [
         "webpack://sortinghat-ui/./src/views/ChangePassword.vue",
         "webpack://sortinghat-ui/./src/views/ChangePassword.vue?9dd6"
     ],
     "sourcesContent": [
-        "<template lang=\"html\">\n  <v-main>\n    <v-card class=\"mx-auto mt-6 section\" max-width=\"500\" elevation=\"0\" outlined>\n      <v-card-title class=\"header\">Password change</v-card-title>\n      <v-card-text class=\"pa-8\">\n        <p v-if=\"showForm\" class=\"mb-8\">\n          Please enter your old password, for security's sake, and then enter\n          your new password twice so we can verify you typed it in correctly.\n        </p>\n        <v-form v-if=\"showForm\" ref=\"form_change_password\">\n          <v-text-field\n            v-model=\"old_password\"\n            label=\"Old password\"\n            name=\"old_password\"\n            type=\"password\"\n            error-count=\"5\"\n            class=\"mb-4\"\n            :error-messages=\"\n              errors.old_password\n                ? errors.old_password.map((error) => error.message)\n                : []\n            \"\n            outlined\n            dense\n          />\n          <v-text-field\n            v-model=\"new_password1\"\n            label=\"New password\"\n            name=\"new_password1\"\n            type=\"password\"\n            error-count=\"5\"\n            class=\"mb-4\"\n            :error-messages=\"\n              errors.new_password1\n                ? errors.new_password1.map((error) => error.message)\n                : []\n            \"\n            outlined\n            dense\n          />\n          <v-text-field\n            v-model=\"new_password2\"\n            label=\"New password confirmation\"\n            name=\"new_password2\"\n            type=\"password\"\n            error-count=\"5\"\n            class=\"mb-4\"\n            :error-messages=\"\n              errors.new_password2\n                ? errors.new_password2.map((error) => error.message)\n                : []\n            \"\n            outlined\n            dense\n          />\n          <v-btn\n            :disabled=\"!old_password || !new_password1 || !new_password2\"\n            color=\"primary\"\n            variant=\"flat\"\n            size=\"default\"\n            @click.prevent=\"onSubmit\"\n          >\n            Save\n          </v-btn>\n        </v-form>\n        <v-alert v-else outlined type=\"success\" text>\n          Password changed successfully\n        </v-alert>\n      </v-card-text>\n    </v-card>\n  </v-main>\n</template>\n\n<script>\nimport Cookies from \"js-cookie\";\n\nexport default {\n  name: \"ChangePassword\",\n  data: () => ({\n    old_password: \"\",\n    new_password1: \"\",\n    new_password2: \"\",\n    errors: {},\n    showForm: true,\n  }),\n  computed: {\n    url() {\n      const pathname = \"/password_change/\";\n      let origin = process.env.BASE_URL.replace(/\\/$/, \"\");\n\n      if (process.env.VUE_APP_API_URL) {\n        origin = new URL(process.env.VUE_APP_API_URL).origin.replace(/\\/$/, \"\");\n      }\n\n      return `${origin}${pathname}`;\n    },\n    headers() {\n      const csrftoken = Cookies.get(\"csrftoken\");\n      const authtoken = Cookies.get(\"sh_authtoken\");\n      const headers = {\n        \"X-CSRFToken\": csrftoken,\n        Authorization: `JWT ${authtoken}`,\n      };\n\n      return headers;\n    },\n  },\n  methods: {\n    onSubmit() {\n      const HTMLForm = this.$refs.form_change_password.$el;\n      const body = new FormData(HTMLForm);\n\n      this.errors = {};\n\n      fetch(this.url, {\n        method: \"POST\",\n        credentials: \"include\",\n        headers: this.headers,\n        body: body,\n      })\n        .then((response) => response.json())\n        .then((data) => {\n          if (data.errors) {\n            this.errors = data.errors;\n            this.$logger.error(\"Error changing password\", data);\n          } else {\n            this.showForm = false;\n            this.$logger.info(`Changed password for user ${data.updated}`);\n          }\n        });\n    },\n  },\n};\n</script>\n",
-        "import { render } from \"./ChangePassword.vue?vue&type=template&id=7243c725&lang=html\"\nimport script from \"./ChangePassword.vue?vue&type=script&lang=js\"\nexport * from \"./ChangePassword.vue?vue&type=script&lang=js\"\n\nimport exportComponent from \"../../node_modules/@vue/cli-service/node_modules/vue-loader/dist/exportHelper.js\"\nconst __exports__ = /*#__PURE__*/exportComponent(script, [['render',render]])\n\nexport default __exports__"
+        "<template lang=\"html\">\n  <v-main>\n    <v-card class=\"mx-auto mt-6 section\" max-width=\"500\" elevation=\"0\" outlined>\n      <v-card-title class=\"header\">Password change</v-card-title>\n      <v-card-text class=\"pa-8\">\n        <p v-if=\"showForm\" class=\"mb-8\">\n          Please enter your old password, for security's sake, and then enter\n          your new password twice so we can verify you typed it in correctly.\n        </p>\n        <v-form v-if=\"showForm\" ref=\"form_change_password\">\n          <v-text-field\n            v-model=\"old_password\"\n            label=\"Old password\"\n            name=\"old_password\"\n            type=\"password\"\n            error-count=\"5\"\n            class=\"mb-4\"\n            :error-messages=\"\n              errors.old_password\n                ? errors.old_password.map((error) => error.message)\n                : []\n            \"\n            outlined\n            dense\n          />\n          <v-text-field\n            v-model=\"new_password1\"\n            label=\"New password\"\n            name=\"new_password1\"\n            type=\"password\"\n            error-count=\"5\"\n            class=\"mb-4\"\n            :error-messages=\"\n              errors.new_password1\n                ? errors.new_password1.map((error) => error.message)\n                : []\n            \"\n            outlined\n            dense\n          />\n          <v-text-field\n            v-model=\"new_password2\"\n            label=\"New password confirmation\"\n            name=\"new_password2\"\n            type=\"password\"\n            error-count=\"5\"\n            class=\"mb-4\"\n            :error-messages=\"\n              errors.new_password2\n                ? errors.new_password2.map((error) => error.message)\n                : []\n            \"\n            outlined\n            dense\n          />\n          <v-btn\n            :disabled=\"!old_password || !new_password1 || !new_password2\"\n            color=\"primary\"\n            variant=\"flat\"\n            size=\"default\"\n            @click.prevent=\"onSubmit\"\n          >\n            Save\n          </v-btn>\n        </v-form>\n        <v-alert v-else outlined type=\"success\" text>\n          Password changed successfully\n        </v-alert>\n      </v-card-text>\n    </v-card>\n  </v-main>\n</template>\n\n<script>\nimport Cookies from \"js-cookie\";\n\nexport default {\n  name: \"ChangePassword\",\n  data: () => ({\n    old_password: \"\",\n    new_password1: \"\",\n    new_password2: \"\",\n    errors: {},\n    showForm: true,\n  }),\n  computed: {\n    url() {\n      const pathname = \"/password_change/\";\n      let origin = process.env.BASE_URL.replace(/\\/$/, \"\");\n\n      if (process.env.VUE_APP_API_URL) {\n        origin = new URL(process.env.VUE_APP_API_URL).origin.replace(/\\/$/, \"\");\n      }\n\n      return `${origin}${pathname}`;\n    },\n    headers() {\n      const csrftoken = Cookies.get(\"csrftoken\");\n      const headers = {\n        \"X-CSRFToken\": csrftoken,\n      };\n\n      return headers;\n    },\n  },\n  methods: {\n    onSubmit() {\n      const HTMLForm = this.$refs.form_change_password.$el;\n      const body = new FormData(HTMLForm);\n\n      this.errors = {};\n\n      fetch(this.url, {\n        method: \"POST\",\n        credentials: \"include\",\n        headers: this.headers,\n        body: body,\n      })\n        .then((response) => response.json())\n        .then((data) => {\n          if (data.errors) {\n            this.errors = data.errors;\n            this.$logger.error(\"Error changing password\", data);\n          } else {\n            this.showForm = false;\n            this.$logger.info(`Changed password for user ${data.updated}`);\n          }\n        });\n    },\n  },\n};\n</script>\n",
+        "import { render } from \"./ChangePassword.vue?vue&type=template&id=0b632147&lang=html\"\nimport script from \"./ChangePassword.vue?vue&type=script&lang=js\"\nexport * from \"./ChangePassword.vue?vue&type=script&lang=js\"\n\nimport exportComponent from \"../../node_modules/@vue/cli-service/node_modules/vue-loader/dist/exportHelper.js\"\nconst __exports__ = /*#__PURE__*/exportComponent(script, [['render',render]])\n\nexport default __exports__"
     ],
     "version": 3
 }
```

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/static/js/253.61ce8eec.js` & `sortinghat-1.0.0rc3/sortinghat/core/static/js/253.61ce8eec.js`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/static/js/253.61ce8eec.js.map` & `sortinghat-1.0.0rc3/sortinghat/core/static/js/253.61ce8eec.js.map`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/static/js/414.13cae85b.js` & `sortinghat-1.0.0rc3/sortinghat/core/static/js/414.13cae85b.js`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/static/js/414.13cae85b.js.map` & `sortinghat-1.0.0rc3/sortinghat/core/static/js/414.13cae85b.js.map`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/static/js/488.0a0d2dda.js` & `sortinghat-1.0.0rc3/sortinghat/core/static/js/488.0a0d2dda.js`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/static/js/488.0a0d2dda.js.map` & `sortinghat-1.0.0rc3/sortinghat/core/static/js/488.0a0d2dda.js.map`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/static/js/544.b1834368.js` & `sortinghat-1.0.0rc3/sortinghat/core/static/js/544.b1834368.js`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/static/js/544.b1834368.js.map` & `sortinghat-1.0.0rc3/sortinghat/core/static/js/544.b1834368.js.map`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/static/js/546.718bab60.js` & `sortinghat-1.0.0rc3/sortinghat/core/static/js/546.718bab60.js`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/static/js/546.718bab60.js.map` & `sortinghat-1.0.0rc3/sortinghat/core/static/js/546.718bab60.js.map`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/static/js/689.e598fac2.js` & `sortinghat-1.0.0rc3/sortinghat/core/static/js/689.e598fac2.js`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/static/js/689.e598fac2.js.map` & `sortinghat-1.0.0rc3/sortinghat/core/static/js/689.e598fac2.js.map`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/static/js/764.5fe45faf.js` & `sortinghat-1.0.0rc3/sortinghat/core/static/js/764.5fe45faf.js`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/static/js/764.5fe45faf.js.map` & `sortinghat-1.0.0rc3/sortinghat/core/static/js/764.5fe45faf.js.map`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/static/js/812.711cab61.js` & `sortinghat-1.0.0rc3/sortinghat/core/static/js/812.711cab61.js`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/static/js/812.711cab61.js.map` & `sortinghat-1.0.0rc3/sortinghat/core/static/js/812.711cab61.js.map`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/static/js/912.ddb83f31.js` & `sortinghat-1.0.0rc3/sortinghat/core/static/js/912.ddb83f31.js`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/static/js/912.ddb83f31.js.map` & `sortinghat-1.0.0rc3/sortinghat/core/static/js/912.ddb83f31.js.map`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/static/js/app.ba14e94f.js` & `sortinghat-1.0.0rc3/sortinghat/core/static/js/app.014c6257.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -340,15 +340,15 @@
                             requiresAuth: !0,
                             title: "Sorting Hat"
                         }
                     }, {
                         path: "/change-password",
                         name: "ChangePassword",
                         component: function() {
-                            return r.e(208).then(r.bind(r, 80208))
+                            return r.e(858).then(r.bind(r, 44858))
                         },
                         meta: {
                             requiresAuth: !0,
                             title: "Password change - Sorting Hat"
                         }
                     }, {
                         path: "/login",
@@ -633,23 +633,23 @@
     })(), (() => {
         r.f = {}, r.e = e => Promise.all(Object.keys(r.f).reduce(((t, n) => (r.f[n](e, t), t)), []))
     })(), (() => {
         r.u = e => "js/" + e + "." + {
             105: "2c5bfa40",
             119: "6bdc5ff2",
             206: "75232ba8",
-            208: "91e4b79e",
             253: "61ce8eec",
             414: "13cae85b",
             488: "0a0d2dda",
             544: "b1834368",
             546: "718bab60",
             689: "e598fac2",
             764: "5fe45faf",
             812: "711cab61",
+            858: "8246391b",
             912: "ddb83f31"
         } [e] + ".js"
     })(), (() => {
         r.miniCssF = e => "css/" + e + "." + {
             105: "858cd75e",
             119: "87ef3a04",
             206: "7bb5d056",
@@ -800,8 +800,8 @@
             },
             n = self["webpackChunksortinghat_ui"] = self["webpackChunksortinghat_ui"] || [];
         n.forEach(t.bind(null, 0)), n.push = t.bind(null, n.push.bind(n))
     })();
     var n = r.O(void 0, [504], (() => r(55864)));
     n = r.O(n)
 })();
-//# sourceMappingURL=app.ba14e94f.js.map
+//# sourceMappingURL=app.014c6257.js.map
```

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/static/js/app.ba14e94f.js.map` & `sortinghat-1.0.0rc3/sortinghat/core/static/js/app.014c6257.js.map`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9226190476190476%*

 * *Differences: {"'file'": "'js/app.014c6257.js'",*

 * * "'sourcesContent'": "{insert: [(13, '// This function allow to reference async "*

 * *                     'chunks\\n__webpack_require__.u = (chunkId) => {\\n\\t// return url for '*

 * *                     'filenames based on template\\n\\treturn "js/" + chunkId + "." + '*

 * *                     '{"105":"2c5bfa40","119":"6bdc5ff2","206":"75232ba8","253":"61ce8eec","414":"13cae85b","488":"0a0d2dda","544":"b1834368","546":"718bab60","689":"e598fac2","764":"5fe45faf","812":"711cab61","8 […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "file": "js/app.ba14e94f.js",
+    "file": "js/app.014c6257.js",
     "mappings": "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",
     "names": [
         "key",
         "_createBlock",
         "_component_v_app",
         "_withCtx",
         "_createVNode",
@@ -410,15 +410,15 @@
         "const errorMessages = {\n  install(app) {\n    const ERRORS = {\n      14: `The individual is already enrolled in the organization on the\n        selected dates.`,\n      129: `Invalid credentials. Please check your username and password and\n        try again.`,\n    };\n\n    app.config.globalProperties.$getErrorMessage = (error) => {\n      if (error.graphQLErrors && error.graphQLErrors.length > 0) {\n        return error.graphQLErrors\n          .map((error) => {\n            const code = error.extensions.code;\n            return ERRORS[code] || error.message;\n          })\n          .join(\". \");\n      } else if (error.networkError) {\n        if (error.networkError.result) {\n          return error.networkError.result.errors\n            .map((error) => error.message)\n            .join(\". \");\n        } else {\n          return error.networkError.message;\n        }\n      }\n      return error.message;\n    };\n  },\n};\n\nexport default errorMessages;\n",
         "import { createApp } from \"vue\";\nimport App from \"./App.vue\";\nimport router from \"./router\";\nimport { store } from \"./store\";\nimport Cookies from \"js-cookie\";\nimport { createApolloProvider } from \"@vue/apollo-option\";\nimport {\n  ApolloClient,\n  ApolloLink,\n  createHttpLink,\n  InMemoryCache,\n  defaultDataIdFromObject,\n} from \"@apollo/client/core\";\nimport vuetify from \"./plugins/vuetify\";\nimport logger from \"./plugins/logger\";\nimport errorMessages from \"./plugins/errors\";\n\nconst API_URL = process.env.VUE_APP_API_URL || `${process.env.BASE_URL}api/`;\n\n// HTTP connection to the API\nconst httpLink = createHttpLink({\n  uri: API_URL,\n  credentials: \"include\",\n});\n\n// Cache implementation\n// Specify object IDs so Apollo can update the cache automatically\n// https://www.apollographql.com/docs/react/v2/caching/cache-configuration/#custom-identifiers\nconst cache = new InMemoryCache({\n  dataIdFromObject: (object) => {\n    switch (object.__typename) {\n      case \"IndividualType\":\n        return object.mk;\n      case \"IdentityType\":\n        return object.uuid;\n      default:\n        return defaultDataIdFromObject(object);\n    }\n  },\n});\n\nconst AuthLink = (operation, next) => {\n  const csrftoken = Cookies.get(\"csrftoken\");\n\n  operation.setContext((context) => ({\n    ...context,\n    headers: {\n      ...context.headers,\n      \"X-CSRFToken\": csrftoken,\n    },\n  }));\n  return next(operation);\n};\n\nconst link = ApolloLink.from([AuthLink, httpLink]);\n\n// Create the apollo client\nconst apolloClient = new ApolloClient({\n  link: link,\n  cache,\n});\n\nconst apolloProvider = new createApolloProvider({\n  defaultClient: apolloClient,\n});\n\ncreateApp(App)\n  .use(apolloProvider)\n  .use(errorMessages)\n  .use(logger)\n  .use(store)\n  .use(router)\n  .use(vuetify)\n  .mount(\"#app\");\n",
         "// The module cache\nvar __webpack_module_cache__ = {};\n\n// The require function\nfunction __webpack_require__(moduleId) {\n\t// Check if module is in cache\n\tvar cachedModule = __webpack_module_cache__[moduleId];\n\tif (cachedModule !== undefined) {\n\t\treturn cachedModule.exports;\n\t}\n\t// Create a new module (and put it into the cache)\n\tvar module = __webpack_module_cache__[moduleId] = {\n\t\t// no module.id needed\n\t\t// no module.loaded needed\n\t\texports: {}\n\t};\n\n\t// Execute the module function\n\t__webpack_modules__[moduleId].call(module.exports, module, module.exports, __webpack_require__);\n\n\t// Return the exports of the module\n\treturn module.exports;\n}\n\n// expose the modules object (__webpack_modules__)\n__webpack_require__.m = __webpack_modules__;\n\n",
         "var deferred = [];\n__webpack_require__.O = (result, chunkIds, fn, priority) => {\n\tif(chunkIds) {\n\t\tpriority = priority || 0;\n\t\tfor(var i = deferred.length; i > 0 && deferred[i - 1][2] > priority; i--) deferred[i] = deferred[i - 1];\n\t\tdeferred[i] = [chunkIds, fn, priority];\n\t\treturn;\n\t}\n\tvar notFulfilled = Infinity;\n\tfor (var i = 0; i < deferred.length; i++) {\n\t\tvar [chunkIds, fn, priority] = deferred[i];\n\t\tvar fulfilled = true;\n\t\tfor (var j = 0; j < chunkIds.length; j++) {\n\t\t\tif ((priority & 1 === 0 || notFulfilled >= priority) && Object.keys(__webpack_require__.O).every((key) => (__webpack_require__.O[key](chunkIds[j])))) {\n\t\t\t\tchunkIds.splice(j--, 1);\n\t\t\t} else {\n\t\t\t\tfulfilled = false;\n\t\t\t\tif(priority < notFulfilled) notFulfilled = priority;\n\t\t\t}\n\t\t}\n\t\tif(fulfilled) {\n\t\t\tdeferred.splice(i--, 1)\n\t\t\tvar r = fn();\n\t\t\tif (r !== undefined) result = r;\n\t\t}\n\t}\n\treturn result;\n};",
         "// getDefaultExport function for compatibility with non-harmony modules\n__webpack_require__.n = (module) => {\n\tvar getter = module && module.__esModule ?\n\t\t() => (module['default']) :\n\t\t() => (module);\n\t__webpack_require__.d(getter, { a: getter });\n\treturn getter;\n};",
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.f = {};\n// This file contains only the entry chunk.\n// The chunk loading function for additional chunks\n__webpack_require__.e = (chunkId) => {\n\treturn Promise.all(Object.keys(__webpack_require__.f).reduce((promises, key) => {\n\t\t__webpack_require__.f[key](chunkId, promises);\n\t\treturn promises;\n\t}, []));\n};",
-        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"js/\" + chunkId + \".\" + {\"105\":\"2c5bfa40\",\"119\":\"6bdc5ff2\",\"206\":\"75232ba8\",\"208\":\"91e4b79e\",\"253\":\"61ce8eec\",\"414\":\"13cae85b\",\"488\":\"0a0d2dda\",\"544\":\"b1834368\",\"546\":\"718bab60\",\"689\":\"e598fac2\",\"764\":\"5fe45faf\",\"812\":\"711cab61\",\"912\":\"ddb83f31\"}[chunkId] + \".js\";\n};",
+        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"js/\" + chunkId + \".\" + {\"105\":\"2c5bfa40\",\"119\":\"6bdc5ff2\",\"206\":\"75232ba8\",\"253\":\"61ce8eec\",\"414\":\"13cae85b\",\"488\":\"0a0d2dda\",\"544\":\"b1834368\",\"546\":\"718bab60\",\"689\":\"e598fac2\",\"764\":\"5fe45faf\",\"812\":\"711cab61\",\"858\":\"8246391b\",\"912\":\"ddb83f31\"}[chunkId] + \".js\";\n};",
         "// This function allow to reference async chunks\n__webpack_require__.miniCssF = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"css/\" + chunkId + \".\" + {\"105\":\"858cd75e\",\"119\":\"87ef3a04\",\"206\":\"7bb5d056\",\"253\":\"193dbe55\",\"488\":\"19ce97b1\",\"546\":\"696b6ba4\",\"764\":\"ddc4524e\",\"812\":\"39b5238d\",\"912\":\"a5e49ce0\"}[chunkId] + \".css\";\n};",
         "__webpack_require__.g = (function() {\n\tif (typeof globalThis === 'object') return globalThis;\n\ttry {\n\t\treturn this || new Function('return this')();\n\t} catch (e) {\n\t\tif (typeof window === 'object') return window;\n\t}\n})();",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "var inProgress = {};\nvar dataWebpackPrefix = \"sortinghat-ui:\";\n// loadScript function to load a script via script tag\n__webpack_require__.l = (url, done, key, chunkId) => {\n\tif(inProgress[url]) { inProgress[url].push(done); return; }\n\tvar script, needAttach;\n\tif(key !== undefined) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tfor(var i = 0; i < scripts.length; i++) {\n\t\t\tvar s = scripts[i];\n\t\t\tif(s.getAttribute(\"src\") == url || s.getAttribute(\"data-webpack\") == dataWebpackPrefix + key) { script = s; break; }\n\t\t}\n\t}\n\tif(!script) {\n\t\tneedAttach = true;\n\t\tscript = document.createElement('script');\n\n\t\tscript.charset = 'utf-8';\n\t\tscript.timeout = 120;\n\t\tif (__webpack_require__.nc) {\n\t\t\tscript.setAttribute(\"nonce\", __webpack_require__.nc);\n\t\t}\n\t\tscript.setAttribute(\"data-webpack\", dataWebpackPrefix + key);\n\n\t\tscript.src = url;\n\t}\n\tinProgress[url] = [done];\n\tvar onScriptComplete = (prev, event) => {\n\t\t// avoid mem leaks in IE.\n\t\tscript.onerror = script.onload = null;\n\t\tclearTimeout(timeout);\n\t\tvar doneFns = inProgress[url];\n\t\tdelete inProgress[url];\n\t\tscript.parentNode && script.parentNode.removeChild(script);\n\t\tdoneFns && doneFns.forEach((fn) => (fn(event)));\n\t\tif(prev) return prev(event);\n\t}\n\tvar timeout = setTimeout(onScriptComplete.bind(null, undefined, { type: 'timeout', target: script }), 120000);\n\tscript.onerror = onScriptComplete.bind(null, script.onerror);\n\tscript.onload = onScriptComplete.bind(null, script.onload);\n\tneedAttach && document.head.appendChild(script);\n};",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
         "__webpack_require__.p = \"/identities/\";",
         "if (typeof document === \"undefined\") return;\nvar createStylesheet = (chunkId, fullhref, oldTag, resolve, reject) => {\n\tvar linkTag = document.createElement(\"link\");\n\n\tlinkTag.rel = \"stylesheet\";\n\tlinkTag.type = \"text/css\";\n\tif (__webpack_require__.nc) {\n\t\tlinkTag.nonce = __webpack_require__.nc;\n\t}\n\tvar onLinkComplete = (event) => {\n\t\t// avoid mem leaks.\n\t\tlinkTag.onerror = linkTag.onload = null;\n\t\tif (event.type === 'load') {\n\t\t\tresolve();\n\t\t} else {\n\t\t\tvar errorType = event && event.type;\n\t\t\tvar realHref = event && event.target && event.target.href || fullhref;\n\t\t\tvar err = new Error(\"Loading CSS chunk \" + chunkId + \" failed.\\n(\" + errorType + \": \" + realHref + \")\");\n\t\t\terr.name = \"ChunkLoadError\";\n\t\t\terr.code = \"CSS_CHUNK_LOAD_FAILED\";\n\t\t\terr.type = errorType;\n\t\t\terr.request = realHref;\n\t\t\tif (linkTag.parentNode) linkTag.parentNode.removeChild(linkTag)\n\t\t\treject(err);\n\t\t}\n\t}\n\tlinkTag.onerror = linkTag.onload = onLinkComplete;\n\tlinkTag.href = fullhref;\n\n\n\tif (oldTag) {\n\t\toldTag.parentNode.insertBefore(linkTag, oldTag.nextSibling);\n\t} else {\n\t\tdocument.head.appendChild(linkTag);\n\t}\n\treturn linkTag;\n};\nvar findStylesheet = (href, fullhref) => {\n\tvar existingLinkTags = document.getElementsByTagName(\"link\");\n\tfor(var i = 0; i < existingLinkTags.length; i++) {\n\t\tvar tag = existingLinkTags[i];\n\t\tvar dataHref = tag.getAttribute(\"data-href\") || tag.getAttribute(\"href\");\n\t\tif(tag.rel === \"stylesheet\" && (dataHref === href || dataHref === fullhref)) return tag;\n\t}\n\tvar existingStyleTags = document.getElementsByTagName(\"style\");\n\tfor(var i = 0; i < existingStyleTags.length; i++) {\n\t\tvar tag = existingStyleTags[i];\n\t\tvar dataHref = tag.getAttribute(\"data-href\");\n\t\tif(dataHref === href || dataHref === fullhref) return tag;\n\t}\n};\nvar loadStylesheet = (chunkId) => {\n\treturn new Promise((resolve, reject) => {\n\t\tvar href = __webpack_require__.miniCssF(chunkId);\n\t\tvar fullhref = __webpack_require__.p + href;\n\t\tif(findStylesheet(href, fullhref)) return resolve();\n\t\tcreateStylesheet(chunkId, fullhref, null, resolve, reject);\n\t});\n}\n// object to store loaded CSS chunks\nvar installedCssChunks = {\n\t524: 0\n};\n\n__webpack_require__.f.miniCss = (chunkId, promises) => {\n\tvar cssChunks = {\"105\":1,\"119\":1,\"206\":1,\"253\":1,\"488\":1,\"546\":1,\"764\":1,\"812\":1,\"912\":1};\n\tif(installedCssChunks[chunkId]) promises.push(installedCssChunks[chunkId]);\n\telse if(installedCssChunks[chunkId] !== 0 && cssChunks[chunkId]) {\n\t\tpromises.push(installedCssChunks[chunkId] = loadStylesheet(chunkId).then(() => {\n\t\t\tinstalledCssChunks[chunkId] = 0;\n\t\t}, (e) => {\n\t\t\tdelete installedCssChunks[chunkId];\n\t\t\tthrow e;\n\t\t}));\n\t}\n};\n\n// no hmr",
```

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/static/js/chunk-vendors.dba6d507.js` & `sortinghat-1.0.0rc3/sortinghat/core/static/js/chunk-vendors.dba6d507.js`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/static/js/chunk-vendors.dba6d507.js.map` & `sortinghat-1.0.0rc3/sortinghat/core/static/js/chunk-vendors.dba6d507.js.map`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/templates/index.html` & `sortinghat-1.0.0rc3/sortinghat/core/templates/index.html`

 * *Files 12% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><meta charset="utf-8"><meta http-equiv="X-UA-Compatible" content="IE=edge"><meta name="viewport" content="width=device-width,initial-scale=1"><link rel="icon" href="/identities/favicon-grimoirelab.ico"><title>sortinghat-ui</title><link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@mdi/font@latest/css/materialdesignicons.min.css"><script defer="defer" src="/identities/js/chunk-vendors.dba6d507.js"></script><script defer="defer" src="/identities/js/app.ba14e94f.js"></script><link href="/identities/css/chunk-vendors.42fea764.css" rel="stylesheet"><link href="/identities/css/app.1adeaa19.css" rel="stylesheet"></head><body><noscript><strong>We're sorry but sortinghat-ui doesn't work properly without JavaScript enabled. Please enable it to continue.</strong></noscript>{% csrf_token %}<div id="app"></div></body></html>
+<!doctype html><html lang="en"><head><meta charset="utf-8"><meta http-equiv="X-UA-Compatible" content="IE=edge"><meta name="viewport" content="width=device-width,initial-scale=1"><link rel="icon" href="/identities/favicon-grimoirelab.ico"><title>sortinghat-ui</title><link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@mdi/font@latest/css/materialdesignicons.min.css"><script defer="defer" src="/identities/js/chunk-vendors.dba6d507.js"></script><script defer="defer" src="/identities/js/app.014c6257.js"></script><link href="/identities/css/chunk-vendors.42fea764.css" rel="stylesheet"><link href="/identities/css/app.1adeaa19.css" rel="stylesheet"></head><body><noscript><strong>We're sorry but sortinghat-ui doesn't work properly without JavaScript enabled. Please enable it to continue.</strong></noscript>{% csrf_token %}<div id="app"></div></body></html>
```

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/tenant.py` & `sortinghat-1.0.0rc3/sortinghat/core/tenant.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/core/views.py` & `sortinghat-1.0.0rc3/sortinghat/core/views.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/server/sortinghat_admin.py` & `sortinghat-1.0.0rc3/sortinghat/server/sortinghat_admin.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/server/sortinghatd.py` & `sortinghat-1.0.0rc3/sortinghat/server/sortinghatd.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/server/sortinghatw.py` & `sortinghat-1.0.0rc3/sortinghat/server/sortinghatw.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/server/utils/create_sh_0_7_fixture.py` & `sortinghat-1.0.0rc3/sortinghat/server/utils/create_sh_0_7_fixture.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/sortinghat/utils/__init__.py` & `sortinghat-1.0.0rc3/sortinghat/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/tests/cli/test_cmd_add.py` & `sortinghat-1.0.0rc3/tests/cli/test_cmd_add.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/tests/cli/test_cmd_config.py` & `sortinghat-1.0.0rc3/tests/cli/test_cmd_config.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/tests/cli/test_cmd_countries.py` & `sortinghat-1.0.0rc3/tests/cli/test_cmd_countries.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/tests/cli/test_cmd_enroll.py` & `sortinghat-1.0.0rc3/tests/cli/test_cmd_enroll.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/tests/cli/test_cmd_lock.py` & `sortinghat-1.0.0rc3/tests/cli/test_cmd_lock.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/tests/cli/test_cmd_merge.py` & `sortinghat-1.0.0rc3/tests/cli/test_cmd_merge.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/tests/cli/test_cmd_mv.py` & `sortinghat-1.0.0rc3/tests/cli/test_cmd_mv.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/tests/cli/test_cmd_orgs.py` & `sortinghat-1.0.0rc3/tests/cli/test_cmd_orgs.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/tests/cli/test_cmd_profile.py` & `sortinghat-1.0.0rc3/tests/cli/test_cmd_profile.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/tests/cli/test_cmd_rm.py` & `sortinghat-1.0.0rc3/tests/cli/test_cmd_rm.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/tests/cli/test_cmd_show.py` & `sortinghat-1.0.0rc3/tests/cli/test_cmd_show.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/tests/cli/test_cmd_split.py` & `sortinghat-1.0.0rc3/tests/cli/test_cmd_split.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/tests/cli/test_cmd_withdraw.py` & `sortinghat-1.0.0rc3/tests/cli/test_cmd_withdraw.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/tests/importer/mocked_package/backend_a.py` & `sortinghat-1.0.0rc3/tests/importer/mocked_package/backend_a.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/tests/importer/mocked_package/nested_package/nested_backend_b.py` & `sortinghat-1.0.0rc3/tests/importer/mocked_package/nested_package/nested_backend_b.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/tests/importer/mocked_package/nested_package/nested_backend_c.py` & `sortinghat-1.0.0rc3/tests/importer/mocked_package/nested_package/nested_backend_c.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/tests/importer/mocked_package/nested_package/nested_not_backend.py` & `sortinghat-1.0.0rc3/tests/importer/mocked_package/nested_package/nested_not_backend.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/tests/importer/test_backend.py` & `sortinghat-1.0.0rc3/tests/importer/test_backend.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/tests/importer/test_gitdm.py` & `sortinghat-1.0.0rc3/tests/importer/test_gitdm.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/tests/importer/test_utils.py` & `sortinghat-1.0.0rc3/tests/importer/test_utils.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/tests/rec/test_affiliations.py` & `sortinghat-1.0.0rc3/tests/rec/test_affiliations.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/tests/rec/test_engine.py` & `sortinghat-1.0.0rc3/tests/rec/test_engine.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/tests/rec/test_exclusion.py` & `sortinghat-1.0.0rc3/tests/rec/test_exclusion.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/tests/rec/test_gender.py` & `sortinghat-1.0.0rc3/tests/rec/test_gender.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/tests/rec/test_matches.py` & `sortinghat-1.0.0rc3/tests/rec/test_matches.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/tests/runners.py` & `sortinghat-1.0.0rc3/tests/runners.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/tests/tenants/test_jobs.py` & `sortinghat-1.0.0rc3/tests/tenants/test_jobs.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,11 +191,11 @@
 
         queue = jobs.get_tenant_queue('tenant_2')
         self.assertEqual(queue.name, 'default')
 
     def test_not_found_queue(self):
         """Check it an error is raised when the queue is not found"""
 
-        # The configuration in settings.testing_tenant ignores
+        # The configuration in settings.config_testing_tenant ignores
         # the creation of this queue, so it should raise an error.
         with self.assertRaisesRegex(JobError, "Queue 'error_tenant' not found."):
             jobs.get_tenant_queue('error_tenant')
```

### Comparing `sortinghat-1.0.0rc2/tests/tenants/test_middleware.py` & `sortinghat-1.0.0rc3/tests/tenants/test_middleware.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/tests/tenants/test_schema.py` & `sortinghat-1.0.0rc3/tests/tenants/test_schema.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/tests/test_api.py` & `sortinghat-1.0.0rc3/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/tests/test_aux.py` & `sortinghat-1.0.0rc3/tests/test_aux.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/tests/test_client.py` & `sortinghat-1.0.0rc3/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/tests/test_db.py` & `sortinghat-1.0.0rc3/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/tests/test_errors.py` & `sortinghat-1.0.0rc3/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/tests/test_jobs.py` & `sortinghat-1.0.0rc3/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/tests/test_log.py` & `sortinghat-1.0.0rc3/tests/test_log.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/tests/test_model.py` & `sortinghat-1.0.0rc3/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/tests/test_schema.py` & `sortinghat-1.0.0rc3/tests/test_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,14 @@
 ORGANIZATION_EXAMPLE_DOES_NOT_EXIST_ERROR = "Example not found in the registry"
 ORGANIZATION_LIBRESOFT_DOES_NOT_EXIST_ERROR = "LibreSoft not found in the registry"
 TEAM_EXAMPLE_DOES_NOT_EXIST_ERROR = "Example_team not found in the registry"
 ENROLLMENT_DOES_NOT_EXIST_ERROR = "enrollment with range '2050-01-01 00:00:00+00:00'-'2060-01-01 00:00:00+00:00'"\
                                   " for Example not found in the registry"
 PAGINATION_NO_RESULTS_ERROR = "That page contains no results"
 PAGINATION_PAGE_LESS_THAN_ONE_ERROR = "That page number is less than 1"
-PAGINATION_PAGE_SIZE_NEGATIVE_ERROR = "Negative indexing is not supported."
 PAGINATION_PAGE_SIZE_ZERO_ERROR = "division by zero"
 AUTHENTICATION_ERROR = "You do not have permission to perform this action"
 PARSE_DATE_INVALID_DATE_ERROR = "{} is not a valid date"
 PARSE_DATE_INVALID_FORMAT_ERROR = "Filter format is not valid"
 INVALID_FILTER_DATE_ERROR = "Error in {} filter: {} is not a valid date"
 INVALID_FILTER_FORMAT_ERROR = "Error in {} filter: Filter format is not valid"
 INVALID_FILTER_RANGE_ERROR = "Error in {} filter: Date range is invalid. {}"
@@ -1414,15 +1413,15 @@
 
         client = graphene.test.Client(schema)
         test_query = SH_OPERATIONS_QUERY_PAGINATION % (1, -2)
         executed = client.execute(test_query,
                                   context_value=self.context_value)
 
         msg = executed['errors'][0]['message']
-        self.assertEqual(msg, PAGINATION_PAGE_SIZE_NEGATIVE_ERROR)
+        self.assertEqual(msg, PAGINATION_NO_RESULTS_ERROR)
 
     def test_page_size_zero(self):
         """Check if it fails when `pageSize` is set to `0`"""
 
         client = graphene.test.Client(schema)
         test_query = SH_OPERATIONS_QUERY_PAGINATION % (1, 0)
         executed = client.execute(test_query,
```

### Comparing `sortinghat-1.0.0rc2/tests/test_utils.py` & `sortinghat-1.0.0rc3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc2/PKG-INFO` & `sortinghat-1.0.0rc3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sortinghat
-Version: 1.0.0rc2
+Version: 1.0.0rc3
 Summary: A tool to manage identities.
 Home-page: https://chaoss.github.io/grimoirelab/
 License: GPL-3.0+
 Keywords: development,grimoirelab
 Author: GrimoireLab Developers
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -12,15 +12,15 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
-Requires-Dist: Django (>=3.2,<4.0)
+Requires-Dist: Django (>=4.2,<5.0)
 Requires-Dist: Jinja2 (>=3.1.1,<4.0.0)
 Requires-Dist: PyJWT (>=2.4.0,<3.0.0)
 Requires-Dist: click (==7.1.1)
 Requires-Dist: django-cors-headers (>=3.7.0,<4.0.0)
 Requires-Dist: django-graphql-jwt (>=0.3.0,<0.4.0)
 Requires-Dist: django-rq (>=2.3.2,<3.0.0)
 Requires-Dist: django-storages[google] (>=1.13.2,<2.0.0)
@@ -59,15 +59,15 @@
 
 
 ## Requirements
 
 * Python >= 3.8
 * Poetry >= 1.1.0
 * MySQL >= 5.7 or MariaDB 10.0
-* Django = 3.2
+* Django = 4.2
 * Graphene-Django >= 2.0
 * uWSGI >= 2.0
 
 You will also need some other libraries for running the tool, you can find the
 whole list of dependencies in [pyproject.toml](pyproject.toml) file.
 
 
@@ -111,15 +111,15 @@
 ```
 
 #### Installation and configuration
 
 **Note**: these examples use `sortinghat.config.settings` configuration file.
 In order to use that configuration you need to define the environment variable
 `SORTINGHAT_SECRET_KEY` with a secret. More info here:
-https://docs.djangoproject.com/en/3.2/ref/settings/#std:setting-SECRET_KEY
+https://docs.djangoproject.com/en/4.2/ref/settings/#std:setting-SECRET_KEY
 
 
 Install the required dependencies (this will also create a virtual environment).
 ```
 $ poetry install
 ```
 
@@ -326,16 +326,16 @@
 ## Running tests
 
 SortingHat comes with a comprehensive list of unit tests for both 
 frontend and backend.
 
 #### Backend test suite
 ```
-(.venv)$ ./manage.py test --settings=config.settings.testing
-(.venv)$ ./manage.py test --settings=config.settings.testing_tenant
+(.venv)$ ./manage.py test --settings=config.settings.config_testing
+(.venv)$ ./manage.py test --settings=config.settings.config_testing_tenant
 ```
 
 #### Frontend test suite
 ```
 $ cd ui/
 $ yarn test:unit
 ```
```

