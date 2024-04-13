# Comparing `tmp/django_tbase_post_product-2024.3.1317103017.tar.gz` & `tmp/django_tbase_post_product-2024.4.1317130137.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_tbase_post_product-2024.3.1317103017.tar", last modified: Wed Mar 13 03:48:55 2024, max compression
+gzip compressed data, was "django_tbase_post_product-2024.4.1317130137.tar", last modified: Sat Apr 13 13:09:13 2024, max compression
```

## Comparing `django_tbase_post_product-2024.3.1317103017.tar` & `django_tbase_post_product-2024.4.1317130137.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-03-13 03:48:55.491528 django_tbase_post_product-2024.3.1317103017/
--rw-rw-r--   0 terry     (1000) terry     (1000)      143 2023-12-03 08:49:22.000000 django_tbase_post_product-2024.3.1317103017/MANIFEST.in
--rw-rw-r--   0 terry     (1000) terry     (1000)     1806 2024-03-13 03:48:55.491528 django_tbase_post_product-2024.3.1317103017/PKG-INFO
--rw-rw-r--   0 terry     (1000) terry     (1000)     1483 2024-03-12 14:23:55.000000 django_tbase_post_product-2024.3.1317103017/README.md
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-03-13 03:48:55.487528 django_tbase_post_product-2024.3.1317103017/django_tbase_post_product.egg-info/
--rw-rw-r--   0 terry     (1000) terry     (1000)     1806 2024-03-13 03:48:55.000000 django_tbase_post_product-2024.3.1317103017/django_tbase_post_product.egg-info/PKG-INFO
--rw-rw-r--   0 terry     (1000) terry     (1000)     1983 2024-03-13 03:48:55.000000 django_tbase_post_product-2024.3.1317103017/django_tbase_post_product.egg-info/SOURCES.txt
--rw-rw-r--   0 terry     (1000) terry     (1000)        1 2024-03-13 03:48:55.000000 django_tbase_post_product-2024.3.1317103017/django_tbase_post_product.egg-info/dependency_links.txt
--rw-rw-r--   0 terry     (1000) terry     (1000)       83 2024-03-13 03:48:55.000000 django_tbase_post_product-2024.3.1317103017/django_tbase_post_product.egg-info/requires.txt
--rw-rw-r--   0 terry     (1000) terry     (1000)       11 2024-03-13 03:48:55.000000 django_tbase_post_product-2024.3.1317103017/django_tbase_post_product.egg-info/top_level.txt
--rw-rw-r--   0 terry     (1000) terry     (1000)       38 2024-03-13 03:48:55.491528 django_tbase_post_product-2024.3.1317103017/setup.cfg
--rw-rw-r--   0 terry     (1000) terry     (1000)     2305 2023-12-03 08:49:22.000000 django_tbase_post_product-2024.3.1317103017/setup.py
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-03-13 03:48:55.487528 django_tbase_post_product-2024.3.1317103017/tbase_post/
--rw-rw-r--   0 terry     (1000) terry     (1000)     7569 2024-03-12 15:28:36.000000 django_tbase_post_product-2024.3.1317103017/tbase_post/0001_initial.py
--rw-rw-r--   0 terry     (1000) terry     (1000)        0 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.3.1317103017/tbase_post/__init__.py
--rw-rw-r--   0 terry     (1000) terry     (1000)     6331 2024-03-13 03:45:25.000000 django_tbase_post_product-2024.3.1317103017/tbase_post/admin.py
--rw-rw-r--   0 terry     (1000) terry     (1000)      146 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.3.1317103017/tbase_post/apps.py
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-03-13 03:48:55.487528 django_tbase_post_product-2024.3.1317103017/tbase_post/migrations/
--rw-rw-r--   0 terry     (1000) terry     (1000)        0 2023-12-03 07:39:38.000000 django_tbase_post_product-2024.3.1317103017/tbase_post/migrations/__init__.py
--rw-rw-r--   0 terry     (1000) terry     (1000)    10301 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.3.1317103017/tbase_post/models.py
--rw-rw-r--   0 terry     (1000) terry     (1000)      616 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.3.1317103017/tbase_post/sitemaps.py
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-03-13 03:48:55.487528 django_tbase_post_product-2024.3.1317103017/tbase_post/static/
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-03-13 03:48:55.487528 django_tbase_post_product-2024.3.1317103017/tbase_post/static/images/
--rw-rw-r--   0 terry     (1000) terry     (1000)    59619 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.3.1317103017/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg
--rw-rw-r--   0 terry     (1000) terry     (1000)       94 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.3.1317103017/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg:Zone.Identifier
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-03-13 03:48:55.491528 django_tbase_post_product-2024.3.1317103017/tbase_post/templates/
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-03-13 03:48:55.491528 django_tbase_post_product-2024.3.1317103017/tbase_post/templates/post/
--rw-rw-r--   0 terry     (1000) terry     (1000)     5494 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.3.1317103017/tbase_post/templates/post/article_list_by_tag.html
--rw-rw-r--   0 terry     (1000) terry     (1000)     3448 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.3.1317103017/tbase_post/templates/post/blog_index.html
--rw-rw-r--   0 terry     (1000) terry     (1000)    16264 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.3.1317103017/tbase_post/templates/post/detail.html
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-03-13 03:48:55.491528 django_tbase_post_product-2024.3.1317103017/tbase_post/templates/post/extras/
--rw-rw-r--   0 terry     (1000) terry     (1000)      732 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.3.1317103017/tbase_post/templates/post/extras/amazon_ads.html
--rw-rw-r--   0 terry     (1000) terry     (1000)      591 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.3.1317103017/tbase_post/templates/post/extras/amazon_link.html
--rw-rw-r--   0 terry     (1000) terry     (1000)      884 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.3.1317103017/tbase_post/templates/post/extras/hitcount_lowest_post.html
--rw-rw-r--   0 terry     (1000) terry     (1000)      818 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.3.1317103017/tbase_post/templates/post/extras/hitcount_top_post.html
--rw-rw-r--   0 terry     (1000) terry     (1000)     1946 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.3.1317103017/tbase_post/templates/post/extras/last_update.html
--rw-rw-r--   0 terry     (1000) terry     (1000)     1796 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.3.1317103017/tbase_post/templates/post/extras/related_post_by_tags.html
--rw-rw-r--   0 terry     (1000) terry     (1000)      827 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.3.1317103017/tbase_post/templates/post/extras/seo_top_links.html
--rw-rw-r--   0 terry     (1000) terry     (1000)      569 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.3.1317103017/tbase_post/templates/post/extras/tags.html
--rw-rw-r--   0 terry     (1000) terry     (1000)      132 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.3.1317103017/tbase_post/templates/post/extras/templ.html
--rw-rw-r--   0 terry     (1000) terry     (1000)      576 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.3.1317103017/tbase_post/templates/post/extras/youtube_player.html
--rw-rw-r--   0 terry     (1000) terry     (1000)     2109 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.3.1317103017/tbase_post/templates/post/last_index.html
--rw-rw-r--   0 terry     (1000) terry     (1000)      255 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.3.1317103017/tbase_post/templates/post/prompt_task_detail copy.html
--rw-rw-r--   0 terry     (1000) terry     (1000)     4751 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.3.1317103017/tbase_post/templates/post/prompt_task_detail.html
--rw-rw-r--   0 terry     (1000) terry     (1000)      426 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.3.1317103017/tbase_post/templates/post/prompt_task_list.html
--rw-rw-r--   0 terry     (1000) terry     (1000)     2483 2024-03-13 03:47:25.000000 django_tbase_post_product-2024.3.1317103017/tbase_post/templates/post/prompt_task_post_detail.html
--rw-rw-r--   0 terry     (1000) terry     (1000)     4733 2024-03-13 03:36:27.000000 django_tbase_post_product-2024.3.1317103017/tbase_post/templates/post/prompt_task_post_list.html
--rw-rw-r--   0 terry     (1000) terry     (1000)      765 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.3.1317103017/tbase_post/templates/post_list.html
--rw-rw-r--   0 terry     (1000) terry     (1000)      391 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.3.1317103017/tbase_post/templates/sitemap.xml
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-03-13 03:48:55.491528 django_tbase_post_product-2024.3.1317103017/tbase_post/templatetags/
--rw-rw-r--   0 terry     (1000) terry     (1000)        0 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.3.1317103017/tbase_post/templatetags/__init__.py
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-03-13 03:48:55.491528 django_tbase_post_product-2024.3.1317103017/tbase_post/templatetags/__pycache__/
--rw-rw-r--   0 terry     (1000) terry     (1000)      196 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.3.1317103017/tbase_post/templatetags/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 terry     (1000) terry     (1000)      190 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.3.1317103017/tbase_post/templatetags/__pycache__/__init__.cpython-39.pyc
--rw-rw-r--   0 terry     (1000) terry     (1000)     6290 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.3.1317103017/tbase_post/templatetags/__pycache__/post_extras.cpython-310.pyc
--rw-rw-r--   0 terry     (1000) terry     (1000)     4111 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.3.1317103017/tbase_post/templatetags/__pycache__/post_extras.cpython-39.pyc
--rw-rw-r--   0 terry     (1000) terry     (1000)    11661 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.3.1317103017/tbase_post/templatetags/post_extras.py
--rw-rw-r--   0 terry     (1000) terry     (1000)       60 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.3.1317103017/tbase_post/tests.py
--rw-rw-r--   0 terry     (1000) terry     (1000)     1571 2024-03-13 03:17:25.000000 django_tbase_post_product-2024.3.1317103017/tbase_post/urls.py
--rw-rw-r--   0 terry     (1000) terry     (1000)    11928 2024-03-13 03:43:23.000000 django_tbase_post_product-2024.3.1317103017/tbase_post/views.py
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-04-13 13:09:13.168593 django_tbase_post_product-2024.4.1317130137/
+-rw-rw-r--   0 terry     (1000) terry     (1000)      143 2023-12-03 08:49:22.000000 django_tbase_post_product-2024.4.1317130137/MANIFEST.in
+-rw-rw-r--   0 terry     (1000) terry     (1000)     1900 2024-04-13 13:09:13.168593 django_tbase_post_product-2024.4.1317130137/PKG-INFO
+-rw-rw-r--   0 terry     (1000) terry     (1000)     1577 2024-04-13 13:07:21.000000 django_tbase_post_product-2024.4.1317130137/README.md
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-04-13 13:09:13.160593 django_tbase_post_product-2024.4.1317130137/django_tbase_post_product.egg-info/
+-rw-rw-r--   0 terry     (1000) terry     (1000)     1900 2024-04-13 13:09:13.000000 django_tbase_post_product-2024.4.1317130137/django_tbase_post_product.egg-info/PKG-INFO
+-rw-rw-r--   0 terry     (1000) terry     (1000)     1983 2024-04-13 13:09:13.000000 django_tbase_post_product-2024.4.1317130137/django_tbase_post_product.egg-info/SOURCES.txt
+-rw-rw-r--   0 terry     (1000) terry     (1000)        1 2024-04-13 13:09:13.000000 django_tbase_post_product-2024.4.1317130137/django_tbase_post_product.egg-info/dependency_links.txt
+-rw-rw-r--   0 terry     (1000) terry     (1000)       83 2024-04-13 13:09:13.000000 django_tbase_post_product-2024.4.1317130137/django_tbase_post_product.egg-info/requires.txt
+-rw-rw-r--   0 terry     (1000) terry     (1000)       11 2024-04-13 13:09:13.000000 django_tbase_post_product-2024.4.1317130137/django_tbase_post_product.egg-info/top_level.txt
+-rw-rw-r--   0 terry     (1000) terry     (1000)       38 2024-04-13 13:09:13.168593 django_tbase_post_product-2024.4.1317130137/setup.cfg
+-rw-rw-r--   0 terry     (1000) terry     (1000)     2305 2023-12-03 08:49:22.000000 django_tbase_post_product-2024.4.1317130137/setup.py
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-04-13 13:09:13.164593 django_tbase_post_product-2024.4.1317130137/tbase_post/
+-rw-rw-r--   0 terry     (1000) terry     (1000)     7569 2024-03-12 15:28:36.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/0001_initial.py
+-rw-rw-r--   0 terry     (1000) terry     (1000)        0 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/__init__.py
+-rw-rw-r--   0 terry     (1000) terry     (1000)     6331 2024-03-13 03:45:25.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/admin.py
+-rw-rw-r--   0 terry     (1000) terry     (1000)      146 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/apps.py
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-04-13 13:09:13.164593 django_tbase_post_product-2024.4.1317130137/tbase_post/migrations/
+-rw-rw-r--   0 terry     (1000) terry     (1000)        0 2023-12-03 07:39:38.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/migrations/__init__.py
+-rw-rw-r--   0 terry     (1000) terry     (1000)    10357 2024-04-13 13:06:33.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/models.py
+-rw-rw-r--   0 terry     (1000) terry     (1000)      616 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/sitemaps.py
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-04-13 13:09:13.160593 django_tbase_post_product-2024.4.1317130137/tbase_post/static/
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-04-13 13:09:13.164593 django_tbase_post_product-2024.4.1317130137/tbase_post/static/images/
+-rw-rw-r--   0 terry     (1000) terry     (1000)    59619 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg
+-rw-rw-r--   0 terry     (1000) terry     (1000)       94 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg:Zone.Identifier
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-04-13 13:09:13.164593 django_tbase_post_product-2024.4.1317130137/tbase_post/templates/
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-04-13 13:09:13.164593 django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/
+-rw-rw-r--   0 terry     (1000) terry     (1000)     5494 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/article_list_by_tag.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)     2994 2024-04-13 11:28:01.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/blog_index.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)    11325 2024-04-13 11:36:48.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/detail.html
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-04-13 13:09:13.164593 django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/extras/
+-rw-rw-r--   0 terry     (1000) terry     (1000)      732 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/extras/amazon_ads.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)      591 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/extras/amazon_link.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)      884 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/extras/hitcount_lowest_post.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)      818 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/extras/hitcount_top_post.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)     1946 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/extras/last_update.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)     1796 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/extras/related_post_by_tags.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)      827 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/extras/seo_top_links.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)      569 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/extras/tags.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)      132 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/extras/templ.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)      576 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/extras/youtube_player.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)     2109 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/last_index.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)      255 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/prompt_task_detail copy.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)     4751 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/prompt_task_detail.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)      426 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/prompt_task_list.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)     2483 2024-03-13 03:47:25.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/prompt_task_post_detail.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)     4733 2024-03-13 03:36:27.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/prompt_task_post_list.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)      765 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post_list.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)      391 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/templates/sitemap.xml
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-04-13 13:09:13.164593 django_tbase_post_product-2024.4.1317130137/tbase_post/templatetags/
+-rw-rw-r--   0 terry     (1000) terry     (1000)        0 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/templatetags/__init__.py
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-04-13 13:09:13.168593 django_tbase_post_product-2024.4.1317130137/tbase_post/templatetags/__pycache__/
+-rw-rw-r--   0 terry     (1000) terry     (1000)      196 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/templatetags/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 terry     (1000) terry     (1000)      190 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/templatetags/__pycache__/__init__.cpython-39.pyc
+-rw-rw-r--   0 terry     (1000) terry     (1000)     6290 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/templatetags/__pycache__/post_extras.cpython-310.pyc
+-rw-rw-r--   0 terry     (1000) terry     (1000)     4111 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/templatetags/__pycache__/post_extras.cpython-39.pyc
+-rw-rw-r--   0 terry     (1000) terry     (1000)    11661 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/templatetags/post_extras.py
+-rw-rw-r--   0 terry     (1000) terry     (1000)       60 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/tests.py
+-rw-rw-r--   0 terry     (1000) terry     (1000)     1571 2024-03-13 03:17:25.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/urls.py
+-rw-rw-r--   0 terry     (1000) terry     (1000)    11928 2024-03-13 03:43:23.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/views.py
```

### Comparing `django_tbase_post_product-2024.3.1317103017/PKG-INFO` & `django_tbase_post_product-2024.4.1317130137/django_tbase_post_product.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: django_tbase_post_product
-Version: 2024.3.1317103017
+Name: django-tbase-post-product
+Version: 2024.4.1317130137
 Summary: Terry django base post ,
 Home-page: https://terrychanorg.jetbrains.space/p/django-expand/repositories/tbase_post_product/files/README.md
 Author: Terry Chan
 Author-email: napoler2008@gmail.com
 Description-Content-Type: text/markdown
 
 # django-expand/tbase_post_product
