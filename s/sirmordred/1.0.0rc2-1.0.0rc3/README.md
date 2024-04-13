# Comparing `tmp/sirmordred-1.0.0rc2.tar.gz` & `tmp/sirmordred-1.0.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sirmordred-1.0.0rc2.tar", max compression
+gzip compressed data, was "sirmordred-1.0.0rc3.tar", max compression
```

## Comparing `sirmordred-1.0.0rc2.tar` & `sirmordred-1.0.0rc3.tar`

### file list

```diff
@@ -1,98 +1,98 @@
--rw-r--r--   0        0        0    35147 2024-04-11 11:14:40.122902 sirmordred-1.0.0rc2/LICENSE
--rw-r--r--   0        0        0    40852 2024-04-11 11:14:40.122902 sirmordred-1.0.0rc2/README.md
--rw-r--r--   0        0        0     8246 2024-04-11 11:14:40.126902 sirmordred-1.0.0rc2/menu.yaml
--rw-r--r--   0        0        0     2182 2024-04-11 11:14:40.126902 sirmordred-1.0.0rc2/pyproject.toml
--rw-r--r--   0        0        0      835 2024-04-11 11:14:40.130902 sirmordred-1.0.0rc2/sirmordred/__init__.py
--rw-r--r--   0        0        0       91 2024-04-11 11:14:40.130902 sirmordred-1.0.0rc2/sirmordred/_version.py
--rwxr-xr-x   0        0        0     5022 2024-04-11 11:14:40.130902 sirmordred-1.0.0rc2/sirmordred/bin/sirmordred.py
--rw-r--r--   0        0        0    33508 2024-04-11 11:14:40.130902 sirmordred-1.0.0rc2/sirmordred/config.py
--rw-r--r--   0        0        0     1836 2024-04-11 11:14:40.130902 sirmordred-1.0.0rc2/sirmordred/error.py
--rw-r--r--   0        0        0     2306 2024-04-11 11:14:40.130902 sirmordred-1.0.0rc2/sirmordred/github.py
--rwxr-xr-x   0        0        0    12432 2024-04-11 11:14:40.130902 sirmordred-1.0.0rc2/sirmordred/sirmordred.py
--rw-r--r--   0        0        0    10093 2024-04-11 11:14:40.130902 sirmordred-1.0.0rc2/sirmordred/task.py
--rw-r--r--   0        0        0     7762 2024-04-11 11:14:40.130902 sirmordred-1.0.0rc2/sirmordred/task_autorefresh.py
--rw-r--r--   0        0        0     6487 2024-04-11 11:14:40.130902 sirmordred-1.0.0rc2/sirmordred/task_collection.py
--rw-r--r--   0        0        0    21143 2024-04-11 11:14:40.130902 sirmordred-1.0.0rc2/sirmordred/task_enrich.py
--rw-r--r--   0        0        0     3396 2024-04-11 11:14:40.130902 sirmordred-1.0.0rc2/sirmordred/task_identities.py
--rw-r--r--   0        0        0     4424 2024-04-11 11:14:40.130902 sirmordred-1.0.0rc2/sirmordred/task_manager.py
--rw-r--r--   0        0        0    29060 2024-04-11 11:14:40.130902 sirmordred-1.0.0rc2/sirmordred/task_panels.py
--rw-r--r--   0        0        0     6484 2024-04-11 11:14:40.130902 sirmordred-1.0.0rc2/sirmordred/task_projects.py
--rw-r--r--   0        0        0     1981 2024-04-11 11:14:40.130902 sirmordred-1.0.0rc2/sirmordred/utils/find_affiliation_conflicts.py
--rw-r--r--   0        0        0      766 2024-04-11 11:14:40.130902 sirmordred-1.0.0rc2/sirmordred/utils/grimoirelab_valid.yml
--rwxr-xr-x   0        0        0     4709 2024-04-11 11:14:40.130902 sirmordred-1.0.0rc2/sirmordred/utils/healthcheck.py
--rw-r--r--   0        0        0        0 2024-04-11 11:14:40.130902 sirmordred-1.0.0rc2/sirmordred/utils/logs/all.log
--rw-r--r--   0        0        0     7849 2024-04-11 11:14:40.130902 sirmordred-1.0.0rc2/sirmordred/utils/micro.py
--rw-r--r--   0        0        0     2858 2024-04-11 11:14:40.130902 sirmordred-1.0.0rc2/sirmordred/utils/panels_config.py
--rw-r--r--   0        0        0      864 2024-04-11 11:14:40.130902 sirmordred-1.0.0rc2/sirmordred/utils/projects.json
--rw-r--r--   0        0        0     3141 2024-04-11 11:14:40.130902 sirmordred-1.0.0rc2/sirmordred/utils/projects_json2yml.py
--rw-r--r--   0        0        0     3634 2024-04-11 11:14:40.130902 sirmordred-1.0.0rc2/sirmordred/utils/setup.cfg
--rw-r--r--   0        0        0     4398 2024-04-11 11:14:40.130902 sirmordred-1.0.0rc2/tests/aliases.json
--rw-r--r--   0        0        0   497664 2024-04-11 11:14:40.130902 sirmordred-1.0.0rc2/tests/archives/askbot.archive
--rw-r--r--   0        0        0   150528 2024-04-11 11:14:40.130902 sirmordred-1.0.0rc2/tests/archives/bugzilla.archive
--rw-r--r--   0        0        0    52224 2024-04-11 11:14:40.130902 sirmordred-1.0.0rc2/tests/archives/bugzillarest.archive
--rw-r--r--   0        0        0    73728 2024-04-11 11:14:40.134902 sirmordred-1.0.0rc2/tests/archives/confluence.archive
--rw-r--r--   0        0        0  7141376 2024-04-11 11:14:40.150902 sirmordred-1.0.0rc2/tests/archives/crates.archive
--rw-r--r--   0        0        0   291840 2024-04-11 11:14:40.154902 sirmordred-1.0.0rc2/tests/archives/discourse.archive
--rw-r--r--   0        0        0    16384 2024-04-11 11:14:40.154902 sirmordred-1.0.0rc2/tests/archives/dockerhub.archive
--rw-r--r--   0        0        0  1713152 2024-04-11 11:14:40.158902 sirmordred-1.0.0rc2/tests/archives/functest.archive
--rw-r--r--   0        0        0    49152 2024-04-11 11:14:40.158902 sirmordred-1.0.0rc2/tests/archives/gerrit.archive
--rw-r--r--   0        0        0  9424896 2024-04-11 11:14:40.210902 sirmordred-1.0.0rc2/tests/archives/github-issue.archive
--rw-r--r--   0        0        0 23023616 2024-04-11 11:14:40.238902 sirmordred-1.0.0rc2/tests/archives/github-pull.archive
--rw-r--r--   0        0        0   208896 2024-04-11 11:14:40.238902 sirmordred-1.0.0rc2/tests/archives/gitlab-issue.archive
--rw-r--r--   0        0        0   937984 2024-04-11 11:14:40.242902 sirmordred-1.0.0rc2/tests/archives/gitlab-merge.archive
--rw-r--r--   0        0        0    65536 2024-04-11 11:14:40.242902 sirmordred-1.0.0rc2/tests/archives/googlehits.archive
--rw-r--r--   0        0        0   228352 2024-04-11 11:14:40.242902 sirmordred-1.0.0rc2/tests/archives/jenkins.archive
--rw-r--r--   0        0        0    86016 2024-04-11 11:14:40.242902 sirmordred-1.0.0rc2/tests/archives/jira.archive
--rw-r--r--   0        0        0    69632 2024-04-11 11:14:40.242902 sirmordred-1.0.0rc2/tests/archives/launchpad.archive
--rw-r--r--   0        0        0    31744 2024-04-11 11:14:40.242902 sirmordred-1.0.0rc2/tests/archives/mediawiki-1.23.archive
--rw-r--r--   0        0        0   245760 2024-04-11 11:14:40.242902 sirmordred-1.0.0rc2/tests/archives/mediawiki-1.28.archive
--rw-r--r--   0        0        0   136192 2024-04-11 11:14:40.246903 sirmordred-1.0.0rc2/tests/archives/meetup.archive
--rw-r--r--   0        0        0  2310144 2024-04-11 11:14:40.250903 sirmordred-1.0.0rc2/tests/archives/mozillaclub.archive
--rw-r--r--   0        0        0    35840 2024-04-11 11:14:40.250903 sirmordred-1.0.0rc2/tests/archives/nntp.archive
--rw-r--r--   0        0        0    88064 2024-04-11 11:14:40.250903 sirmordred-1.0.0rc2/tests/archives/phabricator.archive
--rw-r--r--   0        0        0    61440 2024-04-11 11:14:40.250903 sirmordred-1.0.0rc2/tests/archives/redmine.archive
--rw-r--r--   0        0        0   182272 2024-04-11 11:14:40.250903 sirmordred-1.0.0rc2/tests/archives/remo.archive
--rw-r--r--   0        0        0    25600 2024-04-11 11:14:40.250903 sirmordred-1.0.0rc2/tests/archives/rss.archive
--rw-r--r--   0        0        0    86016 2024-04-11 11:14:40.250903 sirmordred-1.0.0rc2/tests/archives/slack.archive
--rw-r--r--   0        0        0    17408 2024-04-11 11:14:40.250903 sirmordred-1.0.0rc2/tests/archives/stackexchange.archive
--rw-r--r--   0        0        0    15360 2024-04-11 11:14:40.250903 sirmordred-1.0.0rc2/tests/archives/telegram.archive
--rw-r--r--   0        0        0   385024 2024-04-11 11:14:40.254902 sirmordred-1.0.0rc2/tests/archives/twitter.archive
--rw-r--r--   0        0        0     1769 2024-04-11 11:14:40.130902 sirmordred-1.0.0rc2/tests/archives-test-projects.json
--rw-r--r--   0        0        0     5845 2024-04-11 11:14:40.130902 sirmordred-1.0.0rc2/tests/archives-test.cfg
--rw-r--r--   0        0        0 15031534 2024-04-11 11:14:40.294903 sirmordred-1.0.0rc2/tests/data/eclipse-projects.json
--rw-r--r--   0        0        0       55 2024-04-11 11:14:40.294903 sirmordred-1.0.0rc2/tests/data/healthcheck_cache_invalid.json
--rw-r--r--   0        0        0       56 2024-04-11 11:14:40.294903 sirmordred-1.0.0rc2/tests/data/healthcheck_cache_valid.json
--rw-r--r--   0        0        0       56 2024-04-11 11:14:40.294903 sirmordred-1.0.0rc2/tests/data/healthcheck_cache_wrong_key.json
--rw-r--r--   0        0        0     2932 2024-04-11 11:14:40.294903 sirmordred-1.0.0rc2/tests/data/mordred.log
--rw-r--r--   0        0        0     3244 2024-04-11 11:14:40.294903 sirmordred-1.0.0rc2/tests/data/orgs_sortinghat.json
--rw-r--r--   0        0        0     3587 2024-04-11 11:14:40.294903 sirmordred-1.0.0rc2/tests/data/perceval_identities_sortinghat.json
--rw-r--r--   0        0        0     3607 2024-04-11 11:14:40.294903 sirmordred-1.0.0rc2/tests/data/remote_identities_sortinghat.json
--rw-r--r--   0        0        0     2032 2024-04-11 11:14:40.294903 sirmordred-1.0.0rc2/tests/data/task-identities-data.json
--rw-r--r--   0        0        0     4487 2024-04-11 11:14:40.294903 sirmordred-1.0.0rc2/tests/data/task-params-expected
--rw-r--r--   0        0        0     1716 2024-04-11 11:14:40.294903 sirmordred-1.0.0rc2/tests/data/task-params-test-projects.json
--rw-r--r--   0        0        0     4392 2024-04-11 11:14:40.294903 sirmordred-1.0.0rc2/tests/data/task-params-test.cfg
--rw-r--r--   0        0        0     2484 2024-04-11 11:14:40.294903 sirmordred-1.0.0rc2/tests/data/url-projects.json
--rwxr-xr-x   0        0        0     1166 2024-04-11 11:14:40.294903 sirmordred-1.0.0rc2/tests/run_tests.py
--rw-r--r--   0        0        0     6585 2024-04-11 11:14:40.294903 sirmordred-1.0.0rc2/tests/sortinghat_settings.py
--rw-r--r--   0        0        0     1451 2024-04-11 11:14:40.294903 sirmordred-1.0.0rc2/tests/test-no-collection.cfg
--rw-r--r--   0        0        0     4655 2024-04-11 11:14:40.294903 sirmordred-1.0.0rc2/tests/test-no-sh.cfg
--rw-r--r--   0        0        0      178 2024-04-11 11:14:40.294903 sirmordred-1.0.0rc2/tests/test-projects-no-collection.json
--rw-r--r--   0        0        0     2484 2024-04-11 11:14:40.294903 sirmordred-1.0.0rc2/tests/test-projects.json
--rw-r--r--   0        0        0      721 2024-04-11 11:14:40.294903 sirmordred-1.0.0rc2/tests/test-repos-projects.json
--rw-r--r--   0        0        0     1798 2024-04-11 11:14:40.294903 sirmordred-1.0.0rc2/tests/test-repos.cfg
--rw-r--r--   0        0        0     4936 2024-04-11 11:14:40.294903 sirmordred-1.0.0rc2/tests/test.cfg
--rw-r--r--   0        0        0    14731 2024-04-11 11:14:40.294903 sirmordred-1.0.0rc2/tests/test_config.py
--rw-r--r--   0        0        0     1849 2024-04-11 11:14:40.294903 sirmordred-1.0.0rc2/tests/test_github.py
--rw-r--r--   0        0        0     3235 2024-04-11 11:14:40.294903 sirmordred-1.0.0rc2/tests/test_healthcheck.py
--rw-r--r--   0        0        0     2706 2024-04-11 11:14:40.294903 sirmordred-1.0.0rc2/tests/test_sirmordred.py
--rw-r--r--   0        0        0     7303 2024-04-11 11:14:40.294903 sirmordred-1.0.0rc2/tests/test_studies.cfg
--rw-r--r--   0        0        0     5392 2024-04-11 11:14:40.294903 sirmordred-1.0.0rc2/tests/test_task.py
--rw-r--r--   0        0        0     6715 2024-04-11 11:14:40.294903 sirmordred-1.0.0rc2/tests/test_task_autorefresh.py
--rw-r--r--   0        0        0     5956 2024-04-11 11:14:40.294903 sirmordred-1.0.0rc2/tests/test_task_collection.py
--rw-r--r--   0        0        0    11770 2024-04-11 11:14:40.294903 sirmordred-1.0.0rc2/tests/test_task_enrich.py
--rw-r--r--   0        0        0     5817 2024-04-11 11:14:40.294903 sirmordred-1.0.0rc2/tests/test_task_identities.py
--rw-r--r--   0        0        0    10141 2024-04-11 11:14:40.294903 sirmordred-1.0.0rc2/tests/test_task_manager.py
--rw-r--r--   0        0        0     6380 2024-04-11 11:14:40.294903 sirmordred-1.0.0rc2/tests/test_task_panels.py
--rw-r--r--   0        0        0    13869 2024-04-11 11:14:40.294903 sirmordred-1.0.0rc2/tests/test_task_projects.py
--rw-r--r--   0        0        0     1499 2024-04-11 11:14:40.294903 sirmordred-1.0.0rc2/tests/test_wrong.cfg
--rw-r--r--   0        0        0    42454 1970-01-01 00:00:00.000000 sirmordred-1.0.0rc2/PKG-INFO
+-rw-r--r--   0        0        0    35147 2024-04-12 16:00:59.783423 sirmordred-1.0.0rc3/LICENSE
+-rw-r--r--   0        0        0    40852 2024-04-12 16:00:59.783423 sirmordred-1.0.0rc3/README.md
+-rw-r--r--   0        0        0     8246 2024-04-12 16:00:59.783423 sirmordred-1.0.0rc3/menu.yaml
+-rw-r--r--   0        0        0     2182 2024-04-12 16:00:59.783423 sirmordred-1.0.0rc3/pyproject.toml
+-rw-r--r--   0        0        0      835 2024-04-12 16:00:59.787423 sirmordred-1.0.0rc3/sirmordred/__init__.py
+-rw-r--r--   0        0        0       91 2024-04-12 16:00:59.787423 sirmordred-1.0.0rc3/sirmordred/_version.py
+-rwxr-xr-x   0        0        0     5022 2024-04-12 16:00:59.787423 sirmordred-1.0.0rc3/sirmordred/bin/sirmordred.py
+-rw-r--r--   0        0        0    33508 2024-04-12 16:00:59.787423 sirmordred-1.0.0rc3/sirmordred/config.py
+-rw-r--r--   0        0        0     1836 2024-04-12 16:00:59.787423 sirmordred-1.0.0rc3/sirmordred/error.py
+-rw-r--r--   0        0        0     2306 2024-04-12 16:00:59.787423 sirmordred-1.0.0rc3/sirmordred/github.py
+-rwxr-xr-x   0        0        0    12432 2024-04-12 16:00:59.787423 sirmordred-1.0.0rc3/sirmordred/sirmordred.py
+-rw-r--r--   0        0        0    10093 2024-04-12 16:00:59.787423 sirmordred-1.0.0rc3/sirmordred/task.py
+-rw-r--r--   0        0        0     7762 2024-04-12 16:00:59.787423 sirmordred-1.0.0rc3/sirmordred/task_autorefresh.py
+-rw-r--r--   0        0        0     6487 2024-04-12 16:00:59.787423 sirmordred-1.0.0rc3/sirmordred/task_collection.py
+-rw-r--r--   0        0        0    21143 2024-04-12 16:00:59.787423 sirmordred-1.0.0rc3/sirmordred/task_enrich.py
+-rw-r--r--   0        0        0     3396 2024-04-12 16:00:59.787423 sirmordred-1.0.0rc3/sirmordred/task_identities.py
+-rw-r--r--   0        0        0     4424 2024-04-12 16:00:59.787423 sirmordred-1.0.0rc3/sirmordred/task_manager.py
+-rw-r--r--   0        0        0    29060 2024-04-12 16:00:59.787423 sirmordred-1.0.0rc3/sirmordred/task_panels.py
+-rw-r--r--   0        0        0     6484 2024-04-12 16:00:59.787423 sirmordred-1.0.0rc3/sirmordred/task_projects.py
+-rw-r--r--   0        0        0     1981 2024-04-12 16:00:59.787423 sirmordred-1.0.0rc3/sirmordred/utils/find_affiliation_conflicts.py
+-rw-r--r--   0        0        0      766 2024-04-12 16:00:59.787423 sirmordred-1.0.0rc3/sirmordred/utils/grimoirelab_valid.yml
+-rwxr-xr-x   0        0        0     4709 2024-04-12 16:00:59.787423 sirmordred-1.0.0rc3/sirmordred/utils/healthcheck.py
+-rw-r--r--   0        0        0        0 2024-04-12 16:00:59.787423 sirmordred-1.0.0rc3/sirmordred/utils/logs/all.log
+-rw-r--r--   0        0        0     7849 2024-04-12 16:00:59.787423 sirmordred-1.0.0rc3/sirmordred/utils/micro.py
+-rw-r--r--   0        0        0     2858 2024-04-12 16:00:59.787423 sirmordred-1.0.0rc3/sirmordred/utils/panels_config.py
+-rw-r--r--   0        0        0      864 2024-04-12 16:00:59.787423 sirmordred-1.0.0rc3/sirmordred/utils/projects.json
+-rw-r--r--   0        0        0     3141 2024-04-12 16:00:59.787423 sirmordred-1.0.0rc3/sirmordred/utils/projects_json2yml.py
+-rw-r--r--   0        0        0     3634 2024-04-12 16:00:59.787423 sirmordred-1.0.0rc3/sirmordred/utils/setup.cfg
+-rw-r--r--   0        0        0     4398 2024-04-12 16:00:59.787423 sirmordred-1.0.0rc3/tests/aliases.json
+-rw-r--r--   0        0        0   497664 2024-04-12 16:00:59.791423 sirmordred-1.0.0rc3/tests/archives/askbot.archive
+-rw-r--r--   0        0        0   150528 2024-04-12 16:00:59.791423 sirmordred-1.0.0rc3/tests/archives/bugzilla.archive
+-rw-r--r--   0        0        0    52224 2024-04-12 16:00:59.791423 sirmordred-1.0.0rc3/tests/archives/bugzillarest.archive
+-rw-r--r--   0        0        0    73728 2024-04-12 16:00:59.791423 sirmordred-1.0.0rc3/tests/archives/confluence.archive
+-rw-r--r--   0        0        0  7141376 2024-04-12 16:00:59.811423 sirmordred-1.0.0rc3/tests/archives/crates.archive
+-rw-r--r--   0        0        0   291840 2024-04-12 16:00:59.811423 sirmordred-1.0.0rc3/tests/archives/discourse.archive
+-rw-r--r--   0        0        0    16384 2024-04-12 16:00:59.811423 sirmordred-1.0.0rc3/tests/archives/dockerhub.archive
+-rw-r--r--   0        0        0  1713152 2024-04-12 16:00:59.815423 sirmordred-1.0.0rc3/tests/archives/functest.archive
+-rw-r--r--   0        0        0    49152 2024-04-12 16:00:59.815423 sirmordred-1.0.0rc3/tests/archives/gerrit.archive
+-rw-r--r--   0        0        0  9424896 2024-04-12 16:00:59.867423 sirmordred-1.0.0rc3/tests/archives/github-issue.archive
+-rw-r--r--   0        0        0 23023616 2024-04-12 16:00:59.895423 sirmordred-1.0.0rc3/tests/archives/github-pull.archive
+-rw-r--r--   0        0        0   208896 2024-04-12 16:00:59.895423 sirmordred-1.0.0rc3/tests/archives/gitlab-issue.archive
+-rw-r--r--   0        0        0   937984 2024-04-12 16:00:59.899423 sirmordred-1.0.0rc3/tests/archives/gitlab-merge.archive
+-rw-r--r--   0        0        0    65536 2024-04-12 16:00:59.899423 sirmordred-1.0.0rc3/tests/archives/googlehits.archive
+-rw-r--r--   0        0        0   228352 2024-04-12 16:00:59.899423 sirmordred-1.0.0rc3/tests/archives/jenkins.archive
+-rw-r--r--   0        0        0    86016 2024-04-12 16:00:59.899423 sirmordred-1.0.0rc3/tests/archives/jira.archive
+-rw-r--r--   0        0        0    69632 2024-04-12 16:00:59.899423 sirmordred-1.0.0rc3/tests/archives/launchpad.archive
+-rw-r--r--   0        0        0    31744 2024-04-12 16:00:59.899423 sirmordred-1.0.0rc3/tests/archives/mediawiki-1.23.archive
+-rw-r--r--   0        0        0   245760 2024-04-12 16:00:59.899423 sirmordred-1.0.0rc3/tests/archives/mediawiki-1.28.archive
+-rw-r--r--   0        0        0   136192 2024-04-12 16:00:59.899423 sirmordred-1.0.0rc3/tests/archives/meetup.archive
+-rw-r--r--   0        0        0  2310144 2024-04-12 16:00:59.907423 sirmordred-1.0.0rc3/tests/archives/mozillaclub.archive
+-rw-r--r--   0        0        0    35840 2024-04-12 16:00:59.907423 sirmordred-1.0.0rc3/tests/archives/nntp.archive
+-rw-r--r--   0        0        0    88064 2024-04-12 16:00:59.907423 sirmordred-1.0.0rc3/tests/archives/phabricator.archive
+-rw-r--r--   0        0        0    61440 2024-04-12 16:00:59.907423 sirmordred-1.0.0rc3/tests/archives/redmine.archive
+-rw-r--r--   0        0        0   182272 2024-04-12 16:00:59.907423 sirmordred-1.0.0rc3/tests/archives/remo.archive
+-rw-r--r--   0        0        0    25600 2024-04-12 16:00:59.907423 sirmordred-1.0.0rc3/tests/archives/rss.archive
+-rw-r--r--   0        0        0    86016 2024-04-12 16:00:59.907423 sirmordred-1.0.0rc3/tests/archives/slack.archive
+-rw-r--r--   0        0        0    17408 2024-04-12 16:00:59.907423 sirmordred-1.0.0rc3/tests/archives/stackexchange.archive
+-rw-r--r--   0        0        0    15360 2024-04-12 16:00:59.907423 sirmordred-1.0.0rc3/tests/archives/telegram.archive
+-rw-r--r--   0        0        0   385024 2024-04-12 16:00:59.907423 sirmordred-1.0.0rc3/tests/archives/twitter.archive
+-rw-r--r--   0        0        0     1769 2024-04-12 16:00:59.787423 sirmordred-1.0.0rc3/tests/archives-test-projects.json
+-rw-r--r--   0        0        0     5845 2024-04-12 16:00:59.787423 sirmordred-1.0.0rc3/tests/archives-test.cfg
+-rw-r--r--   0        0        0 15031534 2024-04-12 16:00:59.947422 sirmordred-1.0.0rc3/tests/data/eclipse-projects.json
+-rw-r--r--   0        0        0       55 2024-04-12 16:00:59.947422 sirmordred-1.0.0rc3/tests/data/healthcheck_cache_invalid.json
+-rw-r--r--   0        0        0       56 2024-04-12 16:00:59.947422 sirmordred-1.0.0rc3/tests/data/healthcheck_cache_valid.json
+-rw-r--r--   0        0        0       56 2024-04-12 16:00:59.947422 sirmordred-1.0.0rc3/tests/data/healthcheck_cache_wrong_key.json
+-rw-r--r--   0        0        0     2932 2024-04-12 16:00:59.951422 sirmordred-1.0.0rc3/tests/data/mordred.log
+-rw-r--r--   0        0        0     3244 2024-04-12 16:00:59.951422 sirmordred-1.0.0rc3/tests/data/orgs_sortinghat.json
+-rw-r--r--   0        0        0     3587 2024-04-12 16:00:59.951422 sirmordred-1.0.0rc3/tests/data/perceval_identities_sortinghat.json
+-rw-r--r--   0        0        0     3607 2024-04-12 16:00:59.951422 sirmordred-1.0.0rc3/tests/data/remote_identities_sortinghat.json
+-rw-r--r--   0        0        0     2032 2024-04-12 16:00:59.951422 sirmordred-1.0.0rc3/tests/data/task-identities-data.json
+-rw-r--r--   0        0        0     4487 2024-04-12 16:00:59.951422 sirmordred-1.0.0rc3/tests/data/task-params-expected
+-rw-r--r--   0        0        0     1716 2024-04-12 16:00:59.951422 sirmordred-1.0.0rc3/tests/data/task-params-test-projects.json
+-rw-r--r--   0        0        0     4392 2024-04-12 16:00:59.951422 sirmordred-1.0.0rc3/tests/data/task-params-test.cfg
+-rw-r--r--   0        0        0     2484 2024-04-12 16:00:59.951422 sirmordred-1.0.0rc3/tests/data/url-projects.json
+-rwxr-xr-x   0        0        0     1166 2024-04-12 16:00:59.951422 sirmordred-1.0.0rc3/tests/run_tests.py
+-rw-r--r--   0        0        0     6585 2024-04-12 16:00:59.951422 sirmordred-1.0.0rc3/tests/sortinghat_settings.py
+-rw-r--r--   0        0        0     1451 2024-04-12 16:00:59.951422 sirmordred-1.0.0rc3/tests/test-no-collection.cfg
+-rw-r--r--   0        0        0     4655 2024-04-12 16:00:59.951422 sirmordred-1.0.0rc3/tests/test-no-sh.cfg
+-rw-r--r--   0        0        0      178 2024-04-12 16:00:59.951422 sirmordred-1.0.0rc3/tests/test-projects-no-collection.json
+-rw-r--r--   0        0        0     2484 2024-04-12 16:00:59.951422 sirmordred-1.0.0rc3/tests/test-projects.json
+-rw-r--r--   0        0        0      721 2024-04-12 16:00:59.951422 sirmordred-1.0.0rc3/tests/test-repos-projects.json
+-rw-r--r--   0        0        0     1798 2024-04-12 16:00:59.951422 sirmordred-1.0.0rc3/tests/test-repos.cfg
+-rw-r--r--   0        0        0     4936 2024-04-12 16:00:59.951422 sirmordred-1.0.0rc3/tests/test.cfg
+-rw-r--r--   0        0        0    14731 2024-04-12 16:00:59.951422 sirmordred-1.0.0rc3/tests/test_config.py
+-rw-r--r--   0        0        0     1849 2024-04-12 16:00:59.951422 sirmordred-1.0.0rc3/tests/test_github.py
+-rw-r--r--   0        0        0     3235 2024-04-12 16:00:59.951422 sirmordred-1.0.0rc3/tests/test_healthcheck.py
+-rw-r--r--   0        0        0     2706 2024-04-12 16:00:59.951422 sirmordred-1.0.0rc3/tests/test_sirmordred.py
+-rw-r--r--   0        0        0     7303 2024-04-12 16:00:59.951422 sirmordred-1.0.0rc3/tests/test_studies.cfg
+-rw-r--r--   0        0        0     5392 2024-04-12 16:00:59.951422 sirmordred-1.0.0rc3/tests/test_task.py
+-rw-r--r--   0        0        0     6715 2024-04-12 16:00:59.951422 sirmordred-1.0.0rc3/tests/test_task_autorefresh.py
+-rw-r--r--   0        0        0     5956 2024-04-12 16:00:59.951422 sirmordred-1.0.0rc3/tests/test_task_collection.py
+-rw-r--r--   0        0        0    11770 2024-04-12 16:00:59.951422 sirmordred-1.0.0rc3/tests/test_task_enrich.py
+-rw-r--r--   0        0        0     5817 2024-04-12 16:00:59.951422 sirmordred-1.0.0rc3/tests/test_task_identities.py
+-rw-r--r--   0        0        0    10141 2024-04-12 16:00:59.951422 sirmordred-1.0.0rc3/tests/test_task_manager.py
+-rw-r--r--   0        0        0     6380 2024-04-12 16:00:59.951422 sirmordred-1.0.0rc3/tests/test_task_panels.py
+-rw-r--r--   0        0        0    13869 2024-04-12 16:00:59.951422 sirmordred-1.0.0rc3/tests/test_task_projects.py
+-rw-r--r--   0        0        0     1499 2024-04-12 16:00:59.951422 sirmordred-1.0.0rc3/tests/test_wrong.cfg
+-rw-r--r--   0        0        0    42454 1970-01-01 00:00:00.000000 sirmordred-1.0.0rc3/PKG-INFO
```

### Comparing `sirmordred-1.0.0rc2/LICENSE` & `sirmordred-1.0.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/README.md` & `sirmordred-1.0.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/menu.yaml` & `sirmordred-1.0.0rc3/menu.yaml`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/pyproject.toml` & `sirmordred-1.0.0rc3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sirmordred"
-version = "1.0.0-rc.2"
+version = "1.0.0-rc.3"
 description = "Drive GrimoireLab tools to produce a dashboard"
 authors = [
     "GrimoireLab Developers"
 ]
 license = "GPL-3.0+"
 
 readme = "README.md"
```

