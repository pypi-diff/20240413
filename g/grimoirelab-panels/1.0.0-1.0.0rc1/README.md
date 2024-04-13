# Comparing `tmp/grimoirelab_panels-1.0.0.tar.gz` & `tmp/grimoirelab_panels-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grimoirelab_panels-1.0.0.tar", max compression
+gzip compressed data, was "grimoirelab_panels-1.0.0rc1.tar", max compression
```

## Comparing `grimoirelab_panels-1.0.0.tar` & `grimoirelab_panels-1.0.0rc1.tar`

### file list

```diff
@@ -1,173 +1,173 @@
--rw-r--r--   0        0        0      381 2024-04-13 07:20:59.827931 grimoirelab_panels-1.0.0/AUTHORS
--rw-r--r--   0        0        0    35147 2024-04-13 07:20:59.827931 grimoirelab_panels-1.0.0/LICENSE
--rw-r--r--   0        0        0      871 2024-04-13 07:20:59.827931 grimoirelab_panels-1.0.0/NEWS
--rw-r--r--   0        0        0     6549 2024-04-13 07:20:59.827931 grimoirelab_panels-1.0.0/README.md
--rw-r--r--   0        0        0        0 2024-04-13 07:20:59.963930 grimoirelab_panels-1.0.0/panels/__init__.py
--rw-r--r--   0        0        0       86 2024-04-13 07:20:59.963930 grimoirelab_panels-1.0.0/panels/_version.py
--rw-r--r--   0        0        0     7506 2024-04-13 07:20:59.963930 grimoirelab_panels-1.0.0/panels/json/about.json
--rw-r--r--   0        0        0    92381 2024-04-13 07:20:59.963930 grimoirelab_panels-1.0.0/panels/json/affiliations-index-pattern.json
--rw-r--r--   0        0        0    14883 2024-04-13 07:20:59.963930 grimoirelab_panels-1.0.0/panels/json/affiliations.json
--rw-r--r--   0        0        0    56854 2024-04-13 07:20:59.963930 grimoirelab_panels-1.0.0/panels/json/all_enriched-index-pattern.json
--rw-r--r--   0        0        0    15123 2024-04-13 07:20:59.963930 grimoirelab_panels-1.0.0/panels/json/all_enriched_tickets-index-pattern.json
--rw-r--r--   0        0        0     3517 2024-04-13 07:20:59.963930 grimoirelab_panels-1.0.0/panels/json/all_onion-index-pattern.json
--rw-r--r--   0        0        0     3157 2024-04-13 07:20:59.963930 grimoirelab_panels-1.0.0/panels/json/apache-index-pattern.json
--rw-r--r--   0        0        0    14699 2024-04-13 07:20:59.963930 grimoirelab_panels-1.0.0/panels/json/apache.json
--rw-r--r--   0        0        0     8849 2024-04-13 07:20:59.963930 grimoirelab_panels-1.0.0/panels/json/askbot-index-pattern.json
--rw-r--r--   0        0        0    28220 2024-04-13 07:20:59.963930 grimoirelab_panels-1.0.0/panels/json/askbot.json
--rw-r--r--   0        0        0    29699 2024-04-13 07:20:59.963930 grimoirelab_panels-1.0.0/panels/json/attracted-contributors.json
--rw-r--r--   0        0        0    19600 2024-04-13 07:20:59.963930 grimoirelab_panels-1.0.0/panels/json/bugzilla-index-pattern.json
--rw-r--r--   0        0        0    16078 2024-04-13 07:20:59.963930 grimoirelab_panels-1.0.0/panels/json/bugzilla.json
--rw-r--r--   0        0        0    16857 2024-04-13 07:20:59.963930 grimoirelab_panels-1.0.0/panels/json/bugzilla_backlog.json
--rw-r--r--   0        0        0    29242 2024-04-13 07:20:59.963930 grimoirelab_panels-1.0.0/panels/json/bugzilla_timing.json
--rw-r--r--   0        0        0     5836 2024-04-13 07:20:59.963930 grimoirelab_panels-1.0.0/panels/json/cocom-index-pattern.json
--rw-r--r--   0        0        0    23781 2024-04-13 07:20:59.963930 grimoirelab_panels-1.0.0/panels/json/cocom.json
--rw-r--r--   0        0        0     3711 2024-04-13 07:20:59.963930 grimoirelab_panels-1.0.0/panels/json/cocom_study-index-pattern.json
--rw-r--r--   0        0        0     5413 2024-04-13 07:20:59.963930 grimoirelab_panels-1.0.0/panels/json/colic-index-pattern.json
--rw-r--r--   0        0        0    23795 2024-04-13 07:20:59.963930 grimoirelab_panels-1.0.0/panels/json/colic.json
--rw-r--r--   0        0        0     2656 2024-04-13 07:20:59.963930 grimoirelab_panels-1.0.0/panels/json/colic_study-index-pattern.json
--rw-r--r--   0        0        0     7887 2024-04-13 07:20:59.963930 grimoirelab_panels-1.0.0/panels/json/confluence-index-pattern.json
--rw-r--r--   0        0        0    16237 2024-04-13 07:20:59.963930 grimoirelab_panels-1.0.0/panels/json/confluence.json
--rw-r--r--   0        0        0    10565 2024-04-13 07:20:59.963930 grimoirelab_panels-1.0.0/panels/json/contributors_growth.json
--rw-r--r--   0        0        0    62471 2024-04-13 07:20:59.963930 grimoirelab_panels-1.0.0/panels/json/data_status.json
--rw-r--r--   0        0        0    16442 2024-04-13 07:20:59.963930 grimoirelab_panels-1.0.0/panels/json/demographics-index-pattern.json
--rw-r--r--   0        0        0    22408 2024-04-13 07:20:59.963930 grimoirelab_panels-1.0.0/panels/json/demographics.json
--rw-r--r--   0        0        0    22967 2024-04-13 07:20:59.963930 grimoirelab_panels-1.0.0/panels/json/demographics_contribution-index-pattern.json
--rw-r--r--   0        0        0     9092 2024-04-13 07:20:59.963930 grimoirelab_panels-1.0.0/panels/json/discourse-index-pattern.json
--rw-r--r--   0        0        0    26733 2024-04-13 07:20:59.963930 grimoirelab_panels-1.0.0/panels/json/discourse.json
--rw-r--r--   0        0        0     6199 2024-04-13 07:20:59.963930 grimoirelab_panels-1.0.0/panels/json/discourse_devrel.json
--rw-r--r--   0        0        0    17850 2024-04-13 07:20:59.963930 grimoirelab_panels-1.0.0/panels/json/docker.json
--rw-r--r--   0        0        0     3136 2024-04-13 07:20:59.963930 grimoirelab_panels-1.0.0/panels/json/docker_deps-index-pattern.json
--rw-r--r--   0        0        0     3427 2024-04-13 07:20:59.963930 grimoirelab_panels-1.0.0/panels/json/docker_smells-index-pattern.json
--rw-r--r--   0        0        0     4642 2024-04-13 07:20:59.963930 grimoirelab_panels-1.0.0/panels/json/dockerhub-index-pattern.json
--rw-r--r--   0        0        0     8082 2024-04-13 07:20:59.963930 grimoirelab_panels-1.0.0/panels/json/dockerhub.json
--rw-r--r--   0        0        0     9208 2024-04-13 07:20:59.967930 grimoirelab_panels-1.0.0/panels/json/emtech/adoption/crates-emergintech-index-pattern.json
--rw-r--r--   0        0        0    12721 2024-04-13 07:20:59.967930 grimoirelab_panels-1.0.0/panels/json/emtech/adoption/emerging_tech_adoption.json
--rw-r--r--   0        0        0     7374 2024-04-13 07:20:59.967930 grimoirelab_panels-1.0.0/panels/json/emtech/adoption/emerging_tech_adoption_no_crates.json
--rw-r--r--   0        0        0    11551 2024-04-13 07:20:59.967930 grimoirelab_panels-1.0.0/panels/json/emtech/adoption/github_issues-index-pattern.json
--rw-r--r--   0        0        0    49294 2024-04-13 07:20:59.967930 grimoirelab_panels-1.0.0/panels/json/emtech/dev/emerging_tech_dev.json
--rw-r--r--   0        0        0    11652 2024-04-13 07:20:59.967930 grimoirelab_panels-1.0.0/panels/json/emtech/dev/git-emergingtech-index-pattern.json
--rw-r--r--   0        0        0     6424 2024-04-13 07:20:59.967930 grimoirelab_panels-1.0.0/panels/json/emtech/dev/git_areas_of_code-index-pattern.json
--rw-r--r--   0        0        0    11840 2024-04-13 07:20:59.967930 grimoirelab_panels-1.0.0/panels/json/emtech/dev/github-emergingtech-index-pattern.json
--rw-r--r--   0        0        0    37258 2024-04-13 07:20:59.967930 grimoirelab_panels-1.0.0/panels/json/emtech/social/emerging_tech_social.json
--rw-r--r--   0        0        0     6333 2024-04-13 07:20:59.967930 grimoirelab_panels-1.0.0/panels/json/emtech/social/irc-emergingtech-index-pattern.json
--rw-r--r--   0        0        0    12257 2024-04-13 07:20:59.967930 grimoirelab_panels-1.0.0/panels/json/emtech/social/meetup-emergingtech-index-pattern.json
--rw-r--r--   0        0        0    11496 2024-04-13 07:20:59.967930 grimoirelab_panels-1.0.0/panels/json/emtech/social/slack-emergingtech-index-pattern.json
--rw-r--r--   0        0        0    10218 2024-04-13 07:20:59.967930 grimoirelab_panels-1.0.0/panels/json/emtech/social/stackoverflow-emergingtech-index-pattern.json
--rw-r--r--   0        0        0    10286 2024-04-13 07:20:59.967930 grimoirelab_panels-1.0.0/panels/json/emtech/social/twitter_emergingtech-index-pattern.json
--rw-r--r--   0        0        0    10779 2024-04-13 07:20:59.967930 grimoirelab_panels-1.0.0/panels/json/engagement_by_contributions.json
--rw-r--r--   0        0        0     4856 2024-04-13 07:20:59.967930 grimoirelab_panels-1.0.0/panels/json/functest-index-pattern.json
--rw-r--r--   0        0        0    22360 2024-04-13 07:20:59.967930 grimoirelab_panels-1.0.0/panels/json/gerrit-index-pattern.json
--rw-r--r--   0        0        0    21175 2024-04-13 07:20:59.967930 grimoirelab_panels-1.0.0/panels/json/gerrit.json
--rw-r--r--   0        0        0    20808 2024-04-13 07:20:59.967930 grimoirelab_panels-1.0.0/panels/json/gerrit_approvals.json
--rw-r--r--   0        0        0    18636 2024-04-13 07:20:59.967930 grimoirelab_panels-1.0.0/panels/json/gerrit_backlog.json
--rw-r--r--   0        0        0    10022 2024-04-13 07:20:59.967930 grimoirelab_panels-1.0.0/panels/json/gerrit_efficiency.json
--rw-r--r--   0        0        0    25489 2024-04-13 07:20:59.967930 grimoirelab_panels-1.0.0/panels/json/gerrit_retention_newcomers.json
--rw-r--r--   0        0        0    17434 2024-04-13 07:20:59.967930 grimoirelab_panels-1.0.0/panels/json/gerrit_timing.json
--rw-r--r--   0        0        0    26898 2024-04-13 07:20:59.967930 grimoirelab_panels-1.0.0/panels/json/git-index-pattern.json
--rw-r--r--   0        0        0    19030 2024-04-13 07:20:59.967930 grimoirelab_panels-1.0.0/panels/json/git.json
--rw-r--r--   0        0        0     7040 2024-04-13 07:20:59.967930 grimoirelab_panels-1.0.0/panels/json/git_areas_of_code-index-pattern.json
--rw-r--r--   0        0        0    20965 2024-04-13 07:20:59.967930 grimoirelab_panels-1.0.0/panels/json/git_areas_of_code.json
--rw-r--r--   0        0        0    23802 2024-04-13 07:20:59.967930 grimoirelab_panels-1.0.0/panels/json/git_demographics.json
--rw-r--r--   0        0        0    19262 2024-04-13 07:20:59.967930 grimoirelab_panels-1.0.0/panels/json/git_pair_programming.json
--rw-r--r--   0        0        0    19173 2024-04-13 07:20:59.967930 grimoirelab_panels-1.0.0/panels/json/github2_issues-index-pattern.json
--rw-r--r--   0        0        0    20757 2024-04-13 07:20:59.967930 grimoirelab_panels-1.0.0/panels/json/github2_issues_comments_and_collaboration.json
--rw-r--r--   0        0        0    32469 2024-04-13 07:20:59.967930 grimoirelab_panels-1.0.0/panels/json/github2_issues_comments_feelings.json
--rw-r--r--   0        0        0    21762 2024-04-13 07:20:59.967930 grimoirelab_panels-1.0.0/panels/json/github2_pull_requests-index-pattern.json
--rw-r--r--   0        0        0    21093 2024-04-13 07:20:59.967930 grimoirelab_panels-1.0.0/panels/json/github2_pull_requests_comments_and_collaboration.json
--rw-r--r--   0        0        0    15171 2024-04-13 07:20:59.967930 grimoirelab_panels-1.0.0/panels/json/github_devrel.json
--rw-r--r--   0        0        0    21142 2024-04-13 07:20:59.967930 grimoirelab_panels-1.0.0/panels/json/github_events-index-pattern.json
--rw-r--r--   0        0        0    18416 2024-04-13 07:20:59.967930 grimoirelab_panels-1.0.0/panels/json/github_events_closed.json
--rw-r--r--   0        0        0    31092 2024-04-13 07:20:59.967930 grimoirelab_panels-1.0.0/panels/json/github_events_labels.json
--rw-r--r--   0        0        0    18716 2024-04-13 07:20:59.967930 grimoirelab_panels-1.0.0/panels/json/github_issues-index-pattern.json
--rw-r--r--   0        0        0    17412 2024-04-13 07:20:59.967930 grimoirelab_panels-1.0.0/panels/json/github_issues.json
--rw-r--r--   0        0        0    17482 2024-04-13 07:20:59.967930 grimoirelab_panels-1.0.0/panels/json/github_issues_backlog.json
--rw-r--r--   0        0        0    11033 2024-04-13 07:20:59.967930 grimoirelab_panels-1.0.0/panels/json/github_issues_efficiency.json
--rw-r--r--   0        0        0    26375 2024-04-13 07:20:59.967930 grimoirelab_panels-1.0.0/panels/json/github_issues_timing.json
--rw-r--r--   0        0        0    17034 2024-04-13 07:20:59.967930 grimoirelab_panels-1.0.0/panels/json/github_pull_requests.json
--rw-r--r--   0        0        0    18852 2024-04-13 07:20:59.967930 grimoirelab_panels-1.0.0/panels/json/github_pull_requests_backlog.json
--rw-r--r--   0        0        0    11156 2024-04-13 07:20:59.967930 grimoirelab_panels-1.0.0/panels/json/github_pull_requests_efficiency.json
--rw-r--r--   0        0        0    26979 2024-04-13 07:20:59.967930 grimoirelab_panels-1.0.0/panels/json/github_pull_requests_timing.json
--rw-r--r--   0        0        0     4619 2024-04-13 07:20:59.967930 grimoirelab_panels-1.0.0/panels/json/github_repositories-index-pattern.json
--rw-r--r--   0        0        0    16044 2024-04-13 07:20:59.967930 grimoirelab_panels-1.0.0/panels/json/github_repositories.json
--rw-r--r--   0        0        0    10656 2024-04-13 07:20:59.967930 grimoirelab_panels-1.0.0/panels/json/gitlab_issues-index-pattern.json
--rw-r--r--   0        0        0    20483 2024-04-13 07:20:59.967930 grimoirelab_panels-1.0.0/panels/json/gitlab_issues.json
--rw-r--r--   0        0        0    19812 2024-04-13 07:20:59.967930 grimoirelab_panels-1.0.0/panels/json/gitlab_issues_backlog.json
--rw-r--r--   0        0        0     9623 2024-04-13 07:20:59.967930 grimoirelab_panels-1.0.0/panels/json/gitlab_issues_efficiency.json
--rw-r--r--   0        0        0    26291 2024-04-13 07:20:59.967930 grimoirelab_panels-1.0.0/panels/json/gitlab_issues_timing.json
--rw-r--r--   0        0        0    10574 2024-04-13 07:20:59.971931 grimoirelab_panels-1.0.0/panels/json/gitlab_merge_requests-index-pattern.json
--rw-r--r--   0        0        0    20199 2024-04-13 07:20:59.971931 grimoirelab_panels-1.0.0/panels/json/gitlab_merge_requests.json
--rw-r--r--   0        0        0    19767 2024-04-13 07:20:59.971931 grimoirelab_panels-1.0.0/panels/json/gitlab_merge_requests_backlog.json
--rw-r--r--   0        0        0    10064 2024-04-13 07:20:59.971931 grimoirelab_panels-1.0.0/panels/json/gitlab_merge_requests_efficiency.json
--rw-r--r--   0        0        0    29536 2024-04-13 07:20:59.971931 grimoirelab_panels-1.0.0/panels/json/gitlab_merge_requests_timing.json
--rw-r--r--   0        0        0     7574 2024-04-13 07:20:59.971931 grimoirelab_panels-1.0.0/panels/json/gitter-index-pattern.json
--rw-r--r--   0        0        0    19582 2024-04-13 07:20:59.971931 grimoirelab_panels-1.0.0/panels/json/gitter.json
--rw-r--r--   0        0        0     3542 2024-04-13 07:20:59.971931 grimoirelab_panels-1.0.0/panels/json/google-hits-index-pattern.json
--rw-r--r--   0        0        0     9632 2024-04-13 07:20:59.971931 grimoirelab_panels-1.0.0/panels/json/google-hits.json
--rw-r--r--   0        0        0     6558 2024-04-13 07:20:59.971931 grimoirelab_panels-1.0.0/panels/json/irc-index-pattern.json
--rw-r--r--   0        0        0    17705 2024-04-13 07:20:59.971931 grimoirelab_panels-1.0.0/panels/json/irc.json
--rw-r--r--   0        0        0     6167 2024-04-13 07:20:59.971931 grimoirelab_panels-1.0.0/panels/json/jenkins-index-pattern.json
--rw-r--r--   0        0        0    13189 2024-04-13 07:20:59.971931 grimoirelab_panels-1.0.0/panels/json/jenkins.json
--rw-r--r--   0        0        0     2746 2024-04-13 07:20:59.971931 grimoirelab_panels-1.0.0/panels/json/jenkins_export.json
--rw-r--r--   0        0        0    16882 2024-04-13 07:20:59.971931 grimoirelab_panels-1.0.0/panels/json/jenkins_job_categories.json
--rw-r--r--   0        0        0    15146 2024-04-13 07:20:59.971931 grimoirelab_panels-1.0.0/panels/json/jenkins_jobs.json
--rw-r--r--   0        0        0    15317 2024-04-13 07:20:59.971931 grimoirelab_panels-1.0.0/panels/json/jenkins_nodes.json
--rw-r--r--   0        0        0    20804 2024-04-13 07:20:59.971931 grimoirelab_panels-1.0.0/panels/json/jira-index-pattern.json
--rw-r--r--   0        0        0    19907 2024-04-13 07:20:59.971931 grimoirelab_panels-1.0.0/panels/json/jira.json
--rw-r--r--   0        0        0    19425 2024-04-13 07:20:59.971931 grimoirelab_panels-1.0.0/panels/json/jira_backlog.json
--rw-r--r--   0        0        0    24630 2024-04-13 07:20:59.971931 grimoirelab_panels-1.0.0/panels/json/jira_effort.json
--rw-r--r--   0        0        0    19082 2024-04-13 07:20:59.971931 grimoirelab_panels-1.0.0/panels/json/jira_resolution_date-index-pattern.json
--rw-r--r--   0        0        0    28482 2024-04-13 07:20:59.971931 grimoirelab_panels-1.0.0/panels/json/jira_timing.json
--rw-r--r--   0        0        0     9950 2024-04-13 07:20:59.971931 grimoirelab_panels-1.0.0/panels/json/kafka-index-pattern.json
--rw-r--r--   0        0        0    14107 2024-04-13 07:20:59.971931 grimoirelab_panels-1.0.0/panels/json/kip.json
--rw-r--r--   0        0        0     8116 2024-04-13 07:20:59.971931 grimoirelab_panels-1.0.0/panels/json/lifecycle.json
--rw-r--r--   0        0        0    14332 2024-04-13 07:20:59.971931 grimoirelab_panels-1.0.0/panels/json/mailinglists.json
--rw-r--r--   0        0        0    13603 2024-04-13 07:20:59.971931 grimoirelab_panels-1.0.0/panels/json/maniphest-index-pattern.json
--rw-r--r--   0        0        0    16790 2024-04-13 07:20:59.971931 grimoirelab_panels-1.0.0/panels/json/maniphest.json
--rw-r--r--   0        0        0    17533 2024-04-13 07:20:59.971931 grimoirelab_panels-1.0.0/panels/json/maniphest_backlog.json
--rw-r--r--   0        0        0    27034 2024-04-13 07:20:59.971931 grimoirelab_panels-1.0.0/panels/json/maniphest_timing.json
--rw-r--r--   0        0        0    11840 2024-04-13 07:20:59.971931 grimoirelab_panels-1.0.0/panels/json/mattermost-index-pattern.json
--rw-r--r--   0        0        0    21734 2024-04-13 07:20:59.971931 grimoirelab_panels-1.0.0/panels/json/mattermost.json
--rw-r--r--   0        0        0     7114 2024-04-13 07:20:59.971931 grimoirelab_panels-1.0.0/panels/json/mbox-index-pattern.json
--rw-r--r--   0        0        0     7005 2024-04-13 07:20:59.971931 grimoirelab_panels-1.0.0/panels/json/mediawiki-index-pattern.json
--rw-r--r--   0        0        0    18868 2024-04-13 07:20:59.971931 grimoirelab_panels-1.0.0/panels/json/mediawiki.json
--rw-r--r--   0        0        0    13488 2024-04-13 07:20:59.971931 grimoirelab_panels-1.0.0/panels/json/meetup-index-pattern.json
--rw-r--r--   0        0        0    20703 2024-04-13 07:20:59.971931 grimoirelab_panels-1.0.0/panels/json/meetup.json
--rw-r--r--   0        0        0    10948 2024-04-13 07:20:59.971931 grimoirelab_panels-1.0.0/panels/json/meetup_locations.json
--rw-r--r--   0        0        0     8367 2024-04-13 07:20:59.971931 grimoirelab_panels-1.0.0/panels/json/mozilla_club-index-pattern.json
--rw-r--r--   0        0        0    17732 2024-04-13 07:20:59.971931 grimoirelab_panels-1.0.0/panels/json/mozilla_club.json
--rw-r--r--   0        0        0    15146 2024-04-13 07:20:59.971931 grimoirelab_panels-1.0.0/panels/json/onion_organizations.json
--rw-r--r--   0        0        0    12407 2024-04-13 07:20:59.971931 grimoirelab_panels-1.0.0/panels/json/onion_overall.json
--rw-r--r--   0        0        0    14969 2024-04-13 07:20:59.971931 grimoirelab_panels-1.0.0/panels/json/onion_projects.json
--rw-r--r--   0        0        0    46107 2024-04-13 07:20:59.971931 grimoirelab_panels-1.0.0/panels/json/organization_tracking_overview.json
--rw-r--r--   0        0        0    11610 2024-04-13 07:20:59.971931 grimoirelab_panels-1.0.0/panels/json/organizational_diversity.json
--rw-r--r--   0        0        0    11569 2024-04-13 07:20:59.971931 grimoirelab_panels-1.0.0/panels/json/organizational_diversity_by_domains.json
--rw-r--r--   0        0        0   165494 2024-04-13 07:20:59.971931 grimoirelab_panels-1.0.0/panels/json/overview.json
--rw-r--r--   0        0        0    10602 2024-04-13 07:20:59.971931 grimoirelab_panels-1.0.0/panels/json/redmine-index-pattern.json
--rw-r--r--   0        0        0    18860 2024-04-13 07:20:59.971931 grimoirelab_panels-1.0.0/panels/json/redmine.json
--rw-r--r--   0        0        0    17155 2024-04-13 07:20:59.971931 grimoirelab_panels-1.0.0/panels/json/redmine_backlog.json
--rw-r--r--   0        0        0    27521 2024-04-13 07:20:59.971931 grimoirelab_panels-1.0.0/panels/json/redmine_timing.json
--rw-r--r--   0        0        0     7975 2024-04-13 07:20:59.971931 grimoirelab_panels-1.0.0/panels/json/remo-activities-index-pattern.json
--rw-r--r--   0        0        0     7751 2024-04-13 07:20:59.971931 grimoirelab_panels-1.0.0/panels/json/remo-activities_metadata__timestamp-index-pattern.json
--rw-r--r--   0        0        0     8502 2024-04-13 07:20:59.971931 grimoirelab_panels-1.0.0/panels/json/remo-events-index-pattern.json
--rw-r--r--   0        0        0     8167 2024-04-13 07:20:59.971931 grimoirelab_panels-1.0.0/panels/json/remo-events_metadata__timestamp-index-pattern.json
--rw-r--r--   0        0        0    24655 2024-04-13 07:20:59.971931 grimoirelab_panels-1.0.0/panels/json/reps_activities.json
--rw-r--r--   0        0        0    21751 2024-04-13 07:20:59.975931 grimoirelab_panels-1.0.0/panels/json/reps_events.json
--rw-r--r--   0        0        0     5345 2024-04-13 07:20:59.975931 grimoirelab_panels-1.0.0/panels/json/rss-index-pattern.json
--rw-r--r--   0        0        0    14709 2024-04-13 07:20:59.975931 grimoirelab_panels-1.0.0/panels/json/rss.json
--rw-r--r--   0        0        0    10977 2024-04-13 07:20:59.975931 grimoirelab_panels-1.0.0/panels/json/slack-index-pattern.json
--rw-r--r--   0        0        0    21493 2024-04-13 07:20:59.975931 grimoirelab_panels-1.0.0/panels/json/slack.json
--rw-r--r--   0        0        0    17191 2024-04-13 07:20:59.975931 grimoirelab_panels-1.0.0/panels/json/slack_devrel.json
--rw-r--r--   0        0        0    10161 2024-04-13 07:20:59.975931 grimoirelab_panels-1.0.0/panels/json/stackoverflow-index-pattern.json
--rw-r--r--   0        0        0    27607 2024-04-13 07:20:59.975931 grimoirelab_panels-1.0.0/panels/json/stackoverflow.json
--rw-r--r--   0        0        0     4985 2024-04-13 07:20:59.975931 grimoirelab_panels-1.0.0/panels/json/telegram-index-pattern.json
--rw-r--r--   0        0        0    10920 2024-04-13 07:20:59.975931 grimoirelab_panels-1.0.0/panels/json/telegram.json
--rw-r--r--   0        0        0    13711 2024-04-13 07:20:59.975931 grimoirelab_panels-1.0.0/panels/json/testing_all.json
--rw-r--r--   0        0        0    16900 2024-04-13 07:20:59.975931 grimoirelab_panels-1.0.0/panels/json/testing_functest.json
--rw-r--r--   0        0        0    16961 2024-04-13 07:20:59.975931 grimoirelab_panels-1.0.0/panels/json/timing_overview_tickets.json
--rw-r--r--   0        0        0    10741 2024-04-13 07:20:59.975931 grimoirelab_panels-1.0.0/panels/json/twitter-index-pattern.json
--rw-r--r--   0        0        0    18301 2024-04-13 07:20:59.975931 grimoirelab_panels-1.0.0/panels/json/twitter.json
--rw-r--r--   0        0        0    12282 2024-04-13 07:20:59.975931 grimoirelab_panels-1.0.0/panels/json/weblate-index-pattern.json
--rw-r--r--   0        0        0    23008 2024-04-13 07:20:59.975931 grimoirelab_panels-1.0.0/panels/json/weblate_demographics.json
--rw-r--r--   0        0        0    18934 2024-04-13 07:20:59.975931 grimoirelab_panels-1.0.0/panels/json/weblate_overview.json
--rw-r--r--   0        0        0     1132 2024-04-13 07:20:59.975931 grimoirelab_panels-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     7502 1970-01-01 00:00:00.000000 grimoirelab_panels-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      381 2024-04-09 16:06:27.318267 grimoirelab_panels-1.0.0rc1/AUTHORS
+-rw-r--r--   0        0        0    35147 2024-04-09 16:06:27.318267 grimoirelab_panels-1.0.0rc1/LICENSE
+-rw-r--r--   0        0        0      709 2024-04-09 16:06:27.318267 grimoirelab_panels-1.0.0rc1/NEWS
+-rw-r--r--   0        0        0     6549 2024-04-09 16:06:27.318267 grimoirelab_panels-1.0.0rc1/README.md
+-rw-r--r--   0        0        0        0 2024-04-09 16:06:27.458266 grimoirelab_panels-1.0.0rc1/panels/__init__.py
+-rw-r--r--   0        0        0       91 2024-04-09 16:06:27.458266 grimoirelab_panels-1.0.0rc1/panels/_version.py
+-rw-r--r--   0        0        0     7506 2024-04-09 16:06:27.458266 grimoirelab_panels-1.0.0rc1/panels/json/about.json
+-rw-r--r--   0        0        0    92381 2024-04-09 16:06:27.458266 grimoirelab_panels-1.0.0rc1/panels/json/affiliations-index-pattern.json
+-rw-r--r--   0        0        0    14883 2024-04-09 16:06:27.458266 grimoirelab_panels-1.0.0rc1/panels/json/affiliations.json
+-rw-r--r--   0        0        0    56854 2024-04-09 16:06:27.458266 grimoirelab_panels-1.0.0rc1/panels/json/all_enriched-index-pattern.json
+-rw-r--r--   0        0        0    15123 2024-04-09 16:06:27.458266 grimoirelab_panels-1.0.0rc1/panels/json/all_enriched_tickets-index-pattern.json
+-rw-r--r--   0        0        0     3517 2024-04-09 16:06:27.458266 grimoirelab_panels-1.0.0rc1/panels/json/all_onion-index-pattern.json
+-rw-r--r--   0        0        0     3157 2024-04-09 16:06:27.458266 grimoirelab_panels-1.0.0rc1/panels/json/apache-index-pattern.json
+-rw-r--r--   0        0        0    14699 2024-04-09 16:06:27.458266 grimoirelab_panels-1.0.0rc1/panels/json/apache.json
+-rw-r--r--   0        0        0     8849 2024-04-09 16:06:27.458266 grimoirelab_panels-1.0.0rc1/panels/json/askbot-index-pattern.json
+-rw-r--r--   0        0        0    28220 2024-04-09 16:06:27.462266 grimoirelab_panels-1.0.0rc1/panels/json/askbot.json
+-rw-r--r--   0        0        0    29699 2024-04-09 16:06:27.462266 grimoirelab_panels-1.0.0rc1/panels/json/attracted-contributors.json
+-rw-r--r--   0        0        0    19600 2024-04-09 16:06:27.462266 grimoirelab_panels-1.0.0rc1/panels/json/bugzilla-index-pattern.json
+-rw-r--r--   0        0        0    16078 2024-04-09 16:06:27.462266 grimoirelab_panels-1.0.0rc1/panels/json/bugzilla.json
+-rw-r--r--   0        0        0    16857 2024-04-09 16:06:27.462266 grimoirelab_panels-1.0.0rc1/panels/json/bugzilla_backlog.json
+-rw-r--r--   0        0        0    29242 2024-04-09 16:06:27.462266 grimoirelab_panels-1.0.0rc1/panels/json/bugzilla_timing.json
+-rw-r--r--   0        0        0     5836 2024-04-09 16:06:27.462266 grimoirelab_panels-1.0.0rc1/panels/json/cocom-index-pattern.json
+-rw-r--r--   0        0        0    23781 2024-04-09 16:06:27.462266 grimoirelab_panels-1.0.0rc1/panels/json/cocom.json
+-rw-r--r--   0        0        0     3711 2024-04-09 16:06:27.462266 grimoirelab_panels-1.0.0rc1/panels/json/cocom_study-index-pattern.json
+-rw-r--r--   0        0        0     5413 2024-04-09 16:06:27.462266 grimoirelab_panels-1.0.0rc1/panels/json/colic-index-pattern.json
+-rw-r--r--   0        0        0    23795 2024-04-09 16:06:27.462266 grimoirelab_panels-1.0.0rc1/panels/json/colic.json
+-rw-r--r--   0        0        0     2656 2024-04-09 16:06:27.462266 grimoirelab_panels-1.0.0rc1/panels/json/colic_study-index-pattern.json
+-rw-r--r--   0        0        0     7887 2024-04-09 16:06:27.462266 grimoirelab_panels-1.0.0rc1/panels/json/confluence-index-pattern.json
+-rw-r--r--   0        0        0    16237 2024-04-09 16:06:27.462266 grimoirelab_panels-1.0.0rc1/panels/json/confluence.json
+-rw-r--r--   0        0        0    10565 2024-04-09 16:06:27.462266 grimoirelab_panels-1.0.0rc1/panels/json/contributors_growth.json
+-rw-r--r--   0        0        0    62471 2024-04-09 16:06:27.462266 grimoirelab_panels-1.0.0rc1/panels/json/data_status.json
+-rw-r--r--   0        0        0    16442 2024-04-09 16:06:27.462266 grimoirelab_panels-1.0.0rc1/panels/json/demographics-index-pattern.json
+-rw-r--r--   0        0        0    22408 2024-04-09 16:06:27.462266 grimoirelab_panels-1.0.0rc1/panels/json/demographics.json
+-rw-r--r--   0        0        0    22967 2024-04-09 16:06:27.462266 grimoirelab_panels-1.0.0rc1/panels/json/demographics_contribution-index-pattern.json
+-rw-r--r--   0        0        0     9092 2024-04-09 16:06:27.462266 grimoirelab_panels-1.0.0rc1/panels/json/discourse-index-pattern.json
+-rw-r--r--   0        0        0    26733 2024-04-09 16:06:27.462266 grimoirelab_panels-1.0.0rc1/panels/json/discourse.json
+-rw-r--r--   0        0        0     6199 2024-04-09 16:06:27.462266 grimoirelab_panels-1.0.0rc1/panels/json/discourse_devrel.json
+-rw-r--r--   0        0        0    17850 2024-04-09 16:06:27.462266 grimoirelab_panels-1.0.0rc1/panels/json/docker.json
+-rw-r--r--   0        0        0     3136 2024-04-09 16:06:27.462266 grimoirelab_panels-1.0.0rc1/panels/json/docker_deps-index-pattern.json
+-rw-r--r--   0        0        0     3427 2024-04-09 16:06:27.462266 grimoirelab_panels-1.0.0rc1/panels/json/docker_smells-index-pattern.json
+-rw-r--r--   0        0        0     4642 2024-04-09 16:06:27.462266 grimoirelab_panels-1.0.0rc1/panels/json/dockerhub-index-pattern.json
+-rw-r--r--   0        0        0     8082 2024-04-09 16:06:27.462266 grimoirelab_panels-1.0.0rc1/panels/json/dockerhub.json
+-rw-r--r--   0        0        0     9208 2024-04-09 16:06:27.462266 grimoirelab_panels-1.0.0rc1/panels/json/emtech/adoption/crates-emergintech-index-pattern.json
+-rw-r--r--   0        0        0    12721 2024-04-09 16:06:27.462266 grimoirelab_panels-1.0.0rc1/panels/json/emtech/adoption/emerging_tech_adoption.json
+-rw-r--r--   0        0        0     7374 2024-04-09 16:06:27.462266 grimoirelab_panels-1.0.0rc1/panels/json/emtech/adoption/emerging_tech_adoption_no_crates.json
+-rw-r--r--   0        0        0    11551 2024-04-09 16:06:27.462266 grimoirelab_panels-1.0.0rc1/panels/json/emtech/adoption/github_issues-index-pattern.json
+-rw-r--r--   0        0        0    49294 2024-04-09 16:06:27.462266 grimoirelab_panels-1.0.0rc1/panels/json/emtech/dev/emerging_tech_dev.json
+-rw-r--r--   0        0        0    11652 2024-04-09 16:06:27.462266 grimoirelab_panels-1.0.0rc1/panels/json/emtech/dev/git-emergingtech-index-pattern.json
+-rw-r--r--   0        0        0     6424 2024-04-09 16:06:27.462266 grimoirelab_panels-1.0.0rc1/panels/json/emtech/dev/git_areas_of_code-index-pattern.json
+-rw-r--r--   0        0        0    11840 2024-04-09 16:06:27.462266 grimoirelab_panels-1.0.0rc1/panels/json/emtech/dev/github-emergingtech-index-pattern.json
+-rw-r--r--   0        0        0    37258 2024-04-09 16:06:27.462266 grimoirelab_panels-1.0.0rc1/panels/json/emtech/social/emerging_tech_social.json
+-rw-r--r--   0        0        0     6333 2024-04-09 16:06:27.462266 grimoirelab_panels-1.0.0rc1/panels/json/emtech/social/irc-emergingtech-index-pattern.json
+-rw-r--r--   0        0        0    12257 2024-04-09 16:06:27.462266 grimoirelab_panels-1.0.0rc1/panels/json/emtech/social/meetup-emergingtech-index-pattern.json
+-rw-r--r--   0        0        0    11496 2024-04-09 16:06:27.462266 grimoirelab_panels-1.0.0rc1/panels/json/emtech/social/slack-emergingtech-index-pattern.json
+-rw-r--r--   0        0        0    10218 2024-04-09 16:06:27.462266 grimoirelab_panels-1.0.0rc1/panels/json/emtech/social/stackoverflow-emergingtech-index-pattern.json
+-rw-r--r--   0        0        0    10286 2024-04-09 16:06:27.462266 grimoirelab_panels-1.0.0rc1/panels/json/emtech/social/twitter_emergingtech-index-pattern.json
+-rw-r--r--   0        0        0    10779 2024-04-09 16:06:27.462266 grimoirelab_panels-1.0.0rc1/panels/json/engagement_by_contributions.json
+-rw-r--r--   0        0        0     4856 2024-04-09 16:06:27.462266 grimoirelab_panels-1.0.0rc1/panels/json/functest-index-pattern.json
+-rw-r--r--   0        0        0    22360 2024-04-09 16:06:27.462266 grimoirelab_panels-1.0.0rc1/panels/json/gerrit-index-pattern.json
+-rw-r--r--   0        0        0    21175 2024-04-09 16:06:27.462266 grimoirelab_panels-1.0.0rc1/panels/json/gerrit.json
+-rw-r--r--   0        0        0    20808 2024-04-09 16:06:27.462266 grimoirelab_panels-1.0.0rc1/panels/json/gerrit_approvals.json
+-rw-r--r--   0        0        0    18636 2024-04-09 16:06:27.462266 grimoirelab_panels-1.0.0rc1/panels/json/gerrit_backlog.json
+-rw-r--r--   0        0        0    10022 2024-04-09 16:06:27.462266 grimoirelab_panels-1.0.0rc1/panels/json/gerrit_efficiency.json
+-rw-r--r--   0        0        0    25489 2024-04-09 16:06:27.462266 grimoirelab_panels-1.0.0rc1/panels/json/gerrit_retention_newcomers.json
+-rw-r--r--   0        0        0    17434 2024-04-09 16:06:27.462266 grimoirelab_panels-1.0.0rc1/panels/json/gerrit_timing.json
+-rw-r--r--   0        0        0    26898 2024-04-09 16:06:27.462266 grimoirelab_panels-1.0.0rc1/panels/json/git-index-pattern.json
+-rw-r--r--   0        0        0    19030 2024-04-09 16:06:27.466266 grimoirelab_panels-1.0.0rc1/panels/json/git.json
+-rw-r--r--   0        0        0     7040 2024-04-09 16:06:27.466266 grimoirelab_panels-1.0.0rc1/panels/json/git_areas_of_code-index-pattern.json
+-rw-r--r--   0        0        0    20965 2024-04-09 16:06:27.466266 grimoirelab_panels-1.0.0rc1/panels/json/git_areas_of_code.json
+-rw-r--r--   0        0        0    23802 2024-04-09 16:06:27.466266 grimoirelab_panels-1.0.0rc1/panels/json/git_demographics.json
+-rw-r--r--   0        0        0    19262 2024-04-09 16:06:27.466266 grimoirelab_panels-1.0.0rc1/panels/json/git_pair_programming.json
+-rw-r--r--   0        0        0    19173 2024-04-09 16:06:27.466266 grimoirelab_panels-1.0.0rc1/panels/json/github2_issues-index-pattern.json
+-rw-r--r--   0        0        0    20757 2024-04-09 16:06:27.466266 grimoirelab_panels-1.0.0rc1/panels/json/github2_issues_comments_and_collaboration.json
+-rw-r--r--   0        0        0    32469 2024-04-09 16:06:27.466266 grimoirelab_panels-1.0.0rc1/panels/json/github2_issues_comments_feelings.json
+-rw-r--r--   0        0        0    21762 2024-04-09 16:06:27.466266 grimoirelab_panels-1.0.0rc1/panels/json/github2_pull_requests-index-pattern.json
+-rw-r--r--   0        0        0    21093 2024-04-09 16:06:27.466266 grimoirelab_panels-1.0.0rc1/panels/json/github2_pull_requests_comments_and_collaboration.json
+-rw-r--r--   0        0        0    15171 2024-04-09 16:06:27.466266 grimoirelab_panels-1.0.0rc1/panels/json/github_devrel.json
+-rw-r--r--   0        0        0    21142 2024-04-09 16:06:27.466266 grimoirelab_panels-1.0.0rc1/panels/json/github_events-index-pattern.json
+-rw-r--r--   0        0        0    18416 2024-04-09 16:06:27.466266 grimoirelab_panels-1.0.0rc1/panels/json/github_events_closed.json
+-rw-r--r--   0        0        0    31092 2024-04-09 16:06:27.466266 grimoirelab_panels-1.0.0rc1/panels/json/github_events_labels.json
+-rw-r--r--   0        0        0    18716 2024-04-09 16:06:27.466266 grimoirelab_panels-1.0.0rc1/panels/json/github_issues-index-pattern.json
+-rw-r--r--   0        0        0    17412 2024-04-09 16:06:27.466266 grimoirelab_panels-1.0.0rc1/panels/json/github_issues.json
+-rw-r--r--   0        0        0    17482 2024-04-09 16:06:27.466266 grimoirelab_panels-1.0.0rc1/panels/json/github_issues_backlog.json
+-rw-r--r--   0        0        0    11033 2024-04-09 16:06:27.466266 grimoirelab_panels-1.0.0rc1/panels/json/github_issues_efficiency.json
+-rw-r--r--   0        0        0    26375 2024-04-09 16:06:27.466266 grimoirelab_panels-1.0.0rc1/panels/json/github_issues_timing.json
+-rw-r--r--   0        0        0    17034 2024-04-09 16:06:27.466266 grimoirelab_panels-1.0.0rc1/panels/json/github_pull_requests.json
+-rw-r--r--   0        0        0    18852 2024-04-09 16:06:27.466266 grimoirelab_panels-1.0.0rc1/panels/json/github_pull_requests_backlog.json
+-rw-r--r--   0        0        0    11156 2024-04-09 16:06:27.466266 grimoirelab_panels-1.0.0rc1/panels/json/github_pull_requests_efficiency.json
+-rw-r--r--   0        0        0    26979 2024-04-09 16:06:27.466266 grimoirelab_panels-1.0.0rc1/panels/json/github_pull_requests_timing.json
+-rw-r--r--   0        0        0     4619 2024-04-09 16:06:27.466266 grimoirelab_panels-1.0.0rc1/panels/json/github_repositories-index-pattern.json
+-rw-r--r--   0        0        0    16044 2024-04-09 16:06:27.466266 grimoirelab_panels-1.0.0rc1/panels/json/github_repositories.json
+-rw-r--r--   0        0        0    10656 2024-04-09 16:06:27.466266 grimoirelab_panels-1.0.0rc1/panels/json/gitlab_issues-index-pattern.json
+-rw-r--r--   0        0        0    20483 2024-04-09 16:06:27.466266 grimoirelab_panels-1.0.0rc1/panels/json/gitlab_issues.json
+-rw-r--r--   0        0        0    19812 2024-04-09 16:06:27.466266 grimoirelab_panels-1.0.0rc1/panels/json/gitlab_issues_backlog.json
+-rw-r--r--   0        0        0     9623 2024-04-09 16:06:27.466266 grimoirelab_panels-1.0.0rc1/panels/json/gitlab_issues_efficiency.json
+-rw-r--r--   0        0        0    26291 2024-04-09 16:06:27.466266 grimoirelab_panels-1.0.0rc1/panels/json/gitlab_issues_timing.json
+-rw-r--r--   0        0        0    10574 2024-04-09 16:06:27.466266 grimoirelab_panels-1.0.0rc1/panels/json/gitlab_merge_requests-index-pattern.json
+-rw-r--r--   0        0        0    20199 2024-04-09 16:06:27.466266 grimoirelab_panels-1.0.0rc1/panels/json/gitlab_merge_requests.json
+-rw-r--r--   0        0        0    19767 2024-04-09 16:06:27.466266 grimoirelab_panels-1.0.0rc1/panels/json/gitlab_merge_requests_backlog.json
+-rw-r--r--   0        0        0    10064 2024-04-09 16:06:27.466266 grimoirelab_panels-1.0.0rc1/panels/json/gitlab_merge_requests_efficiency.json
+-rw-r--r--   0        0        0    29536 2024-04-09 16:06:27.466266 grimoirelab_panels-1.0.0rc1/panels/json/gitlab_merge_requests_timing.json
+-rw-r--r--   0        0        0     7574 2024-04-09 16:06:27.466266 grimoirelab_panels-1.0.0rc1/panels/json/gitter-index-pattern.json
+-rw-r--r--   0        0        0    19582 2024-04-09 16:06:27.466266 grimoirelab_panels-1.0.0rc1/panels/json/gitter.json
+-rw-r--r--   0        0        0     3542 2024-04-09 16:06:27.466266 grimoirelab_panels-1.0.0rc1/panels/json/google-hits-index-pattern.json
+-rw-r--r--   0        0        0     9632 2024-04-09 16:06:27.466266 grimoirelab_panels-1.0.0rc1/panels/json/google-hits.json
+-rw-r--r--   0        0        0     6558 2024-04-09 16:06:27.466266 grimoirelab_panels-1.0.0rc1/panels/json/irc-index-pattern.json
+-rw-r--r--   0        0        0    17705 2024-04-09 16:06:27.466266 grimoirelab_panels-1.0.0rc1/panels/json/irc.json
+-rw-r--r--   0        0        0     6167 2024-04-09 16:06:27.466266 grimoirelab_panels-1.0.0rc1/panels/json/jenkins-index-pattern.json
+-rw-r--r--   0        0        0    13189 2024-04-09 16:06:27.466266 grimoirelab_panels-1.0.0rc1/panels/json/jenkins.json
+-rw-r--r--   0        0        0     2746 2024-04-09 16:06:27.466266 grimoirelab_panels-1.0.0rc1/panels/json/jenkins_export.json
+-rw-r--r--   0        0        0    16882 2024-04-09 16:06:27.466266 grimoirelab_panels-1.0.0rc1/panels/json/jenkins_job_categories.json
+-rw-r--r--   0        0        0    15146 2024-04-09 16:06:27.466266 grimoirelab_panels-1.0.0rc1/panels/json/jenkins_jobs.json
+-rw-r--r--   0        0        0    15317 2024-04-09 16:06:27.466266 grimoirelab_panels-1.0.0rc1/panels/json/jenkins_nodes.json
+-rw-r--r--   0        0        0    20804 2024-04-09 16:06:27.466266 grimoirelab_panels-1.0.0rc1/panels/json/jira-index-pattern.json
+-rw-r--r--   0        0        0    19907 2024-04-09 16:06:27.466266 grimoirelab_panels-1.0.0rc1/panels/json/jira.json
+-rw-r--r--   0        0        0    19425 2024-04-09 16:06:27.466266 grimoirelab_panels-1.0.0rc1/panels/json/jira_backlog.json
+-rw-r--r--   0        0        0    24630 2024-04-09 16:06:27.466266 grimoirelab_panels-1.0.0rc1/panels/json/jira_effort.json
+-rw-r--r--   0        0        0    19082 2024-04-09 16:06:27.466266 grimoirelab_panels-1.0.0rc1/panels/json/jira_resolution_date-index-pattern.json
+-rw-r--r--   0        0        0    28482 2024-04-09 16:06:27.466266 grimoirelab_panels-1.0.0rc1/panels/json/jira_timing.json
+-rw-r--r--   0        0        0     9950 2024-04-09 16:06:27.466266 grimoirelab_panels-1.0.0rc1/panels/json/kafka-index-pattern.json
+-rw-r--r--   0        0        0    14107 2024-04-09 16:06:27.466266 grimoirelab_panels-1.0.0rc1/panels/json/kip.json
+-rw-r--r--   0        0        0     8116 2024-04-09 16:06:27.466266 grimoirelab_panels-1.0.0rc1/panels/json/lifecycle.json
+-rw-r--r--   0        0        0    14332 2024-04-09 16:06:27.470266 grimoirelab_panels-1.0.0rc1/panels/json/mailinglists.json
+-rw-r--r--   0        0        0    13603 2024-04-09 16:06:27.470266 grimoirelab_panels-1.0.0rc1/panels/json/maniphest-index-pattern.json
+-rw-r--r--   0        0        0    16790 2024-04-09 16:06:27.470266 grimoirelab_panels-1.0.0rc1/panels/json/maniphest.json
+-rw-r--r--   0        0        0    17533 2024-04-09 16:06:27.470266 grimoirelab_panels-1.0.0rc1/panels/json/maniphest_backlog.json
+-rw-r--r--   0        0        0    27034 2024-04-09 16:06:27.470266 grimoirelab_panels-1.0.0rc1/panels/json/maniphest_timing.json
+-rw-r--r--   0        0        0    11840 2024-04-09 16:06:27.470266 grimoirelab_panels-1.0.0rc1/panels/json/mattermost-index-pattern.json
+-rw-r--r--   0        0        0    21734 2024-04-09 16:06:27.470266 grimoirelab_panels-1.0.0rc1/panels/json/mattermost.json
+-rw-r--r--   0        0        0     7114 2024-04-09 16:06:27.470266 grimoirelab_panels-1.0.0rc1/panels/json/mbox-index-pattern.json
+-rw-r--r--   0        0        0     7005 2024-04-09 16:06:27.470266 grimoirelab_panels-1.0.0rc1/panels/json/mediawiki-index-pattern.json
+-rw-r--r--   0        0        0    18868 2024-04-09 16:06:27.470266 grimoirelab_panels-1.0.0rc1/panels/json/mediawiki.json
+-rw-r--r--   0        0        0    13488 2024-04-09 16:06:27.470266 grimoirelab_panels-1.0.0rc1/panels/json/meetup-index-pattern.json
+-rw-r--r--   0        0        0    20703 2024-04-09 16:06:27.470266 grimoirelab_panels-1.0.0rc1/panels/json/meetup.json
+-rw-r--r--   0        0        0    10948 2024-04-09 16:06:27.470266 grimoirelab_panels-1.0.0rc1/panels/json/meetup_locations.json
+-rw-r--r--   0        0        0     8367 2024-04-09 16:06:27.470266 grimoirelab_panels-1.0.0rc1/panels/json/mozilla_club-index-pattern.json
+-rw-r--r--   0        0        0    17732 2024-04-09 16:06:27.470266 grimoirelab_panels-1.0.0rc1/panels/json/mozilla_club.json
+-rw-r--r--   0        0        0    15146 2024-04-09 16:06:27.470266 grimoirelab_panels-1.0.0rc1/panels/json/onion_organizations.json
+-rw-r--r--   0        0        0    12407 2024-04-09 16:06:27.470266 grimoirelab_panels-1.0.0rc1/panels/json/onion_overall.json
+-rw-r--r--   0        0        0    14969 2024-04-09 16:06:27.470266 grimoirelab_panels-1.0.0rc1/panels/json/onion_projects.json
+-rw-r--r--   0        0        0    46107 2024-04-09 16:06:27.470266 grimoirelab_panels-1.0.0rc1/panels/json/organization_tracking_overview.json
+-rw-r--r--   0        0        0    11610 2024-04-09 16:06:27.470266 grimoirelab_panels-1.0.0rc1/panels/json/organizational_diversity.json
+-rw-r--r--   0        0        0    11569 2024-04-09 16:06:27.470266 grimoirelab_panels-1.0.0rc1/panels/json/organizational_diversity_by_domains.json
+-rw-r--r--   0        0        0   165494 2024-04-09 16:06:27.470266 grimoirelab_panels-1.0.0rc1/panels/json/overview.json
+-rw-r--r--   0        0        0    10602 2024-04-09 16:06:27.470266 grimoirelab_panels-1.0.0rc1/panels/json/redmine-index-pattern.json
+-rw-r--r--   0        0        0    18860 2024-04-09 16:06:27.470266 grimoirelab_panels-1.0.0rc1/panels/json/redmine.json
+-rw-r--r--   0        0        0    17155 2024-04-09 16:06:27.470266 grimoirelab_panels-1.0.0rc1/panels/json/redmine_backlog.json
+-rw-r--r--   0        0        0    27521 2024-04-09 16:06:27.470266 grimoirelab_panels-1.0.0rc1/panels/json/redmine_timing.json
+-rw-r--r--   0        0        0     7975 2024-04-09 16:06:27.470266 grimoirelab_panels-1.0.0rc1/panels/json/remo-activities-index-pattern.json
+-rw-r--r--   0        0        0     7751 2024-04-09 16:06:27.470266 grimoirelab_panels-1.0.0rc1/panels/json/remo-activities_metadata__timestamp-index-pattern.json
+-rw-r--r--   0        0        0     8502 2024-04-09 16:06:27.470266 grimoirelab_panels-1.0.0rc1/panels/json/remo-events-index-pattern.json
+-rw-r--r--   0        0        0     8167 2024-04-09 16:06:27.470266 grimoirelab_panels-1.0.0rc1/panels/json/remo-events_metadata__timestamp-index-pattern.json
+-rw-r--r--   0        0        0    24655 2024-04-09 16:06:27.470266 grimoirelab_panels-1.0.0rc1/panels/json/reps_activities.json
+-rw-r--r--   0        0        0    21751 2024-04-09 16:06:27.470266 grimoirelab_panels-1.0.0rc1/panels/json/reps_events.json
+-rw-r--r--   0        0        0     5345 2024-04-09 16:06:27.470266 grimoirelab_panels-1.0.0rc1/panels/json/rss-index-pattern.json
+-rw-r--r--   0        0        0    14709 2024-04-09 16:06:27.470266 grimoirelab_panels-1.0.0rc1/panels/json/rss.json
+-rw-r--r--   0        0        0    10977 2024-04-09 16:06:27.470266 grimoirelab_panels-1.0.0rc1/panels/json/slack-index-pattern.json
+-rw-r--r--   0        0        0    21493 2024-04-09 16:06:27.470266 grimoirelab_panels-1.0.0rc1/panels/json/slack.json
+-rw-r--r--   0        0        0    17191 2024-04-09 16:06:27.470266 grimoirelab_panels-1.0.0rc1/panels/json/slack_devrel.json
+-rw-r--r--   0        0        0    10161 2024-04-09 16:06:27.470266 grimoirelab_panels-1.0.0rc1/panels/json/stackoverflow-index-pattern.json
+-rw-r--r--   0        0        0    27607 2024-04-09 16:06:27.470266 grimoirelab_panels-1.0.0rc1/panels/json/stackoverflow.json
+-rw-r--r--   0        0        0     4985 2024-04-09 16:06:27.470266 grimoirelab_panels-1.0.0rc1/panels/json/telegram-index-pattern.json
+-rw-r--r--   0        0        0    10920 2024-04-09 16:06:27.470266 grimoirelab_panels-1.0.0rc1/panels/json/telegram.json
+-rw-r--r--   0        0        0    13711 2024-04-09 16:06:27.470266 grimoirelab_panels-1.0.0rc1/panels/json/testing_all.json
+-rw-r--r--   0        0        0    16900 2024-04-09 16:06:27.470266 grimoirelab_panels-1.0.0rc1/panels/json/testing_functest.json
+-rw-r--r--   0        0        0    16961 2024-04-09 16:06:27.470266 grimoirelab_panels-1.0.0rc1/panels/json/timing_overview_tickets.json
+-rw-r--r--   0        0        0    10741 2024-04-09 16:06:27.470266 grimoirelab_panels-1.0.0rc1/panels/json/twitter-index-pattern.json
+-rw-r--r--   0        0        0    18301 2024-04-09 16:06:27.470266 grimoirelab_panels-1.0.0rc1/panels/json/twitter.json
+-rw-r--r--   0        0        0    12282 2024-04-09 16:06:27.470266 grimoirelab_panels-1.0.0rc1/panels/json/weblate-index-pattern.json
+-rw-r--r--   0        0        0    23008 2024-04-09 16:06:27.470266 grimoirelab_panels-1.0.0rc1/panels/json/weblate_demographics.json
+-rw-r--r--   0        0        0    18934 2024-04-09 16:06:27.470266 grimoirelab_panels-1.0.0rc1/panels/json/weblate_overview.json
+-rw-r--r--   0        0        0     1137 2024-04-09 16:06:27.470266 grimoirelab_panels-1.0.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     7505 1970-01-01 00:00:00.000000 grimoirelab_panels-1.0.0rc1/PKG-INFO
```

### Comparing `grimoirelab_panels-1.0.0/LICENSE` & `grimoirelab_panels-1.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/NEWS` & `grimoirelab_panels-1.0.0rc1/NEWS`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,9 @@
 # Releases
 
-## grimoirelab-panels 1.0.0 - (2024-04-13)
-
-**New features:**
-
- * First major release\
-   GrimoireLab reached a stable status. This is our first major release.
-
-
 ## grimoirelab-panels 0.3.0 - (2023-10-20)
 
 **Feature removals:**
 
  * Drop Python 3.7 support\
    Python 3.7 reaches the end of life in June 2023. This means it won't
    receive new updates or patches to fix security issues. Therefore, this
```