@@ -33,14 +33,20 @@
 
  ]
 ```
 
 
 ## 更新
 
+- 2024/04/13
+优化展示
+
+- 2024/03/13
+添加post对应提示词列表，添加对应跳转
+
 - 2024/03/12
 添加提示词生成
 
 
 - 2024/02/26
 添加低频率链接推荐
 修改缓存时间
```

### Comparing `django_tbase_post_product-2024.3.1317103017/README.md` & `django_tbase_post_product-2024.4.1317130137/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -24,14 +24,20 @@
 
  ]
 ```
 
 
 ## 更新
 
+- 2024/04/13
+优化展示
+
+- 2024/03/13
+添加post对应提示词列表，添加对应跳转
+
 - 2024/03/12
 添加提示词生成
 
 
 - 2024/02/26
 添加低频率链接推荐
 修改缓存时间
```

### Comparing `django_tbase_post_product-2024.3.1317103017/django_tbase_post_product.egg-info/PKG-INFO` & `django_tbase_post_product-2024.4.1317130137/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: django-tbase-post-product
-Version: 2024.3.1317103017
+Name: django_tbase_post_product
+Version: 2024.4.1317130137
 Summary: Terry django base post ,
 Home-page: https://terrychanorg.jetbrains.space/p/django-expand/repositories/tbase_post_product/files/README.md
 Author: Terry Chan
 Author-email: napoler2008@gmail.com
 Description-Content-Type: text/markdown
 
 # django-expand/tbase_post_product