### Comparing `sirmordred-1.0.0rc2/sirmordred/__init__.py` & `sirmordred-1.0.0rc3/sirmordred/__init__.py`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/sirmordred/bin/sirmordred.py` & `sirmordred-1.0.0rc3/sirmordred/bin/sirmordred.py`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/sirmordred/config.py` & `sirmordred-1.0.0rc3/sirmordred/config.py`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/sirmordred/error.py` & `sirmordred-1.0.0rc3/sirmordred/error.py`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/sirmordred/github.py` & `sirmordred-1.0.0rc3/sirmordred/github.py`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/sirmordred/sirmordred.py` & `sirmordred-1.0.0rc3/sirmordred/sirmordred.py`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/sirmordred/task.py` & `sirmordred-1.0.0rc3/sirmordred/task.py`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/sirmordred/task_autorefresh.py` & `sirmordred-1.0.0rc3/sirmordred/task_autorefresh.py`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/sirmordred/task_collection.py` & `sirmordred-1.0.0rc3/sirmordred/task_collection.py`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/sirmordred/task_enrich.py` & `sirmordred-1.0.0rc3/sirmordred/task_enrich.py`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/sirmordred/task_identities.py` & `sirmordred-1.0.0rc3/sirmordred/task_identities.py`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/sirmordred/task_manager.py` & `sirmordred-1.0.0rc3/sirmordred/task_manager.py`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/sirmordred/task_panels.py` & `sirmordred-1.0.0rc3/sirmordred/task_panels.py`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/sirmordred/task_projects.py` & `sirmordred-1.0.0rc3/sirmordred/task_projects.py`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/sirmordred/utils/find_affiliation_conflicts.py` & `sirmordred-1.0.0rc3/sirmordred/utils/find_affiliation_conflicts.py`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/sirmordred/utils/grimoirelab_valid.yml` & `sirmordred-1.0.0rc3/sirmordred/utils/grimoirelab_valid.yml`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/sirmordred/utils/healthcheck.py` & `sirmordred-1.0.0rc3/sirmordred/utils/healthcheck.py`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/sirmordred/utils/micro.py` & `sirmordred-1.0.0rc3/sirmordred/utils/micro.py`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/sirmordred/utils/panels_config.py` & `sirmordred-1.0.0rc3/sirmordred/utils/panels_config.py`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/sirmordred/utils/projects.json` & `sirmordred-1.0.0rc3/sirmordred/utils/projects.json`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/sirmordred/utils/projects_json2yml.py` & `sirmordred-1.0.0rc3/sirmordred/utils/projects_json2yml.py`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/sirmordred/utils/setup.cfg` & `sirmordred-1.0.0rc3/sirmordred/utils/setup.cfg`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/tests/aliases.json` & `sirmordred-1.0.0rc3/tests/aliases.json`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/tests/archives/askbot.archive` & `sirmordred-1.0.0rc3/tests/archives/askbot.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/tests/archives/bugzilla.archive` & `sirmordred-1.0.0rc3/tests/archives/bugzilla.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/tests/archives/bugzillarest.archive` & `sirmordred-1.0.0rc3/tests/archives/bugzillarest.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/tests/archives/confluence.archive` & `sirmordred-1.0.0rc3/tests/archives/confluence.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/tests/archives/crates.archive` & `sirmordred-1.0.0rc3/tests/archives/crates.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/tests/archives/discourse.archive` & `sirmordred-1.0.0rc3/tests/archives/discourse.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/tests/archives/dockerhub.archive` & `sirmordred-1.0.0rc3/tests/archives/dockerhub.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/tests/archives/functest.archive` & `sirmordred-1.0.0rc3/tests/archives/functest.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/tests/archives/gerrit.archive` & `sirmordred-1.0.0rc3/tests/archives/gerrit.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/tests/archives/github-issue.archive` & `sirmordred-1.0.0rc3/tests/archives/github-issue.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/tests/archives/github-pull.archive` & `sirmordred-1.0.0rc3/tests/archives/github-pull.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/tests/archives/gitlab-issue.archive` & `sirmordred-1.0.0rc3/tests/archives/gitlab-issue.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/tests/archives/gitlab-merge.archive` & `sirmordred-1.0.0rc3/tests/archives/gitlab-merge.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/tests/archives/googlehits.archive` & `sirmordred-1.0.0rc3/tests/archives/googlehits.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/tests/archives/jenkins.archive` & `sirmordred-1.0.0rc3/tests/archives/jenkins.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/tests/archives/jira.archive` & `sirmordred-1.0.0rc3/tests/archives/jira.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/tests/archives/launchpad.archive` & `sirmordred-1.0.0rc3/tests/archives/launchpad.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/tests/archives/mediawiki-1.23.archive` & `sirmordred-1.0.0rc3/tests/archives/mediawiki-1.23.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/tests/archives/mediawiki-1.28.archive` & `sirmordred-1.0.0rc3/tests/archives/mediawiki-1.28.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/tests/archives/meetup.archive` & `sirmordred-1.0.0rc3/tests/archives/meetup.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/tests/archives/mozillaclub.archive` & `sirmordred-1.0.0rc3/tests/archives/mozillaclub.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/tests/archives/nntp.archive` & `sirmordred-1.0.0rc3/tests/archives/nntp.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/tests/archives/phabricator.archive` & `sirmordred-1.0.0rc3/tests/archives/phabricator.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/tests/archives/redmine.archive` & `sirmordred-1.0.0rc3/tests/archives/redmine.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/tests/archives/remo.archive` & `sirmordred-1.0.0rc3/tests/archives/remo.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/tests/archives/rss.archive` & `sirmordred-1.0.0rc3/tests/archives/rss.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/tests/archives/slack.archive` & `sirmordred-1.0.0rc3/tests/archives/slack.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/tests/archives/stackexchange.archive` & `sirmordred-1.0.0rc3/tests/archives/stackexchange.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/tests/archives/telegram.archive` & `sirmordred-1.0.0rc3/tests/archives/telegram.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/tests/archives/twitter.archive` & `sirmordred-1.0.0rc3/tests/archives/twitter.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/tests/archives-test-projects.json` & `sirmordred-1.0.0rc3/tests/archives-test-projects.json`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/tests/archives-test.cfg` & `sirmordred-1.0.0rc3/tests/archives-test.cfg`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/tests/data/eclipse-projects.json` & `sirmordred-1.0.0rc3/tests/data/eclipse-projects.json`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/tests/data/mordred.log` & `sirmordred-1.0.0rc3/tests/data/mordred.log`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/tests/data/orgs_sortinghat.json` & `sirmordred-1.0.0rc3/tests/data/orgs_sortinghat.json`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/tests/data/perceval_identities_sortinghat.json` & `sirmordred-1.0.0rc3/tests/data/perceval_identities_sortinghat.json`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/tests/data/remote_identities_sortinghat.json` & `sirmordred-1.0.0rc3/tests/data/remote_identities_sortinghat.json`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/tests/data/task-identities-data.json` & `sirmordred-1.0.0rc3/tests/data/task-identities-data.json`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/tests/data/task-params-expected` & `sirmordred-1.0.0rc3/tests/data/task-params-expected`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/tests/data/task-params-test-projects.json` & `sirmordred-1.0.0rc3/tests/data/task-params-test-projects.json`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/tests/data/task-params-test.cfg` & `sirmordred-1.0.0rc3/tests/data/task-params-test.cfg`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/tests/data/url-projects.json` & `sirmordred-1.0.0rc3/tests/data/url-projects.json`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/tests/run_tests.py` & `sirmordred-1.0.0rc3/tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/tests/sortinghat_settings.py` & `sirmordred-1.0.0rc3/tests/sortinghat_settings.py`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/tests/test-no-collection.cfg` & `sirmordred-1.0.0rc3/tests/test-no-collection.cfg`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/tests/test-no-sh.cfg` & `sirmordred-1.0.0rc3/tests/test-no-sh.cfg`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/tests/test-projects.json` & `sirmordred-1.0.0rc3/tests/test-projects.json`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/tests/test-repos-projects.json` & `sirmordred-1.0.0rc3/tests/test-repos-projects.json`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/tests/test-repos.cfg` & `sirmordred-1.0.0rc3/tests/test-repos.cfg`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/tests/test.cfg` & `sirmordred-1.0.0rc3/tests/test.cfg`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/tests/test_config.py` & `sirmordred-1.0.0rc3/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/tests/test_github.py` & `sirmordred-1.0.0rc3/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/tests/test_healthcheck.py` & `sirmordred-1.0.0rc3/tests/test_healthcheck.py`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/tests/test_sirmordred.py` & `sirmordred-1.0.0rc3/tests/test_sirmordred.py`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/tests/test_studies.cfg` & `sirmordred-1.0.0rc3/tests/test_studies.cfg`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/tests/test_task.py` & `sirmordred-1.0.0rc3/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/tests/test_task_autorefresh.py` & `sirmordred-1.0.0rc3/tests/test_task_autorefresh.py`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/tests/test_task_collection.py` & `sirmordred-1.0.0rc3/tests/test_task_collection.py`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/tests/test_task_enrich.py` & `sirmordred-1.0.0rc3/tests/test_task_enrich.py`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/tests/test_task_identities.py` & `sirmordred-1.0.0rc3/tests/test_task_identities.py`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/tests/test_task_manager.py` & `sirmordred-1.0.0rc3/tests/test_task_manager.py`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/tests/test_task_panels.py` & `sirmordred-1.0.0rc3/tests/test_task_panels.py`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/tests/test_task_projects.py` & `sirmordred-1.0.0rc3/tests/test_task_projects.py`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/tests/test_wrong.cfg` & `sirmordred-1.0.0rc3/tests/test_wrong.cfg`

 * *Files identical despite different names*

### Comparing `sirmordred-1.0.0rc2/PKG-INFO` & `sirmordred-1.0.0rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sirmordred
-Version: 1.0.0rc2
+Version: 1.0.0rc3
 Summary: Drive GrimoireLab tools to produce a dashboard
 Home-page: https://chaoss.github.io/grimoirelab/
 License: GPL-3.0+
 Keywords: development,grimoirelab
 Author: GrimoireLab Developers
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