### Comparing `grimoirelab_panels-1.0.0/README.md` & `grimoirelab_panels-1.0.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/about.json` & `grimoirelab_panels-1.0.0rc1/panels/json/about.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/affiliations-index-pattern.json` & `grimoirelab_panels-1.0.0rc1/panels/json/affiliations-index-pattern.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/affiliations.json` & `grimoirelab_panels-1.0.0rc1/panels/json/affiliations.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/all_enriched-index-pattern.json` & `grimoirelab_panels-1.0.0rc1/panels/json/all_enriched-index-pattern.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/all_enriched_tickets-index-pattern.json` & `grimoirelab_panels-1.0.0rc1/panels/json/all_enriched_tickets-index-pattern.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/all_onion-index-pattern.json` & `grimoirelab_panels-1.0.0rc1/panels/json/all_onion-index-pattern.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/apache-index-pattern.json` & `grimoirelab_panels-1.0.0rc1/panels/json/apache-index-pattern.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/apache.json` & `grimoirelab_panels-1.0.0rc1/panels/json/apache.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/askbot-index-pattern.json` & `grimoirelab_panels-1.0.0rc1/panels/json/askbot-index-pattern.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/askbot.json` & `grimoirelab_panels-1.0.0rc1/panels/json/askbot.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/attracted-contributors.json` & `grimoirelab_panels-1.0.0rc1/panels/json/attracted-contributors.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/bugzilla-index-pattern.json` & `grimoirelab_panels-1.0.0rc1/panels/json/bugzilla-index-pattern.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/bugzilla.json` & `grimoirelab_panels-1.0.0rc1/panels/json/bugzilla.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/bugzilla_backlog.json` & `grimoirelab_panels-1.0.0rc1/panels/json/bugzilla_backlog.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/bugzilla_timing.json` & `grimoirelab_panels-1.0.0rc1/panels/json/bugzilla_timing.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/cocom-index-pattern.json` & `grimoirelab_panels-1.0.0rc1/panels/json/cocom-index-pattern.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/cocom.json` & `grimoirelab_panels-1.0.0rc1/panels/json/cocom.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/cocom_study-index-pattern.json` & `grimoirelab_panels-1.0.0rc1/panels/json/cocom_study-index-pattern.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/colic-index-pattern.json` & `grimoirelab_panels-1.0.0rc1/panels/json/colic-index-pattern.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/colic.json` & `grimoirelab_panels-1.0.0rc1/panels/json/colic.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/colic_study-index-pattern.json` & `grimoirelab_panels-1.0.0rc1/panels/json/colic_study-index-pattern.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/confluence-index-pattern.json` & `grimoirelab_panels-1.0.0rc1/panels/json/confluence-index-pattern.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/confluence.json` & `grimoirelab_panels-1.0.0rc1/panels/json/confluence.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/contributors_growth.json` & `grimoirelab_panels-1.0.0rc1/panels/json/contributors_growth.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/data_status.json` & `grimoirelab_panels-1.0.0rc1/panels/json/data_status.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/demographics-index-pattern.json` & `grimoirelab_panels-1.0.0rc1/panels/json/demographics-index-pattern.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/demographics.json` & `grimoirelab_panels-1.0.0rc1/panels/json/demographics.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/demographics_contribution-index-pattern.json` & `grimoirelab_panels-1.0.0rc1/panels/json/demographics_contribution-index-pattern.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/discourse-index-pattern.json` & `grimoirelab_panels-1.0.0rc1/panels/json/discourse-index-pattern.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/discourse.json` & `grimoirelab_panels-1.0.0rc1/panels/json/discourse.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/discourse_devrel.json` & `grimoirelab_panels-1.0.0rc1/panels/json/discourse_devrel.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/docker.json` & `grimoirelab_panels-1.0.0rc1/panels/json/docker.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/docker_deps-index-pattern.json` & `grimoirelab_panels-1.0.0rc1/panels/json/docker_deps-index-pattern.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/docker_smells-index-pattern.json` & `grimoirelab_panels-1.0.0rc1/panels/json/docker_smells-index-pattern.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/dockerhub-index-pattern.json` & `grimoirelab_panels-1.0.0rc1/panels/json/dockerhub-index-pattern.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/dockerhub.json` & `grimoirelab_panels-1.0.0rc1/panels/json/dockerhub.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/emtech/adoption/crates-emergintech-index-pattern.json` & `grimoirelab_panels-1.0.0rc1/panels/json/emtech/adoption/crates-emergintech-index-pattern.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/emtech/adoption/emerging_tech_adoption.json` & `grimoirelab_panels-1.0.0rc1/panels/json/emtech/adoption/emerging_tech_adoption.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/emtech/adoption/emerging_tech_adoption_no_crates.json` & `grimoirelab_panels-1.0.0rc1/panels/json/emtech/adoption/emerging_tech_adoption_no_crates.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/emtech/adoption/github_issues-index-pattern.json` & `grimoirelab_panels-1.0.0rc1/panels/json/emtech/adoption/github_issues-index-pattern.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/emtech/dev/emerging_tech_dev.json` & `grimoirelab_panels-1.0.0rc1/panels/json/emtech/dev/emerging_tech_dev.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/emtech/dev/git-emergingtech-index-pattern.json` & `grimoirelab_panels-1.0.0rc1/panels/json/emtech/dev/git-emergingtech-index-pattern.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/emtech/dev/git_areas_of_code-index-pattern.json` & `grimoirelab_panels-1.0.0rc1/panels/json/emtech/dev/git_areas_of_code-index-pattern.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/emtech/dev/github-emergingtech-index-pattern.json` & `grimoirelab_panels-1.0.0rc1/panels/json/emtech/dev/github-emergingtech-index-pattern.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/emtech/social/emerging_tech_social.json` & `grimoirelab_panels-1.0.0rc1/panels/json/emtech/social/emerging_tech_social.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/emtech/social/irc-emergingtech-index-pattern.json` & `grimoirelab_panels-1.0.0rc1/panels/json/emtech/social/irc-emergingtech-index-pattern.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/emtech/social/meetup-emergingtech-index-pattern.json` & `grimoirelab_panels-1.0.0rc1/panels/json/emtech/social/meetup-emergingtech-index-pattern.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/emtech/social/slack-emergingtech-index-pattern.json` & `grimoirelab_panels-1.0.0rc1/panels/json/emtech/social/slack-emergingtech-index-pattern.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/emtech/social/stackoverflow-emergingtech-index-pattern.json` & `grimoirelab_panels-1.0.0rc1/panels/json/emtech/social/stackoverflow-emergingtech-index-pattern.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/emtech/social/twitter_emergingtech-index-pattern.json` & `grimoirelab_panels-1.0.0rc1/panels/json/emtech/social/twitter_emergingtech-index-pattern.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/engagement_by_contributions.json` & `grimoirelab_panels-1.0.0rc1/panels/json/engagement_by_contributions.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/functest-index-pattern.json` & `grimoirelab_panels-1.0.0rc1/panels/json/functest-index-pattern.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/gerrit-index-pattern.json` & `grimoirelab_panels-1.0.0rc1/panels/json/gerrit-index-pattern.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/gerrit.json` & `grimoirelab_panels-1.0.0rc1/panels/json/gerrit.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/gerrit_approvals.json` & `grimoirelab_panels-1.0.0rc1/panels/json/gerrit_approvals.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/gerrit_backlog.json` & `grimoirelab_panels-1.0.0rc1/panels/json/gerrit_backlog.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/gerrit_efficiency.json` & `grimoirelab_panels-1.0.0rc1/panels/json/gerrit_efficiency.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/gerrit_retention_newcomers.json` & `grimoirelab_panels-1.0.0rc1/panels/json/gerrit_retention_newcomers.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/gerrit_timing.json` & `grimoirelab_panels-1.0.0rc1/panels/json/gerrit_timing.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/git-index-pattern.json` & `grimoirelab_panels-1.0.0rc1/panels/json/git-index-pattern.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/git.json` & `grimoirelab_panels-1.0.0rc1/panels/json/git.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/git_areas_of_code-index-pattern.json` & `grimoirelab_panels-1.0.0rc1/panels/json/git_areas_of_code-index-pattern.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/git_areas_of_code.json` & `grimoirelab_panels-1.0.0rc1/panels/json/git_areas_of_code.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/git_demographics.json` & `grimoirelab_panels-1.0.0rc1/panels/json/git_demographics.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/git_pair_programming.json` & `grimoirelab_panels-1.0.0rc1/panels/json/git_pair_programming.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/github2_issues-index-pattern.json` & `grimoirelab_panels-1.0.0rc1/panels/json/github2_issues-index-pattern.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/github2_issues_comments_and_collaboration.json` & `grimoirelab_panels-1.0.0rc1/panels/json/github2_issues_comments_and_collaboration.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/github2_issues_comments_feelings.json` & `grimoirelab_panels-1.0.0rc1/panels/json/github2_issues_comments_feelings.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/github2_pull_requests-index-pattern.json` & `grimoirelab_panels-1.0.0rc1/panels/json/github2_pull_requests-index-pattern.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/github2_pull_requests_comments_and_collaboration.json` & `grimoirelab_panels-1.0.0rc1/panels/json/github2_pull_requests_comments_and_collaboration.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/github_devrel.json` & `grimoirelab_panels-1.0.0rc1/panels/json/github_devrel.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/github_events-index-pattern.json` & `grimoirelab_panels-1.0.0rc1/panels/json/github_events-index-pattern.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/github_events_closed.json` & `grimoirelab_panels-1.0.0rc1/panels/json/github_events_closed.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/github_events_labels.json` & `grimoirelab_panels-1.0.0rc1/panels/json/github_events_labels.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/github_issues-index-pattern.json` & `grimoirelab_panels-1.0.0rc1/panels/json/github_issues-index-pattern.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/github_issues.json` & `grimoirelab_panels-1.0.0rc1/panels/json/github_issues.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/github_issues_backlog.json` & `grimoirelab_panels-1.0.0rc1/panels/json/github_issues_backlog.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/github_issues_efficiency.json` & `grimoirelab_panels-1.0.0rc1/panels/json/github_issues_efficiency.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/github_issues_timing.json` & `grimoirelab_panels-1.0.0rc1/panels/json/github_issues_timing.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/github_pull_requests.json` & `grimoirelab_panels-1.0.0rc1/panels/json/github_pull_requests.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/github_pull_requests_backlog.json` & `grimoirelab_panels-1.0.0rc1/panels/json/github_pull_requests_backlog.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/github_pull_requests_efficiency.json` & `grimoirelab_panels-1.0.0rc1/panels/json/github_pull_requests_efficiency.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/github_pull_requests_timing.json` & `grimoirelab_panels-1.0.0rc1/panels/json/github_pull_requests_timing.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/github_repositories-index-pattern.json` & `grimoirelab_panels-1.0.0rc1/panels/json/github_repositories-index-pattern.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/github_repositories.json` & `grimoirelab_panels-1.0.0rc1/panels/json/github_repositories.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/gitlab_issues-index-pattern.json` & `grimoirelab_panels-1.0.0rc1/panels/json/gitlab_issues-index-pattern.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/gitlab_issues.json` & `grimoirelab_panels-1.0.0rc1/panels/json/gitlab_issues.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/gitlab_issues_backlog.json` & `grimoirelab_panels-1.0.0rc1/panels/json/gitlab_issues_backlog.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/gitlab_issues_efficiency.json` & `grimoirelab_panels-1.0.0rc1/panels/json/gitlab_issues_efficiency.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/gitlab_issues_timing.json` & `grimoirelab_panels-1.0.0rc1/panels/json/gitlab_issues_timing.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/gitlab_merge_requests-index-pattern.json` & `grimoirelab_panels-1.0.0rc1/panels/json/gitlab_merge_requests-index-pattern.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/gitlab_merge_requests.json` & `grimoirelab_panels-1.0.0rc1/panels/json/gitlab_merge_requests.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/gitlab_merge_requests_backlog.json` & `grimoirelab_panels-1.0.0rc1/panels/json/gitlab_merge_requests_backlog.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/gitlab_merge_requests_efficiency.json` & `grimoirelab_panels-1.0.0rc1/panels/json/gitlab_merge_requests_efficiency.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/gitlab_merge_requests_timing.json` & `grimoirelab_panels-1.0.0rc1/panels/json/gitlab_merge_requests_timing.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/gitter-index-pattern.json` & `grimoirelab_panels-1.0.0rc1/panels/json/gitter-index-pattern.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/gitter.json` & `grimoirelab_panels-1.0.0rc1/panels/json/gitter.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/google-hits-index-pattern.json` & `grimoirelab_panels-1.0.0rc1/panels/json/google-hits-index-pattern.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/google-hits.json` & `grimoirelab_panels-1.0.0rc1/panels/json/google-hits.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/irc-index-pattern.json` & `grimoirelab_panels-1.0.0rc1/panels/json/irc-index-pattern.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/irc.json` & `grimoirelab_panels-1.0.0rc1/panels/json/irc.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/jenkins-index-pattern.json` & `grimoirelab_panels-1.0.0rc1/panels/json/jenkins-index-pattern.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/jenkins.json` & `grimoirelab_panels-1.0.0rc1/panels/json/jenkins.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/jenkins_export.json` & `grimoirelab_panels-1.0.0rc1/panels/json/jenkins_export.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/jenkins_job_categories.json` & `grimoirelab_panels-1.0.0rc1/panels/json/jenkins_job_categories.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/jenkins_jobs.json` & `grimoirelab_panels-1.0.0rc1/panels/json/jenkins_jobs.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/jenkins_nodes.json` & `grimoirelab_panels-1.0.0rc1/panels/json/jenkins_nodes.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/jira-index-pattern.json` & `grimoirelab_panels-1.0.0rc1/panels/json/jira-index-pattern.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/jira.json` & `grimoirelab_panels-1.0.0rc1/panels/json/jira.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/jira_backlog.json` & `grimoirelab_panels-1.0.0rc1/panels/json/jira_backlog.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/jira_effort.json` & `grimoirelab_panels-1.0.0rc1/panels/json/jira_effort.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/jira_resolution_date-index-pattern.json` & `grimoirelab_panels-1.0.0rc1/panels/json/jira_resolution_date-index-pattern.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/jira_timing.json` & `grimoirelab_panels-1.0.0rc1/panels/json/jira_timing.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/kafka-index-pattern.json` & `grimoirelab_panels-1.0.0rc1/panels/json/kafka-index-pattern.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/kip.json` & `grimoirelab_panels-1.0.0rc1/panels/json/kip.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/lifecycle.json` & `grimoirelab_panels-1.0.0rc1/panels/json/lifecycle.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/mailinglists.json` & `grimoirelab_panels-1.0.0rc1/panels/json/mailinglists.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/maniphest-index-pattern.json` & `grimoirelab_panels-1.0.0rc1/panels/json/maniphest-index-pattern.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/maniphest.json` & `grimoirelab_panels-1.0.0rc1/panels/json/maniphest.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/maniphest_backlog.json` & `grimoirelab_panels-1.0.0rc1/panels/json/maniphest_backlog.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/maniphest_timing.json` & `grimoirelab_panels-1.0.0rc1/panels/json/maniphest_timing.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/mattermost-index-pattern.json` & `grimoirelab_panels-1.0.0rc1/panels/json/mattermost-index-pattern.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/mattermost.json` & `grimoirelab_panels-1.0.0rc1/panels/json/mattermost.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/mbox-index-pattern.json` & `grimoirelab_panels-1.0.0rc1/panels/json/mbox-index-pattern.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/mediawiki-index-pattern.json` & `grimoirelab_panels-1.0.0rc1/panels/json/mediawiki-index-pattern.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/mediawiki.json` & `grimoirelab_panels-1.0.0rc1/panels/json/mediawiki.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/meetup-index-pattern.json` & `grimoirelab_panels-1.0.0rc1/panels/json/meetup-index-pattern.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/meetup.json` & `grimoirelab_panels-1.0.0rc1/panels/json/meetup.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/meetup_locations.json` & `grimoirelab_panels-1.0.0rc1/panels/json/meetup_locations.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/mozilla_club-index-pattern.json` & `grimoirelab_panels-1.0.0rc1/panels/json/mozilla_club-index-pattern.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/mozilla_club.json` & `grimoirelab_panels-1.0.0rc1/panels/json/mozilla_club.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/onion_organizations.json` & `grimoirelab_panels-1.0.0rc1/panels/json/onion_organizations.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/onion_overall.json` & `grimoirelab_panels-1.0.0rc1/panels/json/onion_overall.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/onion_projects.json` & `grimoirelab_panels-1.0.0rc1/panels/json/onion_projects.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/organization_tracking_overview.json` & `grimoirelab_panels-1.0.0rc1/panels/json/organization_tracking_overview.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/organizational_diversity.json` & `grimoirelab_panels-1.0.0rc1/panels/json/organizational_diversity.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/organizational_diversity_by_domains.json` & `grimoirelab_panels-1.0.0rc1/panels/json/organizational_diversity_by_domains.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/overview.json` & `grimoirelab_panels-1.0.0rc1/panels/json/overview.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/redmine-index-pattern.json` & `grimoirelab_panels-1.0.0rc1/panels/json/redmine-index-pattern.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/redmine.json` & `grimoirelab_panels-1.0.0rc1/panels/json/redmine.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/redmine_backlog.json` & `grimoirelab_panels-1.0.0rc1/panels/json/redmine_backlog.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/redmine_timing.json` & `grimoirelab_panels-1.0.0rc1/panels/json/redmine_timing.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/remo-activities-index-pattern.json` & `grimoirelab_panels-1.0.0rc1/panels/json/remo-activities-index-pattern.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/remo-activities_metadata__timestamp-index-pattern.json` & `grimoirelab_panels-1.0.0rc1/panels/json/remo-activities_metadata__timestamp-index-pattern.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/remo-events-index-pattern.json` & `grimoirelab_panels-1.0.0rc1/panels/json/remo-events-index-pattern.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/remo-events_metadata__timestamp-index-pattern.json` & `grimoirelab_panels-1.0.0rc1/panels/json/remo-events_metadata__timestamp-index-pattern.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/reps_activities.json` & `grimoirelab_panels-1.0.0rc1/panels/json/reps_activities.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/reps_events.json` & `grimoirelab_panels-1.0.0rc1/panels/json/reps_events.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/rss-index-pattern.json` & `grimoirelab_panels-1.0.0rc1/panels/json/rss-index-pattern.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/rss.json` & `grimoirelab_panels-1.0.0rc1/panels/json/rss.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/slack-index-pattern.json` & `grimoirelab_panels-1.0.0rc1/panels/json/slack-index-pattern.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/slack.json` & `grimoirelab_panels-1.0.0rc1/panels/json/slack.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/slack_devrel.json` & `grimoirelab_panels-1.0.0rc1/panels/json/slack_devrel.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/stackoverflow-index-pattern.json` & `grimoirelab_panels-1.0.0rc1/panels/json/stackoverflow-index-pattern.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/stackoverflow.json` & `grimoirelab_panels-1.0.0rc1/panels/json/stackoverflow.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/telegram-index-pattern.json` & `grimoirelab_panels-1.0.0rc1/panels/json/telegram-index-pattern.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/telegram.json` & `grimoirelab_panels-1.0.0rc1/panels/json/telegram.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/testing_all.json` & `grimoirelab_panels-1.0.0rc1/panels/json/testing_all.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/testing_functest.json` & `grimoirelab_panels-1.0.0rc1/panels/json/testing_functest.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/timing_overview_tickets.json` & `grimoirelab_panels-1.0.0rc1/panels/json/timing_overview_tickets.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/twitter-index-pattern.json` & `grimoirelab_panels-1.0.0rc1/panels/json/twitter-index-pattern.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/twitter.json` & `grimoirelab_panels-1.0.0rc1/panels/json/twitter.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/weblate-index-pattern.json` & `grimoirelab_panels-1.0.0rc1/panels/json/weblate-index-pattern.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/weblate_demographics.json` & `grimoirelab_panels-1.0.0rc1/panels/json/weblate_demographics.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/panels/json/weblate_overview.json` & `grimoirelab_panels-1.0.0rc1/panels/json/weblate_overview.json`

 * *Files identical despite different names*

### Comparing `grimoirelab_panels-1.0.0/pyproject.toml` & `grimoirelab_panels-1.0.0rc1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grimoirelab-panels"
-version = "1.0.0"
+version = "1.0.0-rc.1"
 description = "Panels and visualizations for GrimoireLab dashboards"
 authors = [
     "GrimoireLab Developers"
 ]
 license = "GPL-3.0+"
 
 readme = "README.md"
```

### Comparing `grimoirelab_panels-1.0.0/PKG-INFO` & `grimoirelab_panels-1.0.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grimoirelab-panels
-Version: 1.0.0
+Version: 1.0.0rc1
 Summary: Panels and visualizations for GrimoireLab dashboards
 Home-page: https://chaoss.github.io/grimoirelab/
 License: GPL-3.0+
 Keywords: development,grimoirelab
 Author: GrimoireLab Developers
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