@@ -33,14 +33,20 @@
 
  ]
 ```
 
 
 ## 更新
 
+- 2024/04/13
+优化展示
+
+- 2024/03/13
+添加post对应提示词列表，添加对应跳转
+
 - 2024/03/12
 添加提示词生成
 
 
 - 2024/02/26
 添加低频率链接推荐
 修改缓存时间
```

### Comparing `django_tbase_post_product-2024.3.1317103017/django_tbase_post_product.egg-info/SOURCES.txt` & `django_tbase_post_product-2024.4.1317130137/django_tbase_post_product.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.3.1317103017/setup.py` & `django_tbase_post_product-2024.4.1317130137/setup.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.3.1317103017/tbase_post/0001_initial.py` & `django_tbase_post_product-2024.4.1317130137/tbase_post/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.3.1317103017/tbase_post/admin.py` & `django_tbase_post_product-2024.4.1317130137/tbase_post/admin.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.3.1317103017/tbase_post/models.py` & `django_tbase_post_product-2024.4.1317130137/tbase_post/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -77,25 +77,25 @@
     prompt_task = models.ForeignKey(PromptTask, on_delete=models.CASCADE)
     prompt = models.ForeignKey(Prompt, on_delete=models.CASCADE)
     order = models.PositiveIntegerField(default=0)
 
     def __str__(self):
         return f"{self.prompt_task} - {self.prompt}"
 
-
-
-
-
+ 
 
  
 class Link(models.Model):
     title =  models.CharField("标题",max_length=255,)
     url = models.URLField("URL",max_length=255, default='', null=True, blank=True)
     updated_on = models.DateTimeField("更新时间",auto_now=True)
-
+    
+    def __str__(self):
+        return self.title
+    
 class Post(models.Model):
     title = models.CharField("标题",max_length=255,)
     # slug = models.SlugField(
     #     unique=True,
     #     max_length=255,
     # )
     # content = models.TextField()
```

### Comparing `django_tbase_post_product-2024.3.1317103017/tbase_post/sitemaps.py` & `django_tbase_post_product-2024.4.1317130137/tbase_post/sitemaps.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.3.1317103017/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg` & `django_tbase_post_product-2024.4.1317130137/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.3.1317103017/tbase_post/templates/post/article_list_by_tag.html` & `django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/article_list_by_tag.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.3.1317103017/tbase_post/templates/post/blog_index.html` & `django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/blog_index.html`

 * *Files 8% similar despite different names*

```diff
@@ -26,26 +26,15 @@
                 <ul class="flex items-center justify-between font-bold text-sm text-white uppercase no-underline">
                     <li><a class="hover:text-gray-200 hover:underline px-4" href="{% url 'home'%}">Home</a></li>
                     <li><a class="hover:text-gray-200 hover:underline px-4"  rel="nofollow" href="{% url  'last_index' %}">Update</a></li>
                 </ul>
             </nav>
 
             <div class="flex items-center text-lg no-underline text-white pr-6">
-                <!-- <a class="" href="#">
-                    <i class="fab fa-facebook"></i>
-                </a>
-                <a class="pl-6" href="#">
-                    <i class="fab fa-instagram"></i>
-                </a>
-                <a class="pl-6" href="#">
-                    <i class="fab fa-twitter"></i>
-                </a>
-                <a class="pl-6" href="#">
-                    <i class="fab fa-linkedin"></i>
-                </a> -->
+          
             </div>
         </div>
 
     </nav>
     {% comment %} top_toolbar end {% endcomment %}
 {% endblock %}
```

### Comparing `django_tbase_post_product-2024.3.1317103017/tbase_post/templates/post/detail.html` & `django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/detail.html`

 * *Files 24% similar despite different names*

```diff
@@ -153,87 +153,60 @@
 <!--亚马逊推广链接结束-->
 
 </script>
 
 
 
 <script id="banner-img-tpl" type="text/html">
-
     <div class="w-full  bg-white border border-gray-200 rounded-lg shadow dark:bg-gray-800 dark:border-gray-700">
         <a  rel="nofollow" href="{% amazon_base_link object.product_id detail.product_name amazon.store_id %}">
-            <img class="p-8 rounded-t-lg mx-auto  h-90 " src="{{detail.article_img}}" alt="product {{detail.product_name}}" />
+            <img class="p-8 rounded-t-lg mx-auto  h-40 " src="{{detail.article_img}}" alt="product {{detail.product_name}}" />
         </a>
         <div class="px-5 pb-5">
-            <a href="#">
                 <h5 class="text-xl font-semibold tracking-tight text-gray-900 dark:text-white  text-center">{{detail.product_name}}</h5>
-            </a>
             <div class="flex items-center mt-2.5 mb-5">
-                <!-- <svg class="w-4 h-4 text-yellow-300 mr-1" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="currentColor" viewBox="0 0 22 20">
-                    <path d="M20.924 7.625a1.523 1.523 0 0 0-1.238-1.044l-5.051-.734-2.259-4.577a1.534 1.534 0 0 0-2.752 0L7.365 5.847l-5.051.734A1.535 1.535 0 0 0 1.463 9.2l3.656 3.563-.863 5.031a1.532 1.532 0 0 0 2.226 1.616L11 17.033l4.518 2.375a1.534 1.534 0 0 0 2.226-1.617l-.863-5.03L20.537 9.2a1.523 1.523 0 0 0 .387-1.575Z"/>
-                </svg>
-                <svg class="w-4 h-4 text-yellow-300 mr-1" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="currentColor" viewBox="0 0 22 20">
-                    <path d="M20.924 7.625a1.523 1.523 0 0 0-1.238-1.044l-5.051-.734-2.259-4.577a1.534 1.534 0 0 0-2.752 0L7.365 5.847l-5.051.734A1.535 1.535 0 0 0 1.463 9.2l3.656 3.563-.863 5.031a1.532 1.532 0 0 0 2.226 1.616L11 17.033l4.518 2.375a1.534 1.534 0 0 0 2.226-1.617l-.863-5.03L20.537 9.2a1.523 1.523 0 0 0 .387-1.575Z"/>
-                </svg>
-                <svg class="w-4 h-4 text-yellow-300 mr-1" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="currentColor" viewBox="0 0 22 20">
-                    <path d="M20.924 7.625a1.523 1.523 0 0 0-1.238-1.044l-5.051-.734-2.259-4.577a1.534 1.534 0 0 0-2.752 0L7.365 5.847l-5.051.734A1.535 1.535 0 0 0 1.463 9.2l3.656 3.563-.863 5.031a1.532 1.532 0 0 0 2.226 1.616L11 17.033l4.518 2.375a1.534 1.534 0 0 0 2.226-1.617l-.863-5.03L20.537 9.2a1.523 1.523 0 0 0 .387-1.575Z"/>
-                </svg>
-                <svg class="w-4 h-4 text-yellow-300 mr-1" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="currentColor" viewBox="0 0 22 20">
-                    <path d="M20.924 7.625a1.523 1.523 0 0 0-1.238-1.044l-5.051-.734-2.259-4.577a1.534 1.534 0 0 0-2.752 0L7.365 5.847l-5.051.734A1.535 1.535 0 0 0 1.463 9.2l3.656 3.563-.863 5.031a1.532 1.532 0 0 0 2.226 1.616L11 17.033l4.518 2.375a1.534 1.534 0 0 0 2.226-1.617l-.863-5.03L20.537 9.2a1.523 1.523 0 0 0 .387-1.575Z"/>
-                </svg>
-                <svg class="w-4 h-4 text-gray-200 dark:text-gray-600" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="currentColor" viewBox="0 0 22 20">
-                    <path d="M20.924 7.625a1.523 1.523 0 0 0-1.238-1.044l-5.051-.734-2.259-4.577a1.534 1.534 0 0 0-2.752 0L7.365 5.847l-5.051.734A1.535 1.535 0 0 0 1.463 9.2l3.656 3.563-.863 5.031a1.532 1.532 0 0 0 2.226 1.616L11 17.033l4.518 2.375a1.534 1.534 0 0 0 2.226-1.617l-.863-5.03L20.537 9.2a1.523 1.523 0 0 0 .387-1.575Z"/>
-                </svg>
-                <span class="bg-blue-100 text-blue-800 text-xs font-semibold mr-2 px-2.5 py-0.5 rounded dark:bg-blue-200 dark:text-blue-800 ml-3">5.0</span>
-        -->   
-    
+             
     </div> 
             <div class="flex items-center justify-between">
                 <span class="text-3xl font-bold text-gray-900 dark:text-white"></span>
                 <a  rel="nofollow" href="{% amazon_base_link object.product_id detail.product_name amazon.store_id %}"
                  class="text-white bg-blue-700 hover:bg-blue-800 focus:ring-4 focus:outline-none focus:ring-blue-300 font-medium rounded-lg text-sm px-5 py-2.5 text-center dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800"> Buy on Amazon</a>
             </div>
         </div>
     
     
     </div>
-     
-    </script>
+</script>
 
 
 <script id="banner-amazon-footer-tpl" type="text/html">
 
     <div class="fixed bottom-0 left-0 w-full bg-gray-800 text-white py-4 px-6">
         <!-- 这里放置固定顶端内容 -->
          <div class="container mx-auto flex flex-wrap py-1 px-3 ">
               
              <div class="w-full md:w-2/3 flex flex-row px-2">
                  <div class="w-auto px-3">
-                     
                      <img alt="{{detail.product_name}}" class="max-h-10" src="{{detail.article_img}}">
                  </div>
-                 <div class="">
+                 <div class="amz-banner">
 <!--亚马逊推广链接-->
 {% get_solo 'tbase_post.AmazonSettings' as amazon %}
 {% amazon_link object.product_id detail.product_name amazon.store_id %}
 <!--亚马逊推广链接结束-->
 
                  </div>
-                
-         
              </div>
              <div class="w-full md:w-1/3 flex flex-col items-center px-3">
 
 
              </div>
 
          </div>
-
-
-
-
+ 
    </div>
    
 </script>
 
 
 
 
@@ -310,123 +283,86 @@
 
 {% block text_header %}
 {% endblock %}
 
 {% block article_img %}
 {%if detail.article_img%}
  
-
 {% get_solo 'tbase_post.AmazonSettings' as amazon %}
 
-
 <div id="banner-img"></div>
 
-
 {%endif%}
 {% endblock %}
+<!-- block article_img end -->
 
-{% block article %}
-
-
- <!-- <p class="text-blue-700 text-sm font-bold uppercase pb-4">{{detail.product_name}}</p>  -->
 
+{% block article %}
+ 
 <h1 class="text-3xl font-bold pb-3">{{detail.title}}</h1>
-                    {% comment %} <a href="#" class="text-3xl font-bold hover:text-gray-700 pb-4">Lorem Ipsum Dolor Sit Amet Dolor Sit Amet</a> {% endcomment %}
-                    <p href="#" class="text-sm pb-8">
-                        {% comment %} By <a href="#" class="font-semibold hover:text-gray-800">David Grzyb</a>,  {% endcomment %}
-                        Published on {{detail.created_on}}
-                    </p>
-
+<p class="text-sm pb-8">Published on {{detail.created_on}}</p>
 
 <!-- youtube播放 -->
-                    {% youtube_player object.youtube_id %}
+{% youtube_player object.youtube_id %}
 <!-- youtube播放 结束-->
 
 
-    <div class="pb-3">
- 
-               <!--亚马逊推广链接-->   
-                <!-- {% get_solo 'tbase_post.AmazonSettings' as amazon %}
-               <a rel="nofollow" href="{% amazon_base_link object.product_id detail.product_name amazon.store_id %}" class="m-2 p-2  flex flex-col items-center bg-white border border-gray-200 rounded-lg shadow md:flex-row md:max-w-xl hover:bg-gray-100 dark:border-gray-700 dark:bg-gray-800 dark:hover:bg-gray-700">
-                <img class="object-cover w-full rounded-t-lg h-96 md:h-auto md:w-48 md:rounded-none md:rounded-l-lg" src="{{detail.article_img}}" alt="">
-                <div class="flex flex-col justify-between p-4 leading-normal">
-                    <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">{{detail.product_name}}</h5>
-    
-                    <div class="mb-3 font-normal text-gray-700 dark:text-gray-400">
-                         <div>
-                            <button class="inline-block bg-red-500 hover:bg-red-700 text-white font-bold py-2 px-4 rounded">
-                                Buy on Amazon
-                                </button>
-                         </div>
-                    
-                    </div>
-    
-    
-                        
-                </div>
-            </a> -->
-            
-        <!--亚马逊推广链接结束-->
-        <!--主体正文-->
-        {{ detail.content|safe_markdown }}
-        <!--主体正文结束-->
- 
-<div id="banner-amazon"></div>
-
-
+<div class="pb-3">
 
+<!--主体正文-->
+{{ detail.content|safe_markdown }}
+<!--主体正文结束-->
 
+<div id="banner-amazon"></div>
 
 <!-- 广告代码 ads_content1 -->
-    {% autoescape off %}
-    {% get_solo 'tbase_post.AmazonSettings' as amz %}
-    {% if amz.ads_content1 %}
-    {{amz.ads_content1}}
+{% autoescape off %}
+{% get_solo 'tbase_post.AmazonSettings' as amz %}
+{% if amz.ads_content1 %}
+{{amz.ads_content1}}
 
-    {% endif %}
-    {% endautoescape %}
+{% endif %}
+{% endautoescape %}
 <!-- 广告代码结束 -->
 <div id="banner-amazon-footer"></div>
 
 
 
 
 
 <script type="text/javascript">
-    data={}
-    var htmlStr = template('banner-amazon-tpl', data)
-    $('#banner-amazon').html(htmlStr)
-    
-    data={}
-    var htmlStr = template('banner-img-tpl', data)
-        $('#banner-img').html(htmlStr)
-        data={}
-    var htmlStr = template('banner-amazon-footer-tpl', data)
-        $('#banner-amazon-footer').html(htmlStr)
-    
-    </script>
+data={}
+var htmlStr = template('banner-amazon-tpl', data)
+$('#banner-amazon').html(htmlStr)
+
+data={}
+var htmlStr = template('banner-img-tpl', data)
+$('#banner-img').html(htmlStr)
+data={}
+var htmlStr = template('banner-amazon-footer-tpl', data)
+$('#banner-amazon-footer').html(htmlStr)
+
+</script>
 
  
 <!--标签-->
 {% tags object.tags 5 object.pk %}
- 
+ <!--标签end-->
+
 <div class="pt-6  columns-1 md:columns-2">
 <div class=" bg-white text-left ">
     {% hitcount_top_post 20 detail.pk %}
 </div>
 <div class="  bg-white text-left">
     {% hitcount_lowest_post 20 detail.pk %}
-
     </div>
 </div>
 
 
-
-
-    </div>
+</div>
 
 <!--相关内容-->
 <div class="pt-6  columns-1 md:columns-2">
 <div class=" bg-white text-left ">
 
  
 {% related_post_by_tags object.tags 10 object.pk %}
@@ -445,28 +381,28 @@
 {% endblock %}
 
 
 <!--上一页下一页链接区域-->
 
 {% block article_previous_next %}
 
-                {% if detail.get_previous_by_created_on  %}
-                <a href="{% url 'detail_view' detail.get_previous_by_created_on.pk %}" class="w-1/2 bg-white shadow hover:shadow-md text-left p-6">
-                    <p class="text-lg text-blue-800 font-bold flex items-center"><i class="fas fa-arrow-left pr-1"></i> {{detail.get_previous_by_created_on.title}}</p>
-                    <p class="pt-2"></p>
-                </a>
+{% if detail.get_previous_by_created_on  %}
+<a href="{% url 'detail_view' detail.get_previous_by_created_on.pk %}" class="w-1/2 bg-white shadow hover:shadow-md text-left p-6">
+<p class="text-lg text-blue-800 font-bold flex items-center"><i class="fas fa-arrow-left pr-1"></i> {{detail.get_previous_by_created_on.title}}</p>
+<p class="pt-2"></p>
+</a>
 
-    {%endif%}
-                {% if detail.get_next_by_created_on  %}
-                <a href="{% url 'detail_view' detail.get_next_by_created_on.pk %}" class="w-1/2 bg-white shadow hover:shadow-md text-right p-6">
-                    <p class="text-lg text-blue-800 font-bold flex items-center justify-end">{{detail.get_next_by_created_on.title}} <i class="fas fa-arrow-right pl-1"></i></p>
-                    <p class="pt-2"></p>
-                </a>
+{%endif%}
+{% if detail.get_next_by_created_on  %}
+<a href="{% url 'detail_view' detail.get_next_by_created_on.pk %}" class="w-1/2 bg-white shadow hover:shadow-md text-right p-6">
+<p class="text-lg text-blue-800 font-bold flex items-center justify-end">{{detail.get_next_by_created_on.title}} <i class="fas fa-arrow-right pl-1"></i></p>
+<p class="pt-2"></p>
+</a>
 
-            {%endif%}
+{%endif%}
 {% endblock %}
 <!--上一页下一页链接区域 结束-->
 
 
 
 <!--作者信息-->
 {% block article_author %}
@@ -476,17 +412,17 @@
 
 
   
 
 {% block sidebar_section %}
 <!-- sidebar_section -->
  
-    <div class="w-full bg-white shadow flex flex-col my-4 p-6">
-            {% seo_top_links 50 %}
-    </div>
+<div class="w-full bg-white shadow flex flex-col my-4 p-6">
+        {% seo_top_links 50 %}
+</div>
 
 <!-- 广告代码  ads_sidebar-->
 {% autoescape off %}
  
     <!--亚马逊推广链接-->
     {% get_solo 'tbase_post.AmazonSettings' as amazon %}
     {% amazon_ads object.product_id detail.product_name amazon.store_id %}
```

### Comparing `django_tbase_post_product-2024.3.1317103017/tbase_post/templates/post/extras/amazon_ads.html` & `django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/extras/amazon_ads.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.3.1317103017/tbase_post/templates/post/extras/amazon_link.html` & `django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/extras/amazon_link.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.3.1317103017/tbase_post/templates/post/extras/hitcount_lowest_post.html` & `django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/extras/hitcount_lowest_post.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.3.1317103017/tbase_post/templates/post/extras/hitcount_top_post.html` & `django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/extras/hitcount_top_post.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.3.1317103017/tbase_post/templates/post/extras/last_update.html` & `django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/extras/last_update.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.3.1317103017/tbase_post/templates/post/extras/related_post_by_tags.html` & `django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/extras/related_post_by_tags.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.3.1317103017/tbase_post/templates/post/extras/seo_top_links.html` & `django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/extras/seo_top_links.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.3.1317103017/tbase_post/templates/post/extras/tags.html` & `django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/extras/tags.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.3.1317103017/tbase_post/templates/post/extras/youtube_player.html` & `django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/extras/youtube_player.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.3.1317103017/tbase_post/templates/post/last_index.html` & `django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/last_index.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.3.1317103017/tbase_post/templates/post/prompt_task_detail.html` & `django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/prompt_task_detail.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.3.1317103017/tbase_post/templates/post/prompt_task_post_detail.html` & `django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/prompt_task_post_detail.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.3.1317103017/tbase_post/templates/post/prompt_task_post_list.html` & `django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/prompt_task_post_list.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.3.1317103017/tbase_post/templates/post_list.html` & `django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post_list.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.3.1317103017/tbase_post/templatetags/__pycache__/post_extras.cpython-310.pyc` & `django_tbase_post_product-2024.4.1317130137/tbase_post/templatetags/__pycache__/post_extras.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.3.1317103017/tbase_post/templatetags/__pycache__/post_extras.cpython-39.pyc` & `django_tbase_post_product-2024.4.1317130137/tbase_post/templatetags/__pycache__/post_extras.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.3.1317103017/tbase_post/templatetags/post_extras.py` & `django_tbase_post_product-2024.4.1317130137/tbase_post/templatetags/post_extras.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.3.1317103017/tbase_post/urls.py` & `django_tbase_post_product-2024.4.1317130137/tbase_post/urls.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.3.1317103017/tbase_post/views.py` & `django_tbase_post_product-2024.4.1317130137/tbase_post/views.py`

 * *Files identical despite different names*

