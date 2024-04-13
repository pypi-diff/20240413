# Comparing `tmp/kcli-99.0.202404122133.tar.gz` & `tmp/kcli-99.0.202404131016.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kcli-99.0.202404122133.tar", last modified: Fri Apr 12 21:33:40 2024, max compression
+gzip compressed data, was "kcli-99.0.202404131016.tar", last modified: Sat Apr 13 10:16:47 2024, max compression
```

## Comparing `kcli-99.0.202404122133.tar` & `kcli-99.0.202404131016.tar`

### file list

```diff
@@ -1,788 +1,788 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.320762 kcli-99.0.202404122133/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-12 21:33:40.320762 kcli-99.0.202404122133/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.232762 kcli-99.0.202404122133/extras/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/extras/Dockerfile_curl
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/extras/Dockerfile_kubectl
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/extras/autoscale.yml
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/extras/aws_peering.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/extras/aws_peering_cleaning.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.232762 kcli-99.0.202404122133/extras/controller/
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/extras/controller/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/extras/controller/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/extras/controller/crd.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/extras/controller/deploy.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.232762 kcli-99.0.202404122133/extras/controller/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/extras/controller/examples/cluster_simple.yml
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/extras/controller/examples/plan_complex.yml
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/extras/controller/examples/plan_simple.yml
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/extras/controller/examples/plan_simple_with_file.yml
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/extras/controller/examples/vm_centos8stream.yml
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/extras/controller/examples/vm_cirros.yml
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/extras/controller/examples/vm_empty.yml
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/extras/controller/examples/vm_fedora.yml
--rw-r--r--   0 runner    (1001) docker     (127)     9970 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/extras/controller/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/extras/controller/stress_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/extras/debian
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.232762 kcli-99.0.202404122133/extras/expose/
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/extras/expose/kcli.conf
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/extras/expose/kcli.wsgi
--rwxr-xr-x   0 runner    (1001) docker     (127)      106 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/extras/genrst.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/extras/haproxy.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/extras/haproxy_multiple_clusters.cfg
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/extras/i_am_a_container
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/extras/k8sdeploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/extras/kfish.md
--rw-r--r--   0 runner    (1001) docker     (127)    38837 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/extras/kfish.png
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/extras/missing_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/extras/openstack.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/extras/openstack.sh.sample
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/extras/zerotier.service
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.232762 kcli-99.0.202404122133/kcli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-12 21:33:39.000000 kcli-99.0.202404122133/kcli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    27395 2024-04-12 21:33:39.000000 kcli-99.0.202404122133/kcli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 21:33:39.000000 kcli-99.0.202404122133/kcli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-12 21:33:39.000000 kcli-99.0.202404122133/kcli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 21:32:39.000000 kcli-99.0.202404122133/kcli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-04-12 21:33:39.000000 kcli-99.0.202404122133/kcli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-12 21:33:39.000000 kcli-99.0.202404122133/kcli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.236762 kcli-99.0.202404122133/kvirt/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.236762 kcli-99.0.202404122133/kvirt/ansibleutils/
--rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/ansibleutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    98893 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/baseconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)   171487 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/bottle.py
--rw-r--r--   0 runner    (1001) docker     (127)   278792 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.236762 kcli-99.0.202404122133/kvirt/cluster/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.236762 kcli-99.0.202404122133/kvirt/cluster/aks/
--rw-r--r--   0 runner    (1001) docker     (127)     9397 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/aks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/aks/fake.yml
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/aks/kcli_default.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.236762 kcli-99.0.202404122133/kvirt/cluster/eks/
--rw-r--r--   0 runner    (1001) docker     (127)    12290 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/eks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/eks/fake.yml
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/eks/kcli_default.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.240762 kcli-99.0.202404122133/kvirt/cluster/gke/
--rw-r--r--   0 runner    (1001) docker     (127)    12628 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/gke/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/gke/fake.yml
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/gke/kcli_default.yml
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/gke/kubeconfig.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.240762 kcli-99.0.202404122133/kvirt/cluster/hypershift/
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/hypershift/99-apps.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/hypershift/99-forcedns
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/hypershift/99-notifications.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/hypershift/Corefile
--rw-r--r--   0 runner    (1001) docker     (127)    46690 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/hypershift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/hypershift/assisted_infra.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/hypershift/assisted_ingress.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/hypershift/autoapprovercron.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/hypershift/bmc.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/hypershift/calico.sh.j2
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/hypershift/cilium.sh.j2
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/hypershift/cloud_lb_apps.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/hypershift/disconnected.sh
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/hypershift/extras.service
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/hypershift/extras.sh
--rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/hypershift/hostedcluster.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/hypershift/httpd.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/hypershift/ignition.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/hypershift/kcli_plan.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/hypershift/kcli_plan_default.yml
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/hypershift/keepalived.conf
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/hypershift/nmstateconfig.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/hypershift/nodepool.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/hypershift/nonlocalbind.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.240762 kcli-99.0.202404122133/kvirt/cluster/hypershift/staticpods/
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/hypershift/staticpods/coredns.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/hypershift/staticpods/keepalived.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/hypershift/staticpods/mdns.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.244762 kcli-99.0.202404122133/kvirt/cluster/k3s/
--rw-r--r--   0 runner    (1001) docker     (127)    13990 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/k3s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/k3s/bootstrap.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/k3s/bootstrap.yml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/k3s/cloud_lb_api.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/k3s/ctlplanes.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/k3s/ctlplanes.yml
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/k3s/join.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/k3s/kcli_default.yml
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/k3s/keepalived.conf
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/k3s/keepalived.sh
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/k3s/workers.sh
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/k3s/workers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.244762 kcli-99.0.202404122133/kvirt/cluster/kubeadm/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubeadm/10-flannel.link
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubeadm/90-flannel.rules
--rw-r--r--   0 runner    (1001) docker     (127)    14324 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubeadm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.220762 kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.248762 kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/argocd/
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/argocd/ingress.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/argocd/install.sh
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/argocd/kcli_default.yml
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/argocd/uninstall.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.248762 kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/autolabeller/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/autolabeller/install.sh
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/autolabeller/uninstall.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.248762 kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/certmanager/
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/certmanager/install.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.248762 kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/dashboard/
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/dashboard/admin.yml
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/dashboard/ingress.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/dashboard/install.sh
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/dashboard/kcli_default.yml
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/dashboard/user.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.248762 kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/falco/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/falco/falco_advertisements.yml
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/falco/falco_ip.yml
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/falco/install.sh
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/falco/kcli_default.yml
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/falco/uninstall.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.248762 kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/ingress/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/ingress/install.sh
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/ingress/uninstall.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.248762 kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/istio/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/istio/install.sh
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/istio/istio-minimal-operator.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.248762 kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/katacontainer/
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/katacontainer/install.sh
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/katacontainer/uninstall.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.248762 kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/knative/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/knative/cr_eventing.yml
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/knative/cr_serving.yml
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/knative/install.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.248762 kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/kubevirt/
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/kubevirt/install.sh
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/kubevirt/kcli_default.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.252762 kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/metallb/
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/metallb/install.sh
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/metallb/kcli_default.yml
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/metallb/metallb_advertisement.yml
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/metallb/metallb_cr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/metallb/uninstall.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.252762 kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/olm/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/olm/install.sh
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/olm/uninstall.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.252762 kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/policy_as_code/
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/policy_as_code/install.sh
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/policy_as_code/kcli_default.yml
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/policy_as_code/uninstall.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.252762 kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/rancher/
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/rancher/install.sh
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/rancher/kcli_default.yml
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/rancher/rancher_advertisements.yml
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/rancher/rancher_ip.yml
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/rancher/uninstall.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.252762 kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/rook/
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/rook/install.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.252762 kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/submariner/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/submariner/install.sh
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/submariner/kcli_default.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.252762 kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/tekton/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/tekton/install.sh
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/tekton/uninstall.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     3158 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubeadm/bootstrap.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubeadm/bootstrap.yml
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubeadm/cloud_lb_api.yml
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubeadm/crictl.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubeadm/ctlplanes.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)      343 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubeadm/deploy.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      598 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubeadm/join.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubeadm/kcli_default.yml
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubeadm/keepalived.conf
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubeadm/keepalived.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubeadm/nfs.sh
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubeadm/nfs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubeadm/pre_el.sh
--rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubeadm/pre_ubuntu.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubeadm/registry.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubeadm/workers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.252762 kcli-99.0.202404122133/kvirt/cluster/kubecommon/
--rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubecommon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.252762 kcli-99.0.202404122133/kvirt/cluster/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (127)     8809 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/kubernetes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.252762 kcli-99.0.202404122133/kvirt/cluster/microshift/
--rw-r--r--   0 runner    (1001) docker     (127)     4801 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/microshift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/microshift/kcli_plan.yml
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/microshift/kcli_plan_default.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.256762 kcli-99.0.202404122133/kvirt/cluster/microshift/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/microshift/scripts/00_sslip.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/microshift/scripts/01_clients.sh
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/microshift/scripts/02_crio.sh
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/microshift/scripts/03_microshift.sh
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/microshift/scripts/04_kubeconfig.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/microshift/scripts/05_acm.sh
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/microshift/scripts/deploy.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.264762 kcli-99.0.202404122133/kvirt/cluster/openshift/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/01-workload-partitioning
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/10-node-ip-hint.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/20-localhost-fix.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/99-apps.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/99-autologin.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/99-bootstrap-deletion-2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/99-bootstrap-deletion.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/99-chrony.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/99-forcedns
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/99-forcedns-ibm
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/99-kubevirt-fix.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/99-metal3-fake-machine.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/99-metal3-provisioning.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/99-notifications.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/99-operatorhub.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/99-ovn.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/99-sno.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/Corefile
--rwxr-xr-x   0 runner    (1001) docker     (127)    97690 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.264762 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.264762 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/advanced-cluster-management/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/advanced-cluster-management/99-metal3-provisioning.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/advanced-cluster-management/assisted-service.sample.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)     2839 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/advanced-cluster-management/assisted-service.sh
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/advanced-cluster-management/cr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/advanced-cluster-management/gen_registries.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/advanced-cluster-management/kcli_default.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/advanced-cluster-management/post.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.264762 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/argocd/
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/argocd/configmap.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/argocd/install.sh
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/argocd/kcli_default.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.264762 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/autolabeller/
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/autolabeller/cr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/autolabeller/install.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/autolabeller/install.yml
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/autolabeller/kcli_default.yml
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/autolabeller/uninstall.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.264762 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/cluster-logging/
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/cluster-logging/cr.yml
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/cluster-logging/kcli_default.yml
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/cr.sh
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/install.yml.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.264762 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/istio/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/istio/install.sh
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/istio/istio-cni.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.264762 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/kubernetes-nmstate-operator/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/kubernetes-nmstate-operator/cr.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.264762 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/kubevirt-hyperconverged/
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/kubevirt-hyperconverged/cr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/kubevirt-hyperconverged/kcli_default.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.268762 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/local-storage-operator/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/local-storage-operator/cr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/local-storage-operator/kcli_default.yml
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/local-storage-operator/post.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.268762 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/lvms-operator/
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/lvms-operator/cr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/lvms-operator/kcli_default.yml
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/lvms-operator/post.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.268762 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/metallb-operator/
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/metallb-operator/cr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/metallb-operator/kcli_default.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.268762 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/multicluster-engine/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/multicluster-engine/99-metal3-provisioning.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/multicluster-engine/assisted-service.sample.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)     2846 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/multicluster-engine/assisted-service.sh
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/multicluster-engine/cr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/multicluster-engine/gen_registries.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/multicluster-engine/kcli_default.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)       55 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/multicluster-engine/post.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.268762 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/nfs/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2297 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/nfs/install.sh
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/nfs/kcli_default.yml
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/nfs/uninstall.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.268762 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/odf-operator/
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/odf-operator/cr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/odf-operator/kcli_default.yml
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/odf-operator/nad_cluster.yml
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/odf-operator/nad_public.yml
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/odf-operator/post.sh
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/odf-operator/pre.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.268762 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/serverless-operator/
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/serverless-operator/cr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/serverless-operator/kcli_default.yml
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/serverless-operator/post.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.272762 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/users/
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/users/install.sh
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/users/kcli_default.yml
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/users/oauth.yml
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/users/oauth_hypershift.yml
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/apps/users/uninstall.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/autoapprovercron.yml
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/autorules.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/bootstrap.yml
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/calico.sh.j2
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/chrony.conf
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/cilium.sh.j2
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/cloud_bootstrap.yml
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/cloud_ctlplanes.yml
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/cloud_dns.yml
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/cloud_lb_api.yml
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/cloud_lb_apps.yml
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/cloud_workers.yml
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/cluster-ingress-02-config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/cluster-scheduler-02-config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/config.hcl.templ
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/ctlplanes.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.272762 kcli-99.0.202404122133/kvirt/cluster/openshift/customisation/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/customisation/00-kcli-namespace.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/customisation/97-autoapprovercron-sa.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/customisation/98-autoapprovercron-binding.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/customisation/99-autoapprovercron-cronjob.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/customisation/99-ingress-controller.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/customisation/99-iptables.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/customisation/99-monitoring.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/customisation/99-registry.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/dhcp.conf
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/dhcp.sh
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/dhcp.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.272762 kcli-99.0.202404122133/kvirt/cluster/openshift/disconnected/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.272762 kcli-99.0.202404122133/kvirt/cluster/openshift/disconnected/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)      357 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/disconnected/bin/sync_image.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/disconnected/haproxy.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/disconnected/registry.service
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.272762 kcli-99.0.202404122133/kvirt/cluster/openshift/disconnected/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)      201 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/disconnected/scripts/01_get_oc.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      243 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/disconnected/scripts/02_packages.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     2412 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/disconnected/scripts/03_mirror.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     2101 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/disconnected/scripts/03_registry.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      331 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/disconnected/scripts/04_extras.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     2349 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/disconnected/scripts/05_olm.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      197 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/disconnected/scripts/06_web.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      841 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/disconnected/scripts/deploy.sh
--rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/disconnected/scripts/mirror-config.yaml.sample
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/disconnected.yml
--rw-r--r--   0 runner    (1001) docker     (127)     8945 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/fake_kubeconfig.json
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/fake_pull.json
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/haproxy.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/haproxy.cfg.kubevirt
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/httpd.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/icsp.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/ignition.j2
--rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/install-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/iso.sh
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/kcli-ipv6.conf.j2
--rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/kcli_default.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/keepalived.conf
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/nonlocalbind.conf
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/openshift-workload-pinning
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/patch_ipv6.json
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/relocate-ip-bootstrap.service
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/relocate-ip-bootstrap.sh
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/relocate-ip.sh
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/sno-finish.service
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/sno-finish.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/sno.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/sno_default.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.272762 kcli-99.0.202404122133/kvirt/cluster/openshift/staticpods/
--rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/staticpods/coredns.yml
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/staticpods/haproxy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/staticpods/keepalived.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/staticpods/mdns.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/openshift/workers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.276762 kcli-99.0.202404122133/kvirt/cluster/profiles/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/profiles/sample-kubeadm-default.yml
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/profiles/sample-openshift-compact.yml
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/profiles/sample-openshift-contrail.yml
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/profiles/sample-openshift-ipv6.yml
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/profiles/sample-openshift-sno-bm.yml
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/profiles/sample-openshift-sno.yml
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/cluster/sampleprovider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.276762 kcli-99.0.202404122133/kvirt/common/
--rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/common/Jenkinsfile.j2
--rw-r--r--   0 runner    (1001) docker     (127)   105973 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/common/autoscale.yaml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     8945 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/common/fake_kubeconfig.json
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/common/ignition.j2
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/common/kubevirt_kcli_conf.j2
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/common/local_kcli_conf.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/common/pipeline.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/common/pipeline_kube.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/common/playbook.j2
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/common/storage.sh.aws
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/common/storage.sh.gcp
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/common/storage.sh.ibmcloud
--rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/common/vm.ovf.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/common/workflow.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/common/workflow_script.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)   191138 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.276762 kcli-99.0.202404122133/kvirt/container/
--rw-r--r--   0 runner    (1001) docker     (127)    14188 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/containerconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)    10807 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/defaults.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1475 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/ekstoken.py
--rw-r--r--   0 runner    (1001) docker     (127)    25462 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/examples.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.276762 kcli-99.0.202404122133/kvirt/expose/
--rw-r--r--   0 runner    (1001) docker     (127)    12263 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/expose/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.224762 kcli-99.0.202404122133/kvirt/expose/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.276762 kcli-99.0.202404122133/kvirt/expose/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/expose/static/css/bootstrap-notify.css
--rw-r--r--   0 runner    (1001) docker     (127)   121125 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/expose/static/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/expose/static/css/dataTables.checkboxes.css
--rw-r--r--   0 runner    (1001) docker     (127)    13587 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/expose/static/css/jquery.dataTables.min.css
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/expose/static/css/kcli.css
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/expose/static/css/wheel.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.280762 kcli-99.0.202404122133/kvirt/expose/static/images/
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/expose/static/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/expose/static/images/sort_asc.png
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/expose/static/images/sort_both.png
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/expose/static/images/sort_desc.png
--rw-r--r--   0 runner    (1001) docker     (127)    24772 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/expose/static/images/wheel.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.280762 kcli-99.0.202404122133/kvirt/expose/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)    12398 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/expose/static/js/dataTables.checkboxes.min.js
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/expose/static/js/exposeactions.js
--rw-r--r--   0 runner    (1001) docker     (127)    83059 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/expose/static/js/jquery.dataTables.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    89795 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/expose/static/js/jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/expose/static/js/list.js
--rw-r--r--   0 runner    (1001) docker     (127)     4319 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/expose/swagger.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.280762 kcli-99.0.202404122133/kvirt/expose/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/expose/templates/form.html
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/expose/templates/head.html
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/expose/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/expose/templates/infoplan.html
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/expose/templates/planstable.html
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/expose/templates/result.html
--rwxr-xr-x   0 runner    (1001) docker     (127)     1047 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/gketoken.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4333 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/ignitionmerger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.280762 kcli-99.0.202404122133/kvirt/internalplans/
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/internalplans/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.280762 kcli-99.0.202404122133/kvirt/jinjafilters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/jinjafilters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6102 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/jinjafilters/jinjafilters.py
--rw-r--r--   0 runner    (1001) docker     (127)     9972 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/keywords.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.280762 kcli-99.0.202404122133/kvirt/kfish/
--rw-r--r--   0 runner    (1001) docker     (127)    13060 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/kfish/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3395 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/klist.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.280762 kcli-99.0.202404122133/kvirt/ksushy/
--rw-r--r--   0 runner    (1001) docker     (127)    13633 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/ksushy/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      121 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/ksushy/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.280762 kcli-99.0.202404122133/kvirt/ksushy/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/ksushy/templates/bios.json
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/ksushy/templates/interface.json
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/ksushy/templates/interfaces.json
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/ksushy/templates/manager.json
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/ksushy/templates/managers.json
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/ksushy/templates/root.json
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/ksushy/templates/system.json
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/ksushy/templates/systems.json
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/ksushy/templates/virtualmedia_cd.json
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/ksushy/templates/virtualmedias.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.284762 kcli-99.0.202404122133/kvirt/miniconsole/
--rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/miniconsole/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.284762 kcli-99.0.202404122133/kvirt/nameutils/
--rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/nameutils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.284762 kcli-99.0.202404122133/kvirt/providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.284762 kcli-99.0.202404122133/kvirt/providers/aws/
--rw-r--r--   0 runner    (1001) docker     (127)   106425 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/providers/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/providers/aws/assume_policy.json
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/providers/aws/ctlplane_policy.json
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/providers/aws/worker_policy.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.284762 kcli-99.0.202404122133/kvirt/providers/azure/
--rw-r--r--   0 runner    (1001) docker     (127)    78530 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/providers/azure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.284762 kcli-99.0.202404122133/kvirt/providers/fake/
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/providers/fake/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.284762 kcli-99.0.202404122133/kvirt/providers/gcp/
--rw-r--r--   0 runner    (1001) docker     (127)   101005 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/providers/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/providers/gcp/gcp-hack.service
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/providers/gcp/gcp-hack.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.284762 kcli-99.0.202404122133/kvirt/providers/ibm/
--rw-r--r--   0 runner    (1001) docker     (127)    65793 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/providers/ibm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.284762 kcli-99.0.202404122133/kvirt/providers/kubevirt/
--rw-r--r--   0 runner    (1001) docker     (127)    86428 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/providers/kubevirt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.284762 kcli-99.0.202404122133/kvirt/providers/kvm/
--rw-r--r--   0 runner    (1001) docker     (127)   186681 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/providers/kvm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/providers/kvm/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.284762 kcli-99.0.202404122133/kvirt/providers/openstack/
--rw-r--r--   0 runner    (1001) docker     (127)    58301 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/providers/openstack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.284762 kcli-99.0.202404122133/kvirt/providers/ovirt/
--rw-r--r--   0 runner    (1001) docker     (127)    63291 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/providers/ovirt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.284762 kcli-99.0.202404122133/kvirt/providers/packet/
--rw-r--r--   0 runner    (1001) docker     (127)    31823 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/providers/packet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.288762 kcli-99.0.202404122133/kvirt/providers/proxmox/
--rw-r--r--   0 runner    (1001) docker     (127)    35211 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/providers/proxmox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9555 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/providers/sampleprovider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.288762 kcli-99.0.202404122133/kvirt/providers/vsphere/
--rw-r--r--   0 runner    (1001) docker     (127)    73908 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/providers/vsphere/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13503 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/providers/vsphere/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4893 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/providers/vsphere/tagging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.288762 kcli-99.0.202404122133/kvirt/providers/web/
--rw-r--r--   0 runner    (1001) docker     (127)    22043 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/providers/web/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.288762 kcli-99.0.202404122133/kvirt/version/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-12 21:33:39.000000 kcli-99.0.202404122133/kvirt/version/git
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.288762 kcli-99.0.202404122133/kvirt/web/
--rwxr-xr-x   0 runner    (1001) docker     (127)    46680 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.228762 kcli-99.0.202404122133/kvirt/web/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.288762 kcli-99.0.202404122133/kvirt/web/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/css/bootstrap-notify.css
--rw-r--r--   0 runner    (1001) docker     (127)    23409 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/css/bootstrap-theme.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   121125 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/css/dataTables.checkboxes.css
--rw-r--r--   0 runner    (1001) docker     (127)    13587 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/css/jquery.dataTables.min.css
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/css/kcli.css
--rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/css/navbar.css
--rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/css/spice.css
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/css/wheel.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.288762 kcli-99.0.202404122133/kvirt/web/static/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)    18028 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.292762 kcli-99.0.202404122133/kvirt/web/static/images/
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/images/Centos.png
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/images/Debian.png
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/images/Fedora.png
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/images/Redhat.png
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/images/Suse.png
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/images/Tux.png
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/images/Ubuntu.png
--rw-r--r--   0 runner    (1001) docker     (127)     4213 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/images/delete.png
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)    23320 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/images/kcli-small.png
--rw-r--r--   0 runner    (1001) docker     (127)    27185 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/images/kcli.jpg
--rw-r--r--   0 runner    (1001) docker     (127)   113928 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/images/kcli.png
--rw-r--r--   0 runner    (1001) docker     (127)    48809 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/images/logo-header.svg
--rw-r--r--   0 runner    (1001) docker     (127)    48809 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/images/logo-main.svg
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/images/sort_asc.png
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/images/sort_both.png
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/images/sort_desc.png
--rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/images/start.png
--rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/images/stop.png
--rw-r--r--   0 runner    (1001) docker     (127)    24772 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/images/wheel.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.296762 kcli-99.0.202404122133/kvirt/web/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/js/bootstrap-notify.js
--rw-r--r--   0 runner    (1001) docker     (127)    37045 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/js/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/js/containeraction.js
--rw-r--r--   0 runner    (1001) docker     (127)    12398 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/js/dataTables.checkboxes.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/js/hostaction.js
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/js/imageaction.js
--rw-r--r--   0 runner    (1001) docker     (127)    83059 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/js/jquery.dataTables.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    87462 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/js/jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/js/kcli.js
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/js/kubeaction.js
--rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/js/list.js
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/js/networkaction.js
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/js/planaction.js
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/js/poolaction.js
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/js/productaction.js
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/js/refresh.js
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/js/repoaction.js
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/js/snapshotaction.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.300762 kcli-99.0.202404122133/kvirt/web/static/js/spice/
--rw-r--r--   0 runner    (1001) docker     (127)     9944 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/js/spice/atKeynames.js
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/js/spice/bitmap.js
--rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/js/spice/cursor.js
--rw-r--r--   0 runner    (1001) docker     (127)    49214 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/js/spice/display.js
--rw-r--r--   0 runner    (1001) docker     (127)    13253 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/js/spice/enums.js
--rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/js/spice/filexfer.js
--rw-r--r--   0 runner    (1001) docker     (127)     9535 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/js/spice/inputs.js
--rw-r--r--   0 runner    (1001) docker     (127)     6176 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/js/spice/lz.js
--rw-r--r--   0 runner    (1001) docker     (127)    18370 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/js/spice/main.js
--rw-r--r--   0 runner    (1001) docker     (127)    12677 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/js/spice/playback.js
--rw-r--r--   0 runner    (1001) docker     (127)     7036 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/js/spice/png.js
--rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/js/spice/port.js
--rw-r--r--   0 runner    (1001) docker     (127)    44531 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/js/spice/quic.js
--rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/js/spice/resize.js
--rw-r--r--   0 runner    (1001) docker     (127)     7282 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/js/spice/simulatecursor.js
--rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/js/spice/spicearraybuffer.js
--rw-r--r--   0 runner    (1001) docker     (127)    18202 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/js/spice/spiceconn.js
--rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/js/spice/spicedataview.js
--rw-r--r--   0 runner    (1001) docker     (127)    33015 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/js/spice/spicemsg.js
--rw-r--r--   0 runner    (1001) docker     (127)    12767 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/js/spice/spicetype.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.300762 kcli-99.0.202404122133/kvirt/web/static/js/spice/thirdparty/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.300762 kcli-99.0.202404122133/kvirt/web/static/js/spice/thirdparty/browser-es-module-loader/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/js/spice/thirdparty/browser-es-module-loader/.npmignore
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/js/spice/thirdparty/browser-es-module-loader/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/js/spice/thirdparty/browser-es-module-loader/rollup.config.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.300762 kcli-99.0.202404122133/kvirt/web/static/js/spice/thirdparty/browser-es-module-loader/src/
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/js/spice/thirdparty/browser-es-module-loader/src/babel-worker.js
--rw-r--r--   0 runner    (1001) docker     (127)     8601 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/js/spice/thirdparty/browser-es-module-loader/src/browser-es-module-loader.js
--rw-r--r--   0 runner    (1001) docker     (127)    16580 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/js/spice/thirdparty/jsbn.js
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/js/spice/thirdparty/prng4.js
--rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/js/spice/thirdparty/rng.js
--rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/js/spice/thirdparty/rsa.js
--rw-r--r--   0 runner    (1001) docker     (127)    10671 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/js/spice/thirdparty/sha1.js
--rw-r--r--   0 runner    (1001) docker     (127)     6808 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/js/spice/ticket.js
--rw-r--r--   0 runner    (1001) docker     (127)    13628 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/js/spice/utils.js
--rw-r--r--   0 runner    (1001) docker     (127)    21577 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/js/spice/webm.js
--rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/js/spice/wire.js
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/js/vmaction.js
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/js/wheel.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.228762 kcli-99.0.202404122133/kvirt/web/static/vnc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.300762 kcli-99.0.202404122133/kvirt/web/static/vnc/app/
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/app/error-handler.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.304762 kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/
--rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/alt.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/clipboard.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/connect.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4381 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/ctrl.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3237 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/ctrlaltdel.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5062 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/disconnect.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4684 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/drag.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/error.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/esc.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/expander.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/fullscreen.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/handle.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6386 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/handle_bg.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.304762 kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/icons/
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/icons/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/icons/novnc-120x120.png
--rw-r--r--   0 runner    (1001) docker     (127)     4582 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/icons/novnc-144x144.png
--rw-r--r--   0 runner    (1001) docker     (127)     5216 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/icons/novnc-152x152.png
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/icons/novnc-16x16.png
--rw-r--r--   0 runner    (1001) docker     (127)     5787 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/icons/novnc-192x192.png
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/icons/novnc-24x24.png
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/icons/novnc-32x32.png
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/icons/novnc-48x48.png
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/icons/novnc-60x60.png
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/icons/novnc-64x64.png
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/icons/novnc-72x72.png
--rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/icons/novnc-76x76.png
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/icons/novnc-96x96.png
--rw-r--r--   0 runner    (1001) docker     (127)    11685 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/icons/novnc-icon-sm.svg
--rw-r--r--   0 runner    (1001) docker     (127)    11549 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/icons/novnc-icon.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/info.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6404 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/keyboard.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7000 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/mouse_left.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7002 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/mouse_middle.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6993 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/mouse_none.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7001 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/mouse_right.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/power.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/settings.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/tab.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/toggleextrakeys.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/warning.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/windows.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.308761 kcli-99.0.202404122133/kvirt/web/static/vnc/app/locale/
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/app/locale/cs.json
--rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/app/locale/de.json
--rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/app/locale/el.json
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/app/locale/es.json
--rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/app/locale/ja.json
--rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/app/locale/ko.json
--rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/app/locale/nl.json
--rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/app/locale/pl.json
--rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/app/locale/ru.json
--rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/app/locale/sv.json
--rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/app/locale/tr.json
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/app/locale/zh_CN.json
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/app/locale/zh_TW.json
--rw-r--r--   0 runner    (1001) docker     (127)     5682 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/app/localization.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.308761 kcli-99.0.202404122133/kvirt/web/static/vnc/app/sounds/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/app/sounds/CREDITS
--rw-r--r--   0 runner    (1001) docker     (127)     4531 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/app/sounds/bell.mp3
--rw-r--r--   0 runner    (1001) docker     (127)     8495 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/app/sounds/bell.oga
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.308761 kcli-99.0.202404122133/kvirt/web/static/vnc/app/styles/
--rw-r--r--   0 runner    (1001) docker     (127)    38580 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/app/styles/Orbitron700.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    17472 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/app/styles/Orbitron700.woff
--rw-r--r--   0 runner    (1001) docker     (127)    18450 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/app/styles/base.css
--rw-r--r--   0 runner    (1001) docker     (127)    56845 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/app/ui.js
--rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/app/webutil.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.308761 kcli-99.0.202404122133/kvirt/web/static/vnc/core/
--rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/core/base64.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.308761 kcli-99.0.202404122133/kvirt/web/static/vnc/core/decoders/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/core/decoders/copyrect.js
--rw-r--r--   0 runner    (1001) docker     (127)     4814 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/core/decoders/hextile.js
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/core/decoders/raw.js
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/core/decoders/rre.js
--rw-r--r--   0 runner    (1001) docker     (127)     9662 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/core/decoders/tight.js
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/core/decoders/tightpng.js
--rw-r--r--   0 runner    (1001) docker     (127)    11241 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/core/des.js
--rw-r--r--   0 runner    (1001) docker     (127)    20381 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/core/display.js
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/core/encodings.js
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/core/inflator.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.312761 kcli-99.0.202404122133/kvirt/web/static/vnc/core/input/
--rw-r--r--   0 runner    (1001) docker     (127)    11438 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/core/input/domkeytable.js
--rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/core/input/fixedkeys.js
--rw-r--r--   0 runner    (1001) docker     (127)    13090 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/core/input/keyboard.js
--rw-r--r--   0 runner    (1001) docker     (127)    34609 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/core/input/keysym.js
--rw-r--r--   0 runner    (1001) docker     (127)    25374 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/core/input/keysymdef.js
--rw-r--r--   0 runner    (1001) docker     (127)     9995 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/core/input/mouse.js
--rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/core/input/util.js
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/core/input/vkeys.js
--rw-r--r--   0 runner    (1001) docker     (127)    14256 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/core/input/xtscancodes.js
--rw-r--r--   0 runner    (1001) docker     (127)    74196 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/core/rfb.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.312761 kcli-99.0.202404122133/kvirt/web/static/vnc/core/util/
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/core/util/browser.js
--rw-r--r--   0 runner    (1001) docker     (127)     7556 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/core/util/cursor.js
--rw-r--r--   0 runner    (1001) docker     (127)     4221 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/core/util/events.js
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/core/util/eventtarget.js
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/core/util/logging.js
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/core/util/polyfill.js
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/core/util/strings.js
--rw-r--r--   0 runner    (1001) docker     (127)     9130 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/core/websock.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.312761 kcli-99.0.202404122133/kvirt/web/static/vnc/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.312761 kcli-99.0.202404122133/kvirt/web/static/vnc/vendor/browser-es-module-loader/
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/vendor/browser-es-module-loader/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/vendor/browser-es-module-loader/rollup.config.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.312761 kcli-99.0.202404122133/kvirt/web/static/vnc/vendor/browser-es-module-loader/src/
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/vendor/browser-es-module-loader/src/babel-worker.js
--rw-r--r--   0 runner    (1001) docker     (127)     8498 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/vendor/browser-es-module-loader/src/browser-es-module-loader.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.312761 kcli-99.0.202404122133/kvirt/web/static/vnc/vendor/pako/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/vendor/pako/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/vendor/pako/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.228762 kcli-99.0.202404122133/kvirt/web/static/vnc/vendor/pako/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.312761 kcli-99.0.202404122133/kvirt/web/static/vnc/vendor/pako/lib/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/vendor/pako/lib/utils/common.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.316762 kcli-99.0.202404122133/kvirt/web/static/vnc/vendor/pako/lib/zlib/
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/vendor/pako/lib/zlib/adler32.js
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/vendor/pako/lib/zlib/constants.js
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/vendor/pako/lib/zlib/crc32.js
--rw-r--r--   0 runner    (1001) docker     (127)    60016 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/vendor/pako/lib/zlib/deflate.js
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/vendor/pako/lib/zlib/gzheader.js
--rw-r--r--   0 runner    (1001) docker     (127)    11690 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/vendor/pako/lib/zlib/inffast.js
--rw-r--r--   0 runner    (1001) docker     (127)    47128 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/vendor/pako/lib/zlib/inflate.js
--rw-r--r--   0 runner    (1001) docker     (127)    11527 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/vendor/pako/lib/zlib/inftrees.js
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/vendor/pako/lib/zlib/messages.js
--rw-r--r--   0 runner    (1001) docker     (127)    38767 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/vendor/pako/lib/zlib/trees.js
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/vendor/pako/lib/zlib/zstream.js
--rw-r--r--   0 runner    (1001) docker     (127)     7388 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/static/vnc/vendor/promise.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.320762 kcli-99.0.202404122133/kvirt/web/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/templates/bootstrap.html
--rw-r--r--   0 runner    (1001) docker     (127)    14595 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/templates/console.html
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/templates/containercreate.html
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/templates/containerprofiles.html
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/templates/containerprofilestable.html
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/templates/containers.html
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/templates/containerstable.html
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/templates/head.html
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/templates/hosts.html
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/templates/hoststable.html
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/templates/imagecreate.html
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/templates/images.html
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/templates/imagestable.html
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/templates/isos.html
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/templates/isostable.html
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/templates/kubecreate.html
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/templates/kubeinfo.html
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/templates/kubeprofiles.html
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/templates/kubeprofilestable.html
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/templates/kubes.html
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/templates/kubestable.html
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (127)     5517 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/templates/navbar.html
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/templates/networkcreate.html
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/templates/networks.html
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/templates/networkstable.html
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/templates/plancreate.html
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/templates/plans.html
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/templates/planstable.html
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/templates/poolcreate.html
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/templates/pools.html
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/templates/poolstable.html
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/templates/productcreate.html
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/templates/products.html
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/templates/productstable.html
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/templates/repocreate.html
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/templates/repos.html
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/templates/repostable.html
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/templates/vmcreate.html
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/templates/vmprofiles.html
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/templates/vmprofilestable.html
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/templates/vms.html
--rw-r--r--   0 runner    (1001) docker     (127)     4894 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/kvirt/web/templates/vmstable.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.320762 kcli-99.0.202404122133/samples/
--rw-r--r--   0 runner    (1001) docker     (127)     8879 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/samples/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/samples/profiles.yml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 21:33:40.320762 kcli-99.0.202404122133/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-04-12 21:33:39.000000 kcli-99.0.202404122133/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:33:40.320762 kcli-99.0.202404122133/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-12 21:31:40.000000 kcli-99.0.202404122133/tests/test_kvirt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.223247 kcli-99.0.202404131016/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-13 10:16:47.223247 kcli-99.0.202404131016/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.139247 kcli-99.0.202404131016/extras/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/extras/Dockerfile_curl
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/extras/Dockerfile_kubectl
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/extras/autoscale.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/extras/aws_peering.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/extras/aws_peering_cleaning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.139247 kcli-99.0.202404131016/extras/controller/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/extras/controller/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/extras/controller/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/extras/controller/crd.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/extras/controller/deploy.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.139247 kcli-99.0.202404131016/extras/controller/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/extras/controller/examples/cluster_simple.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/extras/controller/examples/plan_complex.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/extras/controller/examples/plan_simple.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/extras/controller/examples/plan_simple_with_file.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/extras/controller/examples/vm_centos8stream.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/extras/controller/examples/vm_cirros.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/extras/controller/examples/vm_empty.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/extras/controller/examples/vm_fedora.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     9970 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/extras/controller/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/extras/controller/stress_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/extras/debian
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.143247 kcli-99.0.202404131016/extras/expose/
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/extras/expose/kcli.conf
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/extras/expose/kcli.wsgi
+-rwxr-xr-x   0 runner    (1001) docker     (127)      106 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/extras/genrst.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/extras/haproxy.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/extras/haproxy_multiple_clusters.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/extras/i_am_a_container
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/extras/k8sdeploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/extras/kfish.md
+-rw-r--r--   0 runner    (1001) docker     (127)    38837 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/extras/kfish.png
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/extras/missing_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/extras/openstack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/extras/openstack.sh.sample
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/extras/zerotier.service
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.143247 kcli-99.0.202404131016/kcli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-13 10:16:46.000000 kcli-99.0.202404131016/kcli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    27395 2024-04-13 10:16:46.000000 kcli-99.0.202404131016/kcli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 10:16:46.000000 kcli-99.0.202404131016/kcli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-13 10:16:46.000000 kcli-99.0.202404131016/kcli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 10:15:02.000000 kcli-99.0.202404131016/kcli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-04-13 10:16:46.000000 kcli-99.0.202404131016/kcli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-13 10:16:46.000000 kcli-99.0.202404131016/kcli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.147247 kcli-99.0.202404131016/kvirt/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.147247 kcli-99.0.202404131016/kvirt/ansibleutils/
+-rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/ansibleutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    98893 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/baseconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)   171487 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/bottle.py
+-rw-r--r--   0 runner    (1001) docker     (127)   278792 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.147247 kcli-99.0.202404131016/kvirt/cluster/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.147247 kcli-99.0.202404131016/kvirt/cluster/aks/
+-rw-r--r--   0 runner    (1001) docker     (127)     9397 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/aks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/aks/fake.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/aks/kcli_default.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.147247 kcli-99.0.202404131016/kvirt/cluster/eks/
+-rw-r--r--   0 runner    (1001) docker     (127)    12290 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/eks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/eks/fake.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/eks/kcli_default.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.147247 kcli-99.0.202404131016/kvirt/cluster/gke/
+-rw-r--r--   0 runner    (1001) docker     (127)    12628 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/gke/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/gke/fake.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/gke/kcli_default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/gke/kubeconfig.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.151247 kcli-99.0.202404131016/kvirt/cluster/hypershift/
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/hypershift/99-apps.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/hypershift/99-forcedns
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/hypershift/99-notifications.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/hypershift/Corefile
+-rw-r--r--   0 runner    (1001) docker     (127)    46690 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/hypershift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/hypershift/assisted_infra.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/hypershift/assisted_ingress.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/hypershift/autoapprovercron.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/hypershift/bmc.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/hypershift/calico.sh.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/hypershift/cilium.sh.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/hypershift/cloud_lb_apps.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/hypershift/disconnected.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/hypershift/extras.service
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/hypershift/extras.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/hypershift/hostedcluster.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/hypershift/httpd.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/hypershift/ignition.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/hypershift/kcli_plan.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/hypershift/kcli_plan_default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/hypershift/keepalived.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/hypershift/nmstateconfig.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/hypershift/nodepool.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/hypershift/nonlocalbind.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.151247 kcli-99.0.202404131016/kvirt/cluster/hypershift/staticpods/
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/hypershift/staticpods/coredns.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/hypershift/staticpods/keepalived.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/hypershift/staticpods/mdns.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.151247 kcli-99.0.202404131016/kvirt/cluster/k3s/
+-rw-r--r--   0 runner    (1001) docker     (127)    13990 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/k3s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/k3s/bootstrap.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/k3s/bootstrap.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/k3s/cloud_lb_api.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/k3s/ctlplanes.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/k3s/ctlplanes.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/k3s/join.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/k3s/kcli_default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/k3s/keepalived.conf
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/k3s/keepalived.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/k3s/workers.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/k3s/workers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.155247 kcli-99.0.202404131016/kvirt/cluster/kubeadm/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubeadm/10-flannel.link
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubeadm/90-flannel.rules
+-rw-r--r--   0 runner    (1001) docker     (127)    14324 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubeadm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.127246 kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.155247 kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/argocd/
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/argocd/ingress.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/argocd/install.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/argocd/kcli_default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/argocd/uninstall.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.155247 kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/autolabeller/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/autolabeller/install.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/autolabeller/uninstall.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.155247 kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/certmanager/
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/certmanager/install.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.155247 kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/dashboard/admin.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/dashboard/ingress.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/dashboard/install.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/dashboard/kcli_default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/dashboard/user.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.155247 kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/falco/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/falco/falco_advertisements.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/falco/falco_ip.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/falco/install.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/falco/kcli_default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/falco/uninstall.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.155247 kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/ingress/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/ingress/install.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/ingress/uninstall.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.159247 kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/istio/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/istio/install.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/istio/istio-minimal-operator.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.159247 kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/katacontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/katacontainer/install.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/katacontainer/uninstall.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.159247 kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/knative/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/knative/cr_eventing.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/knative/cr_serving.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/knative/install.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.159247 kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/kubevirt/
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/kubevirt/install.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/kubevirt/kcli_default.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.159247 kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/metallb/
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/metallb/install.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/metallb/kcli_default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/metallb/metallb_advertisement.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/metallb/metallb_cr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/metallb/uninstall.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.159247 kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/olm/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/olm/install.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/olm/uninstall.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.159247 kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/policy_as_code/
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/policy_as_code/install.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/policy_as_code/kcli_default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/policy_as_code/uninstall.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.159247 kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/rancher/
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/rancher/install.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/rancher/kcli_default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/rancher/rancher_advertisements.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/rancher/rancher_ip.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/rancher/uninstall.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.159247 kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/rook/
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/rook/install.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.159247 kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/submariner/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/submariner/install.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/submariner/kcli_default.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.159247 kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/tekton/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/tekton/install.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/tekton/uninstall.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3158 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubeadm/bootstrap.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubeadm/bootstrap.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubeadm/cloud_lb_api.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubeadm/crictl.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubeadm/ctlplanes.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      343 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubeadm/deploy.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      598 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubeadm/join.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubeadm/kcli_default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubeadm/keepalived.conf
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubeadm/keepalived.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubeadm/nfs.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubeadm/nfs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubeadm/pre_el.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubeadm/pre_ubuntu.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubeadm/registry.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubeadm/workers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.159247 kcli-99.0.202404131016/kvirt/cluster/kubecommon/
+-rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubecommon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.159247 kcli-99.0.202404131016/kvirt/cluster/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (127)     8809 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/kubernetes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.163247 kcli-99.0.202404131016/kvirt/cluster/microshift/
+-rw-r--r--   0 runner    (1001) docker     (127)     4801 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/microshift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/microshift/kcli_plan.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/microshift/kcli_plan_default.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.163247 kcli-99.0.202404131016/kvirt/cluster/microshift/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/microshift/scripts/00_sslip.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/microshift/scripts/01_clients.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/microshift/scripts/02_crio.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/microshift/scripts/03_microshift.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/microshift/scripts/04_kubeconfig.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/microshift/scripts/05_acm.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/microshift/scripts/deploy.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.171247 kcli-99.0.202404131016/kvirt/cluster/openshift/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/01-workload-partitioning
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/10-node-ip-hint.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/20-localhost-fix.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/99-apps.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/99-autologin.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/99-bootstrap-deletion-2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/99-bootstrap-deletion.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/99-chrony.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/99-forcedns
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/99-forcedns-ibm
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/99-kubevirt-fix.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/99-metal3-fake-machine.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/99-metal3-provisioning.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/99-notifications.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/99-operatorhub.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/99-ovn.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/99-sno.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/Corefile
+-rwxr-xr-x   0 runner    (1001) docker     (127)    97690 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.171247 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.171247 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/advanced-cluster-management/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/advanced-cluster-management/99-metal3-provisioning.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/advanced-cluster-management/assisted-service.sample.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2839 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/advanced-cluster-management/assisted-service.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/advanced-cluster-management/cr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/advanced-cluster-management/gen_registries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/advanced-cluster-management/kcli_default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/advanced-cluster-management/post.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.171247 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/argocd/
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/argocd/configmap.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/argocd/install.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/argocd/kcli_default.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.171247 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/autolabeller/
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/autolabeller/cr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/autolabeller/install.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/autolabeller/install.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/autolabeller/kcli_default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/autolabeller/uninstall.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.171247 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/cluster-logging/
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/cluster-logging/cr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/cluster-logging/kcli_default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/cr.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/install.yml.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.175247 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/istio/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/istio/install.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/istio/istio-cni.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.175247 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/kubernetes-nmstate-operator/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/kubernetes-nmstate-operator/cr.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.175247 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/kubevirt-hyperconverged/
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/kubevirt-hyperconverged/cr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/kubevirt-hyperconverged/kcli_default.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.175247 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/local-storage-operator/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/local-storage-operator/cr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/local-storage-operator/kcli_default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/local-storage-operator/post.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.175247 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/lvms-operator/
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/lvms-operator/cr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/lvms-operator/kcli_default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/lvms-operator/post.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.175247 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/metallb-operator/
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/metallb-operator/cr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/metallb-operator/kcli_default.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.175247 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/multicluster-engine/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/multicluster-engine/99-metal3-provisioning.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/multicluster-engine/assisted-service.sample.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2846 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/multicluster-engine/assisted-service.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/multicluster-engine/cr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/multicluster-engine/gen_registries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/multicluster-engine/kcli_default.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)       55 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/multicluster-engine/post.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.175247 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/nfs/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2297 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/nfs/install.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/nfs/kcli_default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/nfs/uninstall.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.175247 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/odf-operator/
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/odf-operator/cr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/odf-operator/kcli_default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/odf-operator/nad_cluster.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/odf-operator/nad_public.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/odf-operator/post.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/odf-operator/pre.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.179247 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/serverless-operator/
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/serverless-operator/cr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/serverless-operator/kcli_default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/serverless-operator/post.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.179247 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/users/
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/users/install.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/users/kcli_default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/users/oauth.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/users/oauth_hypershift.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/apps/users/uninstall.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/autoapprovercron.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/autorules.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/bootstrap.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/calico.sh.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/chrony.conf
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/cilium.sh.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/cloud_bootstrap.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/cloud_ctlplanes.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/cloud_dns.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/cloud_lb_api.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/cloud_lb_apps.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/cloud_workers.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/cluster-ingress-02-config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/cluster-scheduler-02-config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/config.hcl.templ
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/ctlplanes.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.179247 kcli-99.0.202404131016/kvirt/cluster/openshift/customisation/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/customisation/00-kcli-namespace.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/customisation/97-autoapprovercron-sa.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/customisation/98-autoapprovercron-binding.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/customisation/99-autoapprovercron-cronjob.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/customisation/99-ingress-controller.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/customisation/99-iptables.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/customisation/99-monitoring.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/customisation/99-registry.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/dhcp.conf
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/dhcp.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/dhcp.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.179247 kcli-99.0.202404131016/kvirt/cluster/openshift/disconnected/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.179247 kcli-99.0.202404131016/kvirt/cluster/openshift/disconnected/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      357 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/disconnected/bin/sync_image.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/disconnected/haproxy.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/disconnected/registry.service
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.179247 kcli-99.0.202404131016/kvirt/cluster/openshift/disconnected/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      201 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/disconnected/scripts/01_get_oc.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      243 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/disconnected/scripts/02_packages.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2412 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/disconnected/scripts/03_mirror.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2101 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/disconnected/scripts/03_registry.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      331 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/disconnected/scripts/04_extras.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2349 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/disconnected/scripts/05_olm.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      197 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/disconnected/scripts/06_web.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      841 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/disconnected/scripts/deploy.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/disconnected/scripts/mirror-config.yaml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/disconnected.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     8945 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/fake_kubeconfig.json
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/fake_pull.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/haproxy.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/haproxy.cfg.kubevirt
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/httpd.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/icsp.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/ignition.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/install-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/iso.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/kcli-ipv6.conf.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/kcli_default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/keepalived.conf
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/nonlocalbind.conf
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/openshift-workload-pinning
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/patch_ipv6.json
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/relocate-ip-bootstrap.service
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/relocate-ip-bootstrap.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/relocate-ip.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/sno-finish.service
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/sno-finish.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/sno.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/sno_default.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.179247 kcli-99.0.202404131016/kvirt/cluster/openshift/staticpods/
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/staticpods/coredns.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/staticpods/haproxy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/staticpods/keepalived.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/staticpods/mdns.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/openshift/workers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.183247 kcli-99.0.202404131016/kvirt/cluster/profiles/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/profiles/sample-kubeadm-default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/profiles/sample-openshift-compact.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/profiles/sample-openshift-contrail.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/profiles/sample-openshift-ipv6.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/profiles/sample-openshift-sno-bm.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/profiles/sample-openshift-sno.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/cluster/sampleprovider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.183247 kcli-99.0.202404131016/kvirt/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/common/Jenkinsfile.j2
+-rw-r--r--   0 runner    (1001) docker     (127)   105973 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/common/autoscale.yaml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     8945 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/common/fake_kubeconfig.json
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/common/ignition.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/common/kubevirt_kcli_conf.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/common/local_kcli_conf.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/common/pipeline.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/common/pipeline_kube.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/common/playbook.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/common/storage.sh.aws
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/common/storage.sh.gcp
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/common/storage.sh.ibmcloud
+-rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/common/vm.ovf.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/common/workflow.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/common/workflow_script.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)   191136 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.183247 kcli-99.0.202404131016/kvirt/container/
+-rw-r--r--   0 runner    (1001) docker     (127)    14188 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/containerconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10807 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/defaults.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1475 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/ekstoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25462 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/examples.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.183247 kcli-99.0.202404131016/kvirt/expose/
+-rw-r--r--   0 runner    (1001) docker     (127)    12263 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/expose/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.131247 kcli-99.0.202404131016/kvirt/expose/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.183247 kcli-99.0.202404131016/kvirt/expose/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/expose/static/css/bootstrap-notify.css
+-rw-r--r--   0 runner    (1001) docker     (127)   121125 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/expose/static/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/expose/static/css/dataTables.checkboxes.css
+-rw-r--r--   0 runner    (1001) docker     (127)    13587 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/expose/static/css/jquery.dataTables.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/expose/static/css/kcli.css
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/expose/static/css/wheel.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.187247 kcli-99.0.202404131016/kvirt/expose/static/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/expose/static/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/expose/static/images/sort_asc.png
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/expose/static/images/sort_both.png
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/expose/static/images/sort_desc.png
+-rw-r--r--   0 runner    (1001) docker     (127)    24772 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/expose/static/images/wheel.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.187247 kcli-99.0.202404131016/kvirt/expose/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    12398 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/expose/static/js/dataTables.checkboxes.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/expose/static/js/exposeactions.js
+-rw-r--r--   0 runner    (1001) docker     (127)    83059 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/expose/static/js/jquery.dataTables.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    89795 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/expose/static/js/jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/expose/static/js/list.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4319 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/expose/swagger.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.187247 kcli-99.0.202404131016/kvirt/expose/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/expose/templates/form.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/expose/templates/head.html
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/expose/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/expose/templates/infoplan.html
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/expose/templates/planstable.html
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/expose/templates/result.html
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1047 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/gketoken.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4333 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/ignitionmerger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.187247 kcli-99.0.202404131016/kvirt/internalplans/
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/internalplans/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.187247 kcli-99.0.202404131016/kvirt/jinjafilters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/jinjafilters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6102 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/jinjafilters/jinjafilters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9972 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/keywords.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.187247 kcli-99.0.202404131016/kvirt/kfish/
+-rw-r--r--   0 runner    (1001) docker     (127)    13060 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/kfish/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3395 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/klist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.187247 kcli-99.0.202404131016/kvirt/ksushy/
+-rw-r--r--   0 runner    (1001) docker     (127)    13633 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/ksushy/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      121 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/ksushy/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.187247 kcli-99.0.202404131016/kvirt/ksushy/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/ksushy/templates/bios.json
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/ksushy/templates/interface.json
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/ksushy/templates/interfaces.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/ksushy/templates/manager.json
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/ksushy/templates/managers.json
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/ksushy/templates/root.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/ksushy/templates/system.json
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/ksushy/templates/systems.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/ksushy/templates/virtualmedia_cd.json
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/ksushy/templates/virtualmedias.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.187247 kcli-99.0.202404131016/kvirt/miniconsole/
+-rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/miniconsole/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.187247 kcli-99.0.202404131016/kvirt/nameutils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/nameutils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.191247 kcli-99.0.202404131016/kvirt/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.191247 kcli-99.0.202404131016/kvirt/providers/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)   106425 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/providers/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/providers/aws/assume_policy.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/providers/aws/ctlplane_policy.json
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/providers/aws/worker_policy.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.191247 kcli-99.0.202404131016/kvirt/providers/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)    78530 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/providers/azure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.191247 kcli-99.0.202404131016/kvirt/providers/fake/
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/providers/fake/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.191247 kcli-99.0.202404131016/kvirt/providers/gcp/
+-rw-r--r--   0 runner    (1001) docker     (127)   101005 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/providers/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/providers/gcp/gcp-hack.service
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/providers/gcp/gcp-hack.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.191247 kcli-99.0.202404131016/kvirt/providers/ibm/
+-rw-r--r--   0 runner    (1001) docker     (127)    65793 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/providers/ibm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.191247 kcli-99.0.202404131016/kvirt/providers/kubevirt/
+-rw-r--r--   0 runner    (1001) docker     (127)    86428 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/providers/kubevirt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.191247 kcli-99.0.202404131016/kvirt/providers/kvm/
+-rw-r--r--   0 runner    (1001) docker     (127)   186681 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/providers/kvm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/providers/kvm/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.191247 kcli-99.0.202404131016/kvirt/providers/openstack/
+-rw-r--r--   0 runner    (1001) docker     (127)    58301 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/providers/openstack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.191247 kcli-99.0.202404131016/kvirt/providers/ovirt/
+-rw-r--r--   0 runner    (1001) docker     (127)    63291 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/providers/ovirt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.191247 kcli-99.0.202404131016/kvirt/providers/packet/
+-rw-r--r--   0 runner    (1001) docker     (127)    31823 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/providers/packet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.191247 kcli-99.0.202404131016/kvirt/providers/proxmox/
+-rw-r--r--   0 runner    (1001) docker     (127)    35211 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/providers/proxmox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9555 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/providers/sampleprovider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.191247 kcli-99.0.202404131016/kvirt/providers/vsphere/
+-rw-r--r--   0 runner    (1001) docker     (127)    73908 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/providers/vsphere/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13503 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/providers/vsphere/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4893 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/providers/vsphere/tagging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.191247 kcli-99.0.202404131016/kvirt/providers/web/
+-rw-r--r--   0 runner    (1001) docker     (127)    22043 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/providers/web/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.191247 kcli-99.0.202404131016/kvirt/version/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-13 10:16:46.000000 kcli-99.0.202404131016/kvirt/version/git
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.195247 kcli-99.0.202404131016/kvirt/web/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    46680 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.135247 kcli-99.0.202404131016/kvirt/web/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.195247 kcli-99.0.202404131016/kvirt/web/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/css/bootstrap-notify.css
+-rw-r--r--   0 runner    (1001) docker     (127)    23409 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/css/bootstrap-theme.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   121125 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/css/dataTables.checkboxes.css
+-rw-r--r--   0 runner    (1001) docker     (127)    13587 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/css/jquery.dataTables.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/css/kcli.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/css/navbar.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/css/spice.css
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/css/wheel.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.195247 kcli-99.0.202404131016/kvirt/web/static/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)    18028 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/fonts/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.199247 kcli-99.0.202404131016/kvirt/web/static/images/
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/images/Centos.png
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/images/Debian.png
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/images/Fedora.png
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/images/Redhat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/images/Suse.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/images/Tux.png
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/images/Ubuntu.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4213 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/images/delete.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    23320 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/images/kcli-small.png
+-rw-r--r--   0 runner    (1001) docker     (127)    27185 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/images/kcli.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)   113928 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/images/kcli.png
+-rw-r--r--   0 runner    (1001) docker     (127)    48809 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/images/logo-header.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    48809 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/images/logo-main.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/images/sort_asc.png
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/images/sort_both.png
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/images/sort_desc.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/images/start.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/images/stop.png
+-rw-r--r--   0 runner    (1001) docker     (127)    24772 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/images/wheel.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.199247 kcli-99.0.202404131016/kvirt/web/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/js/bootstrap-notify.js
+-rw-r--r--   0 runner    (1001) docker     (127)    37045 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/js/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/js/containeraction.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12398 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/js/dataTables.checkboxes.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/js/hostaction.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/js/imageaction.js
+-rw-r--r--   0 runner    (1001) docker     (127)    83059 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/js/jquery.dataTables.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    87462 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/js/jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/js/kcli.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/js/kubeaction.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/js/list.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/js/networkaction.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/js/planaction.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/js/poolaction.js
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/js/productaction.js
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/js/refresh.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/js/repoaction.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/js/snapshotaction.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.203247 kcli-99.0.202404131016/kvirt/web/static/js/spice/
+-rw-r--r--   0 runner    (1001) docker     (127)     9944 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/js/spice/atKeynames.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/js/spice/bitmap.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/js/spice/cursor.js
+-rw-r--r--   0 runner    (1001) docker     (127)    49214 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/js/spice/display.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13253 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/js/spice/enums.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/js/spice/filexfer.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9535 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/js/spice/inputs.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6176 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/js/spice/lz.js
+-rw-r--r--   0 runner    (1001) docker     (127)    18370 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/js/spice/main.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12677 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/js/spice/playback.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7036 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/js/spice/png.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/js/spice/port.js
+-rw-r--r--   0 runner    (1001) docker     (127)    44531 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/js/spice/quic.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/js/spice/resize.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7282 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/js/spice/simulatecursor.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/js/spice/spicearraybuffer.js
+-rw-r--r--   0 runner    (1001) docker     (127)    18202 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/js/spice/spiceconn.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/js/spice/spicedataview.js
+-rw-r--r--   0 runner    (1001) docker     (127)    33015 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/js/spice/spicemsg.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12767 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/js/spice/spicetype.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.203247 kcli-99.0.202404131016/kvirt/web/static/js/spice/thirdparty/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.203247 kcli-99.0.202404131016/kvirt/web/static/js/spice/thirdparty/browser-es-module-loader/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/js/spice/thirdparty/browser-es-module-loader/.npmignore
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/js/spice/thirdparty/browser-es-module-loader/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/js/spice/thirdparty/browser-es-module-loader/rollup.config.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.203247 kcli-99.0.202404131016/kvirt/web/static/js/spice/thirdparty/browser-es-module-loader/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/js/spice/thirdparty/browser-es-module-loader/src/babel-worker.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8601 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/js/spice/thirdparty/browser-es-module-loader/src/browser-es-module-loader.js
+-rw-r--r--   0 runner    (1001) docker     (127)    16580 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/js/spice/thirdparty/jsbn.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/js/spice/thirdparty/prng4.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/js/spice/thirdparty/rng.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/js/spice/thirdparty/rsa.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10671 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/js/spice/thirdparty/sha1.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6808 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/js/spice/ticket.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13628 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/js/spice/utils.js
+-rw-r--r--   0 runner    (1001) docker     (127)    21577 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/js/spice/webm.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/js/spice/wire.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/js/vmaction.js
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/js/wheel.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.135247 kcli-99.0.202404131016/kvirt/web/static/vnc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.203247 kcli-99.0.202404131016/kvirt/web/static/vnc/app/
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/app/error-handler.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.207247 kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/alt.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/clipboard.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/connect.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4381 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/ctrl.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3237 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/ctrlaltdel.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5062 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/disconnect.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4684 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/drag.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/error.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/esc.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/expander.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/fullscreen.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/handle.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6386 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/handle_bg.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.211247 kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/icons/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/icons/novnc-120x120.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4582 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/icons/novnc-144x144.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5216 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/icons/novnc-152x152.png
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/icons/novnc-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5787 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/icons/novnc-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/icons/novnc-24x24.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/icons/novnc-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/icons/novnc-48x48.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/icons/novnc-60x60.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/icons/novnc-64x64.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/icons/novnc-72x72.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/icons/novnc-76x76.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/icons/novnc-96x96.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11685 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/icons/novnc-icon-sm.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    11549 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/icons/novnc-icon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/info.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6404 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/keyboard.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7000 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/mouse_left.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7002 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/mouse_middle.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6993 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/mouse_none.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7001 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/mouse_right.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/power.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/settings.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/tab.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/toggleextrakeys.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/warning.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/windows.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.211247 kcli-99.0.202404131016/kvirt/web/static/vnc/app/locale/
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/app/locale/cs.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/app/locale/de.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/app/locale/el.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/app/locale/es.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/app/locale/ja.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/app/locale/ko.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/app/locale/nl.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/app/locale/pl.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/app/locale/ru.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/app/locale/sv.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/app/locale/tr.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/app/locale/zh_CN.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/app/locale/zh_TW.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5682 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/app/localization.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.211247 kcli-99.0.202404131016/kvirt/web/static/vnc/app/sounds/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/app/sounds/CREDITS
+-rw-r--r--   0 runner    (1001) docker     (127)     4531 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/app/sounds/bell.mp3
+-rw-r--r--   0 runner    (1001) docker     (127)     8495 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/app/sounds/bell.oga
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.211247 kcli-99.0.202404131016/kvirt/web/static/vnc/app/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)    38580 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/app/styles/Orbitron700.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    17472 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/app/styles/Orbitron700.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    18450 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/app/styles/base.css
+-rw-r--r--   0 runner    (1001) docker     (127)    56845 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/app/ui.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/app/webutil.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.211247 kcli-99.0.202404131016/kvirt/web/static/vnc/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/core/base64.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.215247 kcli-99.0.202404131016/kvirt/web/static/vnc/core/decoders/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/core/decoders/copyrect.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4814 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/core/decoders/hextile.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/core/decoders/raw.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/core/decoders/rre.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9662 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/core/decoders/tight.js
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/core/decoders/tightpng.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11241 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/core/des.js
+-rw-r--r--   0 runner    (1001) docker     (127)    20381 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/core/display.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/core/encodings.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/core/inflator.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.215247 kcli-99.0.202404131016/kvirt/web/static/vnc/core/input/
+-rw-r--r--   0 runner    (1001) docker     (127)    11438 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/core/input/domkeytable.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/core/input/fixedkeys.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13090 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/core/input/keyboard.js
+-rw-r--r--   0 runner    (1001) docker     (127)    34609 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/core/input/keysym.js
+-rw-r--r--   0 runner    (1001) docker     (127)    25374 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/core/input/keysymdef.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9995 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/core/input/mouse.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/core/input/util.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/core/input/vkeys.js
+-rw-r--r--   0 runner    (1001) docker     (127)    14256 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/core/input/xtscancodes.js
+-rw-r--r--   0 runner    (1001) docker     (127)    74196 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/core/rfb.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.215247 kcli-99.0.202404131016/kvirt/web/static/vnc/core/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/core/util/browser.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7556 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/core/util/cursor.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4221 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/core/util/events.js
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/core/util/eventtarget.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/core/util/logging.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/core/util/polyfill.js
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/core/util/strings.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9130 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/core/websock.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.215247 kcli-99.0.202404131016/kvirt/web/static/vnc/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.215247 kcli-99.0.202404131016/kvirt/web/static/vnc/vendor/browser-es-module-loader/
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/vendor/browser-es-module-loader/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/vendor/browser-es-module-loader/rollup.config.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.215247 kcli-99.0.202404131016/kvirt/web/static/vnc/vendor/browser-es-module-loader/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/vendor/browser-es-module-loader/src/babel-worker.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8498 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/vendor/browser-es-module-loader/src/browser-es-module-loader.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.215247 kcli-99.0.202404131016/kvirt/web/static/vnc/vendor/pako/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/vendor/pako/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/vendor/pako/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.135247 kcli-99.0.202404131016/kvirt/web/static/vnc/vendor/pako/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.215247 kcli-99.0.202404131016/kvirt/web/static/vnc/vendor/pako/lib/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/vendor/pako/lib/utils/common.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.219247 kcli-99.0.202404131016/kvirt/web/static/vnc/vendor/pako/lib/zlib/
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/vendor/pako/lib/zlib/adler32.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/vendor/pako/lib/zlib/constants.js
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/vendor/pako/lib/zlib/crc32.js
+-rw-r--r--   0 runner    (1001) docker     (127)    60016 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/vendor/pako/lib/zlib/deflate.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/vendor/pako/lib/zlib/gzheader.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11690 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/vendor/pako/lib/zlib/inffast.js
+-rw-r--r--   0 runner    (1001) docker     (127)    47128 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/vendor/pako/lib/zlib/inflate.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11527 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/vendor/pako/lib/zlib/inftrees.js
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/vendor/pako/lib/zlib/messages.js
+-rw-r--r--   0 runner    (1001) docker     (127)    38767 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/vendor/pako/lib/zlib/trees.js
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/vendor/pako/lib/zlib/zstream.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7388 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/static/vnc/vendor/promise.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.223247 kcli-99.0.202404131016/kvirt/web/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/templates/bootstrap.html
+-rw-r--r--   0 runner    (1001) docker     (127)    14595 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/templates/console.html
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/templates/containercreate.html
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/templates/containerprofiles.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/templates/containerprofilestable.html
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/templates/containers.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/templates/containerstable.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/templates/head.html
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/templates/hosts.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/templates/hoststable.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/templates/imagecreate.html
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/templates/images.html
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/templates/imagestable.html
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/templates/isos.html
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/templates/isostable.html
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/templates/kubecreate.html
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/templates/kubeinfo.html
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/templates/kubeprofiles.html
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/templates/kubeprofilestable.html
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/templates/kubes.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/templates/kubestable.html
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5517 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/templates/navbar.html
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/templates/networkcreate.html
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/templates/networks.html
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/templates/networkstable.html
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/templates/plancreate.html
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/templates/plans.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/templates/planstable.html
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/templates/poolcreate.html
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/templates/pools.html
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/templates/poolstable.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/templates/productcreate.html
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/templates/products.html
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/templates/productstable.html
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/templates/repocreate.html
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/templates/repos.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/templates/repostable.html
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/templates/vmcreate.html
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/templates/vmprofiles.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/templates/vmprofilestable.html
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/templates/vms.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4894 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/kvirt/web/templates/vmstable.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.223247 kcli-99.0.202404131016/samples/
+-rw-r--r--   0 runner    (1001) docker     (127)     8879 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/samples/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/samples/profiles.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 10:16:47.223247 kcli-99.0.202404131016/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-04-13 10:16:46.000000 kcli-99.0.202404131016/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:16:47.223247 kcli-99.0.202404131016/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-13 10:14:12.000000 kcli-99.0.202404131016/tests/test_kvirt.py
```

### Comparing `kcli-99.0.202404122133/LICENSE` & `kcli-99.0.202404131016/LICENSE`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/MANIFEST.in` & `kcli-99.0.202404131016/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/PKG-INFO` & `kcli-99.0.202404131016/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kcli
-Version: 99.0.202404122133
+Version: 99.0.202404131016
 Summary: Provisioner/Manager for Libvirt/Vsphere/Aws/Gcp/Kubevirt/Ovirt/Openstack/IBM Cloud and containers
 Home-page: http://github.com/karmab/kcli
 Author: Karim Boumedhel
 Author-email: karimboumedhel@gmail.com
 License: ASL
 Platform: UNKNOWN
 Provides-Extra: all
```

### Comparing `kcli-99.0.202404122133/README.md` & `kcli-99.0.202404131016/README.md`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/extras/autoscale.yml` & `kcli-99.0.202404131016/extras/autoscale.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/extras/aws_peering.py` & `kcli-99.0.202404131016/extras/aws_peering.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/extras/aws_peering_cleaning.py` & `kcli-99.0.202404131016/extras/aws_peering_cleaning.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/extras/controller/README.md` & `kcli-99.0.202404131016/extras/controller/README.md`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/extras/controller/crd.yml` & `kcli-99.0.202404131016/extras/controller/crd.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/extras/controller/deploy.yml` & `kcli-99.0.202404131016/extras/controller/deploy.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/extras/controller/examples/plan_complex.yml` & `kcli-99.0.202404131016/extras/controller/examples/plan_complex.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/extras/controller/handlers.py` & `kcli-99.0.202404131016/extras/controller/handlers.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/extras/controller/stress_test.yml` & `kcli-99.0.202404131016/extras/controller/stress_test.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/extras/debian` & `kcli-99.0.202404131016/extras/debian`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/extras/haproxy.cfg` & `kcli-99.0.202404131016/extras/haproxy.cfg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/extras/haproxy_multiple_clusters.cfg` & `kcli-99.0.202404131016/extras/haproxy_multiple_clusters.cfg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/extras/k8sdeploy.yml` & `kcli-99.0.202404131016/extras/k8sdeploy.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/extras/kfish.md` & `kcli-99.0.202404131016/extras/kfish.md`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/extras/kfish.png` & `kcli-99.0.202404131016/extras/kfish.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/extras/openstack.py` & `kcli-99.0.202404131016/extras/openstack.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/extras/openstack.sh.sample` & `kcli-99.0.202404131016/extras/openstack.sh.sample`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/extras/zerotier.service` & `kcli-99.0.202404131016/extras/zerotier.service`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kcli.egg-info/PKG-INFO` & `kcli-99.0.202404131016/kcli.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kcli
-Version: 99.0.202404122133
+Version: 99.0.202404131016
 Summary: Provisioner/Manager for Libvirt/Vsphere/Aws/Gcp/Kubevirt/Ovirt/Openstack/IBM Cloud and containers
 Home-page: http://github.com/karmab/kcli
 Author: Karim Boumedhel
 Author-email: karimboumedhel@gmail.com
 License: ASL
 Platform: UNKNOWN
 Provides-Extra: all
```

### Comparing `kcli-99.0.202404122133/kcli.egg-info/SOURCES.txt` & `kcli-99.0.202404131016/kcli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kcli.egg-info/requires.txt` & `kcli-99.0.202404131016/kcli.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/ansibleutils/__init__.py` & `kcli-99.0.202404131016/kvirt/ansibleutils/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/baseconfig.py` & `kcli-99.0.202404131016/kvirt/baseconfig.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/bottle.py` & `kcli-99.0.202404131016/kvirt/bottle.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cli.py` & `kcli-99.0.202404131016/kvirt/cli.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/aks/__init__.py` & `kcli-99.0.202404131016/kvirt/cluster/aks/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/eks/__init__.py` & `kcli-99.0.202404131016/kvirt/cluster/eks/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/gke/__init__.py` & `kcli-99.0.202404131016/kvirt/cluster/gke/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/hypershift/99-apps.yaml` & `kcli-99.0.202404131016/kvirt/cluster/hypershift/99-apps.yaml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/hypershift/99-forcedns` & `kcli-99.0.202404131016/kvirt/cluster/hypershift/99-forcedns`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/hypershift/99-notifications.yaml` & `kcli-99.0.202404131016/kvirt/cluster/hypershift/99-notifications.yaml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/hypershift/Corefile` & `kcli-99.0.202404131016/kvirt/cluster/hypershift/Corefile`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/hypershift/__init__.py` & `kcli-99.0.202404131016/kvirt/cluster/hypershift/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/hypershift/assisted_infra.yml` & `kcli-99.0.202404131016/kvirt/cluster/hypershift/assisted_infra.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/hypershift/assisted_ingress.yml` & `kcli-99.0.202404131016/kvirt/cluster/hypershift/assisted_ingress.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/hypershift/autoapprovercron.yml` & `kcli-99.0.202404131016/kvirt/cluster/hypershift/autoapprovercron.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/hypershift/bmc.yml.j2` & `kcli-99.0.202404131016/kvirt/cluster/hypershift/bmc.yml.j2`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/hypershift/calico.sh.j2` & `kcli-99.0.202404131016/kvirt/cluster/hypershift/calico.sh.j2`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/hypershift/cilium.sh.j2` & `kcli-99.0.202404131016/kvirt/cluster/hypershift/cilium.sh.j2`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/hypershift/disconnected.sh` & `kcli-99.0.202404131016/kvirt/cluster/hypershift/disconnected.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/hypershift/extras.sh` & `kcli-99.0.202404131016/kvirt/cluster/hypershift/extras.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/hypershift/hostedcluster.yaml` & `kcli-99.0.202404131016/kvirt/cluster/hypershift/hostedcluster.yaml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/hypershift/httpd.yaml` & `kcli-99.0.202404131016/kvirt/cluster/hypershift/httpd.yaml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/hypershift/ignition.sh` & `kcli-99.0.202404131016/kvirt/cluster/hypershift/ignition.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/hypershift/kcli_plan.yml` & `kcli-99.0.202404131016/kvirt/cluster/hypershift/kcli_plan.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/hypershift/kcli_plan_default.yml` & `kcli-99.0.202404131016/kvirt/cluster/hypershift/kcli_plan_default.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/hypershift/nmstateconfig.yml.j2` & `kcli-99.0.202404131016/kvirt/cluster/hypershift/nmstateconfig.yml.j2`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/hypershift/nodepool.yaml` & `kcli-99.0.202404131016/kvirt/cluster/hypershift/nodepool.yaml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/hypershift/staticpods/coredns.yml` & `kcli-99.0.202404131016/kvirt/cluster/hypershift/staticpods/coredns.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/hypershift/staticpods/keepalived.yml` & `kcli-99.0.202404131016/kvirt/cluster/hypershift/staticpods/keepalived.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/hypershift/staticpods/mdns.yml` & `kcli-99.0.202404131016/kvirt/cluster/hypershift/staticpods/mdns.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/k3s/__init__.py` & `kcli-99.0.202404131016/kvirt/cluster/k3s/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/k3s/bootstrap.sh` & `kcli-99.0.202404131016/kvirt/cluster/k3s/bootstrap.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/k3s/bootstrap.yml` & `kcli-99.0.202404131016/kvirt/cluster/k3s/bootstrap.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/k3s/ctlplanes.sh` & `kcli-99.0.202404131016/kvirt/cluster/k3s/ctlplanes.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/k3s/ctlplanes.yml` & `kcli-99.0.202404131016/kvirt/cluster/k3s/ctlplanes.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/k3s/kcli_default.yml` & `kcli-99.0.202404131016/kvirt/cluster/k3s/kcli_default.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/k3s/workers.yml` & `kcli-99.0.202404131016/kvirt/cluster/k3s/workers.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/kubeadm/__init__.py` & `kcli-99.0.202404131016/kvirt/cluster/kubeadm/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/argocd/install.sh` & `kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/argocd/install.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/dashboard/install.sh` & `kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/dashboard/install.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/falco/install.sh` & `kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/falco/install.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/istio/istio-minimal-operator.yaml` & `kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/istio/istio-minimal-operator.yaml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/katacontainer/install.sh` & `kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/katacontainer/install.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/katacontainer/uninstall.sh` & `kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/katacontainer/uninstall.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/kubevirt/install.sh` & `kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/kubevirt/install.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/metallb/install.sh` & `kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/metallb/install.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/metallb/metallb_advertisement.yml` & `kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/metallb/metallb_advertisement.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/rancher/install.sh` & `kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/rancher/install.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/kubeadm/apps/rook/install.sh` & `kcli-99.0.202404131016/kvirt/cluster/kubeadm/apps/rook/install.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/kubeadm/bootstrap.sh` & `kcli-99.0.202404131016/kvirt/cluster/kubeadm/bootstrap.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/kubeadm/bootstrap.yml` & `kcli-99.0.202404131016/kvirt/cluster/kubeadm/bootstrap.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/kubeadm/ctlplanes.yml` & `kcli-99.0.202404131016/kvirt/cluster/kubeadm/ctlplanes.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/kubeadm/join.sh` & `kcli-99.0.202404131016/kvirt/cluster/kubeadm/join.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/kubeadm/kcli_default.yml` & `kcli-99.0.202404131016/kvirt/cluster/kubeadm/kcli_default.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/kubeadm/keepalived.conf` & `kcli-99.0.202404131016/kvirt/cluster/kubeadm/keepalived.conf`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/kubeadm/nfs.sh` & `kcli-99.0.202404131016/kvirt/cluster/kubeadm/nfs.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/kubeadm/pre_el.sh` & `kcli-99.0.202404131016/kvirt/cluster/kubeadm/pre_el.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/kubeadm/pre_ubuntu.sh` & `kcli-99.0.202404131016/kvirt/cluster/kubeadm/pre_ubuntu.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/kubeadm/registry.yml` & `kcli-99.0.202404131016/kvirt/cluster/kubeadm/registry.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/kubeadm/workers.yml` & `kcli-99.0.202404131016/kvirt/cluster/kubeadm/workers.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/kubecommon/__init__.py` & `kcli-99.0.202404131016/kvirt/cluster/kubecommon/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/kubernetes/__init__.py` & `kcli-99.0.202404131016/kvirt/cluster/kubernetes/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/microshift/__init__.py` & `kcli-99.0.202404131016/kvirt/cluster/microshift/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/microshift/kcli_plan.yml` & `kcli-99.0.202404131016/kvirt/cluster/microshift/kcli_plan.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/microshift/kcli_plan_default.yml` & `kcli-99.0.202404131016/kvirt/cluster/microshift/kcli_plan_default.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/microshift/scripts/01_clients.sh` & `kcli-99.0.202404131016/kvirt/cluster/microshift/scripts/01_clients.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/microshift/scripts/03_microshift.sh` & `kcli-99.0.202404131016/kvirt/cluster/microshift/scripts/03_microshift.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/microshift/scripts/05_acm.sh` & `kcli-99.0.202404131016/kvirt/cluster/microshift/scripts/05_acm.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/microshift/scripts/deploy.sh` & `kcli-99.0.202404131016/kvirt/cluster/microshift/scripts/deploy.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/10-node-ip-hint.yaml` & `kcli-99.0.202404131016/kvirt/cluster/openshift/10-node-ip-hint.yaml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/20-localhost-fix.yaml` & `kcli-99.0.202404131016/kvirt/cluster/openshift/20-localhost-fix.yaml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/99-apps.yaml` & `kcli-99.0.202404131016/kvirt/cluster/openshift/99-apps.yaml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/99-autologin.yaml` & `kcli-99.0.202404131016/kvirt/cluster/openshift/99-autologin.yaml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/99-bootstrap-deletion-2.yaml` & `kcli-99.0.202404131016/kvirt/cluster/openshift/99-bootstrap-deletion-2.yaml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/99-bootstrap-deletion.yaml` & `kcli-99.0.202404131016/kvirt/cluster/openshift/99-bootstrap-deletion.yaml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/99-chrony.yaml` & `kcli-99.0.202404131016/kvirt/cluster/openshift/99-chrony.yaml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/99-forcedns` & `kcli-99.0.202404131016/kvirt/cluster/openshift/99-forcedns`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/99-kubevirt-fix.yaml` & `kcli-99.0.202404131016/kvirt/cluster/openshift/99-kubevirt-fix.yaml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/99-notifications.yaml` & `kcli-99.0.202404131016/kvirt/cluster/openshift/99-notifications.yaml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/99-sno.yaml` & `kcli-99.0.202404131016/kvirt/cluster/openshift/99-sno.yaml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/Corefile` & `kcli-99.0.202404131016/kvirt/cluster/openshift/Corefile`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/__init__.py` & `kcli-99.0.202404131016/kvirt/cluster/openshift/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/apps/advanced-cluster-management/assisted-service.sample.yml` & `kcli-99.0.202404131016/kvirt/cluster/openshift/apps/advanced-cluster-management/assisted-service.sample.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/apps/advanced-cluster-management/assisted-service.sh` & `kcli-99.0.202404131016/kvirt/cluster/openshift/apps/advanced-cluster-management/assisted-service.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/apps/advanced-cluster-management/gen_registries.py` & `kcli-99.0.202404131016/kvirt/cluster/openshift/apps/advanced-cluster-management/gen_registries.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/apps/advanced-cluster-management/post.sh` & `kcli-99.0.202404131016/kvirt/cluster/openshift/apps/advanced-cluster-management/post.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/apps/argocd/configmap.yml` & `kcli-99.0.202404131016/kvirt/cluster/openshift/apps/argocd/configmap.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/apps/argocd/install.sh` & `kcli-99.0.202404131016/kvirt/cluster/openshift/apps/argocd/install.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/apps/autolabeller/cr.yml` & `kcli-99.0.202404131016/kvirt/cluster/openshift/apps/autolabeller/cr.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/apps/autolabeller/install.yml` & `kcli-99.0.202404131016/kvirt/cluster/openshift/apps/autolabeller/install.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/apps/cluster-logging/cr.yml` & `kcli-99.0.202404131016/kvirt/cluster/openshift/apps/cluster-logging/cr.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/apps/install.yml.j2` & `kcli-99.0.202404131016/kvirt/cluster/openshift/apps/install.yml.j2`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/apps/kubevirt-hyperconverged/cr.yml` & `kcli-99.0.202404131016/kvirt/cluster/openshift/apps/kubevirt-hyperconverged/cr.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/apps/local-storage-operator/cr.yml` & `kcli-99.0.202404131016/kvirt/cluster/openshift/apps/local-storage-operator/cr.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/apps/local-storage-operator/post.sh` & `kcli-99.0.202404131016/kvirt/cluster/openshift/apps/local-storage-operator/post.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/apps/lvms-operator/cr.yml` & `kcli-99.0.202404131016/kvirt/cluster/openshift/apps/lvms-operator/cr.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/apps/lvms-operator/post.sh` & `kcli-99.0.202404131016/kvirt/cluster/openshift/apps/lvms-operator/post.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/apps/metallb-operator/cr.yml` & `kcli-99.0.202404131016/kvirt/cluster/openshift/apps/metallb-operator/cr.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/apps/multicluster-engine/assisted-service.sample.yml` & `kcli-99.0.202404131016/kvirt/cluster/openshift/apps/multicluster-engine/assisted-service.sample.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/apps/multicluster-engine/assisted-service.sh` & `kcli-99.0.202404131016/kvirt/cluster/openshift/apps/multicluster-engine/assisted-service.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/apps/multicluster-engine/gen_registries.py` & `kcli-99.0.202404131016/kvirt/cluster/openshift/apps/multicluster-engine/gen_registries.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/apps/nfs/install.sh` & `kcli-99.0.202404131016/kvirt/cluster/openshift/apps/nfs/install.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/apps/odf-operator/cr.yml` & `kcli-99.0.202404131016/kvirt/cluster/openshift/apps/odf-operator/cr.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/apps/odf-operator/post.sh` & `kcli-99.0.202404131016/kvirt/cluster/openshift/apps/odf-operator/post.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/apps/odf-operator/pre.sh` & `kcli-99.0.202404131016/kvirt/cluster/openshift/apps/odf-operator/pre.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/apps/users/install.sh` & `kcli-99.0.202404131016/kvirt/cluster/openshift/apps/users/install.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/autoapprovercron.yml` & `kcli-99.0.202404131016/kvirt/cluster/openshift/autoapprovercron.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/autorules.yml` & `kcli-99.0.202404131016/kvirt/cluster/openshift/autorules.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/bootstrap.yml` & `kcli-99.0.202404131016/kvirt/cluster/openshift/bootstrap.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/cilium.sh.j2` & `kcli-99.0.202404131016/kvirt/cluster/openshift/cilium.sh.j2`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/cloud_bootstrap.yml` & `kcli-99.0.202404131016/kvirt/cluster/openshift/cloud_bootstrap.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/cloud_ctlplanes.yml` & `kcli-99.0.202404131016/kvirt/cluster/openshift/cloud_ctlplanes.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/cloud_workers.yml` & `kcli-99.0.202404131016/kvirt/cluster/openshift/cloud_workers.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/ctlplanes.yml` & `kcli-99.0.202404131016/kvirt/cluster/openshift/ctlplanes.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/customisation/99-autoapprovercron-cronjob.yaml` & `kcli-99.0.202404131016/kvirt/cluster/openshift/customisation/99-autoapprovercron-cronjob.yaml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/customisation/99-iptables.yaml` & `kcli-99.0.202404131016/kvirt/cluster/openshift/customisation/99-iptables.yaml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/dhcp.yml` & `kcli-99.0.202404131016/kvirt/cluster/openshift/dhcp.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/disconnected/haproxy.cfg` & `kcli-99.0.202404131016/kvirt/cluster/openshift/disconnected/haproxy.cfg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/disconnected/scripts/03_mirror.sh` & `kcli-99.0.202404131016/kvirt/cluster/openshift/disconnected/scripts/03_mirror.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/disconnected/scripts/03_registry.sh` & `kcli-99.0.202404131016/kvirt/cluster/openshift/disconnected/scripts/03_registry.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/disconnected/scripts/05_olm.sh` & `kcli-99.0.202404131016/kvirt/cluster/openshift/disconnected/scripts/05_olm.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/disconnected/scripts/deploy.sh` & `kcli-99.0.202404131016/kvirt/cluster/openshift/disconnected/scripts/deploy.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/disconnected/scripts/mirror-config.yaml.sample` & `kcli-99.0.202404131016/kvirt/cluster/openshift/disconnected/scripts/mirror-config.yaml.sample`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/disconnected.yml` & `kcli-99.0.202404131016/kvirt/cluster/openshift/disconnected.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/fake_kubeconfig.json` & `kcli-99.0.202404131016/kvirt/cluster/openshift/fake_kubeconfig.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/haproxy.cfg` & `kcli-99.0.202404131016/kvirt/cluster/openshift/haproxy.cfg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/haproxy.cfg.kubevirt` & `kcli-99.0.202404131016/kvirt/cluster/openshift/haproxy.cfg.kubevirt`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/httpd.yaml` & `kcli-99.0.202404131016/kvirt/cluster/openshift/httpd.yaml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/ignition.j2` & `kcli-99.0.202404131016/kvirt/cluster/openshift/ignition.j2`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/install-config.yaml` & `kcli-99.0.202404131016/kvirt/cluster/openshift/install-config.yaml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/iso.sh` & `kcli-99.0.202404131016/kvirt/cluster/openshift/iso.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/kcli_default.yml` & `kcli-99.0.202404131016/kvirt/cluster/openshift/kcli_default.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/keepalived.conf` & `kcli-99.0.202404131016/kvirt/cluster/openshift/keepalived.conf`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/relocate-ip.sh` & `kcli-99.0.202404131016/kvirt/cluster/openshift/relocate-ip.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/sno-finish.sh` & `kcli-99.0.202404131016/kvirt/cluster/openshift/sno-finish.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/sno.yml` & `kcli-99.0.202404131016/kvirt/cluster/openshift/sno.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/sno_default.yml` & `kcli-99.0.202404131016/kvirt/cluster/openshift/sno_default.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/staticpods/coredns.yml` & `kcli-99.0.202404131016/kvirt/cluster/openshift/staticpods/coredns.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/staticpods/haproxy.yml` & `kcli-99.0.202404131016/kvirt/cluster/openshift/staticpods/haproxy.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/staticpods/keepalived.yml` & `kcli-99.0.202404131016/kvirt/cluster/openshift/staticpods/keepalived.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/staticpods/mdns.yml` & `kcli-99.0.202404131016/kvirt/cluster/openshift/staticpods/mdns.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/cluster/openshift/workers.yml` & `kcli-99.0.202404131016/kvirt/cluster/openshift/workers.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/common/Jenkinsfile.j2` & `kcli-99.0.202404131016/kvirt/common/Jenkinsfile.j2`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/common/__init__.py` & `kcli-99.0.202404131016/kvirt/common/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/common/autoscale.yaml.j2` & `kcli-99.0.202404131016/kvirt/common/autoscale.yaml.j2`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/common/fake_kubeconfig.json` & `kcli-99.0.202404131016/kvirt/common/fake_kubeconfig.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/common/ignition.j2` & `kcli-99.0.202404131016/kvirt/common/ignition.j2`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/common/pipeline.yml.j2` & `kcli-99.0.202404131016/kvirt/common/pipeline.yml.j2`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/common/pipeline_kube.yml.j2` & `kcli-99.0.202404131016/kvirt/common/pipeline_kube.yml.j2`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/common/playbook.j2` & `kcli-99.0.202404131016/kvirt/common/playbook.j2`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/common/storage.sh.aws` & `kcli-99.0.202404131016/kvirt/common/storage.sh.aws`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/common/storage.sh.gcp` & `kcli-99.0.202404131016/kvirt/common/storage.sh.gcp`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/common/vm.ovf.j2` & `kcli-99.0.202404131016/kvirt/common/vm.ovf.j2`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/common/workflow.yml.j2` & `kcli-99.0.202404131016/kvirt/common/workflow.yml.j2`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/common/workflow_script.yml.j2` & `kcli-99.0.202404131016/kvirt/common/workflow_script.yml.j2`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/config.py` & `kcli-99.0.202404131016/kvirt/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -8849,3099 +8849,3098 @@
 00022900: 616b 0a20 2020 2020 2020 2073 6c65 6570  ak.        sleep
 00022910: 2835 290a 2020 2020 2020 2020 6f6c 646f  (5).        oldo
 00022920: 7574 7075 7420 3d20 2727 0a20 2020 2020  utput = ''.     
 00022930: 2020 2074 696d 656f 7574 203d 2030 0a20     timeout = 0. 
 00022940: 2020 2020 2020 2077 6869 6c65 2054 7275         while Tru
 00022950: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
 00022960: 7368 636d 6420 3d20 636f 6d6d 6f6e 2e73  shcmd = common.s
-00022970: 7368 286e 616d 652c 2075 7365 723d 2772  sh(name, user='r
-00022980: 6f6f 7427 2c20 6970 3d69 702c 2074 756e  oot', ip=ip, tun
-00022990: 6e65 6c3d 636f 6e66 6967 2e74 756e 6e65  nel=config.tunne
-000229a0: 6c2c 2074 756e 6e65 6c68 6f73 743d 636f  l, tunnelhost=co
-000229b0: 6e66 6967 2e74 756e 6e65 6c68 6f73 742c  nfig.tunnelhost,
-000229c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000229d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000229e0: 2076 6d70 6f72 743d 766d 706f 7274 2c20   vmport=vmport, 
-000229f0: 7475 6e6e 656c 706f 7274 3d63 6f6e 6669  tunnelport=confi
-00022a00: 672e 7475 6e6e 656c 706f 7274 2c20 7475  g.tunnelport, tu
-00022a10: 6e6e 656c 7573 6572 3d63 6f6e 6669 672e  nneluser=config.
-00022a20: 7475 6e6e 656c 7573 6572 2c0a 2020 2020  tunneluser,.    
+00022970: 7368 286e 616d 652c 2075 7365 723d 7573  sh(name, user=us
+00022980: 6572 2c20 6970 3d69 702c 2074 756e 6e65  er, ip=ip, tunne
+00022990: 6c3d 636f 6e66 6967 2e74 756e 6e65 6c2c  l=config.tunnel,
+000229a0: 2074 756e 6e65 6c68 6f73 743d 636f 6e66   tunnelhost=conf
+000229b0: 6967 2e74 756e 6e65 6c68 6f73 742c 0a20  ig.tunnelhost,. 
+000229c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000229d0: 2020 2020 2020 2020 2020 2020 2020 2076                 v
+000229e0: 6d70 6f72 743d 766d 706f 7274 2c20 7475  mport=vmport, tu
+000229f0: 6e6e 656c 706f 7274 3d63 6f6e 6669 672e  nnelport=config.
+00022a00: 7475 6e6e 656c 706f 7274 2c20 7475 6e6e  tunnelport, tunn
+00022a10: 656c 7573 6572 3d63 6f6e 6669 672e 7475  eluser=config.tu
+00022a20: 6e6e 656c 7573 6572 2c0a 2020 2020 2020  nneluser,.      
 00022a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022a40: 2020 2020 2020 2020 2020 2020 696e 7365              inse
-00022a50: 6375 7265 3d63 6f6e 6669 672e 696e 7365  cure=config.inse
-00022a60: 6375 7265 2c20 636d 643d 636d 642c 2069  cure, cmd=cmd, i
-00022a70: 6465 6e74 6974 7966 696c 653d 6964 656e  dentityfile=iden
-00022a80: 7469 7479 6669 6c65 2c20 7061 7373 776f  tityfile, passwo
-00022a90: 7264 3d46 616c 7365 290a 2020 2020 2020  rd=False).      
-00022aa0: 2020 2020 2020 6f75 7470 7574 203d 206f        output = o
-00022ab0: 732e 706f 7065 6e28 7373 6863 6d64 292e  s.popen(sshcmd).
-00022ac0: 7265 6164 2829 0a20 2020 2020 2020 2020  read().         
-00022ad0: 2020 2069 6620 7761 6974 636f 6d6d 616e     if waitcomman
-00022ae0: 6420 6973 206e 6f74 204e 6f6e 653a 0a20  d is not None:. 
-00022af0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00022b00: 6620 6f75 7470 7574 2021 3d20 2727 3a0a  f output != '':.
+00022a40: 2020 2020 2020 2020 2020 696e 7365 6375            insecu
+00022a50: 7265 3d63 6f6e 6669 672e 696e 7365 6375  re=config.insecu
+00022a60: 7265 2c20 636d 643d 636d 642c 2069 6465  re, cmd=cmd, ide
+00022a70: 6e74 6974 7966 696c 653d 6964 656e 7469  ntityfile=identi
+00022a80: 7479 6669 6c65 2c20 7061 7373 776f 7264  tyfile, password
+00022a90: 3d46 616c 7365 290a 2020 2020 2020 2020  =False).        
+00022aa0: 2020 2020 6f75 7470 7574 203d 206f 732e      output = os.
+00022ab0: 706f 7065 6e28 7373 6863 6d64 292e 7265  popen(sshcmd).re
+00022ac0: 6164 2829 0a20 2020 2020 2020 2020 2020  ad().           
+00022ad0: 2069 6620 7761 6974 636f 6d6d 616e 6420   if waitcommand 
+00022ae0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00022af0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00022b00: 6f75 7470 7574 2021 3d20 2727 3a0a 2020  output != '':.  
 00022b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022b20: 2020 2020 7072 696e 7428 6f75 7470 7574      print(output
-00022b30: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00022b40: 2020 2020 2020 6272 6561 6b0a 2020 2020        break.    
-00022b50: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00022b60: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00022b70: 2020 2020 2020 7070 7269 6e74 2822 5761        pprint("Wa
-00022b80: 6974 696e 6720 666f 7220 7761 6974 636f  iting for waitco
-00022b90: 6d6d 616e 6420 746f 2073 7563 6365 6564  mmand to succeed
-00022ba0: 2e2e 2e22 290a 2020 2020 2020 2020 2020  ...").          
-00022bb0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00022bc0: 2020 2020 2020 2020 6966 2027 6b63 6c69          if 'kcli
-00022bd0: 2062 6f6f 7420 6669 6e69 7368 6564 2720   boot finished' 
-00022be0: 696e 206f 7574 7075 7420 6f72 2027 4967  in output or 'Ig
-00022bf0: 6e69 7469 6f6e 2066 696e 6973 6865 6420  nition finished 
-00022c00: 7375 6363 6573 7366 756c 6c79 2720 696e  successfully' in
-00022c10: 206f 7574 7075 7420 6f72 5c0a 2020 2020   output or\.    
-00022c20: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00022c30: 4669 6e69 7368 6564 2043 6f6d 6275 7374  Finished Combust
-00022c40: 696f 6e27 2069 6e20 6f75 7470 7574 3a0a  ion' in output:.
+00022b20: 2020 7072 696e 7428 6f75 7470 7574 290a    print(output).
+00022b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022b40: 2020 2020 6272 6561 6b0a 2020 2020 2020      break.      
+00022b50: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+00022b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022b70: 2020 2020 7070 7269 6e74 2822 5761 6974      pprint("Wait
+00022b80: 696e 6720 666f 7220 7761 6974 636f 6d6d  ing for waitcomm
+00022b90: 616e 6420 746f 2073 7563 6365 6564 2e2e  and to succeed..
+00022ba0: 2e22 290a 2020 2020 2020 2020 2020 2020  .").            
+00022bb0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00022bc0: 2020 2020 2020 6966 2027 6b63 6c69 2062        if 'kcli b
+00022bd0: 6f6f 7420 6669 6e69 7368 6564 2720 696e  oot finished' in
+00022be0: 206f 7574 7075 7420 6f72 2027 4967 6e69   output or 'Igni
+00022bf0: 7469 6f6e 2066 696e 6973 6865 6420 7375  tion finished su
+00022c00: 6363 6573 7366 756c 6c79 2720 696e 206f  ccessfully' in o
+00022c10: 7574 7075 7420 6f72 5c0a 2020 2020 2020  utput or\.      
+00022c20: 2020 2020 2020 2020 2020 2020 2027 4669               'Fi
+00022c30: 6e69 7368 6564 2043 6f6d 6275 7374 696f  nished Combustio
+00022c40: 6e27 2069 6e20 6f75 7470 7574 3a0a 2020  n' in output:.  
 00022c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022c60: 2020 2020 6272 6561 6b0a 2020 2020 2020      break.      
-00022c70: 2020 2020 2020 2020 2020 6f75 7470 7574            output
-00022c80: 203d 206f 7574 7075 742e 7265 706c 6163   = output.replac
-00022c90: 6528 6f6c 646f 7574 7075 742c 2027 2729  e(oldoutput, '')
-00022ca0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00022cb0: 2069 6620 6e6f 7420 7175 6965 743a 0a20   if not quiet:. 
+00022c60: 2020 6272 6561 6b0a 2020 2020 2020 2020    break.        
+00022c70: 2020 2020 2020 2020 6f75 7470 7574 203d          output =
+00022c80: 206f 7574 7075 742e 7265 706c 6163 6528   output.replace(
+00022c90: 6f6c 646f 7574 7075 742c 2027 2729 0a20  oldoutput, ''). 
+00022ca0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00022cb0: 6620 6e6f 7420 7175 6965 743a 0a20 2020  f not quiet:.   
 00022cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022cd0: 2020 2070 7269 6e74 286f 7574 7075 7429     print(output)
-00022ce0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00022cf0: 206f 6c64 6f75 7470 7574 203d 206f 7574   oldoutput = out
-00022d00: 7075 740a 2020 2020 2020 2020 2020 2020  put.            
-00022d10: 736c 6565 7028 3229 0a20 2020 2020 2020  sleep(2).       
-00022d20: 2020 2020 2074 696d 656f 7574 202b 3d20       timeout += 
-00022d30: 320a 2020 2020 2020 2020 2020 2020 6966  2.            if
-00022d40: 2077 6169 7474 696d 656f 7574 203e 2030   waittimeout > 0
-00022d50: 2061 6e64 2074 696d 656f 7574 203e 2077   and timeout > w
-00022d60: 6169 7474 696d 656f 7574 3a0a 2020 2020  aittimeout:.    
-00022d70: 2020 2020 2020 2020 2020 2020 6572 726f              erro
-00022d80: 7228 2254 696d 656f 7574 2077 6169 7469  r("Timeout waiti
-00022d90: 6e67 2066 6f72 2077 6169 7463 6f6d 6d61  ng for waitcomma
-00022da0: 6e64 2074 6f20 6578 6563 7574 652e 2e2e  nd to execute...
-00022db0: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
-00022dc0: 2020 2062 7265 616b 0a20 2020 2020 2020     break.       
-00022dd0: 2072 6574 7572 6e20 5472 7565 0a0a 2020   return True..  
-00022de0: 2020 6465 6620 636c 6561 6e5f 7465 6d70    def clean_temp
-00022df0: 6b65 7928 7365 6c66 2c20 6e61 6d65 2c20  key(self, name, 
-00022e00: 6964 656e 7469 7479 6669 6c65 3d4e 6f6e  identityfile=Non
-00022e10: 6529 3a0a 2020 2020 2020 2020 636d 6420  e):.        cmd 
-00022e20: 3d20 2273 6564 202d 6920 272f 7465 6d70  = "sed -i '/temp
-00022e30: 2d6b 636c 692d 6b65 792f 6427 202f 686f  -kcli-key/d' /ho
-00022e40: 6d65 2f2a 2f2e 7373 682f 6175 7468 6f72  me/*/.ssh/author
-00022e50: 697a 6564 5f6b 6579 7320 2f72 6f6f 742f  ized_keys /root/
-00022e60: 2e73 7368 2f61 7574 686f 7269 7a65 645f  .ssh/authorized_
-00022e70: 6b65 7973 220a 2020 2020 2020 2020 6b20  keys".        k 
-00022e80: 3d20 7365 6c66 2e6b 0a20 2020 2020 2020  = self.k.       
-00022e90: 2069 6e66 6f20 3d20 6b2e 696e 666f 286e   info = k.info(n
-00022ea0: 616d 6529 0a20 2020 2020 2020 2076 6d70  ame).        vmp
-00022eb0: 6f72 7420 3d20 4e6f 6e65 0a20 2020 2020  ort = None.     
-00022ec0: 2020 2069 7020 3d20 696e 666f 2e67 6574     ip = info.get
-00022ed0: 2827 6970 2729 0a20 2020 2020 2020 2069  ('ip').        i
-00022ee0: 6620 7365 6c66 2e74 7970 6520 3d3d 2027  f self.type == '
-00022ef0: 6b75 6265 7669 7274 273a 0a20 2020 2020  kubevirt':.     
-00022f00: 2020 2020 2020 2069 6620 6b2e 6163 6365         if k.acce
-00022f10: 7373 5f6d 6f64 6520 3d3d 2027 4e6f 6465  ss_mode == 'Node
-00022f20: 506f 7274 273a 0a20 2020 2020 2020 2020  Port':.         
-00022f30: 2020 2020 2020 2076 6d70 6f72 7420 3d20         vmport = 
-00022f40: 696e 666f 2e67 6574 2827 6e6f 6465 706f  info.get('nodepo
-00022f50: 7274 2729 0a20 2020 2020 2020 2020 2020  rt').           
-00022f60: 2020 2020 2069 7020 3d20 6b2e 6e6f 6465       ip = k.node
-00022f70: 5f68 6f73 7428 6e61 6d65 3d69 6e66 6f2e  _host(name=info.
-00022f80: 6765 7428 2768 6f73 7427 2929 0a20 2020  get('host')).   
-00022f90: 2020 2020 2020 2020 2065 6c69 6620 6b2e           elif k.
-00022fa0: 6163 6365 7373 5f6d 6f64 6520 3d3d 2027  access_mode == '
-00022fb0: 4c6f 6164 4261 6c61 6e63 6572 273a 0a20  LoadBalancer':. 
-00022fc0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00022fd0: 7020 3d20 696e 666f 2e67 6574 2827 6c6f  p = info.get('lo
-00022fe0: 6164 6261 6c61 6e63 6572 6970 2729 0a20  adbalancerip'). 
-00022ff0: 2020 2020 2020 2073 7368 636d 6420 3d20         sshcmd = 
-00023000: 636f 6d6d 6f6e 2e73 7368 286e 616d 652c  common.ssh(name,
-00023010: 2075 7365 723d 2772 6f6f 7427 2c20 6970   user='root', ip
-00023020: 3d69 702c 2074 756e 6e65 6c3d 7365 6c66  =ip, tunnel=self
-00023030: 2e74 756e 6e65 6c2c 2074 756e 6e65 6c68  .tunnel, tunnelh
-00023040: 6f73 743d 7365 6c66 2e74 756e 6e65 6c68  ost=self.tunnelh
-00023050: 6f73 742c 2076 6d70 6f72 743d 766d 706f  ost, vmport=vmpo
-00023060: 7274 2c0a 2020 2020 2020 2020 2020 2020  rt,.            
-00023070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023080: 7475 6e6e 656c 706f 7274 3d73 656c 662e  tunnelport=self.
-00023090: 7475 6e6e 656c 706f 7274 2c20 7475 6e6e  tunnelport, tunn
-000230a0: 656c 7573 6572 3d73 656c 662e 7475 6e6e  eluser=self.tunn
-000230b0: 656c 7573 6572 2c20 696e 7365 6375 7265  eluser, insecure
-000230c0: 3d73 656c 662e 696e 7365 6375 7265 2c20  =self.insecure, 
-000230d0: 636d 643d 636d 642c 0a20 2020 2020 2020  cmd=cmd,.       
+00022cd0: 2070 7269 6e74 286f 7574 7075 7429 0a20   print(output). 
+00022ce0: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+00022cf0: 6c64 6f75 7470 7574 203d 206f 7574 7075  ldoutput = outpu
+00022d00: 740a 2020 2020 2020 2020 2020 2020 736c  t.            sl
+00022d10: 6565 7028 3229 0a20 2020 2020 2020 2020  eep(2).         
+00022d20: 2020 2074 696d 656f 7574 202b 3d20 320a     timeout += 2.
+00022d30: 2020 2020 2020 2020 2020 2020 6966 2077              if w
+00022d40: 6169 7474 696d 656f 7574 203e 2030 2061  aittimeout > 0 a
+00022d50: 6e64 2074 696d 656f 7574 203e 2077 6169  nd timeout > wai
+00022d60: 7474 696d 656f 7574 3a0a 2020 2020 2020  ttimeout:.      
+00022d70: 2020 2020 2020 2020 2020 6572 726f 7228            error(
+00022d80: 2254 696d 656f 7574 2077 6169 7469 6e67  "Timeout waiting
+00022d90: 2066 6f72 2077 6169 7463 6f6d 6d61 6e64   for waitcommand
+00022da0: 2074 6f20 6578 6563 7574 652e 2e2e 2229   to execute...")
+00022db0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00022dc0: 2062 7265 616b 0a20 2020 2020 2020 2072   break.        r
+00022dd0: 6574 7572 6e20 5472 7565 0a0a 2020 2020  eturn True..    
+00022de0: 6465 6620 636c 6561 6e5f 7465 6d70 6b65  def clean_tempke
+00022df0: 7928 7365 6c66 2c20 6e61 6d65 2c20 6964  y(self, name, id
+00022e00: 656e 7469 7479 6669 6c65 3d4e 6f6e 6529  entityfile=None)
+00022e10: 3a0a 2020 2020 2020 2020 636d 6420 3d20  :.        cmd = 
+00022e20: 2273 6564 202d 6920 272f 7465 6d70 2d6b  "sed -i '/temp-k
+00022e30: 636c 692d 6b65 792f 6427 202f 686f 6d65  cli-key/d' /home
+00022e40: 2f2a 2f2e 7373 682f 6175 7468 6f72 697a  /*/.ssh/authoriz
+00022e50: 6564 5f6b 6579 7320 2f72 6f6f 742f 2e73  ed_keys /root/.s
+00022e60: 7368 2f61 7574 686f 7269 7a65 645f 6b65  sh/authorized_ke
+00022e70: 7973 220a 2020 2020 2020 2020 6b20 3d20  ys".        k = 
+00022e80: 7365 6c66 2e6b 0a20 2020 2020 2020 2069  self.k.        i
+00022e90: 6e66 6f20 3d20 6b2e 696e 666f 286e 616d  nfo = k.info(nam
+00022ea0: 6529 0a20 2020 2020 2020 2076 6d70 6f72  e).        vmpor
+00022eb0: 7420 3d20 4e6f 6e65 0a20 2020 2020 2020  t = None.       
+00022ec0: 2069 7020 3d20 696e 666f 2e67 6574 2827   ip = info.get('
+00022ed0: 6970 2729 0a20 2020 2020 2020 2069 6620  ip').        if 
+00022ee0: 7365 6c66 2e74 7970 6520 3d3d 2027 6b75  self.type == 'ku
+00022ef0: 6265 7669 7274 273a 0a20 2020 2020 2020  bevirt':.       
+00022f00: 2020 2020 2069 6620 6b2e 6163 6365 7373       if k.access
+00022f10: 5f6d 6f64 6520 3d3d 2027 4e6f 6465 506f  _mode == 'NodePo
+00022f20: 7274 273a 0a20 2020 2020 2020 2020 2020  rt':.           
+00022f30: 2020 2020 2076 6d70 6f72 7420 3d20 696e       vmport = in
+00022f40: 666f 2e67 6574 2827 6e6f 6465 706f 7274  fo.get('nodeport
+00022f50: 2729 0a20 2020 2020 2020 2020 2020 2020  ').             
+00022f60: 2020 2069 7020 3d20 6b2e 6e6f 6465 5f68     ip = k.node_h
+00022f70: 6f73 7428 6e61 6d65 3d69 6e66 6f2e 6765  ost(name=info.ge
+00022f80: 7428 2768 6f73 7427 2929 0a20 2020 2020  t('host')).     
+00022f90: 2020 2020 2020 2065 6c69 6620 6b2e 6163         elif k.ac
+00022fa0: 6365 7373 5f6d 6f64 6520 3d3d 2027 4c6f  cess_mode == 'Lo
+00022fb0: 6164 4261 6c61 6e63 6572 273a 0a20 2020  adBalancer':.   
+00022fc0: 2020 2020 2020 2020 2020 2020 2069 7020               ip 
+00022fd0: 3d20 696e 666f 2e67 6574 2827 6c6f 6164  = info.get('load
+00022fe0: 6261 6c61 6e63 6572 6970 2729 0a20 2020  balancerip').   
+00022ff0: 2020 2020 2073 7368 636d 6420 3d20 636f       sshcmd = co
+00023000: 6d6d 6f6e 2e73 7368 286e 616d 652c 2075  mmon.ssh(name, u
+00023010: 7365 723d 2772 6f6f 7427 2c20 6970 3d69  ser='root', ip=i
+00023020: 702c 2074 756e 6e65 6c3d 7365 6c66 2e74  p, tunnel=self.t
+00023030: 756e 6e65 6c2c 2074 756e 6e65 6c68 6f73  unnel, tunnelhos
+00023040: 743d 7365 6c66 2e74 756e 6e65 6c68 6f73  t=self.tunnelhos
+00023050: 742c 2076 6d70 6f72 743d 766d 706f 7274  t, vmport=vmport
+00023060: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00023070: 2020 2020 2020 2020 2020 2020 2020 7475                tu
+00023080: 6e6e 656c 706f 7274 3d73 656c 662e 7475  nnelport=self.tu
+00023090: 6e6e 656c 706f 7274 2c20 7475 6e6e 656c  nnelport, tunnel
+000230a0: 7573 6572 3d73 656c 662e 7475 6e6e 656c  user=self.tunnel
+000230b0: 7573 6572 2c20 696e 7365 6375 7265 3d73  user, insecure=s
+000230c0: 656c 662e 696e 7365 6375 7265 2c20 636d  elf.insecure, cm
+000230d0: 643d 636d 642c 0a20 2020 2020 2020 2020  d=cmd,.         
 000230e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000230f0: 2020 2020 2069 6465 6e74 6974 7966 696c       identityfil
-00023100: 653d 6964 656e 7469 7479 6669 6c65 2c20  e=identityfile, 
-00023110: 7061 7373 776f 7264 3d46 616c 7365 290a  password=False).
-00023120: 2020 2020 2020 2020 6f73 2e70 6f70 656e          os.popen
-00023130: 2873 7368 636d 6429 2e72 6561 6428 290a  (sshcmd).read().
-00023140: 0a20 2020 2064 6566 2074 6872 6561 6465  .    def threade
-00023150: 645f 6372 6561 7465 5f6b 7562 6528 7365  d_create_kube(se
-00023160: 6c66 2c20 636c 7573 7465 722c 206b 7562  lf, cluster, kub
-00023170: 6574 7970 652c 206b 7562 655f 6f76 6572  etype, kube_over
-00023180: 7269 6465 7329 3a0a 2020 2020 2020 2020  rides):.        
-00023190: 6970 706f 6f6c 203d 206b 7562 655f 6f76  ippool = kube_ov
-000231a0: 6572 7269 6465 732e 6765 7428 2769 7070  errides.get('ipp
-000231b0: 6f6f 6c27 2920 6f72 206b 7562 655f 6f76  ool') or kube_ov
-000231c0: 6572 7269 6465 732e 6765 7428 2763 6f6e  errides.get('con
-000231d0: 6670 6f6f 6c27 290a 2020 2020 2020 2020  fpool').        
-000231e0: 6261 7265 6d65 7461 6c70 6f6f 6c20 3d20  baremetalpool = 
-000231f0: 6b75 6265 5f6f 7665 7272 6964 6573 2e67  kube_overrides.g
-00023200: 6574 2827 6970 706f 6f6c 2729 206f 7220  et('ippool') or 
-00023210: 6b75 6265 5f6f 7665 7272 6964 6573 2e67  kube_overrides.g
-00023220: 6574 2827 636f 6e66 706f 6f6c 2729 0a20  et('confpool'). 
-00023230: 2020 2020 2020 2069 6620 6970 706f 6f6c         if ippool
-00023240: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00023250: 2020 2020 2020 2020 2020 7365 6c66 2e67            self.g
-00023260: 6574 5f76 6970 5f66 726f 6d5f 636f 6e66  et_vip_from_conf
-00023270: 706f 6f6c 2863 6c75 7374 6572 2c20 6970  pool(cluster, ip
-00023280: 706f 6f6c 2c20 6f76 6572 7269 6465 733d  pool, overrides=
-00023290: 6b75 6265 5f6f 7665 7272 6964 6573 290a  kube_overrides).
-000232a0: 2020 2020 2020 2020 6966 2062 6172 656d          if barem
-000232b0: 6574 616c 706f 6f6c 2069 7320 6e6f 7420  etalpool is not 
-000232c0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000232d0: 2020 7365 6c66 2e67 6574 5f62 6172 656d    self.get_barem
-000232e0: 6574 616c 5f68 6f73 7473 5f66 726f 6d5f  etal_hosts_from_
-000232f0: 636f 6e66 706f 6f6c 2863 6c75 7374 6572  confpool(cluster
-00023300: 2c20 6261 7265 6d65 7461 6c70 6f6f 6c2c  , baremetalpool,
-00023310: 206f 7665 7272 6964 6573 3d6b 7562 655f   overrides=kube_
-00023320: 6f76 6572 7269 6465 7329 0a20 2020 2020  overrides).     
-00023330: 2020 2073 656c 662e 6372 6561 7465 5f6b     self.create_k
-00023340: 7562 6528 636c 7573 7465 722c 206b 7562  ube(cluster, kub
-00023350: 6574 7970 652c 206b 7562 655f 6f76 6572  etype, kube_over
-00023360: 7269 6465 7329 0a0a 2020 2020 6465 6620  rides)..    def 
-00023370: 6372 6561 7465 5f6b 7562 6528 7365 6c66  create_kube(self
-00023380: 2c20 636c 7573 7465 722c 206b 7562 6574  , cluster, kubet
-00023390: 7970 652c 206f 7665 7272 6964 6573 3d7b  ype, overrides={
-000233a0: 7d29 3a0a 2020 2020 2020 2020 6966 2073  }):.        if s
-000233b0: 656c 662e 7479 7065 203d 3d20 2777 6562  elf.type == 'web
-000233c0: 2720 616e 6420 7365 6c66 2e6b 2e6c 6f63  ' and self.k.loc
-000233d0: 616c 6b75 6265 3a0a 2020 2020 2020 2020  alkube:.        
-000233e0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-000233f0: 6b2e 6372 6561 7465 5f6b 7562 6528 636c  k.create_kube(cl
-00023400: 7573 7465 722c 206b 7562 6574 7970 652c  uster, kubetype,
-00023410: 206f 7665 7272 6964 6573 3d6f 7665 7272   overrides=overr
-00023420: 6964 6573 290a 2020 2020 2020 2020 6970  ides).        ip
-00023430: 706f 6f6c 203d 206f 7665 7272 6964 6573  pool = overrides
-00023440: 2e67 6574 2827 6970 706f 6f6c 2729 206f  .get('ippool') o
-00023450: 7220 6f76 6572 7269 6465 732e 6765 7428  r overrides.get(
-00023460: 2763 6f6e 6670 6f6f 6c27 290a 2020 2020  'confpool').    
-00023470: 2020 2020 6261 7265 6d65 7461 6c70 6f6f      baremetalpoo
-00023480: 6c20 3d20 6f76 6572 7269 6465 732e 6765  l = overrides.ge
-00023490: 7428 2769 7070 6f6f 6c27 2920 6f72 206f  t('ippool') or o
-000234a0: 7665 7272 6964 6573 2e67 6574 2827 636f  verrides.get('co
-000234b0: 6e66 706f 6f6c 2729 0a20 2020 2020 2020  nfpool').       
-000234c0: 2069 6620 6970 706f 6f6c 2069 7320 6e6f   if ippool is no
-000234d0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000234e0: 2020 2020 7365 6c66 2e67 6574 5f76 6970      self.get_vip
-000234f0: 5f66 726f 6d5f 636f 6e66 706f 6f6c 2863  _from_confpool(c
-00023500: 6c75 7374 6572 2c20 6970 706f 6f6c 2c20  luster, ippool, 
-00023510: 6f76 6572 7269 6465 733d 6f76 6572 7269  overrides=overri
-00023520: 6465 7329 0a20 2020 2020 2020 2069 6620  des).        if 
-00023530: 6261 7265 6d65 7461 6c70 6f6f 6c20 6973  baremetalpool is
-00023540: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00023550: 2020 2020 2020 2073 656c 662e 6765 745f         self.get_
-00023560: 6261 7265 6d65 7461 6c5f 686f 7374 735f  baremetal_hosts_
-00023570: 6672 6f6d 5f63 6f6e 6670 6f6f 6c28 636c  from_confpool(cl
-00023580: 7573 7465 722c 2062 6172 656d 6574 616c  uster, baremetal
-00023590: 706f 6f6c 2c20 6f76 6572 7269 6465 733d  pool, overrides=
-000235a0: 6f76 6572 7269 6465 7329 0a20 2020 2020  overrides).     
-000235b0: 2020 2069 6620 6b75 6265 7479 7065 203d     if kubetype =
-000235c0: 3d20 276f 7065 6e73 6869 6674 273a 0a20  = 'openshift':. 
-000235d0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-000235e0: 7420 3d20 7365 6c66 2e63 7265 6174 655f  t = self.create_
-000235f0: 6b75 6265 5f6f 7065 6e73 6869 6674 2863  kube_openshift(c
-00023600: 6c75 7374 6572 2c20 6f76 6572 7269 6465  luster, override
-00023610: 733d 6f76 6572 7269 6465 7329 0a20 2020  s=overrides).   
-00023620: 2020 2020 2065 6c69 6620 6b75 6265 7479       elif kubety
-00023630: 7065 203d 3d20 276f 7065 6e73 6869 6674  pe == 'openshift
-00023640: 2d73 6e6f 273a 0a20 2020 2020 2020 2020  -sno':.         
-00023650: 2020 206f 7665 7272 6964 6573 5b27 736e     overrides['sn
-00023660: 6f27 5d20 3d20 5472 7565 0a20 2020 2020  o'] = True.     
-00023670: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
-00023680: 7365 6c66 2e63 7265 6174 655f 6b75 6265  self.create_kube
-00023690: 5f6f 7065 6e73 6869 6674 2863 6c75 7374  _openshift(clust
-000236a0: 6572 2c20 6f76 6572 7269 6465 733d 6f76  er, overrides=ov
-000236b0: 6572 7269 6465 7329 0a20 2020 2020 2020  errides).       
-000236c0: 2065 6c69 6620 6b75 6265 7479 7065 203d   elif kubetype =
-000236d0: 3d20 2768 7970 6572 7368 6966 7427 3a0a  = 'hypershift':.
-000236e0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-000236f0: 6c74 203d 2073 656c 662e 6372 6561 7465  lt = self.create
-00023700: 5f6b 7562 655f 6879 7065 7273 6869 6674  _kube_hypershift
-00023710: 2863 6c75 7374 6572 2c20 6f76 6572 7269  (cluster, overri
-00023720: 6465 733d 6f76 6572 7269 6465 7329 0a20  des=overrides). 
-00023730: 2020 2020 2020 2065 6c69 6620 6b75 6265         elif kube
-00023740: 7479 7065 203d 3d20 276d 6963 726f 7368  type == 'microsh
-00023750: 6966 7427 3a0a 2020 2020 2020 2020 2020  ift':.          
-00023760: 2020 7265 7375 6c74 203d 2073 656c 662e    result = self.
-00023770: 6372 6561 7465 5f6b 7562 655f 6d69 6372  create_kube_micr
-00023780: 6f73 6869 6674 2863 6c75 7374 6572 2c20  oshift(cluster, 
-00023790: 6f76 6572 7269 6465 733d 6f76 6572 7269  overrides=overri
-000237a0: 6465 7329 0a20 2020 2020 2020 2065 6c69  des).        eli
-000237b0: 6620 6b75 6265 7479 7065 203d 3d20 276b  f kubetype == 'k
-000237c0: 3373 273a 0a20 2020 2020 2020 2020 2020  3s':.           
-000237d0: 2072 6573 756c 7420 3d20 7365 6c66 2e63   result = self.c
-000237e0: 7265 6174 655f 6b75 6265 5f6b 3373 2863  reate_kube_k3s(c
-000237f0: 6c75 7374 6572 2c20 6f76 6572 7269 6465  luster, override
-00023800: 733d 6f76 6572 7269 6465 7329 0a20 2020  s=overrides).   
-00023810: 2020 2020 2065 6c69 6620 6b75 6265 7479       elif kubety
-00023820: 7065 203d 3d20 2767 6b65 273a 0a20 2020  pe == 'gke':.   
-00023830: 2020 2020 2020 2020 2072 6573 756c 7420           result 
-00023840: 3d20 7365 6c66 2e63 7265 6174 655f 6b75  = self.create_ku
-00023850: 6265 5f67 6b65 2863 6c75 7374 6572 2c20  be_gke(cluster, 
-00023860: 6f76 6572 7269 6465 733d 6f76 6572 7269  overrides=overri
-00023870: 6465 7329 0a20 2020 2020 2020 2065 6c69  des).        eli
-00023880: 6620 6b75 6265 7479 7065 203d 3d20 2765  f kubetype == 'e
-00023890: 6b73 273a 0a20 2020 2020 2020 2020 2020  ks':.           
-000238a0: 2072 6573 756c 7420 3d20 7365 6c66 2e63   result = self.c
-000238b0: 7265 6174 655f 6b75 6265 5f65 6b73 2863  reate_kube_eks(c
-000238c0: 6c75 7374 6572 2c20 6f76 6572 7269 6465  luster, override
-000238d0: 733d 6f76 6572 7269 6465 7329 0a20 2020  s=overrides).   
-000238e0: 2020 2020 2065 6c69 6620 6b75 6265 7479       elif kubety
-000238f0: 7065 203d 3d20 2761 6b73 273a 0a20 2020  pe == 'aks':.   
-00023900: 2020 2020 2020 2020 2072 6573 756c 7420           result 
-00023910: 3d20 7365 6c66 2e63 7265 6174 655f 6b75  = self.create_ku
-00023920: 6265 5f61 6b73 2863 6c75 7374 6572 2c20  be_aks(cluster, 
-00023930: 6f76 6572 7269 6465 733d 6f76 6572 7269  overrides=overri
-00023940: 6465 7329 0a20 2020 2020 2020 2065 6c73  des).        els
-00023950: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00023960: 6573 756c 7420 3d20 7365 6c66 2e63 7265  esult = self.cre
-00023970: 6174 655f 6b75 6265 5f67 656e 6572 6963  ate_kube_generic
-00023980: 2863 6c75 7374 6572 2c20 6f76 6572 7269  (cluster, overri
-00023990: 6465 733d 6f76 6572 7269 6465 7329 0a20  des=overrides). 
-000239a0: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-000239b0: 7375 6c74 0a0a 2020 2020 6465 6620 6372  sult..    def cr
-000239c0: 6561 7465 5f6b 7562 655f 616b 7328 7365  eate_kube_aks(se
-000239d0: 6c66 2c20 636c 7573 7465 722c 206f 7665  lf, cluster, ove
-000239e0: 7272 6964 6573 3d7b 7d29 3a0a 2020 2020  rrides={}):.    
-000239f0: 2020 2020 6672 6f6d 206b 7669 7274 2e63      from kvirt.c
-00023a00: 6c75 7374 6572 2069 6d70 6f72 7420 616b  luster import ak
-00023a10: 730a 2020 2020 2020 2020 6966 2063 6f6e  s.        if con
-00023a20: 7461 696e 6572 5f6d 6f64 6528 293a 0a20  tainer_mode():. 
-00023a30: 2020 2020 2020 2020 2020 206f 732e 656e             os.en
-00023a40: 7669 726f 6e5b 2750 4154 4827 5d20 2b3d  viron['PATH'] +=
-00023a50: 2027 3a2f 776f 726b 6469 7227 0a20 2020   ':/workdir'.   
-00023a60: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00023a70: 2020 2020 2020 206f 732e 656e 7669 726f         os.enviro
-00023a80: 6e5b 2750 4154 4827 5d20 2b3d 2027 3a25  n['PATH'] += ':%
-00023a90: 7327 2025 206f 732e 6765 7463 7764 2829  s' % os.getcwd()
-00023aa0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00023ab0: 616b 732e 6372 6561 7465 2873 656c 662c  aks.create(self,
-00023ac0: 2063 6c75 7374 6572 2c20 6f76 6572 7269   cluster, overri
-00023ad0: 6465 7329 0a0a 2020 2020 6465 6620 6372  des)..    def cr
-00023ae0: 6561 7465 5f6b 7562 655f 656b 7328 7365  eate_kube_eks(se
-00023af0: 6c66 2c20 636c 7573 7465 722c 206f 7665  lf, cluster, ove
-00023b00: 7272 6964 6573 3d7b 7d29 3a0a 2020 2020  rrides={}):.    
-00023b10: 2020 2020 6672 6f6d 206b 7669 7274 2e63      from kvirt.c
-00023b20: 6c75 7374 6572 2069 6d70 6f72 7420 656b  luster import ek
-00023b30: 730a 2020 2020 2020 2020 6966 2063 6f6e  s.        if con
-00023b40: 7461 696e 6572 5f6d 6f64 6528 293a 0a20  tainer_mode():. 
-00023b50: 2020 2020 2020 2020 2020 206f 732e 656e             os.en
-00023b60: 7669 726f 6e5b 2750 4154 4827 5d20 2b3d  viron['PATH'] +=
-00023b70: 2027 3a2f 776f 726b 6469 7227 0a20 2020   ':/workdir'.   
-00023b80: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00023b90: 2020 2020 2020 206f 732e 656e 7669 726f         os.enviro
-00023ba0: 6e5b 2750 4154 4827 5d20 2b3d 2027 3a25  n['PATH'] += ':%
-00023bb0: 7327 2025 206f 732e 6765 7463 7764 2829  s' % os.getcwd()
-00023bc0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00023bd0: 656b 732e 6372 6561 7465 2873 656c 662c  eks.create(self,
-00023be0: 2063 6c75 7374 6572 2c20 6f76 6572 7269   cluster, overri
-00023bf0: 6465 7329 0a0a 2020 2020 6465 6620 6372  des)..    def cr
-00023c00: 6561 7465 5f6b 7562 655f 6765 6e65 7269  eate_kube_generi
-00023c10: 6328 7365 6c66 2c20 636c 7573 7465 722c  c(self, cluster,
-00023c20: 206f 7665 7272 6964 6573 3d7b 7d29 3a0a   overrides={}):.
-00023c30: 2020 2020 2020 2020 6966 2063 6f6e 7461          if conta
-00023c40: 696e 6572 5f6d 6f64 6528 293a 0a20 2020  iner_mode():.   
-00023c50: 2020 2020 2020 2020 206f 732e 656e 7669           os.envi
-00023c60: 726f 6e5b 2750 4154 4827 5d20 2b3d 2027  ron['PATH'] += '
-00023c70: 3a2f 776f 726b 6469 7227 0a20 2020 2020  :/workdir'.     
-00023c80: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00023c90: 2020 2020 206f 732e 656e 7669 726f 6e5b       os.environ[
-00023ca0: 2750 4154 4827 5d20 2b3d 2027 3a25 7327  'PATH'] += ':%s'
-00023cb0: 2025 206f 732e 6765 7463 7764 2829 0a20   % os.getcwd(). 
-00023cc0: 2020 2020 2020 2070 6c61 6e64 6972 203d         plandir =
-00023cd0: 206f 732e 7061 7468 2e64 6972 6e61 6d65   os.path.dirname
-00023ce0: 286b 7562 6561 646d 2e63 7265 6174 652e  (kubeadm.create.
-00023cf0: 5f5f 636f 6465 5f5f 2e63 6f5f 6669 6c65  __code__.co_file
-00023d00: 6e61 6d65 290a 2020 2020 2020 2020 7265  name).        re
-00023d10: 7475 726e 206b 7562 6561 646d 2e63 7265  turn kubeadm.cre
-00023d20: 6174 6528 7365 6c66 2c20 706c 616e 6469  ate(self, plandi
-00023d30: 722c 2063 6c75 7374 6572 2c20 6f76 6572  r, cluster, over
-00023d40: 7269 6465 7329 0a0a 2020 2020 6465 6620  rides)..    def 
-00023d50: 6372 6561 7465 5f6b 7562 655f 676b 6528  create_kube_gke(
-00023d60: 7365 6c66 2c20 636c 7573 7465 722c 206f  self, cluster, o
-00023d70: 7665 7272 6964 6573 3d7b 7d29 3a0a 2020  verrides={}):.  
-00023d80: 2020 2020 2020 6672 6f6d 206b 7669 7274        from kvirt
-00023d90: 2e63 6c75 7374 6572 2069 6d70 6f72 7420  .cluster import 
-00023da0: 676b 650a 2020 2020 2020 2020 6966 2063  gke.        if c
-00023db0: 6f6e 7461 696e 6572 5f6d 6f64 6528 293a  ontainer_mode():
-00023dc0: 0a20 2020 2020 2020 2020 2020 206f 732e  .            os.
-00023dd0: 656e 7669 726f 6e5b 2750 4154 4827 5d20  environ['PATH'] 
-00023de0: 2b3d 2027 3a2f 776f 726b 6469 7227 0a20  += ':/workdir'. 
-00023df0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00023e00: 2020 2020 2020 2020 206f 732e 656e 7669           os.envi
-00023e10: 726f 6e5b 2750 4154 4827 5d20 2b3d 2027  ron['PATH'] += '
-00023e20: 3a25 7327 2025 206f 732e 6765 7463 7764  :%s' % os.getcwd
-00023e30: 2829 0a20 2020 2020 2020 2072 6574 7572  ().        retur
-00023e40: 6e20 676b 652e 6372 6561 7465 2873 656c  n gke.create(sel
-00023e50: 662c 2063 6c75 7374 6572 2c20 6f76 6572  f, cluster, over
-00023e60: 7269 6465 7329 0a0a 2020 2020 6465 6620  rides)..    def 
-00023e70: 6372 6561 7465 5f6b 7562 655f 6d69 6372  create_kube_micr
-00023e80: 6f73 6869 6674 2873 656c 662c 2063 6c75  oshift(self, clu
-00023e90: 7374 6572 2c20 6f76 6572 7269 6465 733d  ster, overrides=
-00023ea0: 7b7d 293a 0a20 2020 2020 2020 2069 6620  {}):.        if 
-00023eb0: 636f 6e74 6169 6e65 725f 6d6f 6465 2829  container_mode()
-00023ec0: 3a0a 2020 2020 2020 2020 2020 2020 6f73  :.            os
-00023ed0: 2e65 6e76 6972 6f6e 5b27 5041 5448 275d  .environ['PATH']
-00023ee0: 202b 3d20 273a 2f77 6f72 6b64 6972 270a   += ':/workdir'.
-00023ef0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00023f00: 2020 2020 2020 2020 2020 6f73 2e65 6e76            os.env
-00023f10: 6972 6f6e 5b27 5041 5448 275d 202b 3d20  iron['PATH'] += 
-00023f20: 273a 2573 2720 2520 6f73 2e67 6574 6377  ':%s' % os.getcw
-00023f30: 6428 290a 2020 2020 2020 2020 706c 616e  d().        plan
-00023f40: 6469 7220 3d20 6f73 2e70 6174 682e 6469  dir = os.path.di
-00023f50: 726e 616d 6528 6d69 6372 6f73 6869 6674  rname(microshift
-00023f60: 2e63 7265 6174 652e 5f5f 636f 6465 5f5f  .create.__code__
-00023f70: 2e63 6f5f 6669 6c65 6e61 6d65 290a 2020  .co_filename).  
-00023f80: 2020 2020 2020 7265 7475 726e 206d 6963        return mic
-00023f90: 726f 7368 6966 742e 6372 6561 7465 2873  roshift.create(s
-00023fa0: 656c 662c 2070 6c61 6e64 6972 2c20 636c  elf, plandir, cl
-00023fb0: 7573 7465 722c 206f 7665 7272 6964 6573  uster, overrides
-00023fc0: 290a 0a20 2020 2064 6566 2063 7265 6174  )..    def creat
-00023fd0: 655f 6b75 6265 5f6b 3373 2873 656c 662c  e_kube_k3s(self,
-00023fe0: 2063 6c75 7374 6572 2c20 6f76 6572 7269   cluster, overri
-00023ff0: 6465 733d 7b7d 293a 0a20 2020 2020 2020  des={}):.       
-00024000: 2069 6620 636f 6e74 6169 6e65 725f 6d6f   if container_mo
-00024010: 6465 2829 3a0a 2020 2020 2020 2020 2020  de():.          
-00024020: 2020 6f73 2e65 6e76 6972 6f6e 5b27 5041    os.environ['PA
-00024030: 5448 275d 202b 3d20 273a 2f77 6f72 6b64  TH'] += ':/workd
-00024040: 6972 270a 2020 2020 2020 2020 656c 7365  ir'.        else
-00024050: 3a0a 2020 2020 2020 2020 2020 2020 6f73  :.            os
-00024060: 2e65 6e76 6972 6f6e 5b27 5041 5448 275d  .environ['PATH']
-00024070: 202b 3d20 273a 2573 2720 2520 6f73 2e67   += ':%s' % os.g
-00024080: 6574 6377 6428 290a 2020 2020 2020 2020  etcwd().        
-00024090: 706c 616e 6469 7220 3d20 6f73 2e70 6174  plandir = os.pat
-000240a0: 682e 6469 726e 616d 6528 6b33 732e 6372  h.dirname(k3s.cr
-000240b0: 6561 7465 2e5f 5f63 6f64 655f 5f2e 636f  eate.__code__.co
-000240c0: 5f66 696c 656e 616d 6529 0a20 2020 2020  _filename).     
-000240d0: 2020 2072 6574 7572 6e20 6b33 732e 6372     return k3s.cr
-000240e0: 6561 7465 2873 656c 662c 2070 6c61 6e64  eate(self, pland
-000240f0: 6972 2c20 636c 7573 7465 722c 206f 7665  ir, cluster, ove
-00024100: 7272 6964 6573 290a 0a20 2020 2064 6566  rrides)..    def
-00024110: 2063 7265 6174 655f 6b75 6265 5f68 7970   create_kube_hyp
-00024120: 6572 7368 6966 7428 7365 6c66 2c20 636c  ershift(self, cl
-00024130: 7573 7465 722c 206f 7665 7272 6964 6573  uster, overrides
-00024140: 3d7b 7d29 3a0a 2020 2020 2020 2020 6966  ={}):.        if
-00024150: 2063 6f6e 7461 696e 6572 5f6d 6f64 6528   container_mode(
-00024160: 293a 0a20 2020 2020 2020 2020 2020 206f  ):.            o
-00024170: 732e 656e 7669 726f 6e5b 2750 4154 4827  s.environ['PATH'
-00024180: 5d20 2b3d 2027 3a2f 776f 726b 6469 7227  ] += ':/workdir'
-00024190: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-000241a0: 2020 2020 2020 2020 2020 206f 732e 656e             os.en
-000241b0: 7669 726f 6e5b 2750 4154 4827 5d20 2b3d  viron['PATH'] +=
-000241c0: 2027 3a25 7327 2025 206f 732e 6765 7463   ':%s' % os.getc
-000241d0: 7764 2829 0a20 2020 2020 2020 2070 6c61  wd().        pla
-000241e0: 6e64 6972 203d 206f 732e 7061 7468 2e64  ndir = os.path.d
-000241f0: 6972 6e61 6d65 2868 7970 6572 7368 6966  irname(hypershif
-00024200: 742e 6372 6561 7465 2e5f 5f63 6f64 655f  t.create.__code_
-00024210: 5f2e 636f 5f66 696c 656e 616d 6529 0a20  _.co_filename). 
-00024220: 2020 2020 2020 2023 2064 6e73 636c 6965         # dnsclie
-00024230: 6e74 203d 206f 7665 7272 6964 6573 2e67  nt = overrides.g
-00024240: 6574 2827 646e 7363 6c69 656e 7427 290a  et('dnsclient').
-00024250: 2020 2020 2020 2020 2320 646e 7363 6f6e          # dnscon
-00024260: 6669 6720 3d20 4b63 6f6e 6669 6728 636c  fig = Kconfig(cl
-00024270: 6965 6e74 3d64 6e73 636c 6965 6e74 2920  ient=dnsclient) 
-00024280: 6966 2064 6e73 636c 6965 6e74 2069 7320  if dnsclient is 
-00024290: 6e6f 7420 4e6f 6e65 2065 6c73 6520 4e6f  not None else No
-000242a0: 6e65 0a20 2020 2020 2020 2072 6574 7572  ne.        retur
-000242b0: 6e20 6879 7065 7273 6869 6674 2e63 7265  n hypershift.cre
-000242c0: 6174 6528 7365 6c66 2c20 706c 616e 6469  ate(self, plandi
-000242d0: 722c 2063 6c75 7374 6572 2c20 6f76 6572  r, cluster, over
-000242e0: 7269 6465 7329 0a0a 2020 2020 6465 6620  rides)..    def 
-000242f0: 6372 6561 7465 5f6b 7562 655f 6f70 656e  create_kube_open
-00024300: 7368 6966 7428 7365 6c66 2c20 636c 7573  shift(self, clus
-00024310: 7465 722c 206f 7665 7272 6964 6573 3d7b  ter, overrides={
-00024320: 7d29 3a0a 2020 2020 2020 2020 6966 2063  }):.        if c
-00024330: 6f6e 7461 696e 6572 5f6d 6f64 6528 293a  ontainer_mode():
-00024340: 0a20 2020 2020 2020 2020 2020 206f 732e  .            os.
-00024350: 656e 7669 726f 6e5b 2750 4154 4827 5d20  environ['PATH'] 
-00024360: 2b3d 2027 3a2f 776f 726b 6469 7227 0a20  += ':/workdir'. 
-00024370: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00024380: 2020 2020 2020 2020 206f 732e 656e 7669           os.envi
-00024390: 726f 6e5b 2750 4154 4827 5d20 2b3d 2027  ron['PATH'] += '
-000243a0: 3a25 7327 2025 206f 732e 6765 7463 7764  :%s' % os.getcwd
-000243b0: 2829 0a20 2020 2020 2020 2070 6c61 6e64  ().        pland
-000243c0: 6972 203d 206f 732e 7061 7468 2e64 6972  ir = os.path.dir
-000243d0: 6e61 6d65 286f 7065 6e73 6869 6674 2e63  name(openshift.c
-000243e0: 7265 6174 652e 5f5f 636f 6465 5f5f 2e63  reate.__code__.c
-000243f0: 6f5f 6669 6c65 6e61 6d65 290a 2020 2020  o_filename).    
-00024400: 2020 2020 646e 7363 6c69 656e 7420 3d20      dnsclient = 
-00024410: 6f76 6572 7269 6465 732e 6765 7428 2764  overrides.get('d
-00024420: 6e73 636c 6965 6e74 2729 0a20 2020 2020  nsclient').     
-00024430: 2020 2064 6e73 636f 6e66 6967 203d 204b     dnsconfig = K
-00024440: 636f 6e66 6967 2863 6c69 656e 743d 646e  config(client=dn
-00024450: 7363 6c69 656e 7429 2069 6620 646e 7363  sclient) if dnsc
-00024460: 6c69 656e 7420 6973 206e 6f74 204e 6f6e  lient is not Non
-00024470: 6520 656c 7365 204e 6f6e 650a 2020 2020  e else None.    
-00024480: 2020 2020 7265 7475 726e 206f 7065 6e73      return opens
-00024490: 6869 6674 2e63 7265 6174 6528 7365 6c66  hift.create(self
-000244a0: 2c20 706c 616e 6469 722c 2063 6c75 7374  , plandir, clust
-000244b0: 6572 2c20 6f76 6572 7269 6465 732c 2064  er, overrides, d
-000244c0: 6e73 636f 6e66 6967 3d64 6e73 636f 6e66  nsconfig=dnsconf
-000244d0: 6967 290a 0a20 2020 2064 6566 2064 656c  ig)..    def del
-000244e0: 6574 655f 6b75 6265 2873 656c 662c 2063  ete_kube(self, c
-000244f0: 6c75 7374 6572 2c20 6f76 6572 7269 6465  luster, override
-00024500: 733d 7b7d 293a 0a20 2020 2020 2020 206b  s={}):.        k
-00024510: 203d 2073 656c 662e 6b0a 2020 2020 2020   = self.k.      
-00024520: 2020 6879 7065 7273 6869 6674 203d 206f    hypershift = o
-00024530: 7665 7272 6964 6573 2e67 6574 2827 6b75  verrides.get('ku
-00024540: 6265 7479 7065 272c 2027 7878 7827 2920  betype', 'xxx') 
-00024550: 3d3d 2027 6879 7065 7273 6869 6674 270a  == 'hypershift'.
-00024560: 2020 2020 2020 2020 6173 7369 7374 6564          assisted
-00024570: 203d 2046 616c 7365 0a20 2020 2020 2020   = False.       
-00024580: 2061 6b73 203d 206f 7665 7272 6964 6573   aks = overrides
-00024590: 2e67 6574 2827 6b75 6265 7479 7065 272c  .get('kubetype',
-000245a0: 2027 7878 7827 2920 3d3d 2027 616b 7327   'xxx') == 'aks'
-000245b0: 0a20 2020 2020 2020 2065 6b73 203d 206f  .        eks = o
-000245c0: 7665 7272 6964 6573 2e67 6574 2827 6b75  verrides.get('ku
-000245d0: 6265 7479 7065 272c 2027 7878 7827 2920  betype', 'xxx') 
-000245e0: 3d3d 2027 656b 7327 0a20 2020 2020 2020  == 'eks'.       
-000245f0: 2067 6b65 203d 206f 7665 7272 6964 6573   gke = overrides
-00024600: 2e67 6574 2827 6b75 6265 7479 7065 272c  .get('kubetype',
-00024610: 2027 7878 7827 2920 3d3d 2027 676b 6527   'xxx') == 'gke'
-00024620: 0a20 2020 2020 2020 2064 6f6d 6169 6e20  .        domain 
-00024630: 3d20 6f76 6572 7269 6465 732e 6765 7428  = overrides.get(
-00024640: 2764 6f6d 6169 6e27 2c20 276b 6172 6d61  'domain', 'karma
-00024650: 6c61 6273 2e63 6f72 7027 290a 2020 2020  labs.corp').    
-00024660: 2020 2020 6b75 6265 7479 7065 203d 206f      kubetype = o
-00024670: 7665 7272 6964 6573 2e67 6574 2827 6b75  verrides.get('ku
-00024680: 6265 7479 7065 272c 2027 6765 6e65 7269  betype', 'generi
-00024690: 6327 290a 2020 2020 2020 2020 646e 7363  c').        dnsc
-000246a0: 6c69 656e 7420 3d20 4e6f 6e65 0a20 2020  lient = None.   
-000246b0: 2020 2020 2069 6620 7365 6c66 2e74 7970       if self.typ
-000246c0: 6520 3d3d 2027 7765 6227 2061 6e64 206b  e == 'web' and k
-000246d0: 2e6c 6f63 616c 6b75 6265 3a0a 2020 2020  .localkube:.    
-000246e0: 2020 2020 2020 2020 7265 7475 726e 206b          return k
-000246f0: 2e64 656c 6574 655f 6b75 6265 2863 6c75  .delete_kube(clu
-00024700: 7374 6572 2c20 6b75 6265 7479 7065 2c20  ster, kubetype, 
-00024710: 6f76 6572 7269 6465 733d 6f76 6572 7269  overrides=overri
-00024720: 6465 7329 0a20 2020 2020 2020 2063 6c75  des).        clu
-00024730: 7374 6572 203d 206f 7665 7272 6964 6573  ster = overrides
-00024740: 2e67 6574 2827 636c 7573 7465 7227 2c20  .get('cluster', 
-00024750: 636c 7573 7465 7229 0a20 2020 2020 2020  cluster).       
-00024760: 2069 6620 636c 7573 7465 7220 6973 204e   if cluster is N
-00024770: 6f6e 6520 6f72 2063 6c75 7374 6572 203d  one or cluster =
-00024780: 3d20 2727 3a0a 2020 2020 2020 2020 2020  = '':.          
-00024790: 2020 6465 6661 756c 745f 636c 7573 7465    default_cluste
-000247a0: 7273 203d 207b 2767 656e 6572 6963 273a  rs = {'generic':
-000247b0: 2027 6d79 6b75 6265 272c 2027 6879 7065   'mykube', 'hype
-000247c0: 7273 6869 6674 273a 2027 6d79 6879 7065  rshift': 'myhype
-000247d0: 7273 6869 6674 272c 2027 6f70 656e 7368  rshift', 'opensh
-000247e0: 6966 7427 3a20 276d 796f 7065 6e73 6869  ift': 'myopenshi
-000247f0: 6674 272c 0a20 2020 2020 2020 2020 2020  ft',.           
+000230f0: 2020 2069 6465 6e74 6974 7966 696c 653d     identityfile=
+00023100: 6964 656e 7469 7479 6669 6c65 2c20 7061  identityfile, pa
+00023110: 7373 776f 7264 3d46 616c 7365 290a 2020  ssword=False).  
+00023120: 2020 2020 2020 6f73 2e70 6f70 656e 2873        os.popen(s
+00023130: 7368 636d 6429 2e72 6561 6428 290a 0a20  shcmd).read().. 
+00023140: 2020 2064 6566 2074 6872 6561 6465 645f     def threaded_
+00023150: 6372 6561 7465 5f6b 7562 6528 7365 6c66  create_kube(self
+00023160: 2c20 636c 7573 7465 722c 206b 7562 6574  , cluster, kubet
+00023170: 7970 652c 206b 7562 655f 6f76 6572 7269  ype, kube_overri
+00023180: 6465 7329 3a0a 2020 2020 2020 2020 6970  des):.        ip
+00023190: 706f 6f6c 203d 206b 7562 655f 6f76 6572  pool = kube_over
+000231a0: 7269 6465 732e 6765 7428 2769 7070 6f6f  rides.get('ippoo
+000231b0: 6c27 2920 6f72 206b 7562 655f 6f76 6572  l') or kube_over
+000231c0: 7269 6465 732e 6765 7428 2763 6f6e 6670  rides.get('confp
+000231d0: 6f6f 6c27 290a 2020 2020 2020 2020 6261  ool').        ba
+000231e0: 7265 6d65 7461 6c70 6f6f 6c20 3d20 6b75  remetalpool = ku
+000231f0: 6265 5f6f 7665 7272 6964 6573 2e67 6574  be_overrides.get
+00023200: 2827 6970 706f 6f6c 2729 206f 7220 6b75  ('ippool') or ku
+00023210: 6265 5f6f 7665 7272 6964 6573 2e67 6574  be_overrides.get
+00023220: 2827 636f 6e66 706f 6f6c 2729 0a20 2020  ('confpool').   
+00023230: 2020 2020 2069 6620 6970 706f 6f6c 2069       if ippool i
+00023240: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00023250: 2020 2020 2020 2020 7365 6c66 2e67 6574          self.get
+00023260: 5f76 6970 5f66 726f 6d5f 636f 6e66 706f  _vip_from_confpo
+00023270: 6f6c 2863 6c75 7374 6572 2c20 6970 706f  ol(cluster, ippo
+00023280: 6f6c 2c20 6f76 6572 7269 6465 733d 6b75  ol, overrides=ku
+00023290: 6265 5f6f 7665 7272 6964 6573 290a 2020  be_overrides).  
+000232a0: 2020 2020 2020 6966 2062 6172 656d 6574        if baremet
+000232b0: 616c 706f 6f6c 2069 7320 6e6f 7420 4e6f  alpool is not No
+000232c0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000232d0: 7365 6c66 2e67 6574 5f62 6172 656d 6574  self.get_baremet
+000232e0: 616c 5f68 6f73 7473 5f66 726f 6d5f 636f  al_hosts_from_co
+000232f0: 6e66 706f 6f6c 2863 6c75 7374 6572 2c20  nfpool(cluster, 
+00023300: 6261 7265 6d65 7461 6c70 6f6f 6c2c 206f  baremetalpool, o
+00023310: 7665 7272 6964 6573 3d6b 7562 655f 6f76  verrides=kube_ov
+00023320: 6572 7269 6465 7329 0a20 2020 2020 2020  errides).       
+00023330: 2073 656c 662e 6372 6561 7465 5f6b 7562   self.create_kub
+00023340: 6528 636c 7573 7465 722c 206b 7562 6574  e(cluster, kubet
+00023350: 7970 652c 206b 7562 655f 6f76 6572 7269  ype, kube_overri
+00023360: 6465 7329 0a0a 2020 2020 6465 6620 6372  des)..    def cr
+00023370: 6561 7465 5f6b 7562 6528 7365 6c66 2c20  eate_kube(self, 
+00023380: 636c 7573 7465 722c 206b 7562 6574 7970  cluster, kubetyp
+00023390: 652c 206f 7665 7272 6964 6573 3d7b 7d29  e, overrides={})
+000233a0: 3a0a 2020 2020 2020 2020 6966 2073 656c  :.        if sel
+000233b0: 662e 7479 7065 203d 3d20 2777 6562 2720  f.type == 'web' 
+000233c0: 616e 6420 7365 6c66 2e6b 2e6c 6f63 616c  and self.k.local
+000233d0: 6b75 6265 3a0a 2020 2020 2020 2020 2020  kube:.          
+000233e0: 2020 7265 7475 726e 2073 656c 662e 6b2e    return self.k.
+000233f0: 6372 6561 7465 5f6b 7562 6528 636c 7573  create_kube(clus
+00023400: 7465 722c 206b 7562 6574 7970 652c 206f  ter, kubetype, o
+00023410: 7665 7272 6964 6573 3d6f 7665 7272 6964  verrides=overrid
+00023420: 6573 290a 2020 2020 2020 2020 6970 706f  es).        ippo
+00023430: 6f6c 203d 206f 7665 7272 6964 6573 2e67  ol = overrides.g
+00023440: 6574 2827 6970 706f 6f6c 2729 206f 7220  et('ippool') or 
+00023450: 6f76 6572 7269 6465 732e 6765 7428 2763  overrides.get('c
+00023460: 6f6e 6670 6f6f 6c27 290a 2020 2020 2020  onfpool').      
+00023470: 2020 6261 7265 6d65 7461 6c70 6f6f 6c20    baremetalpool 
+00023480: 3d20 6f76 6572 7269 6465 732e 6765 7428  = overrides.get(
+00023490: 2769 7070 6f6f 6c27 2920 6f72 206f 7665  'ippool') or ove
+000234a0: 7272 6964 6573 2e67 6574 2827 636f 6e66  rrides.get('conf
+000234b0: 706f 6f6c 2729 0a20 2020 2020 2020 2069  pool').        i
+000234c0: 6620 6970 706f 6f6c 2069 7320 6e6f 7420  f ippool is not 
+000234d0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000234e0: 2020 7365 6c66 2e67 6574 5f76 6970 5f66    self.get_vip_f
+000234f0: 726f 6d5f 636f 6e66 706f 6f6c 2863 6c75  rom_confpool(clu
+00023500: 7374 6572 2c20 6970 706f 6f6c 2c20 6f76  ster, ippool, ov
+00023510: 6572 7269 6465 733d 6f76 6572 7269 6465  errides=override
+00023520: 7329 0a20 2020 2020 2020 2069 6620 6261  s).        if ba
+00023530: 7265 6d65 7461 6c70 6f6f 6c20 6973 206e  remetalpool is n
+00023540: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00023550: 2020 2020 2073 656c 662e 6765 745f 6261       self.get_ba
+00023560: 7265 6d65 7461 6c5f 686f 7374 735f 6672  remetal_hosts_fr
+00023570: 6f6d 5f63 6f6e 6670 6f6f 6c28 636c 7573  om_confpool(clus
+00023580: 7465 722c 2062 6172 656d 6574 616c 706f  ter, baremetalpo
+00023590: 6f6c 2c20 6f76 6572 7269 6465 733d 6f76  ol, overrides=ov
+000235a0: 6572 7269 6465 7329 0a20 2020 2020 2020  errides).       
+000235b0: 2069 6620 6b75 6265 7479 7065 203d 3d20   if kubetype == 
+000235c0: 276f 7065 6e73 6869 6674 273a 0a20 2020  'openshift':.   
+000235d0: 2020 2020 2020 2020 2072 6573 756c 7420           result 
+000235e0: 3d20 7365 6c66 2e63 7265 6174 655f 6b75  = self.create_ku
+000235f0: 6265 5f6f 7065 6e73 6869 6674 2863 6c75  be_openshift(clu
+00023600: 7374 6572 2c20 6f76 6572 7269 6465 733d  ster, overrides=
+00023610: 6f76 6572 7269 6465 7329 0a20 2020 2020  overrides).     
+00023620: 2020 2065 6c69 6620 6b75 6265 7479 7065     elif kubetype
+00023630: 203d 3d20 276f 7065 6e73 6869 6674 2d73   == 'openshift-s
+00023640: 6e6f 273a 0a20 2020 2020 2020 2020 2020  no':.           
+00023650: 206f 7665 7272 6964 6573 5b27 736e 6f27   overrides['sno'
+00023660: 5d20 3d20 5472 7565 0a20 2020 2020 2020  ] = True.       
+00023670: 2020 2020 2072 6573 756c 7420 3d20 7365       result = se
+00023680: 6c66 2e63 7265 6174 655f 6b75 6265 5f6f  lf.create_kube_o
+00023690: 7065 6e73 6869 6674 2863 6c75 7374 6572  penshift(cluster
+000236a0: 2c20 6f76 6572 7269 6465 733d 6f76 6572  , overrides=over
+000236b0: 7269 6465 7329 0a20 2020 2020 2020 2065  rides).        e
+000236c0: 6c69 6620 6b75 6265 7479 7065 203d 3d20  lif kubetype == 
+000236d0: 2768 7970 6572 7368 6966 7427 3a0a 2020  'hypershift':.  
+000236e0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+000236f0: 203d 2073 656c 662e 6372 6561 7465 5f6b   = self.create_k
+00023700: 7562 655f 6879 7065 7273 6869 6674 2863  ube_hypershift(c
+00023710: 6c75 7374 6572 2c20 6f76 6572 7269 6465  luster, override
+00023720: 733d 6f76 6572 7269 6465 7329 0a20 2020  s=overrides).   
+00023730: 2020 2020 2065 6c69 6620 6b75 6265 7479       elif kubety
+00023740: 7065 203d 3d20 276d 6963 726f 7368 6966  pe == 'microshif
+00023750: 7427 3a0a 2020 2020 2020 2020 2020 2020  t':.            
+00023760: 7265 7375 6c74 203d 2073 656c 662e 6372  result = self.cr
+00023770: 6561 7465 5f6b 7562 655f 6d69 6372 6f73  eate_kube_micros
+00023780: 6869 6674 2863 6c75 7374 6572 2c20 6f76  hift(cluster, ov
+00023790: 6572 7269 6465 733d 6f76 6572 7269 6465  errides=override
+000237a0: 7329 0a20 2020 2020 2020 2065 6c69 6620  s).        elif 
+000237b0: 6b75 6265 7479 7065 203d 3d20 276b 3373  kubetype == 'k3s
+000237c0: 273a 0a20 2020 2020 2020 2020 2020 2072  ':.            r
+000237d0: 6573 756c 7420 3d20 7365 6c66 2e63 7265  esult = self.cre
+000237e0: 6174 655f 6b75 6265 5f6b 3373 2863 6c75  ate_kube_k3s(clu
+000237f0: 7374 6572 2c20 6f76 6572 7269 6465 733d  ster, overrides=
+00023800: 6f76 6572 7269 6465 7329 0a20 2020 2020  overrides).     
+00023810: 2020 2065 6c69 6620 6b75 6265 7479 7065     elif kubetype
+00023820: 203d 3d20 2767 6b65 273a 0a20 2020 2020   == 'gke':.     
+00023830: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+00023840: 7365 6c66 2e63 7265 6174 655f 6b75 6265  self.create_kube
+00023850: 5f67 6b65 2863 6c75 7374 6572 2c20 6f76  _gke(cluster, ov
+00023860: 6572 7269 6465 733d 6f76 6572 7269 6465  errides=override
+00023870: 7329 0a20 2020 2020 2020 2065 6c69 6620  s).        elif 
+00023880: 6b75 6265 7479 7065 203d 3d20 2765 6b73  kubetype == 'eks
+00023890: 273a 0a20 2020 2020 2020 2020 2020 2072  ':.            r
+000238a0: 6573 756c 7420 3d20 7365 6c66 2e63 7265  esult = self.cre
+000238b0: 6174 655f 6b75 6265 5f65 6b73 2863 6c75  ate_kube_eks(clu
+000238c0: 7374 6572 2c20 6f76 6572 7269 6465 733d  ster, overrides=
+000238d0: 6f76 6572 7269 6465 7329 0a20 2020 2020  overrides).     
+000238e0: 2020 2065 6c69 6620 6b75 6265 7479 7065     elif kubetype
+000238f0: 203d 3d20 2761 6b73 273a 0a20 2020 2020   == 'aks':.     
+00023900: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+00023910: 7365 6c66 2e63 7265 6174 655f 6b75 6265  self.create_kube
+00023920: 5f61 6b73 2863 6c75 7374 6572 2c20 6f76  _aks(cluster, ov
+00023930: 6572 7269 6465 733d 6f76 6572 7269 6465  errides=override
+00023940: 7329 0a20 2020 2020 2020 2065 6c73 653a  s).        else:
+00023950: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00023960: 756c 7420 3d20 7365 6c66 2e63 7265 6174  ult = self.creat
+00023970: 655f 6b75 6265 5f67 656e 6572 6963 2863  e_kube_generic(c
+00023980: 6c75 7374 6572 2c20 6f76 6572 7269 6465  luster, override
+00023990: 733d 6f76 6572 7269 6465 7329 0a20 2020  s=overrides).   
+000239a0: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
+000239b0: 6c74 0a0a 2020 2020 6465 6620 6372 6561  lt..    def crea
+000239c0: 7465 5f6b 7562 655f 616b 7328 7365 6c66  te_kube_aks(self
+000239d0: 2c20 636c 7573 7465 722c 206f 7665 7272  , cluster, overr
+000239e0: 6964 6573 3d7b 7d29 3a0a 2020 2020 2020  ides={}):.      
+000239f0: 2020 6672 6f6d 206b 7669 7274 2e63 6c75    from kvirt.clu
+00023a00: 7374 6572 2069 6d70 6f72 7420 616b 730a  ster import aks.
+00023a10: 2020 2020 2020 2020 6966 2063 6f6e 7461          if conta
+00023a20: 696e 6572 5f6d 6f64 6528 293a 0a20 2020  iner_mode():.   
+00023a30: 2020 2020 2020 2020 206f 732e 656e 7669           os.envi
+00023a40: 726f 6e5b 2750 4154 4827 5d20 2b3d 2027  ron['PATH'] += '
+00023a50: 3a2f 776f 726b 6469 7227 0a20 2020 2020  :/workdir'.     
+00023a60: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00023a70: 2020 2020 206f 732e 656e 7669 726f 6e5b       os.environ[
+00023a80: 2750 4154 4827 5d20 2b3d 2027 3a25 7327  'PATH'] += ':%s'
+00023a90: 2025 206f 732e 6765 7463 7764 2829 0a20   % os.getcwd(). 
+00023aa0: 2020 2020 2020 2072 6574 7572 6e20 616b         return ak
+00023ab0: 732e 6372 6561 7465 2873 656c 662c 2063  s.create(self, c
+00023ac0: 6c75 7374 6572 2c20 6f76 6572 7269 6465  luster, override
+00023ad0: 7329 0a0a 2020 2020 6465 6620 6372 6561  s)..    def crea
+00023ae0: 7465 5f6b 7562 655f 656b 7328 7365 6c66  te_kube_eks(self
+00023af0: 2c20 636c 7573 7465 722c 206f 7665 7272  , cluster, overr
+00023b00: 6964 6573 3d7b 7d29 3a0a 2020 2020 2020  ides={}):.      
+00023b10: 2020 6672 6f6d 206b 7669 7274 2e63 6c75    from kvirt.clu
+00023b20: 7374 6572 2069 6d70 6f72 7420 656b 730a  ster import eks.
+00023b30: 2020 2020 2020 2020 6966 2063 6f6e 7461          if conta
+00023b40: 696e 6572 5f6d 6f64 6528 293a 0a20 2020  iner_mode():.   
+00023b50: 2020 2020 2020 2020 206f 732e 656e 7669           os.envi
+00023b60: 726f 6e5b 2750 4154 4827 5d20 2b3d 2027  ron['PATH'] += '
+00023b70: 3a2f 776f 726b 6469 7227 0a20 2020 2020  :/workdir'.     
+00023b80: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00023b90: 2020 2020 206f 732e 656e 7669 726f 6e5b       os.environ[
+00023ba0: 2750 4154 4827 5d20 2b3d 2027 3a25 7327  'PATH'] += ':%s'
+00023bb0: 2025 206f 732e 6765 7463 7764 2829 0a20   % os.getcwd(). 
+00023bc0: 2020 2020 2020 2072 6574 7572 6e20 656b         return ek
+00023bd0: 732e 6372 6561 7465 2873 656c 662c 2063  s.create(self, c
+00023be0: 6c75 7374 6572 2c20 6f76 6572 7269 6465  luster, override
+00023bf0: 7329 0a0a 2020 2020 6465 6620 6372 6561  s)..    def crea
+00023c00: 7465 5f6b 7562 655f 6765 6e65 7269 6328  te_kube_generic(
+00023c10: 7365 6c66 2c20 636c 7573 7465 722c 206f  self, cluster, o
+00023c20: 7665 7272 6964 6573 3d7b 7d29 3a0a 2020  verrides={}):.  
+00023c30: 2020 2020 2020 6966 2063 6f6e 7461 696e        if contain
+00023c40: 6572 5f6d 6f64 6528 293a 0a20 2020 2020  er_mode():.     
+00023c50: 2020 2020 2020 206f 732e 656e 7669 726f         os.enviro
+00023c60: 6e5b 2750 4154 4827 5d20 2b3d 2027 3a2f  n['PATH'] += ':/
+00023c70: 776f 726b 6469 7227 0a20 2020 2020 2020  workdir'.       
+00023c80: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00023c90: 2020 206f 732e 656e 7669 726f 6e5b 2750     os.environ['P
+00023ca0: 4154 4827 5d20 2b3d 2027 3a25 7327 2025  ATH'] += ':%s' %
+00023cb0: 206f 732e 6765 7463 7764 2829 0a20 2020   os.getcwd().   
+00023cc0: 2020 2020 2070 6c61 6e64 6972 203d 206f       plandir = o
+00023cd0: 732e 7061 7468 2e64 6972 6e61 6d65 286b  s.path.dirname(k
+00023ce0: 7562 6561 646d 2e63 7265 6174 652e 5f5f  ubeadm.create.__
+00023cf0: 636f 6465 5f5f 2e63 6f5f 6669 6c65 6e61  code__.co_filena
+00023d00: 6d65 290a 2020 2020 2020 2020 7265 7475  me).        retu
+00023d10: 726e 206b 7562 6561 646d 2e63 7265 6174  rn kubeadm.creat
+00023d20: 6528 7365 6c66 2c20 706c 616e 6469 722c  e(self, plandir,
+00023d30: 2063 6c75 7374 6572 2c20 6f76 6572 7269   cluster, overri
+00023d40: 6465 7329 0a0a 2020 2020 6465 6620 6372  des)..    def cr
+00023d50: 6561 7465 5f6b 7562 655f 676b 6528 7365  eate_kube_gke(se
+00023d60: 6c66 2c20 636c 7573 7465 722c 206f 7665  lf, cluster, ove
+00023d70: 7272 6964 6573 3d7b 7d29 3a0a 2020 2020  rrides={}):.    
+00023d80: 2020 2020 6672 6f6d 206b 7669 7274 2e63      from kvirt.c
+00023d90: 6c75 7374 6572 2069 6d70 6f72 7420 676b  luster import gk
+00023da0: 650a 2020 2020 2020 2020 6966 2063 6f6e  e.        if con
+00023db0: 7461 696e 6572 5f6d 6f64 6528 293a 0a20  tainer_mode():. 
+00023dc0: 2020 2020 2020 2020 2020 206f 732e 656e             os.en
+00023dd0: 7669 726f 6e5b 2750 4154 4827 5d20 2b3d  viron['PATH'] +=
+00023de0: 2027 3a2f 776f 726b 6469 7227 0a20 2020   ':/workdir'.   
+00023df0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00023e00: 2020 2020 2020 206f 732e 656e 7669 726f         os.enviro
+00023e10: 6e5b 2750 4154 4827 5d20 2b3d 2027 3a25  n['PATH'] += ':%
+00023e20: 7327 2025 206f 732e 6765 7463 7764 2829  s' % os.getcwd()
+00023e30: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00023e40: 676b 652e 6372 6561 7465 2873 656c 662c  gke.create(self,
+00023e50: 2063 6c75 7374 6572 2c20 6f76 6572 7269   cluster, overri
+00023e60: 6465 7329 0a0a 2020 2020 6465 6620 6372  des)..    def cr
+00023e70: 6561 7465 5f6b 7562 655f 6d69 6372 6f73  eate_kube_micros
+00023e80: 6869 6674 2873 656c 662c 2063 6c75 7374  hift(self, clust
+00023e90: 6572 2c20 6f76 6572 7269 6465 733d 7b7d  er, overrides={}
+00023ea0: 293a 0a20 2020 2020 2020 2069 6620 636f  ):.        if co
+00023eb0: 6e74 6169 6e65 725f 6d6f 6465 2829 3a0a  ntainer_mode():.
+00023ec0: 2020 2020 2020 2020 2020 2020 6f73 2e65              os.e
+00023ed0: 6e76 6972 6f6e 5b27 5041 5448 275d 202b  nviron['PATH'] +
+00023ee0: 3d20 273a 2f77 6f72 6b64 6972 270a 2020  = ':/workdir'.  
+00023ef0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00023f00: 2020 2020 2020 2020 6f73 2e65 6e76 6972          os.envir
+00023f10: 6f6e 5b27 5041 5448 275d 202b 3d20 273a  on['PATH'] += ':
+00023f20: 2573 2720 2520 6f73 2e67 6574 6377 6428  %s' % os.getcwd(
+00023f30: 290a 2020 2020 2020 2020 706c 616e 6469  ).        plandi
+00023f40: 7220 3d20 6f73 2e70 6174 682e 6469 726e  r = os.path.dirn
+00023f50: 616d 6528 6d69 6372 6f73 6869 6674 2e63  ame(microshift.c
+00023f60: 7265 6174 652e 5f5f 636f 6465 5f5f 2e63  reate.__code__.c
+00023f70: 6f5f 6669 6c65 6e61 6d65 290a 2020 2020  o_filename).    
+00023f80: 2020 2020 7265 7475 726e 206d 6963 726f      return micro
+00023f90: 7368 6966 742e 6372 6561 7465 2873 656c  shift.create(sel
+00023fa0: 662c 2070 6c61 6e64 6972 2c20 636c 7573  f, plandir, clus
+00023fb0: 7465 722c 206f 7665 7272 6964 6573 290a  ter, overrides).
+00023fc0: 0a20 2020 2064 6566 2063 7265 6174 655f  .    def create_
+00023fd0: 6b75 6265 5f6b 3373 2873 656c 662c 2063  kube_k3s(self, c
+00023fe0: 6c75 7374 6572 2c20 6f76 6572 7269 6465  luster, override
+00023ff0: 733d 7b7d 293a 0a20 2020 2020 2020 2069  s={}):.        i
+00024000: 6620 636f 6e74 6169 6e65 725f 6d6f 6465  f container_mode
+00024010: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+00024020: 6f73 2e65 6e76 6972 6f6e 5b27 5041 5448  os.environ['PATH
+00024030: 275d 202b 3d20 273a 2f77 6f72 6b64 6972  '] += ':/workdir
+00024040: 270a 2020 2020 2020 2020 656c 7365 3a0a  '.        else:.
+00024050: 2020 2020 2020 2020 2020 2020 6f73 2e65              os.e
+00024060: 6e76 6972 6f6e 5b27 5041 5448 275d 202b  nviron['PATH'] +
+00024070: 3d20 273a 2573 2720 2520 6f73 2e67 6574  = ':%s' % os.get
+00024080: 6377 6428 290a 2020 2020 2020 2020 706c  cwd().        pl
+00024090: 616e 6469 7220 3d20 6f73 2e70 6174 682e  andir = os.path.
+000240a0: 6469 726e 616d 6528 6b33 732e 6372 6561  dirname(k3s.crea
+000240b0: 7465 2e5f 5f63 6f64 655f 5f2e 636f 5f66  te.__code__.co_f
+000240c0: 696c 656e 616d 6529 0a20 2020 2020 2020  ilename).       
+000240d0: 2072 6574 7572 6e20 6b33 732e 6372 6561   return k3s.crea
+000240e0: 7465 2873 656c 662c 2070 6c61 6e64 6972  te(self, plandir
+000240f0: 2c20 636c 7573 7465 722c 206f 7665 7272  , cluster, overr
+00024100: 6964 6573 290a 0a20 2020 2064 6566 2063  ides)..    def c
+00024110: 7265 6174 655f 6b75 6265 5f68 7970 6572  reate_kube_hyper
+00024120: 7368 6966 7428 7365 6c66 2c20 636c 7573  shift(self, clus
+00024130: 7465 722c 206f 7665 7272 6964 6573 3d7b  ter, overrides={
+00024140: 7d29 3a0a 2020 2020 2020 2020 6966 2063  }):.        if c
+00024150: 6f6e 7461 696e 6572 5f6d 6f64 6528 293a  ontainer_mode():
+00024160: 0a20 2020 2020 2020 2020 2020 206f 732e  .            os.
+00024170: 656e 7669 726f 6e5b 2750 4154 4827 5d20  environ['PATH'] 
+00024180: 2b3d 2027 3a2f 776f 726b 6469 7227 0a20  += ':/workdir'. 
+00024190: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+000241a0: 2020 2020 2020 2020 206f 732e 656e 7669           os.envi
+000241b0: 726f 6e5b 2750 4154 4827 5d20 2b3d 2027  ron['PATH'] += '
+000241c0: 3a25 7327 2025 206f 732e 6765 7463 7764  :%s' % os.getcwd
+000241d0: 2829 0a20 2020 2020 2020 2070 6c61 6e64  ().        pland
+000241e0: 6972 203d 206f 732e 7061 7468 2e64 6972  ir = os.path.dir
+000241f0: 6e61 6d65 2868 7970 6572 7368 6966 742e  name(hypershift.
+00024200: 6372 6561 7465 2e5f 5f63 6f64 655f 5f2e  create.__code__.
+00024210: 636f 5f66 696c 656e 616d 6529 0a20 2020  co_filename).   
+00024220: 2020 2020 2023 2064 6e73 636c 6965 6e74       # dnsclient
+00024230: 203d 206f 7665 7272 6964 6573 2e67 6574   = overrides.get
+00024240: 2827 646e 7363 6c69 656e 7427 290a 2020  ('dnsclient').  
+00024250: 2020 2020 2020 2320 646e 7363 6f6e 6669        # dnsconfi
+00024260: 6720 3d20 4b63 6f6e 6669 6728 636c 6965  g = Kconfig(clie
+00024270: 6e74 3d64 6e73 636c 6965 6e74 2920 6966  nt=dnsclient) if
+00024280: 2064 6e73 636c 6965 6e74 2069 7320 6e6f   dnsclient is no
+00024290: 7420 4e6f 6e65 2065 6c73 6520 4e6f 6e65  t None else None
+000242a0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000242b0: 6879 7065 7273 6869 6674 2e63 7265 6174  hypershift.creat
+000242c0: 6528 7365 6c66 2c20 706c 616e 6469 722c  e(self, plandir,
+000242d0: 2063 6c75 7374 6572 2c20 6f76 6572 7269   cluster, overri
+000242e0: 6465 7329 0a0a 2020 2020 6465 6620 6372  des)..    def cr
+000242f0: 6561 7465 5f6b 7562 655f 6f70 656e 7368  eate_kube_opensh
+00024300: 6966 7428 7365 6c66 2c20 636c 7573 7465  ift(self, cluste
+00024310: 722c 206f 7665 7272 6964 6573 3d7b 7d29  r, overrides={})
+00024320: 3a0a 2020 2020 2020 2020 6966 2063 6f6e  :.        if con
+00024330: 7461 696e 6572 5f6d 6f64 6528 293a 0a20  tainer_mode():. 
+00024340: 2020 2020 2020 2020 2020 206f 732e 656e             os.en
+00024350: 7669 726f 6e5b 2750 4154 4827 5d20 2b3d  viron['PATH'] +=
+00024360: 2027 3a2f 776f 726b 6469 7227 0a20 2020   ':/workdir'.   
+00024370: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00024380: 2020 2020 2020 206f 732e 656e 7669 726f         os.enviro
+00024390: 6e5b 2750 4154 4827 5d20 2b3d 2027 3a25  n['PATH'] += ':%
+000243a0: 7327 2025 206f 732e 6765 7463 7764 2829  s' % os.getcwd()
+000243b0: 0a20 2020 2020 2020 2070 6c61 6e64 6972  .        plandir
+000243c0: 203d 206f 732e 7061 7468 2e64 6972 6e61   = os.path.dirna
+000243d0: 6d65 286f 7065 6e73 6869 6674 2e63 7265  me(openshift.cre
+000243e0: 6174 652e 5f5f 636f 6465 5f5f 2e63 6f5f  ate.__code__.co_
+000243f0: 6669 6c65 6e61 6d65 290a 2020 2020 2020  filename).      
+00024400: 2020 646e 7363 6c69 656e 7420 3d20 6f76    dnsclient = ov
+00024410: 6572 7269 6465 732e 6765 7428 2764 6e73  errides.get('dns
+00024420: 636c 6965 6e74 2729 0a20 2020 2020 2020  client').       
+00024430: 2064 6e73 636f 6e66 6967 203d 204b 636f   dnsconfig = Kco
+00024440: 6e66 6967 2863 6c69 656e 743d 646e 7363  nfig(client=dnsc
+00024450: 6c69 656e 7429 2069 6620 646e 7363 6c69  lient) if dnscli
+00024460: 656e 7420 6973 206e 6f74 204e 6f6e 6520  ent is not None 
+00024470: 656c 7365 204e 6f6e 650a 2020 2020 2020  else None.      
+00024480: 2020 7265 7475 726e 206f 7065 6e73 6869    return openshi
+00024490: 6674 2e63 7265 6174 6528 7365 6c66 2c20  ft.create(self, 
+000244a0: 706c 616e 6469 722c 2063 6c75 7374 6572  plandir, cluster
+000244b0: 2c20 6f76 6572 7269 6465 732c 2064 6e73  , overrides, dns
+000244c0: 636f 6e66 6967 3d64 6e73 636f 6e66 6967  config=dnsconfig
+000244d0: 290a 0a20 2020 2064 6566 2064 656c 6574  )..    def delet
+000244e0: 655f 6b75 6265 2873 656c 662c 2063 6c75  e_kube(self, clu
+000244f0: 7374 6572 2c20 6f76 6572 7269 6465 733d  ster, overrides=
+00024500: 7b7d 293a 0a20 2020 2020 2020 206b 203d  {}):.        k =
+00024510: 2073 656c 662e 6b0a 2020 2020 2020 2020   self.k.        
+00024520: 6879 7065 7273 6869 6674 203d 206f 7665  hypershift = ove
+00024530: 7272 6964 6573 2e67 6574 2827 6b75 6265  rrides.get('kube
+00024540: 7479 7065 272c 2027 7878 7827 2920 3d3d  type', 'xxx') ==
+00024550: 2027 6879 7065 7273 6869 6674 270a 2020   'hypershift'.  
+00024560: 2020 2020 2020 6173 7369 7374 6564 203d        assisted =
+00024570: 2046 616c 7365 0a20 2020 2020 2020 2061   False.        a
+00024580: 6b73 203d 206f 7665 7272 6964 6573 2e67  ks = overrides.g
+00024590: 6574 2827 6b75 6265 7479 7065 272c 2027  et('kubetype', '
+000245a0: 7878 7827 2920 3d3d 2027 616b 7327 0a20  xxx') == 'aks'. 
+000245b0: 2020 2020 2020 2065 6b73 203d 206f 7665         eks = ove
+000245c0: 7272 6964 6573 2e67 6574 2827 6b75 6265  rrides.get('kube
+000245d0: 7479 7065 272c 2027 7878 7827 2920 3d3d  type', 'xxx') ==
+000245e0: 2027 656b 7327 0a20 2020 2020 2020 2067   'eks'.        g
+000245f0: 6b65 203d 206f 7665 7272 6964 6573 2e67  ke = overrides.g
+00024600: 6574 2827 6b75 6265 7479 7065 272c 2027  et('kubetype', '
+00024610: 7878 7827 2920 3d3d 2027 676b 6527 0a20  xxx') == 'gke'. 
+00024620: 2020 2020 2020 2064 6f6d 6169 6e20 3d20         domain = 
+00024630: 6f76 6572 7269 6465 732e 6765 7428 2764  overrides.get('d
+00024640: 6f6d 6169 6e27 2c20 276b 6172 6d61 6c61  omain', 'karmala
+00024650: 6273 2e63 6f72 7027 290a 2020 2020 2020  bs.corp').      
+00024660: 2020 6b75 6265 7479 7065 203d 206f 7665    kubetype = ove
+00024670: 7272 6964 6573 2e67 6574 2827 6b75 6265  rrides.get('kube
+00024680: 7479 7065 272c 2027 6765 6e65 7269 6327  type', 'generic'
+00024690: 290a 2020 2020 2020 2020 646e 7363 6c69  ).        dnscli
+000246a0: 656e 7420 3d20 4e6f 6e65 0a20 2020 2020  ent = None.     
+000246b0: 2020 2069 6620 7365 6c66 2e74 7970 6520     if self.type 
+000246c0: 3d3d 2027 7765 6227 2061 6e64 206b 2e6c  == 'web' and k.l
+000246d0: 6f63 616c 6b75 6265 3a0a 2020 2020 2020  ocalkube:.      
+000246e0: 2020 2020 2020 7265 7475 726e 206b 2e64        return k.d
+000246f0: 656c 6574 655f 6b75 6265 2863 6c75 7374  elete_kube(clust
+00024700: 6572 2c20 6b75 6265 7479 7065 2c20 6f76  er, kubetype, ov
+00024710: 6572 7269 6465 733d 6f76 6572 7269 6465  errides=override
+00024720: 7329 0a20 2020 2020 2020 2063 6c75 7374  s).        clust
+00024730: 6572 203d 206f 7665 7272 6964 6573 2e67  er = overrides.g
+00024740: 6574 2827 636c 7573 7465 7227 2c20 636c  et('cluster', cl
+00024750: 7573 7465 7229 0a20 2020 2020 2020 2069  uster).        i
+00024760: 6620 636c 7573 7465 7220 6973 204e 6f6e  f cluster is Non
+00024770: 6520 6f72 2063 6c75 7374 6572 203d 3d20  e or cluster == 
+00024780: 2727 3a0a 2020 2020 2020 2020 2020 2020  '':.            
+00024790: 6465 6661 756c 745f 636c 7573 7465 7273  default_clusters
+000247a0: 203d 207b 2767 656e 6572 6963 273a 2027   = {'generic': '
+000247b0: 6d79 6b75 6265 272c 2027 6879 7065 7273  mykube', 'hypers
+000247c0: 6869 6674 273a 2027 6d79 6879 7065 7273  hift': 'myhypers
+000247d0: 6869 6674 272c 2027 6f70 656e 7368 6966  hift', 'openshif
+000247e0: 7427 3a20 276d 796f 7065 6e73 6869 6674  t': 'myopenshift
+000247f0: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
 00024800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024810: 2020 2020 2027 6b33 7327 3a20 276d 796b       'k3s': 'myk
-00024820: 3373 272c 2027 6d69 6372 6f73 6869 6674  3s', 'microshift
-00024830: 273a 2027 6d79 6d69 6372 6f73 6869 6674  ': 'mymicroshift
-00024840: 272c 2027 676b 6527 3a20 276d 7967 6b65  ', 'gke': 'mygke
-00024850: 272c 2027 656b 7327 3a20 276d 7965 6b73  ', 'eks': 'myeks
-00024860: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
+00024810: 2020 2027 6b33 7327 3a20 276d 796b 3373     'k3s': 'myk3s
+00024820: 272c 2027 6d69 6372 6f73 6869 6674 273a  ', 'microshift':
+00024830: 2027 6d79 6d69 6372 6f73 6869 6674 272c   'mymicroshift',
+00024840: 2027 676b 6527 3a20 276d 7967 6b65 272c   'gke': 'mygke',
+00024850: 2027 656b 7327 3a20 276d 7965 6b73 272c   'eks': 'myeks',
+00024860: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00024870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024880: 2020 2027 616b 7327 3a20 276d 7961 6b73     'aks': 'myaks
-00024890: 277d 0a20 2020 2020 2020 2020 2020 2063  '}.            c
-000248a0: 6c75 7374 6572 203d 2064 6566 6175 6c74  luster = default
-000248b0: 5f63 6c75 7374 6572 735b 6b75 6265 7479  _clusters[kubety
-000248c0: 7065 5d0a 2020 2020 2020 2020 636c 7573  pe].        clus
-000248d0: 7465 7264 6174 6120 3d20 7b7d 0a20 2020  terdata = {}.   
-000248e0: 2020 2020 2063 6c75 7374 6572 6469 7220       clusterdir 
-000248f0: 3d20 6f73 2e70 6174 682e 6578 7061 6e64  = os.path.expand
-00024900: 7573 6572 2866 227e 2f2e 6b63 6c69 2f63  user(f"~/.kcli/c
-00024910: 6c75 7374 6572 732f 7b63 6c75 7374 6572  lusters/{cluster
-00024920: 7d22 290a 2020 2020 2020 2020 6966 206f  }").        if o
-00024930: 732e 7061 7468 2e65 7869 7374 7328 636c  s.path.exists(cl
-00024940: 7573 7465 7264 6972 293a 0a20 2020 2020  usterdir):.     
-00024950: 2020 2020 2020 2070 6172 616d 6574 6572         parameter
-00024960: 7366 696c 6520 3d20 6622 7b63 6c75 7374  sfile = f"{clust
-00024970: 6572 6469 727d 2f6b 636c 695f 7061 7261  erdir}/kcli_para
-00024980: 6d65 7465 7273 2e79 6d6c 220a 2020 2020  meters.yml".    
-00024990: 2020 2020 2020 2020 6966 206f 732e 7061          if os.pa
-000249a0: 7468 2e65 7869 7374 7328 7061 7261 6d65  th.exists(parame
-000249b0: 7465 7273 6669 6c65 293a 0a20 2020 2020  tersfile):.     
-000249c0: 2020 2020 2020 2020 2020 2077 6974 6820             with 
-000249d0: 6f70 656e 2870 6172 616d 6574 6572 7366  open(parametersf
-000249e0: 696c 6529 2061 7320 663a 0a20 2020 2020  ile) as f:.     
-000249f0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00024a00: 6c75 7374 6572 6461 7461 203d 2079 616d  lusterdata = yam
-00024a10: 6c2e 7361 6665 5f6c 6f61 6428 6629 0a20  l.safe_load(f). 
+00024880: 2027 616b 7327 3a20 276d 7961 6b73 277d   'aks': 'myaks'}
+00024890: 0a20 2020 2020 2020 2020 2020 2063 6c75  .            clu
+000248a0: 7374 6572 203d 2064 6566 6175 6c74 5f63  ster = default_c
+000248b0: 6c75 7374 6572 735b 6b75 6265 7479 7065  lusters[kubetype
+000248c0: 5d0a 2020 2020 2020 2020 636c 7573 7465  ].        cluste
+000248d0: 7264 6174 6120 3d20 7b7d 0a20 2020 2020  rdata = {}.     
+000248e0: 2020 2063 6c75 7374 6572 6469 7220 3d20     clusterdir = 
+000248f0: 6f73 2e70 6174 682e 6578 7061 6e64 7573  os.path.expandus
+00024900: 6572 2866 227e 2f2e 6b63 6c69 2f63 6c75  er(f"~/.kcli/clu
+00024910: 7374 6572 732f 7b63 6c75 7374 6572 7d22  sters/{cluster}"
+00024920: 290a 2020 2020 2020 2020 6966 206f 732e  ).        if os.
+00024930: 7061 7468 2e65 7869 7374 7328 636c 7573  path.exists(clus
+00024940: 7465 7264 6972 293a 0a20 2020 2020 2020  terdir):.       
+00024950: 2020 2020 2070 6172 616d 6574 6572 7366       parametersf
+00024960: 696c 6520 3d20 6622 7b63 6c75 7374 6572  ile = f"{cluster
+00024970: 6469 727d 2f6b 636c 695f 7061 7261 6d65  dir}/kcli_parame
+00024980: 7465 7273 2e79 6d6c 220a 2020 2020 2020  ters.yml".      
+00024990: 2020 2020 2020 6966 206f 732e 7061 7468        if os.path
+000249a0: 2e65 7869 7374 7328 7061 7261 6d65 7465  .exists(paramete
+000249b0: 7273 6669 6c65 293a 0a20 2020 2020 2020  rsfile):.       
+000249c0: 2020 2020 2020 2020 2077 6974 6820 6f70           with op
+000249d0: 656e 2870 6172 616d 6574 6572 7366 696c  en(parametersfil
+000249e0: 6529 2061 7320 663a 0a20 2020 2020 2020  e) as f:.       
+000249f0: 2020 2020 2020 2020 2020 2020 2063 6c75               clu
+00024a00: 7374 6572 6461 7461 203d 2079 616d 6c2e  sterdata = yaml.
+00024a10: 7361 6665 5f6c 6f61 6428 6629 0a20 2020  safe_load(f).   
 00024a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024a30: 2020 206b 7562 6574 7970 6520 3d20 636c     kubetype = cl
-00024a40: 7573 7465 7264 6174 612e 6765 7428 276b  usterdata.get('k
-00024a50: 7562 6574 7970 6527 2c20 2767 656e 6572  ubetype', 'gener
-00024a60: 6963 2729 0a20 2020 2020 2020 2020 2020  ic').           
-00024a70: 2020 2020 2020 2020 2069 6620 6b75 6265           if kube
-00024a80: 7479 7065 203d 3d20 2768 7970 6572 7368  type == 'hypersh
-00024a90: 6966 7427 3a0a 2020 2020 2020 2020 2020  ift':.          
-00024aa0: 2020 2020 2020 2020 2020 2020 2020 6879                hy
-00024ab0: 7065 7273 6869 6674 203d 2054 7275 650a  pershift = True.
+00024a30: 206b 7562 6574 7970 6520 3d20 636c 7573   kubetype = clus
+00024a40: 7465 7264 6174 612e 6765 7428 276b 7562  terdata.get('kub
+00024a50: 6574 7970 6527 2c20 2767 656e 6572 6963  etype', 'generic
+00024a60: 2729 0a20 2020 2020 2020 2020 2020 2020  ').             
+00024a70: 2020 2020 2020 2069 6620 6b75 6265 7479         if kubety
+00024a80: 7065 203d 3d20 2768 7970 6572 7368 6966  pe == 'hypershif
+00024a90: 7427 3a0a 2020 2020 2020 2020 2020 2020  t':.            
+00024aa0: 2020 2020 2020 2020 2020 2020 6879 7065              hype
+00024ab0: 7273 6869 6674 203d 2054 7275 650a 2020  rshift = True.  
 00024ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024ad0: 2020 2020 2020 2020 6173 7369 7374 6564          assisted
-00024ae0: 203d 2063 6c75 7374 6572 6461 7461 2e67   = clusterdata.g
-00024af0: 6574 2827 6173 7369 7374 6564 272c 2046  et('assisted', F
-00024b00: 616c 7365 290a 2020 2020 2020 2020 2020  alse).          
-00024b10: 2020 2020 2020 2020 2020 646f 6d61 696e            domain
-00024b20: 203d 2063 6c75 7374 6572 6461 7461 2e67   = clusterdata.g
-00024b30: 6574 2827 646f 6d61 696e 272c 2064 6f6d  et('domain', dom
-00024b40: 6169 6e29 0a20 2020 2020 2020 2020 2020  ain).           
-00024b50: 2020 2020 2020 2020 2064 6e73 636c 6965           dnsclie
-00024b60: 6e74 203d 2063 6c75 7374 6572 6461 7461  nt = clusterdata
-00024b70: 2e67 6574 2827 646e 7363 6c69 656e 7427  .get('dnsclient'
-00024b80: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00024b90: 2020 2020 2020 676b 6520 3d20 6b75 6265        gke = kube
-00024ba0: 7479 7065 203d 3d20 2767 6b65 270a 2020  type == 'gke'.  
+00024ad0: 2020 2020 2020 6173 7369 7374 6564 203d        assisted =
+00024ae0: 2063 6c75 7374 6572 6461 7461 2e67 6574   clusterdata.get
+00024af0: 2827 6173 7369 7374 6564 272c 2046 616c  ('assisted', Fal
+00024b00: 7365 290a 2020 2020 2020 2020 2020 2020  se).            
+00024b10: 2020 2020 2020 2020 646f 6d61 696e 203d          domain =
+00024b20: 2063 6c75 7374 6572 6461 7461 2e67 6574   clusterdata.get
+00024b30: 2827 646f 6d61 696e 272c 2064 6f6d 6169  ('domain', domai
+00024b40: 6e29 0a20 2020 2020 2020 2020 2020 2020  n).             
+00024b50: 2020 2020 2020 2064 6e73 636c 6965 6e74         dnsclient
+00024b60: 203d 2063 6c75 7374 6572 6461 7461 2e67   = clusterdata.g
+00024b70: 6574 2827 646e 7363 6c69 656e 7427 290a  et('dnsclient').
+00024b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024b90: 2020 2020 676b 6520 3d20 6b75 6265 7479      gke = kubety
+00024ba0: 7065 203d 3d20 2767 6b65 270a 2020 2020  pe == 'gke'.    
 00024bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024bc0: 2020 656b 7320 3d20 6b75 6265 7479 7065    eks = kubetype
-00024bd0: 203d 3d20 2765 6b73 270a 2020 2020 2020   == 'eks'.      
-00024be0: 2020 2020 2020 2020 2020 2020 2020 616b                ak
-00024bf0: 7320 3d20 6b75 6265 7479 7065 203d 3d20  s = kubetype == 
-00024c00: 2761 6b73 270a 2020 2020 2020 2020 2020  'aks'.          
-00024c10: 2020 2020 2020 2020 2020 6966 2027 636c            if 'cl
-00024c20: 6965 6e74 2720 696e 2063 6c75 7374 6572  ient' in cluster
-00024c30: 6461 7461 2061 6e64 2063 6c75 7374 6572  data and cluster
-00024c40: 6461 7461 5b27 636c 6965 6e74 275d 2021  data['client'] !
-00024c50: 3d20 7365 6c66 2e63 6c69 656e 743a 0a20  = self.client:. 
+00024bc0: 656b 7320 3d20 6b75 6265 7479 7065 203d  eks = kubetype =
+00024bd0: 3d20 2765 6b73 270a 2020 2020 2020 2020  = 'eks'.        
+00024be0: 2020 2020 2020 2020 2020 2020 616b 7320              aks 
+00024bf0: 3d20 6b75 6265 7479 7065 203d 3d20 2761  = kubetype == 'a
+00024c00: 6b73 270a 2020 2020 2020 2020 2020 2020  ks'.            
+00024c10: 2020 2020 2020 2020 6966 2027 636c 6965          if 'clie
+00024c20: 6e74 2720 696e 2063 6c75 7374 6572 6461  nt' in clusterda
+00024c30: 7461 2061 6e64 2063 6c75 7374 6572 6461  ta and clusterda
+00024c40: 7461 5b27 636c 6965 6e74 275d 2021 3d20  ta['client'] != 
+00024c50: 7365 6c66 2e63 6c69 656e 743a 0a20 2020  self.client:.   
 00024c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024c70: 2020 2020 2020 2073 656c 662e 5f5f 696e         self.__in
-00024c80: 6974 5f5f 2863 6c69 656e 743d 636c 7573  it__(client=clus
-00024c90: 7465 7264 6174 615b 2763 6c69 656e 7427  terdata['client'
-00024ca0: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
-00024cb0: 2020 2020 2020 2020 2020 206b 203d 2073             k = s
-00024cc0: 656c 662e 6b0a 2020 2020 2020 2020 6465  elf.k.        de
-00024cd0: 6c65 7465 636c 6965 6e74 7320 3d20 7b73  leteclients = {s
-00024ce0: 656c 662e 636c 6965 6e74 3a20 6b7d 0a20  elf.client: k}. 
-00024cf0: 2020 2020 2020 2076 6d63 6c69 656e 7473         vmclients
-00024d00: 203d 205b 5d0a 2020 2020 2020 2020 766d   = [].        vm
-00024d10: 636c 6965 6e74 735f 6669 6c65 203d 206f  clients_file = o
-00024d20: 732e 7061 7468 2e65 7870 616e 6475 7365  s.path.expanduse
-00024d30: 7228 6627 7e2f 2e6b 636c 692f 766d 636c  r(f'~/.kcli/vmcl
-00024d40: 6965 6e74 735f 7b63 6c75 7374 6572 7d27  ients_{cluster}'
-00024d50: 290a 2020 2020 2020 2020 6966 206f 732e  ).        if os.
-00024d60: 7061 7468 2e65 7869 7374 7328 766d 636c  path.exists(vmcl
-00024d70: 6965 6e74 735f 6669 6c65 293a 0a20 2020  ients_file):.   
-00024d80: 2020 2020 2020 2020 2076 6d63 6c69 656e           vmclien
-00024d90: 7473 203d 2079 616d 6c2e 7361 6665 5f6c  ts = yaml.safe_l
-00024da0: 6f61 6428 6f70 656e 2876 6d63 6c69 656e  oad(open(vmclien
-00024db0: 7473 5f66 696c 6529 290a 2020 2020 2020  ts_file)).      
-00024dc0: 2020 2020 2020 6f73 2e72 656d 6f76 6528        os.remove(
-00024dd0: 766d 636c 6965 6e74 735f 6669 6c65 290a  vmclients_file).
-00024de0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00024df0: 6578 7472 6163 6c69 656e 7473 3a0a 2020  extraclients:.  
-00024e00: 2020 2020 2020 2020 2020 6465 6c65 7465            delete
-00024e10: 636c 6965 6e74 732e 7570 6461 7465 2873  clients.update(s
-00024e20: 656c 662e 6578 7472 6163 6c69 656e 7473  elf.extraclients
-00024e30: 290a 2020 2020 2020 2020 656c 6966 2076  ).        elif v
-00024e40: 6d63 6c69 656e 7473 3a0a 2020 2020 2020  mclients:.      
-00024e50: 2020 2020 2020 6465 6c65 7465 636c 6965        deleteclie
-00024e60: 6e74 732e 7570 6461 7465 287b 636c 693a  nts.update({cli:
-00024e70: 204b 636f 6e66 6967 2863 6c69 656e 743d   Kconfig(client=
-00024e80: 636c 6929 2e6b 2066 6f72 2063 6c69 2069  cli).k for cli i
-00024e90: 6e20 766d 636c 6965 6e74 7320 6966 2063  n vmclients if c
-00024ea0: 6c69 2021 3d20 7365 6c66 2e63 6c69 656e  li != self.clien
-00024eb0: 747d 290a 2020 2020 2020 2020 666f 7220  t}).        for 
-00024ec0: 6879 7065 7276 6973 6f72 2069 6e20 6465  hypervisor in de
-00024ed0: 6c65 7465 636c 6965 6e74 733a 0a20 2020  leteclients:.   
-00024ee0: 2020 2020 2020 2020 2063 203d 2064 656c           c = del
-00024ef0: 6574 6563 6c69 656e 7473 5b68 7970 6572  eteclients[hyper
-00024f00: 7669 736f 725d 0a20 2020 2020 2020 2020  visor].         
-00024f10: 2020 2066 6f72 2076 6d20 696e 2073 6f72     for vm in sor
-00024f20: 7465 6428 632e 6c69 7374 2829 2c20 6b65  ted(c.list(), ke
-00024f30: 793d 6c61 6d62 6461 2078 3a20 785b 276e  y=lambda x: x['n
-00024f40: 616d 6527 5d29 3a0a 2020 2020 2020 2020  ame']):.        
-00024f50: 2020 2020 2020 2020 6e61 6d65 203d 2076          name = v
-00024f60: 6d5b 276e 616d 6527 5d0a 2020 2020 2020  m['name'].      
-00024f70: 2020 2020 2020 2020 2020 646e 7363 6c69            dnscli
-00024f80: 656e 7420 3d20 766d 2e67 6574 2827 646e  ent = vm.get('dn
-00024f90: 7363 6c69 656e 7427 2920 6f72 2064 6e73  sclient') or dns
-00024fa0: 636c 6965 6e74 0a20 2020 2020 2020 2020  client.         
-00024fb0: 2020 2020 2020 2063 7572 7265 6e74 636c         currentcl
-00024fc0: 7573 7465 7220 3d20 766d 2e67 6574 2827  uster = vm.get('
-00024fd0: 6b75 6265 2729 0a20 2020 2020 2020 2020  kube').         
-00024fe0: 2020 2020 2020 206b 7562 6574 7970 6520         kubetype 
-00024ff0: 3d20 766d 2e67 6574 2827 6b75 6265 7479  = vm.get('kubety
-00025000: 7065 272c 2027 6765 6e65 7269 6327 290a  pe', 'generic').
-00025010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025020: 6966 2063 7572 7265 6e74 636c 7573 7465  if currentcluste
-00025030: 7220 6973 206e 6f74 204e 6f6e 6520 616e  r is not None an
-00025040: 6420 6375 7272 656e 7463 6c75 7374 6572  d currentcluster
-00025050: 203d 3d20 636c 7573 7465 723a 0a20 2020   == cluster:.   
-00025060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025070: 2069 6620 6b75 6265 7479 7065 203d 3d20   if kubetype == 
-00025080: 2767 6b65 273a 0a20 2020 2020 2020 2020  'gke':.         
-00025090: 2020 2020 2020 2020 2020 2020 2020 2067                 g
-000250a0: 6b65 203d 2054 7275 650a 2020 2020 2020  ke = True.      
+00024c70: 2020 2020 2073 656c 662e 5f5f 696e 6974       self.__init
+00024c80: 5f5f 2863 6c69 656e 743d 636c 7573 7465  __(client=cluste
+00024c90: 7264 6174 615b 2763 6c69 656e 7427 5d29  rdata['client'])
+00024ca0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00024cb0: 2020 2020 2020 2020 206b 203d 2073 656c           k = sel
+00024cc0: 662e 6b0a 2020 2020 2020 2020 6465 6c65  f.k.        dele
+00024cd0: 7465 636c 6965 6e74 7320 3d20 7b73 656c  teclients = {sel
+00024ce0: 662e 636c 6965 6e74 3a20 6b7d 0a20 2020  f.client: k}.   
+00024cf0: 2020 2020 2076 6d63 6c69 656e 7473 203d       vmclients =
+00024d00: 205b 5d0a 2020 2020 2020 2020 766d 636c   [].        vmcl
+00024d10: 6965 6e74 735f 6669 6c65 203d 206f 732e  ients_file = os.
+00024d20: 7061 7468 2e65 7870 616e 6475 7365 7228  path.expanduser(
+00024d30: 6627 7e2f 2e6b 636c 692f 766d 636c 6965  f'~/.kcli/vmclie
+00024d40: 6e74 735f 7b63 6c75 7374 6572 7d27 290a  nts_{cluster}').
+00024d50: 2020 2020 2020 2020 6966 206f 732e 7061          if os.pa
+00024d60: 7468 2e65 7869 7374 7328 766d 636c 6965  th.exists(vmclie
+00024d70: 6e74 735f 6669 6c65 293a 0a20 2020 2020  nts_file):.     
+00024d80: 2020 2020 2020 2076 6d63 6c69 656e 7473         vmclients
+00024d90: 203d 2079 616d 6c2e 7361 6665 5f6c 6f61   = yaml.safe_loa
+00024da0: 6428 6f70 656e 2876 6d63 6c69 656e 7473  d(open(vmclients
+00024db0: 5f66 696c 6529 290a 2020 2020 2020 2020  _file)).        
+00024dc0: 2020 2020 6f73 2e72 656d 6f76 6528 766d      os.remove(vm
+00024dd0: 636c 6965 6e74 735f 6669 6c65 290a 2020  clients_file).  
+00024de0: 2020 2020 2020 6966 2073 656c 662e 6578        if self.ex
+00024df0: 7472 6163 6c69 656e 7473 3a0a 2020 2020  traclients:.    
+00024e00: 2020 2020 2020 2020 6465 6c65 7465 636c          deletecl
+00024e10: 6965 6e74 732e 7570 6461 7465 2873 656c  ients.update(sel
+00024e20: 662e 6578 7472 6163 6c69 656e 7473 290a  f.extraclients).
+00024e30: 2020 2020 2020 2020 656c 6966 2076 6d63          elif vmc
+00024e40: 6c69 656e 7473 3a0a 2020 2020 2020 2020  lients:.        
+00024e50: 2020 2020 6465 6c65 7465 636c 6965 6e74      deleteclient
+00024e60: 732e 7570 6461 7465 287b 636c 693a 204b  s.update({cli: K
+00024e70: 636f 6e66 6967 2863 6c69 656e 743d 636c  config(client=cl
+00024e80: 6929 2e6b 2066 6f72 2063 6c69 2069 6e20  i).k for cli in 
+00024e90: 766d 636c 6965 6e74 7320 6966 2063 6c69  vmclients if cli
+00024ea0: 2021 3d20 7365 6c66 2e63 6c69 656e 747d   != self.client}
+00024eb0: 290a 2020 2020 2020 2020 666f 7220 6879  ).        for hy
+00024ec0: 7065 7276 6973 6f72 2069 6e20 6465 6c65  pervisor in dele
+00024ed0: 7465 636c 6965 6e74 733a 0a20 2020 2020  teclients:.     
+00024ee0: 2020 2020 2020 2063 203d 2064 656c 6574         c = delet
+00024ef0: 6563 6c69 656e 7473 5b68 7970 6572 7669  eclients[hypervi
+00024f00: 736f 725d 0a20 2020 2020 2020 2020 2020  sor].           
+00024f10: 2066 6f72 2076 6d20 696e 2073 6f72 7465   for vm in sorte
+00024f20: 6428 632e 6c69 7374 2829 2c20 6b65 793d  d(c.list(), key=
+00024f30: 6c61 6d62 6461 2078 3a20 785b 276e 616d  lambda x: x['nam
+00024f40: 6527 5d29 3a0a 2020 2020 2020 2020 2020  e']):.          
+00024f50: 2020 2020 2020 6e61 6d65 203d 2076 6d5b        name = vm[
+00024f60: 276e 616d 6527 5d0a 2020 2020 2020 2020  'name'].        
+00024f70: 2020 2020 2020 2020 646e 7363 6c69 656e          dnsclien
+00024f80: 7420 3d20 766d 2e67 6574 2827 646e 7363  t = vm.get('dnsc
+00024f90: 6c69 656e 7427 2920 6f72 2064 6e73 636c  lient') or dnscl
+00024fa0: 6965 6e74 0a20 2020 2020 2020 2020 2020  ient.           
+00024fb0: 2020 2020 2063 7572 7265 6e74 636c 7573       currentclus
+00024fc0: 7465 7220 3d20 766d 2e67 6574 2827 6b75  ter = vm.get('ku
+00024fd0: 6265 2729 0a20 2020 2020 2020 2020 2020  be').           
+00024fe0: 2020 2020 206b 7562 6574 7970 6520 3d20       kubetype = 
+00024ff0: 766d 2e67 6574 2827 6b75 6265 7479 7065  vm.get('kubetype
+00025000: 272c 2027 6765 6e65 7269 6327 290a 2020  ', 'generic').  
+00025010: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00025020: 2063 7572 7265 6e74 636c 7573 7465 7220   currentcluster 
+00025030: 6973 206e 6f74 204e 6f6e 6520 616e 6420  is not None and 
+00025040: 6375 7272 656e 7463 6c75 7374 6572 203d  currentcluster =
+00025050: 3d20 636c 7573 7465 723a 0a20 2020 2020  = cluster:.     
+00025060: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00025070: 6620 6b75 6265 7479 7065 203d 3d20 2767  f kubetype == 'g
+00025080: 6b65 273a 0a20 2020 2020 2020 2020 2020  ke':.           
+00025090: 2020 2020 2020 2020 2020 2020 2067 6b65               gke
+000250a0: 203d 2054 7275 650a 2020 2020 2020 2020   = True.        
 000250b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000250c0: 2020 6272 6561 6b0a 2020 2020 2020 2020    break.        
-000250d0: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-000250e0: 206b 7562 6574 7970 6520 3d3d 2027 656b   kubetype == 'ek
-000250f0: 7327 3a0a 2020 2020 2020 2020 2020 2020  s':.            
-00025100: 2020 2020 2020 2020 2020 2020 656b 7320              eks 
-00025110: 3d20 5472 7565 0a20 2020 2020 2020 2020  = True.         
-00025120: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-00025130: 7265 616b 0a20 2020 2020 2020 2020 2020  reak.           
-00025140: 2020 2020 2020 2020 2065 6c69 6620 6b75           elif ku
-00025150: 6265 7479 7065 203d 3d20 2761 6b73 273a  betype == 'aks':
-00025160: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00025170: 2020 2020 2020 2020 2061 6b73 203d 2054           aks = T
-00025180: 7275 650a 2020 2020 2020 2020 2020 2020  rue.            
-00025190: 2020 2020 2020 2020 2020 2020 6272 6561              brea
-000251a0: 6b0a 2020 2020 2020 2020 2020 2020 2020  k.              
-000251b0: 2020 2020 2020 632e 6465 6c65 7465 286e        c.delete(n
-000251c0: 616d 652c 2073 6e61 7073 686f 7473 3d54  ame, snapshots=T
-000251d0: 7275 6529 0a20 2020 2020 2020 2020 2020  rue).           
-000251e0: 2020 2020 2020 2020 2063 6f6d 6d6f 6e2e           common.
-000251f0: 6465 6c65 7465 5f6c 6173 7476 6d28 6e61  delete_lastvm(na
-00025200: 6d65 2c20 7365 6c66 2e63 6c69 656e 7429  me, self.client)
-00025210: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00025220: 2020 2020 2073 7563 6365 7373 2866 227b       success(f"{
-00025230: 6e61 6d65 7d20 6465 6c65 7465 6420 6f6e  name} deleted on
-00025240: 207b 6879 7065 7276 6973 6f72 7d21 2229   {hypervisor}!")
-00025250: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00025260: 2e74 7970 6520 3d3d 2027 6b75 6265 7669  .type == 'kubevi
-00025270: 7274 273a 0a20 2020 2020 2020 2020 2020  rt':.           
-00025280: 2069 6620 6622 7b63 6c75 7374 6572 7d2d   if f"{cluster}-
-00025290: 6170 6922 2069 6e20 6b2e 6c69 7374 5f73  api" in k.list_s
-000252a0: 6572 7669 6365 7328 6b2e 6e61 6d65 7370  ervices(k.namesp
-000252b0: 6163 6529 3a0a 2020 2020 2020 2020 2020  ace):.          
-000252c0: 2020 2020 2020 6b2e 6465 6c65 7465 5f73        k.delete_s
-000252d0: 6572 7669 6365 2866 227b 636c 7573 7465  ervice(f"{cluste
-000252e0: 727d 2d61 7069 222c 206b 2e6e 616d 6573  r}-api", k.names
-000252f0: 7061 6365 290a 2020 2020 2020 2020 2020  pace).          
-00025300: 2020 6966 2066 227b 636c 7573 7465 727d    if f"{cluster}
-00025310: 2d69 6e67 7265 7373 2220 696e 206b 2e6c  -ingress" in k.l
-00025320: 6973 745f 7365 7276 6963 6573 286b 2e6e  ist_services(k.n
-00025330: 616d 6573 7061 6365 293a 0a20 2020 2020  amespace):.     
-00025340: 2020 2020 2020 2020 2020 206b 2e64 656c             k.del
-00025350: 6574 655f 7365 7276 6963 6528 6622 7b63  ete_service(f"{c
-00025360: 6c75 7374 6572 7d2d 696e 6772 6573 7322  luster}-ingress"
-00025370: 2c20 6b2e 6e61 6d65 7370 6163 6529 0a20  , k.namespace). 
-00025380: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
-00025390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000253a0: 6361 6c6c 2866 276f 6320 6465 6c65 7465  call(f'oc delete
-000253b0: 202d 6e20 7b6b 2e6e 616d 6573 7061 6365   -n {k.namespace
-000253c0: 7d20 726f 7574 6520 7b63 6c75 7374 6572  } route {cluster
-000253d0: 7d2d 696e 6772 6573 7327 2c20 7368 656c  }-ingress', shel
-000253e0: 6c3d 5472 7565 290a 2020 2020 2020 2020  l=True).        
-000253f0: 2020 2020 6578 6365 7074 3a0a 2020 2020      except:.    
-00025400: 2020 2020 2020 2020 2020 2020 7061 7373              pass
-00025410: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00025420: 2e74 7970 6520 696e 205b 2761 7773 272c  .type in ['aws',
-00025430: 2027 617a 7572 6527 2c20 2767 6370 272c   'azure', 'gcp',
-00025440: 2027 6962 6d27 5d20 616e 6420 6e6f 7420   'ibm'] and not 
-00025450: 676b 6520 616e 6420 6e6f 7420 656b 7320  gke and not eks 
-00025460: 616e 6420 6e6f 7420 616b 733a 0a20 2020  and not aks:.   
-00025470: 2020 2020 2020 2020 2065 7869 7374 696e           existin
-00025480: 675f 6c62 7320 3d20 5b6c 5b30 5d20 666f  g_lbs = [l[0] fo
-00025490: 7220 6c20 696e 2073 656c 662e 6c69 7374  r l in self.list
-000254a0: 5f6c 6f61 6462 616c 616e 6365 7273 2829  _loadbalancers()
-000254b0: 2069 6620 6c5b 305d 2e65 6e64 7377 6974   if l[0].endswit
-000254c0: 6828 636c 7573 7465 7229 2061 6e64 0a20  h(cluster) and. 
+000250c0: 6272 6561 6b0a 2020 2020 2020 2020 2020  break.          
+000250d0: 2020 2020 2020 2020 2020 656c 6966 206b            elif k
+000250e0: 7562 6574 7970 6520 3d3d 2027 656b 7327  ubetype == 'eks'
+000250f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00025100: 2020 2020 2020 2020 2020 656b 7320 3d20            eks = 
+00025110: 5472 7565 0a20 2020 2020 2020 2020 2020  True.           
+00025120: 2020 2020 2020 2020 2020 2020 2062 7265               bre
+00025130: 616b 0a20 2020 2020 2020 2020 2020 2020  ak.             
+00025140: 2020 2020 2020 2065 6c69 6620 6b75 6265         elif kube
+00025150: 7479 7065 203d 3d20 2761 6b73 273a 0a20  type == 'aks':. 
+00025160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025170: 2020 2020 2020 2061 6b73 203d 2054 7275         aks = Tru
+00025180: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+00025190: 2020 2020 2020 2020 2020 6272 6561 6b0a            break.
+000251a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000251b0: 2020 2020 632e 6465 6c65 7465 286e 616d      c.delete(nam
+000251c0: 652c 2073 6e61 7073 686f 7473 3d54 7275  e, snapshots=Tru
+000251d0: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
+000251e0: 2020 2020 2020 2063 6f6d 6d6f 6e2e 6465         common.de
+000251f0: 6c65 7465 5f6c 6173 7476 6d28 6e61 6d65  lete_lastvm(name
+00025200: 2c20 7365 6c66 2e63 6c69 656e 7429 0a20  , self.client). 
+00025210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025220: 2020 2073 7563 6365 7373 2866 227b 6e61     success(f"{na
+00025230: 6d65 7d20 6465 6c65 7465 6420 6f6e 207b  me} deleted on {
+00025240: 6879 7065 7276 6973 6f72 7d21 2229 0a20  hypervisor}!"). 
+00025250: 2020 2020 2020 2069 6620 7365 6c66 2e74         if self.t
+00025260: 7970 6520 3d3d 2027 6b75 6265 7669 7274  ype == 'kubevirt
+00025270: 273a 0a20 2020 2020 2020 2020 2020 2069  ':.            i
+00025280: 6620 6622 7b63 6c75 7374 6572 7d2d 6170  f f"{cluster}-ap
+00025290: 6922 2069 6e20 6b2e 6c69 7374 5f73 6572  i" in k.list_ser
+000252a0: 7669 6365 7328 6b2e 6e61 6d65 7370 6163  vices(k.namespac
+000252b0: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
+000252c0: 2020 2020 6b2e 6465 6c65 7465 5f73 6572      k.delete_ser
+000252d0: 7669 6365 2866 227b 636c 7573 7465 727d  vice(f"{cluster}
+000252e0: 2d61 7069 222c 206b 2e6e 616d 6573 7061  -api", k.namespa
+000252f0: 6365 290a 2020 2020 2020 2020 2020 2020  ce).            
+00025300: 6966 2066 227b 636c 7573 7465 727d 2d69  if f"{cluster}-i
+00025310: 6e67 7265 7373 2220 696e 206b 2e6c 6973  ngress" in k.lis
+00025320: 745f 7365 7276 6963 6573 286b 2e6e 616d  t_services(k.nam
+00025330: 6573 7061 6365 293a 0a20 2020 2020 2020  espace):.       
+00025340: 2020 2020 2020 2020 206b 2e64 656c 6574           k.delet
+00025350: 655f 7365 7276 6963 6528 6622 7b63 6c75  e_service(f"{clu
+00025360: 7374 6572 7d2d 696e 6772 6573 7322 2c20  ster}-ingress", 
+00025370: 6b2e 6e61 6d65 7370 6163 6529 0a20 2020  k.namespace).   
+00025380: 2020 2020 2020 2020 2074 7279 3a0a 2020           try:.  
+00025390: 2020 2020 2020 2020 2020 2020 2020 6361                ca
+000253a0: 6c6c 2866 276f 6320 6465 6c65 7465 202d  ll(f'oc delete -
+000253b0: 6e20 7b6b 2e6e 616d 6573 7061 6365 7d20  n {k.namespace} 
+000253c0: 726f 7574 6520 7b63 6c75 7374 6572 7d2d  route {cluster}-
+000253d0: 696e 6772 6573 7327 2c20 7368 656c 6c3d  ingress', shell=
+000253e0: 5472 7565 290a 2020 2020 2020 2020 2020  True).          
+000253f0: 2020 6578 6365 7074 3a0a 2020 2020 2020    except:.      
+00025400: 2020 2020 2020 2020 2020 7061 7373 0a20            pass. 
+00025410: 2020 2020 2020 2069 6620 7365 6c66 2e74         if self.t
+00025420: 7970 6520 696e 205b 2761 7773 272c 2027  ype in ['aws', '
+00025430: 617a 7572 6527 2c20 2767 6370 272c 2027  azure', 'gcp', '
+00025440: 6962 6d27 5d20 616e 6420 6e6f 7420 676b  ibm'] and not gk
+00025450: 6520 616e 6420 6e6f 7420 656b 7320 616e  e and not eks an
+00025460: 6420 6e6f 7420 616b 733a 0a20 2020 2020  d not aks:.     
+00025470: 2020 2020 2020 2065 7869 7374 696e 675f         existing_
+00025480: 6c62 7320 3d20 5b6c 5b30 5d20 666f 7220  lbs = [l[0] for 
+00025490: 6c20 696e 2073 656c 662e 6c69 7374 5f6c  l in self.list_l
+000254a0: 6f61 6462 616c 616e 6365 7273 2829 2069  oadbalancers() i
+000254b0: 6620 6c5b 305d 2e65 6e64 7377 6974 6828  f l[0].endswith(
+000254c0: 636c 7573 7465 7229 2061 6e64 0a20 2020  cluster) and.   
 000254d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000254e0: 2020 2020 2020 2020 2020 2028 6c5b 305d             (l[0]
-000254f0: 2e73 7461 7274 7377 6974 6828 2761 7069  .startswith('api
-00025500: 2729 206f 7220 6c5b 305d 2e73 7461 7274  ') or l[0].start
-00025510: 7377 6974 6828 2761 7070 7327 2929 5d0a  swith('apps'))].
-00025520: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00025530: 6c62 2069 6e20 6578 6973 7469 6e67 5f6c  lb in existing_l
-00025540: 6273 3a0a 2020 2020 2020 2020 2020 2020  bs:.            
-00025550: 2020 2020 7365 6c66 2e64 656c 6574 655f      self.delete_
-00025560: 6c6f 6164 6261 6c61 6e63 6572 286c 622c  loadbalancer(lb,
-00025570: 2064 6f6d 6169 6e3d 646f 6d61 696e 290a   domain=domain).
-00025580: 2020 2020 2020 2020 2020 2020 6275 636b              buck
-00025590: 6574 203d 2066 227b 636c 7573 7465 727d  et = f"{cluster}
-000255a0: 2d7b 646f 6d61 696e 7d22 0a20 2020 2020  -{domain}".     
-000255b0: 2020 2020 2020 2069 6620 6275 636b 6574         if bucket
-000255c0: 2069 6e20 7365 6c66 2e6b 2e6c 6973 745f   in self.k.list_
-000255d0: 6275 636b 6574 7328 293a 0a20 2020 2020  buckets():.     
-000255e0: 2020 2020 2020 2020 2020 2070 7072 696e             pprin
-000255f0: 7428 6622 4465 6c65 7469 6e67 2062 7563  t(f"Deleting buc
-00025600: 6b65 7420 7b62 7563 6b65 747d 2229 0a20  ket {bucket}"). 
-00025610: 2020 2020 2020 2020 2020 2020 2020 206b                 k
-00025620: 2e64 656c 6574 655f 6275 636b 6574 2862  .delete_bucket(b
-00025630: 7563 6b65 7429 0a20 2020 2020 2020 2020  ucket).         
-00025640: 2020 2069 6620 7365 6c66 2e74 7970 6520     if self.type 
-00025650: 3d3d 2027 6177 7327 2061 6e64 2063 6c75  == 'aws' and clu
-00025660: 7374 6572 2069 6e20 6b2e 6c69 7374 5f69  ster in k.list_i
-00025670: 6e73 7461 6e63 655f 7072 6f66 696c 6573  nstance_profiles
-00025680: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-00025690: 2020 2020 6961 6d5f 726f 6c65 203d 2063      iam_role = c
-000256a0: 6c75 7374 6572 6461 7461 2e67 6574 2827  lusterdata.get('
-000256b0: 726f 6c65 272c 2063 6c75 7374 6572 290a  role', cluster).
-000256c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000256d0: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
-000256e0: 2020 2020 2020 2020 206b 2e64 656c 6574           k.delet
-000256f0: 655f 696e 7374 616e 6365 5f70 726f 6669  e_instance_profi
-00025700: 6c65 2863 6c75 7374 6572 2c20 6961 6d5f  le(cluster, iam_
-00025710: 726f 6c65 290a 2020 2020 2020 2020 2020  role).          
-00025720: 2020 2020 2020 6578 6365 7074 3a0a 2020        except:.  
+000254e0: 2020 2020 2020 2020 2028 6c5b 305d 2e73           (l[0].s
+000254f0: 7461 7274 7377 6974 6828 2761 7069 2729  tartswith('api')
+00025500: 206f 7220 6c5b 305d 2e73 7461 7274 7377   or l[0].startsw
+00025510: 6974 6828 2761 7070 7327 2929 5d0a 2020  ith('apps'))].  
+00025520: 2020 2020 2020 2020 2020 666f 7220 6c62            for lb
+00025530: 2069 6e20 6578 6973 7469 6e67 5f6c 6273   in existing_lbs
+00025540: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00025550: 2020 7365 6c66 2e64 656c 6574 655f 6c6f    self.delete_lo
+00025560: 6164 6261 6c61 6e63 6572 286c 622c 2064  adbalancer(lb, d
+00025570: 6f6d 6169 6e3d 646f 6d61 696e 290a 2020  omain=domain).  
+00025580: 2020 2020 2020 2020 2020 6275 636b 6574            bucket
+00025590: 203d 2066 227b 636c 7573 7465 727d 2d7b   = f"{cluster}-{
+000255a0: 646f 6d61 696e 7d22 0a20 2020 2020 2020  domain}".       
+000255b0: 2020 2020 2069 6620 6275 636b 6574 2069       if bucket i
+000255c0: 6e20 7365 6c66 2e6b 2e6c 6973 745f 6275  n self.k.list_bu
+000255d0: 636b 6574 7328 293a 0a20 2020 2020 2020  ckets():.       
+000255e0: 2020 2020 2020 2020 2070 7072 696e 7428           pprint(
+000255f0: 6622 4465 6c65 7469 6e67 2062 7563 6b65  f"Deleting bucke
+00025600: 7420 7b62 7563 6b65 747d 2229 0a20 2020  t {bucket}").   
+00025610: 2020 2020 2020 2020 2020 2020 206b 2e64               k.d
+00025620: 656c 6574 655f 6275 636b 6574 2862 7563  elete_bucket(buc
+00025630: 6b65 7429 0a20 2020 2020 2020 2020 2020  ket).           
+00025640: 2069 6620 7365 6c66 2e74 7970 6520 3d3d   if self.type ==
+00025650: 2027 6177 7327 2061 6e64 2063 6c75 7374   'aws' and clust
+00025660: 6572 2069 6e20 6b2e 6c69 7374 5f69 6e73  er in k.list_ins
+00025670: 7461 6e63 655f 7072 6f66 696c 6573 2829  tance_profiles()
+00025680: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00025690: 2020 6961 6d5f 726f 6c65 203d 2063 6c75    iam_role = clu
+000256a0: 7374 6572 6461 7461 2e67 6574 2827 726f  sterdata.get('ro
+000256b0: 6c65 272c 2063 6c75 7374 6572 290a 2020  le', cluster).  
+000256c0: 2020 2020 2020 2020 2020 2020 2020 7472                tr
+000256d0: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
+000256e0: 2020 2020 2020 206b 2e64 656c 6574 655f         k.delete_
+000256f0: 696e 7374 616e 6365 5f70 726f 6669 6c65  instance_profile
+00025700: 2863 6c75 7374 6572 2c20 6961 6d5f 726f  (cluster, iam_ro
+00025710: 6c65 290a 2020 2020 2020 2020 2020 2020  le).            
+00025720: 2020 2020 6578 6365 7074 3a0a 2020 2020      except:.    
 00025730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025740: 2020 7061 7373 0a20 2020 2020 2020 2020    pass.         
-00025750: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
-00025760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025770: 6b2e 6465 6c65 7465 5f72 6f6c 6528 6961  k.delete_role(ia
-00025780: 6d5f 726f 6c65 290a 2020 2020 2020 2020  m_role).        
-00025790: 2020 2020 2020 2020 6578 6365 7074 3a0a          except:.
+00025740: 7061 7373 0a20 2020 2020 2020 2020 2020  pass.           
+00025750: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+00025760: 2020 2020 2020 2020 2020 2020 2020 6b2e                k.
+00025770: 6465 6c65 7465 5f72 6f6c 6528 6961 6d5f  delete_role(iam_
+00025780: 726f 6c65 290a 2020 2020 2020 2020 2020  role).          
+00025790: 2020 2020 2020 6578 6365 7074 3a0a 2020        except:.  
 000257a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000257b0: 2020 2020 7061 7373 0a20 2020 2020 2020      pass.       
-000257c0: 2020 2020 2069 6620 7365 6c66 2e74 7970       if self.typ
-000257d0: 6520 3d3d 2027 6763 7027 2061 6e64 206b  e == 'gcp' and k
-000257e0: 7562 6574 7970 6520 3d3d 2027 6f70 656e  ubetype == 'open
-000257f0: 7368 6966 7427 2061 6e64 206f 732e 7061  shift' and os.pa
-00025800: 7468 2e65 7869 7374 7328 6627 7b63 6c75  th.exists(f'{clu
-00025810: 7374 6572 6469 727d 2f6d 6574 6164 6174  sterdir}/metadat
-00025820: 612e 6a73 6f6e 2729 3a0a 2020 2020 2020  a.json'):.      
-00025830: 2020 2020 2020 2020 2020 636c 7573 7465            cluste
-00025840: 725f 6964 203d 2079 616d 6c2e 7361 6665  r_id = yaml.safe
-00025850: 5f6c 6f61 6428 6f70 656e 2866 277b 636c  _load(open(f'{cl
-00025860: 7573 7465 7264 6972 7d2f 6d65 7461 6461  usterdir}/metada
-00025870: 7461 2e6a 736f 6e27 2929 5b27 696e 6672  ta.json'))['infr
-00025880: 6149 4427 5d0a 2020 2020 2020 2020 2020  aID'].          
-00025890: 2020 2020 2020 6b2e 6465 6c65 7465 5f73        k.delete_s
-000258a0: 6572 7669 6365 5f61 6363 6f75 6e74 7328  ervice_accounts(
-000258b0: 636c 7573 7465 725f 6964 290a 2020 2020  cluster_id).    
-000258c0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000258d0: 7479 7065 2069 6e20 5b27 6177 7327 2c20  type in ['aws', 
-000258e0: 2767 6370 275d 3a0a 2020 2020 2020 2020  'gcp']:.        
-000258f0: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
-00025900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025910: 2073 656c 662e 6b2e 6465 6c65 7465 5f73   self.k.delete_s
-00025920: 6563 7572 6974 795f 6772 6f75 7028 636c  ecurity_group(cl
-00025930: 7573 7465 7229 0a20 2020 2020 2020 2020  uster).         
-00025940: 2020 2020 2020 2065 7863 6570 743a 0a20         except:. 
+000257b0: 2020 7061 7373 0a20 2020 2020 2020 2020    pass.         
+000257c0: 2020 2069 6620 7365 6c66 2e74 7970 6520     if self.type 
+000257d0: 3d3d 2027 6763 7027 2061 6e64 206b 7562  == 'gcp' and kub
+000257e0: 6574 7970 6520 3d3d 2027 6f70 656e 7368  etype == 'opensh
+000257f0: 6966 7427 2061 6e64 206f 732e 7061 7468  ift' and os.path
+00025800: 2e65 7869 7374 7328 6627 7b63 6c75 7374  .exists(f'{clust
+00025810: 6572 6469 727d 2f6d 6574 6164 6174 612e  erdir}/metadata.
+00025820: 6a73 6f6e 2729 3a0a 2020 2020 2020 2020  json'):.        
+00025830: 2020 2020 2020 2020 636c 7573 7465 725f          cluster_
+00025840: 6964 203d 2079 616d 6c2e 7361 6665 5f6c  id = yaml.safe_l
+00025850: 6f61 6428 6f70 656e 2866 277b 636c 7573  oad(open(f'{clus
+00025860: 7465 7264 6972 7d2f 6d65 7461 6461 7461  terdir}/metadata
+00025870: 2e6a 736f 6e27 2929 5b27 696e 6672 6149  .json'))['infraI
+00025880: 4427 5d0a 2020 2020 2020 2020 2020 2020  D'].            
+00025890: 2020 2020 6b2e 6465 6c65 7465 5f73 6572      k.delete_ser
+000258a0: 7669 6365 5f61 6363 6f75 6e74 7328 636c  vice_accounts(cl
+000258b0: 7573 7465 725f 6964 290a 2020 2020 2020  uster_id).      
+000258c0: 2020 2020 2020 6966 2073 656c 662e 7479        if self.ty
+000258d0: 7065 2069 6e20 5b27 6177 7327 2c20 2767  pe in ['aws', 'g
+000258e0: 6370 275d 3a0a 2020 2020 2020 2020 2020  cp']:.          
+000258f0: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
+00025900: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00025910: 656c 662e 6b2e 6465 6c65 7465 5f73 6563  elf.k.delete_sec
+00025920: 7572 6974 795f 6772 6f75 7028 636c 7573  urity_group(clus
+00025930: 7465 7229 0a20 2020 2020 2020 2020 2020  ter).           
+00025940: 2020 2020 2065 7863 6570 743a 0a20 2020       except:.   
 00025950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025960: 2020 2070 6173 730a 2020 2020 2020 2020     pass.        
-00025970: 2020 2020 6966 2073 656c 662e 7479 7065      if self.type
-00025980: 203d 3d20 2761 7a75 7265 273a 0a20 2020   == 'azure':.   
-00025990: 2020 2020 2020 2020 2020 2020 2074 7279               try
-000259a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000259b0: 2020 2020 2020 7365 6c66 2e6b 2e64 656c        self.k.del
-000259c0: 6574 655f 6964 656e 7469 7479 2866 276b  ete_identity(f'k
-000259d0: 636c 692d 7b63 6c75 7374 6572 7d27 290a  cli-{cluster}').
-000259e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000259f0: 6578 6365 7074 3a0a 2020 2020 2020 2020  except:.        
-00025a00: 2020 2020 2020 2020 2020 2020 7061 7373              pass
-00025a10: 0a20 2020 2020 2020 2065 6c69 6620 646e  .        elif dn
-00025a20: 7363 6c69 656e 7420 6973 206e 6f74 204e  sclient is not N
-00025a30: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00025a40: 207a 203d 204b 636f 6e66 6967 2863 6c69   z = Kconfig(cli
-00025a50: 656e 743d 646e 7363 6c69 656e 7429 2e6b  ent=dnsclient).k
-00025a60: 0a20 2020 2020 2020 2020 2020 207a 2e64  .            z.d
-00025a70: 656c 6574 655f 646e 7328 6622 6170 692e  elete_dns(f"api.
-00025a80: 7b63 6c75 7374 6572 7d22 2c20 646f 6d61  {cluster}", doma
-00025a90: 696e 290a 2020 2020 2020 2020 2020 2020  in).            
-00025aa0: 7a2e 6465 6c65 7465 5f64 6e73 2866 2261  z.delete_dns(f"a
-00025ab0: 7070 732e 7b63 6c75 7374 6572 7d22 2c20  pps.{cluster}", 
-00025ac0: 646f 6d61 696e 290a 2020 2020 2020 2020  domain).        
-00025ad0: 6966 2068 7970 6572 7368 6966 743a 0a20  if hypershift:. 
-00025ae0: 2020 2020 2020 2020 2020 206b 7562 6563             kubec
-00025af0: 6f6e 6669 676d 676d 7420 3d20 6622 7b63  onfigmgmt = f"{c
-00025b00: 6c75 7374 6572 6469 727d 2f6b 7562 6563  lusterdir}/kubec
-00025b10: 6f6e 6669 672e 6d67 6d74 220a 2020 2020  onfig.mgmt".    
-00025b20: 2020 2020 2020 2020 6966 206f 732e 7061          if os.pa
-00025b30: 7468 2e65 7869 7374 7328 6627 7b63 6c75  th.exists(f'{clu
-00025b40: 7374 6572 6469 727d 2f62 6d63 732e 796d  sterdir}/bmcs.ym
-00025b50: 6c27 293a 0a20 2020 2020 2020 2020 2020  l'):.           
-00025b60: 2020 2020 2063 616c 6c28 6627 4b55 4245       call(f'KUBE
-00025b70: 434f 4e46 4947 3d7b 6b75 6265 636f 6e66  CONFIG={kubeconf
-00025b80: 6967 6d67 6d74 7d20 6f63 2064 656c 6574  igmgmt} oc delet
-00025b90: 6520 2d66 207b 636c 7573 7465 7264 6972  e -f {clusterdir
-00025ba0: 7d2f 626d 6373 2e79 6d6c 272c 2073 6865  }/bmcs.yml', she
-00025bb0: 6c6c 3d54 7275 6529 0a20 2020 2020 2020  ll=True).       
-00025bc0: 2020 2020 2063 616c 6c28 6627 4b55 4245       call(f'KUBE
-00025bd0: 434f 4e46 4947 3d7b 6b75 6265 636f 6e66  CONFIG={kubeconf
-00025be0: 6967 6d67 6d74 7d20 6f63 2064 656c 6574  igmgmt} oc delet
-00025bf0: 6520 2d66 207b 636c 7573 7465 7264 6972  e -f {clusterdir
-00025c00: 7d2f 6175 746f 6170 7072 6f76 6572 6372  }/autoapprovercr
-00025c10: 6f6e 2e79 6d6c 272c 2073 6865 6c6c 3d54  on.yml', shell=T
-00025c20: 7275 6529 0a20 2020 2020 2020 2020 2020  rue).           
-00025c30: 2063 616c 6c28 6627 4b55 4245 434f 4e46   call(f'KUBECONF
-00025c40: 4947 3d7b 6b75 6265 636f 6e66 6967 6d67  IG={kubeconfigmg
-00025c50: 6d74 7d20 6f63 2064 656c 6574 6520 2d66  mt} oc delete -f
-00025c60: 207b 636c 7573 7465 7264 6972 7d2f 6e6f   {clusterdir}/no
-00025c70: 6465 706f 6f6c 2e79 616d 6c27 2c20 7368  depool.yaml', sh
-00025c80: 656c 6c3d 5472 7565 290a 2020 2020 2020  ell=True).      
-00025c90: 2020 2020 2020 6361 6c6c 2866 274b 5542        call(f'KUB
-00025ca0: 4543 4f4e 4649 473d 7b6b 7562 6563 6f6e  ECONFIG={kubecon
-00025cb0: 6669 676d 676d 747d 206f 6320 6465 6c65  figmgmt} oc dele
-00025cc0: 7465 202d 6620 7b63 6c75 7374 6572 6469  te -f {clusterdi
-00025cd0: 727d 2f68 6f73 7465 6463 6c75 7374 6572  r}/hostedcluster
-00025ce0: 2e79 616d 6c27 2c20 7368 656c 6c3d 5472  .yaml', shell=Tr
-00025cf0: 7565 290a 2020 2020 2020 2020 2020 2020  ue).            
-00025d00: 6966 206f 732e 7061 7468 2e65 7869 7374  if os.path.exist
-00025d10: 7328 6627 7b63 6c75 7374 6572 6469 727d  s(f'{clusterdir}
-00025d20: 2f61 7373 6973 7465 645f 696e 6672 612e  /assisted_infra.
-00025d30: 796d 6c27 293a 0a20 2020 2020 2020 2020  yml'):.         
-00025d40: 2020 2020 2020 2063 616c 6c28 6627 4b55         call(f'KU
-00025d50: 4245 434f 4e46 4947 3d7b 6b75 6265 636f  BECONFIG={kubeco
-00025d60: 6e66 6967 6d67 6d74 7d20 6f63 2064 656c  nfigmgmt} oc del
-00025d70: 6574 6520 2d66 207b 636c 7573 7465 7264  ete -f {clusterd
-00025d80: 6972 7d2f 6173 7369 7374 6564 5f69 6e66  ir}/assisted_inf
-00025d90: 7261 2e79 6d6c 272c 2073 6865 6c6c 3d54  ra.yml', shell=T
-00025da0: 7275 6529 0a20 2020 2020 2020 2020 2020  rue).           
-00025db0: 2069 6620 6e6f 7420 6173 7369 7374 6564   if not assisted
-00025dc0: 2061 6e64 2028 2762 6172 656d 6574 616c   and ('baremetal
-00025dd0: 5f69 736f 2720 696e 2063 6c75 7374 6572  _iso' in cluster
-00025de0: 6461 7461 206f 7220 2762 6172 656d 6574  data or 'baremet
-00025df0: 616c 5f68 6f73 7473 2720 696e 2063 6c75  al_hosts' in clu
-00025e00: 7374 6572 6461 7461 293a 0a20 2020 2020  sterdata):.     
-00025e10: 2020 2020 2020 2020 2020 2063 616c 6c28             call(
-00025e20: 6627 4b55 4245 434f 4e46 4947 3d7b 6b75  f'KUBECONFIG={ku
-00025e30: 6265 636f 6e66 6967 6d67 6d74 7d20 6f63  beconfigmgmt} oc
-00025e40: 202d 6e20 6465 6661 756c 7420 6465 6c65   -n default dele
-00025e50: 7465 2061 6c6c 202d 6c20 6170 703d 6874  te all -l app=ht
-00025e60: 7470 642d 6b63 6c69 272c 2073 6865 6c6c  tpd-kcli', shell
-00025e70: 3d54 7275 6529 0a20 2020 2020 2020 2020  =True).         
-00025e80: 2020 2020 2020 2063 616c 6c28 6627 4b55         call(f'KU
-00025e90: 4245 434f 4e46 4947 3d7b 6b75 6265 636f  BECONFIG={kubeco
-00025ea0: 6e66 6967 6d67 6d74 7d20 6f63 202d 6e20  nfigmgmt} oc -n 
-00025eb0: 6465 6661 756c 7420 6465 6c65 7465 2070  default delete p
-00025ec0: 7663 2068 7474 7064 2d6b 636c 692d 7076  vc httpd-kcli-pv
-00025ed0: 6327 2c20 7368 656c 6c3d 5472 7565 290a  c', shell=True).
-00025ee0: 2020 2020 2020 2020 2020 2020 696e 6772              ingr
-00025ef0: 6573 735f 6970 203d 2063 6c75 7374 6572  ess_ip = cluster
-00025f00: 6461 7461 2e67 6574 2827 696e 6772 6573  data.get('ingres
-00025f10: 735f 6970 2729 0a20 2020 2020 2020 2020  s_ip').         
-00025f20: 2020 2069 6620 7365 6c66 2e74 7970 6520     if self.type 
-00025f30: 3d3d 2027 6b75 6265 7669 7274 2720 616e  == 'kubevirt' an
-00025f40: 6420 636c 7573 7465 7264 6174 612e 6765  d clusterdata.ge
-00025f50: 7428 2770 6c61 7466 6f72 6d27 2920 6973  t('platform') is
-00025f60: 204e 6f6e 6520 616e 6420 696e 6772 6573   None and ingres
-00025f70: 735f 6970 2069 7320 4e6f 6e65 3a0a 2020  s_ip is None:.  
-00025f80: 2020 2020 2020 2020 2020 2020 2020 6361                ca
-00025f90: 6c6c 2866 274b 5542 4543 4f4e 4649 473d  ll(f'KUBECONFIG=
-00025fa0: 7b6b 7562 6563 6f6e 6669 676d 676d 747d  {kubeconfigmgmt}
-00025fb0: 206f 6320 2d6e 207b 6b2e 6e61 6d65 7370   oc -n {k.namesp
-00025fc0: 6163 657d 2064 656c 6574 6520 726f 7574  ace} delete rout
-00025fd0: 6520 7b63 6c75 7374 6572 7d2d 696e 6772  e {cluster}-ingr
-00025fe0: 6573 7327 2c20 7368 656c 6c3d 5472 7565  ess', shell=True
-00025ff0: 290a 2020 2020 2020 2020 6966 2067 6b65  ).        if gke
-00026000: 3a0a 2020 2020 2020 2020 2020 2020 6763  :.            gc
-00026010: 7063 6c69 656e 7420 3d20 4e6f 6e65 0a20  pclient = None. 
-00026020: 2020 2020 2020 2020 2020 2069 6620 2763             if 'c
-00026030: 6c69 656e 7427 2069 6e20 636c 7573 7465  lient' in cluste
-00026040: 7264 6174 613a 0a20 2020 2020 2020 2020  rdata:.         
-00026050: 2020 2020 2020 2067 6370 636c 6965 6e74         gcpclient
-00026060: 203d 2063 6c75 7374 6572 6461 7461 5b27   = clusterdata['
-00026070: 636c 6965 6e74 275d 0a20 2020 2020 2020  client'].       
-00026080: 2020 2020 2065 6c69 6620 7365 6c66 2e74       elif self.t
-00026090: 7970 6520 3d3d 2027 6763 7027 3a0a 2020  ype == 'gcp':.  
-000260a0: 2020 2020 2020 2020 2020 2020 2020 6763                gc
-000260b0: 7063 6c69 656e 7420 3d20 7365 6c66 2e63  pclient = self.c
-000260c0: 6c69 656e 740a 2020 2020 2020 2020 2020  lient.          
-000260d0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-000260e0: 2020 2020 2020 2020 6d73 6720 3d20 2244          msg = "D
-000260f0: 656c 6574 696e 6720 676b 6520 636c 7573  eleting gke clus
-00026100: 7465 7220 7265 7175 6972 6573 2074 6f20  ter requires to 
-00026110: 696e 7374 616e 7469 6174 6520 6763 7020  instantiate gcp 
-00026120: 7072 6f76 6964 6572 220a 2020 2020 2020  provider".      
-00026130: 2020 2020 2020 2020 2020 6572 726f 7228            error(
-00026140: 6d73 6729 0a20 2020 2020 2020 2020 2020  msg).           
-00026150: 2020 2020 2072 6574 7572 6e20 7b27 7265       return {'re
-00026160: 7375 6c74 273a 2027 6661 696c 7572 6527  sult': 'failure'
-00026170: 2c20 2772 6561 736f 6e27 3a20 6d73 677d  , 'reason': msg}
-00026180: 0a20 2020 2020 2020 2020 2020 2066 726f  .            fro
-00026190: 6d20 6b76 6972 742e 636c 7573 7465 7220  m kvirt.cluster 
-000261a0: 696d 706f 7274 2067 6b65 0a20 2020 2020  import gke.     
-000261b0: 2020 2020 2020 2063 7572 7265 6e74 636f         currentco
-000261c0: 6e66 6967 203d 204b 636f 6e66 6967 2863  nfig = Kconfig(c
-000261d0: 6c69 656e 743d 6763 7063 6c69 656e 7429  lient=gcpclient)
-000261e0: 2e6b 2069 6620 6763 7063 6c69 656e 7420  .k if gcpclient 
-000261f0: 213d 2073 656c 662e 636c 6965 6e74 2065  != self.client e
-00026200: 6c73 6520 7365 6c66 0a20 2020 2020 2020  lse self.       
-00026210: 2020 2020 207a 6f6e 616c 203d 2063 6c75       zonal = clu
-00026220: 7374 6572 6461 7461 2e67 6574 2827 7a6f  sterdata.get('zo
-00026230: 6e61 6c27 2c20 5472 7565 290a 2020 2020  nal', True).    
-00026240: 2020 2020 2020 2020 676b 652e 6465 6c65          gke.dele
-00026250: 7465 2863 7572 7265 6e74 636f 6e66 6967  te(currentconfig
-00026260: 2c20 636c 7573 7465 722c 207a 6f6e 616c  , cluster, zonal
-00026270: 290a 2020 2020 2020 2020 656c 6966 2065  ).        elif e
-00026280: 6b73 3a0a 2020 2020 2020 2020 2020 2020  ks:.            
-00026290: 656b 7363 6c69 656e 7420 3d20 4e6f 6e65  eksclient = None
-000262a0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-000262b0: 2763 6c69 656e 7427 2069 6e20 636c 7573  'client' in clus
-000262c0: 7465 7264 6174 613a 0a20 2020 2020 2020  terdata:.       
-000262d0: 2020 2020 2020 2020 2065 6b73 636c 6965           eksclie
-000262e0: 6e74 203d 2063 6c75 7374 6572 6461 7461  nt = clusterdata
-000262f0: 5b27 636c 6965 6e74 275d 0a20 2020 2020  ['client'].     
-00026300: 2020 2020 2020 2065 6c69 6620 7365 6c66         elif self
-00026310: 2e74 7970 6520 3d3d 2027 6177 7327 3a0a  .type == 'aws':.
-00026320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026330: 656b 7363 6c69 656e 7420 3d20 7365 6c66  eksclient = self
-00026340: 2e63 6c69 656e 740a 2020 2020 2020 2020  .client.        
-00026350: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00026360: 2020 2020 2020 2020 2020 6d73 6720 3d20            msg = 
-00026370: 2244 656c 6574 696e 6720 656b 7320 636c  "Deleting eks cl
-00026380: 7573 7465 7220 7265 7175 6972 6573 2074  uster requires t
-00026390: 6f20 696e 7374 616e 7469 6174 6520 6177  o instantiate aw
-000263a0: 7320 7072 6f76 6964 6572 220a 2020 2020  s provider".    
-000263b0: 2020 2020 2020 2020 2020 2020 6572 726f              erro
-000263c0: 7228 6d73 6729 0a20 2020 2020 2020 2020  r(msg).         
-000263d0: 2020 2020 2020 2072 6574 7572 6e20 7b27         return {'
-000263e0: 7265 7375 6c74 273a 2027 6661 696c 7572  result': 'failur
-000263f0: 6527 2c20 2772 6561 736f 6e27 3a20 6d73  e', 'reason': ms
-00026400: 677d 0a20 2020 2020 2020 2020 2020 2066  g}.            f
-00026410: 726f 6d20 6b76 6972 742e 636c 7573 7465  rom kvirt.cluste
-00026420: 7220 696d 706f 7274 2065 6b73 0a20 2020  r import eks.   
-00026430: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-00026440: 636f 6e66 6967 203d 204b 636f 6e66 6967  config = Kconfig
-00026450: 2863 6c69 656e 743d 656b 7363 6c69 656e  (client=eksclien
-00026460: 7429 2e6b 2069 6620 656b 7363 6c69 656e  t).k if eksclien
-00026470: 7420 213d 2073 656c 662e 636c 6965 6e74  t != self.client
-00026480: 2065 6c73 6520 7365 6c66 0a20 2020 2020   else self.     
-00026490: 2020 2020 2020 2065 6b73 2e64 656c 6574         eks.delet
-000264a0: 6528 6375 7272 656e 7463 6f6e 6669 672c  e(currentconfig,
-000264b0: 2063 6c75 7374 6572 290a 2020 2020 2020   cluster).      
-000264c0: 2020 656c 6966 2061 6b73 3a0a 2020 2020    elif aks:.    
-000264d0: 2020 2020 2020 2020 616b 7363 6c69 656e          aksclien
-000264e0: 7420 3d20 4e6f 6e65 0a20 2020 2020 2020  t = None.       
-000264f0: 2020 2020 2069 6620 2763 6c69 656e 7427       if 'client'
-00026500: 2069 6e20 636c 7573 7465 7264 6174 613a   in clusterdata:
-00026510: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00026520: 2061 6b73 636c 6965 6e74 203d 2063 6c75   aksclient = clu
-00026530: 7374 6572 6461 7461 5b27 636c 6965 6e74  sterdata['client
-00026540: 275d 0a20 2020 2020 2020 2020 2020 2065  '].            e
-00026550: 6c69 6620 7365 6c66 2e74 7970 6520 3d3d  lif self.type ==
-00026560: 2027 617a 7572 6527 3a0a 2020 2020 2020   'azure':.      
-00026570: 2020 2020 2020 2020 2020 616b 7363 6c69            akscli
-00026580: 656e 7420 3d20 7365 6c66 2e63 6c69 656e  ent = self.clien
-00026590: 740a 2020 2020 2020 2020 2020 2020 656c  t.            el
-000265a0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-000265b0: 2020 2020 6d73 6720 3d20 2244 656c 6574      msg = "Delet
-000265c0: 696e 6720 616b 7320 636c 7573 7465 7220  ing aks cluster 
-000265d0: 7265 7175 6972 6573 2074 6f20 696e 7374  requires to inst
-000265e0: 616e 7469 6174 6520 617a 7572 6520 7072  antiate azure pr
-000265f0: 6f76 6964 6572 220a 2020 2020 2020 2020  ovider".        
-00026600: 2020 2020 2020 2020 6572 726f 7228 6d73          error(ms
-00026610: 6729 0a20 2020 2020 2020 2020 2020 2020  g).             
-00026620: 2020 2072 6574 7572 6e20 7b27 7265 7375     return {'resu
-00026630: 6c74 273a 2027 6661 696c 7572 6527 2c20  lt': 'failure', 
-00026640: 2772 6561 736f 6e27 3a20 6d73 677d 0a20  'reason': msg}. 
-00026650: 2020 2020 2020 2020 2020 2066 726f 6d20             from 
-00026660: 6b76 6972 742e 636c 7573 7465 7220 696d  kvirt.cluster im
-00026670: 706f 7274 2061 6b73 0a20 2020 2020 2020  port aks.       
-00026680: 2020 2020 2063 7572 7265 6e74 636f 6e66       currentconf
-00026690: 6967 203d 204b 636f 6e66 6967 2863 6c69  ig = Kconfig(cli
-000266a0: 656e 743d 616b 7363 6c69 656e 7429 2e6b  ent=aksclient).k
-000266b0: 2069 6620 616b 7363 6c69 656e 7420 213d   if aksclient !=
-000266c0: 2073 656c 662e 636c 6965 6e74 2065 6c73   self.client els
-000266d0: 6520 7365 6c66 0a20 2020 2020 2020 2020  e self.         
-000266e0: 2020 2061 6b73 2e64 656c 6574 6528 6375     aks.delete(cu
-000266f0: 7272 656e 7463 6f6e 6669 672c 2063 6c75  rrentconfig, clu
-00026700: 7374 6572 290a 2020 2020 2020 2020 666f  ster).        fo
-00026710: 7220 636f 6e66 706f 6f6c 2069 6e20 7365  r confpool in se
-00026720: 6c66 2e63 6f6e 6670 6f6f 6c73 3a0a 2020  lf.confpools:.  
-00026730: 2020 2020 2020 2020 2020 6970 5f72 6573            ip_res
-00026740: 6572 7661 7469 6f6e 7320 3d20 7365 6c66  ervations = self
-00026750: 2e63 6f6e 6670 6f6f 6c73 5b63 6f6e 6670  .confpools[confp
-00026760: 6f6f 6c5d 2e67 6574 2827 6970 5f72 6573  ool].get('ip_res
-00026770: 6572 7661 7469 6f6e 7327 2c20 7b7d 290a  ervations', {}).
-00026780: 2020 2020 2020 2020 2020 2020 6966 2063              if c
-00026790: 6c75 7374 6572 2069 6e20 6970 5f72 6573  luster in ip_res
-000267a0: 6572 7661 7469 6f6e 733a 0a20 2020 2020  ervations:.     
-000267b0: 2020 2020 2020 2020 2020 2064 656c 2069             del i
-000267c0: 705f 7265 7365 7276 6174 696f 6e73 5b63  p_reservations[c
-000267d0: 6c75 7374 6572 5d0a 2020 2020 2020 2020  luster].        
-000267e0: 2020 2020 2020 2020 7365 6c66 2e75 7064          self.upd
-000267f0: 6174 655f 636f 6e66 706f 6f6c 2863 6f6e  ate_confpool(con
-00026800: 6670 6f6f 6c2c 207b 2769 705f 7265 7365  fpool, {'ip_rese
-00026810: 7276 6174 696f 6e73 273a 2069 705f 7265  rvations': ip_re
-00026820: 7365 7276 6174 696f 6e73 7d29 0a20 2020  servations}).   
-00026830: 2020 2020 2020 2020 206e 616d 655f 7265           name_re
-00026840: 7365 7276 6174 696f 6e73 203d 2073 656c  servations = sel
-00026850: 662e 636f 6e66 706f 6f6c 735b 636f 6e66  f.confpools[conf
-00026860: 706f 6f6c 5d2e 6765 7428 276e 616d 655f  pool].get('name_
-00026870: 7265 7365 7276 6174 696f 6e73 272c 205b  reservations', [
-00026880: 5d29 0a20 2020 2020 2020 2020 2020 2069  ]).            i
-00026890: 6620 636c 7573 7465 7220 696e 206e 616d  f cluster in nam
-000268a0: 655f 7265 7365 7276 6174 696f 6e73 3a0a  e_reservations:.
-000268b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000268c0: 6e61 6d65 5f72 6573 6572 7661 7469 6f6e  name_reservation
-000268d0: 732e 7265 6d6f 7665 2863 6c75 7374 6572  s.remove(cluster
-000268e0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000268f0: 2020 7365 6c66 2e75 7064 6174 655f 636f    self.update_co
-00026900: 6e66 706f 6f6c 2863 6f6e 6670 6f6f 6c2c  nfpool(confpool,
-00026910: 207b 276e 616d 655f 7265 7365 7276 6174   {'name_reservat
-00026920: 696f 6e73 273a 206e 616d 655f 7265 7365  ions': name_rese
-00026930: 7276 6174 696f 6e73 7d29 0a20 2020 2020  rvations}).     
-00026940: 2020 2020 2020 2063 6c75 7374 6572 5f62         cluster_b
-00026950: 6172 656d 6574 616c 5f72 6573 6572 7661  aremetal_reserva
-00026960: 7469 6f6e 7320 3d20 7365 6c66 2e63 6f6e  tions = self.con
-00026970: 6670 6f6f 6c73 5b63 6f6e 6670 6f6f 6c5d  fpools[confpool]
-00026980: 2e67 6574 2827 636c 7573 7465 725f 6261  .get('cluster_ba
-00026990: 7265 6d65 7461 6c5f 7265 7365 7276 6174  remetal_reservat
-000269a0: 696f 6e73 272c 207b 7d29 0a20 2020 2020  ions', {}).     
-000269b0: 2020 2020 2020 2069 6620 636c 7573 7465         if cluste
-000269c0: 7220 696e 2063 6c75 7374 6572 5f62 6172  r in cluster_bar
-000269d0: 656d 6574 616c 5f72 6573 6572 7661 7469  emetal_reservati
-000269e0: 6f6e 733a 0a20 2020 2020 2020 2020 2020  ons:.           
-000269f0: 2020 2020 2064 656c 2063 6c75 7374 6572       del cluster
-00026a00: 5f62 6172 656d 6574 616c 5f72 6573 6572  _baremetal_reser
-00026a10: 7661 7469 6f6e 735b 636c 7573 7465 725d  vations[cluster]
-00026a20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00026a30: 2073 656c 662e 7570 6461 7465 5f63 6f6e   self.update_con
-00026a40: 6670 6f6f 6c28 636f 6e66 706f 6f6c 2c20  fpool(confpool, 
-00026a50: 7b27 636c 7573 7465 725f 6261 7265 6d65  {'cluster_bareme
-00026a60: 7461 6c5f 7265 7365 7276 6174 696f 6e73  tal_reservations
-00026a70: 273a 2063 6c75 7374 6572 5f62 6172 656d  ': cluster_barem
-00026a80: 6574 616c 5f72 6573 6572 7661 7469 6f6e  etal_reservation
-00026a90: 737d 290a 2020 2020 2020 2020 6966 206f  s}).        if o
-00026aa0: 732e 7061 7468 2e65 7869 7374 7328 636c  s.path.exists(cl
-00026ab0: 7573 7465 7264 6972 293a 0a20 2020 2020  usterdir):.     
-00026ac0: 2020 2020 2020 2070 7072 696e 7428 6622         pprint(f"
-00026ad0: 4465 6c65 7469 6e67 2064 6972 6563 746f  Deleting directo
-00026ae0: 7279 207b 636c 7573 7465 7264 6972 7d22  ry {clusterdir}"
-00026af0: 290a 2020 2020 2020 2020 2020 2020 726d  ).            rm
-00026b00: 7472 6565 2863 6c75 7374 6572 6469 7229  tree(clusterdir)
-00026b10: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00026b20: 7b27 7265 7375 6c74 273a 2027 7375 6363  {'result': 'succ
-00026b30: 6573 7327 7d0a 0a20 2020 2064 6566 2073  ess'}..    def s
-00026b40: 6361 6c65 5f6b 7562 6528 7365 6c66 2c20  cale_kube(self, 
-00026b50: 636c 7573 7465 722c 206b 7562 6574 7970  cluster, kubetyp
-00026b60: 652c 206f 7665 7272 6964 6573 3d7b 7d29  e, overrides={})
-00026b70: 3a0a 2020 2020 2020 2020 6966 206b 7562  :.        if kub
-00026b80: 6574 7970 6520 3d3d 2027 6765 6e65 7269  etype == 'generi
-00026b90: 6327 3a0a 2020 2020 2020 2020 2020 2020  c':.            
-00026ba0: 7265 7375 6c74 203d 2073 656c 662e 7363  result = self.sc
-00026bb0: 616c 655f 6b75 6265 5f67 656e 6572 6963  ale_kube_generic
-00026bc0: 2863 6c75 7374 6572 2c20 6f76 6572 7269  (cluster, overri
-00026bd0: 6465 733d 6f76 6572 7269 6465 7329 0a20  des=overrides). 
-00026be0: 2020 2020 2020 2065 6c69 6620 6b75 6265         elif kube
-00026bf0: 7479 7065 203d 3d20 276b 3373 273a 0a20  type == 'k3s':. 
-00026c00: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-00026c10: 7420 3d20 7365 6c66 2e73 6361 6c65 5f6b  t = self.scale_k
-00026c20: 7562 655f 6b33 7328 636c 7573 7465 722c  ube_k3s(cluster,
-00026c30: 206f 7665 7272 6964 6573 3d6f 7665 7272   overrides=overr
-00026c40: 6964 6573 290a 2020 2020 2020 2020 656c  ides).        el
-00026c50: 6966 206b 7562 6574 7970 6520 3d3d 2027  if kubetype == '
-00026c60: 6f70 656e 7368 6966 7427 3a0a 2020 2020  openshift':.    
-00026c70: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
-00026c80: 2073 656c 662e 7363 616c 655f 6b75 6265   self.scale_kube
-00026c90: 5f6f 7065 6e73 6869 6674 2863 6c75 7374  _openshift(clust
-00026ca0: 6572 2c20 6f76 6572 7269 6465 733d 6f76  er, overrides=ov
-00026cb0: 6572 7269 6465 7329 0a20 2020 2020 2020  errides).       
-00026cc0: 2065 6c69 6620 6b75 6265 7479 7065 203d   elif kubetype =
-00026cd0: 3d20 2768 7970 6572 7368 6966 7427 3a0a  = 'hypershift':.
-00026ce0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00026cf0: 6c74 203d 2073 656c 662e 7363 616c 655f  lt = self.scale_
-00026d00: 6b75 6265 5f68 7970 6572 7368 6966 7428  kube_hypershift(
-00026d10: 636c 7573 7465 722c 206f 7665 7272 6964  cluster, overrid
-00026d20: 6573 3d6f 7665 7272 6964 6573 290a 2020  es=overrides).  
-00026d30: 2020 2020 2020 656c 6966 206b 7562 6574        elif kubet
-00026d40: 7970 6520 3d3d 2027 676b 6527 3a0a 2020  ype == 'gke':.  
-00026d50: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00026d60: 203d 2073 656c 662e 7363 616c 655f 6b75   = self.scale_ku
-00026d70: 6265 5f67 6b65 2863 6c75 7374 6572 2c20  be_gke(cluster, 
-00026d80: 6f76 6572 7269 6465 733d 6f76 6572 7269  overrides=overri
-00026d90: 6465 7329 0a20 2020 2020 2020 2065 6c69  des).        eli
-00026da0: 6620 6b75 6265 7479 7065 203d 3d20 2765  f kubetype == 'e
-00026db0: 6b73 273a 0a20 2020 2020 2020 2020 2020  ks':.           
-00026dc0: 2072 6573 756c 7420 3d20 7365 6c66 2e73   result = self.s
-00026dd0: 6361 6c65 5f6b 7562 655f 656b 7328 636c  cale_kube_eks(cl
-00026de0: 7573 7465 722c 206f 7665 7272 6964 6573  uster, overrides
-00026df0: 3d6f 7665 7272 6964 6573 290a 2020 2020  =overrides).    
-00026e00: 2020 2020 656c 6966 206b 7562 6574 7970      elif kubetyp
-00026e10: 6520 3d3d 2027 616b 7327 3a0a 2020 2020  e == 'aks':.    
-00026e20: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
-00026e30: 2073 656c 662e 7363 616c 655f 6b75 6265   self.scale_kube
-00026e40: 5f61 6b73 2863 6c75 7374 6572 2c20 6f76  _aks(cluster, ov
-00026e50: 6572 7269 6465 733d 6f76 6572 7269 6465  errides=override
-00026e60: 7329 0a20 2020 2020 2020 2072 6574 7572  s).        retur
-00026e70: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
-00026e80: 6620 7363 616c 655f 6b75 6265 5f61 6b73  f scale_kube_aks
-00026e90: 2873 656c 662c 2063 6c75 7374 6572 2c20  (self, cluster, 
-00026ea0: 6f76 6572 7269 6465 733d 7b7d 293a 0a20  overrides={}):. 
-00026eb0: 2020 2020 2020 2066 726f 6d20 6b76 6972         from kvir
-00026ec0: 742e 636c 7573 7465 7220 696d 706f 7274  t.cluster import
-00026ed0: 2061 6b73 0a20 2020 2020 2020 2072 6574   aks.        ret
-00026ee0: 7572 6e20 616b 732e 7363 616c 6528 7365  urn aks.scale(se
-00026ef0: 6c66 2c20 636c 7573 7465 722c 206f 7665  lf, cluster, ove
-00026f00: 7272 6964 6573 290a 0a20 2020 2064 6566  rrides)..    def
-00026f10: 2073 6361 6c65 5f6b 7562 655f 656b 7328   scale_kube_eks(
-00026f20: 7365 6c66 2c20 636c 7573 7465 722c 206f  self, cluster, o
-00026f30: 7665 7272 6964 6573 3d7b 7d29 3a0a 2020  verrides={}):.  
-00026f40: 2020 2020 2020 6672 6f6d 206b 7669 7274        from kvirt
-00026f50: 2e63 6c75 7374 6572 2069 6d70 6f72 7420  .cluster import 
-00026f60: 656b 730a 2020 2020 2020 2020 7265 7475  eks.        retu
-00026f70: 726e 2065 6b73 2e73 6361 6c65 2873 656c  rn eks.scale(sel
-00026f80: 662c 2063 6c75 7374 6572 2c20 6f76 6572  f, cluster, over
-00026f90: 7269 6465 7329 0a0a 2020 2020 6465 6620  rides)..    def 
-00026fa0: 7363 616c 655f 6b75 6265 5f67 656e 6572  scale_kube_gener
-00026fb0: 6963 2873 656c 662c 2063 6c75 7374 6572  ic(self, cluster
-00026fc0: 2c20 6f76 6572 7269 6465 733d 7b7d 293a  , overrides={}):
-00026fd0: 0a20 2020 2020 2020 2070 6c61 6e64 6972  .        plandir
-00026fe0: 203d 206f 732e 7061 7468 2e64 6972 6e61   = os.path.dirna
-00026ff0: 6d65 286b 7562 6561 646d 2e63 7265 6174  me(kubeadm.creat
-00027000: 652e 5f5f 636f 6465 5f5f 2e63 6f5f 6669  e.__code__.co_fi
-00027010: 6c65 6e61 6d65 290a 2020 2020 2020 2020  lename).        
-00027020: 7265 7475 726e 206b 7562 6561 646d 2e73  return kubeadm.s
-00027030: 6361 6c65 2873 656c 662c 2070 6c61 6e64  cale(self, pland
-00027040: 6972 2c20 636c 7573 7465 722c 206f 7665  ir, cluster, ove
-00027050: 7272 6964 6573 290a 0a20 2020 2064 6566  rrides)..    def
-00027060: 2073 6361 6c65 5f6b 7562 655f 676b 6528   scale_kube_gke(
-00027070: 7365 6c66 2c20 636c 7573 7465 722c 206f  self, cluster, o
-00027080: 7665 7272 6964 6573 3d7b 7d29 3a0a 2020  verrides={}):.  
-00027090: 2020 2020 2020 6672 6f6d 206b 7669 7274        from kvirt
-000270a0: 2e63 6c75 7374 6572 2069 6d70 6f72 7420  .cluster import 
-000270b0: 676b 650a 2020 2020 2020 2020 7265 7475  gke.        retu
-000270c0: 726e 2067 6b65 2e73 6361 6c65 2873 656c  rn gke.scale(sel
-000270d0: 662c 2063 6c75 7374 6572 2c20 6f76 6572  f, cluster, over
-000270e0: 7269 6465 7329 0a0a 2020 2020 6465 6620  rides)..    def 
-000270f0: 7363 616c 655f 6b75 6265 5f68 7970 6572  scale_kube_hyper
-00027100: 7368 6966 7428 7365 6c66 2c20 636c 7573  shift(self, clus
-00027110: 7465 722c 206f 7665 7272 6964 6573 3d7b  ter, overrides={
-00027120: 7d29 3a0a 2020 2020 2020 2020 706c 616e  }):.        plan
-00027130: 6469 7220 3d20 6f73 2e70 6174 682e 6469  dir = os.path.di
-00027140: 726e 616d 6528 6879 7065 7273 6869 6674  rname(hypershift
-00027150: 2e63 7265 6174 652e 5f5f 636f 6465 5f5f  .create.__code__
-00027160: 2e63 6f5f 6669 6c65 6e61 6d65 290a 2020  .co_filename).  
-00027170: 2020 2020 2020 7265 7475 726e 2068 7970        return hyp
-00027180: 6572 7368 6966 742e 7363 616c 6528 7365  ershift.scale(se
-00027190: 6c66 2c20 706c 616e 6469 722c 2063 6c75  lf, plandir, clu
-000271a0: 7374 6572 2c20 6f76 6572 7269 6465 7329  ster, overrides)
-000271b0: 0a0a 2020 2020 6465 6620 7363 616c 655f  ..    def scale_
-000271c0: 6b75 6265 5f6b 3373 2873 656c 662c 2063  kube_k3s(self, c
-000271d0: 6c75 7374 6572 2c20 6f76 6572 7269 6465  luster, override
-000271e0: 733d 7b7d 293a 0a20 2020 2020 2020 2070  s={}):.        p
-000271f0: 6c61 6e64 6972 203d 206f 732e 7061 7468  landir = os.path
-00027200: 2e64 6972 6e61 6d65 286b 3373 2e63 7265  .dirname(k3s.cre
-00027210: 6174 652e 5f5f 636f 6465 5f5f 2e63 6f5f  ate.__code__.co_
-00027220: 6669 6c65 6e61 6d65 290a 2020 2020 2020  filename).      
-00027230: 2020 7265 7475 726e 206b 3373 2e73 6361    return k3s.sca
-00027240: 6c65 2873 656c 662c 2070 6c61 6e64 6972  le(self, plandir
-00027250: 2c20 636c 7573 7465 722c 206f 7665 7272  , cluster, overr
-00027260: 6964 6573 290a 0a20 2020 2064 6566 2073  ides)..    def s
-00027270: 6361 6c65 5f6b 7562 655f 6f70 656e 7368  cale_kube_opensh
-00027280: 6966 7428 7365 6c66 2c20 636c 7573 7465  ift(self, cluste
-00027290: 722c 206f 7665 7272 6964 6573 3d7b 7d29  r, overrides={})
-000272a0: 3a0a 2020 2020 2020 2020 706c 616e 6469  :.        plandi
-000272b0: 7220 3d20 6f73 2e70 6174 682e 6469 726e  r = os.path.dirn
-000272c0: 616d 6528 6f70 656e 7368 6966 742e 6372  ame(openshift.cr
-000272d0: 6561 7465 2e5f 5f63 6f64 655f 5f2e 636f  eate.__code__.co
-000272e0: 5f66 696c 656e 616d 6529 0a20 2020 2020  _filename).     
-000272f0: 2020 2072 6574 7572 6e20 6f70 656e 7368     return opensh
-00027300: 6966 742e 7363 616c 6528 7365 6c66 2c20  ift.scale(self, 
-00027310: 706c 616e 6469 722c 2063 6c75 7374 6572  plandir, cluster
-00027320: 2c20 6f76 6572 7269 6465 7329 0a0a 2020  , overrides)..  
-00027330: 2020 6465 6620 7570 6461 7465 5f6b 7562    def update_kub
-00027340: 6528 7365 6c66 2c20 636c 7573 7465 722c  e(self, cluster,
-00027350: 205f 7479 7065 2c20 6f76 6572 7269 6465   _type, override
-00027360: 733d 7b7d 2c20 706c 616e 3d4e 6f6e 6529  s={}, plan=None)
-00027370: 3a0a 2020 2020 2020 2020 6f76 6572 7269  :.        overri
-00027380: 6465 735b 2773 6b69 705f 6669 6c65 735f  des['skip_files_
-00027390: 7265 6d65 6469 6174 696f 6e27 5d20 3d20  remediation'] = 
-000273a0: 5472 7565 0a20 2020 2020 2020 206f 7665  True.        ove
-000273b0: 7272 6964 6573 5b27 7363 616c 6527 5d20  rrides['scale'] 
-000273c0: 3d20 5472 7565 0a20 2020 2020 2020 2063  = True.        c
-000273d0: 6c75 7374 6572 6469 7220 3d20 6f73 2e70  lusterdir = os.p
-000273e0: 6174 682e 6578 7061 6e64 7573 6572 2866  ath.expanduser(f
-000273f0: 227e 2f2e 6b63 6c69 2f63 6c75 7374 6572  "~/.kcli/cluster
-00027400: 732f 7b63 6c75 7374 6572 7d22 290a 2020  s/{cluster}").  
-00027410: 2020 2020 2020 706c 616e 766d 7320 3d20        planvms = 
-00027420: 5b5d 0a20 2020 2020 2020 2069 6620 706c  [].        if pl
-00027430: 616e 2069 7320 4e6f 6e65 3a0a 2020 2020  an is None:.    
-00027440: 2020 2020 2020 2020 706c 616e 203d 2063          plan = c
-00027450: 6c75 7374 6572 0a20 2020 2020 2020 2069  luster.        i
-00027460: 6620 5f74 7970 6520 3d3d 2027 616b 7327  f _type == 'aks'
-00027470: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00027480: 6c66 2e73 6361 6c65 5f6b 7562 655f 616b  lf.scale_kube_ak
-00027490: 7328 636c 7573 7465 722c 206f 7665 7272  s(cluster, overr
-000274a0: 6964 6573 3d6f 7665 7272 6964 6573 290a  ides=overrides).
-000274b0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-000274c0: 726e 0a20 2020 2020 2020 2069 6620 5f74  rn.        if _t
-000274d0: 7970 6520 3d3d 2027 656b 7327 3a0a 2020  ype == 'eks':.  
-000274e0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-000274f0: 6361 6c65 5f6b 7562 655f 656b 7328 636c  cale_kube_eks(cl
-00027500: 7573 7465 722c 206f 7665 7272 6964 6573  uster, overrides
-00027510: 3d6f 7665 7272 6964 6573 290a 2020 2020  =overrides).    
-00027520: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
-00027530: 2020 2020 2020 2069 6620 5f74 7970 6520         if _type 
-00027540: 3d3d 2027 676b 6527 3a0a 2020 2020 2020  == 'gke':.      
-00027550: 2020 2020 2020 7365 6c66 2e73 6361 6c65        self.scale
-00027560: 5f6b 7562 655f 676b 6528 636c 7573 7465  _kube_gke(cluste
-00027570: 722c 206f 7665 7272 6964 6573 3d6f 7665  r, overrides=ove
-00027580: 7272 6964 6573 290a 2020 2020 2020 2020  rrides).        
-00027590: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
-000275a0: 2020 2069 6620 5f74 7970 6520 3d3d 2027     if _type == '
-000275b0: 6765 6e65 7269 6327 3a0a 2020 2020 2020  generic':.      
-000275c0: 2020 2020 2020 726f 6c65 7320 3d20 5b27        roles = ['
-000275d0: 6374 6c70 6c61 6e65 7327 2c20 2777 6f72  ctlplanes', 'wor
-000275e0: 6b65 7273 275d 0a20 2020 2020 2020 2020  kers'].         
-000275f0: 2020 2070 6c61 6e64 6972 203d 206f 732e     plandir = os.
-00027600: 7061 7468 2e64 6972 6e61 6d65 286b 7562  path.dirname(kub
-00027610: 6561 646d 2e63 7265 6174 652e 5f5f 636f  eadm.create.__co
-00027620: 6465 5f5f 2e63 6f5f 6669 6c65 6e61 6d65  de__.co_filename
-00027630: 290a 2020 2020 2020 2020 656c 6966 205f  ).        elif _
-00027640: 7479 7065 203d 3d20 276b 3373 273a 0a20  type == 'k3s':. 
-00027650: 2020 2020 2020 2020 2020 2070 6c61 6e64             pland
-00027660: 6972 203d 206f 732e 7061 7468 2e64 6972  ir = os.path.dir
-00027670: 6e61 6d65 286b 3373 2e63 7265 6174 652e  name(k3s.create.
-00027680: 5f5f 636f 6465 5f5f 2e63 6f5f 6669 6c65  __code__.co_file
-00027690: 6e61 6d65 290a 2020 2020 2020 2020 2020  name).          
-000276a0: 2020 726f 6c65 7320 3d20 5b27 626f 6f74    roles = ['boot
-000276b0: 7374 7261 7027 2c20 2777 6f72 6b65 7273  strap', 'workers
-000276c0: 275d 2069 6620 6f76 6572 7269 6465 732e  '] if overrides.
-000276d0: 6765 7428 2763 746c 706c 616e 6573 272c  get('ctlplanes',
-000276e0: 2031 2920 3d3d 2031 2065 6c73 6520 5b27   1) == 1 else ['
-000276f0: 626f 6f74 7374 7261 7027 2c20 2763 746c  bootstrap', 'ctl
-00027700: 706c 616e 6573 272c 0a20 2020 2020 2020  planes',.       
+00025960: 2070 6173 730a 2020 2020 2020 2020 2020   pass.          
+00025970: 2020 6966 2073 656c 662e 7479 7065 203d    if self.type =
+00025980: 3d20 2761 7a75 7265 273a 0a20 2020 2020  = 'azure':.     
+00025990: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
+000259a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000259b0: 2020 2020 7365 6c66 2e6b 2e64 656c 6574      self.k.delet
+000259c0: 655f 6964 656e 7469 7479 2866 276b 636c  e_identity(f'kcl
+000259d0: 692d 7b63 6c75 7374 6572 7d27 290a 2020  i-{cluster}').  
+000259e0: 2020 2020 2020 2020 2020 2020 2020 6578                ex
+000259f0: 6365 7074 3a0a 2020 2020 2020 2020 2020  cept:.          
+00025a00: 2020 2020 2020 2020 2020 7061 7373 0a20            pass. 
+00025a10: 2020 2020 2020 2065 6c69 6620 646e 7363         elif dnsc
+00025a20: 6c69 656e 7420 6973 206e 6f74 204e 6f6e  lient is not Non
+00025a30: 653a 0a20 2020 2020 2020 2020 2020 207a  e:.            z
+00025a40: 203d 204b 636f 6e66 6967 2863 6c69 656e   = Kconfig(clien
+00025a50: 743d 646e 7363 6c69 656e 7429 2e6b 0a20  t=dnsclient).k. 
+00025a60: 2020 2020 2020 2020 2020 207a 2e64 656c             z.del
+00025a70: 6574 655f 646e 7328 6622 6170 692e 7b63  ete_dns(f"api.{c
+00025a80: 6c75 7374 6572 7d22 2c20 646f 6d61 696e  luster}", domain
+00025a90: 290a 2020 2020 2020 2020 2020 2020 7a2e  ).            z.
+00025aa0: 6465 6c65 7465 5f64 6e73 2866 2261 7070  delete_dns(f"app
+00025ab0: 732e 7b63 6c75 7374 6572 7d22 2c20 646f  s.{cluster}", do
+00025ac0: 6d61 696e 290a 2020 2020 2020 2020 6966  main).        if
+00025ad0: 2068 7970 6572 7368 6966 743a 0a20 2020   hypershift:.   
+00025ae0: 2020 2020 2020 2020 206b 7562 6563 6f6e           kubecon
+00025af0: 6669 676d 676d 7420 3d20 6622 7b63 6c75  figmgmt = f"{clu
+00025b00: 7374 6572 6469 727d 2f6b 7562 6563 6f6e  sterdir}/kubecon
+00025b10: 6669 672e 6d67 6d74 220a 2020 2020 2020  fig.mgmt".      
+00025b20: 2020 2020 2020 6966 206f 732e 7061 7468        if os.path
+00025b30: 2e65 7869 7374 7328 6627 7b63 6c75 7374  .exists(f'{clust
+00025b40: 6572 6469 727d 2f62 6d63 732e 796d 6c27  erdir}/bmcs.yml'
+00025b50: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00025b60: 2020 2063 616c 6c28 6627 4b55 4245 434f     call(f'KUBECO
+00025b70: 4e46 4947 3d7b 6b75 6265 636f 6e66 6967  NFIG={kubeconfig
+00025b80: 6d67 6d74 7d20 6f63 2064 656c 6574 6520  mgmt} oc delete 
+00025b90: 2d66 207b 636c 7573 7465 7264 6972 7d2f  -f {clusterdir}/
+00025ba0: 626d 6373 2e79 6d6c 272c 2073 6865 6c6c  bmcs.yml', shell
+00025bb0: 3d54 7275 6529 0a20 2020 2020 2020 2020  =True).         
+00025bc0: 2020 2063 616c 6c28 6627 4b55 4245 434f     call(f'KUBECO
+00025bd0: 4e46 4947 3d7b 6b75 6265 636f 6e66 6967  NFIG={kubeconfig
+00025be0: 6d67 6d74 7d20 6f63 2064 656c 6574 6520  mgmt} oc delete 
+00025bf0: 2d66 207b 636c 7573 7465 7264 6972 7d2f  -f {clusterdir}/
+00025c00: 6175 746f 6170 7072 6f76 6572 6372 6f6e  autoapprovercron
+00025c10: 2e79 6d6c 272c 2073 6865 6c6c 3d54 7275  .yml', shell=Tru
+00025c20: 6529 0a20 2020 2020 2020 2020 2020 2063  e).            c
+00025c30: 616c 6c28 6627 4b55 4245 434f 4e46 4947  all(f'KUBECONFIG
+00025c40: 3d7b 6b75 6265 636f 6e66 6967 6d67 6d74  ={kubeconfigmgmt
+00025c50: 7d20 6f63 2064 656c 6574 6520 2d66 207b  } oc delete -f {
+00025c60: 636c 7573 7465 7264 6972 7d2f 6e6f 6465  clusterdir}/node
+00025c70: 706f 6f6c 2e79 616d 6c27 2c20 7368 656c  pool.yaml', shel
+00025c80: 6c3d 5472 7565 290a 2020 2020 2020 2020  l=True).        
+00025c90: 2020 2020 6361 6c6c 2866 274b 5542 4543      call(f'KUBEC
+00025ca0: 4f4e 4649 473d 7b6b 7562 6563 6f6e 6669  ONFIG={kubeconfi
+00025cb0: 676d 676d 747d 206f 6320 6465 6c65 7465  gmgmt} oc delete
+00025cc0: 202d 6620 7b63 6c75 7374 6572 6469 727d   -f {clusterdir}
+00025cd0: 2f68 6f73 7465 6463 6c75 7374 6572 2e79  /hostedcluster.y
+00025ce0: 616d 6c27 2c20 7368 656c 6c3d 5472 7565  aml', shell=True
+00025cf0: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+00025d00: 206f 732e 7061 7468 2e65 7869 7374 7328   os.path.exists(
+00025d10: 6627 7b63 6c75 7374 6572 6469 727d 2f61  f'{clusterdir}/a
+00025d20: 7373 6973 7465 645f 696e 6672 612e 796d  ssisted_infra.ym
+00025d30: 6c27 293a 0a20 2020 2020 2020 2020 2020  l'):.           
+00025d40: 2020 2020 2063 616c 6c28 6627 4b55 4245       call(f'KUBE
+00025d50: 434f 4e46 4947 3d7b 6b75 6265 636f 6e66  CONFIG={kubeconf
+00025d60: 6967 6d67 6d74 7d20 6f63 2064 656c 6574  igmgmt} oc delet
+00025d70: 6520 2d66 207b 636c 7573 7465 7264 6972  e -f {clusterdir
+00025d80: 7d2f 6173 7369 7374 6564 5f69 6e66 7261  }/assisted_infra
+00025d90: 2e79 6d6c 272c 2073 6865 6c6c 3d54 7275  .yml', shell=Tru
+00025da0: 6529 0a20 2020 2020 2020 2020 2020 2069  e).            i
+00025db0: 6620 6e6f 7420 6173 7369 7374 6564 2061  f not assisted a
+00025dc0: 6e64 2028 2762 6172 656d 6574 616c 5f69  nd ('baremetal_i
+00025dd0: 736f 2720 696e 2063 6c75 7374 6572 6461  so' in clusterda
+00025de0: 7461 206f 7220 2762 6172 656d 6574 616c  ta or 'baremetal
+00025df0: 5f68 6f73 7473 2720 696e 2063 6c75 7374  _hosts' in clust
+00025e00: 6572 6461 7461 293a 0a20 2020 2020 2020  erdata):.       
+00025e10: 2020 2020 2020 2020 2063 616c 6c28 6627           call(f'
+00025e20: 4b55 4245 434f 4e46 4947 3d7b 6b75 6265  KUBECONFIG={kube
+00025e30: 636f 6e66 6967 6d67 6d74 7d20 6f63 202d  configmgmt} oc -
+00025e40: 6e20 6465 6661 756c 7420 6465 6c65 7465  n default delete
+00025e50: 2061 6c6c 202d 6c20 6170 703d 6874 7470   all -l app=http
+00025e60: 642d 6b63 6c69 272c 2073 6865 6c6c 3d54  d-kcli', shell=T
+00025e70: 7275 6529 0a20 2020 2020 2020 2020 2020  rue).           
+00025e80: 2020 2020 2063 616c 6c28 6627 4b55 4245       call(f'KUBE
+00025e90: 434f 4e46 4947 3d7b 6b75 6265 636f 6e66  CONFIG={kubeconf
+00025ea0: 6967 6d67 6d74 7d20 6f63 202d 6e20 6465  igmgmt} oc -n de
+00025eb0: 6661 756c 7420 6465 6c65 7465 2070 7663  fault delete pvc
+00025ec0: 2068 7474 7064 2d6b 636c 692d 7076 6327   httpd-kcli-pvc'
+00025ed0: 2c20 7368 656c 6c3d 5472 7565 290a 2020  , shell=True).  
+00025ee0: 2020 2020 2020 2020 2020 696e 6772 6573            ingres
+00025ef0: 735f 6970 203d 2063 6c75 7374 6572 6461  s_ip = clusterda
+00025f00: 7461 2e67 6574 2827 696e 6772 6573 735f  ta.get('ingress_
+00025f10: 6970 2729 0a20 2020 2020 2020 2020 2020  ip').           
+00025f20: 2069 6620 7365 6c66 2e74 7970 6520 3d3d   if self.type ==
+00025f30: 2027 6b75 6265 7669 7274 2720 616e 6420   'kubevirt' and 
+00025f40: 636c 7573 7465 7264 6174 612e 6765 7428  clusterdata.get(
+00025f50: 2770 6c61 7466 6f72 6d27 2920 6973 204e  'platform') is N
+00025f60: 6f6e 6520 616e 6420 696e 6772 6573 735f  one and ingress_
+00025f70: 6970 2069 7320 4e6f 6e65 3a0a 2020 2020  ip is None:.    
+00025f80: 2020 2020 2020 2020 2020 2020 6361 6c6c              call
+00025f90: 2866 274b 5542 4543 4f4e 4649 473d 7b6b  (f'KUBECONFIG={k
+00025fa0: 7562 6563 6f6e 6669 676d 676d 747d 206f  ubeconfigmgmt} o
+00025fb0: 6320 2d6e 207b 6b2e 6e61 6d65 7370 6163  c -n {k.namespac
+00025fc0: 657d 2064 656c 6574 6520 726f 7574 6520  e} delete route 
+00025fd0: 7b63 6c75 7374 6572 7d2d 696e 6772 6573  {cluster}-ingres
+00025fe0: 7327 2c20 7368 656c 6c3d 5472 7565 290a  s', shell=True).
+00025ff0: 2020 2020 2020 2020 6966 2067 6b65 3a0a          if gke:.
+00026000: 2020 2020 2020 2020 2020 2020 6763 7063              gcpc
+00026010: 6c69 656e 7420 3d20 4e6f 6e65 0a20 2020  lient = None.   
+00026020: 2020 2020 2020 2020 2069 6620 2763 6c69           if 'cli
+00026030: 656e 7427 2069 6e20 636c 7573 7465 7264  ent' in clusterd
+00026040: 6174 613a 0a20 2020 2020 2020 2020 2020  ata:.           
+00026050: 2020 2020 2067 6370 636c 6965 6e74 203d       gcpclient =
+00026060: 2063 6c75 7374 6572 6461 7461 5b27 636c   clusterdata['cl
+00026070: 6965 6e74 275d 0a20 2020 2020 2020 2020  ient'].         
+00026080: 2020 2065 6c69 6620 7365 6c66 2e74 7970     elif self.typ
+00026090: 6520 3d3d 2027 6763 7027 3a0a 2020 2020  e == 'gcp':.    
+000260a0: 2020 2020 2020 2020 2020 2020 6763 7063              gcpc
+000260b0: 6c69 656e 7420 3d20 7365 6c66 2e63 6c69  lient = self.cli
+000260c0: 656e 740a 2020 2020 2020 2020 2020 2020  ent.            
+000260d0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+000260e0: 2020 2020 2020 6d73 6720 3d20 2244 656c        msg = "Del
+000260f0: 6574 696e 6720 676b 6520 636c 7573 7465  eting gke cluste
+00026100: 7220 7265 7175 6972 6573 2074 6f20 696e  r requires to in
+00026110: 7374 616e 7469 6174 6520 6763 7020 7072  stantiate gcp pr
+00026120: 6f76 6964 6572 220a 2020 2020 2020 2020  ovider".        
+00026130: 2020 2020 2020 2020 6572 726f 7228 6d73          error(ms
+00026140: 6729 0a20 2020 2020 2020 2020 2020 2020  g).             
+00026150: 2020 2072 6574 7572 6e20 7b27 7265 7375     return {'resu
+00026160: 6c74 273a 2027 6661 696c 7572 6527 2c20  lt': 'failure', 
+00026170: 2772 6561 736f 6e27 3a20 6d73 677d 0a20  'reason': msg}. 
+00026180: 2020 2020 2020 2020 2020 2066 726f 6d20             from 
+00026190: 6b76 6972 742e 636c 7573 7465 7220 696d  kvirt.cluster im
+000261a0: 706f 7274 2067 6b65 0a20 2020 2020 2020  port gke.       
+000261b0: 2020 2020 2063 7572 7265 6e74 636f 6e66       currentconf
+000261c0: 6967 203d 204b 636f 6e66 6967 2863 6c69  ig = Kconfig(cli
+000261d0: 656e 743d 6763 7063 6c69 656e 7429 2e6b  ent=gcpclient).k
+000261e0: 2069 6620 6763 7063 6c69 656e 7420 213d   if gcpclient !=
+000261f0: 2073 656c 662e 636c 6965 6e74 2065 6c73   self.client els
+00026200: 6520 7365 6c66 0a20 2020 2020 2020 2020  e self.         
+00026210: 2020 207a 6f6e 616c 203d 2063 6c75 7374     zonal = clust
+00026220: 6572 6461 7461 2e67 6574 2827 7a6f 6e61  erdata.get('zona
+00026230: 6c27 2c20 5472 7565 290a 2020 2020 2020  l', True).      
+00026240: 2020 2020 2020 676b 652e 6465 6c65 7465        gke.delete
+00026250: 2863 7572 7265 6e74 636f 6e66 6967 2c20  (currentconfig, 
+00026260: 636c 7573 7465 722c 207a 6f6e 616c 290a  cluster, zonal).
+00026270: 2020 2020 2020 2020 656c 6966 2065 6b73          elif eks
+00026280: 3a0a 2020 2020 2020 2020 2020 2020 656b  :.            ek
+00026290: 7363 6c69 656e 7420 3d20 4e6f 6e65 0a20  sclient = None. 
+000262a0: 2020 2020 2020 2020 2020 2069 6620 2763             if 'c
+000262b0: 6c69 656e 7427 2069 6e20 636c 7573 7465  lient' in cluste
+000262c0: 7264 6174 613a 0a20 2020 2020 2020 2020  rdata:.         
+000262d0: 2020 2020 2020 2065 6b73 636c 6965 6e74         eksclient
+000262e0: 203d 2063 6c75 7374 6572 6461 7461 5b27   = clusterdata['
+000262f0: 636c 6965 6e74 275d 0a20 2020 2020 2020  client'].       
+00026300: 2020 2020 2065 6c69 6620 7365 6c66 2e74       elif self.t
+00026310: 7970 6520 3d3d 2027 6177 7327 3a0a 2020  ype == 'aws':.  
+00026320: 2020 2020 2020 2020 2020 2020 2020 656b                ek
+00026330: 7363 6c69 656e 7420 3d20 7365 6c66 2e63  sclient = self.c
+00026340: 6c69 656e 740a 2020 2020 2020 2020 2020  lient.          
+00026350: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00026360: 2020 2020 2020 2020 6d73 6720 3d20 2244          msg = "D
+00026370: 656c 6574 696e 6720 656b 7320 636c 7573  eleting eks clus
+00026380: 7465 7220 7265 7175 6972 6573 2074 6f20  ter requires to 
+00026390: 696e 7374 616e 7469 6174 6520 6177 7320  instantiate aws 
+000263a0: 7072 6f76 6964 6572 220a 2020 2020 2020  provider".      
+000263b0: 2020 2020 2020 2020 2020 6572 726f 7228            error(
+000263c0: 6d73 6729 0a20 2020 2020 2020 2020 2020  msg).           
+000263d0: 2020 2020 2072 6574 7572 6e20 7b27 7265       return {'re
+000263e0: 7375 6c74 273a 2027 6661 696c 7572 6527  sult': 'failure'
+000263f0: 2c20 2772 6561 736f 6e27 3a20 6d73 677d  , 'reason': msg}
+00026400: 0a20 2020 2020 2020 2020 2020 2066 726f  .            fro
+00026410: 6d20 6b76 6972 742e 636c 7573 7465 7220  m kvirt.cluster 
+00026420: 696d 706f 7274 2065 6b73 0a20 2020 2020  import eks.     
+00026430: 2020 2020 2020 2063 7572 7265 6e74 636f         currentco
+00026440: 6e66 6967 203d 204b 636f 6e66 6967 2863  nfig = Kconfig(c
+00026450: 6c69 656e 743d 656b 7363 6c69 656e 7429  lient=eksclient)
+00026460: 2e6b 2069 6620 656b 7363 6c69 656e 7420  .k if eksclient 
+00026470: 213d 2073 656c 662e 636c 6965 6e74 2065  != self.client e
+00026480: 6c73 6520 7365 6c66 0a20 2020 2020 2020  lse self.       
+00026490: 2020 2020 2065 6b73 2e64 656c 6574 6528       eks.delete(
+000264a0: 6375 7272 656e 7463 6f6e 6669 672c 2063  currentconfig, c
+000264b0: 6c75 7374 6572 290a 2020 2020 2020 2020  luster).        
+000264c0: 656c 6966 2061 6b73 3a0a 2020 2020 2020  elif aks:.      
+000264d0: 2020 2020 2020 616b 7363 6c69 656e 7420        aksclient 
+000264e0: 3d20 4e6f 6e65 0a20 2020 2020 2020 2020  = None.         
+000264f0: 2020 2069 6620 2763 6c69 656e 7427 2069     if 'client' i
+00026500: 6e20 636c 7573 7465 7264 6174 613a 0a20  n clusterdata:. 
+00026510: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00026520: 6b73 636c 6965 6e74 203d 2063 6c75 7374  ksclient = clust
+00026530: 6572 6461 7461 5b27 636c 6965 6e74 275d  erdata['client']
+00026540: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
+00026550: 6620 7365 6c66 2e74 7970 6520 3d3d 2027  f self.type == '
+00026560: 617a 7572 6527 3a0a 2020 2020 2020 2020  azure':.        
+00026570: 2020 2020 2020 2020 616b 7363 6c69 656e          aksclien
+00026580: 7420 3d20 7365 6c66 2e63 6c69 656e 740a  t = self.client.
+00026590: 2020 2020 2020 2020 2020 2020 656c 7365              else
+000265a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000265b0: 2020 6d73 6720 3d20 2244 656c 6574 696e    msg = "Deletin
+000265c0: 6720 616b 7320 636c 7573 7465 7220 7265  g aks cluster re
+000265d0: 7175 6972 6573 2074 6f20 696e 7374 616e  quires to instan
+000265e0: 7469 6174 6520 617a 7572 6520 7072 6f76  tiate azure prov
+000265f0: 6964 6572 220a 2020 2020 2020 2020 2020  ider".          
+00026600: 2020 2020 2020 6572 726f 7228 6d73 6729        error(msg)
+00026610: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00026620: 2072 6574 7572 6e20 7b27 7265 7375 6c74   return {'result
+00026630: 273a 2027 6661 696c 7572 6527 2c20 2772  ': 'failure', 'r
+00026640: 6561 736f 6e27 3a20 6d73 677d 0a20 2020  eason': msg}.   
+00026650: 2020 2020 2020 2020 2066 726f 6d20 6b76           from kv
+00026660: 6972 742e 636c 7573 7465 7220 696d 706f  irt.cluster impo
+00026670: 7274 2061 6b73 0a20 2020 2020 2020 2020  rt aks.         
+00026680: 2020 2063 7572 7265 6e74 636f 6e66 6967     currentconfig
+00026690: 203d 204b 636f 6e66 6967 2863 6c69 656e   = Kconfig(clien
+000266a0: 743d 616b 7363 6c69 656e 7429 2e6b 2069  t=aksclient).k i
+000266b0: 6620 616b 7363 6c69 656e 7420 213d 2073  f aksclient != s
+000266c0: 656c 662e 636c 6965 6e74 2065 6c73 6520  elf.client else 
+000266d0: 7365 6c66 0a20 2020 2020 2020 2020 2020  self.           
+000266e0: 2061 6b73 2e64 656c 6574 6528 6375 7272   aks.delete(curr
+000266f0: 656e 7463 6f6e 6669 672c 2063 6c75 7374  entconfig, clust
+00026700: 6572 290a 2020 2020 2020 2020 666f 7220  er).        for 
+00026710: 636f 6e66 706f 6f6c 2069 6e20 7365 6c66  confpool in self
+00026720: 2e63 6f6e 6670 6f6f 6c73 3a0a 2020 2020  .confpools:.    
+00026730: 2020 2020 2020 2020 6970 5f72 6573 6572          ip_reser
+00026740: 7661 7469 6f6e 7320 3d20 7365 6c66 2e63  vations = self.c
+00026750: 6f6e 6670 6f6f 6c73 5b63 6f6e 6670 6f6f  onfpools[confpoo
+00026760: 6c5d 2e67 6574 2827 6970 5f72 6573 6572  l].get('ip_reser
+00026770: 7661 7469 6f6e 7327 2c20 7b7d 290a 2020  vations', {}).  
+00026780: 2020 2020 2020 2020 2020 6966 2063 6c75            if clu
+00026790: 7374 6572 2069 6e20 6970 5f72 6573 6572  ster in ip_reser
+000267a0: 7661 7469 6f6e 733a 0a20 2020 2020 2020  vations:.       
+000267b0: 2020 2020 2020 2020 2064 656c 2069 705f           del ip_
+000267c0: 7265 7365 7276 6174 696f 6e73 5b63 6c75  reservations[clu
+000267d0: 7374 6572 5d0a 2020 2020 2020 2020 2020  ster].          
+000267e0: 2020 2020 2020 7365 6c66 2e75 7064 6174        self.updat
+000267f0: 655f 636f 6e66 706f 6f6c 2863 6f6e 6670  e_confpool(confp
+00026800: 6f6f 6c2c 207b 2769 705f 7265 7365 7276  ool, {'ip_reserv
+00026810: 6174 696f 6e73 273a 2069 705f 7265 7365  ations': ip_rese
+00026820: 7276 6174 696f 6e73 7d29 0a20 2020 2020  rvations}).     
+00026830: 2020 2020 2020 206e 616d 655f 7265 7365         name_rese
+00026840: 7276 6174 696f 6e73 203d 2073 656c 662e  rvations = self.
+00026850: 636f 6e66 706f 6f6c 735b 636f 6e66 706f  confpools[confpo
+00026860: 6f6c 5d2e 6765 7428 276e 616d 655f 7265  ol].get('name_re
+00026870: 7365 7276 6174 696f 6e73 272c 205b 5d29  servations', [])
+00026880: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00026890: 636c 7573 7465 7220 696e 206e 616d 655f  cluster in name_
+000268a0: 7265 7365 7276 6174 696f 6e73 3a0a 2020  reservations:.  
+000268b0: 2020 2020 2020 2020 2020 2020 2020 6e61                na
+000268c0: 6d65 5f72 6573 6572 7661 7469 6f6e 732e  me_reservations.
+000268d0: 7265 6d6f 7665 2863 6c75 7374 6572 290a  remove(cluster).
+000268e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000268f0: 7365 6c66 2e75 7064 6174 655f 636f 6e66  self.update_conf
+00026900: 706f 6f6c 2863 6f6e 6670 6f6f 6c2c 207b  pool(confpool, {
+00026910: 276e 616d 655f 7265 7365 7276 6174 696f  'name_reservatio
+00026920: 6e73 273a 206e 616d 655f 7265 7365 7276  ns': name_reserv
+00026930: 6174 696f 6e73 7d29 0a20 2020 2020 2020  ations}).       
+00026940: 2020 2020 2063 6c75 7374 6572 5f62 6172       cluster_bar
+00026950: 656d 6574 616c 5f72 6573 6572 7661 7469  emetal_reservati
+00026960: 6f6e 7320 3d20 7365 6c66 2e63 6f6e 6670  ons = self.confp
+00026970: 6f6f 6c73 5b63 6f6e 6670 6f6f 6c5d 2e67  ools[confpool].g
+00026980: 6574 2827 636c 7573 7465 725f 6261 7265  et('cluster_bare
+00026990: 6d65 7461 6c5f 7265 7365 7276 6174 696f  metal_reservatio
+000269a0: 6e73 272c 207b 7d29 0a20 2020 2020 2020  ns', {}).       
+000269b0: 2020 2020 2069 6620 636c 7573 7465 7220       if cluster 
+000269c0: 696e 2063 6c75 7374 6572 5f62 6172 656d  in cluster_barem
+000269d0: 6574 616c 5f72 6573 6572 7661 7469 6f6e  etal_reservation
+000269e0: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+000269f0: 2020 2064 656c 2063 6c75 7374 6572 5f62     del cluster_b
+00026a00: 6172 656d 6574 616c 5f72 6573 6572 7661  aremetal_reserva
+00026a10: 7469 6f6e 735b 636c 7573 7465 725d 0a20  tions[cluster]. 
+00026a20: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00026a30: 656c 662e 7570 6461 7465 5f63 6f6e 6670  elf.update_confp
+00026a40: 6f6f 6c28 636f 6e66 706f 6f6c 2c20 7b27  ool(confpool, {'
+00026a50: 636c 7573 7465 725f 6261 7265 6d65 7461  cluster_baremeta
+00026a60: 6c5f 7265 7365 7276 6174 696f 6e73 273a  l_reservations':
+00026a70: 2063 6c75 7374 6572 5f62 6172 656d 6574   cluster_baremet
+00026a80: 616c 5f72 6573 6572 7661 7469 6f6e 737d  al_reservations}
+00026a90: 290a 2020 2020 2020 2020 6966 206f 732e  ).        if os.
+00026aa0: 7061 7468 2e65 7869 7374 7328 636c 7573  path.exists(clus
+00026ab0: 7465 7264 6972 293a 0a20 2020 2020 2020  terdir):.       
+00026ac0: 2020 2020 2070 7072 696e 7428 6622 4465       pprint(f"De
+00026ad0: 6c65 7469 6e67 2064 6972 6563 746f 7279  leting directory
+00026ae0: 207b 636c 7573 7465 7264 6972 7d22 290a   {clusterdir}").
+00026af0: 2020 2020 2020 2020 2020 2020 726d 7472              rmtr
+00026b00: 6565 2863 6c75 7374 6572 6469 7229 0a20  ee(clusterdir). 
+00026b10: 2020 2020 2020 2072 6574 7572 6e20 7b27         return {'
+00026b20: 7265 7375 6c74 273a 2027 7375 6363 6573  result': 'succes
+00026b30: 7327 7d0a 0a20 2020 2064 6566 2073 6361  s'}..    def sca
+00026b40: 6c65 5f6b 7562 6528 7365 6c66 2c20 636c  le_kube(self, cl
+00026b50: 7573 7465 722c 206b 7562 6574 7970 652c  uster, kubetype,
+00026b60: 206f 7665 7272 6964 6573 3d7b 7d29 3a0a   overrides={}):.
+00026b70: 2020 2020 2020 2020 6966 206b 7562 6574          if kubet
+00026b80: 7970 6520 3d3d 2027 6765 6e65 7269 6327  ype == 'generic'
+00026b90: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00026ba0: 7375 6c74 203d 2073 656c 662e 7363 616c  sult = self.scal
+00026bb0: 655f 6b75 6265 5f67 656e 6572 6963 2863  e_kube_generic(c
+00026bc0: 6c75 7374 6572 2c20 6f76 6572 7269 6465  luster, override
+00026bd0: 733d 6f76 6572 7269 6465 7329 0a20 2020  s=overrides).   
+00026be0: 2020 2020 2065 6c69 6620 6b75 6265 7479       elif kubety
+00026bf0: 7065 203d 3d20 276b 3373 273a 0a20 2020  pe == 'k3s':.   
+00026c00: 2020 2020 2020 2020 2072 6573 756c 7420           result 
+00026c10: 3d20 7365 6c66 2e73 6361 6c65 5f6b 7562  = self.scale_kub
+00026c20: 655f 6b33 7328 636c 7573 7465 722c 206f  e_k3s(cluster, o
+00026c30: 7665 7272 6964 6573 3d6f 7665 7272 6964  verrides=overrid
+00026c40: 6573 290a 2020 2020 2020 2020 656c 6966  es).        elif
+00026c50: 206b 7562 6574 7970 6520 3d3d 2027 6f70   kubetype == 'op
+00026c60: 656e 7368 6966 7427 3a0a 2020 2020 2020  enshift':.      
+00026c70: 2020 2020 2020 7265 7375 6c74 203d 2073        result = s
+00026c80: 656c 662e 7363 616c 655f 6b75 6265 5f6f  elf.scale_kube_o
+00026c90: 7065 6e73 6869 6674 2863 6c75 7374 6572  penshift(cluster
+00026ca0: 2c20 6f76 6572 7269 6465 733d 6f76 6572  , overrides=over
+00026cb0: 7269 6465 7329 0a20 2020 2020 2020 2065  rides).        e
+00026cc0: 6c69 6620 6b75 6265 7479 7065 203d 3d20  lif kubetype == 
+00026cd0: 2768 7970 6572 7368 6966 7427 3a0a 2020  'hypershift':.  
+00026ce0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00026cf0: 203d 2073 656c 662e 7363 616c 655f 6b75   = self.scale_ku
+00026d00: 6265 5f68 7970 6572 7368 6966 7428 636c  be_hypershift(cl
+00026d10: 7573 7465 722c 206f 7665 7272 6964 6573  uster, overrides
+00026d20: 3d6f 7665 7272 6964 6573 290a 2020 2020  =overrides).    
+00026d30: 2020 2020 656c 6966 206b 7562 6574 7970      elif kubetyp
+00026d40: 6520 3d3d 2027 676b 6527 3a0a 2020 2020  e == 'gke':.    
+00026d50: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
+00026d60: 2073 656c 662e 7363 616c 655f 6b75 6265   self.scale_kube
+00026d70: 5f67 6b65 2863 6c75 7374 6572 2c20 6f76  _gke(cluster, ov
+00026d80: 6572 7269 6465 733d 6f76 6572 7269 6465  errides=override
+00026d90: 7329 0a20 2020 2020 2020 2065 6c69 6620  s).        elif 
+00026da0: 6b75 6265 7479 7065 203d 3d20 2765 6b73  kubetype == 'eks
+00026db0: 273a 0a20 2020 2020 2020 2020 2020 2072  ':.            r
+00026dc0: 6573 756c 7420 3d20 7365 6c66 2e73 6361  esult = self.sca
+00026dd0: 6c65 5f6b 7562 655f 656b 7328 636c 7573  le_kube_eks(clus
+00026de0: 7465 722c 206f 7665 7272 6964 6573 3d6f  ter, overrides=o
+00026df0: 7665 7272 6964 6573 290a 2020 2020 2020  verrides).      
+00026e00: 2020 656c 6966 206b 7562 6574 7970 6520    elif kubetype 
+00026e10: 3d3d 2027 616b 7327 3a0a 2020 2020 2020  == 'aks':.      
+00026e20: 2020 2020 2020 7265 7375 6c74 203d 2073        result = s
+00026e30: 656c 662e 7363 616c 655f 6b75 6265 5f61  elf.scale_kube_a
+00026e40: 6b73 2863 6c75 7374 6572 2c20 6f76 6572  ks(cluster, over
+00026e50: 7269 6465 733d 6f76 6572 7269 6465 7329  rides=overrides)
+00026e60: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00026e70: 7265 7375 6c74 0a0a 2020 2020 6465 6620  result..    def 
+00026e80: 7363 616c 655f 6b75 6265 5f61 6b73 2873  scale_kube_aks(s
+00026e90: 656c 662c 2063 6c75 7374 6572 2c20 6f76  elf, cluster, ov
+00026ea0: 6572 7269 6465 733d 7b7d 293a 0a20 2020  errides={}):.   
+00026eb0: 2020 2020 2066 726f 6d20 6b76 6972 742e       from kvirt.
+00026ec0: 636c 7573 7465 7220 696d 706f 7274 2061  cluster import a
+00026ed0: 6b73 0a20 2020 2020 2020 2072 6574 7572  ks.        retur
+00026ee0: 6e20 616b 732e 7363 616c 6528 7365 6c66  n aks.scale(self
+00026ef0: 2c20 636c 7573 7465 722c 206f 7665 7272  , cluster, overr
+00026f00: 6964 6573 290a 0a20 2020 2064 6566 2073  ides)..    def s
+00026f10: 6361 6c65 5f6b 7562 655f 656b 7328 7365  cale_kube_eks(se
+00026f20: 6c66 2c20 636c 7573 7465 722c 206f 7665  lf, cluster, ove
+00026f30: 7272 6964 6573 3d7b 7d29 3a0a 2020 2020  rrides={}):.    
+00026f40: 2020 2020 6672 6f6d 206b 7669 7274 2e63      from kvirt.c
+00026f50: 6c75 7374 6572 2069 6d70 6f72 7420 656b  luster import ek
+00026f60: 730a 2020 2020 2020 2020 7265 7475 726e  s.        return
+00026f70: 2065 6b73 2e73 6361 6c65 2873 656c 662c   eks.scale(self,
+00026f80: 2063 6c75 7374 6572 2c20 6f76 6572 7269   cluster, overri
+00026f90: 6465 7329 0a0a 2020 2020 6465 6620 7363  des)..    def sc
+00026fa0: 616c 655f 6b75 6265 5f67 656e 6572 6963  ale_kube_generic
+00026fb0: 2873 656c 662c 2063 6c75 7374 6572 2c20  (self, cluster, 
+00026fc0: 6f76 6572 7269 6465 733d 7b7d 293a 0a20  overrides={}):. 
+00026fd0: 2020 2020 2020 2070 6c61 6e64 6972 203d         plandir =
+00026fe0: 206f 732e 7061 7468 2e64 6972 6e61 6d65   os.path.dirname
+00026ff0: 286b 7562 6561 646d 2e63 7265 6174 652e  (kubeadm.create.
+00027000: 5f5f 636f 6465 5f5f 2e63 6f5f 6669 6c65  __code__.co_file
+00027010: 6e61 6d65 290a 2020 2020 2020 2020 7265  name).        re
+00027020: 7475 726e 206b 7562 6561 646d 2e73 6361  turn kubeadm.sca
+00027030: 6c65 2873 656c 662c 2070 6c61 6e64 6972  le(self, plandir
+00027040: 2c20 636c 7573 7465 722c 206f 7665 7272  , cluster, overr
+00027050: 6964 6573 290a 0a20 2020 2064 6566 2073  ides)..    def s
+00027060: 6361 6c65 5f6b 7562 655f 676b 6528 7365  cale_kube_gke(se
+00027070: 6c66 2c20 636c 7573 7465 722c 206f 7665  lf, cluster, ove
+00027080: 7272 6964 6573 3d7b 7d29 3a0a 2020 2020  rrides={}):.    
+00027090: 2020 2020 6672 6f6d 206b 7669 7274 2e63      from kvirt.c
+000270a0: 6c75 7374 6572 2069 6d70 6f72 7420 676b  luster import gk
+000270b0: 650a 2020 2020 2020 2020 7265 7475 726e  e.        return
+000270c0: 2067 6b65 2e73 6361 6c65 2873 656c 662c   gke.scale(self,
+000270d0: 2063 6c75 7374 6572 2c20 6f76 6572 7269   cluster, overri
+000270e0: 6465 7329 0a0a 2020 2020 6465 6620 7363  des)..    def sc
+000270f0: 616c 655f 6b75 6265 5f68 7970 6572 7368  ale_kube_hypersh
+00027100: 6966 7428 7365 6c66 2c20 636c 7573 7465  ift(self, cluste
+00027110: 722c 206f 7665 7272 6964 6573 3d7b 7d29  r, overrides={})
+00027120: 3a0a 2020 2020 2020 2020 706c 616e 6469  :.        plandi
+00027130: 7220 3d20 6f73 2e70 6174 682e 6469 726e  r = os.path.dirn
+00027140: 616d 6528 6879 7065 7273 6869 6674 2e63  ame(hypershift.c
+00027150: 7265 6174 652e 5f5f 636f 6465 5f5f 2e63  reate.__code__.c
+00027160: 6f5f 6669 6c65 6e61 6d65 290a 2020 2020  o_filename).    
+00027170: 2020 2020 7265 7475 726e 2068 7970 6572      return hyper
+00027180: 7368 6966 742e 7363 616c 6528 7365 6c66  shift.scale(self
+00027190: 2c20 706c 616e 6469 722c 2063 6c75 7374  , plandir, clust
+000271a0: 6572 2c20 6f76 6572 7269 6465 7329 0a0a  er, overrides)..
+000271b0: 2020 2020 6465 6620 7363 616c 655f 6b75      def scale_ku
+000271c0: 6265 5f6b 3373 2873 656c 662c 2063 6c75  be_k3s(self, clu
+000271d0: 7374 6572 2c20 6f76 6572 7269 6465 733d  ster, overrides=
+000271e0: 7b7d 293a 0a20 2020 2020 2020 2070 6c61  {}):.        pla
+000271f0: 6e64 6972 203d 206f 732e 7061 7468 2e64  ndir = os.path.d
+00027200: 6972 6e61 6d65 286b 3373 2e63 7265 6174  irname(k3s.creat
+00027210: 652e 5f5f 636f 6465 5f5f 2e63 6f5f 6669  e.__code__.co_fi
+00027220: 6c65 6e61 6d65 290a 2020 2020 2020 2020  lename).        
+00027230: 7265 7475 726e 206b 3373 2e73 6361 6c65  return k3s.scale
+00027240: 2873 656c 662c 2070 6c61 6e64 6972 2c20  (self, plandir, 
+00027250: 636c 7573 7465 722c 206f 7665 7272 6964  cluster, overrid
+00027260: 6573 290a 0a20 2020 2064 6566 2073 6361  es)..    def sca
+00027270: 6c65 5f6b 7562 655f 6f70 656e 7368 6966  le_kube_openshif
+00027280: 7428 7365 6c66 2c20 636c 7573 7465 722c  t(self, cluster,
+00027290: 206f 7665 7272 6964 6573 3d7b 7d29 3a0a   overrides={}):.
+000272a0: 2020 2020 2020 2020 706c 616e 6469 7220          plandir 
+000272b0: 3d20 6f73 2e70 6174 682e 6469 726e 616d  = os.path.dirnam
+000272c0: 6528 6f70 656e 7368 6966 742e 6372 6561  e(openshift.crea
+000272d0: 7465 2e5f 5f63 6f64 655f 5f2e 636f 5f66  te.__code__.co_f
+000272e0: 696c 656e 616d 6529 0a20 2020 2020 2020  ilename).       
+000272f0: 2072 6574 7572 6e20 6f70 656e 7368 6966   return openshif
+00027300: 742e 7363 616c 6528 7365 6c66 2c20 706c  t.scale(self, pl
+00027310: 616e 6469 722c 2063 6c75 7374 6572 2c20  andir, cluster, 
+00027320: 6f76 6572 7269 6465 7329 0a0a 2020 2020  overrides)..    
+00027330: 6465 6620 7570 6461 7465 5f6b 7562 6528  def update_kube(
+00027340: 7365 6c66 2c20 636c 7573 7465 722c 205f  self, cluster, _
+00027350: 7479 7065 2c20 6f76 6572 7269 6465 733d  type, overrides=
+00027360: 7b7d 2c20 706c 616e 3d4e 6f6e 6529 3a0a  {}, plan=None):.
+00027370: 2020 2020 2020 2020 6f76 6572 7269 6465          override
+00027380: 735b 2773 6b69 705f 6669 6c65 735f 7265  s['skip_files_re
+00027390: 6d65 6469 6174 696f 6e27 5d20 3d20 5472  mediation'] = Tr
+000273a0: 7565 0a20 2020 2020 2020 206f 7665 7272  ue.        overr
+000273b0: 6964 6573 5b27 7363 616c 6527 5d20 3d20  ides['scale'] = 
+000273c0: 5472 7565 0a20 2020 2020 2020 2063 6c75  True.        clu
+000273d0: 7374 6572 6469 7220 3d20 6f73 2e70 6174  sterdir = os.pat
+000273e0: 682e 6578 7061 6e64 7573 6572 2866 227e  h.expanduser(f"~
+000273f0: 2f2e 6b63 6c69 2f63 6c75 7374 6572 732f  /.kcli/clusters/
+00027400: 7b63 6c75 7374 6572 7d22 290a 2020 2020  {cluster}").    
+00027410: 2020 2020 706c 616e 766d 7320 3d20 5b5d      planvms = []
+00027420: 0a20 2020 2020 2020 2069 6620 706c 616e  .        if plan
+00027430: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+00027440: 2020 2020 2020 706c 616e 203d 2063 6c75        plan = clu
+00027450: 7374 6572 0a20 2020 2020 2020 2069 6620  ster.        if 
+00027460: 5f74 7970 6520 3d3d 2027 616b 7327 3a0a  _type == 'aks':.
+00027470: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00027480: 2e73 6361 6c65 5f6b 7562 655f 616b 7328  .scale_kube_aks(
+00027490: 636c 7573 7465 722c 206f 7665 7272 6964  cluster, overrid
+000274a0: 6573 3d6f 7665 7272 6964 6573 290a 2020  es=overrides).  
+000274b0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+000274c0: 0a20 2020 2020 2020 2069 6620 5f74 7970  .        if _typ
+000274d0: 6520 3d3d 2027 656b 7327 3a0a 2020 2020  e == 'eks':.    
+000274e0: 2020 2020 2020 2020 7365 6c66 2e73 6361          self.sca
+000274f0: 6c65 5f6b 7562 655f 656b 7328 636c 7573  le_kube_eks(clus
+00027500: 7465 722c 206f 7665 7272 6964 6573 3d6f  ter, overrides=o
+00027510: 7665 7272 6964 6573 290a 2020 2020 2020  verrides).      
+00027520: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
+00027530: 2020 2020 2069 6620 5f74 7970 6520 3d3d       if _type ==
+00027540: 2027 676b 6527 3a0a 2020 2020 2020 2020   'gke':.        
+00027550: 2020 2020 7365 6c66 2e73 6361 6c65 5f6b      self.scale_k
+00027560: 7562 655f 676b 6528 636c 7573 7465 722c  ube_gke(cluster,
+00027570: 206f 7665 7272 6964 6573 3d6f 7665 7272   overrides=overr
+00027580: 6964 6573 290a 2020 2020 2020 2020 2020  ides).          
+00027590: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
+000275a0: 2069 6620 5f74 7970 6520 3d3d 2027 6765   if _type == 'ge
+000275b0: 6e65 7269 6327 3a0a 2020 2020 2020 2020  neric':.        
+000275c0: 2020 2020 726f 6c65 7320 3d20 5b27 6374      roles = ['ct
+000275d0: 6c70 6c61 6e65 7327 2c20 2777 6f72 6b65  lplanes', 'worke
+000275e0: 7273 275d 0a20 2020 2020 2020 2020 2020  rs'].           
+000275f0: 2070 6c61 6e64 6972 203d 206f 732e 7061   plandir = os.pa
+00027600: 7468 2e64 6972 6e61 6d65 286b 7562 6561  th.dirname(kubea
+00027610: 646d 2e63 7265 6174 652e 5f5f 636f 6465  dm.create.__code
+00027620: 5f5f 2e63 6f5f 6669 6c65 6e61 6d65 290a  __.co_filename).
+00027630: 2020 2020 2020 2020 656c 6966 205f 7479          elif _ty
+00027640: 7065 203d 3d20 276b 3373 273a 0a20 2020  pe == 'k3s':.   
+00027650: 2020 2020 2020 2020 2070 6c61 6e64 6972           plandir
+00027660: 203d 206f 732e 7061 7468 2e64 6972 6e61   = os.path.dirna
+00027670: 6d65 286b 3373 2e63 7265 6174 652e 5f5f  me(k3s.create.__
+00027680: 636f 6465 5f5f 2e63 6f5f 6669 6c65 6e61  code__.co_filena
+00027690: 6d65 290a 2020 2020 2020 2020 2020 2020  me).            
+000276a0: 726f 6c65 7320 3d20 5b27 626f 6f74 7374  roles = ['bootst
+000276b0: 7261 7027 2c20 2777 6f72 6b65 7273 275d  rap', 'workers']
+000276c0: 2069 6620 6f76 6572 7269 6465 732e 6765   if overrides.ge
+000276d0: 7428 2763 746c 706c 616e 6573 272c 2031  t('ctlplanes', 1
+000276e0: 2920 3d3d 2031 2065 6c73 6520 5b27 626f  ) == 1 else ['bo
+000276f0: 6f74 7374 7261 7027 2c20 2763 746c 706c  otstrap', 'ctlpl
+00027700: 616e 6573 272c 0a20 2020 2020 2020 2020  anes',.         
 00027710: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00027720: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00027730: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00027740: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00027750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027760: 2020 2777 6f72 6b65 7273 275d 0a20 2020    'workers'].   
-00027770: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00027780: 2020 2020 2020 2070 6c61 6e64 6972 203d         plandir =
-00027790: 206f 732e 7061 7468 2e64 6972 6e61 6d65   os.path.dirname
-000277a0: 286f 7065 6e73 6869 6674 2e63 7265 6174  (openshift.creat
-000277b0: 652e 5f5f 636f 6465 5f5f 2e63 6f5f 6669  e.__code__.co_fi
-000277c0: 6c65 6e61 6d65 290a 2020 2020 2020 2020  lename).        
-000277d0: 2020 2020 726f 6c65 7320 3d20 5b27 6374      roles = ['ct
-000277e0: 6c70 6c61 6e65 7327 2c20 2777 6f72 6b65  lplanes', 'worke
-000277f0: 7273 275d 0a20 2020 2020 2020 2020 2020  rs'].           
-00027800: 2069 6620 7365 6c66 2e74 7970 6520 696e   if self.type in
-00027810: 205b 2761 7773 272c 2027 617a 7572 6527   ['aws', 'azure'
-00027820: 2c20 2767 6370 275d 3a0a 2020 2020 2020  , 'gcp']:.      
-00027830: 2020 2020 2020 2020 2020 726f 6c65 7320            roles 
-00027840: 3d20 5b66 2763 6c6f 7564 5f7b 726f 6c65  = [f'cloud_{role
-00027850: 7d27 2066 6f72 2072 6f6c 6520 696e 2072  }' for role in r
-00027860: 6f6c 6573 5d0a 2020 2020 2020 2020 6966  oles].        if
-00027870: 206f 7665 7272 6964 6573 2e67 6574 2827   overrides.get('
-00027880: 776f 726b 6572 7327 2c20 3029 203d 3d20  workers', 0) == 
-00027890: 303a 0a20 2020 2020 2020 2020 2020 2064  0:.            d
-000278a0: 656c 2072 6f6c 6573 5b2d 315d 0a20 2020  el roles[-1].   
-000278b0: 2020 2020 2069 6620 6f73 2e70 6174 682e       if os.path.
-000278c0: 6578 6973 7473 2866 227b 636c 7573 7465  exists(f"{cluste
-000278d0: 7264 6972 7d2f 6b63 6c69 5f70 6172 616d  rdir}/kcli_param
-000278e0: 6574 6572 732e 796d 6c22 293a 0a20 2020  eters.yml"):.   
-000278f0: 2020 2020 2020 2020 2064 6174 6120 3d20           data = 
-00027900: 7b27 636c 7573 7465 7227 3a20 636c 7573  {'cluster': clus
-00027910: 7465 722c 2027 6b75 6265 273a 2063 6c75  ter, 'kube': clu
-00027920: 7374 6572 2c20 276b 7562 6574 7970 6527  ster, 'kubetype'
-00027930: 3a20 5f74 7970 657d 0a20 2020 2020 2020  : _type}.       
-00027940: 2020 2020 2077 6974 6820 6f70 656e 2866       with open(f
-00027950: 227b 636c 7573 7465 7264 6972 7d2f 6b63  "{clusterdir}/kc
-00027960: 6c69 5f70 6172 616d 6574 6572 732e 796d  li_parameters.ym
-00027970: 6c22 2c20 2772 2729 2061 7320 696e 7374  l", 'r') as inst
-00027980: 616c 6c3a 0a20 2020 2020 2020 2020 2020  all:.           
-00027990: 2020 2020 2069 6e73 7461 6c6c 7061 7261       installpara
-000279a0: 6d20 3d20 7961 6d6c 2e73 6166 655f 6c6f  m = yaml.safe_lo
-000279b0: 6164 2869 6e73 7461 6c6c 290a 2020 2020  ad(install).    
-000279c0: 2020 2020 2020 2020 2020 2020 6461 7461              data
-000279d0: 2e75 7064 6174 6528 696e 7374 616c 6c70  .update(installp
-000279e0: 6172 616d 290a 2020 2020 2020 2020 2020  aram).          
-000279f0: 2020 2020 2020 706c 616e 203d 2069 6e73        plan = ins
-00027a00: 7461 6c6c 7061 7261 6d2e 6765 7428 2770  tallparam.get('p
-00027a10: 6c61 6e27 2c20 706c 616e 290a 2020 2020  lan', plan).    
-00027a20: 2020 2020 2020 2020 6461 7461 2e75 7064          data.upd
-00027a30: 6174 6528 6f76 6572 7269 6465 7329 0a20  ate(overrides). 
-00027a40: 2020 2020 2020 2020 2020 2077 6974 6820             with 
-00027a50: 6f70 656e 2866 227b 636c 7573 7465 7264  open(f"{clusterd
-00027a60: 6972 7d2f 6b63 6c69 5f70 6172 616d 6574  ir}/kcli_paramet
-00027a70: 6572 732e 796d 6c22 2c20 2777 2729 2061  ers.yml", 'w') a
-00027a80: 7320 7061 7261 6d66 696c 653a 0a20 2020  s paramfile:.   
-00027a90: 2020 2020 2020 2020 2020 2020 2079 616d               yam
-00027aa0: 6c2e 7361 6665 5f64 756d 7028 6461 7461  l.safe_dump(data
-00027ab0: 2c20 7061 7261 6d66 696c 6529 0a20 2020  , paramfile).   
-00027ac0: 2020 2020 206f 732e 6368 6469 7228 6f73       os.chdir(os
-00027ad0: 2e70 6174 682e 6578 7061 6e64 7573 6572  .path.expanduser
-00027ae0: 2822 7e2f 2e6b 636c 6922 2929 0a20 2020  ("~/.kcli")).   
-00027af0: 2020 2020 2066 6f72 2072 6f6c 6520 696e       for role in
-00027b00: 2072 6f6c 6573 3a0a 2020 2020 2020 2020   roles:.        
-00027b10: 2020 2020 7070 7269 6e74 2866 2255 7064      pprint(f"Upd
-00027b20: 6174 696e 6720 766d 7320 7769 7468 207b  ating vms with {
-00027b30: 726f 6c65 7d20 726f 6c65 2229 0a20 2020  role} role").   
-00027b40: 2020 2020 2020 2020 2070 6c61 6e64 6174           plandat
-00027b50: 6120 3d20 7365 6c66 2e70 6c61 6e28 706c  a = self.plan(pl
-00027b60: 616e 2c20 696e 7075 7466 696c 653d 6627  an, inputfile=f'
-00027b70: 7b70 6c61 6e64 6972 7d2f 7b72 6f6c 657d  {plandir}/{role}
-00027b80: 2e79 6d6c 272c 206f 7665 7272 6964 6573  .yml', overrides
-00027b90: 3d6f 7665 7272 6964 6573 2c20 7570 6461  =overrides, upda
-00027ba0: 7465 3d54 7275 6529 0a20 2020 2020 2020  te=True).       
-00027bb0: 2020 2020 2070 6c61 6e76 6d73 2e65 7874       planvms.ext
-00027bc0: 656e 6428 706c 616e 6461 7461 5b27 6e65  end(plandata['ne
-00027bd0: 7776 6d73 275d 202b 2070 6c61 6e64 6174  wvms'] + plandat
-00027be0: 615b 2765 7869 7374 696e 6776 6d73 275d  a['existingvms']
-00027bf0: 290a 2020 2020 2020 2020 6578 6973 7469  ).        existi
-00027c00: 6e67 5f63 746c 706c 616e 6573 203d 206c  ng_ctlplanes = l
-00027c10: 656e 285b 7620 666f 7220 7620 696e 2070  en([v for v in p
-00027c20: 6c61 6e76 6d73 2069 6620 762e 7374 6172  lanvms if v.star
-00027c30: 7473 7769 7468 2866 277b 636c 7573 7465  tswith(f'{cluste
-00027c40: 727d 2d63 746c 706c 616e 652d 2729 5d29  r}-ctlplane-')])
-00027c50: 0a20 2020 2020 2020 2065 7869 7374 696e  .        existin
-00027c60: 675f 776f 726b 6572 7320 3d20 6c65 6e28  g_workers = len(
-00027c70: 5b76 2066 6f72 2076 2069 6e20 706c 616e  [v for v in plan
-00027c80: 766d 7320 6966 2076 2e73 7461 7274 7377  vms if v.startsw
-00027c90: 6974 6828 6627 7b63 6c75 7374 6572 7d2d  ith(f'{cluster}-
-00027ca0: 776f 726b 6572 2d27 295d 290a 2020 2020  worker-')]).    
-00027cb0: 2020 2020 6966 2064 6174 615b 2763 746c      if data['ctl
-00027cc0: 706c 616e 6573 275d 2021 3d20 6578 6973  planes'] != exis
-00027cd0: 7469 6e67 5f63 746c 706c 616e 6573 206f  ting_ctlplanes o
-00027ce0: 7220 6461 7461 5b27 776f 726b 6572 7327  r data['workers'
-00027cf0: 5d20 213d 2065 7869 7374 696e 675f 776f  ] != existing_wo
-00027d00: 726b 6572 733a 0a20 2020 2020 2020 2020  rkers:.         
-00027d10: 2020 206f 732e 656e 7669 726f 6e5b 274b     os.environ['K
-00027d20: 5542 4543 4f4e 4649 4727 5d20 3d20 6622  UBECONFIG'] = f"
-00027d30: 7b63 6c75 7374 6572 6469 727d 2f61 7574  {clusterdir}/aut
-00027d40: 682f 6b75 6265 636f 6e66 6967 220a 2020  h/kubeconfig".  
-00027d50: 2020 2020 2020 2020 2020 6269 6e61 7279            binary
-00027d60: 203d 2027 6f63 2720 6966 2077 6869 6368   = 'oc' if which
-00027d70: 2827 6f63 2729 2069 7320 6e6f 7420 4e6f  ('oc') is not No
-00027d80: 6e65 2065 6c73 6520 276b 7562 6563 746c  ne else 'kubectl
-00027d90: 270a 2020 2020 2020 2020 2020 2020 6e6f  '.            no
-00027da0: 6465 7363 6d64 203d 2066 277b 6269 6e61  descmd = f'{bina
-00027db0: 7279 7d20 6765 7420 6e6f 6465 202d 6f20  ry} get node -o 
-00027dc0: 6e61 6d65 270a 2020 2020 2020 2020 2020  name'.          
-00027dd0: 2020 6e6f 6465 7320 3d20 5b6e 2e73 7472    nodes = [n.str
-00027de0: 6970 2829 2e72 6570 6c61 6365 2827 6e6f  ip().replace('no
-00027df0: 6465 2f27 2c20 2727 2920 666f 7220 6e20  de/', '') for n 
-00027e00: 696e 206f 732e 706f 7065 6e28 6e6f 6465  in os.popen(node
-00027e10: 7363 6d64 292e 7265 6164 6c69 6e65 7328  scmd).readlines(
-00027e20: 295d 0a20 2020 2020 2020 2020 2020 2066  )].            f
-00027e30: 6f72 2076 6d20 696e 2073 656c 662e 6b2e  or vm in self.k.
-00027e40: 6c69 7374 2829 3a0a 2020 2020 2020 2020  list():.        
-00027e50: 2020 2020 2020 2020 766d 6e61 6d65 203d          vmname =
-00027e60: 2076 6d5b 276e 616d 6527 5d0a 2020 2020   vm['name'].    
-00027e70: 2020 2020 2020 2020 2020 2020 766d 706c              vmpl
-00027e80: 616e 203d 2076 6d2e 6765 7428 2770 6c61  an = vm.get('pla
-00027e90: 6e27 2c20 276b 7669 7274 2729 0a20 2020  n', 'kvirt').   
-00027ea0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00027eb0: 766d 706c 616e 203d 3d20 706c 616e 2061  vmplan == plan a
-00027ec0: 6e64 2076 6d6e 616d 6520 6e6f 7420 696e  nd vmname not in
-00027ed0: 2070 6c61 6e76 6d73 3a0a 2020 2020 2020   planvms:.      
-00027ee0: 2020 2020 2020 2020 2020 2020 2020 7070                pp
-00027ef0: 7269 6e74 2866 2244 656c 6574 696e 6720  rint(f"Deleting 
-00027f00: 766d 207b 766d 6e61 6d65 7d22 290a 2020  vm {vmname}").  
+00027760: 2777 6f72 6b65 7273 275d 0a20 2020 2020  'workers'].     
+00027770: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00027780: 2020 2020 2070 6c61 6e64 6972 203d 206f       plandir = o
+00027790: 732e 7061 7468 2e64 6972 6e61 6d65 286f  s.path.dirname(o
+000277a0: 7065 6e73 6869 6674 2e63 7265 6174 652e  penshift.create.
+000277b0: 5f5f 636f 6465 5f5f 2e63 6f5f 6669 6c65  __code__.co_file
+000277c0: 6e61 6d65 290a 2020 2020 2020 2020 2020  name).          
+000277d0: 2020 726f 6c65 7320 3d20 5b27 6374 6c70    roles = ['ctlp
+000277e0: 6c61 6e65 7327 2c20 2777 6f72 6b65 7273  lanes', 'workers
+000277f0: 275d 0a20 2020 2020 2020 2020 2020 2069  '].            i
+00027800: 6620 7365 6c66 2e74 7970 6520 696e 205b  f self.type in [
+00027810: 2761 7773 272c 2027 617a 7572 6527 2c20  'aws', 'azure', 
+00027820: 2767 6370 275d 3a0a 2020 2020 2020 2020  'gcp']:.        
+00027830: 2020 2020 2020 2020 726f 6c65 7320 3d20          roles = 
+00027840: 5b66 2763 6c6f 7564 5f7b 726f 6c65 7d27  [f'cloud_{role}'
+00027850: 2066 6f72 2072 6f6c 6520 696e 2072 6f6c   for role in rol
+00027860: 6573 5d0a 2020 2020 2020 2020 6966 206f  es].        if o
+00027870: 7665 7272 6964 6573 2e67 6574 2827 776f  verrides.get('wo
+00027880: 726b 6572 7327 2c20 3029 203d 3d20 303a  rkers', 0) == 0:
+00027890: 0a20 2020 2020 2020 2020 2020 2064 656c  .            del
+000278a0: 2072 6f6c 6573 5b2d 315d 0a20 2020 2020   roles[-1].     
+000278b0: 2020 2069 6620 6f73 2e70 6174 682e 6578     if os.path.ex
+000278c0: 6973 7473 2866 227b 636c 7573 7465 7264  ists(f"{clusterd
+000278d0: 6972 7d2f 6b63 6c69 5f70 6172 616d 6574  ir}/kcli_paramet
+000278e0: 6572 732e 796d 6c22 293a 0a20 2020 2020  ers.yml"):.     
+000278f0: 2020 2020 2020 2064 6174 6120 3d20 7b27         data = {'
+00027900: 636c 7573 7465 7227 3a20 636c 7573 7465  cluster': cluste
+00027910: 722c 2027 6b75 6265 273a 2063 6c75 7374  r, 'kube': clust
+00027920: 6572 2c20 276b 7562 6574 7970 6527 3a20  er, 'kubetype': 
+00027930: 5f74 7970 657d 0a20 2020 2020 2020 2020  _type}.         
+00027940: 2020 2077 6974 6820 6f70 656e 2866 227b     with open(f"{
+00027950: 636c 7573 7465 7264 6972 7d2f 6b63 6c69  clusterdir}/kcli
+00027960: 5f70 6172 616d 6574 6572 732e 796d 6c22  _parameters.yml"
+00027970: 2c20 2772 2729 2061 7320 696e 7374 616c  , 'r') as instal
+00027980: 6c3a 0a20 2020 2020 2020 2020 2020 2020  l:.             
+00027990: 2020 2069 6e73 7461 6c6c 7061 7261 6d20     installparam 
+000279a0: 3d20 7961 6d6c 2e73 6166 655f 6c6f 6164  = yaml.safe_load
+000279b0: 2869 6e73 7461 6c6c 290a 2020 2020 2020  (install).      
+000279c0: 2020 2020 2020 2020 2020 6461 7461 2e75            data.u
+000279d0: 7064 6174 6528 696e 7374 616c 6c70 6172  pdate(installpar
+000279e0: 616d 290a 2020 2020 2020 2020 2020 2020  am).            
+000279f0: 2020 2020 706c 616e 203d 2069 6e73 7461      plan = insta
+00027a00: 6c6c 7061 7261 6d2e 6765 7428 2770 6c61  llparam.get('pla
+00027a10: 6e27 2c20 706c 616e 290a 2020 2020 2020  n', plan).      
+00027a20: 2020 2020 2020 6461 7461 2e75 7064 6174        data.updat
+00027a30: 6528 6f76 6572 7269 6465 7329 0a20 2020  e(overrides).   
+00027a40: 2020 2020 2020 2020 2077 6974 6820 6f70           with op
+00027a50: 656e 2866 227b 636c 7573 7465 7264 6972  en(f"{clusterdir
+00027a60: 7d2f 6b63 6c69 5f70 6172 616d 6574 6572  }/kcli_parameter
+00027a70: 732e 796d 6c22 2c20 2777 2729 2061 7320  s.yml", 'w') as 
+00027a80: 7061 7261 6d66 696c 653a 0a20 2020 2020  paramfile:.     
+00027a90: 2020 2020 2020 2020 2020 2079 616d 6c2e             yaml.
+00027aa0: 7361 6665 5f64 756d 7028 6461 7461 2c20  safe_dump(data, 
+00027ab0: 7061 7261 6d66 696c 6529 0a20 2020 2020  paramfile).     
+00027ac0: 2020 206f 732e 6368 6469 7228 6f73 2e70     os.chdir(os.p
+00027ad0: 6174 682e 6578 7061 6e64 7573 6572 2822  ath.expanduser("
+00027ae0: 7e2f 2e6b 636c 6922 2929 0a20 2020 2020  ~/.kcli")).     
+00027af0: 2020 2066 6f72 2072 6f6c 6520 696e 2072     for role in r
+00027b00: 6f6c 6573 3a0a 2020 2020 2020 2020 2020  oles:.          
+00027b10: 2020 7070 7269 6e74 2866 2255 7064 6174    pprint(f"Updat
+00027b20: 696e 6720 766d 7320 7769 7468 207b 726f  ing vms with {ro
+00027b30: 6c65 7d20 726f 6c65 2229 0a20 2020 2020  le} role").     
+00027b40: 2020 2020 2020 2070 6c61 6e64 6174 6120         plandata 
+00027b50: 3d20 7365 6c66 2e70 6c61 6e28 706c 616e  = self.plan(plan
+00027b60: 2c20 696e 7075 7466 696c 653d 6627 7b70  , inputfile=f'{p
+00027b70: 6c61 6e64 6972 7d2f 7b72 6f6c 657d 2e79  landir}/{role}.y
+00027b80: 6d6c 272c 206f 7665 7272 6964 6573 3d6f  ml', overrides=o
+00027b90: 7665 7272 6964 6573 2c20 7570 6461 7465  verrides, update
+00027ba0: 3d54 7275 6529 0a20 2020 2020 2020 2020  =True).         
+00027bb0: 2020 2070 6c61 6e76 6d73 2e65 7874 656e     planvms.exten
+00027bc0: 6428 706c 616e 6461 7461 5b27 6e65 7776  d(plandata['newv
+00027bd0: 6d73 275d 202b 2070 6c61 6e64 6174 615b  ms'] + plandata[
+00027be0: 2765 7869 7374 696e 6776 6d73 275d 290a  'existingvms']).
+00027bf0: 2020 2020 2020 2020 6578 6973 7469 6e67          existing
+00027c00: 5f63 746c 706c 616e 6573 203d 206c 656e  _ctlplanes = len
+00027c10: 285b 7620 666f 7220 7620 696e 2070 6c61  ([v for v in pla
+00027c20: 6e76 6d73 2069 6620 762e 7374 6172 7473  nvms if v.starts
+00027c30: 7769 7468 2866 277b 636c 7573 7465 727d  with(f'{cluster}
+00027c40: 2d63 746c 706c 616e 652d 2729 5d29 0a20  -ctlplane-')]). 
+00027c50: 2020 2020 2020 2065 7869 7374 696e 675f         existing_
+00027c60: 776f 726b 6572 7320 3d20 6c65 6e28 5b76  workers = len([v
+00027c70: 2066 6f72 2076 2069 6e20 706c 616e 766d   for v in planvm
+00027c80: 7320 6966 2076 2e73 7461 7274 7377 6974  s if v.startswit
+00027c90: 6828 6627 7b63 6c75 7374 6572 7d2d 776f  h(f'{cluster}-wo
+00027ca0: 726b 6572 2d27 295d 290a 2020 2020 2020  rker-')]).      
+00027cb0: 2020 6966 2064 6174 615b 2763 746c 706c    if data['ctlpl
+00027cc0: 616e 6573 275d 2021 3d20 6578 6973 7469  anes'] != existi
+00027cd0: 6e67 5f63 746c 706c 616e 6573 206f 7220  ng_ctlplanes or 
+00027ce0: 6461 7461 5b27 776f 726b 6572 7327 5d20  data['workers'] 
+00027cf0: 213d 2065 7869 7374 696e 675f 776f 726b  != existing_work
+00027d00: 6572 733a 0a20 2020 2020 2020 2020 2020  ers:.           
+00027d10: 206f 732e 656e 7669 726f 6e5b 274b 5542   os.environ['KUB
+00027d20: 4543 4f4e 4649 4727 5d20 3d20 6622 7b63  ECONFIG'] = f"{c
+00027d30: 6c75 7374 6572 6469 727d 2f61 7574 682f  lusterdir}/auth/
+00027d40: 6b75 6265 636f 6e66 6967 220a 2020 2020  kubeconfig".    
+00027d50: 2020 2020 2020 2020 6269 6e61 7279 203d          binary =
+00027d60: 2027 6f63 2720 6966 2077 6869 6368 2827   'oc' if which('
+00027d70: 6f63 2729 2069 7320 6e6f 7420 4e6f 6e65  oc') is not None
+00027d80: 2065 6c73 6520 276b 7562 6563 746c 270a   else 'kubectl'.
+00027d90: 2020 2020 2020 2020 2020 2020 6e6f 6465              node
+00027da0: 7363 6d64 203d 2066 277b 6269 6e61 7279  scmd = f'{binary
+00027db0: 7d20 6765 7420 6e6f 6465 202d 6f20 6e61  } get node -o na
+00027dc0: 6d65 270a 2020 2020 2020 2020 2020 2020  me'.            
+00027dd0: 6e6f 6465 7320 3d20 5b6e 2e73 7472 6970  nodes = [n.strip
+00027de0: 2829 2e72 6570 6c61 6365 2827 6e6f 6465  ().replace('node
+00027df0: 2f27 2c20 2727 2920 666f 7220 6e20 696e  /', '') for n in
+00027e00: 206f 732e 706f 7065 6e28 6e6f 6465 7363   os.popen(nodesc
+00027e10: 6d64 292e 7265 6164 6c69 6e65 7328 295d  md).readlines()]
+00027e20: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+00027e30: 2076 6d20 696e 2073 656c 662e 6b2e 6c69   vm in self.k.li
+00027e40: 7374 2829 3a0a 2020 2020 2020 2020 2020  st():.          
+00027e50: 2020 2020 2020 766d 6e61 6d65 203d 2076        vmname = v
+00027e60: 6d5b 276e 616d 6527 5d0a 2020 2020 2020  m['name'].      
+00027e70: 2020 2020 2020 2020 2020 766d 706c 616e            vmplan
+00027e80: 203d 2076 6d2e 6765 7428 2770 6c61 6e27   = vm.get('plan'
+00027e90: 2c20 276b 7669 7274 2729 0a20 2020 2020  , 'kvirt').     
+00027ea0: 2020 2020 2020 2020 2020 2069 6620 766d             if vm
+00027eb0: 706c 616e 203d 3d20 706c 616e 2061 6e64  plan == plan and
+00027ec0: 2076 6d6e 616d 6520 6e6f 7420 696e 2070   vmname not in p
+00027ed0: 6c61 6e76 6d73 3a0a 2020 2020 2020 2020  lanvms:.        
+00027ee0: 2020 2020 2020 2020 2020 2020 7070 7269              ppri
+00027ef0: 6e74 2866 2244 656c 6574 696e 6720 766d  nt(f"Deleting vm
+00027f00: 207b 766d 6e61 6d65 7d22 290a 2020 2020   {vmname}").    
 00027f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027f20: 2020 666f 7220 6e6f 6465 2069 6e20 6e6f    for node in no
-00027f30: 6465 733a 0a20 2020 2020 2020 2020 2020  des:.           
-00027f40: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00027f50: 6e6f 6465 2e73 706c 6974 2827 2e27 295b  node.split('.')[
-00027f60: 305d 203d 3d20 766d 6e61 6d65 3a0a 2020  0] == vmname:.  
+00027f20: 666f 7220 6e6f 6465 2069 6e20 6e6f 6465  for node in node
+00027f30: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+00027f40: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
+00027f50: 6465 2e73 706c 6974 2827 2e27 295b 305d  de.split('.')[0]
+00027f60: 203d 3d20 766d 6e61 6d65 3a0a 2020 2020   == vmname:.    
 00027f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027f80: 2020 2020 2020 2020 2020 7070 7269 6e74            pprint
-00027f90: 2866 2244 656c 6574 696e 6720 6e6f 6465  (f"Deleting node
-00027fa0: 207b 6e6f 6465 7d20 6672 6f6d 2079 6f75   {node} from you
-00027fb0: 7220 636c 7573 7465 7222 290a 2020 2020  r cluster").    
+00027f80: 2020 2020 2020 2020 7070 7269 6e74 2866          pprint(f
+00027f90: 2244 656c 6574 696e 6720 6e6f 6465 207b  "Deleting node {
+00027fa0: 6e6f 6465 7d20 6672 6f6d 2079 6f75 7220  node} from your 
+00027fb0: 636c 7573 7465 7222 290a 2020 2020 2020  cluster").      
 00027fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027fd0: 2020 2020 2020 2020 6361 6c6c 2866 277b          call(f'{
-00027fe0: 6269 6e61 7279 7d20 6465 6c65 7465 206e  binary} delete n
-00027ff0: 6f64 6520 7b6e 6f64 657d 272c 2073 6865  ode {node}', she
-00028000: 6c6c 3d54 7275 6529 0a20 2020 2020 2020  ll=True).       
+00027fd0: 2020 2020 2020 6361 6c6c 2866 277b 6269        call(f'{bi
+00027fe0: 6e61 7279 7d20 6465 6c65 7465 206e 6f64  nary} delete nod
+00027ff0: 6520 7b6e 6f64 657d 272c 2073 6865 6c6c  e {node}', shell
+00028000: 3d54 7275 6529 0a20 2020 2020 2020 2020  =True).         
 00028010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028020: 2020 2020 2062 7265 616b 0a20 2020 2020       break.     
-00028030: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00028040: 656c 662e 6b2e 6465 6c65 7465 2876 6d6e  elf.k.delete(vmn
-00028050: 616d 6529 0a0a 2020 2020 6465 6620 6578  ame)..    def ex
-00028060: 706f 7365 5f70 6c61 6e28 7365 6c66 2c20  pose_plan(self, 
-00028070: 706c 616e 2c20 696e 7075 7466 696c 653d  plan, inputfile=
-00028080: 4e6f 6e65 2c20 6f76 6572 7269 6465 733d  None, overrides=
-00028090: 7b7d 2c20 706f 7274 3d39 3030 302c 2070  {}, port=9000, p
-000280a0: 666d 6f64 653d 4661 6c73 652c 2063 6c75  fmode=False, clu
-000280b0: 7374 6572 3d46 616c 7365 2c20 6578 7472  ster=False, extr
-000280c0: 6173 3d46 616c 7365 293a 0a20 2020 2020  as=False):.     
-000280d0: 2020 2069 6e70 7574 6669 6c65 203d 206f     inputfile = o
-000280e0: 732e 7061 7468 2e65 7870 616e 6475 7365  s.path.expanduse
-000280f0: 7228 696e 7075 7466 696c 6529 0a20 2020  r(inputfile).   
-00028100: 2020 2020 2069 6620 6e6f 7420 6f73 2e70       if not os.p
-00028110: 6174 682e 6578 6973 7473 2869 6e70 7574  ath.exists(input
-00028120: 6669 6c65 293a 0a20 2020 2020 2020 2020  file):.         
-00028130: 2020 2065 7272 6f72 2822 4e6f 2069 6e70     error("No inp
-00028140: 7574 2066 696c 6520 666f 756e 6420 6e6f  ut file found no
-00028150: 7220 6465 6661 756c 7420 6b63 6c69 5f70  r default kcli_p
-00028160: 6c61 6e2e 796d 6c2e 4c65 6176 696e 672e  lan.yml.Leaving.
-00028170: 2e2e 2e22 290a 2020 2020 2020 2020 2020  ...").          
-00028180: 2020 7379 732e 6578 6974 2831 290a 2020    sys.exit(1).  
-00028190: 2020 2020 2020 7070 7269 6e74 2866 2248        pprint(f"H
-000281a0: 616e 646c 696e 6720 6578 706f 7365 206f  andling expose o
-000281b0: 6620 706c 616e 2077 6974 6820 6e61 6d65  f plan with name
-000281c0: 207b 706c 616e 7d20 616e 6420 696e 7075   {plan} and inpu
-000281d0: 7466 696c 6520 7b69 6e70 7574 6669 6c65  tfile {inputfile
-000281e0: 7d22 290a 2020 2020 2020 2020 6b65 7870  }").        kexp
-000281f0: 6f73 6572 203d 204b 6578 706f 7365 7228  oser = Kexposer(
-00028200: 7365 6c66 2c20 706c 616e 2c20 696e 7075  self, plan, inpu
-00028210: 7466 696c 652c 206f 7665 7272 6964 6573  tfile, overrides
-00028220: 3d6f 7665 7272 6964 6573 2c20 706f 7274  =overrides, port
-00028230: 3d70 6f72 742c 2070 666d 6f64 653d 7066  =port, pfmode=pf
-00028240: 6d6f 6465 2c20 636c 7573 7465 723d 636c  mode, cluster=cl
-00028250: 7573 7465 722c 0a20 2020 2020 2020 2020  uster,.         
+00028020: 2020 2062 7265 616b 0a20 2020 2020 2020     break.       
+00028030: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00028040: 662e 6b2e 6465 6c65 7465 2876 6d6e 616d  f.k.delete(vmnam
+00028050: 6529 0a0a 2020 2020 6465 6620 6578 706f  e)..    def expo
+00028060: 7365 5f70 6c61 6e28 7365 6c66 2c20 706c  se_plan(self, pl
+00028070: 616e 2c20 696e 7075 7466 696c 653d 4e6f  an, inputfile=No
+00028080: 6e65 2c20 6f76 6572 7269 6465 733d 7b7d  ne, overrides={}
+00028090: 2c20 706f 7274 3d39 3030 302c 2070 666d  , port=9000, pfm
+000280a0: 6f64 653d 4661 6c73 652c 2063 6c75 7374  ode=False, clust
+000280b0: 6572 3d46 616c 7365 2c20 6578 7472 6173  er=False, extras
+000280c0: 3d46 616c 7365 293a 0a20 2020 2020 2020  =False):.       
+000280d0: 2069 6e70 7574 6669 6c65 203d 206f 732e   inputfile = os.
+000280e0: 7061 7468 2e65 7870 616e 6475 7365 7228  path.expanduser(
+000280f0: 696e 7075 7466 696c 6529 0a20 2020 2020  inputfile).     
+00028100: 2020 2069 6620 6e6f 7420 6f73 2e70 6174     if not os.pat
+00028110: 682e 6578 6973 7473 2869 6e70 7574 6669  h.exists(inputfi
+00028120: 6c65 293a 0a20 2020 2020 2020 2020 2020  le):.           
+00028130: 2065 7272 6f72 2822 4e6f 2069 6e70 7574   error("No input
+00028140: 2066 696c 6520 666f 756e 6420 6e6f 7220   file found nor 
+00028150: 6465 6661 756c 7420 6b63 6c69 5f70 6c61  default kcli_pla
+00028160: 6e2e 796d 6c2e 4c65 6176 696e 672e 2e2e  n.yml.Leaving...
+00028170: 2e22 290a 2020 2020 2020 2020 2020 2020  .").            
+00028180: 7379 732e 6578 6974 2831 290a 2020 2020  sys.exit(1).    
+00028190: 2020 2020 7070 7269 6e74 2866 2248 616e      pprint(f"Han
+000281a0: 646c 696e 6720 6578 706f 7365 206f 6620  dling expose of 
+000281b0: 706c 616e 2077 6974 6820 6e61 6d65 207b  plan with name {
+000281c0: 706c 616e 7d20 616e 6420 696e 7075 7466  plan} and inputf
+000281d0: 696c 6520 7b69 6e70 7574 6669 6c65 7d22  ile {inputfile}"
+000281e0: 290a 2020 2020 2020 2020 6b65 7870 6f73  ).        kexpos
+000281f0: 6572 203d 204b 6578 706f 7365 7228 7365  er = Kexposer(se
+00028200: 6c66 2c20 706c 616e 2c20 696e 7075 7466  lf, plan, inputf
+00028210: 696c 652c 206f 7665 7272 6964 6573 3d6f  ile, overrides=o
+00028220: 7665 7272 6964 6573 2c20 706f 7274 3d70  verrides, port=p
+00028230: 6f72 742c 2070 666d 6f64 653d 7066 6d6f  ort, pfmode=pfmo
+00028240: 6465 2c20 636c 7573 7465 723d 636c 7573  de, cluster=clus
+00028250: 7465 722c 0a20 2020 2020 2020 2020 2020  ter,.           
 00028260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028270: 2020 2065 7874 7261 733d 6578 7472 6173     extras=extras
-00028280: 290a 2020 2020 2020 2020 6b65 7870 6f73  ).        kexpos
-00028290: 6572 2e72 756e 2829 0a0a 2020 2020 6465  er.run()..    de
-000282a0: 6620 6372 6561 7465 5f6f 7065 6e73 6869  f create_openshi
-000282b0: 6674 5f69 736f 2873 656c 662c 2063 6c75  ft_iso(self, clu
-000282c0: 7374 6572 2c20 6f76 6572 7269 6465 733d  ster, overrides=
-000282d0: 7b7d 2c20 6967 6e69 7469 6f6e 6669 6c65  {}, ignitionfile
-000282e0: 3d4e 6f6e 652c 2069 6e73 7461 6c6c 6572  =None, installer
-000282f0: 3d46 616c 7365 2c20 6469 7265 6374 3d46  =False, direct=F
-00028300: 616c 7365 293a 0a20 2020 2020 2020 206d  alse):.        m
-00028310: 6574 616c 5f75 726c 203d 204e 6f6e 650a  etal_url = None.
-00028320: 2020 2020 2020 2020 6973 6f5f 7665 7273          iso_vers
-00028330: 696f 6e20 3d20 7374 7228 6f76 6572 7269  ion = str(overri
-00028340: 6465 732e 6765 7428 2776 6572 7369 6f6e  des.get('version
-00028350: 272c 2027 6c61 7465 7374 2729 290a 2020  ', 'latest')).  
-00028360: 2020 2020 2020 6966 206e 6f74 2069 6e73        if not ins
-00028370: 7461 6c6c 6572 3a0a 2020 2020 2020 2020  taller:.        
-00028380: 2020 2020 6966 2069 736f 5f76 6572 7369      if iso_versi
-00028390: 6f6e 206e 6f74 2069 6e20 5b27 6c61 7465  on not in ['late
-000283a0: 7374 272c 2027 7072 652d 7265 6c65 6173  st', 'pre-releas
-000283b0: 6527 5d20 616e 6420 6e6f 7420 6973 6f5f  e'] and not iso_
-000283c0: 7665 7273 696f 6e2e 7374 6172 7473 7769  version.startswi
-000283d0: 7468 2827 342e 2729 3a0a 2020 2020 2020  th('4.'):.      
-000283e0: 2020 2020 2020 2020 2020 7761 726e 696e            warnin
-000283f0: 6728 2246 6f72 6369 6e67 206c 6976 6520  g("Forcing live 
-00028400: 6973 6f20 7665 7273 696f 6e20 746f 206c  iso version to l
-00028410: 6174 6573 7422 290a 2020 2020 2020 2020  atest").        
-00028420: 2020 2020 2020 2020 6973 6f5f 7665 7273          iso_vers
-00028430: 696f 6e20 3d20 276c 6174 6573 7427 0a20  ion = 'latest'. 
-00028440: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-00028450: 6973 6f5f 7665 7273 696f 6e2e 7374 6172  iso_version.star
-00028460: 7473 7769 7468 2827 342e 2729 3a0a 2020  tswith('4.'):.  
-00028470: 2020 2020 2020 2020 2020 2020 2020 6d69                mi
-00028480: 6e6f 725f 7665 7273 696f 6e20 3d20 6973  nor_version = is
-00028490: 6f5f 7665 7273 696f 6e2e 7370 6c69 7428  o_version.split(
-000284a0: 272e 2729 5b31 5d0a 2020 2020 2020 2020  '.')[1].        
-000284b0: 2020 2020 2020 2020 6966 206d 696e 6f72          if minor
-000284c0: 5f76 6572 7369 6f6e 2e69 7364 6967 6974  _version.isdigit
-000284d0: 2829 2061 6e64 2069 6e74 286d 696e 6f72  () and int(minor
-000284e0: 5f76 6572 7369 6f6e 2920 3c20 363a 0a20  _version) < 6:. 
+00028270: 2065 7874 7261 733d 6578 7472 6173 290a   extras=extras).
+00028280: 2020 2020 2020 2020 6b65 7870 6f73 6572          kexposer
+00028290: 2e72 756e 2829 0a0a 2020 2020 6465 6620  .run()..    def 
+000282a0: 6372 6561 7465 5f6f 7065 6e73 6869 6674  create_openshift
+000282b0: 5f69 736f 2873 656c 662c 2063 6c75 7374  _iso(self, clust
+000282c0: 6572 2c20 6f76 6572 7269 6465 733d 7b7d  er, overrides={}
+000282d0: 2c20 6967 6e69 7469 6f6e 6669 6c65 3d4e  , ignitionfile=N
+000282e0: 6f6e 652c 2069 6e73 7461 6c6c 6572 3d46  one, installer=F
+000282f0: 616c 7365 2c20 6469 7265 6374 3d46 616c  alse, direct=Fal
+00028300: 7365 293a 0a20 2020 2020 2020 206d 6574  se):.        met
+00028310: 616c 5f75 726c 203d 204e 6f6e 650a 2020  al_url = None.  
+00028320: 2020 2020 2020 6973 6f5f 7665 7273 696f        iso_versio
+00028330: 6e20 3d20 7374 7228 6f76 6572 7269 6465  n = str(override
+00028340: 732e 6765 7428 2776 6572 7369 6f6e 272c  s.get('version',
+00028350: 2027 6c61 7465 7374 2729 290a 2020 2020   'latest')).    
+00028360: 2020 2020 6966 206e 6f74 2069 6e73 7461      if not insta
+00028370: 6c6c 6572 3a0a 2020 2020 2020 2020 2020  ller:.          
+00028380: 2020 6966 2069 736f 5f76 6572 7369 6f6e    if iso_version
+00028390: 206e 6f74 2069 6e20 5b27 6c61 7465 7374   not in ['latest
+000283a0: 272c 2027 7072 652d 7265 6c65 6173 6527  ', 'pre-release'
+000283b0: 5d20 616e 6420 6e6f 7420 6973 6f5f 7665  ] and not iso_ve
+000283c0: 7273 696f 6e2e 7374 6172 7473 7769 7468  rsion.startswith
+000283d0: 2827 342e 2729 3a0a 2020 2020 2020 2020  ('4.'):.        
+000283e0: 2020 2020 2020 2020 7761 726e 696e 6728          warning(
+000283f0: 2246 6f72 6369 6e67 206c 6976 6520 6973  "Forcing live is
+00028400: 6f20 7665 7273 696f 6e20 746f 206c 6174  o version to lat
+00028410: 6573 7422 290a 2020 2020 2020 2020 2020  est").          
+00028420: 2020 2020 2020 6973 6f5f 7665 7273 696f        iso_versio
+00028430: 6e20 3d20 276c 6174 6573 7427 0a20 2020  n = 'latest'.   
+00028440: 2020 2020 2020 2020 2065 6c69 6620 6973           elif is
+00028450: 6f5f 7665 7273 696f 6e2e 7374 6172 7473  o_version.starts
+00028460: 7769 7468 2827 342e 2729 3a0a 2020 2020  with('4.'):.    
+00028470: 2020 2020 2020 2020 2020 2020 6d69 6e6f              mino
+00028480: 725f 7665 7273 696f 6e20 3d20 6973 6f5f  r_version = iso_
+00028490: 7665 7273 696f 6e2e 7370 6c69 7428 272e  version.split('.
+000284a0: 2729 5b31 5d0a 2020 2020 2020 2020 2020  ')[1].          
+000284b0: 2020 2020 2020 6966 206d 696e 6f72 5f76        if minor_v
+000284c0: 6572 7369 6f6e 2e69 7364 6967 6974 2829  ersion.isdigit()
+000284d0: 2061 6e64 2069 6e74 286d 696e 6f72 5f76   and int(minor_v
+000284e0: 6572 7369 6f6e 2920 3c20 363a 0a20 2020  ersion) < 6:.   
 000284f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028500: 2020 206d 6574 616c 5f75 726c 203d 2066     metal_url = f
-00028510: 2268 7474 7073 3a2f 2f6d 6972 726f 722e  "https://mirror.
-00028520: 6f70 656e 7368 6966 742e 636f 6d2f 7075  openshift.com/pu
-00028530: 622f 6f70 656e 7368 6966 742d 7634 2f64  b/openshift-v4/d
-00028540: 6570 656e 6465 6e63 6965 732f 7268 636f  ependencies/rhco
-00028550: 732f 7b69 736f 5f76 6572 7369 6f6e 7d2f  s/{iso_version}/
-00028560: 6c61 7465 7374 220a 2020 2020 2020 2020  latest".        
-00028570: 2020 2020 2020 2020 2020 2020 6d65 7461              meta
-00028580: 6c5f 7572 6c20 2b3d 2022 2f72 6863 6f73  l_url += "/rhcos
-00028590: 2d6d 6574 616c 2e78 3836 5f36 342e 7261  -metal.x86_64.ra
-000285a0: 772e 677a 220a 2020 2020 2020 2020 2020  w.gz".          
-000285b0: 2020 2020 2020 2020 2020 7761 726e 696e            warnin
-000285c0: 6728 2245 6d62 6564 6469 6e67 206d 6574  g("Embedding met
-000285d0: 616c 2075 726c 2069 6e20 6973 6f20 666f  al url in iso fo
-000285e0: 7220 7461 7267 6574 2076 6572 7369 6f6e  r target version
-000285f0: 2061 6e64 2069 6e73 7461 6c6c 696e 6720   and installing 
-00028600: 7769 7468 2061 206d 6f72 6520 7265 6365  with a more rece
-00028610: 6e74 2069 736f 2229 0a20 2020 2020 2020  nt iso").       
-00028620: 2020 2020 2020 2020 2069 736f 5f76 6572           iso_ver
-00028630: 7369 6f6e 203d 2027 6c61 7465 7374 270a  sion = 'latest'.
-00028640: 2020 2020 2020 2020 6170 695f 6970 203d          api_ip =
-00028650: 206f 7665 7272 6964 6573 2e67 6574 2827   overrides.get('
-00028660: 6170 695f 6970 2729 0a20 2020 2020 2020  api_ip').       
-00028670: 2069 676e 6974 696f 6e5f 7665 7273 696f   ignition_versio
-00028680: 6e20 3d20 6f76 6572 7269 6465 732e 6765  n = overrides.ge
-00028690: 7428 2769 676e 6974 696f 6e5f 7665 7273  t('ignition_vers
-000286a0: 696f 6e27 2c0a 2020 2020 2020 2020 2020  ion',.          
+00028500: 206d 6574 616c 5f75 726c 203d 2066 2268   metal_url = f"h
+00028510: 7474 7073 3a2f 2f6d 6972 726f 722e 6f70  ttps://mirror.op
+00028520: 656e 7368 6966 742e 636f 6d2f 7075 622f  enshift.com/pub/
+00028530: 6f70 656e 7368 6966 742d 7634 2f64 6570  openshift-v4/dep
+00028540: 656e 6465 6e63 6965 732f 7268 636f 732f  endencies/rhcos/
+00028550: 7b69 736f 5f76 6572 7369 6f6e 7d2f 6c61  {iso_version}/la
+00028560: 7465 7374 220a 2020 2020 2020 2020 2020  test".          
+00028570: 2020 2020 2020 2020 2020 6d65 7461 6c5f            metal_
+00028580: 7572 6c20 2b3d 2022 2f72 6863 6f73 2d6d  url += "/rhcos-m
+00028590: 6574 616c 2e78 3836 5f36 342e 7261 772e  etal.x86_64.raw.
+000285a0: 677a 220a 2020 2020 2020 2020 2020 2020  gz".            
+000285b0: 2020 2020 2020 2020 7761 726e 696e 6728          warning(
+000285c0: 2245 6d62 6564 6469 6e67 206d 6574 616c  "Embedding metal
+000285d0: 2075 726c 2069 6e20 6973 6f20 666f 7220   url in iso for 
+000285e0: 7461 7267 6574 2076 6572 7369 6f6e 2061  target version a
+000285f0: 6e64 2069 6e73 7461 6c6c 696e 6720 7769  nd installing wi
+00028600: 7468 2061 206d 6f72 6520 7265 6365 6e74  th a more recent
+00028610: 2069 736f 2229 0a20 2020 2020 2020 2020   iso").         
+00028620: 2020 2020 2020 2069 736f 5f76 6572 7369         iso_versi
+00028630: 6f6e 203d 2027 6c61 7465 7374 270a 2020  on = 'latest'.  
+00028640: 2020 2020 2020 6170 695f 6970 203d 206f        api_ip = o
+00028650: 7665 7272 6964 6573 2e67 6574 2827 6170  verrides.get('ap
+00028660: 695f 6970 2729 0a20 2020 2020 2020 2069  i_ip').        i
+00028670: 676e 6974 696f 6e5f 7665 7273 696f 6e20  gnition_version 
+00028680: 3d20 6f76 6572 7269 6465 732e 6765 7428  = overrides.get(
+00028690: 2769 676e 6974 696f 6e5f 7665 7273 696f  'ignition_versio
+000286a0: 6e27 2c0a 2020 2020 2020 2020 2020 2020  n',.            
 000286b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000286c0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-000286d0: 6f6d 6d6f 6e2e 6967 6e69 7469 6f6e 5f76  ommon.ignition_v
-000286e0: 6572 7369 6f6e 2822 7268 636f 732d 2573  ersion("rhcos-%s
-000286f0: 2220 2520 6973 6f5f 7665 7273 696f 6e2e  " % iso_version.
-00028700: 7265 706c 6163 6528 272e 272c 2027 2729  replace('.', '')
-00028710: 2929 0a20 2020 2020 2020 2072 6f6c 6520  )).        role 
-00028720: 3d20 6f76 6572 7269 6465 732e 6765 7428  = overrides.get(
-00028730: 2772 6f6c 6527 2c20 2777 6f72 6b65 7227  'role', 'worker'
-00028740: 290a 2020 2020 2020 2020 6973 6f20 3d20  ).        iso = 
-00028750: 6f76 6572 7269 6465 732e 6765 7428 2769  overrides.get('i
-00028760: 736f 272c 2054 7275 6529 0a20 2020 2020  so', True).     
-00028770: 2020 2064 6f6d 6169 6e20 3d20 6f76 6572     domain = over
-00028780: 7269 6465 732e 6765 7428 2764 6f6d 6169  rides.get('domai
-00028790: 6e27 290a 2020 2020 2020 2020 6966 2027  n').        if '
-000287a0: 2e27 2069 6e20 636c 7573 7465 723a 0a20  .' in cluster:. 
-000287b0: 2020 2020 2020 2020 2020 2064 6f6d 6169             domai
-000287c0: 6e20 3d20 272e 272e 6a6f 696e 2863 6c75  n = '.'.join(clu
-000287d0: 7374 6572 2e73 706c 6974 2827 2e27 295b  ster.split('.')[
-000287e0: 313a 5d29 0a20 2020 2020 2020 2020 2020  1:]).           
-000287f0: 2070 7072 696e 7428 6622 5573 696e 6720   pprint(f"Using 
-00028800: 646f 6d61 696e 207b 646f 6d61 696e 7d22  domain {domain}"
-00028810: 290a 2020 2020 2020 2020 2020 2020 636c  ).            cl
-00028820: 7573 7465 7220 3d20 636c 7573 7465 722e  uster = cluster.
-00028830: 7265 706c 6163 6528 6622 2e7b 646f 6d61  replace(f".{doma
-00028840: 696e 7d22 2c20 2727 290a 2020 2020 2020  in}", '').      
-00028850: 2020 6966 2063 6c75 7374 6572 2e73 7461    if cluster.sta
-00028860: 7274 7377 6974 6828 2761 7069 2e27 293a  rtswith('api.'):
-00028870: 0a20 2020 2020 2020 2020 2020 2063 6c75  .            clu
-00028880: 7374 6572 203d 2063 6c75 7374 6572 2e72  ster = cluster.r
-00028890: 6570 6c61 6365 2822 6170 692e 222c 2027  eplace("api.", '
-000288a0: 2729 0a20 2020 2020 2020 2020 2020 2070  ').            p
-000288b0: 7072 696e 7428 6622 5573 696e 6720 636c  print(f"Using cl
-000288c0: 7573 7465 7220 7b63 6c75 7374 6572 7d22  uster {cluster}"
-000288d0: 290a 2020 2020 2020 2020 686f 7374 735f  ).        hosts_
-000288e0: 636f 6e74 656e 7420 3d20 4e6f 6e65 0a20  content = None. 
-000288f0: 2020 2020 2020 2066 696e 616c 6461 7461         finaldata
-00028900: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
-00028910: 6966 2069 676e 6974 696f 6e66 696c 6520  if ignitionfile 
-00028920: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00028930: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
-00028940: 6f73 2e70 6174 682e 6578 6973 7473 2869  os.path.exists(i
-00028950: 676e 6974 696f 6e66 696c 6529 3a0a 2020  gnitionfile):.  
-00028960: 2020 2020 2020 2020 2020 2020 2020 6572                er
-00028970: 726f 7228 6622 7b69 676e 6974 696f 6e66  ror(f"{ignitionf
-00028980: 696c 657d 206e 6f74 2066 6f75 6e64 2229  ile} not found")
-00028990: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000289a0: 2073 7973 2e65 7869 7428 3129 0a20 2020   sys.exit(1).   
-000289b0: 2020 2020 2020 2020 2066 696e 616c 6461           finalda
-000289c0: 7461 203d 206f 7065 6e28 6967 6e69 7469  ta = open(igniti
-000289d0: 6f6e 6669 6c65 292e 7265 6164 2829 0a20  onfile).read(). 
-000289e0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-000289f0: 2020 2020 2020 2020 2069 676e 6974 696f           ignitio
-00028a00: 6e66 696c 6520 3d20 6622 7b72 6f6c 657d  nfile = f"{role}
-00028a10: 2e69 676e 220a 2020 2020 2020 2020 2020  .ign".          
-00028a20: 2020 6966 206f 732e 7061 7468 2e65 7869    if os.path.exi
-00028a30: 7374 7328 6967 6e69 7469 6f6e 6669 6c65  sts(ignitionfile
-00028a40: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00028a50: 2020 2077 6172 6e69 6e67 2866 2255 7369     warning(f"Usi
-00028a60: 6e67 2065 7869 7374 696e 6720 7b69 676e  ng existing {ign
-00028a70: 6974 696f 6e66 696c 657d 2229 0a20 2020  itionfile}").   
-00028a80: 2020 2020 2020 2020 2020 2020 2066 696e               fin
-00028a90: 616c 6461 7461 203d 206f 7065 6e28 6967  aldata = open(ig
-00028aa0: 6e69 7469 6f6e 6669 6c65 292e 7265 6164  nitionfile).read
-00028ab0: 2829 0a20 2020 2020 2020 2020 2020 2065  ().            e
-00028ac0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00028ad0: 2020 2020 2069 6620 6170 695f 6970 2069       if api_ip i
-00028ae0: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-00028af0: 2020 2020 2020 2020 2020 2020 7472 793a              try:
-00028b00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00028b10: 2020 2020 2020 2020 2061 7069 5f69 7020           api_ip 
-00028b20: 3d20 736f 636b 6574 2e67 6574 686f 7374  = socket.gethost
-00028b30: 6279 6e61 6d65 2866 2761 7069 2e7b 636c  byname(f'api.{cl
-00028b40: 7573 7465 727d 2e7b 646f 6d61 696e 7d27  uster}.{domain}'
-00028b50: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00028b60: 2020 2020 2020 6578 6365 7074 3a0a 2020        except:.  
+000286c0: 2020 2020 2020 2020 2020 2020 2063 6f6d               com
+000286d0: 6d6f 6e2e 6967 6e69 7469 6f6e 5f76 6572  mon.ignition_ver
+000286e0: 7369 6f6e 2822 7268 636f 732d 2573 2220  sion("rhcos-%s" 
+000286f0: 2520 6973 6f5f 7665 7273 696f 6e2e 7265  % iso_version.re
+00028700: 706c 6163 6528 272e 272c 2027 2729 2929  place('.', '')))
+00028710: 0a20 2020 2020 2020 2072 6f6c 6520 3d20  .        role = 
+00028720: 6f76 6572 7269 6465 732e 6765 7428 2772  overrides.get('r
+00028730: 6f6c 6527 2c20 2777 6f72 6b65 7227 290a  ole', 'worker').
+00028740: 2020 2020 2020 2020 6973 6f20 3d20 6f76          iso = ov
+00028750: 6572 7269 6465 732e 6765 7428 2769 736f  errides.get('iso
+00028760: 272c 2054 7275 6529 0a20 2020 2020 2020  ', True).       
+00028770: 2064 6f6d 6169 6e20 3d20 6f76 6572 7269   domain = overri
+00028780: 6465 732e 6765 7428 2764 6f6d 6169 6e27  des.get('domain'
+00028790: 290a 2020 2020 2020 2020 6966 2027 2e27  ).        if '.'
+000287a0: 2069 6e20 636c 7573 7465 723a 0a20 2020   in cluster:.   
+000287b0: 2020 2020 2020 2020 2064 6f6d 6169 6e20           domain 
+000287c0: 3d20 272e 272e 6a6f 696e 2863 6c75 7374  = '.'.join(clust
+000287d0: 6572 2e73 706c 6974 2827 2e27 295b 313a  er.split('.')[1:
+000287e0: 5d29 0a20 2020 2020 2020 2020 2020 2070  ]).            p
+000287f0: 7072 696e 7428 6622 5573 696e 6720 646f  print(f"Using do
+00028800: 6d61 696e 207b 646f 6d61 696e 7d22 290a  main {domain}").
+00028810: 2020 2020 2020 2020 2020 2020 636c 7573              clus
+00028820: 7465 7220 3d20 636c 7573 7465 722e 7265  ter = cluster.re
+00028830: 706c 6163 6528 6622 2e7b 646f 6d61 696e  place(f".{domain
+00028840: 7d22 2c20 2727 290a 2020 2020 2020 2020  }", '').        
+00028850: 6966 2063 6c75 7374 6572 2e73 7461 7274  if cluster.start
+00028860: 7377 6974 6828 2761 7069 2e27 293a 0a20  swith('api.'):. 
+00028870: 2020 2020 2020 2020 2020 2063 6c75 7374             clust
+00028880: 6572 203d 2063 6c75 7374 6572 2e72 6570  er = cluster.rep
+00028890: 6c61 6365 2822 6170 692e 222c 2027 2729  lace("api.", '')
+000288a0: 0a20 2020 2020 2020 2020 2020 2070 7072  .            ppr
+000288b0: 696e 7428 6622 5573 696e 6720 636c 7573  int(f"Using clus
+000288c0: 7465 7220 7b63 6c75 7374 6572 7d22 290a  ter {cluster}").
+000288d0: 2020 2020 2020 2020 686f 7374 735f 636f          hosts_co
+000288e0: 6e74 656e 7420 3d20 4e6f 6e65 0a20 2020  ntent = None.   
+000288f0: 2020 2020 2066 696e 616c 6461 7461 203d       finaldata =
+00028900: 204e 6f6e 650a 2020 2020 2020 2020 6966   None.        if
+00028910: 2069 676e 6974 696f 6e66 696c 6520 6973   ignitionfile is
+00028920: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00028930: 2020 2020 2020 2069 6620 6e6f 7420 6f73         if not os
+00028940: 2e70 6174 682e 6578 6973 7473 2869 676e  .path.exists(ign
+00028950: 6974 696f 6e66 696c 6529 3a0a 2020 2020  itionfile):.    
+00028960: 2020 2020 2020 2020 2020 2020 6572 726f              erro
+00028970: 7228 6622 7b69 676e 6974 696f 6e66 696c  r(f"{ignitionfil
+00028980: 657d 206e 6f74 2066 6f75 6e64 2229 0a20  e} not found"). 
+00028990: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000289a0: 7973 2e65 7869 7428 3129 0a20 2020 2020  ys.exit(1).     
+000289b0: 2020 2020 2020 2066 696e 616c 6461 7461         finaldata
+000289c0: 203d 206f 7065 6e28 6967 6e69 7469 6f6e   = open(ignition
+000289d0: 6669 6c65 292e 7265 6164 2829 0a20 2020  file).read().   
+000289e0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+000289f0: 2020 2020 2020 2069 676e 6974 696f 6e66         ignitionf
+00028a00: 696c 6520 3d20 6622 7b72 6f6c 657d 2e69  ile = f"{role}.i
+00028a10: 676e 220a 2020 2020 2020 2020 2020 2020  gn".            
+00028a20: 6966 206f 732e 7061 7468 2e65 7869 7374  if os.path.exist
+00028a30: 7328 6967 6e69 7469 6f6e 6669 6c65 293a  s(ignitionfile):
+00028a40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00028a50: 2077 6172 6e69 6e67 2866 2255 7369 6e67   warning(f"Using
+00028a60: 2065 7869 7374 696e 6720 7b69 676e 6974   existing {ignit
+00028a70: 696f 6e66 696c 657d 2229 0a20 2020 2020  ionfile}").     
+00028a80: 2020 2020 2020 2020 2020 2066 696e 616c             final
+00028a90: 6461 7461 203d 206f 7065 6e28 6967 6e69  data = open(igni
+00028aa0: 7469 6f6e 6669 6c65 292e 7265 6164 2829  tionfile).read()
+00028ab0: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+00028ac0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00028ad0: 2020 2069 6620 6170 695f 6970 2069 7320     if api_ip is 
+00028ae0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00028af0: 2020 2020 2020 2020 2020 7472 793a 0a20            try:. 
+00028b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028b10: 2020 2020 2020 2061 7069 5f69 7020 3d20         api_ip = 
+00028b20: 736f 636b 6574 2e67 6574 686f 7374 6279  socket.gethostby
+00028b30: 6e61 6d65 2866 2761 7069 2e7b 636c 7573  name(f'api.{clus
+00028b40: 7465 727d 2e7b 646f 6d61 696e 7d27 290a  ter}.{domain}').
+00028b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028b60: 2020 2020 6578 6365 7074 3a0a 2020 2020      except:.    
 00028b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028b80: 2020 2020 2020 7061 7373 0a20 2020 2020        pass.     
-00028b90: 2020 2020 2020 2020 2020 2069 6620 6170             if ap
-00028ba0: 695f 6970 2069 7320 4e6f 6e65 3a0a 2020  i_ip is None:.  
+00028b80: 2020 2020 7061 7373 0a20 2020 2020 2020      pass.       
+00028b90: 2020 2020 2020 2020 2069 6620 6170 695f           if api_
+00028ba0: 6970 2069 7320 4e6f 6e65 3a0a 2020 2020  ip is None:.    
 00028bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028bc0: 2020 6966 2064 6f6d 6169 6e20 6973 204e    if domain is N
-00028bd0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00028be0: 2020 2020 2020 2020 2020 2020 2065 7272               err
-00028bf0: 6f72 2822 436f 756c 646e 2774 2066 6967  or("Couldn't fig
-00028c00: 7572 6520 6f75 7420 6170 695f 6970 206e  ure out api_ip n
-00028c10: 6f72 2072 656c 7920 6f6e 2064 6e73 2073  or rely on dns s
-00028c20: 696e 6365 2064 6f6d 6169 6e20 6973 206e  ince domain is n
-00028c30: 6f74 2073 6574 2229 0a20 2020 2020 2020  ot set").       
-00028c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028c50: 2073 7973 2e65 7869 7428 3129 0a20 2020   sys.exit(1).   
-00028c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028c70: 2077 6172 6e69 6e67 2822 436f 756c 646e   warning("Couldn
-00028c80: 2774 2066 6967 7572 6520 6f75 7420 6170  't figure out ap
-00028c90: 695f 6970 2e20 5265 6c79 696e 6720 6f6e  i_ip. Relying on
-00028ca0: 2064 6e73 2229 0a20 2020 2020 2020 2020   dns").         
-00028cb0: 2020 2020 2020 2020 2020 2061 7069 5f69             api_i
-00028cc0: 7020 3d20 6622 6170 692e 7b63 6c75 7374  p = f"api.{clust
-00028cd0: 6572 7d2e 7b64 6f6d 6169 6e7d 220a 2020  er}.{domain}".  
-00028ce0: 2020 2020 2020 2020 2020 2020 2020 656c                el
-00028cf0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00028d00: 2020 2020 2020 2020 686f 7374 735f 636f          hosts_co
-00028d10: 6e74 656e 7420 3d20 2231 3237 2e30 2e30  ntent = "127.0.0
-00028d20: 2e31 2020 206c 6f63 616c 686f 7374 206c  .1   localhost l
-00028d30: 6f63 616c 686f 7374 2e6c 6f63 616c 646f  ocalhost.localdo
-00028d40: 6d61 696e 206c 6f63 616c 686f 7374 3420  main localhost4 
-00028d50: 6c6f 6361 6c68 6f73 7434 2e6c 6f63 616c  localhost4.local
-00028d60: 646f 6d61 696e 345c 6e22 0a20 2020 2020  domain4\n".     
-00028d70: 2020 2020 2020 2020 2020 2020 2020 2068                 h
-00028d80: 6f73 7473 5f63 6f6e 7465 6e74 202b 3d20  osts_content += 
-00028d90: 223a 3a31 2020 2020 2020 2020 206c 6f63  "::1         loc
-00028da0: 616c 686f 7374 206c 6f63 616c 686f 7374  alhost localhost
-00028db0: 2e6c 6f63 616c 646f 6d61 696e 206c 6f63  .localdomain loc
-00028dc0: 616c 686f 7374 3620 6c6f 6361 6c68 6f73  alhost6 localhos
-00028dd0: 7436 2e6c 6f63 616c 646f 6d61 696e 365c  t6.localdomain6\
-00028de0: 6e22 0a20 2020 2020 2020 2020 2020 2020  n".             
-00028df0: 2020 2020 2020 2068 6f73 7473 5f63 6f6e         hosts_con
-00028e00: 7465 6e74 202b 3d20 6622 7b61 7069 5f69  tent += f"{api_i
-00028e10: 707d 2061 7069 2d69 6e74 2e7b 636c 7573  p} api-int.{clus
-00028e20: 7465 727d 2e7b 646f 6d61 696e 7d20 6170  ter}.{domain} ap
-00028e30: 692e 7b63 6c75 7374 6572 7d2e 7b64 6f6d  i.{cluster}.{dom
-00028e40: 6169 6e7d 220a 2020 2020 2020 2020 706c  ain}".        pl
-00028e50: 616e 6469 7220 3d20 6f73 2e70 6174 682e  andir = os.path.
-00028e60: 6469 726e 616d 6528 6f70 656e 7368 6966  dirname(openshif
-00028e70: 742e 6372 6561 7465 2e5f 5f63 6f64 655f  t.create.__code_
-00028e80: 5f2e 636f 5f66 696c 656e 616d 6529 0a20  _.co_filename). 
-00028e90: 2020 2020 2020 2077 6974 6820 6f70 656e         with open
-00028ea0: 2822 6973 6f2e 6967 6e22 2c20 2777 2729  ("iso.ign", 'w')
-00028eb0: 2061 7320 663a 0a20 2020 2020 2020 2020   as f:.         
-00028ec0: 2020 2066 756c 6c5f 6e61 6d65 203d 2066     full_name = f
-00028ed0: 277b 636c 7573 7465 727d 2e7b 646f 6d61  '{cluster}.{doma
-00028ee0: 696e 7d27 2069 6620 646f 6d61 696e 2069  in}' if domain i
-00028ef0: 7320 6e6f 7420 4e6f 6e65 2065 6c73 6520  s not None else 
-00028f00: 636c 7573 7465 720a 2020 2020 2020 2020  cluster.        
-00028f10: 2020 2020 7070 7269 6e74 2866 2257 7269      pprint(f"Wri
-00028f20: 7469 6e67 2066 696c 6520 6973 6f2e 6967  ting file iso.ig
-00028f30: 6e20 666f 7220 7b72 6f6c 657d 2069 6e20  n for {role} in 
-00028f40: 7b66 756c 6c5f 6e61 6d65 7d22 290a 2020  {full_name}").  
-00028f50: 2020 2020 2020 2020 2020 6973 6f64 6972            isodir
-00028f60: 203d 206f 732e 7061 7468 2e64 6972 6e61   = os.path.dirna
-00028f70: 6d65 2863 6f6d 6d6f 6e2e 5f5f 6669 6c65  me(common.__file
-00028f80: 5f5f 290a 2020 2020 2020 2020 2020 2020  __).            
-00028f90: 6966 2066 696e 616c 6461 7461 2069 7320  if finaldata is 
-00028fa0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00028fb0: 2020 2020 2020 656e 7620 3d20 456e 7669        env = Envi
-00028fc0: 726f 6e6d 656e 7428 6c6f 6164 6572 3d46  ronment(loader=F
-00028fd0: 696c 6553 7973 7465 6d4c 6f61 6465 7228  ileSystemLoader(
-00028fe0: 6973 6f64 6972 292c 2065 7874 656e 7369  isodir), extensi
-00028ff0: 6f6e 733d 5b27 6a69 6e6a 6132 2e65 7874  ons=['jinja2.ext
-00029000: 2e64 6f27 5d2c 2074 7269 6d5f 626c 6f63  .do'], trim_bloc
-00029010: 6b73 3d54 7275 652c 0a20 2020 2020 2020  ks=True,.       
+00028bc0: 6966 2064 6f6d 6169 6e20 6973 204e 6f6e  if domain is Non
+00028bd0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00028be0: 2020 2020 2020 2020 2020 2065 7272 6f72             error
+00028bf0: 2822 436f 756c 646e 2774 2066 6967 7572  ("Couldn't figur
+00028c00: 6520 6f75 7420 6170 695f 6970 206e 6f72  e out api_ip nor
+00028c10: 2072 656c 7920 6f6e 2064 6e73 2073 696e   rely on dns sin
+00028c20: 6365 2064 6f6d 6169 6e20 6973 206e 6f74  ce domain is not
+00028c30: 2073 6574 2229 0a20 2020 2020 2020 2020   set").         
+00028c40: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00028c50: 7973 2e65 7869 7428 3129 0a20 2020 2020  ys.exit(1).     
+00028c60: 2020 2020 2020 2020 2020 2020 2020 2077                 w
+00028c70: 6172 6e69 6e67 2822 436f 756c 646e 2774  arning("Couldn't
+00028c80: 2066 6967 7572 6520 6f75 7420 6170 695f   figure out api_
+00028c90: 6970 2e20 5265 6c79 696e 6720 6f6e 2064  ip. Relying on d
+00028ca0: 6e73 2229 0a20 2020 2020 2020 2020 2020  ns").           
+00028cb0: 2020 2020 2020 2020 2061 7069 5f69 7020           api_ip 
+00028cc0: 3d20 6622 6170 692e 7b63 6c75 7374 6572  = f"api.{cluster
+00028cd0: 7d2e 7b64 6f6d 6169 6e7d 220a 2020 2020  }.{domain}".    
+00028ce0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00028cf0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00028d00: 2020 2020 2020 686f 7374 735f 636f 6e74        hosts_cont
+00028d10: 656e 7420 3d20 2231 3237 2e30 2e30 2e31  ent = "127.0.0.1
+00028d20: 2020 206c 6f63 616c 686f 7374 206c 6f63     localhost loc
+00028d30: 616c 686f 7374 2e6c 6f63 616c 646f 6d61  alhost.localdoma
+00028d40: 696e 206c 6f63 616c 686f 7374 3420 6c6f  in localhost4 lo
+00028d50: 6361 6c68 6f73 7434 2e6c 6f63 616c 646f  calhost4.localdo
+00028d60: 6d61 696e 345c 6e22 0a20 2020 2020 2020  main4\n".       
+00028d70: 2020 2020 2020 2020 2020 2020 2068 6f73               hos
+00028d80: 7473 5f63 6f6e 7465 6e74 202b 3d20 223a  ts_content += ":
+00028d90: 3a31 2020 2020 2020 2020 206c 6f63 616c  :1         local
+00028da0: 686f 7374 206c 6f63 616c 686f 7374 2e6c  host localhost.l
+00028db0: 6f63 616c 646f 6d61 696e 206c 6f63 616c  ocaldomain local
+00028dc0: 686f 7374 3620 6c6f 6361 6c68 6f73 7436  host6 localhost6
+00028dd0: 2e6c 6f63 616c 646f 6d61 696e 365c 6e22  .localdomain6\n"
+00028de0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00028df0: 2020 2020 2068 6f73 7473 5f63 6f6e 7465       hosts_conte
+00028e00: 6e74 202b 3d20 6622 7b61 7069 5f69 707d  nt += f"{api_ip}
+00028e10: 2061 7069 2d69 6e74 2e7b 636c 7573 7465   api-int.{cluste
+00028e20: 727d 2e7b 646f 6d61 696e 7d20 6170 692e  r}.{domain} api.
+00028e30: 7b63 6c75 7374 6572 7d2e 7b64 6f6d 6169  {cluster}.{domai
+00028e40: 6e7d 220a 2020 2020 2020 2020 706c 616e  n}".        plan
+00028e50: 6469 7220 3d20 6f73 2e70 6174 682e 6469  dir = os.path.di
+00028e60: 726e 616d 6528 6f70 656e 7368 6966 742e  rname(openshift.
+00028e70: 6372 6561 7465 2e5f 5f63 6f64 655f 5f2e  create.__code__.
+00028e80: 636f 5f66 696c 656e 616d 6529 0a20 2020  co_filename).   
+00028e90: 2020 2020 2077 6974 6820 6f70 656e 2822       with open("
+00028ea0: 6973 6f2e 6967 6e22 2c20 2777 2729 2061  iso.ign", 'w') a
+00028eb0: 7320 663a 0a20 2020 2020 2020 2020 2020  s f:.           
+00028ec0: 2066 756c 6c5f 6e61 6d65 203d 2066 277b   full_name = f'{
+00028ed0: 636c 7573 7465 727d 2e7b 646f 6d61 696e  cluster}.{domain
+00028ee0: 7d27 2069 6620 646f 6d61 696e 2069 7320  }' if domain is 
+00028ef0: 6e6f 7420 4e6f 6e65 2065 6c73 6520 636c  not None else cl
+00028f00: 7573 7465 720a 2020 2020 2020 2020 2020  uster.          
+00028f10: 2020 7070 7269 6e74 2866 2257 7269 7469    pprint(f"Writi
+00028f20: 6e67 2066 696c 6520 6973 6f2e 6967 6e20  ng file iso.ign 
+00028f30: 666f 7220 7b72 6f6c 657d 2069 6e20 7b66  for {role} in {f
+00028f40: 756c 6c5f 6e61 6d65 7d22 290a 2020 2020  ull_name}").    
+00028f50: 2020 2020 2020 2020 6973 6f64 6972 203d          isodir =
+00028f60: 206f 732e 7061 7468 2e64 6972 6e61 6d65   os.path.dirname
+00028f70: 2863 6f6d 6d6f 6e2e 5f5f 6669 6c65 5f5f  (common.__file__
+00028f80: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+00028f90: 2066 696e 616c 6461 7461 2069 7320 4e6f   finaldata is No
+00028fa0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00028fb0: 2020 2020 656e 7620 3d20 456e 7669 726f      env = Enviro
+00028fc0: 6e6d 656e 7428 6c6f 6164 6572 3d46 696c  nment(loader=Fil
+00028fd0: 6553 7973 7465 6d4c 6f61 6465 7228 6973  eSystemLoader(is
+00028fe0: 6f64 6972 292c 2065 7874 656e 7369 6f6e  odir), extension
+00028ff0: 733d 5b27 6a69 6e6a 6132 2e65 7874 2e64  s=['jinja2.ext.d
+00029000: 6f27 5d2c 2074 7269 6d5f 626c 6f63 6b73  o'], trim_blocks
+00029010: 3d54 7275 652c 0a20 2020 2020 2020 2020  =True,.         
 00029020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029030: 2020 2020 2020 2020 2020 206c 7374 7269             lstri
-00029040: 705f 626c 6f63 6b73 3d54 7275 6529 0a20  p_blocks=True). 
-00029050: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00029060: 656d 706c 203d 2065 6e76 2e67 6574 5f74  empl = env.get_t
-00029070: 656d 706c 6174 6528 6f73 2e70 6174 682e  emplate(os.path.
-00029080: 6261 7365 6e61 6d65 2822 6967 6e69 7469  basename("igniti
-00029090: 6f6e 2e6a 3222 2929 0a20 2020 2020 2020  on.j2")).       
-000290a0: 2020 2020 2020 2020 2069 6620 686f 7374           if host
-000290b0: 735f 636f 6e74 656e 7420 6973 206e 6f74  s_content is not
-000290c0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000290d0: 2020 2020 2020 2020 2020 2068 6f73 7473             hosts
-000290e0: 5f63 6f6e 7465 6e74 203d 2062 6173 6536  _content = base6
-000290f0: 342e 6236 3465 6e63 6f64 6528 686f 7374  4.b64encode(host
-00029100: 735f 636f 6e74 656e 742e 656e 636f 6465  s_content.encode
-00029110: 2829 292e 6465 636f 6465 2822 5554 462d  ()).decode("UTF-
-00029120: 3822 290a 2020 2020 2020 2020 2020 2020  8").            
-00029130: 2020 2020 6675 6c6c 5f69 7020 3d20 6170      full_ip = ap
-00029140: 695f 6970 0a20 2020 2020 2020 2020 2020  i_ip.           
-00029150: 2020 2020 2069 6620 273a 2720 696e 2061       if ':' in a
-00029160: 7069 5f69 703a 0a20 2020 2020 2020 2020  pi_ip:.         
-00029170: 2020 2020 2020 2020 2020 2066 756c 6c5f             full_
-00029180: 6970 203d 2066 225b 7b61 7069 5f69 707d  ip = f"[{api_ip}
-00029190: 5d22 0a20 2020 2020 2020 2020 2020 2020  ]".             
-000291a0: 2020 2063 6f6e 6669 675f 726f 6c65 203d     config_role =
-000291b0: 2027 6d61 7374 6572 2720 6966 2072 6f6c   'master' if rol
-000291c0: 6520 3d3d 2027 6374 6c70 6c61 6e65 2720  e == 'ctlplane' 
-000291d0: 656c 7365 2072 6f6c 650a 2020 2020 2020  else role.      
-000291e0: 2020 2020 2020 2020 2020 6967 6e69 7469            igniti
-000291f0: 6f6e 5f75 726c 203d 2066 2268 7474 703a  on_url = f"http:
-00029200: 2f2f 7b66 756c 6c5f 6970 7d3a 3232 3632  //{full_ip}:2262
-00029210: 342f 636f 6e66 6967 2f7b 636f 6e66 6967  4/config/{config
-00029220: 5f72 6f6c 657d 220a 2020 2020 2020 2020  _role}".        
-00029230: 2020 2020 2020 2020 6669 6e61 6c64 6174          finaldat
-00029240: 6120 3d20 7465 6d70 6c2e 7265 6e64 6572  a = templ.render
-00029250: 2869 676e 6974 696f 6e5f 7572 6c3d 6967  (ignition_url=ig
-00029260: 6e69 7469 6f6e 5f75 726c 2c20 686f 7374  nition_url, host
-00029270: 735f 636f 6e74 656e 743d 686f 7374 735f  s_content=hosts_
-00029280: 636f 6e74 656e 742c 0a20 2020 2020 2020  content,.       
+00029030: 2020 2020 2020 2020 206c 7374 7269 705f           lstrip_
+00029040: 626c 6f63 6b73 3d54 7275 6529 0a20 2020  blocks=True).   
+00029050: 2020 2020 2020 2020 2020 2020 2074 656d               tem
+00029060: 706c 203d 2065 6e76 2e67 6574 5f74 656d  pl = env.get_tem
+00029070: 706c 6174 6528 6f73 2e70 6174 682e 6261  plate(os.path.ba
+00029080: 7365 6e61 6d65 2822 6967 6e69 7469 6f6e  sename("ignition
+00029090: 2e6a 3222 2929 0a20 2020 2020 2020 2020  .j2")).         
+000290a0: 2020 2020 2020 2069 6620 686f 7374 735f         if hosts_
+000290b0: 636f 6e74 656e 7420 6973 206e 6f74 204e  content is not N
+000290c0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000290d0: 2020 2020 2020 2020 2068 6f73 7473 5f63           hosts_c
+000290e0: 6f6e 7465 6e74 203d 2062 6173 6536 342e  ontent = base64.
+000290f0: 6236 3465 6e63 6f64 6528 686f 7374 735f  b64encode(hosts_
+00029100: 636f 6e74 656e 742e 656e 636f 6465 2829  content.encode()
+00029110: 292e 6465 636f 6465 2822 5554 462d 3822  ).decode("UTF-8"
+00029120: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00029130: 2020 6675 6c6c 5f69 7020 3d20 6170 695f    full_ip = api_
+00029140: 6970 0a20 2020 2020 2020 2020 2020 2020  ip.             
+00029150: 2020 2069 6620 273a 2720 696e 2061 7069     if ':' in api
+00029160: 5f69 703a 0a20 2020 2020 2020 2020 2020  _ip:.           
+00029170: 2020 2020 2020 2020 2066 756c 6c5f 6970           full_ip
+00029180: 203d 2066 225b 7b61 7069 5f69 707d 5d22   = f"[{api_ip}]"
+00029190: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000291a0: 2063 6f6e 6669 675f 726f 6c65 203d 2027   config_role = '
+000291b0: 6d61 7374 6572 2720 6966 2072 6f6c 6520  master' if role 
+000291c0: 3d3d 2027 6374 6c70 6c61 6e65 2720 656c  == 'ctlplane' el
+000291d0: 7365 2072 6f6c 650a 2020 2020 2020 2020  se role.        
+000291e0: 2020 2020 2020 2020 6967 6e69 7469 6f6e          ignition
+000291f0: 5f75 726c 203d 2066 2268 7474 703a 2f2f  _url = f"http://
+00029200: 7b66 756c 6c5f 6970 7d3a 3232 3632 342f  {full_ip}:22624/
+00029210: 636f 6e66 6967 2f7b 636f 6e66 6967 5f72  config/{config_r
+00029220: 6f6c 657d 220a 2020 2020 2020 2020 2020  ole}".          
+00029230: 2020 2020 2020 6669 6e61 6c64 6174 6120        finaldata 
+00029240: 3d20 7465 6d70 6c2e 7265 6e64 6572 2869  = templ.render(i
+00029250: 676e 6974 696f 6e5f 7572 6c3d 6967 6e69  gnition_url=igni
+00029260: 7469 6f6e 5f75 726c 2c20 686f 7374 735f  tion_url, hosts_
+00029270: 636f 6e74 656e 743d 686f 7374 735f 636f  content=hosts_co
+00029280: 6e74 656e 742c 0a20 2020 2020 2020 2020  ntent,.         
 00029290: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000292a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000292b0: 2020 6967 6e69 7469 6f6e 5f76 6572 7369    ignition_versi
-000292c0: 6f6e 3d69 676e 6974 696f 6e5f 7665 7273  on=ignition_vers
-000292d0: 696f 6e29 0a20 2020 2020 2020 2020 2020  ion).           
-000292e0: 2069 6620 6469 7265 6374 3a0a 2020 2020   if direct:.    
-000292f0: 2020 2020 2020 2020 2020 2020 662e 7772              f.wr
-00029300: 6974 6528 6669 6e61 6c64 6174 6129 0a20  ite(finaldata). 
-00029310: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00029320: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00029330: 205f 6669 6c65 7320 3d20 5b7b 2270 6174   _files = [{"pat
-00029340: 6822 3a20 222f 726f 6f74 2f63 6f6e 6669  h": "/root/confi
-00029350: 672e 6967 6e22 2c20 2263 6f6e 7465 6e74  g.ign", "content
-00029360: 223a 2066 696e 616c 6461 7461 7d5d 0a20  ": finaldata}]. 
-00029370: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00029380: 6620 6f73 2e70 6174 682e 6578 6973 7473  f os.path.exists
-00029390: 2827 6973 6f2e 7368 2729 3a0a 2020 2020  ('iso.sh'):.    
-000293a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000293b0: 7070 7269 6e74 2822 5573 696e 6720 6c6f  pprint("Using lo
-000293c0: 6361 6c20 6973 6f2e 7368 2073 6372 6970  cal iso.sh scrip
-000293d0: 7422 290a 2020 2020 2020 2020 2020 2020  t").            
-000293e0: 2020 2020 2020 2020 6973 6f73 6372 6970          isoscrip
-000293f0: 7420 3d20 2769 736f 2e73 6827 0a20 2020  t = 'iso.sh'.   
-00029400: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-00029410: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00029420: 2020 2020 2020 2069 736f 7363 7269 7074         isoscript
-00029430: 203d 2066 277b 706c 616e 6469 727d 2f69   = f'{plandir}/i
-00029440: 736f 2e73 6827 0a20 2020 2020 2020 2020  so.sh'.         
-00029450: 2020 2020 2020 2063 6c75 7374 6572 6469         clusterdi
-00029460: 7220 3d20 6f73 2e70 6174 682e 6578 7061  r = os.path.expa
-00029470: 6e64 7573 6572 2866 227e 2f2e 6b63 6c69  nduser(f"~/.kcli
-00029480: 2f63 6c75 7374 6572 732f 7b63 6c75 7374  /clusters/{clust
-00029490: 6572 7d22 290a 2020 2020 2020 2020 2020  er}").          
-000294a0: 2020 2020 2020 6966 206f 732e 7061 7468        if os.path
-000294b0: 2e65 7869 7374 7328 6627 7b63 6c75 7374  .exists(f'{clust
-000294c0: 6572 6469 727d 2f6d 6163 732e 7478 7427  erdir}/macs.txt'
-000294d0: 2920 6f72 206f 732e 7061 7468 2e65 7869  ) or os.path.exi
-000294e0: 7374 7328 276d 6163 732e 7478 7427 293a  sts('macs.txt'):
-000294f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00029500: 2020 2020 206d 6163 7364 6972 203d 2066       macsdir = f
-00029510: 277b 636c 7573 7465 7264 6972 7d27 2069  '{clusterdir}' i
-00029520: 6620 6f73 2e70 6174 682e 6578 6973 7473  f os.path.exists
-00029530: 2863 6c75 7374 6572 6469 7229 2065 6c73  (clusterdir) els
-00029540: 6520 272e 270a 2020 2020 2020 2020 2020  e '.'.          
-00029550: 2020 2020 2020 2020 2020 5f66 696c 6573            _files
-00029560: 2e61 7070 656e 6428 7b22 7061 7468 223a  .append({"path":
-00029570: 2022 2f72 6f6f 742f 6d61 6373 2e74 7874   "/root/macs.txt
-00029580: 222c 2022 6f72 6967 696e 223a 2066 277b  ", "origin": f'{
-00029590: 6d61 6373 6469 727d 2f6d 6163 732e 7478  macsdir}/macs.tx
-000295a0: 7427 7d29 0a20 2020 2020 2020 2020 2020  t'}).           
-000295b0: 2020 2020 2069 736f 5f6f 7665 7272 6964       iso_overrid
-000295c0: 6573 203d 207b 2773 6372 6970 7473 273a  es = {'scripts':
-000295d0: 205b 6973 6f73 6372 6970 745d 2c20 2766   [isoscript], 'f
-000295e0: 696c 6573 273a 205f 6669 6c65 732c 2027  iles': _files, '
-000295f0: 6d65 7461 6c5f 7572 6c27 3a20 6d65 7461  metal_url': meta
-00029600: 6c5f 7572 6c2c 2027 6e6f 6e61 6d65 273a  l_url, 'noname':
-00029610: 2054 7275 652c 0a20 2020 2020 2020 2020   True,.         
+000292b0: 6967 6e69 7469 6f6e 5f76 6572 7369 6f6e  ignition_version
+000292c0: 3d69 676e 6974 696f 6e5f 7665 7273 696f  =ignition_versio
+000292d0: 6e29 0a20 2020 2020 2020 2020 2020 2069  n).            i
+000292e0: 6620 6469 7265 6374 3a0a 2020 2020 2020  f direct:.      
+000292f0: 2020 2020 2020 2020 2020 662e 7772 6974            f.writ
+00029300: 6528 6669 6e61 6c64 6174 6129 0a20 2020  e(finaldata).   
+00029310: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+00029320: 2020 2020 2020 2020 2020 2020 2020 205f                 _
+00029330: 6669 6c65 7320 3d20 5b7b 2270 6174 6822  files = [{"path"
+00029340: 3a20 222f 726f 6f74 2f63 6f6e 6669 672e  : "/root/config.
+00029350: 6967 6e22 2c20 2263 6f6e 7465 6e74 223a  ign", "content":
+00029360: 2066 696e 616c 6461 7461 7d5d 0a20 2020   finaldata}].   
+00029370: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00029380: 6f73 2e70 6174 682e 6578 6973 7473 2827  os.path.exists('
+00029390: 6973 6f2e 7368 2729 3a0a 2020 2020 2020  iso.sh'):.      
+000293a0: 2020 2020 2020 2020 2020 2020 2020 7070                pp
+000293b0: 7269 6e74 2822 5573 696e 6720 6c6f 6361  rint("Using loca
+000293c0: 6c20 6973 6f2e 7368 2073 6372 6970 7422  l iso.sh script"
+000293d0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000293e0: 2020 2020 2020 6973 6f73 6372 6970 7420        isoscript 
+000293f0: 3d20 2769 736f 2e73 6827 0a20 2020 2020  = 'iso.sh'.     
+00029400: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00029410: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00029420: 2020 2020 2069 736f 7363 7269 7074 203d       isoscript =
+00029430: 2066 277b 706c 616e 6469 727d 2f69 736f   f'{plandir}/iso
+00029440: 2e73 6827 0a20 2020 2020 2020 2020 2020  .sh'.           
+00029450: 2020 2020 2063 6c75 7374 6572 6469 7220       clusterdir 
+00029460: 3d20 6f73 2e70 6174 682e 6578 7061 6e64  = os.path.expand
+00029470: 7573 6572 2866 227e 2f2e 6b63 6c69 2f63  user(f"~/.kcli/c
+00029480: 6c75 7374 6572 732f 7b63 6c75 7374 6572  lusters/{cluster
+00029490: 7d22 290a 2020 2020 2020 2020 2020 2020  }").            
+000294a0: 2020 2020 6966 206f 732e 7061 7468 2e65      if os.path.e
+000294b0: 7869 7374 7328 6627 7b63 6c75 7374 6572  xists(f'{cluster
+000294c0: 6469 727d 2f6d 6163 732e 7478 7427 2920  dir}/macs.txt') 
+000294d0: 6f72 206f 732e 7061 7468 2e65 7869 7374  or os.path.exist
+000294e0: 7328 276d 6163 732e 7478 7427 293a 0a20  s('macs.txt'):. 
+000294f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029500: 2020 206d 6163 7364 6972 203d 2066 277b     macsdir = f'{
+00029510: 636c 7573 7465 7264 6972 7d27 2069 6620  clusterdir}' if 
+00029520: 6f73 2e70 6174 682e 6578 6973 7473 2863  os.path.exists(c
+00029530: 6c75 7374 6572 6469 7229 2065 6c73 6520  lusterdir) else 
+00029540: 272e 270a 2020 2020 2020 2020 2020 2020  '.'.            
+00029550: 2020 2020 2020 2020 5f66 696c 6573 2e61          _files.a
+00029560: 7070 656e 6428 7b22 7061 7468 223a 2022  ppend({"path": "
+00029570: 2f72 6f6f 742f 6d61 6373 2e74 7874 222c  /root/macs.txt",
+00029580: 2022 6f72 6967 696e 223a 2066 277b 6d61   "origin": f'{ma
+00029590: 6373 6469 727d 2f6d 6163 732e 7478 7427  csdir}/macs.txt'
+000295a0: 7d29 0a20 2020 2020 2020 2020 2020 2020  }).             
+000295b0: 2020 2069 736f 5f6f 7665 7272 6964 6573     iso_overrides
+000295c0: 203d 207b 2773 6372 6970 7473 273a 205b   = {'scripts': [
+000295d0: 6973 6f73 6372 6970 745d 2c20 2766 696c  isoscript], 'fil
+000295e0: 6573 273a 205f 6669 6c65 732c 2027 6d65  es': _files, 'me
+000295f0: 7461 6c5f 7572 6c27 3a20 6d65 7461 6c5f  tal_url': metal_
+00029600: 7572 6c2c 2027 6e6f 6e61 6d65 273a 2054  url, 'noname': T
+00029610: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
 00029620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029630: 2020 2020 2020 2020 2769 6d61 6765 273a          'image':
-00029640: 2027 7268 636f 7334 3030 3027 7d0a 2020   'rhcos4000'}.  
-00029650: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00029660: 206d 6574 616c 5f75 726c 2069 7320 6e6f   metal_url is no
-00029670: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00029680: 2020 2020 2020 2020 2020 2020 6973 6f5f              iso_
-00029690: 6f76 6572 7269 6465 735b 276e 6565 645f  overrides['need_
-000296a0: 6e65 7477 6f72 6b27 5d20 3d20 5472 7565  network'] = True
-000296b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000296c0: 2069 736f 5f6f 7665 7272 6964 6573 2e75   iso_overrides.u
-000296d0: 7064 6174 6528 6f76 6572 7269 6465 7329  pdate(overrides)
-000296e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000296f0: 2069 6620 276e 616d 6527 2069 6e20 6f76   if 'name' in ov
-00029700: 6572 7269 6465 733a 0a20 2020 2020 2020  errides:.       
-00029710: 2020 2020 2020 2020 2020 2020 2069 736f               iso
-00029720: 5f6e 616d 6520 3d20 6f76 6572 7269 6465  _name = override
-00029730: 735b 276e 616d 6527 5d0a 2020 2020 2020  s['name'].      
-00029740: 2020 2020 2020 2020 2020 2020 2020 6973                is
-00029750: 6f5f 6f76 6572 7269 6465 735b 276e 6f6e  o_overrides['non
-00029760: 616d 6527 5d20 3d20 4661 6c73 650a 2020  ame'] = False.  
-00029770: 2020 2020 2020 2020 2020 2020 2020 656c                el
-00029780: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00029790: 2020 2020 2020 2020 6973 6f5f 6e61 6d65          iso_name
-000297a0: 203d 2027 6175 746f 696e 7374 616c 6c65   = 'autoinstalle
-000297b0: 7227 0a20 2020 2020 2020 2020 2020 2020  r'.             
-000297c0: 2020 2072 6573 756c 7420 3d20 7365 6c66     result = self
-000297d0: 2e63 7265 6174 655f 766d 2869 736f 5f6e  .create_vm(iso_n
-000297e0: 616d 652c 206f 7665 7272 6964 6573 3d69  ame, overrides=i
-000297f0: 736f 5f6f 7665 7272 6964 6573 2c20 6f6e  so_overrides, on
-00029800: 6c79 6173 7365 7473 3d54 7275 6529 0a20  lyassets=True). 
-00029810: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00029820: 6620 2772 6561 736f 6e27 2069 6e20 7265  f 'reason' in re
-00029830: 7375 6c74 3a0a 2020 2020 2020 2020 2020  sult:.          
-00029840: 2020 2020 2020 2020 2020 6572 726f 7228            error(
-00029850: 7265 7375 6c74 5b27 7265 6173 6f6e 275d  result['reason']
-00029860: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00029870: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00029880: 2020 2020 2020 2020 2020 2020 662e 7772              f.wr
-00029890: 6974 6528 7265 7375 6c74 5b27 7573 6572  ite(result['user
-000298a0: 6461 7461 275d 290a 2020 2020 2020 2020  data']).        
-000298b0: 6966 2069 736f 3a0a 2020 2020 2020 2020  if iso:.        
-000298c0: 2020 2020 6966 2073 656c 662e 7479 7065      if self.type
-000298d0: 206e 6f74 2069 6e20 5b27 6b76 6d27 2c20   not in ['kvm', 
-000298e0: 2766 616b 6527 2c20 276b 7562 6576 6972  'fake', 'kubevir
-000298f0: 7427 2c20 2776 7370 6865 7265 272c 2027  t', 'vsphere', '
-00029900: 6f70 656e 7374 6163 6b27 5d3a 0a20 2020  openstack']:.   
-00029910: 2020 2020 2020 2020 2020 2020 2077 6172               war
-00029920: 6e69 6e67 2866 2249 736f 2067 656e 6572  ning(f"Iso gener
-00029930: 6174 696f 6e20 6e6f 7420 7375 7070 6f72  ation not suppor
-00029940: 7465 6420 6f6e 207b 7365 6c66 2e74 7970  ted on {self.typ
-00029950: 657d 2229 0a20 2020 2020 2020 2020 2020  e}").           
-00029960: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00029970: 2020 2020 2020 2069 736f 5f70 6f6f 6c20         iso_pool 
-00029980: 3d20 6f76 6572 7269 6465 732e 6765 7428  = overrides.get(
-00029990: 2770 6f6f 6c27 2920 6f72 2073 656c 662e  'pool') or self.
-000299a0: 706f 6f6c 0a20 2020 2020 2020 2020 2020  pool.           
-000299b0: 2020 2020 2067 656e 6572 6174 655f 7268       generate_rh
-000299c0: 636f 735f 6973 6f28 7365 6c66 2e6b 2c20  cos_iso(self.k, 
-000299d0: 6622 7b63 6c75 7374 6572 7d2d 7b72 6f6c  f"{cluster}-{rol
-000299e0: 657d 222c 2069 736f 5f70 6f6f 6c2c 2076  e}", iso_pool, v
-000299f0: 6572 7369 6f6e 3d69 736f 5f76 6572 7369  ersion=iso_versi
-00029a00: 6f6e 2c20 696e 7374 616c 6c65 723d 696e  on, installer=in
-00029a10: 7374 616c 6c65 7229 0a0a 2020 2020 6465  staller)..    de
-00029a20: 6620 6372 6561 7465 5f6f 7065 6e73 6869  f create_openshi
-00029a30: 6674 5f64 6973 636f 6e6e 6563 7465 6428  ft_disconnected(
-00029a40: 7365 6c66 2c20 706c 616e 2c20 6f76 6572  self, plan, over
-00029a50: 7269 6465 733d 7b7d 293a 0a20 2020 2020  rides={}):.     
-00029a60: 2020 2064 6174 6120 3d20 6f76 6572 7269     data = overri
-00029a70: 6465 730a 2020 2020 2020 2020 706c 616e  des.        plan
-00029a80: 6469 7220 3d20 6f73 2e70 6174 682e 6469  dir = os.path.di
-00029a90: 726e 616d 6528 6f70 656e 7368 6966 742e  rname(openshift.
-00029aa0: 6372 6561 7465 2e5f 5f63 6f64 655f 5f2e  create.__code__.
-00029ab0: 636f 5f66 696c 656e 616d 6529 0a20 2020  co_filename).   
-00029ac0: 2020 2020 2063 6c75 7374 6572 203d 2064       cluster = d
-00029ad0: 6174 612e 6765 7428 2763 6c75 7374 6572  ata.get('cluster
-00029ae0: 272c 2027 6d79 6f70 656e 7368 6966 7427  ', 'myopenshift'
-00029af0: 290a 2020 2020 2020 2020 7570 7374 7265  ).        upstre
-00029b00: 616d 203d 2064 6174 612e 6765 7428 2775  am = data.get('u
-00029b10: 7073 7472 6561 6d27 2c20 4661 6c73 6529  pstream', False)
-00029b20: 0a20 2020 2020 2020 2076 6572 7369 6f6e  .        version
-00029b30: 203d 2064 6174 612e 6765 7428 2776 6572   = data.get('ver
-00029b40: 7369 6f6e 272c 2027 7374 6162 6c65 2729  sion', 'stable')
-00029b50: 0a20 2020 2020 2020 2074 6167 203d 2064  .        tag = d
-00029b60: 6174 612e 6765 7428 2774 6167 272c 204f  ata.get('tag', O
-00029b70: 5045 4e53 4849 4654 5f54 4147 290a 2020  PENSHIFT_TAG).  
-00029b80: 2020 2020 2020 7070 7269 6e74 2866 2255        pprint(f"U
-00029b90: 7369 6e67 2076 6572 7369 6f6e 207b 7665  sing version {ve
-00029ba0: 7273 696f 6e7d 2061 6e64 2074 6167 207b  rsion} and tag {
-00029bb0: 7461 677d 2229 0a20 2020 2020 2020 2064  tag}").        d
-00029bc0: 6973 636f 6e6e 6563 7465 645f 766d 203d  isconnected_vm =
-00029bd0: 2066 227b 636c 7573 7465 727d 2d64 6973   f"{cluster}-dis
-00029be0: 636f 6e6e 6563 7465 6422 0a20 2020 2020  connected".     
-00029bf0: 2020 2064 6973 636f 6e6e 6563 7465 645f     disconnected_
-00029c00: 7265 7573 6520 3d20 6461 7461 2e67 6574  reuse = data.get
-00029c10: 2827 6469 7363 6f6e 6e65 6374 6564 5f72  ('disconnected_r
-00029c20: 6575 7365 272c 2046 616c 7365 290a 2020  euse', False).  
-00029c30: 2020 2020 2020 6469 7363 6f6e 6e65 6374        disconnect
-00029c40: 6564 5f73 796e 6320 3d20 6461 7461 2e67  ed_sync = data.g
-00029c50: 6574 2827 6469 7363 6f6e 6e65 6374 6564  et('disconnected
-00029c60: 5f73 796e 6327 2c20 5472 7565 290a 2020  _sync', True).  
-00029c70: 2020 2020 2020 7070 7269 6e74 2866 2244        pprint(f"D
-00029c80: 6570 6c6f 7969 6e67 2064 6973 636f 6e6e  eploying disconn
-00029c90: 6563 7465 6420 766d 207b 6469 7363 6f6e  ected vm {discon
-00029ca0: 6e65 6374 6564 5f76 6d7d 2229 0a20 2020  nected_vm}").   
-00029cb0: 2020 2020 2069 6620 6469 7363 6f6e 6e65       if disconne
-00029cc0: 6374 6564 5f73 796e 633a 0a20 2020 2020  cted_sync:.     
-00029cd0: 2020 2020 2020 2070 756c 6c5f 7365 6372         pull_secr
-00029ce0: 6574 203d 2070 7764 5f70 6174 6828 6461  et = pwd_path(da
-00029cf0: 7461 2e67 6574 2827 7075 6c6c 5f73 6563  ta.get('pull_sec
-00029d00: 7265 7427 2929 2069 6620 6e6f 7420 7570  ret')) if not up
-00029d10: 7374 7265 616d 2065 6c73 6520 6622 7b70  stream else f"{p
-00029d20: 6c61 6e64 6972 7d2f 6661 6b65 5f70 756c  landir}/fake_pul
-00029d30: 6c2e 6a73 6f6e 220a 2020 2020 2020 2020  l.json".        
-00029d40: 2020 2020 6966 206e 6f74 2075 7073 7472      if not upstr
-00029d50: 6561 6d3a 0a20 2020 2020 2020 2020 2020  eam:.           
-00029d60: 2020 2020 2070 756c 6c5f 7365 6372 6574       pull_secret
-00029d70: 203d 2070 7764 5f70 6174 6828 6461 7461   = pwd_path(data
-00029d80: 2e67 6574 2827 7075 6c6c 5f73 6563 7265  .get('pull_secre
-00029d90: 7427 2c20 276f 7065 6e73 6869 6674 5f70  t', 'openshift_p
-00029da0: 756c 6c2e 6a73 6f6e 2729 290a 2020 2020  ull.json')).    
-00029db0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00029dc0: 2020 2020 2020 2020 2020 2020 2020 7075                pu
-00029dd0: 6c6c 5f73 6563 7265 7420 3d20 6622 7b70  ll_secret = f"{p
-00029de0: 6c61 6e64 6972 7d2f 6661 6b65 5f70 756c  landir}/fake_pul
-00029df0: 6c2e 6a73 6f6e 220a 2020 2020 2020 2020  l.json".        
-00029e00: 2020 2020 6966 206e 6f74 206f 732e 7061      if not os.pa
-00029e10: 7468 2e65 7869 7374 7328 7075 6c6c 5f73  th.exists(pull_s
-00029e20: 6563 7265 7429 3a0a 2020 2020 2020 2020  ecret):.        
-00029e30: 2020 2020 2020 2020 6572 726f 7228 6622          error(f"
-00029e40: 4d69 7373 696e 6720 7075 6c6c 2073 6563  Missing pull sec
-00029e50: 7265 7420 6669 6c65 207b 7075 6c6c 5f73  ret file {pull_s
-00029e60: 6563 7265 747d 2229 0a20 2020 2020 2020  ecret}").       
-00029e70: 2020 2020 2020 2020 2073 7973 2e65 7869           sys.exi
-00029e80: 7428 3129 0a20 2020 2020 2020 2020 2020  t(1).           
-00029e90: 2064 6174 615b 2770 756c 6c5f 7365 6372   data['pull_secr
-00029ea0: 6574 275d 203d 2072 652e 7375 6228 7222  et'] = re.sub(r"
-00029eb0: 5c73 222c 2022 222c 206f 7065 6e28 7075  \s", "", open(pu
-00029ec0: 6c6c 5f73 6563 7265 7429 2e72 6561 6428  ll_secret).read(
-00029ed0: 2929 0a20 2020 2020 2020 2064 6973 636f  )).        disco
-00029ee0: 6e6e 6563 7465 645f 706c 616e 203d 2066  nnected_plan = f
-00029ef0: 227b 706c 616e 7d2d 7265 7573 6522 2069  "{plan}-reuse" i
-00029f00: 6620 6469 7363 6f6e 6e65 6374 6564 5f72  f disconnected_r
-00029f10: 6575 7365 2065 6c73 6520 706c 616e 0a20  euse else plan. 
-00029f20: 2020 2020 2020 2069 6620 7665 7273 696f         if versio
-00029f30: 6e20 3d3d 2027 6369 2720 616e 6420 2764  n == 'ci' and 'd
-00029f40: 6973 636f 6e6e 6563 7465 645f 6f72 6967  isconnected_orig
-00029f50: 696e 2720 6e6f 7420 696e 206f 7665 7272  in' not in overr
-00029f60: 6964 6573 3a0a 2020 2020 2020 2020 2020  ides:.          
-00029f70: 2020 7265 6720 3d20 2772 6567 6973 7472    reg = 'registr
-00029f80: 792e 6275 696c 6430 312e 6369 2e6f 7065  y.build01.ci.ope
-00029f90: 6e73 6869 6674 2e6f 7267 2720 6966 2073  nshift.org' if s
-00029fa0: 7472 2874 6167 292e 7374 6172 7473 7769  tr(tag).startswi
-00029fb0: 7468 2827 6369 2d27 2920 656c 7365 2027  th('ci-') else '
-00029fc0: 7265 6769 7374 7279 2e63 692e 6f70 656e  registry.ci.open
-00029fd0: 7368 6966 742e 6f72 6727 0a20 2020 2020  shift.org'.     
-00029fe0: 2020 2020 2020 2077 6172 6e69 6e67 2866         warning(f
-00029ff0: 2246 6f72 6369 6e67 2064 6973 636f 6e6e  "Forcing disconn
-0002a000: 6563 7465 645f 6f72 6967 696e 2074 6f20  ected_origin to 
-0002a010: 7b72 6567 7d22 290a 2020 2020 2020 2020  {reg}").        
-0002a020: 2020 2020 6461 7461 5b27 6469 7363 6f6e      data['discon
-0002a030: 6e65 6374 6564 5f6f 7269 6769 6e27 5d20  nected_origin'] 
-0002a040: 3d20 7265 670a 2020 2020 2020 2020 7265  = reg.        re
-0002a050: 7375 6c74 203d 2073 656c 662e 706c 616e  sult = self.plan
-0002a060: 2864 6973 636f 6e6e 6563 7465 645f 706c  (disconnected_pl
-0002a070: 616e 2c20 696e 7075 7466 696c 653d 6627  an, inputfile=f'
-0002a080: 7b70 6c61 6e64 6972 7d2f 6469 7363 6f6e  {plandir}/discon
-0002a090: 6e65 6374 6564 2e79 6d6c 272c 206f 7665  nected.yml', ove
-0002a0a0: 7272 6964 6573 3d64 6174 6129 0a20 2020  rrides=data).   
-0002a0b0: 2020 2020 2069 6620 7265 7375 6c74 5b27       if result['
-0002a0c0: 7265 7375 6c74 275d 2021 3d20 2773 7563  result'] != 'suc
-0002a0d0: 6365 7373 273a 0a20 2020 2020 2020 2020  cess':.         
-0002a0e0: 2020 2073 7973 2e65 7869 7428 3129 0a20     sys.exit(1). 
-0002a0f0: 2020 2020 2020 206e 616d 6520 3d20 6461         name = da
-0002a100: 7461 2e67 6574 2827 6469 7363 6f6e 6e65  ta.get('disconne
-0002a110: 6374 6564 5f72 6575 7365 5f6e 616d 6527  cted_reuse_name'
-0002a120: 2920 6f72 2063 6c75 7374 6572 0a20 2020  ) or cluster.   
-0002a130: 2020 2020 2069 702c 2076 6d70 6f72 7420       ip, vmport 
-0002a140: 3d20 5f73 7368 5f63 7265 6465 6e74 6961  = _ssh_credentia
-0002a150: 6c73 2873 656c 662e 6b2c 2066 277b 6e61  ls(self.k, f'{na
-0002a160: 6d65 7d2d 6469 7363 6f6e 6e65 6374 6564  me}-disconnected
-0002a170: 2729 5b31 3a5d 0a20 2020 2020 2020 2069  ')[1:].        i
-0002a180: 6620 6469 7363 6f6e 6e65 6374 6564 5f73  f disconnected_s
-0002a190: 796e 633a 0a20 2020 2020 2020 2020 2020  ync:.           
-0002a1a0: 2070 7072 696e 7428 2255 7365 2074 6865   pprint("Use the
-0002a1b0: 2066 6f6c 6c6f 7769 6e67 204f 5045 4e53   following OPENS
-0002a1c0: 4849 4654 5f49 4e53 5441 4c4c 5f52 454c  HIFT_INSTALL_REL
-0002a1d0: 4541 5345 5f49 4d41 4745 5f4f 5645 5252  EASE_IMAGE_OVERR
-0002a1e0: 4944 4522 290a 2020 2020 2020 2020 2020  IDE").          
-0002a1f0: 2020 636d 6420 3d20 2263 6174 202f 726f    cmd = "cat /ro
-0002a200: 6f74 2f76 6572 7369 6f6e 2e74 7874 220a  ot/version.txt".
-0002a210: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0002a220: 2020 2020 2020 2020 2020 7070 7269 6e74            pprint
-0002a230: 2822 5573 6520 7468 6520 666f 6c6c 6f77  ("Use the follow
-0002a240: 696e 6720 6469 7363 6f6e 6e65 6374 6564  ing disconnected
-0002a250: 5f75 726c 2229 0a20 2020 2020 2020 2020  _url").         
-0002a260: 2020 2063 6d64 203d 2022 6361 7420 2f72     cmd = "cat /r
-0002a270: 6f6f 742f 7572 6c2e 7478 7422 0a20 2020  oot/url.txt".   
-0002a280: 2020 2020 2073 7368 636d 6420 3d20 7373       sshcmd = ss
-0002a290: 6828 6e61 6d65 2c20 6970 3d69 702c 2075  h(name, ip=ip, u
-0002a2a0: 7365 723d 2772 6f6f 7427 2c20 7475 6e6e  ser='root', tunn
-0002a2b0: 656c 3d73 656c 662e 7475 6e6e 656c 2c20  el=self.tunnel, 
-0002a2c0: 7475 6e6e 656c 686f 7374 3d73 656c 662e  tunnelhost=self.
-0002a2d0: 7475 6e6e 656c 686f 7374 2c0a 2020 2020  tunnelhost,.    
-0002a2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a2f0: 2074 756e 6e65 6c70 6f72 743d 7365 6c66   tunnelport=self
-0002a300: 2e74 756e 6e65 6c70 6f72 742c 2074 756e  .tunnelport, tun
-0002a310: 6e65 6c75 7365 723d 7365 6c66 2e74 756e  neluser=self.tun
-0002a320: 6e65 6c75 7365 722c 2069 6e73 6563 7572  neluser, insecur
-0002a330: 653d 5472 7565 2c20 636d 643d 636d 642c  e=True, cmd=cmd,
-0002a340: 2076 6d70 6f72 743d 766d 706f 7274 290a   vmport=vmport).
-0002a350: 2020 2020 2020 2020 6f73 2e73 7973 7465          os.syste
-0002a360: 6d28 7373 6863 6d64 290a 0a20 2020 2064  m(sshcmd)..    d
-0002a370: 6566 2068 616e 646c 655f 6669 6e69 7368  ef handle_finish
-0002a380: 6669 6c65 7328 7365 6c66 2c20 6e61 6d65  files(self, name
-0002a390: 2c20 6669 6e69 7368 6669 6c65 732c 2069  , finishfiles, i
-0002a3a0: 6465 6e74 6974 7966 696c 653d 4e6f 6e65  dentityfile=None
-0002a3b0: 2c20 766d 636c 6965 6e74 3d4e 6f6e 6529  , vmclient=None)
-0002a3c0: 3a0a 2020 2020 2020 2020 636f 6e66 6967  :.        config
-0002a3d0: 203d 204b 636f 6e66 6967 2863 6c69 656e   = Kconfig(clien
-0002a3e0: 743d 766d 636c 6965 6e74 2920 6966 2076  t=vmclient) if v
-0002a3f0: 6d63 6c69 656e 7420 6973 206e 6f74 204e  mclient is not N
-0002a400: 6f6e 6520 656c 7365 2073 656c 660a 2020  one else self.  
-0002a410: 2020 2020 2020 6b20 3d20 636f 6e66 6967        k = config
-0002a420: 2e6b 0a20 2020 2020 2020 2063 7572 7265  .k.        curre
-0002a430: 6e74 5f69 7020 3d20 636f 6d6d 6f6e 2e5f  nt_ip = common._
-0002a440: 7373 685f 6372 6564 656e 7469 616c 7328  ssh_credentials(
-0002a450: 6b2c 206e 616d 6529 5b31 5d0a 2020 2020  k, name)[1].    
-0002a460: 2020 2020 666f 7220 6669 6e69 7368 6669      for finishfi
-0002a470: 6c65 2069 6e20 6669 6e69 7368 6669 6c65  le in finishfile
-0002a480: 733a 0a20 2020 2020 2020 2020 2020 2069  s:.            i
-0002a490: 6620 6973 696e 7374 616e 6365 2866 696e  f isinstance(fin
-0002a4a0: 6973 6866 696c 652c 2073 7472 293a 0a20  ishfile, str):. 
-0002a4b0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-0002a4c0: 6573 7469 6e61 7469 6f6e 203d 2027 2e27  estination = '.'
-0002a4d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002a4e0: 2073 6f75 7263 6520 3d20 6669 6e69 7368   source = finish
-0002a4f0: 6669 6c65 2069 6620 272f 2720 696e 2066  file if '/' in f
-0002a500: 696e 6973 6866 696c 6520 656c 7365 2066  inishfile else f
-0002a510: 272f 726f 6f74 2f7b 6669 6e69 7368 6669  '/root/{finishfi
-0002a520: 6c65 7d27 0a20 2020 2020 2020 2020 2020  le}'.           
-0002a530: 2065 6c69 6620 6973 696e 7374 616e 6365   elif isinstance
-0002a540: 2866 696e 6973 6866 696c 652c 2064 6963  (finishfile, dic
-0002a550: 7429 2061 6e64 2027 6f72 6967 696e 2720  t) and 'origin' 
-0002a560: 696e 2066 696e 6973 6866 696c 6520 616e  in finishfile an
-0002a570: 6420 2770 6174 6827 2069 6e20 6669 6e69  d 'path' in fini
-0002a580: 7368 6669 6c65 3a0a 2020 2020 2020 2020  shfile:.        
-0002a590: 2020 2020 2020 2020 736f 7572 6365 2c20          source, 
-0002a5a0: 6465 7374 696e 6174 696f 6e20 3d20 6669  destination = fi
-0002a5b0: 6e69 7368 6669 6c65 2e67 6574 2827 6f72  nishfile.get('or
-0002a5c0: 6967 696e 2729 2c20 6f73 2e70 6174 682e  igin'), os.path.
-0002a5d0: 6578 7061 6e64 7573 6572 2866 696e 6973  expanduser(finis
-0002a5e0: 6866 696c 652e 6765 7428 2770 6174 6827  hfile.get('path'
-0002a5f0: 2c20 272e 2729 290a 2020 2020 2020 2020  , '.')).        
-0002a600: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0002a610: 2020 2020 2020 2020 2020 7761 726e 696e            warnin
-0002a620: 6728 6622 496e 636f 7272 6563 7420 6669  g(f"Incorrect fi
-0002a630: 6e69 7368 6669 6c65 2065 6e74 7279 207b  nishfile entry {
-0002a640: 6669 6e69 7368 6669 6c65 7d2e 2053 6b69  finishfile}. Ski
-0002a650: 7070 696e 6722 290a 2020 2020 2020 2020  pping").        
-0002a660: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
-0002a670: 0a20 2020 2020 2020 2020 2020 2073 6370  .            scp
-0002a680: 636d 6420 3d20 636f 6d6d 6f6e 2e73 6370  cmd = common.scp
-0002a690: 286e 616d 652c 2069 703d 6375 7272 656e  (name, ip=curren
-0002a6a0: 745f 6970 2c20 7573 6572 3d27 726f 6f74  t_ip, user='root
-0002a6b0: 272c 2073 6f75 7263 653d 736f 7572 6365  ', source=source
-0002a6c0: 2c20 6465 7374 696e 6174 696f 6e3d 6465  , destination=de
-0002a6d0: 7374 696e 6174 696f 6e2c 0a20 2020 2020  stination,.     
+00029630: 2020 2020 2020 2769 6d61 6765 273a 2027        'image': '
+00029640: 7268 636f 7334 3030 3027 7d0a 2020 2020  rhcos4000'}.    
+00029650: 2020 2020 2020 2020 2020 2020 6966 206d              if m
+00029660: 6574 616c 5f75 726c 2069 7320 6e6f 7420  etal_url is not 
+00029670: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00029680: 2020 2020 2020 2020 2020 6973 6f5f 6f76            iso_ov
+00029690: 6572 7269 6465 735b 276e 6565 645f 6e65  errides['need_ne
+000296a0: 7477 6f72 6b27 5d20 3d20 5472 7565 0a20  twork'] = True. 
+000296b0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000296c0: 736f 5f6f 7665 7272 6964 6573 2e75 7064  so_overrides.upd
+000296d0: 6174 6528 6f76 6572 7269 6465 7329 0a20  ate(overrides). 
+000296e0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000296f0: 6620 276e 616d 6527 2069 6e20 6f76 6572  f 'name' in over
+00029700: 7269 6465 733a 0a20 2020 2020 2020 2020  rides:.         
+00029710: 2020 2020 2020 2020 2020 2069 736f 5f6e             iso_n
+00029720: 616d 6520 3d20 6f76 6572 7269 6465 735b  ame = overrides[
+00029730: 276e 616d 6527 5d0a 2020 2020 2020 2020  'name'].        
+00029740: 2020 2020 2020 2020 2020 2020 6973 6f5f              iso_
+00029750: 6f76 6572 7269 6465 735b 276e 6f6e 616d  overrides['nonam
+00029760: 6527 5d20 3d20 4661 6c73 650a 2020 2020  e'] = False.    
+00029770: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00029780: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00029790: 2020 2020 2020 6973 6f5f 6e61 6d65 203d        iso_name =
+000297a0: 2027 6175 746f 696e 7374 616c 6c65 7227   'autoinstaller'
+000297b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000297c0: 2072 6573 756c 7420 3d20 7365 6c66 2e63   result = self.c
+000297d0: 7265 6174 655f 766d 2869 736f 5f6e 616d  reate_vm(iso_nam
+000297e0: 652c 206f 7665 7272 6964 6573 3d69 736f  e, overrides=iso
+000297f0: 5f6f 7665 7272 6964 6573 2c20 6f6e 6c79  _overrides, only
+00029800: 6173 7365 7473 3d54 7275 6529 0a20 2020  assets=True).   
+00029810: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00029820: 2772 6561 736f 6e27 2069 6e20 7265 7375  'reason' in resu
+00029830: 6c74 3a0a 2020 2020 2020 2020 2020 2020  lt:.            
+00029840: 2020 2020 2020 2020 6572 726f 7228 7265          error(re
+00029850: 7375 6c74 5b27 7265 6173 6f6e 275d 290a  sult['reason']).
+00029860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029870: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00029880: 2020 2020 2020 2020 2020 662e 7772 6974            f.writ
+00029890: 6528 7265 7375 6c74 5b27 7573 6572 6461  e(result['userda
+000298a0: 7461 275d 290a 2020 2020 2020 2020 6966  ta']).        if
+000298b0: 2069 736f 3a0a 2020 2020 2020 2020 2020   iso:.          
+000298c0: 2020 6966 2073 656c 662e 7479 7065 206e    if self.type n
+000298d0: 6f74 2069 6e20 5b27 6b76 6d27 2c20 2766  ot in ['kvm', 'f
+000298e0: 616b 6527 2c20 276b 7562 6576 6972 7427  ake', 'kubevirt'
+000298f0: 2c20 2776 7370 6865 7265 272c 2027 6f70  , 'vsphere', 'op
+00029900: 656e 7374 6163 6b27 5d3a 0a20 2020 2020  enstack']:.     
+00029910: 2020 2020 2020 2020 2020 2077 6172 6e69             warni
+00029920: 6e67 2866 2249 736f 2067 656e 6572 6174  ng(f"Iso generat
+00029930: 696f 6e20 6e6f 7420 7375 7070 6f72 7465  ion not supporte
+00029940: 6420 6f6e 207b 7365 6c66 2e74 7970 657d  d on {self.type}
+00029950: 2229 0a20 2020 2020 2020 2020 2020 2065  ").            e
+00029960: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00029970: 2020 2020 2069 736f 5f70 6f6f 6c20 3d20       iso_pool = 
+00029980: 6f76 6572 7269 6465 732e 6765 7428 2770  overrides.get('p
+00029990: 6f6f 6c27 2920 6f72 2073 656c 662e 706f  ool') or self.po
+000299a0: 6f6c 0a20 2020 2020 2020 2020 2020 2020  ol.             
+000299b0: 2020 2067 656e 6572 6174 655f 7268 636f     generate_rhco
+000299c0: 735f 6973 6f28 7365 6c66 2e6b 2c20 6622  s_iso(self.k, f"
+000299d0: 7b63 6c75 7374 6572 7d2d 7b72 6f6c 657d  {cluster}-{role}
+000299e0: 222c 2069 736f 5f70 6f6f 6c2c 2076 6572  ", iso_pool, ver
+000299f0: 7369 6f6e 3d69 736f 5f76 6572 7369 6f6e  sion=iso_version
+00029a00: 2c20 696e 7374 616c 6c65 723d 696e 7374  , installer=inst
+00029a10: 616c 6c65 7229 0a0a 2020 2020 6465 6620  aller)..    def 
+00029a20: 6372 6561 7465 5f6f 7065 6e73 6869 6674  create_openshift
+00029a30: 5f64 6973 636f 6e6e 6563 7465 6428 7365  _disconnected(se
+00029a40: 6c66 2c20 706c 616e 2c20 6f76 6572 7269  lf, plan, overri
+00029a50: 6465 733d 7b7d 293a 0a20 2020 2020 2020  des={}):.       
+00029a60: 2064 6174 6120 3d20 6f76 6572 7269 6465   data = override
+00029a70: 730a 2020 2020 2020 2020 706c 616e 6469  s.        plandi
+00029a80: 7220 3d20 6f73 2e70 6174 682e 6469 726e  r = os.path.dirn
+00029a90: 616d 6528 6f70 656e 7368 6966 742e 6372  ame(openshift.cr
+00029aa0: 6561 7465 2e5f 5f63 6f64 655f 5f2e 636f  eate.__code__.co
+00029ab0: 5f66 696c 656e 616d 6529 0a20 2020 2020  _filename).     
+00029ac0: 2020 2063 6c75 7374 6572 203d 2064 6174     cluster = dat
+00029ad0: 612e 6765 7428 2763 6c75 7374 6572 272c  a.get('cluster',
+00029ae0: 2027 6d79 6f70 656e 7368 6966 7427 290a   'myopenshift').
+00029af0: 2020 2020 2020 2020 7570 7374 7265 616d          upstream
+00029b00: 203d 2064 6174 612e 6765 7428 2775 7073   = data.get('ups
+00029b10: 7472 6561 6d27 2c20 4661 6c73 6529 0a20  tream', False). 
+00029b20: 2020 2020 2020 2076 6572 7369 6f6e 203d         version =
+00029b30: 2064 6174 612e 6765 7428 2776 6572 7369   data.get('versi
+00029b40: 6f6e 272c 2027 7374 6162 6c65 2729 0a20  on', 'stable'). 
+00029b50: 2020 2020 2020 2074 6167 203d 2064 6174         tag = dat
+00029b60: 612e 6765 7428 2774 6167 272c 204f 5045  a.get('tag', OPE
+00029b70: 4e53 4849 4654 5f54 4147 290a 2020 2020  NSHIFT_TAG).    
+00029b80: 2020 2020 7070 7269 6e74 2866 2255 7369      pprint(f"Usi
+00029b90: 6e67 2076 6572 7369 6f6e 207b 7665 7273  ng version {vers
+00029ba0: 696f 6e7d 2061 6e64 2074 6167 207b 7461  ion} and tag {ta
+00029bb0: 677d 2229 0a20 2020 2020 2020 2064 6973  g}").        dis
+00029bc0: 636f 6e6e 6563 7465 645f 766d 203d 2066  connected_vm = f
+00029bd0: 227b 636c 7573 7465 727d 2d64 6973 636f  "{cluster}-disco
+00029be0: 6e6e 6563 7465 6422 0a20 2020 2020 2020  nnected".       
+00029bf0: 2064 6973 636f 6e6e 6563 7465 645f 7265   disconnected_re
+00029c00: 7573 6520 3d20 6461 7461 2e67 6574 2827  use = data.get('
+00029c10: 6469 7363 6f6e 6e65 6374 6564 5f72 6575  disconnected_reu
+00029c20: 7365 272c 2046 616c 7365 290a 2020 2020  se', False).    
+00029c30: 2020 2020 6469 7363 6f6e 6e65 6374 6564      disconnected
+00029c40: 5f73 796e 6320 3d20 6461 7461 2e67 6574  _sync = data.get
+00029c50: 2827 6469 7363 6f6e 6e65 6374 6564 5f73  ('disconnected_s
+00029c60: 796e 6327 2c20 5472 7565 290a 2020 2020  ync', True).    
+00029c70: 2020 2020 7070 7269 6e74 2866 2244 6570      pprint(f"Dep
+00029c80: 6c6f 7969 6e67 2064 6973 636f 6e6e 6563  loying disconnec
+00029c90: 7465 6420 766d 207b 6469 7363 6f6e 6e65  ted vm {disconne
+00029ca0: 6374 6564 5f76 6d7d 2229 0a20 2020 2020  cted_vm}").     
+00029cb0: 2020 2069 6620 6469 7363 6f6e 6e65 6374     if disconnect
+00029cc0: 6564 5f73 796e 633a 0a20 2020 2020 2020  ed_sync:.       
+00029cd0: 2020 2020 2070 756c 6c5f 7365 6372 6574       pull_secret
+00029ce0: 203d 2070 7764 5f70 6174 6828 6461 7461   = pwd_path(data
+00029cf0: 2e67 6574 2827 7075 6c6c 5f73 6563 7265  .get('pull_secre
+00029d00: 7427 2929 2069 6620 6e6f 7420 7570 7374  t')) if not upst
+00029d10: 7265 616d 2065 6c73 6520 6622 7b70 6c61  ream else f"{pla
+00029d20: 6e64 6972 7d2f 6661 6b65 5f70 756c 6c2e  ndir}/fake_pull.
+00029d30: 6a73 6f6e 220a 2020 2020 2020 2020 2020  json".          
+00029d40: 2020 6966 206e 6f74 2075 7073 7472 6561    if not upstrea
+00029d50: 6d3a 0a20 2020 2020 2020 2020 2020 2020  m:.             
+00029d60: 2020 2070 756c 6c5f 7365 6372 6574 203d     pull_secret =
+00029d70: 2070 7764 5f70 6174 6828 6461 7461 2e67   pwd_path(data.g
+00029d80: 6574 2827 7075 6c6c 5f73 6563 7265 7427  et('pull_secret'
+00029d90: 2c20 276f 7065 6e73 6869 6674 5f70 756c  , 'openshift_pul
+00029da0: 6c2e 6a73 6f6e 2729 290a 2020 2020 2020  l.json')).      
+00029db0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00029dc0: 2020 2020 2020 2020 2020 2020 7075 6c6c              pull
+00029dd0: 5f73 6563 7265 7420 3d20 6622 7b70 6c61  _secret = f"{pla
+00029de0: 6e64 6972 7d2f 6661 6b65 5f70 756c 6c2e  ndir}/fake_pull.
+00029df0: 6a73 6f6e 220a 2020 2020 2020 2020 2020  json".          
+00029e00: 2020 6966 206e 6f74 206f 732e 7061 7468    if not os.path
+00029e10: 2e65 7869 7374 7328 7075 6c6c 5f73 6563  .exists(pull_sec
+00029e20: 7265 7429 3a0a 2020 2020 2020 2020 2020  ret):.          
+00029e30: 2020 2020 2020 6572 726f 7228 6622 4d69        error(f"Mi
+00029e40: 7373 696e 6720 7075 6c6c 2073 6563 7265  ssing pull secre
+00029e50: 7420 6669 6c65 207b 7075 6c6c 5f73 6563  t file {pull_sec
+00029e60: 7265 747d 2229 0a20 2020 2020 2020 2020  ret}").         
+00029e70: 2020 2020 2020 2073 7973 2e65 7869 7428         sys.exit(
+00029e80: 3129 0a20 2020 2020 2020 2020 2020 2064  1).            d
+00029e90: 6174 615b 2770 756c 6c5f 7365 6372 6574  ata['pull_secret
+00029ea0: 275d 203d 2072 652e 7375 6228 7222 5c73  '] = re.sub(r"\s
+00029eb0: 222c 2022 222c 206f 7065 6e28 7075 6c6c  ", "", open(pull
+00029ec0: 5f73 6563 7265 7429 2e72 6561 6428 2929  _secret).read())
+00029ed0: 0a20 2020 2020 2020 2064 6973 636f 6e6e  .        disconn
+00029ee0: 6563 7465 645f 706c 616e 203d 2066 227b  ected_plan = f"{
+00029ef0: 706c 616e 7d2d 7265 7573 6522 2069 6620  plan}-reuse" if 
+00029f00: 6469 7363 6f6e 6e65 6374 6564 5f72 6575  disconnected_reu
+00029f10: 7365 2065 6c73 6520 706c 616e 0a20 2020  se else plan.   
+00029f20: 2020 2020 2069 6620 7665 7273 696f 6e20       if version 
+00029f30: 3d3d 2027 6369 2720 616e 6420 2764 6973  == 'ci' and 'dis
+00029f40: 636f 6e6e 6563 7465 645f 6f72 6967 696e  connected_origin
+00029f50: 2720 6e6f 7420 696e 206f 7665 7272 6964  ' not in overrid
+00029f60: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
+00029f70: 7265 6720 3d20 2772 6567 6973 7472 792e  reg = 'registry.
+00029f80: 6275 696c 6430 312e 6369 2e6f 7065 6e73  build01.ci.opens
+00029f90: 6869 6674 2e6f 7267 2720 6966 2073 7472  hift.org' if str
+00029fa0: 2874 6167 292e 7374 6172 7473 7769 7468  (tag).startswith
+00029fb0: 2827 6369 2d27 2920 656c 7365 2027 7265  ('ci-') else 're
+00029fc0: 6769 7374 7279 2e63 692e 6f70 656e 7368  gistry.ci.opensh
+00029fd0: 6966 742e 6f72 6727 0a20 2020 2020 2020  ift.org'.       
+00029fe0: 2020 2020 2077 6172 6e69 6e67 2866 2246       warning(f"F
+00029ff0: 6f72 6369 6e67 2064 6973 636f 6e6e 6563  orcing disconnec
+0002a000: 7465 645f 6f72 6967 696e 2074 6f20 7b72  ted_origin to {r
+0002a010: 6567 7d22 290a 2020 2020 2020 2020 2020  eg}").          
+0002a020: 2020 6461 7461 5b27 6469 7363 6f6e 6e65    data['disconne
+0002a030: 6374 6564 5f6f 7269 6769 6e27 5d20 3d20  cted_origin'] = 
+0002a040: 7265 670a 2020 2020 2020 2020 7265 7375  reg.        resu
+0002a050: 6c74 203d 2073 656c 662e 706c 616e 2864  lt = self.plan(d
+0002a060: 6973 636f 6e6e 6563 7465 645f 706c 616e  isconnected_plan
+0002a070: 2c20 696e 7075 7466 696c 653d 6627 7b70  , inputfile=f'{p
+0002a080: 6c61 6e64 6972 7d2f 6469 7363 6f6e 6e65  landir}/disconne
+0002a090: 6374 6564 2e79 6d6c 272c 206f 7665 7272  cted.yml', overr
+0002a0a0: 6964 6573 3d64 6174 6129 0a20 2020 2020  ides=data).     
+0002a0b0: 2020 2069 6620 7265 7375 6c74 5b27 7265     if result['re
+0002a0c0: 7375 6c74 275d 2021 3d20 2773 7563 6365  sult'] != 'succe
+0002a0d0: 7373 273a 0a20 2020 2020 2020 2020 2020  ss':.           
+0002a0e0: 2073 7973 2e65 7869 7428 3129 0a20 2020   sys.exit(1).   
+0002a0f0: 2020 2020 206e 616d 6520 3d20 6461 7461       name = data
+0002a100: 2e67 6574 2827 6469 7363 6f6e 6e65 6374  .get('disconnect
+0002a110: 6564 5f72 6575 7365 5f6e 616d 6527 2920  ed_reuse_name') 
+0002a120: 6f72 2063 6c75 7374 6572 0a20 2020 2020  or cluster.     
+0002a130: 2020 2069 702c 2076 6d70 6f72 7420 3d20     ip, vmport = 
+0002a140: 5f73 7368 5f63 7265 6465 6e74 6961 6c73  _ssh_credentials
+0002a150: 2873 656c 662e 6b2c 2066 277b 6e61 6d65  (self.k, f'{name
+0002a160: 7d2d 6469 7363 6f6e 6e65 6374 6564 2729  }-disconnected')
+0002a170: 5b31 3a5d 0a20 2020 2020 2020 2069 6620  [1:].        if 
+0002a180: 6469 7363 6f6e 6e65 6374 6564 5f73 796e  disconnected_syn
+0002a190: 633a 0a20 2020 2020 2020 2020 2020 2070  c:.            p
+0002a1a0: 7072 696e 7428 2255 7365 2074 6865 2066  print("Use the f
+0002a1b0: 6f6c 6c6f 7769 6e67 204f 5045 4e53 4849  ollowing OPENSHI
+0002a1c0: 4654 5f49 4e53 5441 4c4c 5f52 454c 4541  FT_INSTALL_RELEA
+0002a1d0: 5345 5f49 4d41 4745 5f4f 5645 5252 4944  SE_IMAGE_OVERRID
+0002a1e0: 4522 290a 2020 2020 2020 2020 2020 2020  E").            
+0002a1f0: 636d 6420 3d20 2263 6174 202f 726f 6f74  cmd = "cat /root
+0002a200: 2f76 6572 7369 6f6e 2e74 7874 220a 2020  /version.txt".  
+0002a210: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+0002a220: 2020 2020 2020 2020 7070 7269 6e74 2822          pprint("
+0002a230: 5573 6520 7468 6520 666f 6c6c 6f77 696e  Use the followin
+0002a240: 6720 6469 7363 6f6e 6e65 6374 6564 5f75  g disconnected_u
+0002a250: 726c 2229 0a20 2020 2020 2020 2020 2020  rl").           
+0002a260: 2063 6d64 203d 2022 6361 7420 2f72 6f6f   cmd = "cat /roo
+0002a270: 742f 7572 6c2e 7478 7422 0a20 2020 2020  t/url.txt".     
+0002a280: 2020 2073 7368 636d 6420 3d20 7373 6828     sshcmd = ssh(
+0002a290: 6e61 6d65 2c20 6970 3d69 702c 2075 7365  name, ip=ip, use
+0002a2a0: 723d 2772 6f6f 7427 2c20 7475 6e6e 656c  r='root', tunnel
+0002a2b0: 3d73 656c 662e 7475 6e6e 656c 2c20 7475  =self.tunnel, tu
+0002a2c0: 6e6e 656c 686f 7374 3d73 656c 662e 7475  nnelhost=self.tu
+0002a2d0: 6e6e 656c 686f 7374 2c0a 2020 2020 2020  nnelhost,.      
+0002a2e0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+0002a2f0: 756e 6e65 6c70 6f72 743d 7365 6c66 2e74  unnelport=self.t
+0002a300: 756e 6e65 6c70 6f72 742c 2074 756e 6e65  unnelport, tunne
+0002a310: 6c75 7365 723d 7365 6c66 2e74 756e 6e65  luser=self.tunne
+0002a320: 6c75 7365 722c 2069 6e73 6563 7572 653d  luser, insecure=
+0002a330: 5472 7565 2c20 636d 643d 636d 642c 2076  True, cmd=cmd, v
+0002a340: 6d70 6f72 743d 766d 706f 7274 290a 2020  mport=vmport).  
+0002a350: 2020 2020 2020 6f73 2e73 7973 7465 6d28        os.system(
+0002a360: 7373 6863 6d64 290a 0a20 2020 2064 6566  sshcmd)..    def
+0002a370: 2068 616e 646c 655f 6669 6e69 7368 6669   handle_finishfi
+0002a380: 6c65 7328 7365 6c66 2c20 6e61 6d65 2c20  les(self, name, 
+0002a390: 6669 6e69 7368 6669 6c65 732c 2069 6465  finishfiles, ide
+0002a3a0: 6e74 6974 7966 696c 653d 4e6f 6e65 2c20  ntityfile=None, 
+0002a3b0: 766d 636c 6965 6e74 3d4e 6f6e 6529 3a0a  vmclient=None):.
+0002a3c0: 2020 2020 2020 2020 636f 6e66 6967 203d          config =
+0002a3d0: 204b 636f 6e66 6967 2863 6c69 656e 743d   Kconfig(client=
+0002a3e0: 766d 636c 6965 6e74 2920 6966 2076 6d63  vmclient) if vmc
+0002a3f0: 6c69 656e 7420 6973 206e 6f74 204e 6f6e  lient is not Non
+0002a400: 6520 656c 7365 2073 656c 660a 2020 2020  e else self.    
+0002a410: 2020 2020 6b20 3d20 636f 6e66 6967 2e6b      k = config.k
+0002a420: 0a20 2020 2020 2020 2063 7572 7265 6e74  .        current
+0002a430: 5f69 7020 3d20 636f 6d6d 6f6e 2e5f 7373  _ip = common._ss
+0002a440: 685f 6372 6564 656e 7469 616c 7328 6b2c  h_credentials(k,
+0002a450: 206e 616d 6529 5b31 5d0a 2020 2020 2020   name)[1].      
+0002a460: 2020 666f 7220 6669 6e69 7368 6669 6c65    for finishfile
+0002a470: 2069 6e20 6669 6e69 7368 6669 6c65 733a   in finishfiles:
+0002a480: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0002a490: 6973 696e 7374 616e 6365 2866 696e 6973  isinstance(finis
+0002a4a0: 6866 696c 652c 2073 7472 293a 0a20 2020  hfile, str):.   
+0002a4b0: 2020 2020 2020 2020 2020 2020 2064 6573               des
+0002a4c0: 7469 6e61 7469 6f6e 203d 2027 2e27 0a20  tination = '.'. 
+0002a4d0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0002a4e0: 6f75 7263 6520 3d20 6669 6e69 7368 6669  ource = finishfi
+0002a4f0: 6c65 2069 6620 272f 2720 696e 2066 696e  le if '/' in fin
+0002a500: 6973 6866 696c 6520 656c 7365 2066 272f  ishfile else f'/
+0002a510: 726f 6f74 2f7b 6669 6e69 7368 6669 6c65  root/{finishfile
+0002a520: 7d27 0a20 2020 2020 2020 2020 2020 2065  }'.            e
+0002a530: 6c69 6620 6973 696e 7374 616e 6365 2866  lif isinstance(f
+0002a540: 696e 6973 6866 696c 652c 2064 6963 7429  inishfile, dict)
+0002a550: 2061 6e64 2027 6f72 6967 696e 2720 696e   and 'origin' in
+0002a560: 2066 696e 6973 6866 696c 6520 616e 6420   finishfile and 
+0002a570: 2770 6174 6827 2069 6e20 6669 6e69 7368  'path' in finish
+0002a580: 6669 6c65 3a0a 2020 2020 2020 2020 2020  file:.          
+0002a590: 2020 2020 2020 736f 7572 6365 2c20 6465        source, de
+0002a5a0: 7374 696e 6174 696f 6e20 3d20 6669 6e69  stination = fini
+0002a5b0: 7368 6669 6c65 2e67 6574 2827 6f72 6967  shfile.get('orig
+0002a5c0: 696e 2729 2c20 6f73 2e70 6174 682e 6578  in'), os.path.ex
+0002a5d0: 7061 6e64 7573 6572 2866 696e 6973 6866  panduser(finishf
+0002a5e0: 696c 652e 6765 7428 2770 6174 6827 2c20  ile.get('path', 
+0002a5f0: 272e 2729 290a 2020 2020 2020 2020 2020  '.')).          
+0002a600: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0002a610: 2020 2020 2020 2020 7761 726e 696e 6728          warning(
+0002a620: 6622 496e 636f 7272 6563 7420 6669 6e69  f"Incorrect fini
+0002a630: 7368 6669 6c65 2065 6e74 7279 207b 6669  shfile entry {fi
+0002a640: 6e69 7368 6669 6c65 7d2e 2053 6b69 7070  nishfile}. Skipp
+0002a650: 696e 6722 290a 2020 2020 2020 2020 2020  ing").          
+0002a660: 2020 2020 2020 636f 6e74 696e 7565 0a20        continue. 
+0002a670: 2020 2020 2020 2020 2020 2073 6370 636d             scpcm
+0002a680: 6420 3d20 636f 6d6d 6f6e 2e73 6370 286e  d = common.scp(n
+0002a690: 616d 652c 2069 703d 6375 7272 656e 745f  ame, ip=current_
+0002a6a0: 6970 2c20 7573 6572 3d27 726f 6f74 272c  ip, user='root',
+0002a6b0: 2073 6f75 7263 653d 736f 7572 6365 2c20   source=source, 
+0002a6c0: 6465 7374 696e 6174 696f 6e3d 6465 7374  destination=dest
+0002a6d0: 696e 6174 696f 6e2c 0a20 2020 2020 2020  ination,.       
 0002a6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a6f0: 2020 2020 2020 2020 2020 2074 756e 6e65             tunne
-0002a700: 6c3d 636f 6e66 6967 2e74 756e 6e65 6c2c  l=config.tunnel,
-0002a710: 2074 756e 6e65 6c68 6f73 743d 636f 6e66   tunnelhost=conf
-0002a720: 6967 2e74 756e 6e65 6c68 6f73 742c 2074  ig.tunnelhost, t
-0002a730: 756e 6e65 6c70 6f72 743d 636f 6e66 6967  unnelport=config
-0002a740: 2e74 756e 6e65 6c70 6f72 742c 0a20 2020  .tunnelport,.   
+0002a6f0: 2020 2020 2020 2020 2074 756e 6e65 6c3d           tunnel=
+0002a700: 636f 6e66 6967 2e74 756e 6e65 6c2c 2074  config.tunnel, t
+0002a710: 756e 6e65 6c68 6f73 743d 636f 6e66 6967  unnelhost=config
+0002a720: 2e74 756e 6e65 6c68 6f73 742c 2074 756e  .tunnelhost, tun
+0002a730: 6e65 6c70 6f72 743d 636f 6e66 6967 2e74  nelport=config.t
+0002a740: 756e 6e65 6c70 6f72 742c 0a20 2020 2020  unnelport,.     
 0002a750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a760: 2020 2020 2020 2020 2020 2020 2074 756e               tun
-0002a770: 6e65 6c75 7365 723d 7365 6c66 2e74 756e  neluser=self.tun
-0002a780: 6e65 6c75 7365 722c 2064 6f77 6e6c 6f61  neluser, downloa
-0002a790: 643d 5472 7565 2c20 696e 7365 6375 7265  d=True, insecure
-0002a7a0: 3d54 7275 652c 2069 6465 6e74 6974 7966  =True, identityf
-0002a7b0: 696c 653d 6964 656e 7469 7479 6669 6c65  ile=identityfile
-0002a7c0: 290a 2020 2020 2020 2020 2020 2020 6f73  ).            os
-0002a7d0: 2e73 7973 7465 6d28 7363 7063 6d64 290a  .system(scpcmd).
-0002a7e0: 0a20 2020 2064 6566 2068 616e 646c 655f  .    def handle_
-0002a7f0: 6e6f 7469 6669 6361 7469 6f6e 7328 7365  notifications(se
-0002a800: 6c66 2c20 6e61 6d65 2c20 6e6f 7469 6679  lf, name, notify
-0002a810: 6d65 7468 6f64 733d 5b5d 2c20 7075 7368  methods=[], push
-0002a820: 6275 6c6c 6574 746f 6b65 6e3d 4e6f 6e65  bullettoken=None
-0002a830: 2c20 6e6f 7469 6679 7363 7269 7074 3d4e  , notifyscript=N
-0002a840: 6f6e 652c 206e 6f74 6966 7963 6d64 3d4e  one, notifycmd=N
-0002a850: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
+0002a760: 2020 2020 2020 2020 2020 2074 756e 6e65             tunne
+0002a770: 6c75 7365 723d 7365 6c66 2e74 756e 6e65  luser=self.tunne
+0002a780: 6c75 7365 722c 2064 6f77 6e6c 6f61 643d  luser, download=
+0002a790: 5472 7565 2c20 696e 7365 6375 7265 3d54  True, insecure=T
+0002a7a0: 7275 652c 2069 6465 6e74 6974 7966 696c  rue, identityfil
+0002a7b0: 653d 6964 656e 7469 7479 6669 6c65 290a  e=identityfile).
+0002a7c0: 2020 2020 2020 2020 2020 2020 6f73 2e73              os.s
+0002a7d0: 7973 7465 6d28 7363 7063 6d64 290a 0a20  ystem(scpcmd).. 
+0002a7e0: 2020 2064 6566 2068 616e 646c 655f 6e6f     def handle_no
+0002a7f0: 7469 6669 6361 7469 6f6e 7328 7365 6c66  tifications(self
+0002a800: 2c20 6e61 6d65 2c20 6e6f 7469 6679 6d65  , name, notifyme
+0002a810: 7468 6f64 733d 5b5d 2c20 7075 7368 6275  thods=[], pushbu
+0002a820: 6c6c 6574 746f 6b65 6e3d 4e6f 6e65 2c20  llettoken=None, 
+0002a830: 6e6f 7469 6679 7363 7269 7074 3d4e 6f6e  notifyscript=Non
+0002a840: 652c 206e 6f74 6966 7963 6d64 3d4e 6f6e  e, notifycmd=Non
+0002a850: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
 0002a860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a870: 2020 736c 6163 6b63 6861 6e6e 656c 3d4e    slackchannel=N
-0002a880: 6f6e 652c 2073 6c61 636b 746f 6b65 6e3d  one, slacktoken=
-0002a890: 4e6f 6e65 2c20 6d61 696c 7365 7276 6572  None, mailserver
-0002a8a0: 3d4e 6f6e 652c 206d 6169 6c66 726f 6d3d  =None, mailfrom=
-0002a8b0: 4e6f 6e65 2c20 6d61 696c 746f 3d4e 6f6e  None, mailto=Non
-0002a8c0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-0002a8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a8e0: 636c 7573 7465 723d 4661 6c73 6529 3a0a  cluster=False):.
-0002a8f0: 2020 2020 2020 2020 5f74 7970 6520 3d20          _type = 
-0002a900: 2743 6c75 7374 6572 2720 6966 2063 6c75  'Cluster' if clu
-0002a910: 7374 6572 2065 6c73 6520 2756 6d27 0a20  ster else 'Vm'. 
-0002a920: 2020 2020 2020 2074 6974 6c65 203d 2066         title = f
-0002a930: 227b 5f74 7970 657d 207b 6e61 6d65 7d20  "{_type} {name} 
-0002a940: 6f6e 207b 7365 6c66 2e63 6c69 656e 747d  on {self.client}
-0002a950: 2072 6570 6f72 7422 0a20 2020 2020 2020   report".       
-0002a960: 2063 6d64 732c 206d 6169 6c63 6f6e 7465   cmds, mailconte
-0002a970: 6e74 203d 205b 5d2c 204e 6f6e 650a 2020  nt = [], None.  
-0002a980: 2020 2020 2020 666f 7220 6e6f 7469 6679        for notify
-0002a990: 6d65 7468 6f64 2069 6e20 736f 7274 6564  method in sorted
-0002a9a0: 286e 6f74 6966 796d 6574 686f 6473 2c20  (notifymethods, 
-0002a9b0: 7265 7665 7273 653d 5472 7565 293a 0a20  reverse=True):. 
-0002a9c0: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-0002a9d0: 7469 6679 6d65 7468 6f64 203d 3d20 2770  tifymethod == 'p
-0002a9e0: 7573 6862 756c 6c65 7427 3a0a 2020 2020  ushbullet':.    
-0002a9f0: 2020 2020 2020 2020 2020 2020 6966 2070              if p
-0002aa00: 7573 6862 756c 6c65 7474 6f6b 656e 2069  ushbullettoken i
-0002aa10: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-0002aa20: 2020 2020 2020 2020 2020 2020 7761 726e              warn
-0002aa30: 696e 6728 6622 4e6f 7469 6669 6361 7469  ing(f"Notificati
-0002aa40: 6f6e 2072 6571 7569 7265 6420 666f 7220  on required for 
-0002aa50: 7b6e 616d 657d 2062 7574 206d 6973 7369  {name} but missi
-0002aa60: 6e67 2070 7573 6862 756c 6c65 7474 6f6b  ng pushbullettok
-0002aa70: 656e 2229 0a20 2020 2020 2020 2020 2020  en").           
-0002aa80: 2020 2020 2065 6c69 6620 6e6f 7469 6679       elif notify
-0002aa90: 7363 7269 7074 2069 7320 4e6f 6e65 2061  script is None a
-0002aaa0: 6e64 206e 6f74 6966 7963 6d64 2069 7320  nd notifycmd is 
-0002aab0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0002aac0: 2020 2020 2020 2020 2020 636f 6e74 696e            contin
-0002aad0: 7565 0a20 2020 2020 2020 2020 2020 2020  ue.             
-0002aae0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0002aaf0: 2020 2020 2020 2020 2020 2020 2074 6f6b               tok
-0002ab00: 656e 203d 2070 7573 6862 756c 6c65 7474  en = pushbullett
-0002ab10: 6f6b 656e 0a20 2020 2020 2020 2020 2020  oken.           
-0002ab20: 2020 2020 2020 2020 2070 6263 6d64 203d           pbcmd =
-0002ab30: 2027 6375 726c 202d 7375 2022 2573 3a22   'curl -su "%s:"
-0002ab40: 202d 6420 7479 7065 3d22 6e6f 7465 2220   -d type="note" 
-0002ab50: 2d64 2062 6f64 793d 2260 2573 2032 3e26  -d body="`%s 2>&
-0002ab60: 3160 2220 2d64 2074 6974 6c65 3d22 2573  1`" -d title="%s
-0002ab70: 2220 2720 2520 2874 6f6b 656e 2c0a 2020  " ' % (token,.  
+0002a870: 736c 6163 6b63 6861 6e6e 656c 3d4e 6f6e  slackchannel=Non
+0002a880: 652c 2073 6c61 636b 746f 6b65 6e3d 4e6f  e, slacktoken=No
+0002a890: 6e65 2c20 6d61 696c 7365 7276 6572 3d4e  ne, mailserver=N
+0002a8a0: 6f6e 652c 206d 6169 6c66 726f 6d3d 4e6f  one, mailfrom=No
+0002a8b0: 6e65 2c20 6d61 696c 746f 3d4e 6f6e 652c  ne, mailto=None,
+0002a8c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002a8d0: 2020 2020 2020 2020 2020 2020 2020 636c                cl
+0002a8e0: 7573 7465 723d 4661 6c73 6529 3a0a 2020  uster=False):.  
+0002a8f0: 2020 2020 2020 5f74 7970 6520 3d20 2743        _type = 'C
+0002a900: 6c75 7374 6572 2720 6966 2063 6c75 7374  luster' if clust
+0002a910: 6572 2065 6c73 6520 2756 6d27 0a20 2020  er else 'Vm'.   
+0002a920: 2020 2020 2074 6974 6c65 203d 2066 227b       title = f"{
+0002a930: 5f74 7970 657d 207b 6e61 6d65 7d20 6f6e  _type} {name} on
+0002a940: 207b 7365 6c66 2e63 6c69 656e 747d 2072   {self.client} r
+0002a950: 6570 6f72 7422 0a20 2020 2020 2020 2063  eport".        c
+0002a960: 6d64 732c 206d 6169 6c63 6f6e 7465 6e74  mds, mailcontent
+0002a970: 203d 205b 5d2c 204e 6f6e 650a 2020 2020   = [], None.    
+0002a980: 2020 2020 666f 7220 6e6f 7469 6679 6d65      for notifyme
+0002a990: 7468 6f64 2069 6e20 736f 7274 6564 286e  thod in sorted(n
+0002a9a0: 6f74 6966 796d 6574 686f 6473 2c20 7265  otifymethods, re
+0002a9b0: 7665 7273 653d 5472 7565 293a 0a20 2020  verse=True):.   
+0002a9c0: 2020 2020 2020 2020 2069 6620 6e6f 7469           if noti
+0002a9d0: 6679 6d65 7468 6f64 203d 3d20 2770 7573  fymethod == 'pus
+0002a9e0: 6862 756c 6c65 7427 3a0a 2020 2020 2020  hbullet':.      
+0002a9f0: 2020 2020 2020 2020 2020 6966 2070 7573            if pus
+0002aa00: 6862 756c 6c65 7474 6f6b 656e 2069 7320  hbullettoken is 
+0002aa10: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0002aa20: 2020 2020 2020 2020 2020 7761 726e 696e            warnin
+0002aa30: 6728 6622 4e6f 7469 6669 6361 7469 6f6e  g(f"Notification
+0002aa40: 2072 6571 7569 7265 6420 666f 7220 7b6e   required for {n
+0002aa50: 616d 657d 2062 7574 206d 6973 7369 6e67  ame} but missing
+0002aa60: 2070 7573 6862 756c 6c65 7474 6f6b 656e   pushbullettoken
+0002aa70: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
+0002aa80: 2020 2065 6c69 6620 6e6f 7469 6679 7363     elif notifysc
+0002aa90: 7269 7074 2069 7320 4e6f 6e65 2061 6e64  ript is None and
+0002aaa0: 206e 6f74 6966 7963 6d64 2069 7320 4e6f   notifycmd is No
+0002aab0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0002aac0: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
+0002aad0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002aae0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0002aaf0: 2020 2020 2020 2020 2020 2074 6f6b 656e             token
+0002ab00: 203d 2070 7573 6862 756c 6c65 7474 6f6b   = pushbullettok
+0002ab10: 656e 0a20 2020 2020 2020 2020 2020 2020  en.             
+0002ab20: 2020 2020 2020 2070 6263 6d64 203d 2027         pbcmd = '
+0002ab30: 6375 726c 202d 7375 2022 2573 3a22 202d  curl -su "%s:" -
+0002ab40: 6420 7479 7065 3d22 6e6f 7465 2220 2d64  d type="note" -d
+0002ab50: 2062 6f64 793d 2260 2573 2032 3e26 3160   body="`%s 2>&1`
+0002ab60: 2220 2d64 2074 6974 6c65 3d22 2573 2220  " -d title="%s" 
+0002ab70: 2720 2520 2874 6f6b 656e 2c0a 2020 2020  ' % (token,.    
 0002ab80: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0002ab90: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0002aba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0002abb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0002abc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002abd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002abe0: 6e6f 7469 6679 636d 642c 0a20 2020 2020  notifycmd,.     
+0002abd0: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
+0002abe0: 7469 6679 636d 642c 0a20 2020 2020 2020  tifycmd,.       
 0002abf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0002ac00: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0002ac10: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0002ac20: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0002ac30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002ac40: 2020 2020 2020 2020 2020 2020 2074 6974               tit
-0002ac50: 6c65 290a 2020 2020 2020 2020 2020 2020  le).            
-0002ac60: 2020 2020 2020 2020 7062 636d 6420 2b3d          pbcmd +=
-0002ac70: 2027 6874 7470 733a 2f2f 6170 692e 7075   'https://api.pu
-0002ac80: 7368 6275 6c6c 6574 2e63 6f6d 2f76 322f  shbullet.com/v2/
-0002ac90: 7075 7368 6573 270a 2020 2020 2020 2020  pushes'.        
-0002aca0: 2020 2020 2020 2020 2020 2020 636d 6473              cmds
-0002acb0: 2e61 7070 656e 6428 7062 636d 6429 0a20  .append(pbcmd). 
-0002acc0: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-0002acd0: 6e6f 7469 6679 6d65 7468 6f64 203d 3d20  notifymethod == 
-0002ace0: 2773 6c61 636b 273a 0a20 2020 2020 2020  'slack':.       
-0002acf0: 2020 2020 2020 2020 2069 6620 736c 6163           if slac
-0002ad00: 6b63 6861 6e6e 656c 2069 7320 4e6f 6e65  kchannel is None
-0002ad10: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0002ad20: 2020 2020 2020 7761 726e 696e 6728 6622        warning(f"
-0002ad30: 4e6f 7469 6669 6361 7469 6f6e 2072 6571  Notification req
-0002ad40: 7569 7265 6420 666f 7220 7b6e 616d 657d  uired for {name}
-0002ad50: 2062 7574 206d 6973 7369 6e67 2073 6c61   but missing sla
-0002ad60: 636b 2063 6861 6e6e 656c 2229 0a20 2020  ck channel").   
-0002ad70: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
-0002ad80: 6620 736c 6163 6b74 6f6b 656e 2069 7320  f slacktoken is 
-0002ad90: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0002ada0: 2020 2020 2020 2020 2020 7761 726e 696e            warnin
-0002adb0: 6728 6622 4e6f 7469 6669 6361 7469 6f6e  g(f"Notification
-0002adc0: 2072 6571 7569 7265 6420 666f 7220 7b6e   required for {n
-0002add0: 616d 657d 2062 7574 206d 6973 7369 6e67  ame} but missing
-0002ade0: 2073 6c61 636b 746f 6b65 6e22 290a 2020   slacktoken").  
-0002adf0: 2020 2020 2020 2020 2020 2020 2020 656c                el
-0002ae00: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0002ae10: 2020 2020 2020 2020 736c 6163 6b63 6d64          slackcmd
-0002ae20: 203d 2066 2269 6e66 6f3d 607b 6e6f 7469   = f"info=`{noti
-0002ae30: 6679 636d 647d 2032 3e26 3120 7c20 7365  fycmd} 2>&1 | se
-0002ae40: 6420 2773 2f5c 5c78 322f 202f 6727 603b  d 's/\\x2/ /g'`;
-0002ae50: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-0002ae60: 2020 2020 2020 736c 6163 6b63 6d64 202b        slackcmd +
-0002ae70: 3d20 2222 2263 7572 6c20 2d58 2050 4f53  = """curl -X POS
-0002ae80: 5420 2d48 2027 4175 7468 6f72 697a 6174  T -H 'Authorizat
-0002ae90: 696f 6e3a 2042 6561 7265 7220 2573 270a  ion: Bearer %s'.
-0002aea0: 202d 4820 2743 6f6e 7465 6e74 2d74 7970   -H 'Content-typ
-0002aeb0: 653a 2061 7070 6c69 6361 7469 6f6e 2f6a  e: application/j
-0002aec0: 736f 6e3b 2063 6861 7273 6574 3d75 7466  son; charset=utf
-0002aed0: 2d38 270a 202d 2d64 6174 6120 277b 2263  -8'. --data '{"c
-0002aee0: 6861 6e6e 656c 223a 2225 7322 2c22 7465  hannel":"%s","te
-0002aef0: 7874 223a 2225 7322 2c22 6174 7461 6368  xt":"%s","attach
-0002af00: 6d65 6e74 7322 3a20 5b7b 2274 6578 7422  ments": [{"text"
-0002af10: 3a22 2722 2469 6e66 6f22 2722 2c22 6661  :"'"$info"'","fa
-0002af20: 6c6c 6261 636b 223a 226e 6f74 6869 6e67  llback":"nothing
-0002af30: 222c 0a22 636f 6c6f 7222 3a22 2333 4141  ",."color":"#3AA
-0002af40: 3345 3322 2c22 6174 7461 6368 6d65 6e74  3E3","attachment
-0002af50: 5f74 7970 6522 3a22 6465 6661 756c 7422  _type":"default"
-0002af60: 7d5d 7d27 2068 7474 7073 3a2f 2f73 6c61  }]}' https://sla
-0002af70: 636b 2e63 6f6d 2f61 7069 2f63 6861 742e  ck.com/api/chat.
-0002af80: 706f 7374 4d65 7373 6167 6522 2222 2025  postMessage""" %
-0002af90: 2028 736c 6163 6b74 6f6b 656e 2c0a 2020   (slacktoken,.  
+0002ac40: 2020 2020 2020 2020 2020 2074 6974 6c65             title
+0002ac50: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0002ac60: 2020 2020 2020 7062 636d 6420 2b3d 2027        pbcmd += '
+0002ac70: 6874 7470 733a 2f2f 6170 692e 7075 7368  https://api.push
+0002ac80: 6275 6c6c 6574 2e63 6f6d 2f76 322f 7075  bullet.com/v2/pu
+0002ac90: 7368 6573 270a 2020 2020 2020 2020 2020  shes'.          
+0002aca0: 2020 2020 2020 2020 2020 636d 6473 2e61            cmds.a
+0002acb0: 7070 656e 6428 7062 636d 6429 0a20 2020  ppend(pbcmd).   
+0002acc0: 2020 2020 2020 2020 2065 6c69 6620 6e6f           elif no
+0002acd0: 7469 6679 6d65 7468 6f64 203d 3d20 2773  tifymethod == 's
+0002ace0: 6c61 636b 273a 0a20 2020 2020 2020 2020  lack':.         
+0002acf0: 2020 2020 2020 2069 6620 736c 6163 6b63         if slackc
+0002ad00: 6861 6e6e 656c 2069 7320 4e6f 6e65 3a0a  hannel is None:.
+0002ad10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002ad20: 2020 2020 7761 726e 696e 6728 6622 4e6f      warning(f"No
+0002ad30: 7469 6669 6361 7469 6f6e 2072 6571 7569  tification requi
+0002ad40: 7265 6420 666f 7220 7b6e 616d 657d 2062  red for {name} b
+0002ad50: 7574 206d 6973 7369 6e67 2073 6c61 636b  ut missing slack
+0002ad60: 2063 6861 6e6e 656c 2229 0a20 2020 2020   channel").     
+0002ad70: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+0002ad80: 736c 6163 6b74 6f6b 656e 2069 7320 4e6f  slacktoken is No
+0002ad90: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0002ada0: 2020 2020 2020 2020 7761 726e 696e 6728          warning(
+0002adb0: 6622 4e6f 7469 6669 6361 7469 6f6e 2072  f"Notification r
+0002adc0: 6571 7569 7265 6420 666f 7220 7b6e 616d  equired for {nam
+0002add0: 657d 2062 7574 206d 6973 7369 6e67 2073  e} but missing s
+0002ade0: 6c61 636b 746f 6b65 6e22 290a 2020 2020  lacktoken").    
+0002adf0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+0002ae00: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0002ae10: 2020 2020 2020 736c 6163 6b63 6d64 203d        slackcmd =
+0002ae20: 2066 2269 6e66 6f3d 607b 6e6f 7469 6679   f"info=`{notify
+0002ae30: 636d 647d 2032 3e26 3120 7c20 7365 6420  cmd} 2>&1 | sed 
+0002ae40: 2773 2f5c 5c78 322f 202f 6727 603b 220a  's/\\x2/ /g'`;".
+0002ae50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002ae60: 2020 2020 736c 6163 6b63 6d64 202b 3d20      slackcmd += 
+0002ae70: 2222 2263 7572 6c20 2d58 2050 4f53 5420  """curl -X POST 
+0002ae80: 2d48 2027 4175 7468 6f72 697a 6174 696f  -H 'Authorizatio
+0002ae90: 6e3a 2042 6561 7265 7220 2573 270a 202d  n: Bearer %s'. -
+0002aea0: 4820 2743 6f6e 7465 6e74 2d74 7970 653a  H 'Content-type:
+0002aeb0: 2061 7070 6c69 6361 7469 6f6e 2f6a 736f   application/jso
+0002aec0: 6e3b 2063 6861 7273 6574 3d75 7466 2d38  n; charset=utf-8
+0002aed0: 270a 202d 2d64 6174 6120 277b 2263 6861  '. --data '{"cha
+0002aee0: 6e6e 656c 223a 2225 7322 2c22 7465 7874  nnel":"%s","text
+0002aef0: 223a 2225 7322 2c22 6174 7461 6368 6d65  ":"%s","attachme
+0002af00: 6e74 7322 3a20 5b7b 2274 6578 7422 3a22  nts": [{"text":"
+0002af10: 2722 2469 6e66 6f22 2722 2c22 6661 6c6c  '"$info"'","fall
+0002af20: 6261 636b 223a 226e 6f74 6869 6e67 222c  back":"nothing",
+0002af30: 0a22 636f 6c6f 7222 3a22 2333 4141 3345  ."color":"#3AA3E
+0002af40: 3322 2c22 6174 7461 6368 6d65 6e74 5f74  3","attachment_t
+0002af50: 7970 6522 3a22 6465 6661 756c 7422 7d5d  ype":"default"}]
+0002af60: 7d27 2068 7474 7073 3a2f 2f73 6c61 636b  }' https://slack
+0002af70: 2e63 6f6d 2f61 7069 2f63 6861 742e 706f  .com/api/chat.po
+0002af80: 7374 4d65 7373 6167 6522 2222 2025 2028  stMessage""" % (
+0002af90: 736c 6163 6b74 6f6b 656e 2c0a 2020 2020  slacktoken,.    
 0002afa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0002afb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0002afc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0002afd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0002afe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002aff0: 2020 2020 2020 2020 2020 2020 2073 6c61               sla
-0002b000: 636b 6368 616e 6e65 6c2c 2074 6974 6c65  ckchannel, title
-0002b010: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0002b020: 2020 2020 2020 736c 6163 6b63 6d64 203d        slackcmd =
-0002b030: 2073 6c61 636b 636d 642e 7265 706c 6163   slackcmd.replac
-0002b040: 6528 275c 6e27 2c20 2727 290a 2020 2020  e('\n', '').    
-0002b050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002b060: 636d 6473 2e61 7070 656e 6428 736c 6163  cmds.append(slac
-0002b070: 6b63 6d64 290a 2020 2020 2020 2020 2020  kcmd).          
-0002b080: 2020 656c 6966 206e 6f74 6966 796d 6574    elif notifymet
-0002b090: 686f 6420 3d3d 2027 6d61 696c 273a 0a20  hod == 'mail':. 
-0002b0a0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0002b0b0: 6620 6d61 696c 7365 7276 6572 2069 7320  f mailserver is 
-0002b0c0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0002b0d0: 2020 2020 2020 2020 2020 7761 726e 696e            warnin
-0002b0e0: 6728 6622 4e6f 7469 6669 6361 7469 6f6e  g(f"Notification
-0002b0f0: 2072 6571 7569 7265 6420 666f 7220 7b6e   required for {n
-0002b100: 616d 657d 2062 7574 206d 6973 7369 6e67  ame} but missing
-0002b110: 206d 6169 6c73 6572 7665 7222 290a 2020   mailserver").  
-0002b120: 2020 2020 2020 2020 2020 2020 2020 656c                el
-0002b130: 6966 206d 6169 6c66 726f 6d20 6973 204e  if mailfrom is N
-0002b140: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0002b150: 2020 2020 2020 2020 2077 6172 6e69 6e67           warning
-0002b160: 2866 224e 6f74 6966 6963 6174 696f 6e20  (f"Notification 
-0002b170: 7265 7175 6972 6564 2066 6f72 207b 6e61  required for {na
-0002b180: 6d65 7d20 6275 7420 6d69 7373 696e 6720  me} but missing 
-0002b190: 6d61 696c 6672 6f6d 2229 0a20 2020 2020  mailfrom").     
-0002b1a0: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-0002b1b0: 6e6f 7420 6d61 696c 746f 3a0a 2020 2020  not mailto:.    
-0002b1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002b1d0: 7761 726e 696e 6728 6622 4e6f 7469 6669  warning(f"Notifi
-0002b1e0: 6361 7469 6f6e 2072 6571 7569 7265 6420  cation required 
-0002b1f0: 666f 7220 7b6e 616d 657d 2062 7574 206d  for {name} but m
-0002b200: 6973 7369 6e67 206d 6169 6c74 6f22 290a  issing mailto").
-0002b210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002b220: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0002b230: 2020 2020 2020 2020 2020 6e6f 7720 3d20            now = 
-0002b240: 6461 7465 7469 6d65 2e6e 6f77 2829 0a20  datetime.now(). 
+0002aff0: 2020 2020 2020 2020 2020 2073 6c61 636b             slack
+0002b000: 6368 616e 6e65 6c2c 2074 6974 6c65 290a  channel, title).
+0002b010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002b020: 2020 2020 736c 6163 6b63 6d64 203d 2073      slackcmd = s
+0002b030: 6c61 636b 636d 642e 7265 706c 6163 6528  lackcmd.replace(
+0002b040: 275c 6e27 2c20 2727 290a 2020 2020 2020  '\n', '').      
+0002b050: 2020 2020 2020 2020 2020 2020 2020 636d                cm
+0002b060: 6473 2e61 7070 656e 6428 736c 6163 6b63  ds.append(slackc
+0002b070: 6d64 290a 2020 2020 2020 2020 2020 2020  md).            
+0002b080: 656c 6966 206e 6f74 6966 796d 6574 686f  elif notifymetho
+0002b090: 6420 3d3d 2027 6d61 696c 273a 0a20 2020  d == 'mail':.   
+0002b0a0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0002b0b0: 6d61 696c 7365 7276 6572 2069 7320 4e6f  mailserver is No
+0002b0c0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0002b0d0: 2020 2020 2020 2020 7761 726e 696e 6728          warning(
+0002b0e0: 6622 4e6f 7469 6669 6361 7469 6f6e 2072  f"Notification r
+0002b0f0: 6571 7569 7265 6420 666f 7220 7b6e 616d  equired for {nam
+0002b100: 657d 2062 7574 206d 6973 7369 6e67 206d  e} but missing m
+0002b110: 6169 6c73 6572 7665 7222 290a 2020 2020  ailserver").    
+0002b120: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+0002b130: 206d 6169 6c66 726f 6d20 6973 204e 6f6e   mailfrom is Non
+0002b140: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0002b150: 2020 2020 2020 2077 6172 6e69 6e67 2866         warning(f
+0002b160: 224e 6f74 6966 6963 6174 696f 6e20 7265  "Notification re
+0002b170: 7175 6972 6564 2066 6f72 207b 6e61 6d65  quired for {name
+0002b180: 7d20 6275 7420 6d69 7373 696e 6720 6d61  } but missing ma
+0002b190: 696c 6672 6f6d 2229 0a20 2020 2020 2020  ilfrom").       
+0002b1a0: 2020 2020 2020 2020 2065 6c69 6620 6e6f           elif no
+0002b1b0: 7420 6d61 696c 746f 3a0a 2020 2020 2020  t mailto:.      
+0002b1c0: 2020 2020 2020 2020 2020 2020 2020 7761                wa
+0002b1d0: 726e 696e 6728 6622 4e6f 7469 6669 6361  rning(f"Notifica
+0002b1e0: 7469 6f6e 2072 6571 7569 7265 6420 666f  tion required fo
+0002b1f0: 7220 7b6e 616d 657d 2062 7574 206d 6973  r {name} but mis
+0002b200: 7369 6e67 206d 6169 6c74 6f22 290a 2020  sing mailto").  
+0002b210: 2020 2020 2020 2020 2020 2020 2020 656c                el
+0002b220: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0002b230: 2020 2020 2020 2020 6e6f 7720 3d20 6461          now = da
+0002b240: 7465 7469 6d65 2e6e 6f77 2829 0a20 2020  tetime.now().   
 0002b250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002b260: 2020 206e 6f77 203d 206e 6f77 2e20 7374     now = now. st
-0002b270: 7266 7469 6d65 2822 2561 2c25 6420 2562  rftime("%a,%d %b
-0002b280: 2025 5920 2548 3a25 4d3a 2553 2229 0a20   %Y %H:%M:%S"). 
+0002b260: 206e 6f77 203d 206e 6f77 2e20 7374 7266   now = now. strf
+0002b270: 7469 6d65 2822 2561 2c25 6420 2562 2025  time("%a,%d %b %
+0002b280: 5920 2548 3a25 4d3a 2553 2229 0a20 2020  Y %H:%M:%S").   
 0002b290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002b2a0: 2020 2074 6f73 203d 2027 2c27 2e6a 6f69     tos = ','.joi
-0002b2b0: 6e28 5b66 223c 7b74 6f7d 3e22 2066 6f72  n([f"<{to}>" for
-0002b2c0: 2074 6f20 696e 206d 6169 6c74 6f5d 290a   to in mailto]).
+0002b2a0: 2074 6f73 203d 2027 2c27 2e6a 6f69 6e28   tos = ','.join(
+0002b2b0: 5b66 223c 7b74 6f7d 3e22 2066 6f72 2074  [f"<{to}>" for t
+0002b2c0: 6f20 696e 206d 6169 6c74 6f5d 290a 2020  o in mailto]).  
 0002b2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002b2e0: 2020 2020 6d61 696c 636f 6e74 656e 7420      mailcontent 
-0002b2f0: 3d20 6622 4672 6f6d 3a20 7b6d 6169 6c66  = f"From: {mailf
-0002b300: 726f 6d7d 203c 7b6d 6169 6c66 726f 6d7d  rom} <{mailfrom}
-0002b310: 3e5c 6e54 6f3a 207b 746f 737d 5c6e 4461  >\nTo: {tos}\nDa
-0002b320: 7465 3a20 7b6e 6f77 7d5c 6e53 7562 6a65  te: {now}\nSubje
-0002b330: 6374 3a20 7b74 6974 6c65 7d22 0a20 2020  ct: {title}".   
-0002b340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002b350: 206d 6169 6c63 6d64 203d 205b 5d0a 2020   mailcmd = [].  
+0002b2e0: 2020 6d61 696c 636f 6e74 656e 7420 3d20    mailcontent = 
+0002b2f0: 6622 4672 6f6d 3a20 7b6d 6169 6c66 726f  f"From: {mailfro
+0002b300: 6d7d 203c 7b6d 6169 6c66 726f 6d7d 3e5c  m} <{mailfrom}>\
+0002b310: 6e54 6f3a 207b 746f 737d 5c6e 4461 7465  nTo: {tos}\nDate
+0002b320: 3a20 7b6e 6f77 7d5c 6e53 7562 6a65 6374  : {now}\nSubject
+0002b330: 3a20 7b74 6974 6c65 7d22 0a20 2020 2020  : {title}".     
+0002b340: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+0002b350: 6169 6c63 6d64 203d 205b 5d0a 2020 2020  ailcmd = [].    
 0002b360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002b370: 2020 6966 206e 6f74 2063 6c75 7374 6572    if not cluster
-0002b380: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0002b390: 2020 2020 2020 2020 2020 6d61 696c 636d            mailcm
-0002b3a0: 642e 6170 7065 6e64 2827 7465 7374 202d  d.append('test -
-0002b3b0: 6620 2f65 7463 2f64 6562 6961 6e5f 7665  f /etc/debian_ve
-0002b3c0: 7273 696f 6e20 2626 2061 7074 2d67 6574  rsion && apt-get
-0002b3d0: 202d 7920 696e 7374 616c 6c20 6375 726c   -y install curl
-0002b3e0: 2729 0a20 2020 2020 2020 2020 2020 2020  ').             
-0002b3f0: 2020 2020 2020 2020 2020 206d 6169 6c63             mailc
-0002b400: 6d64 2e61 7070 656e 6428 2765 6368 6f20  md.append('echo 
-0002b410: 2222 203e 3e20 2f76 6172 2f74 6d70 2f6d  "" >> /var/tmp/m
-0002b420: 6169 6c2e 7478 7427 290a 2020 2020 2020  ail.txt').      
-0002b430: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
-0002b440: 696c 636d 642e 6170 7065 6e64 2866 277b  ilcmd.append(f'{
-0002b450: 6e6f 7469 6679 636d 647d 2032 3e26 3120  notifycmd} 2>&1 
-0002b460: 3e3e 202f 7661 722f 746d 702f 6d61 696c  >> /var/tmp/mail
-0002b470: 2e74 7874 2729 0a20 2020 2020 2020 2020  .txt').         
-0002b480: 2020 2020 2020 2020 2020 2063 7572 6c63             curlc
-0002b490: 6d64 203d 2066 2263 7572 6c20 2d2d 7369  md = f"curl --si
-0002b4a0: 6c65 6e74 202d 2d75 726c 2073 6d74 703a  lent --url smtp:
-0002b4b0: 2f2f 7b6d 6169 6c73 6572 7665 727d 3a32  //{mailserver}:2
-0002b4c0: 3520 2d2d 6d61 696c 2d66 726f 6d20 7b6d  5 --mail-from {m
-0002b4d0: 6169 6c66 726f 6d7d 220a 2020 2020 2020  ailfrom}".      
-0002b4e0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-0002b4f0: 7220 6164 6472 6573 7320 696e 206d 6169  r address in mai
-0002b500: 6c74 6f3a 0a20 2020 2020 2020 2020 2020  lto:.           
-0002b510: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-0002b520: 6c63 6d64 202b 3d20 6622 202d 2d6d 6169  lcmd += f" --mai
-0002b530: 6c2d 7263 7074 207b 6164 6472 6573 737d  l-rcpt {address}
-0002b540: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
-0002b550: 2020 2020 2020 2069 6620 636c 7573 7465         if cluste
-0002b560: 723a 0a20 2020 2020 2020 2020 2020 2020  r:.             
-0002b570: 2020 2020 2020 2020 2020 206d 6169 6c63             mailc
-0002b580: 6f6e 7465 6e74 203d 2022 220a 2020 2020  ontent = "".    
+0002b370: 6966 206e 6f74 2063 6c75 7374 6572 3a0a  if not cluster:.
+0002b380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002b390: 2020 2020 2020 2020 6d61 696c 636d 642e          mailcmd.
+0002b3a0: 6170 7065 6e64 2827 7465 7374 202d 6620  append('test -f 
+0002b3b0: 2f65 7463 2f64 6562 6961 6e5f 7665 7273  /etc/debian_vers
+0002b3c0: 696f 6e20 2626 2061 7074 2d67 6574 202d  ion && apt-get -
+0002b3d0: 7920 696e 7374 616c 6c20 6375 726c 2729  y install curl')
+0002b3e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002b3f0: 2020 2020 2020 2020 206d 6169 6c63 6d64           mailcmd
+0002b400: 2e61 7070 656e 6428 2765 6368 6f20 2222  .append('echo ""
+0002b410: 203e 3e20 2f76 6172 2f74 6d70 2f6d 6169   >> /var/tmp/mai
+0002b420: 6c2e 7478 7427 290a 2020 2020 2020 2020  l.txt').        
+0002b430: 2020 2020 2020 2020 2020 2020 6d61 696c              mail
+0002b440: 636d 642e 6170 7065 6e64 2866 277b 6e6f  cmd.append(f'{no
+0002b450: 7469 6679 636d 647d 2032 3e26 3120 3e3e  tifycmd} 2>&1 >>
+0002b460: 202f 7661 722f 746d 702f 6d61 696c 2e74   /var/tmp/mail.t
+0002b470: 7874 2729 0a20 2020 2020 2020 2020 2020  xt').           
+0002b480: 2020 2020 2020 2020 2063 7572 6c63 6d64           curlcmd
+0002b490: 203d 2066 2263 7572 6c20 2d2d 7369 6c65   = f"curl --sile
+0002b4a0: 6e74 202d 2d75 726c 2073 6d74 703a 2f2f  nt --url smtp://
+0002b4b0: 7b6d 6169 6c73 6572 7665 727d 3a32 3520  {mailserver}:25 
+0002b4c0: 2d2d 6d61 696c 2d66 726f 6d20 7b6d 6169  --mail-from {mai
+0002b4d0: 6c66 726f 6d7d 220a 2020 2020 2020 2020  lfrom}".        
+0002b4e0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0002b4f0: 6164 6472 6573 7320 696e 206d 6169 6c74  address in mailt
+0002b500: 6f3a 0a20 2020 2020 2020 2020 2020 2020  o:.             
+0002b510: 2020 2020 2020 2020 2020 2063 7572 6c63             curlc
+0002b520: 6d64 202b 3d20 6622 202d 2d6d 6169 6c2d  md += f" --mail-
+0002b530: 7263 7074 207b 6164 6472 6573 737d 2022  rcpt {address} "
+0002b540: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002b550: 2020 2020 2069 6620 636c 7573 7465 723a       if cluster:
+0002b560: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002b570: 2020 2020 2020 2020 206d 6169 6c63 6f6e           mailcon
+0002b580: 7465 6e74 203d 2022 220a 2020 2020 2020  tent = "".      
 0002b590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002b5a0: 2020 2020 6b75 6265 636f 6e66 6967 203d      kubeconfig =
-0002b5b0: 2066 272f 6574 632f 6b75 6265 726e 6574   f'/etc/kubernet
-0002b5c0: 6573 2f6b 7562 6563 6f6e 6669 672e 7b6e  es/kubeconfig.{n
-0002b5d0: 616d 657d 270a 2020 2020 2020 2020 2020  ame}'.          
-0002b5e0: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-0002b5f0: 726c 636d 6420 2b3d 2066 2720 2d48 2022  rlcmd += f' -H "
-0002b600: 5375 626a 6563 743a 207b 7469 746c 657d  Subject: {title}
-0002b610: 2220 2d48 2022 4672 6f6d 3a20 7b6d 6169  " -H "From: {mai
-0002b620: 6c66 726f 6d7d 203c 7b6d 6169 6c66 726f  lfrom} <{mailfro
-0002b630: 6d7d 3e22 270a 2020 2020 2020 2020 2020  m}>"'.          
-0002b640: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-0002b650: 7220 6164 6472 6573 7320 696e 206d 6169  r address in mai
-0002b660: 6c74 6f3a 0a20 2020 2020 2020 2020 2020  lto:.           
-0002b670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002b680: 2063 7572 6c63 6d64 202b 3d20 6627 202d   curlcmd += f' -
-0002b690: 4820 2254 6f3a 207b 6164 6472 6573 737d  H "To: {address}
-0002b6a0: 203c 7b61 6464 7265 7373 7d3e 2227 0a20   <{address}>"'. 
+0002b5a0: 2020 6b75 6265 636f 6e66 6967 203d 2066    kubeconfig = f
+0002b5b0: 272f 6574 632f 6b75 6265 726e 6574 6573  '/etc/kubernetes
+0002b5c0: 2f6b 7562 6563 6f6e 6669 672e 7b6e 616d  /kubeconfig.{nam
+0002b5d0: 657d 270a 2020 2020 2020 2020 2020 2020  e}'.            
+0002b5e0: 2020 2020 2020 2020 2020 2020 6375 726c              curl
+0002b5f0: 636d 6420 2b3d 2066 2720 2d48 2022 5375  cmd += f' -H "Su
+0002b600: 626a 6563 743a 207b 7469 746c 657d 2220  bject: {title}" 
+0002b610: 2d48 2022 4672 6f6d 3a20 7b6d 6169 6c66  -H "From: {mailf
+0002b620: 726f 6d7d 203c 7b6d 6169 6c66 726f 6d7d  rom} <{mailfrom}
+0002b630: 3e22 270a 2020 2020 2020 2020 2020 2020  >"'.            
+0002b640: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0002b650: 6164 6472 6573 7320 696e 206d 6169 6c74  address in mailt
+0002b660: 6f3a 0a20 2020 2020 2020 2020 2020 2020  o:.             
+0002b670: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0002b680: 7572 6c63 6d64 202b 3d20 6627 202d 4820  urlcmd += f' -H 
+0002b690: 2254 6f3a 207b 6164 6472 6573 737d 203c  "To: {address} <
+0002b6a0: 7b61 6464 7265 7373 7d3e 2227 0a20 2020  {address}>"'.   
 0002b6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002b6c0: 2020 2020 2020 2063 7572 6c63 6d64 202b         curlcmd +
-0002b6d0: 3d20 2720 2d46 2022 3d28 3b74 7970 653d  = ' -F "=(;type=
-0002b6e0: 6d75 6c74 6970 6172 742f 6d69 7865 6422  multipart/mixed"
-0002b6f0: 202d 4620 223d 2428 6361 7420 2f76 6172   -F "=$(cat /var
-0002b700: 2f74 6d70 2f6d 6169 6c2e 7478 7429 3b74  /tmp/mail.txt);t
-0002b710: 7970 653d 7465 7874 2f70 6c61 696e 2227  ype=text/plain"'
-0002b720: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002b730: 2020 2020 2020 2020 2063 7572 6c63 6d64           curlcmd
-0002b740: 202b 3d20 6627 202d 4620 2266 696c 653d   += f' -F "file=
-0002b750: 407b 6b75 6265 636f 6e66 6967 7d3b 7479  @{kubeconfig};ty
-0002b760: 7065 3d74 6578 742f 706c 6169 6e3b 656e  pe=text/plain;en
-0002b770: 636f 6465 723d 6261 7365 3634 2220 2d46  coder=base64" -F
-0002b780: 2022 3d29 2227 0a20 2020 2020 2020 2020   "=)"'.         
-0002b790: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-0002b7a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002b7b0: 2020 2020 2020 2020 2063 7572 6c63 6d64           curlcmd
-0002b7c0: 202b 3d20 2220 2d2d 7570 6c6f 6164 2d66   += " --upload-f
-0002b7d0: 696c 6520 2f76 6172 2f74 6d70 2f6d 6169  ile /var/tmp/mai
-0002b7e0: 6c2e 7478 7422 0a20 2020 2020 2020 2020  l.txt".         
-0002b7f0: 2020 2020 2020 2020 2020 206d 6169 6c63             mailc
-0002b800: 6d64 2e61 7070 656e 6428 6375 726c 636d  md.append(curlcm
-0002b810: 6429 0a20 2020 2020 2020 2020 2020 2020  d).             
-0002b820: 2020 2020 2020 2063 6d64 732e 6578 7465         cmds.exte
-0002b830: 6e64 286d 6169 6c63 6d64 290a 2020 2020  nd(mailcmd).    
-0002b840: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0002b850: 2020 2020 2020 2020 2020 2020 2020 6572                er
-0002b860: 726f 7228 6622 496e 7661 6c69 6420 6d65  ror(f"Invalid me
-0002b870: 7468 6f64 207b 6e6f 7469 6679 6d65 7468  thod {notifymeth
-0002b880: 6f64 7d22 290a 2020 2020 2020 2020 7265  od}").        re
-0002b890: 7475 726e 2063 6d64 732c 206d 6169 6c63  turn cmds, mailc
-0002b8a0: 6f6e 7465 6e74 0a0a 2020 2020 6465 6620  ontent..    def 
-0002b8b0: 6861 6e64 6c65 5f76 6d5f 7265 7375 6c74  handle_vm_result
-0002b8c0: 2873 656c 662c 206e 616d 652c 2070 726f  (self, name, pro
-0002b8d0: 6669 6c65 2c20 7265 7375 6c74 2c20 6e65  file, result, ne
-0002b8e0: 7776 6d73 2c20 6661 696c 6564 766d 732c  wvms, failedvms,
-0002b8f0: 2061 7379 6e63 7761 6974 766d 732c 206f   asyncwaitvms, o
-0002b900: 6e6c 7961 7373 6574 733d 4661 6c73 652c  nlyassets=False,
-0002b910: 206e 6577 6173 7365 7473 3d5b 5d2c 0a20   newassets=[],. 
+0002b6c0: 2020 2020 2063 7572 6c63 6d64 202b 3d20       curlcmd += 
+0002b6d0: 2720 2d46 2022 3d28 3b74 7970 653d 6d75  ' -F "=(;type=mu
+0002b6e0: 6c74 6970 6172 742f 6d69 7865 6422 202d  ltipart/mixed" -
+0002b6f0: 4620 223d 2428 6361 7420 2f76 6172 2f74  F "=$(cat /var/t
+0002b700: 6d70 2f6d 6169 6c2e 7478 7429 3b74 7970  mp/mail.txt);typ
+0002b710: 653d 7465 7874 2f70 6c61 696e 2227 0a20  e=text/plain"'. 
+0002b720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002b730: 2020 2020 2020 2063 7572 6c63 6d64 202b         curlcmd +
+0002b740: 3d20 6627 202d 4620 2266 696c 653d 407b  = f' -F "file=@{
+0002b750: 6b75 6265 636f 6e66 6967 7d3b 7479 7065  kubeconfig};type
+0002b760: 3d74 6578 742f 706c 6169 6e3b 656e 636f  =text/plain;enco
+0002b770: 6465 723d 6261 7365 3634 2220 2d46 2022  der=base64" -F "
+0002b780: 3d29 2227 0a20 2020 2020 2020 2020 2020  =)"'.           
+0002b790: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+0002b7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002b7b0: 2020 2020 2020 2063 7572 6c63 6d64 202b         curlcmd +
+0002b7c0: 3d20 2220 2d2d 7570 6c6f 6164 2d66 696c  = " --upload-fil
+0002b7d0: 6520 2f76 6172 2f74 6d70 2f6d 6169 6c2e  e /var/tmp/mail.
+0002b7e0: 7478 7422 0a20 2020 2020 2020 2020 2020  txt".           
+0002b7f0: 2020 2020 2020 2020 206d 6169 6c63 6d64           mailcmd
+0002b800: 2e61 7070 656e 6428 6375 726c 636d 6429  .append(curlcmd)
+0002b810: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002b820: 2020 2020 2063 6d64 732e 6578 7465 6e64       cmds.extend
+0002b830: 286d 6169 6c63 6d64 290a 2020 2020 2020  (mailcmd).      
+0002b840: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+0002b850: 2020 2020 2020 2020 2020 2020 6572 726f              erro
+0002b860: 7228 6622 496e 7661 6c69 6420 6d65 7468  r(f"Invalid meth
+0002b870: 6f64 207b 6e6f 7469 6679 6d65 7468 6f64  od {notifymethod
+0002b880: 7d22 290a 2020 2020 2020 2020 7265 7475  }").        retu
+0002b890: 726e 2063 6d64 732c 206d 6169 6c63 6f6e  rn cmds, mailcon
+0002b8a0: 7465 6e74 0a0a 2020 2020 6465 6620 6861  tent..    def ha
+0002b8b0: 6e64 6c65 5f76 6d5f 7265 7375 6c74 2873  ndle_vm_result(s
+0002b8c0: 656c 662c 206e 616d 652c 2070 726f 6669  elf, name, profi
+0002b8d0: 6c65 2c20 7265 7375 6c74 2c20 6e65 7776  le, result, newv
+0002b8e0: 6d73 2c20 6661 696c 6564 766d 732c 2061  ms, failedvms, a
+0002b8f0: 7379 6e63 7761 6974 766d 732c 206f 6e6c  syncwaitvms, onl
+0002b900: 7961 7373 6574 733d 4661 6c73 652c 206e  yassets=False, n
+0002b910: 6577 6173 7365 7473 3d5b 5d2c 0a20 2020  ewassets=[],.   
 0002b920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002b930: 2020 2020 2020 2020 766d 636c 6965 6e74          vmclient
-0002b940: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
-0002b950: 6966 2027 7265 7375 6c74 2720 696e 2072  if 'result' in r
-0002b960: 6573 756c 7420 616e 6420 7265 7375 6c74  esult and result
-0002b970: 5b27 7265 7375 6c74 275d 203d 3d20 2773  ['result'] == 's
-0002b980: 7563 6365 7373 273a 0a20 2020 2020 2020  uccess':.       
-0002b990: 2020 2020 206e 6577 766d 732e 6170 7065       newvms.appe
-0002b9a0: 6e64 286e 616d 6529 0a20 2020 2020 2020  nd(name).       
-0002b9b0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0002b9c0: 2020 2066 6169 6c65 6476 6d73 2e61 7070     failedvms.app
-0002b9d0: 656e 6428 7b27 6e61 6d65 273a 206e 616d  end({'name': nam
-0002b9e0: 652c 2027 7265 6173 6f6e 273a 2072 6573  e, 'reason': res
-0002b9f0: 756c 745b 2772 6561 736f 6e27 5d7d 290a  ult['reason']}).
-0002ba00: 2020 2020 2020 2020 7374 6172 7420 3d20          start = 
-0002ba10: 7072 6f66 696c 652e 6765 7428 2773 7461  profile.get('sta
-0002ba20: 7274 272c 2054 7275 6529 0a20 2020 2020  rt', True).     
-0002ba30: 2020 2063 6c6f 7564 696e 6974 203d 2070     cloudinit = p
-0002ba40: 726f 6669 6c65 2e67 6574 2827 636c 6f75  rofile.get('clou
-0002ba50: 6469 6e69 7427 2c20 5472 7565 290a 2020  dinit', True).  
-0002ba60: 2020 2020 2020 6173 796e 6377 6169 7420        asyncwait 
-0002ba70: 3d20 7072 6f66 696c 652e 6765 7428 2761  = profile.get('a
-0002ba80: 7379 6e63 7761 6974 272c 2046 616c 7365  syncwait', False
-0002ba90: 290a 2020 2020 2020 2020 6669 6e69 7368  ).        finish
-0002baa0: 6669 6c65 7320 3d20 7072 6f66 696c 652e  files = profile.
-0002bab0: 6765 7428 2766 696e 6973 6866 696c 6573  get('finishfiles
-0002bac0: 272c 205b 5d29 0a20 2020 2020 2020 2069  ', []).        i
-0002bad0: 6620 6f6e 6c79 6173 7365 7473 3a0a 2020  f onlyassets:.  
-0002bae0: 2020 2020 2020 2020 2020 6966 2027 7573            if 'us
-0002baf0: 6572 6461 7461 2720 696e 2072 6573 756c  erdata' in resul
-0002bb00: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
-0002bb10: 2020 206e 6577 6173 7365 7473 2e61 7070     newassets.app
-0002bb20: 656e 6428 7265 7375 6c74 5b27 7573 6572  end(result['user
-0002bb30: 6461 7461 275d 290a 2020 2020 2020 2020  data']).        
-0002bb40: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0002bb50: 2020 2020 2020 2020 2020 6572 726f 7228            error(
-0002bb60: 7265 7375 6c74 5b27 7265 6173 6f6e 275d  result['reason']
-0002bb70: 290a 2020 2020 2020 2020 6966 206e 6f74  ).        if not
-0002bb80: 2061 7379 6e63 7761 6974 3a0a 2020 2020   asyncwait:.    
-0002bb90: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
-0002bba0: 2020 2020 2020 2065 6c69 6620 6e6f 7420         elif not 
-0002bbb0: 7374 6172 7420 6f72 206e 6f74 2063 6c6f  start or not clo
-0002bbc0: 7564 696e 6974 206f 7220 7072 6f66 696c  udinit or profil
-0002bbd0: 652e 6765 7428 2769 6d61 6765 2729 2069  e.get('image') i
-0002bbe0: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-0002bbf0: 2020 2020 7070 7269 6e74 2866 2253 6b69      pprint(f"Ski
-0002bc00: 7070 696e 6720 7761 6974 206f 6e20 7b6e  pping wait on {n
-0002bc10: 616d 657d 2229 0a20 2020 2020 2020 2065  ame}").        e
-0002bc20: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0002bc30: 2077 6169 7463 6f6d 6d61 6e64 203d 2070   waitcommand = p
-0002bc40: 726f 6669 6c65 2e67 6574 2827 7761 6974  rofile.get('wait
-0002bc50: 636f 6d6d 616e 6427 290a 2020 2020 2020  command').      
-0002bc60: 2020 2020 2020 7761 6974 7469 6d65 6f75        waittimeou
-0002bc70: 7420 3d20 7072 6f66 696c 652e 6765 7428  t = profile.get(
-0002bc80: 2777 6169 7474 696d 656f 7574 272c 2030  'waittimeout', 0
-0002bc90: 290a 2020 2020 2020 2020 2020 2020 6173  ).            as
-0002bca0: 796e 6377 6169 7476 6d20 3d20 7b27 6e61  yncwaitvm = {'na
-0002bcb0: 6d65 273a 206e 616d 652c 2027 6669 6e69  me': name, 'fini
-0002bcc0: 7368 6669 6c65 7327 3a20 6669 6e69 7368  shfiles': finish
-0002bcd0: 6669 6c65 732c 2027 7761 6974 636f 6d6d  files, 'waitcomm
-0002bce0: 616e 6427 3a20 7761 6974 636f 6d6d 616e  and': waitcomman
-0002bcf0: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
-0002bd00: 2020 2020 2020 2020 2020 2020 2020 2777                'w
-0002bd10: 6169 7474 696d 656f 7574 273a 2077 6169  aittimeout': wai
-0002bd20: 7474 696d 656f 7574 2c20 2776 6d63 6c69  ttimeout, 'vmcli
-0002bd30: 656e 7427 3a20 766d 636c 6965 6e74 7d0a  ent': vmclient}.
-0002bd40: 2020 2020 2020 2020 2020 2020 6173 796e              asyn
-0002bd50: 6377 6169 7476 6d73 2e61 7070 656e 6428  cwaitvms.append(
-0002bd60: 6173 796e 6377 6169 7476 6d29 0a0a 2020  asyncwaitvm)..  
-0002bd70: 2020 6465 6620 7468 7265 6164 6564 5f63    def threaded_c
-0002bd80: 7265 6174 655f 766d 2873 656c 662c 206e  reate_vm(self, n
-0002bd90: 616d 652c 2070 726f 6669 6c65 6e61 6d65  ame, profilename
-0002bda0: 2c20 6375 7272 656e 746f 7665 7272 6964  , currentoverrid
-0002bdb0: 6573 2c20 7072 6f66 696c 652c 207a 2c20  es, profile, z, 
-0002bdc0: 706c 616e 2c20 6375 7272 656e 7470 6c61  plan, currentpla
-0002bdd0: 6e64 6972 2c20 766d 636c 6965 6e74 2c0a  ndir, vmclient,.
+0002b930: 2020 2020 2020 766d 636c 6965 6e74 3d4e        vmclient=N
+0002b940: 6f6e 6529 3a0a 2020 2020 2020 2020 6966  one):.        if
+0002b950: 2027 7265 7375 6c74 2720 696e 2072 6573   'result' in res
+0002b960: 756c 7420 616e 6420 7265 7375 6c74 5b27  ult and result['
+0002b970: 7265 7375 6c74 275d 203d 3d20 2773 7563  result'] == 'suc
+0002b980: 6365 7373 273a 0a20 2020 2020 2020 2020  cess':.         
+0002b990: 2020 206e 6577 766d 732e 6170 7065 6e64     newvms.append
+0002b9a0: 286e 616d 6529 0a20 2020 2020 2020 2065  (name).        e
+0002b9b0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+0002b9c0: 2066 6169 6c65 6476 6d73 2e61 7070 656e   failedvms.appen
+0002b9d0: 6428 7b27 6e61 6d65 273a 206e 616d 652c  d({'name': name,
+0002b9e0: 2027 7265 6173 6f6e 273a 2072 6573 756c   'reason': resul
+0002b9f0: 745b 2772 6561 736f 6e27 5d7d 290a 2020  t['reason']}).  
+0002ba00: 2020 2020 2020 7374 6172 7420 3d20 7072        start = pr
+0002ba10: 6f66 696c 652e 6765 7428 2773 7461 7274  ofile.get('start
+0002ba20: 272c 2054 7275 6529 0a20 2020 2020 2020  ', True).       
+0002ba30: 2063 6c6f 7564 696e 6974 203d 2070 726f   cloudinit = pro
+0002ba40: 6669 6c65 2e67 6574 2827 636c 6f75 6469  file.get('cloudi
+0002ba50: 6e69 7427 2c20 5472 7565 290a 2020 2020  nit', True).    
+0002ba60: 2020 2020 6173 796e 6377 6169 7420 3d20      asyncwait = 
+0002ba70: 7072 6f66 696c 652e 6765 7428 2761 7379  profile.get('asy
+0002ba80: 6e63 7761 6974 272c 2046 616c 7365 290a  ncwait', False).
+0002ba90: 2020 2020 2020 2020 6669 6e69 7368 6669          finishfi
+0002baa0: 6c65 7320 3d20 7072 6f66 696c 652e 6765  les = profile.ge
+0002bab0: 7428 2766 696e 6973 6866 696c 6573 272c  t('finishfiles',
+0002bac0: 205b 5d29 0a20 2020 2020 2020 2069 6620   []).        if 
+0002bad0: 6f6e 6c79 6173 7365 7473 3a0a 2020 2020  onlyassets:.    
+0002bae0: 2020 2020 2020 2020 6966 2027 7573 6572          if 'user
+0002baf0: 6461 7461 2720 696e 2072 6573 756c 743a  data' in result:
+0002bb00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002bb10: 206e 6577 6173 7365 7473 2e61 7070 656e   newassets.appen
+0002bb20: 6428 7265 7375 6c74 5b27 7573 6572 6461  d(result['userda
+0002bb30: 7461 275d 290a 2020 2020 2020 2020 2020  ta']).          
+0002bb40: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0002bb50: 2020 2020 2020 2020 6572 726f 7228 7265          error(re
+0002bb60: 7375 6c74 5b27 7265 6173 6f6e 275d 290a  sult['reason']).
+0002bb70: 2020 2020 2020 2020 6966 206e 6f74 2061          if not a
+0002bb80: 7379 6e63 7761 6974 3a0a 2020 2020 2020  syncwait:.      
+0002bb90: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
+0002bba0: 2020 2020 2065 6c69 6620 6e6f 7420 7374       elif not st
+0002bbb0: 6172 7420 6f72 206e 6f74 2063 6c6f 7564  art or not cloud
+0002bbc0: 696e 6974 206f 7220 7072 6f66 696c 652e  init or profile.
+0002bbd0: 6765 7428 2769 6d61 6765 2729 2069 7320  get('image') is 
+0002bbe0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0002bbf0: 2020 7070 7269 6e74 2866 2253 6b69 7070    pprint(f"Skipp
+0002bc00: 696e 6720 7761 6974 206f 6e20 7b6e 616d  ing wait on {nam
+0002bc10: 657d 2229 0a20 2020 2020 2020 2065 6c73  e}").        els
+0002bc20: 653a 0a20 2020 2020 2020 2020 2020 2077  e:.            w
+0002bc30: 6169 7463 6f6d 6d61 6e64 203d 2070 726f  aitcommand = pro
+0002bc40: 6669 6c65 2e67 6574 2827 7761 6974 636f  file.get('waitco
+0002bc50: 6d6d 616e 6427 290a 2020 2020 2020 2020  mmand').        
+0002bc60: 2020 2020 7761 6974 7469 6d65 6f75 7420      waittimeout 
+0002bc70: 3d20 7072 6f66 696c 652e 6765 7428 2777  = profile.get('w
+0002bc80: 6169 7474 696d 656f 7574 272c 2030 290a  aittimeout', 0).
+0002bc90: 2020 2020 2020 2020 2020 2020 6173 796e              asyn
+0002bca0: 6377 6169 7476 6d20 3d20 7b27 6e61 6d65  cwaitvm = {'name
+0002bcb0: 273a 206e 616d 652c 2027 6669 6e69 7368  ': name, 'finish
+0002bcc0: 6669 6c65 7327 3a20 6669 6e69 7368 6669  files': finishfi
+0002bcd0: 6c65 732c 2027 7761 6974 636f 6d6d 616e  les, 'waitcomman
+0002bce0: 6427 3a20 7761 6974 636f 6d6d 616e 642c  d': waitcommand,
+0002bcf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002bd00: 2020 2020 2020 2020 2020 2020 2777 6169              'wai
+0002bd10: 7474 696d 656f 7574 273a 2077 6169 7474  ttimeout': waitt
+0002bd20: 696d 656f 7574 2c20 2776 6d63 6c69 656e  imeout, 'vmclien
+0002bd30: 7427 3a20 766d 636c 6965 6e74 7d0a 2020  t': vmclient}.  
+0002bd40: 2020 2020 2020 2020 2020 6173 796e 6377            asyncw
+0002bd50: 6169 7476 6d73 2e61 7070 656e 6428 6173  aitvms.append(as
+0002bd60: 796e 6377 6169 7476 6d29 0a0a 2020 2020  yncwaitvm)..    
+0002bd70: 6465 6620 7468 7265 6164 6564 5f63 7265  def threaded_cre
+0002bd80: 6174 655f 766d 2873 656c 662c 206e 616d  ate_vm(self, nam
+0002bd90: 652c 2070 726f 6669 6c65 6e61 6d65 2c20  e, profilename, 
+0002bda0: 6375 7272 656e 746f 7665 7272 6964 6573  currentoverrides
+0002bdb0: 2c20 7072 6f66 696c 652c 207a 2c20 706c  , profile, z, pl
+0002bdc0: 616e 2c20 6375 7272 656e 7470 6c61 6e64  an, currentpland
+0002bdd0: 6972 2c20 766d 636c 6965 6e74 2c0a 2020  ir, vmclient,.  
 0002bde0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002bdf0: 2020 2020 2020 2020 2020 206f 6e66 6c79             onfly
-0002be00: 2c20 6f6e 6c79 6173 7365 7473 2c20 6e65  , onlyassets, ne
-0002be10: 7776 6d73 2c20 6661 696c 6564 766d 732c  wvms, failedvms,
-0002be20: 2061 7379 6e63 7761 6974 766d 732c 206e   asyncwaitvms, n
-0002be30: 6577 6173 7365 7473 293a 0a20 2020 2020  ewassets):.     
-0002be40: 2020 2072 6573 756c 7420 3d20 7365 6c66     result = self
-0002be50: 2e63 7265 6174 655f 766d 286e 616d 652c  .create_vm(name,
-0002be60: 2070 726f 6669 6c65 6e61 6d65 2c20 6f76   profilename, ov
-0002be70: 6572 7269 6465 733d 6375 7272 656e 746f  errides=currento
-0002be80: 7665 7272 6964 6573 2c20 6375 7374 6f6d  verrides, custom
-0002be90: 7072 6f66 696c 653d 7072 6f66 696c 652c  profile=profile,
-0002bea0: 206b 3d7a 2c0a 2020 2020 2020 2020 2020   k=z,.          
+0002bdf0: 2020 2020 2020 2020 206f 6e66 6c79 2c20           onfly, 
+0002be00: 6f6e 6c79 6173 7365 7473 2c20 6e65 7776  onlyassets, newv
+0002be10: 6d73 2c20 6661 696c 6564 766d 732c 2061  ms, failedvms, a
+0002be20: 7379 6e63 7761 6974 766d 732c 206e 6577  syncwaitvms, new
+0002be30: 6173 7365 7473 293a 0a20 2020 2020 2020  assets):.       
+0002be40: 2072 6573 756c 7420 3d20 7365 6c66 2e63   result = self.c
+0002be50: 7265 6174 655f 766d 286e 616d 652c 2070  reate_vm(name, p
+0002be60: 726f 6669 6c65 6e61 6d65 2c20 6f76 6572  rofilename, over
+0002be70: 7269 6465 733d 6375 7272 656e 746f 7665  rides=currentove
+0002be80: 7272 6964 6573 2c20 6375 7374 6f6d 7072  rrides, custompr
+0002be90: 6f66 696c 653d 7072 6f66 696c 652c 206b  ofile=profile, k
+0002bea0: 3d7a 2c0a 2020 2020 2020 2020 2020 2020  =z,.            
 0002beb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002bec0: 2020 2020 2020 706c 616e 3d70 6c61 6e2c        plan=plan,
-0002bed0: 2062 6173 6564 6972 3d63 7572 7265 6e74   basedir=current
-0002bee0: 706c 616e 6469 722c 2063 6c69 656e 743d  plandir, client=
-0002bef0: 766d 636c 6965 6e74 2c20 6f6e 666c 793d  vmclient, onfly=
-0002bf00: 6f6e 666c 792c 0a20 2020 2020 2020 2020  onfly,.         
+0002bec0: 2020 2020 706c 616e 3d70 6c61 6e2c 2062      plan=plan, b
+0002bed0: 6173 6564 6972 3d63 7572 7265 6e74 706c  asedir=currentpl
+0002bee0: 616e 6469 722c 2063 6c69 656e 743d 766d  andir, client=vm
+0002bef0: 636c 6965 6e74 2c20 6f6e 666c 793d 6f6e  client, onfly=on
+0002bf00: 666c 792c 0a20 2020 2020 2020 2020 2020  fly,.           
 0002bf10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002bf20: 2020 2020 2020 206f 6e6c 7961 7373 6574         onlyasset
-0002bf30: 733d 6f6e 6c79 6173 7365 7473 290a 2020  s=onlyassets).  
-0002bf40: 2020 2020 2020 6966 206e 6f74 206f 6e6c        if not onl
-0002bf50: 7961 7373 6574 733a 0a20 2020 2020 2020  yassets:.       
-0002bf60: 2020 2020 2063 6f6d 6d6f 6e2e 6861 6e64       common.hand
-0002bf70: 6c65 5f72 6573 706f 6e73 6528 7265 7375  le_response(resu
-0002bf80: 6c74 2c20 6e61 6d65 2c20 636c 6965 6e74  lt, name, client
-0002bf90: 3d76 6d63 6c69 656e 7429 0a20 2020 2020  =vmclient).     
-0002bfa0: 2020 2073 656c 662e 6861 6e64 6c65 5f76     self.handle_v
-0002bfb0: 6d5f 7265 7375 6c74 286e 616d 652c 2070  m_result(name, p
-0002bfc0: 726f 6669 6c65 2c20 7265 7375 6c74 3d72  rofile, result=r
-0002bfd0: 6573 756c 742c 206e 6577 766d 733d 6e65  esult, newvms=ne
-0002bfe0: 7776 6d73 2c20 6661 696c 6564 766d 733d  wvms, failedvms=
-0002bff0: 6661 696c 6564 766d 732c 0a20 2020 2020  failedvms,.     
+0002bf20: 2020 2020 206f 6e6c 7961 7373 6574 733d       onlyassets=
+0002bf30: 6f6e 6c79 6173 7365 7473 290a 2020 2020  onlyassets).    
+0002bf40: 2020 2020 6966 206e 6f74 206f 6e6c 7961      if not onlya
+0002bf50: 7373 6574 733a 0a20 2020 2020 2020 2020  ssets:.         
+0002bf60: 2020 2063 6f6d 6d6f 6e2e 6861 6e64 6c65     common.handle
+0002bf70: 5f72 6573 706f 6e73 6528 7265 7375 6c74  _response(result
+0002bf80: 2c20 6e61 6d65 2c20 636c 6965 6e74 3d76  , name, client=v
+0002bf90: 6d63 6c69 656e 7429 0a20 2020 2020 2020  mclient).       
+0002bfa0: 2073 656c 662e 6861 6e64 6c65 5f76 6d5f   self.handle_vm_
+0002bfb0: 7265 7375 6c74 286e 616d 652c 2070 726f  result(name, pro
+0002bfc0: 6669 6c65 2c20 7265 7375 6c74 3d72 6573  file, result=res
+0002bfd0: 756c 742c 206e 6577 766d 733d 6e65 7776  ult, newvms=newv
+0002bfe0: 6d73 2c20 6661 696c 6564 766d 733d 6661  ms, failedvms=fa
+0002bff0: 696c 6564 766d 732c 0a20 2020 2020 2020  iledvms,.       
 0002c000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c010: 2020 2020 2020 2020 2061 7379 6e63 7761           asyncwa
-0002c020: 6974 766d 733d 6173 796e 6377 6169 7476  itvms=asyncwaitv
-0002c030: 6d73 2c20 6f6e 6c79 6173 7365 7473 3d6f  ms, onlyassets=o
-0002c040: 6e6c 7961 7373 6574 732c 206e 6577 6173  nlyassets, newas
-0002c050: 7365 7473 3d6e 6577 6173 7365 7473 2c20  sets=newassets, 
-0002c060: 766d 636c 6965 6e74 3d76 6d63 6c69 656e  vmclient=vmclien
-0002c070: 7429 0a0a 2020 2020 6465 6620 7061 7273  t)..    def pars
-0002c080: 655f 6669 6c65 7328 7365 6c66 2c20 6e61  e_files(self, na
-0002c090: 6d65 2c20 6669 6c65 732c 2062 6173 6564  me, files, based
-0002c0a0: 6972 3d27 2e27 2c20 6f6e 666c 793d 4e6f  ir='.', onfly=No
-0002c0b0: 6e65 293a 0a20 2020 2020 2020 2069 6620  ne):.        if 
-0002c0c0: 6e6f 7420 6669 6c65 733a 0a20 2020 2020  not files:.     
-0002c0d0: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
-0002c0e0: 2020 2020 2020 666f 7220 696e 6465 782c        for index,
-0002c0f0: 2066 696c 2069 6e20 656e 756d 6572 6174   fil in enumerat
-0002c100: 6528 6669 6c65 7329 3a0a 2020 2020 2020  e(files):.      
-0002c110: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
-0002c120: 6e63 6528 6669 6c2c 2073 7472 293a 0a20  nce(fil, str):. 
-0002c130: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-0002c140: 6174 6820 3d20 6622 2f72 6f6f 742f 7b66  ath = f"/root/{f
-0002c150: 696c 7d22 0a20 2020 2020 2020 2020 2020  il}".           
-0002c160: 2020 2020 2069 6620 6261 7365 6469 7220       if basedir 
-0002c170: 213d 2027 2e27 3a0a 2020 2020 2020 2020  != '.':.        
-0002c180: 2020 2020 2020 2020 2020 2020 6f72 6967              orig
-0002c190: 696e 203d 2066 227b 6261 7365 6469 727d  in = f"{basedir}
-0002c1a0: 2f7b 7061 7468 7d22 0a20 2020 2020 2020  /{path}".       
-0002c1b0: 2020 2020 2020 2020 206f 7269 6769 6e20           origin 
-0002c1c0: 3d20 6669 6c0a 2020 2020 2020 2020 2020  = fil.          
-0002c1d0: 2020 2020 2020 636f 6e74 656e 7420 3d20        content = 
-0002c1e0: 4e6f 6e65 0a20 2020 2020 2020 2020 2020  None.           
-0002c1f0: 2020 2020 2066 696c 6573 5b69 6e64 6578       files[index
-0002c200: 5d20 3d20 7b27 7061 7468 273a 2070 6174  ] = {'path': pat
-0002c210: 682c 2027 6f72 6967 696e 273a 206f 7269  h, 'origin': ori
-0002c220: 6769 6e7d 0a20 2020 2020 2020 2020 2020  gin}.           
-0002c230: 2065 6c69 6620 6973 696e 7374 616e 6365   elif isinstance
-0002c240: 2866 696c 2c20 6469 6374 293a 0a20 2020  (fil, dict):.   
-0002c250: 2020 2020 2020 2020 2020 2020 206f 7269               ori
-0002c260: 6769 6e20 3d20 6669 6c2e 6765 7428 276f  gin = fil.get('o
-0002c270: 7269 6769 6e27 290a 2020 2020 2020 2020  rigin').        
-0002c280: 2020 2020 2020 2020 636f 6e74 656e 7420          content 
-0002c290: 3d20 6669 6c2e 6765 7428 2763 6f6e 7465  = fil.get('conte
-0002c2a0: 6e74 2729 0a20 2020 2020 2020 2020 2020  nt').           
-0002c2b0: 2020 2020 2070 6174 6820 3d20 6669 6c2e       path = fil.
-0002c2c0: 6765 7428 2770 6174 6827 290a 2020 2020  get('path').    
-0002c2d0: 2020 2020 2020 2020 2020 2020 6966 2070              if p
-0002c2e0: 6174 6820 6973 204e 6f6e 653a 0a20 2020  ath is None:.   
-0002c2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c300: 2069 6620 6f72 6967 696e 2069 7320 6e6f   if origin is no
-0002c310: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0002c320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c330: 6669 6c65 735b 696e 6465 785d 5b27 7061  files[index]['pa
-0002c340: 7468 275d 203d 2066 222f 726f 6f74 2f7b  th'] = f"/root/{
-0002c350: 6f72 6967 696e 7d22 0a20 2020 2020 2020  origin}".       
-0002c360: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-0002c370: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0002c380: 2020 2020 2020 2020 2020 2065 7272 6f72             error
-0002c390: 2866 2249 6e63 6f72 7265 6374 2065 6e74  (f"Incorrect ent
-0002c3a0: 7279 207b 6669 6c7d 2e4c 6561 7669 6e67  ry {fil}.Leaving
-0002c3b0: 2e2e 2e22 290a 2020 2020 2020 2020 2020  ...").          
-0002c3c0: 2020 2020 2020 2020 2020 2020 2020 7379                sy
-0002c3d0: 732e 6578 6974 2831 290a 2020 2020 2020  s.exit(1).      
-0002c3e0: 2020 2020 2020 2020 2020 656c 6966 206e            elif n
-0002c3f0: 6f74 2070 6174 682e 7374 6172 7473 7769  ot path.startswi
-0002c400: 7468 2827 2f27 293a 0a20 2020 2020 2020  th('/'):.       
-0002c410: 2020 2020 2020 2020 2020 2020 2065 7272               err
-0002c420: 6f72 2866 2249 6e63 6f72 7265 6374 2070  or(f"Incorrect p
-0002c430: 6174 6820 7b70 6174 687d 2e4c 6561 7669  ath {path}.Leavi
-0002c440: 6e67 2e2e 2e22 290a 2020 2020 2020 2020  ng...").        
-0002c450: 2020 2020 2020 2020 2020 2020 7379 732e              sys.
-0002c460: 6578 6974 2831 290a 2020 2020 2020 2020  exit(1).        
-0002c470: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0002c480: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0002c490: 207b 2772 6573 756c 7427 3a20 2766 6169   {'result': 'fai
-0002c4a0: 6c75 7265 272c 2027 7265 6173 6f6e 273a  lure', 'reason':
-0002c4b0: 2022 496e 636f 7272 6563 7420 6669 6c65   "Incorrect file
-0002c4c0: 2065 6e74 7279 227d 0a20 2020 2020 2020   entry"}.       
-0002c4d0: 2020 2020 2069 6620 6f72 6967 696e 2069       if origin i
-0002c4e0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0002c4f0: 2020 2020 2020 2020 2020 2020 6966 206f              if o
-0002c500: 6e66 6c79 2069 7320 6e6f 7420 4e6f 6e65  nfly is not None
-0002c510: 2061 6e64 2027 7e27 206e 6f74 2069 6e20   and '~' not in 
-0002c520: 6f72 6967 696e 3a0a 2020 2020 2020 2020  origin:.        
-0002c530: 2020 2020 2020 2020 2020 2020 6465 7374              dest
-0002c540: 6469 7220 3d20 6261 7365 6469 720a 2020  dir = basedir.  
+0002c010: 2020 2020 2020 2061 7379 6e63 7761 6974         asyncwait
+0002c020: 766d 733d 6173 796e 6377 6169 7476 6d73  vms=asyncwaitvms
+0002c030: 2c20 6f6e 6c79 6173 7365 7473 3d6f 6e6c  , onlyassets=onl
+0002c040: 7961 7373 6574 732c 206e 6577 6173 7365  yassets, newasse
+0002c050: 7473 3d6e 6577 6173 7365 7473 2c20 766d  ts=newassets, vm
+0002c060: 636c 6965 6e74 3d76 6d63 6c69 656e 7429  client=vmclient)
+0002c070: 0a0a 2020 2020 6465 6620 7061 7273 655f  ..    def parse_
+0002c080: 6669 6c65 7328 7365 6c66 2c20 6e61 6d65  files(self, name
+0002c090: 2c20 6669 6c65 732c 2062 6173 6564 6972  , files, basedir
+0002c0a0: 3d27 2e27 2c20 6f6e 666c 793d 4e6f 6e65  ='.', onfly=None
+0002c0b0: 293a 0a20 2020 2020 2020 2069 6620 6e6f  ):.        if no
+0002c0c0: 7420 6669 6c65 733a 0a20 2020 2020 2020  t files:.       
+0002c0d0: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
+0002c0e0: 2020 2020 666f 7220 696e 6465 782c 2066      for index, f
+0002c0f0: 696c 2069 6e20 656e 756d 6572 6174 6528  il in enumerate(
+0002c100: 6669 6c65 7329 3a0a 2020 2020 2020 2020  files):.        
+0002c110: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
+0002c120: 6528 6669 6c2c 2073 7472 293a 0a20 2020  e(fil, str):.   
+0002c130: 2020 2020 2020 2020 2020 2020 2070 6174               pat
+0002c140: 6820 3d20 6622 2f72 6f6f 742f 7b66 696c  h = f"/root/{fil
+0002c150: 7d22 0a20 2020 2020 2020 2020 2020 2020  }".             
+0002c160: 2020 2069 6620 6261 7365 6469 7220 213d     if basedir !=
+0002c170: 2027 2e27 3a0a 2020 2020 2020 2020 2020   '.':.          
+0002c180: 2020 2020 2020 2020 2020 6f72 6967 696e            origin
+0002c190: 203d 2066 227b 6261 7365 6469 727d 2f7b   = f"{basedir}/{
+0002c1a0: 7061 7468 7d22 0a20 2020 2020 2020 2020  path}".         
+0002c1b0: 2020 2020 2020 206f 7269 6769 6e20 3d20         origin = 
+0002c1c0: 6669 6c0a 2020 2020 2020 2020 2020 2020  fil.            
+0002c1d0: 2020 2020 636f 6e74 656e 7420 3d20 4e6f      content = No
+0002c1e0: 6e65 0a20 2020 2020 2020 2020 2020 2020  ne.             
+0002c1f0: 2020 2066 696c 6573 5b69 6e64 6578 5d20     files[index] 
+0002c200: 3d20 7b27 7061 7468 273a 2070 6174 682c  = {'path': path,
+0002c210: 2027 6f72 6967 696e 273a 206f 7269 6769   'origin': origi
+0002c220: 6e7d 0a20 2020 2020 2020 2020 2020 2065  n}.            e
+0002c230: 6c69 6620 6973 696e 7374 616e 6365 2866  lif isinstance(f
+0002c240: 696c 2c20 6469 6374 293a 0a20 2020 2020  il, dict):.     
+0002c250: 2020 2020 2020 2020 2020 206f 7269 6769             origi
+0002c260: 6e20 3d20 6669 6c2e 6765 7428 276f 7269  n = fil.get('ori
+0002c270: 6769 6e27 290a 2020 2020 2020 2020 2020  gin').          
+0002c280: 2020 2020 2020 636f 6e74 656e 7420 3d20        content = 
+0002c290: 6669 6c2e 6765 7428 2763 6f6e 7465 6e74  fil.get('content
+0002c2a0: 2729 0a20 2020 2020 2020 2020 2020 2020  ').             
+0002c2b0: 2020 2070 6174 6820 3d20 6669 6c2e 6765     path = fil.ge
+0002c2c0: 7428 2770 6174 6827 290a 2020 2020 2020  t('path').      
+0002c2d0: 2020 2020 2020 2020 2020 6966 2070 6174            if pat
+0002c2e0: 6820 6973 204e 6f6e 653a 0a20 2020 2020  h is None:.     
+0002c2f0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0002c300: 6620 6f72 6967 696e 2069 7320 6e6f 7420  f origin is not 
+0002c310: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0002c320: 2020 2020 2020 2020 2020 2020 2020 6669                fi
+0002c330: 6c65 735b 696e 6465 785d 5b27 7061 7468  les[index]['path
+0002c340: 275d 203d 2066 222f 726f 6f74 2f7b 6f72  '] = f"/root/{or
+0002c350: 6967 696e 7d22 0a20 2020 2020 2020 2020  igin}".         
+0002c360: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0002c370: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002c380: 2020 2020 2020 2020 2065 7272 6f72 2866           error(f
+0002c390: 2249 6e63 6f72 7265 6374 2065 6e74 7279  "Incorrect entry
+0002c3a0: 207b 6669 6c7d 2e4c 6561 7669 6e67 2e2e   {fil}.Leaving..
+0002c3b0: 2e22 290a 2020 2020 2020 2020 2020 2020  .").            
+0002c3c0: 2020 2020 2020 2020 2020 2020 7379 732e              sys.
+0002c3d0: 6578 6974 2831 290a 2020 2020 2020 2020  exit(1).        
+0002c3e0: 2020 2020 2020 2020 656c 6966 206e 6f74          elif not
+0002c3f0: 2070 6174 682e 7374 6172 7473 7769 7468   path.startswith
+0002c400: 2827 2f27 293a 0a20 2020 2020 2020 2020  ('/'):.         
+0002c410: 2020 2020 2020 2020 2020 2065 7272 6f72             error
+0002c420: 2866 2249 6e63 6f72 7265 6374 2070 6174  (f"Incorrect pat
+0002c430: 6820 7b70 6174 687d 2e4c 6561 7669 6e67  h {path}.Leaving
+0002c440: 2e2e 2e22 290a 2020 2020 2020 2020 2020  ...").          
+0002c450: 2020 2020 2020 2020 2020 7379 732e 6578            sys.ex
+0002c460: 6974 2831 290a 2020 2020 2020 2020 2020  it(1).          
+0002c470: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0002c480: 2020 2020 2020 2020 7265 7475 726e 207b          return {
+0002c490: 2772 6573 756c 7427 3a20 2766 6169 6c75  'result': 'failu
+0002c4a0: 7265 272c 2027 7265 6173 6f6e 273a 2022  re', 'reason': "
+0002c4b0: 496e 636f 7272 6563 7420 6669 6c65 2065  Incorrect file e
+0002c4c0: 6e74 7279 227d 0a20 2020 2020 2020 2020  ntry"}.         
+0002c4d0: 2020 2069 6620 6f72 6967 696e 2069 7320     if origin is 
+0002c4e0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0002c4f0: 2020 2020 2020 2020 2020 6966 206f 6e66            if onf
+0002c500: 6c79 2069 7320 6e6f 7420 4e6f 6e65 2061  ly is not None a
+0002c510: 6e64 2027 7e27 206e 6f74 2069 6e20 6f72  nd '~' not in or
+0002c520: 6967 696e 3a0a 2020 2020 2020 2020 2020  igin:.          
+0002c530: 2020 2020 2020 2020 2020 6465 7374 6469            destdi
+0002c540: 7220 3d20 6261 7365 6469 720a 2020 2020  r = basedir.    
 0002c550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c560: 2020 6966 2027 2f27 2069 6e20 6f72 6967    if '/' in orig
-0002c570: 696e 3a0a 2020 2020 2020 2020 2020 2020  in:.            
-0002c580: 2020 2020 2020 2020 2020 2020 6465 7374              dest
-0002c590: 6469 7220 3d20 6f73 2e70 6174 682e 6469  dir = os.path.di
-0002c5a0: 726e 616d 6528 6f72 6967 696e 290a 2020  rname(origin).  
+0002c560: 6966 2027 2f27 2069 6e20 6f72 6967 696e  if '/' in origin
+0002c570: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0002c580: 2020 2020 2020 2020 2020 6465 7374 6469            destdi
+0002c590: 7220 3d20 6f73 2e70 6174 682e 6469 726e  r = os.path.dirn
+0002c5a0: 616d 6528 6f72 6967 696e 290a 2020 2020  ame(origin).    
 0002c5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c5c0: 2020 2020 2020 6f73 2e6d 616b 6564 6972        os.makedir
-0002c5d0: 7328 6465 7374 6469 722c 2065 7869 7374  s(destdir, exist
-0002c5e0: 5f6f 6b3d 5472 7565 290a 2020 2020 2020  _ok=True).      
-0002c5f0: 2020 2020 2020 2020 2020 2020 2020 636f                co
-0002c600: 6d6d 6f6e 2e66 6574 6368 2866 227b 6f6e  mmon.fetch(f"{on
-0002c610: 666c 797d 2f7b 6f72 6967 696e 7d22 2c20  fly}/{origin}", 
-0002c620: 6465 7374 6469 7229 0a20 2020 2020 2020  destdir).       
-0002c630: 2020 2020 2020 2020 206f 7269 6769 6e20           origin 
-0002c640: 3d20 6f73 2e70 6174 682e 6578 7061 6e64  = os.path.expand
-0002c650: 7573 6572 286f 7269 6769 6e29 0a20 2020  user(origin).   
-0002c660: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0002c670: 6e6f 7420 6f73 2e70 6174 682e 6973 6162  not os.path.isab
-0002c680: 7328 6f72 6967 696e 293a 0a20 2020 2020  s(origin):.     
-0002c690: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0002c6a0: 6620 6973 696e 7374 616e 6365 2866 696c  f isinstance(fil
-0002c6b0: 2c20 6469 6374 2920 616e 6420 6669 6c2e  , dict) and fil.
-0002c6c0: 6765 7428 2763 7572 7265 6e74 6469 7227  get('currentdir'
-0002c6d0: 2c20 4661 6c73 6529 3a0a 2020 2020 2020  , False):.      
+0002c5c0: 2020 2020 6f73 2e6d 616b 6564 6972 7328      os.makedirs(
+0002c5d0: 6465 7374 6469 722c 2065 7869 7374 5f6f  destdir, exist_o
+0002c5e0: 6b3d 5472 7565 290a 2020 2020 2020 2020  k=True).        
+0002c5f0: 2020 2020 2020 2020 2020 2020 636f 6d6d              comm
+0002c600: 6f6e 2e66 6574 6368 2866 227b 6f6e 666c  on.fetch(f"{onfl
+0002c610: 797d 2f7b 6f72 6967 696e 7d22 2c20 6465  y}/{origin}", de
+0002c620: 7374 6469 7229 0a20 2020 2020 2020 2020  stdir).         
+0002c630: 2020 2020 2020 206f 7269 6769 6e20 3d20         origin = 
+0002c640: 6f73 2e70 6174 682e 6578 7061 6e64 7573  os.path.expandus
+0002c650: 6572 286f 7269 6769 6e29 0a20 2020 2020  er(origin).     
+0002c660: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
+0002c670: 7420 6f73 2e70 6174 682e 6973 6162 7328  t os.path.isabs(
+0002c680: 6f72 6967 696e 293a 0a20 2020 2020 2020  origin):.       
+0002c690: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0002c6a0: 6973 696e 7374 616e 6365 2866 696c 2c20  isinstance(fil, 
+0002c6b0: 6469 6374 2920 616e 6420 6669 6c2e 6765  dict) and fil.ge
+0002c6c0: 7428 2763 7572 7265 6e74 6469 7227 2c20  t('currentdir', 
+0002c6d0: 4661 6c73 6529 3a0a 2020 2020 2020 2020  False):.        
 0002c6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c6f0: 2020 6f72 6967 696e 203d 2066 227b 6f73    origin = f"{os
-0002c700: 2e67 6574 6377 6428 297d 2f7b 6f72 6967  .getcwd()}/{orig
-0002c710: 696e 7d22 0a20 2020 2020 2020 2020 2020  in}".           
-0002c720: 2020 2020 2020 2020 2020 2020 2066 696c               fil
-0002c730: 6573 5b69 6e64 6578 5d5b 276f 7269 6769  es[index]['origi
-0002c740: 6e27 5d20 3d20 6f72 6967 696e 0a20 2020  n'] = origin.   
-0002c750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c760: 2065 6c69 6620 6261 7365 6469 7220 213d   elif basedir !=
-0002c770: 2027 2e27 2061 6e64 206e 6f74 206f 7269   '.' and not ori
-0002c780: 6769 6e2e 7374 6172 7473 7769 7468 2827  gin.startswith('
-0002c790: 2e2f 2729 2061 6e64 206e 6f74 206f 7269  ./') and not ori
-0002c7a0: 6769 6e2e 7374 6172 7473 7769 7468 2827  gin.startswith('
-0002c7b0: 2f77 6f72 6b64 6972 2f27 293a 0a20 2020  /workdir/'):.   
+0002c6f0: 6f72 6967 696e 203d 2066 227b 6f73 2e67  origin = f"{os.g
+0002c700: 6574 6377 6428 297d 2f7b 6f72 6967 696e  etcwd()}/{origin
+0002c710: 7d22 0a20 2020 2020 2020 2020 2020 2020  }".             
+0002c720: 2020 2020 2020 2020 2020 2066 696c 6573             files
+0002c730: 5b69 6e64 6578 5d5b 276f 7269 6769 6e27  [index]['origin'
+0002c740: 5d20 3d20 6f72 6967 696e 0a20 2020 2020  ] = origin.     
+0002c750: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+0002c760: 6c69 6620 6261 7365 6469 7220 213d 2027  lif basedir != '
+0002c770: 2e27 2061 6e64 206e 6f74 206f 7269 6769  .' and not origi
+0002c780: 6e2e 7374 6172 7473 7769 7468 2827 2e2f  n.startswith('./
+0002c790: 2729 2061 6e64 206e 6f74 206f 7269 6769  ') and not origi
+0002c7a0: 6e2e 7374 6172 7473 7769 7468 2827 2f77  n.startswith('/w
+0002c7b0: 6f72 6b64 6972 2f27 293a 0a20 2020 2020  orkdir/'):.     
 0002c7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c7d0: 2020 2020 206f 7269 6769 6e20 3d20 6622       origin = f"
-0002c7e0: 7b62 6173 6564 6972 7d2f 7b6f 7269 6769  {basedir}/{origi
-0002c7f0: 6e7d 220a 2020 2020 2020 2020 2020 2020  n}".            
-0002c800: 2020 2020 2020 2020 2020 2020 6669 6c65              file
-0002c810: 735b 696e 6465 785d 5b27 6f72 6967 696e  s[index]['origin
-0002c820: 275d 203d 206f 7269 6769 6e0a 2020 2020  '] = origin.    
-0002c830: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-0002c840: 6f74 206f 732e 7061 7468 2e65 7869 7374  ot os.path.exist
-0002c850: 7328 6f72 6967 696e 293a 0a20 2020 2020  s(origin):.     
-0002c860: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0002c870: 6574 7572 6e20 7b27 7265 7375 6c74 273a  eturn {'result':
-0002c880: 2027 6661 696c 7572 6527 2c20 2772 6561   'failure', 'rea
-0002c890: 736f 6e27 3a20 6622 4f72 6967 696e 2066  son': f"Origin f
-0002c8a0: 696c 6520 7b6f 7269 6769 6e7d 206e 6f74  ile {origin} not
-0002c8b0: 2066 6f75 6e64 2066 6f72 207b 6e61 6d65   found for {name
-0002c8c0: 7d22 7d0a 2020 2020 2020 2020 2020 2020  }"}.            
-0002c8d0: 656c 6966 2063 6f6e 7465 6e74 2069 7320  elif content is 
-0002c8e0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0002c8f0: 2020 2020 2020 7265 7475 726e 207b 2772        return {'r
-0002c900: 6573 756c 7427 3a20 2766 6169 6c75 7265  esult': 'failure
-0002c910: 272c 2027 7265 6173 6f6e 273a 2066 2243  ', 'reason': f"C
-0002c920: 6f6e 7465 6e74 206f 6620 6669 6c65 207b  ontent of file {
-0002c930: 7061 7468 7d20 6e6f 7420 666f 756e 6420  path} not found 
-0002c940: 666f 7220 7b6e 616d 657d 227d 0a0a 2020  for {name}"}..  
-0002c950: 2020 6465 6620 7072 6570 656e 645f 696e    def prepend_in
-0002c960: 7075 745f 6469 7228 7365 6c66 2c20 6e65  put_dir(self, ne
-0002c970: 7766 696c 6573 2c20 696e 7075 7464 6972  wfiles, inputdir
-0002c980: 293a 0a20 2020 2020 2020 2072 6573 756c  ):.        resul
-0002c990: 7473 203d 205b 5d0a 2020 2020 2020 2020  ts = [].        
-0002c9a0: 666f 7220 6669 6320 696e 206e 6577 6669  for fic in newfi
-0002c9b0: 6c65 733a 0a20 2020 2020 2020 2020 2020  les:.           
-0002c9c0: 2069 6620 6973 696e 7374 616e 6365 2866   if isinstance(f
-0002c9d0: 6963 2c20 7374 7229 2061 6e64 206e 6f74  ic, str) and not
-0002c9e0: 206f 732e 7061 7468 2e69 7361 6273 2866   os.path.isabs(f
-0002c9f0: 6963 293a 0a20 2020 2020 2020 2020 2020  ic):.           
-0002ca00: 2020 2020 206e 6577 5f66 6963 203d 2066       new_fic = f
-0002ca10: 227b 696e 7075 7464 6972 7d2f 7b66 6963  "{inputdir}/{fic
-0002ca20: 7d22 0a20 2020 2020 2020 2020 2020 2065  }".            e
-0002ca30: 6c69 6620 6973 696e 7374 616e 6365 2866  lif isinstance(f
-0002ca40: 6963 2c20 6469 6374 2920 616e 6420 276f  ic, dict) and 'o
-0002ca50: 7269 6769 6e27 2069 6e20 6669 6320 616e  rigin' in fic an
-0002ca60: 6420 6e6f 7420 6f73 2e70 6174 682e 6973  d not os.path.is
-0002ca70: 6162 7328 6f73 2e70 6174 682e 6578 7061  abs(os.path.expa
-0002ca80: 6e64 7573 6572 2866 6963 5b27 6f72 6967  nduser(fic['orig
-0002ca90: 696e 275d 2929 3a0a 2020 2020 2020 2020  in'])):.        
-0002caa0: 2020 2020 2020 2020 6e65 775f 6669 6320          new_fic 
-0002cab0: 3d20 6669 632e 636f 7079 2829 0a20 2020  = fic.copy().   
-0002cac0: 2020 2020 2020 2020 2020 2020 206e 6577               new
-0002cad0: 5f66 6963 5b27 6f72 6967 696e 275d 203d  _fic['origin'] =
-0002cae0: 2066 227b 696e 7075 7464 6972 7d2f 7b66   f"{inputdir}/{f
-0002caf0: 6963 5b27 6f72 6967 696e 275d 7d22 0a20  ic['origin']}". 
-0002cb00: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-0002cb10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002cb20: 206e 6577 5f66 6963 203d 2066 6963 0a20   new_fic = fic. 
-0002cb30: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-0002cb40: 7473 2e61 7070 656e 6428 6e65 775f 6669  ts.append(new_fi
-0002cb50: 6329 0a20 2020 2020 2020 2072 6574 7572  c).        retur
-0002cb60: 6e20 7265 7375 6c74 730a 0a20 2020 2064  n results..    d
-0002cb70: 6566 2072 656d 6564 6961 7465 5f66 696c  ef remediate_fil
-0002cb80: 6573 2873 656c 662c 206e 616d 652c 206e  es(self, name, n
-0002cb90: 6577 6669 6c65 732c 206f 7665 7272 6964  ewfiles, overrid
-0002cba0: 6573 3d7b 7d2c 2069 6e70 7574 6469 723d  es={}, inputdir=
-0002cbb0: 272e 2729 3a0a 2020 2020 2020 2020 7570  '.'):.        up
-0002cbc0: 6461 7465 645f 6669 6c65 7320 3d20 5b5d  dated_files = []
-0002cbd0: 0a20 2020 2020 2020 2069 702c 2076 6d70  .        ip, vmp
-0002cbe0: 6f72 7420 3d20 5f73 7368 5f63 7265 6465  ort = _ssh_crede
-0002cbf0: 6e74 6961 6c73 2873 656c 662e 6b2c 206e  ntials(self.k, n
-0002cc00: 616d 6529 5b31 3a5d 0a20 2020 2020 2020  ame)[1:].       
-0002cc10: 2069 6620 696e 7075 7464 6972 2021 3d20   if inputdir != 
-0002cc20: 272e 273a 0a20 2020 2020 2020 2020 2020  '.':.           
-0002cc30: 206e 6577 6669 6c65 7320 3d20 7365 6c66   newfiles = self
-0002cc40: 2e70 7265 7065 6e64 5f69 6e70 7574 5f64  .prepend_input_d
-0002cc50: 6972 286e 6577 6669 6c65 732c 2069 6e70  ir(newfiles, inp
-0002cc60: 7574 6469 7229 0a20 2020 2020 2020 2073  utdir).        s
-0002cc70: 656c 662e 7061 7273 655f 6669 6c65 7328  elf.parse_files(
-0002cc80: 6e61 6d65 2c20 6e65 7766 696c 6573 290a  name, newfiles).
-0002cc90: 2020 2020 2020 2020 6f76 6572 7269 6465          override
-0002cca0: 735f 6669 6c65 7320 3d20 6f76 6572 7269  s_files = overri
-0002ccb0: 6465 732e 636f 7079 2829 0a20 2020 2020  des.copy().     
-0002ccc0: 2020 206f 7665 7272 6964 6573 5f66 696c     overrides_fil
-0002ccd0: 6573 5b27 6e61 6d65 275d 203d 206e 616d  es['name'] = nam
-0002cce0: 650a 2020 2020 2020 2020 6461 7461 203d  e.        data =
-0002ccf0: 2070 726f 6365 7373 5f66 696c 6573 2866   process_files(f
-0002cd00: 696c 6573 3d6e 6577 6669 6c65 732c 206f  iles=newfiles, o
-0002cd10: 7665 7272 6964 6573 3d6f 7665 7272 6964  verrides=overrid
-0002cd20: 6573 5f66 696c 6573 2c20 7265 6d65 6469  es_files, remedi
-0002cd30: 6174 653d 5472 7565 290a 2020 2020 2020  ate=True).      
-0002cd40: 2020 6461 7461 6469 7273 203d 207b 7d0a    datadirs = {}.
-0002cd50: 2020 2020 2020 2020 7769 7468 2054 656d          with Tem
-0002cd60: 706f 7261 7279 4469 7265 6374 6f72 7928  poraryDirectory(
-0002cd70: 2920 6173 2074 6d70 6469 723a 0a20 2020  ) as tmpdir:.   
-0002cd80: 2020 2020 2020 2020 2066 6f72 2069 6e64           for ind
-0002cd90: 6578 2c20 656e 7472 7920 696e 2065 6e75  ex, entry in enu
-0002cda0: 6d65 7261 7465 2864 6174 6129 3a0a 2020  merate(data):.  
-0002cdb0: 2020 2020 2020 2020 2020 2020 2020 6465                de
-0002cdc0: 7374 696e 6174 696f 6e20 3d20 656e 7472  stination = entr
-0002cdd0: 795b 2770 6174 6827 5d0a 2020 2020 2020  y['path'].      
-0002cde0: 2020 2020 2020 2020 2020 7061 7468 6469            pathdi
-0002cdf0: 7220 3d20 6f73 2e70 6174 682e 6469 726e  r = os.path.dirn
-0002ce00: 616d 6528 6465 7374 696e 6174 696f 6e29  ame(destination)
-0002ce10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002ce20: 2069 6620 7061 7468 6469 7220 6e6f 7420   if pathdir not 
-0002ce30: 696e 2064 6174 6164 6972 733a 0a20 2020  in datadirs:.   
-0002ce40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002ce50: 2070 6174 6864 6972 636d 6420 3d20 6627   pathdircmd = f'
-0002ce60: 6c73 202d 6120 7b70 6174 6864 6972 7d20  ls -a {pathdir} 
-0002ce70: 323e 2631 270a 2020 2020 2020 2020 2020  2>&1'.          
-0002ce80: 2020 2020 2020 2020 2020 7061 7468 6469            pathdi
-0002ce90: 7263 6d64 203d 2073 7368 286e 616d 652c  rcmd = ssh(name,
-0002cea0: 2069 703d 6970 2c20 7573 6572 3d27 726f   ip=ip, user='ro
-0002ceb0: 6f74 272c 2074 756e 6e65 6c3d 7365 6c66  ot', tunnel=self
-0002cec0: 2e74 756e 6e65 6c2c 2074 756e 6e65 6c68  .tunnel, tunnelh
-0002ced0: 6f73 743d 7365 6c66 2e74 756e 6e65 6c68  ost=self.tunnelh
-0002cee0: 6f73 742c 0a20 2020 2020 2020 2020 2020  ost,.           
+0002c7d0: 2020 206f 7269 6769 6e20 3d20 6622 7b62     origin = f"{b
+0002c7e0: 6173 6564 6972 7d2f 7b6f 7269 6769 6e7d  asedir}/{origin}
+0002c7f0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+0002c800: 2020 2020 2020 2020 2020 6669 6c65 735b            files[
+0002c810: 696e 6465 785d 5b27 6f72 6967 696e 275d  index]['origin']
+0002c820: 203d 206f 7269 6769 6e0a 2020 2020 2020   = origin.      
+0002c830: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
+0002c840: 206f 732e 7061 7468 2e65 7869 7374 7328   os.path.exists(
+0002c850: 6f72 6967 696e 293a 0a20 2020 2020 2020  origin):.       
+0002c860: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+0002c870: 7572 6e20 7b27 7265 7375 6c74 273a 2027  urn {'result': '
+0002c880: 6661 696c 7572 6527 2c20 2772 6561 736f  failure', 'reaso
+0002c890: 6e27 3a20 6622 4f72 6967 696e 2066 696c  n': f"Origin fil
+0002c8a0: 6520 7b6f 7269 6769 6e7d 206e 6f74 2066  e {origin} not f
+0002c8b0: 6f75 6e64 2066 6f72 207b 6e61 6d65 7d22  ound for {name}"
+0002c8c0: 7d0a 2020 2020 2020 2020 2020 2020 656c  }.            el
+0002c8d0: 6966 2063 6f6e 7465 6e74 2069 7320 4e6f  if content is No
+0002c8e0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0002c8f0: 2020 2020 7265 7475 726e 207b 2772 6573      return {'res
+0002c900: 756c 7427 3a20 2766 6169 6c75 7265 272c  ult': 'failure',
+0002c910: 2027 7265 6173 6f6e 273a 2066 2243 6f6e   'reason': f"Con
+0002c920: 7465 6e74 206f 6620 6669 6c65 207b 7061  tent of file {pa
+0002c930: 7468 7d20 6e6f 7420 666f 756e 6420 666f  th} not found fo
+0002c940: 7220 7b6e 616d 657d 227d 0a0a 2020 2020  r {name}"}..    
+0002c950: 6465 6620 7072 6570 656e 645f 696e 7075  def prepend_inpu
+0002c960: 745f 6469 7228 7365 6c66 2c20 6e65 7766  t_dir(self, newf
+0002c970: 696c 6573 2c20 696e 7075 7464 6972 293a  iles, inputdir):
+0002c980: 0a20 2020 2020 2020 2072 6573 756c 7473  .        results
+0002c990: 203d 205b 5d0a 2020 2020 2020 2020 666f   = [].        fo
+0002c9a0: 7220 6669 6320 696e 206e 6577 6669 6c65  r fic in newfile
+0002c9b0: 733a 0a20 2020 2020 2020 2020 2020 2069  s:.            i
+0002c9c0: 6620 6973 696e 7374 616e 6365 2866 6963  f isinstance(fic
+0002c9d0: 2c20 7374 7229 2061 6e64 206e 6f74 206f  , str) and not o
+0002c9e0: 732e 7061 7468 2e69 7361 6273 2866 6963  s.path.isabs(fic
+0002c9f0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0002ca00: 2020 206e 6577 5f66 6963 203d 2066 227b     new_fic = f"{
+0002ca10: 696e 7075 7464 6972 7d2f 7b66 6963 7d22  inputdir}/{fic}"
+0002ca20: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
+0002ca30: 6620 6973 696e 7374 616e 6365 2866 6963  f isinstance(fic
+0002ca40: 2c20 6469 6374 2920 616e 6420 276f 7269  , dict) and 'ori
+0002ca50: 6769 6e27 2069 6e20 6669 6320 616e 6420  gin' in fic and 
+0002ca60: 6e6f 7420 6f73 2e70 6174 682e 6973 6162  not os.path.isab
+0002ca70: 7328 6f73 2e70 6174 682e 6578 7061 6e64  s(os.path.expand
+0002ca80: 7573 6572 2866 6963 5b27 6f72 6967 696e  user(fic['origin
+0002ca90: 275d 2929 3a0a 2020 2020 2020 2020 2020  '])):.          
+0002caa0: 2020 2020 2020 6e65 775f 6669 6320 3d20        new_fic = 
+0002cab0: 6669 632e 636f 7079 2829 0a20 2020 2020  fic.copy().     
+0002cac0: 2020 2020 2020 2020 2020 206e 6577 5f66             new_f
+0002cad0: 6963 5b27 6f72 6967 696e 275d 203d 2066  ic['origin'] = f
+0002cae0: 227b 696e 7075 7464 6972 7d2f 7b66 6963  "{inputdir}/{fic
+0002caf0: 5b27 6f72 6967 696e 275d 7d22 0a20 2020  ['origin']}".   
+0002cb00: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+0002cb10: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+0002cb20: 6577 5f66 6963 203d 2066 6963 0a20 2020  ew_fic = fic.   
+0002cb30: 2020 2020 2020 2020 2072 6573 756c 7473           results
+0002cb40: 2e61 7070 656e 6428 6e65 775f 6669 6329  .append(new_fic)
+0002cb50: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0002cb60: 7265 7375 6c74 730a 0a20 2020 2064 6566  results..    def
+0002cb70: 2072 656d 6564 6961 7465 5f66 696c 6573   remediate_files
+0002cb80: 2873 656c 662c 206e 616d 652c 206e 6577  (self, name, new
+0002cb90: 6669 6c65 732c 206f 7665 7272 6964 6573  files, overrides
+0002cba0: 3d7b 7d2c 2069 6e70 7574 6469 723d 272e  ={}, inputdir='.
+0002cbb0: 2729 3a0a 2020 2020 2020 2020 7570 6461  '):.        upda
+0002cbc0: 7465 645f 6669 6c65 7320 3d20 5b5d 0a20  ted_files = []. 
+0002cbd0: 2020 2020 2020 2069 702c 2076 6d70 6f72         ip, vmpor
+0002cbe0: 7420 3d20 5f73 7368 5f63 7265 6465 6e74  t = _ssh_credent
+0002cbf0: 6961 6c73 2873 656c 662e 6b2c 206e 616d  ials(self.k, nam
+0002cc00: 6529 5b31 3a5d 0a20 2020 2020 2020 2069  e)[1:].        i
+0002cc10: 6620 696e 7075 7464 6972 2021 3d20 272e  f inputdir != '.
+0002cc20: 273a 0a20 2020 2020 2020 2020 2020 206e  ':.            n
+0002cc30: 6577 6669 6c65 7320 3d20 7365 6c66 2e70  ewfiles = self.p
+0002cc40: 7265 7065 6e64 5f69 6e70 7574 5f64 6972  repend_input_dir
+0002cc50: 286e 6577 6669 6c65 732c 2069 6e70 7574  (newfiles, input
+0002cc60: 6469 7229 0a20 2020 2020 2020 2073 656c  dir).        sel
+0002cc70: 662e 7061 7273 655f 6669 6c65 7328 6e61  f.parse_files(na
+0002cc80: 6d65 2c20 6e65 7766 696c 6573 290a 2020  me, newfiles).  
+0002cc90: 2020 2020 2020 6f76 6572 7269 6465 735f        overrides_
+0002cca0: 6669 6c65 7320 3d20 6f76 6572 7269 6465  files = override
+0002ccb0: 732e 636f 7079 2829 0a20 2020 2020 2020  s.copy().       
+0002ccc0: 206f 7665 7272 6964 6573 5f66 696c 6573   overrides_files
+0002ccd0: 5b27 6e61 6d65 275d 203d 206e 616d 650a  ['name'] = name.
+0002cce0: 2020 2020 2020 2020 6461 7461 203d 2070          data = p
+0002ccf0: 726f 6365 7373 5f66 696c 6573 2866 696c  rocess_files(fil
+0002cd00: 6573 3d6e 6577 6669 6c65 732c 206f 7665  es=newfiles, ove
+0002cd10: 7272 6964 6573 3d6f 7665 7272 6964 6573  rrides=overrides
+0002cd20: 5f66 696c 6573 2c20 7265 6d65 6469 6174  _files, remediat
+0002cd30: 653d 5472 7565 290a 2020 2020 2020 2020  e=True).        
+0002cd40: 6461 7461 6469 7273 203d 207b 7d0a 2020  datadirs = {}.  
+0002cd50: 2020 2020 2020 7769 7468 2054 656d 706f        with Tempo
+0002cd60: 7261 7279 4469 7265 6374 6f72 7928 2920  raryDirectory() 
+0002cd70: 6173 2074 6d70 6469 723a 0a20 2020 2020  as tmpdir:.     
+0002cd80: 2020 2020 2020 2066 6f72 2069 6e64 6578         for index
+0002cd90: 2c20 656e 7472 7920 696e 2065 6e75 6d65  , entry in enume
+0002cda0: 7261 7465 2864 6174 6129 3a0a 2020 2020  rate(data):.    
+0002cdb0: 2020 2020 2020 2020 2020 2020 6465 7374              dest
+0002cdc0: 696e 6174 696f 6e20 3d20 656e 7472 795b  ination = entry[
+0002cdd0: 2770 6174 6827 5d0a 2020 2020 2020 2020  'path'].        
+0002cde0: 2020 2020 2020 2020 7061 7468 6469 7220          pathdir 
+0002cdf0: 3d20 6f73 2e70 6174 682e 6469 726e 616d  = os.path.dirnam
+0002ce00: 6528 6465 7374 696e 6174 696f 6e29 0a20  e(destination). 
+0002ce10: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0002ce20: 6620 7061 7468 6469 7220 6e6f 7420 696e  f pathdir not in
+0002ce30: 2064 6174 6164 6972 733a 0a20 2020 2020   datadirs:.     
+0002ce40: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0002ce50: 6174 6864 6972 636d 6420 3d20 6627 6c73  athdircmd = f'ls
+0002ce60: 202d 6120 7b70 6174 6864 6972 7d20 323e   -a {pathdir} 2>
+0002ce70: 2631 270a 2020 2020 2020 2020 2020 2020  &1'.            
+0002ce80: 2020 2020 2020 2020 7061 7468 6469 7263          pathdirc
+0002ce90: 6d64 203d 2073 7368 286e 616d 652c 2069  md = ssh(name, i
+0002cea0: 703d 6970 2c20 7573 6572 3d27 726f 6f74  p=ip, user='root
+0002ceb0: 272c 2074 756e 6e65 6c3d 7365 6c66 2e74  ', tunnel=self.t
+0002cec0: 756e 6e65 6c2c 2074 756e 6e65 6c68 6f73  unnel, tunnelhos
+0002ced0: 743d 7365 6c66 2e74 756e 6e65 6c68 6f73  t=self.tunnelhos
+0002cee0: 742c 0a20 2020 2020 2020 2020 2020 2020  t,.             
 0002cef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002cf00: 2020 2020 2020 2020 2020 7475 6e6e 656c            tunnel
-0002cf10: 706f 7274 3d73 656c 662e 7475 6e6e 656c  port=self.tunnel
-0002cf20: 706f 7274 2c20 7475 6e6e 656c 7573 6572  port, tunneluser
-0002cf30: 3d73 656c 662e 7475 6e6e 656c 7573 6572  =self.tunneluser
-0002cf40: 2c20 696e 7365 6375 7265 3d54 7275 652c  , insecure=True,
-0002cf50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002cf00: 2020 2020 2020 2020 7475 6e6e 656c 706f          tunnelpo
+0002cf10: 7274 3d73 656c 662e 7475 6e6e 656c 706f  rt=self.tunnelpo
+0002cf20: 7274 2c20 7475 6e6e 656c 7573 6572 3d73  rt, tunneluser=s
+0002cf30: 656c 662e 7475 6e6e 656c 7573 6572 2c20  elf.tunneluser, 
+0002cf40: 696e 7365 6375 7265 3d54 7275 652c 0a20  insecure=True,. 
+0002cf50: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0002cf60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002cf70: 2020 2020 2020 636d 643d 7061 7468 6469        cmd=pathdi
-0002cf80: 7263 6d64 2c20 766d 706f 7274 3d76 6d70  rcmd, vmport=vmp
-0002cf90: 6f72 7429 0a20 2020 2020 2020 2020 2020  ort).           
-0002cfa0: 2020 2020 2020 2020 2070 6174 6864 6972           pathdir
-0002cfb0: 6669 6c65 7320 3d20 6f73 2e70 6f70 656e  files = os.popen
-0002cfc0: 2870 6174 6864 6972 636d 6429 2e72 6561  (pathdircmd).rea
-0002cfd0: 646c 696e 6573 2829 0a20 2020 2020 2020  dlines().       
-0002cfe0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0002cff0: 6c65 6e28 7061 7468 6469 7266 696c 6573  len(pathdirfiles
-0002d000: 2920 3d3d 2031 2061 6e64 2027 4e6f 2073  ) == 1 and 'No s
-0002d010: 7563 6820 6669 6c65 206f 7220 6469 7265  uch file or dire
-0002d020: 6374 6f72 7927 2069 6e20 7061 7468 6469  ctory' in pathdi
-0002d030: 7266 696c 6573 5b30 5d3a 0a20 2020 2020  rfiles[0]:.     
+0002cf70: 2020 2020 636d 643d 7061 7468 6469 7263      cmd=pathdirc
+0002cf80: 6d64 2c20 766d 706f 7274 3d76 6d70 6f72  md, vmport=vmpor
+0002cf90: 7429 0a20 2020 2020 2020 2020 2020 2020  t).             
+0002cfa0: 2020 2020 2020 2070 6174 6864 6972 6669         pathdirfi
+0002cfb0: 6c65 7320 3d20 6f73 2e70 6f70 656e 2870  les = os.popen(p
+0002cfc0: 6174 6864 6972 636d 6429 2e72 6561 646c  athdircmd).readl
+0002cfd0: 696e 6573 2829 0a20 2020 2020 2020 2020  ines().         
+0002cfe0: 2020 2020 2020 2020 2020 2069 6620 6c65             if le
+0002cff0: 6e28 7061 7468 6469 7266 696c 6573 2920  n(pathdirfiles) 
+0002d000: 3d3d 2031 2061 6e64 2027 4e6f 2073 7563  == 1 and 'No suc
+0002d010: 6820 6669 6c65 206f 7220 6469 7265 6374  h file or direct
+0002d020: 6f72 7927 2069 6e20 7061 7468 6469 7266  ory' in pathdirf
+0002d030: 696c 6573 5b30 5d3a 0a20 2020 2020 2020  iles[0]:.       
 0002d040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002d050: 2020 2063 7265 6174 6564 6972 636d 6420     createdircmd 
-0002d060: 3d20 6627 6d6b 6469 7220 2d70 207b 7061  = f'mkdir -p {pa
-0002d070: 7468 6469 727d 270a 2020 2020 2020 2020  thdir}'.        
-0002d080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002d090: 6372 6561 7465 6469 7263 6d64 203d 2073  createdircmd = s
-0002d0a0: 7368 286e 616d 652c 2069 703d 6970 2c20  sh(name, ip=ip, 
-0002d0b0: 7573 6572 3d27 726f 6f74 272c 2074 756e  user='root', tun
-0002d0c0: 6e65 6c3d 7365 6c66 2e74 756e 6e65 6c2c  nel=self.tunnel,
-0002d0d0: 2074 756e 6e65 6c68 6f73 743d 7365 6c66   tunnelhost=self
-0002d0e0: 2e74 756e 6e65 6c68 6f73 742c 0a20 2020  .tunnelhost,.   
+0002d050: 2063 7265 6174 6564 6972 636d 6420 3d20   createdircmd = 
+0002d060: 6627 6d6b 6469 7220 2d70 207b 7061 7468  f'mkdir -p {path
+0002d070: 6469 727d 270a 2020 2020 2020 2020 2020  dir}'.          
+0002d080: 2020 2020 2020 2020 2020 2020 2020 6372                cr
+0002d090: 6561 7465 6469 7263 6d64 203d 2073 7368  eatedircmd = ssh
+0002d0a0: 286e 616d 652c 2069 703d 6970 2c20 7573  (name, ip=ip, us
+0002d0b0: 6572 3d27 726f 6f74 272c 2074 756e 6e65  er='root', tunne
+0002d0c0: 6c3d 7365 6c66 2e74 756e 6e65 6c2c 2074  l=self.tunnel, t
+0002d0d0: 756e 6e65 6c68 6f73 743d 7365 6c66 2e74  unnelhost=self.t
+0002d0e0: 756e 6e65 6c68 6f73 742c 0a20 2020 2020  unnelhost,.     
 0002d0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0002d100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002d110: 2020 2020 2020 2020 7475 6e6e 656c 706f          tunnelpo
-0002d120: 7274 3d73 656c 662e 7475 6e6e 656c 706f  rt=self.tunnelpo
-0002d130: 7274 2c20 7475 6e6e 656c 7573 6572 3d73  rt, tunneluser=s
-0002d140: 656c 662e 7475 6e6e 656c 7573 6572 2c20  elf.tunneluser, 
-0002d150: 696e 7365 6375 7265 3d54 7275 652c 0a20  insecure=True,. 
+0002d110: 2020 2020 2020 7475 6e6e 656c 706f 7274        tunnelport
+0002d120: 3d73 656c 662e 7475 6e6e 656c 706f 7274  =self.tunnelport
+0002d130: 2c20 7475 6e6e 656c 7573 6572 3d73 656c  , tunneluser=sel
+0002d140: 662e 7475 6e6e 656c 7573 6572 2c20 696e  f.tunneluser, in
+0002d150: 7365 6375 7265 3d54 7275 652c 0a20 2020  secure=True,.   
 0002d160: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0002d170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002d180: 2020 2020 2020 2020 2020 636d 643d 6372            cmd=cr
-0002d190: 6561 7465 6469 7263 6d64 2c20 766d 706f  eatedircmd, vmpo
-0002d1a0: 7274 3d76 6d70 6f72 7429 0a20 2020 2020  rt=vmport).     
+0002d180: 2020 2020 2020 2020 636d 643d 6372 6561          cmd=crea
+0002d190: 7465 6469 7263 6d64 2c20 766d 706f 7274  tedircmd, vmport
+0002d1a0: 3d76 6d70 6f72 7429 0a20 2020 2020 2020  =vmport).       
 0002d1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002d1c0: 2020 206f 732e 706f 7065 6e28 6372 6561     os.popen(crea
-0002d1d0: 7465 6469 7263 6d64 290a 2020 2020 2020  tedircmd).      
+0002d1c0: 206f 732e 706f 7065 6e28 6372 6561 7465   os.popen(create
+0002d1d0: 6469 7263 6d64 290a 2020 2020 2020 2020  dircmd).        
 0002d1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002d1f0: 2020 7061 7468 6469 7266 696c 6573 203d    pathdirfiles =
-0002d200: 205b 5d0a 2020 2020 2020 2020 2020 2020   [].            
-0002d210: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0002d1f0: 7061 7468 6469 7266 696c 6573 203d 205b  pathdirfiles = [
+0002d200: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+0002d210: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
 0002d220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002d230: 2020 2020 2020 7061 7468 6469 7266 696c        pathdirfil
-0002d240: 6573 203d 205b 782e 7374 7269 7028 2920  es = [x.strip() 
-0002d250: 666f 7220 7820 696e 2070 6174 6864 6972  for x in pathdir
-0002d260: 6669 6c65 735d 0a20 2020 2020 2020 2020  files].         
-0002d270: 2020 2020 2020 2020 2020 2064 6174 6164             datad
-0002d280: 6972 735b 7061 7468 6469 725d 203d 2070  irs[pathdir] = p
-0002d290: 6174 6864 6972 6669 6c65 730a 2020 2020  athdirfiles.    
-0002d2a0: 2020 2020 2020 2020 2020 2020 6966 206f              if o
-0002d2b0: 732e 7061 7468 2e62 6173 656e 616d 6528  s.path.basename(
-0002d2c0: 6465 7374 696e 6174 696f 6e29 206e 6f74  destination) not
-0002d2d0: 2069 6e20 6461 7461 6469 7273 5b70 6174   in datadirs[pat
-0002d2e0: 6864 6972 5d3a 0a20 2020 2020 2020 2020  hdir]:.         
-0002d2f0: 2020 2020 2020 2020 2020 2070 7072 696e             pprin
-0002d300: 7428 6622 5570 6461 7469 6e67 207b 6465  t(f"Updating {de
-0002d310: 7374 696e 6174 696f 6e7d 2069 6e20 7b6e  stination} in {n
-0002d320: 616d 657d 2229 0a20 2020 2020 2020 2020  ame}").         
-0002d330: 2020 2020 2020 2020 2020 2073 6f75 7263             sourc
-0002d340: 6520 3d20 6622 7b74 6d70 6469 727d 2f66  e = f"{tmpdir}/f
-0002d350: 6963 7b69 6e64 6578 7d22 0a20 2020 2020  ic{index}".     
-0002d360: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-0002d370: 6974 6820 6f70 656e 2873 6f75 7263 652c  ith open(source,
-0002d380: 2027 7727 2920 6173 2066 3a0a 2020 2020   'w') as f:.    
+0002d230: 2020 2020 7061 7468 6469 7266 696c 6573      pathdirfiles
+0002d240: 203d 205b 782e 7374 7269 7028 2920 666f   = [x.strip() fo
+0002d250: 7220 7820 696e 2070 6174 6864 6972 6669  r x in pathdirfi
+0002d260: 6c65 735d 0a20 2020 2020 2020 2020 2020  les].           
+0002d270: 2020 2020 2020 2020 2064 6174 6164 6972           datadir
+0002d280: 735b 7061 7468 6469 725d 203d 2070 6174  s[pathdir] = pat
+0002d290: 6864 6972 6669 6c65 730a 2020 2020 2020  hdirfiles.      
+0002d2a0: 2020 2020 2020 2020 2020 6966 206f 732e            if os.
+0002d2b0: 7061 7468 2e62 6173 656e 616d 6528 6465  path.basename(de
+0002d2c0: 7374 696e 6174 696f 6e29 206e 6f74 2069  stination) not i
+0002d2d0: 6e20 6461 7461 6469 7273 5b70 6174 6864  n datadirs[pathd
+0002d2e0: 6972 5d3a 0a20 2020 2020 2020 2020 2020  ir]:.           
+0002d2f0: 2020 2020 2020 2020 2070 7072 696e 7428           pprint(
+0002d300: 6622 5570 6461 7469 6e67 207b 6465 7374  f"Updating {dest
+0002d310: 696e 6174 696f 6e7d 2069 6e20 7b6e 616d  ination} in {nam
+0002d320: 657d 2229 0a20 2020 2020 2020 2020 2020  e}").           
+0002d330: 2020 2020 2020 2020 2073 6f75 7263 6520           source 
+0002d340: 3d20 6622 7b74 6d70 6469 727d 2f66 6963  = f"{tmpdir}/fic
+0002d350: 7b69 6e64 6578 7d22 0a20 2020 2020 2020  {index}".       
+0002d360: 2020 2020 2020 2020 2020 2020 2077 6974               wit
+0002d370: 6820 6f70 656e 2873 6f75 7263 652c 2027  h open(source, '
+0002d380: 7727 2920 6173 2066 3a0a 2020 2020 2020  w') as f:.      
 0002d390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002d3a0: 2020 2020 662e 7772 6974 6528 656e 7472      f.write(entr
-0002d3b0: 795b 2763 6f6e 7465 6e74 275d 290a 2020  y['content']).  
+0002d3a0: 2020 662e 7772 6974 6528 656e 7472 795b    f.write(entry[
+0002d3b0: 2763 6f6e 7465 6e74 275d 290a 2020 2020  'content']).    
 0002d3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002d3d0: 2020 7363 7063 6d64 203d 2073 6370 286e    scpcmd = scp(n
-0002d3e0: 616d 652c 2069 703d 6970 2c20 7573 6572  ame, ip=ip, user
-0002d3f0: 3d27 726f 6f74 272c 2073 6f75 7263 653d  ='root', source=
-0002d400: 736f 7572 6365 2c20 6465 7374 696e 6174  source, destinat
-0002d410: 696f 6e3d 6465 7374 696e 6174 696f 6e2c  ion=destination,
-0002d420: 2074 756e 6e65 6c3d 7365 6c66 2e74 756e   tunnel=self.tun
-0002d430: 6e65 6c2c 0a20 2020 2020 2020 2020 2020  nel,.           
+0002d3d0: 7363 7063 6d64 203d 2073 6370 286e 616d  scpcmd = scp(nam
+0002d3e0: 652c 2069 703d 6970 2c20 7573 6572 3d27  e, ip=ip, user='
+0002d3f0: 726f 6f74 272c 2073 6f75 7263 653d 736f  root', source=so
+0002d400: 7572 6365 2c20 6465 7374 696e 6174 696f  urce, destinatio
+0002d410: 6e3d 6465 7374 696e 6174 696f 6e2c 2074  n=destination, t
+0002d420: 756e 6e65 6c3d 7365 6c66 2e74 756e 6e65  unnel=self.tunne
+0002d430: 6c2c 0a20 2020 2020 2020 2020 2020 2020  l,.             
 0002d440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002d450: 2020 2020 2020 7475 6e6e 656c 686f 7374        tunnelhost
-0002d460: 3d73 656c 662e 7475 6e6e 656c 686f 7374  =self.tunnelhost
-0002d470: 2c20 7475 6e6e 656c 706f 7274 3d73 656c  , tunnelport=sel
-0002d480: 662e 7475 6e6e 656c 706f 7274 2c20 7475  f.tunnelport, tu
-0002d490: 6e6e 656c 7573 6572 3d73 656c 662e 7475  nneluser=self.tu
-0002d4a0: 6e6e 656c 7573 6572 2c0a 2020 2020 2020  nneluser,.      
+0002d450: 2020 2020 7475 6e6e 656c 686f 7374 3d73      tunnelhost=s
+0002d460: 656c 662e 7475 6e6e 656c 686f 7374 2c20  elf.tunnelhost, 
+0002d470: 7475 6e6e 656c 706f 7274 3d73 656c 662e  tunnelport=self.
+0002d480: 7475 6e6e 656c 706f 7274 2c20 7475 6e6e  tunnelport, tunn
+0002d490: 656c 7573 6572 3d73 656c 662e 7475 6e6e  eluser=self.tunn
+0002d4a0: 656c 7573 6572 2c0a 2020 2020 2020 2020  eluser,.        
 0002d4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002d4c0: 2020 2020 2020 2020 2020 2064 6f77 6e6c             downl
-0002d4d0: 6f61 643d 4661 6c73 652c 2069 6e73 6563  oad=False, insec
-0002d4e0: 7572 653d 5472 7565 2c20 766d 706f 7274  ure=True, vmport
-0002d4f0: 3d76 6d70 6f72 7429 0a20 2020 2020 2020  =vmport).       
-0002d500: 2020 2020 2020 2020 2020 2020 206f 732e               os.
-0002d510: 7379 7374 656d 2873 6370 636d 6429 0a20  system(scpcmd). 
+0002d4c0: 2020 2020 2020 2020 2064 6f77 6e6c 6f61           downloa
+0002d4d0: 643d 4661 6c73 652c 2069 6e73 6563 7572  d=False, insecur
+0002d4e0: 653d 5472 7565 2c20 766d 706f 7274 3d76  e=True, vmport=v
+0002d4f0: 6d70 6f72 7429 0a20 2020 2020 2020 2020  mport).         
+0002d500: 2020 2020 2020 2020 2020 206f 732e 7379             os.sy
+0002d510: 7374 656d 2873 6370 636d 6429 0a20 2020  stem(scpcmd).   
 0002d520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002d530: 2020 2075 7064 6174 6564 5f66 696c 6573     updated_files
-0002d540: 2e61 7070 656e 6428 6465 7374 696e 6174  .append(destinat
-0002d550: 696f 6e29 0a20 2020 2020 2020 2072 6574  ion).        ret
-0002d560: 7572 6e20 7570 6461 7465 645f 6669 6c65  urn updated_file
-0002d570: 730a 0a20 2020 2064 6566 2069 6e66 6f5f  s..    def info_
-0002d580: 7370 6563 6966 6963 5f70 6c61 6e28 7365  specific_plan(se
-0002d590: 6c66 2c20 706c 616e 2c20 7175 6965 743d  lf, plan, quiet=
-0002d5a0: 4661 6c73 6529 3a0a 2020 2020 2020 2020  False):.        
-0002d5b0: 6966 206e 6f74 2071 7569 6574 3a0a 2020  if not quiet:.  
-0002d5c0: 2020 2020 2020 2020 2020 7070 7269 6e74            pprint
-0002d5d0: 2866 2250 726f 7669 6469 6e67 2069 6e66  (f"Providing inf
-0002d5e0: 6f72 6d61 7469 6f6e 2061 626f 7574 2070  ormation about p
-0002d5f0: 6c61 6e20 7b70 6c61 6e7d 2229 0a20 2020  lan {plan}").   
-0002d600: 2020 2020 206b 203d 2073 656c 662e 6b0a       k = self.k.
-0002d610: 2020 2020 2020 2020 7265 7375 6c74 7320          results 
-0002d620: 3d20 5b5d 0a20 2020 2020 2020 2066 6f72  = [].        for
-0002d630: 2076 6d20 696e 206b 2e6c 6973 7428 293a   vm in k.list():
-0002d640: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0002d650: 766d 2e67 6574 2827 706c 616e 272c 2027  vm.get('plan', '
-0002d660: 2729 203d 3d20 706c 616e 3a0a 2020 2020  ') == plan:.    
-0002d670: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-0002d680: 6c74 732e 6170 7065 6e64 2876 6d29 0a20  lts.append(vm). 
-0002d690: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-0002d6a0: 7375 6c74 730a 0a20 2020 2064 6566 2061  sults..    def a
-0002d6b0: 7574 6f73 6361 6c65 5f63 6c75 7374 6572  utoscale_cluster
-0002d6c0: 2873 656c 662c 206b 7562 652c 206b 7562  (self, kube, kub
-0002d6d0: 6574 7970 652c 2077 6f72 6b65 7273 2c20  etype, workers, 
-0002d6e0: 7468 7265 7368 6f6c 642c 2069 646c 6529  threshold, idle)
-0002d6f0: 3a0a 2020 2020 2020 2020 6966 2074 6872  :.        if thr
-0002d700: 6573 686f 6c64 203e 2039 3939 393a 0a20  eshold > 9999:. 
-0002d710: 2020 2020 2020 2020 2020 2070 7072 696e             pprin
-0002d720: 7428 6622 536b 6970 7069 6e67 2061 7574  t(f"Skipping aut
-0002d730: 6f73 6361 6c69 6e67 2075 7020 6368 6563  oscaling up chec
-0002d740: 6b73 2066 6f72 2063 6c75 7374 6572 207b  ks for cluster {
-0002d750: 6b75 6265 7d20 6173 2070 6572 2074 6872  kube} as per thr
-0002d760: 6573 686f 6c64 207b 7468 7265 7368 6f6c  eshold {threshol
-0002d770: 647d 2229 0a20 2020 2020 2020 2020 2020  d}").           
-0002d780: 2072 6574 7572 6e20 7b27 7265 7375 6c74   return {'result
-0002d790: 273a 2027 7375 6363 6573 7327 2c20 2777  ': 'success', 'w
-0002d7a0: 6f72 6b65 7273 273a 2077 6f72 6b65 7273  orkers': workers
-0002d7b0: 7d0a 2020 2020 2020 2020 6966 2069 646c  }.        if idl
-0002d7c0: 6520 3c20 313a 0a20 2020 2020 2020 2020  e < 1:.         
-0002d7d0: 2020 2070 7072 696e 7428 6622 536b 6970     pprint(f"Skip
-0002d7e0: 7069 6e67 2061 7574 6f73 6361 6c69 6e67  ping autoscaling
-0002d7f0: 2064 6f77 6e20 6368 6563 6b73 2066 6f72   down checks for
-0002d800: 2063 6c75 7374 6572 207b 6b75 6265 7d20   cluster {kube} 
-0002d810: 6173 2070 6572 2069 646c 6520 7b69 646c  as per idle {idl
-0002d820: 657d 2229 0a20 2020 2020 2020 2020 2020  e}").           
-0002d830: 2072 6574 7572 6e20 7b27 7265 7375 6c74   return {'result
-0002d840: 273a 2027 7375 6363 6573 7327 2c20 2777  ': 'success', 'w
-0002d850: 6f72 6b65 7273 273a 2077 6f72 6b65 7273  orkers': workers
-0002d860: 7d0a 2020 2020 2020 2020 7070 7269 6e74  }.        pprint
-0002d870: 2866 2243 6865 636b 696e 6720 6e6f 6e20  (f"Checking non 
-0002d880: 7363 6865 6475 6c65 6420 706f 6473 2063  scheduled pods c
-0002d890: 6f75 6e74 206f 6e20 636c 7573 7465 7220  ount on cluster 
-0002d8a0: 7b6b 7562 657d 2229 0a20 2020 2020 2020  {kube}").       
-0002d8b0: 2073 656c 6563 746f 7220 3d20 2221 6e6f   selector = "!no
-0002d8c0: 6465 2d72 6f6c 652e 6b75 6265 726e 6574  de-role.kubernet
-0002d8d0: 6573 2e69 6f2f 636f 6e74 726f 6c2d 706c  es.io/control-pl
-0002d8e0: 616e 652c 6e6f 6465 2d72 6f6c 652e 6b75  ane,node-role.ku
-0002d8f0: 6265 726e 6574 6573 2e69 6f2f 776f 726b  bernetes.io/work
-0002d900: 6572 220a 2020 2020 2020 2020 6375 7272  er".        curr
-0002d910: 656e 7463 6d64 203d 2066 226b 7562 6563  entcmd = f"kubec
-0002d920: 746c 2067 6574 206e 6f64 6520 2d2d 7365  tl get node --se
-0002d930: 6c65 6374 6f72 3d27 7b73 656c 6563 746f  lector='{selecto
-0002d940: 727d 2722 0a20 2020 2020 2020 2063 7572  r}'".        cur
-0002d950: 7265 6e74 636d 6420 2b3d 2022 207c 2067  rentcmd += " | g
-0002d960: 7265 7020 2720 5265 6164 7927 220a 2020  rep ' Ready'".  
-0002d970: 2020 2020 2020 776f 726b 6572 7320 3d20        workers = 
-0002d980: 6c65 6e28 6f73 2e70 6f70 656e 2863 7572  len(os.popen(cur
-0002d990: 7265 6e74 636d 6429 2e72 6561 646c 696e  rentcmd).readlin
-0002d9a0: 6573 2829 290a 2020 2020 2020 2020 7065  es()).        pe
-0002d9b0: 6e64 696e 6763 6d64 203d 2022 6b75 6265  ndingcmd = "kube
-0002d9c0: 6374 6c20 6765 7420 706f 6473 202d 4120  ctl get pods -A 
-0002d9d0: 2d2d 6669 656c 642d 7365 6c65 6374 6f72  --field-selector
-0002d9e0: 3d73 7461 7475 732e 7068 6173 653d 5065  =status.phase=Pe
-0002d9f0: 6e64 696e 6720 2d6f 2079 616d 6c22 0a20  nding -o yaml". 
-0002da00: 2020 2020 2020 2070 656e 6469 6e67 5f70         pending_p
-0002da10: 6f64 7320 3d20 7961 6d6c 2e73 6166 655f  ods = yaml.safe_
-0002da20: 6c6f 6164 286f 732e 706f 7065 6e28 7065  load(os.popen(pe
-0002da30: 6e64 696e 6763 6d64 292e 7265 6164 2829  ndingcmd).read()
-0002da40: 295b 2769 7465 6d73 275d 0a20 2020 2020  )['items'].     
-0002da50: 2020 2069 6620 6c65 6e28 7065 6e64 696e     if len(pendin
-0002da60: 675f 706f 6473 2920 3e20 7468 7265 7368  g_pods) > thresh
-0002da70: 6f6c 643a 0a20 2020 2020 2020 2020 2020  old:.           
-0002da80: 2070 7072 696e 7428 6622 5472 6967 6765   pprint(f"Trigge
-0002da90: 7269 6e67 2073 6361 6c69 6e67 2075 7020  ring scaling up 
-0002daa0: 666f 7220 636c 7573 7465 7220 7b6b 7562  for cluster {kub
-0002dab0: 657d 2061 7320 7468 6572 6520 6172 6520  e} as there are 
-0002dac0: 7b6c 656e 2870 656e 6469 6e67 5f70 6f64  {len(pending_pod
-0002dad0: 7329 7d20 7065 6e64 696e 6720 706f 6473  s)} pending pods
-0002dae0: 2229 0a20 2020 2020 2020 2020 2020 2077  ").            w
-0002daf0: 6f72 6b65 7273 202b 3d20 310a 2020 2020  orkers += 1.    
-0002db00: 2020 2020 2020 2020 7070 7269 6e74 2822          pprint("
-0002db10: 5363 616c 696e 6720 7570 2063 6c75 7374  Scaling up clust
-0002db20: 6572 207b 6b75 6265 7d20 746f 207b 776f  er {kube} to {wo
-0002db30: 726b 6572 737d 2077 6f72 6b65 7273 2229  rkers} workers")
-0002db40: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-0002db50: 756c 7420 3d20 7365 6c66 2e73 6361 6c65  ult = self.scale
-0002db60: 5f6b 7562 6528 6b75 6265 2c20 6b75 6265  _kube(kube, kube
-0002db70: 7479 7065 2c20 6f76 6572 7269 6465 733d  type, overrides=
-0002db80: 7b27 776f 726b 6572 7327 3a20 776f 726b  {'workers': work
-0002db90: 6572 737d 290a 2020 2020 2020 2020 2020  ers}).          
-0002dba0: 2020 7265 7375 6c74 5b27 776f 726b 6572    result['worker
-0002dbb0: 7327 5d20 3d20 776f 726b 6572 730a 2020  s'] = workers.  
-0002dbc0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0002dbd0: 2072 6573 756c 740a 2020 2020 2020 2020   result.        
-0002dbe0: 6e6f 6465 7320 3d20 7b7d 0a20 2020 2020  nodes = {}.     
-0002dbf0: 2020 2063 7572 7265 6e74 636d 6420 3d20     currentcmd = 
-0002dc00: 226b 7562 6563 746c 2067 6574 2070 6f64  "kubectl get pod
-0002dc10: 202d 4120 2d6f 2079 616d 6c22 0a20 2020   -A -o yaml".   
-0002dc20: 2020 2020 2061 6c6c 706f 6473 203d 2079       allpods = y
-0002dc30: 616d 6c2e 7361 6665 5f6c 6f61 6428 6f73  aml.safe_load(os
-0002dc40: 2e70 6f70 656e 2863 7572 7265 6e74 636d  .popen(currentcm
-0002dc50: 6429 2e72 6561 6428 2929 5b27 6974 656d  d).read())['item
-0002dc60: 7327 5d0a 2020 2020 2020 2020 666f 7220  s'].        for 
-0002dc70: 706f 6420 696e 2061 6c6c 706f 6473 3a0a  pod in allpods:.
-0002dc80: 2020 2020 2020 2020 2020 2020 6e6f 6465              node
-0002dc90: 6e61 6d65 203d 2070 6f64 5b27 7370 6563  name = pod['spec
-0002dca0: 275d 5b27 6e6f 6465 4e61 6d65 275d 0a20  ']['nodeName']. 
-0002dcb0: 2020 2020 2020 2020 2020 2073 7461 7475             statu
-0002dcc0: 7320 3d20 706f 645b 2773 7461 7475 7327  s = pod['status'
-0002dcd0: 5d5b 2770 6861 7365 275d 0a20 2020 2020  ]['phase'].     
-0002dce0: 2020 2020 2020 2069 6620 7374 6174 7573         if status
-0002dcf0: 2021 3d20 2752 756e 6e69 6e67 273a 0a20   != 'Running':. 
-0002dd00: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0002dd10: 6f6e 7469 6e75 650a 2020 2020 2020 2020  ontinue.        
-0002dd20: 2020 2020 6966 206e 6f64 656e 616d 6520      if nodename 
-0002dd30: 6e6f 7420 696e 206e 6f64 6573 3a0a 2020  not in nodes:.  
-0002dd40: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
-0002dd50: 6465 735b 6e6f 6465 6e61 6d65 5d20 3d20  des[nodename] = 
-0002dd60: 310a 2020 2020 2020 2020 2020 2020 656c  1.            el
-0002dd70: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0002dd80: 2020 2020 6e6f 6465 735b 6e6f 6465 6e61      nodes[nodena
-0002dd90: 6d65 5d20 2b3d 2031 0a20 2020 2020 2020  me] += 1.       
-0002dda0: 2074 6f64 656c 6574 6520 3d20 300a 2020   todelete = 0.  
-0002ddb0: 2020 2020 2020 666f 7220 6e6f 6465 2069        for node i
-0002ddc0: 6e20 6e6f 6465 733a 0a20 2020 2020 2020  n nodes:.       
-0002ddd0: 2020 2020 2069 6620 6e6f 6465 735b 6e6f       if nodes[no
-0002dde0: 6465 5d20 3c20 6964 6c65 3a0a 2020 2020  de] < idle:.    
-0002ddf0: 2020 2020 2020 2020 2020 2020 7070 7269              ppri
-0002de00: 6e74 2866 226e 6f64 6520 7b6e 6f64 657d  nt(f"node {node}
-0002de10: 2074 6f20 6265 2072 656d 6f76 6564 2073   to be removed s
-0002de20: 696e 6365 2069 7420 6f6e 6c79 2068 6173  ince it only has
-0002de30: 2074 6865 2066 6f6c 6c6f 7769 6e67 2070   the following p
-0002de40: 6f64 733a 207b 6e6f 6465 735b 6e6f 6465  ods: {nodes[node
-0002de50: 5d7d 2229 0a20 2020 2020 2020 2020 2020  ]}").           
-0002de60: 2020 2020 2074 6f64 656c 6574 6520 2b3d       todelete +=
-0002de70: 2031 0a20 2020 2020 2020 2069 6620 746f   1.        if to
-0002de80: 6465 6c65 7465 203e 2030 3a0a 2020 2020  delete > 0:.    
-0002de90: 2020 2020 2020 2020 7070 7269 6e74 2866          pprint(f
-0002dea0: 2254 7269 6767 6572 696e 6720 7363 616c  "Triggering scal
-0002deb0: 696e 6720 646f 776e 2066 6f72 2063 6c75  ing down for clu
-0002dec0: 7374 6572 207b 6b75 6265 7d20 6173 2074  ster {kube} as t
-0002ded0: 6865 7265 2061 7265 207b 746f 6465 6c65  here are {todele
-0002dee0: 7465 7d20 6964 6c65 206e 6f64 6573 2229  te} idle nodes")
-0002def0: 0a20 2020 2020 2020 2020 2020 2077 6f72  .            wor
-0002df00: 6b65 7273 203d 2077 6f72 6b65 7273 202d  kers = workers -
-0002df10: 2074 6f64 656c 6574 650a 2020 2020 2020   todelete.      
-0002df20: 2020 2020 2020 7070 7269 6e74 2866 2253        pprint(f"S
-0002df30: 6361 6c69 6e67 2064 6f77 6e20 636c 7573  caling down clus
-0002df40: 7465 7220 7b6b 7562 657d 2074 6f20 7b77  ter {kube} to {w
-0002df50: 6f72 6b65 7273 7d20 776f 726b 6572 7322  orkers} workers"
-0002df60: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
-0002df70: 7375 6c74 203d 2073 656c 662e 7363 616c  sult = self.scal
-0002df80: 655f 6b75 6265 286b 7562 652c 206b 7562  e_kube(kube, kub
-0002df90: 6574 7970 652c 206f 7665 7272 6964 6573  etype, overrides
-0002dfa0: 3d7b 2777 6f72 6b65 7273 273a 2077 6f72  ={'workers': wor
-0002dfb0: 6b65 7273 7d29 0a20 2020 2020 2020 2020  kers}).         
-0002dfc0: 2020 2072 6573 756c 745b 2777 6f72 6b65     result['worke
-0002dfd0: 7273 275d 203d 2077 6f72 6b65 7273 0a20  rs'] = workers. 
-0002dfe0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0002dff0: 6e20 7265 7375 6c74 0a20 2020 2020 2020  n result.       
-0002e000: 2072 6574 7572 6e20 7b27 7265 7375 6c74   return {'result
-0002e010: 273a 2027 7375 6363 6573 7327 2c20 2777  ': 'success', 'w
-0002e020: 6f72 6b65 7273 273a 2077 6f72 6b65 7273  orkers': workers
-0002e030: 7d0a 0a20 2020 2064 6566 206c 6f6f 705f  }..    def loop_
-0002e040: 6175 746f 7363 616c 655f 636c 7573 7465  autoscale_cluste
-0002e050: 7228 7365 6c66 2c20 6b75 6265 2c20 6b75  r(self, kube, ku
-0002e060: 6265 7479 7065 2c20 776f 726b 6572 732c  betype, workers,
-0002e070: 2074 6872 6573 686f 6c64 2c20 6964 6c65   threshold, idle
-0002e080: 293a 0a20 2020 2020 2020 2070 7072 696e  ):.        pprin
-0002e090: 7428 6622 5374 6172 7469 6e67 2077 6974  t(f"Starting wit
-0002e0a0: 6820 7b77 6f72 6b65 7273 7d20 776f 726b  h {workers} work
-0002e0b0: 6572 7322 290a 2020 2020 2020 2020 6966  ers").        if
-0002e0c0: 2077 6869 6368 2827 6b75 6265 6374 6c27   which('kubectl'
-0002e0d0: 2920 6973 204e 6f6e 653a 0a20 2020 2020  ) is None:.     
-0002e0e0: 2020 2020 2020 2063 6f6d 6d6f 6e2e 6765         common.ge
-0002e0f0: 745f 6b75 6265 6374 6c28 290a 2020 2020  t_kubectl().    
-0002e100: 2020 2020 2020 2020 6f73 2e65 6e76 6972          os.envir
-0002e110: 6f6e 5b27 5041 5448 275d 202b 3d20 273a  on['PATH'] += ':
-0002e120: 2e27 0a20 2020 2020 2020 2077 6869 6c65  .'.        while
-0002e130: 2054 7275 653a 0a20 2020 2020 2020 2020   True:.         
-0002e140: 2020 2073 656c 6563 746f 7220 3d20 2221     selector = "!
-0002e150: 6e6f 6465 2d72 6f6c 652e 6b75 6265 726e  node-role.kubern
-0002e160: 6574 6573 2e69 6f2f 636f 6e74 726f 6c2d  etes.io/control-
-0002e170: 706c 616e 652c 6e6f 6465 2d72 6f6c 652e  plane,node-role.
-0002e180: 6b75 6265 726e 6574 6573 2e69 6f2f 776f  kubernetes.io/wo
-0002e190: 726b 6572 220a 2020 2020 2020 2020 2020  rker".          
-0002e1a0: 2020 6375 7272 656e 7463 6d64 203d 2066    currentcmd = f
-0002e1b0: 226b 7562 6563 746c 2067 6574 206e 6f64  "kubectl get nod
-0002e1c0: 6520 2d2d 7365 6c65 6374 6f72 3d27 7b73  e --selector='{s
-0002e1d0: 656c 6563 746f 727d 2722 0a20 2020 2020  elector}'".     
-0002e1e0: 2020 2020 2020 2063 7572 7265 6e74 636d         currentcm
-0002e1f0: 6420 2b3d 2022 207c 2067 7265 7020 2720  d += " | grep ' 
-0002e200: 5265 6164 7927 220a 2020 2020 2020 2020  Ready'".        
-0002e210: 2020 2020 6375 7272 656e 746e 6f64 6573      currentnodes
-0002e220: 203d 206f 732e 706f 7065 6e28 6375 7272   = os.popen(curr
-0002e230: 656e 7463 6d64 292e 7265 6164 6c69 6e65  entcmd).readline
-0002e240: 7328 290a 2020 2020 2020 2020 2020 2020  s().            
-0002e250: 6966 206c 656e 2863 7572 7265 6e74 6e6f  if len(currentno
-0002e260: 6465 7329 2021 3d20 776f 726b 6572 733a  des) != workers:
-0002e270: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002e280: 2070 7072 696e 7428 6622 4f6e 676f 696e   pprint(f"Ongoin
-0002e290: 6720 7363 616c 696e 6720 6f70 6572 6174  g scaling operat
-0002e2a0: 696f 6e20 6f6e 2063 6c75 7374 6572 207b  ion on cluster {
-0002e2b0: 6b75 6265 7d22 290a 2020 2020 2020 2020  kube}").        
-0002e2c0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0002e2d0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-0002e2e0: 203d 2073 656c 662e 6175 746f 7363 616c   = self.autoscal
-0002e2f0: 655f 636c 7573 7465 7228 6b75 6265 2c20  e_cluster(kube, 
-0002e300: 6b75 6265 7479 7065 2c20 776f 726b 6572  kubetype, worker
-0002e310: 732c 2074 6872 6573 686f 6c64 2c20 6964  s, threshold, id
-0002e320: 6c65 290a 2020 2020 2020 2020 2020 2020  le).            
-0002e330: 2020 2020 6966 2072 6573 756c 745b 2772      if result['r
-0002e340: 6573 756c 7427 5d20 213d 2027 7375 6363  esult'] != 'succ
-0002e350: 6573 7327 3a0a 2020 2020 2020 2020 2020  ess':.          
-0002e360: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0002e370: 2072 6573 756c 740a 2020 2020 2020 2020   result.        
-0002e380: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0002d530: 2075 7064 6174 6564 5f66 696c 6573 2e61   updated_files.a
+0002d540: 7070 656e 6428 6465 7374 696e 6174 696f  ppend(destinatio
+0002d550: 6e29 0a20 2020 2020 2020 2072 6574 7572  n).        retur
+0002d560: 6e20 7570 6461 7465 645f 6669 6c65 730a  n updated_files.
+0002d570: 0a20 2020 2064 6566 2069 6e66 6f5f 7370  .    def info_sp
+0002d580: 6563 6966 6963 5f70 6c61 6e28 7365 6c66  ecific_plan(self
+0002d590: 2c20 706c 616e 2c20 7175 6965 743d 4661  , plan, quiet=Fa
+0002d5a0: 6c73 6529 3a0a 2020 2020 2020 2020 6966  lse):.        if
+0002d5b0: 206e 6f74 2071 7569 6574 3a0a 2020 2020   not quiet:.    
+0002d5c0: 2020 2020 2020 2020 7070 7269 6e74 2866          pprint(f
+0002d5d0: 2250 726f 7669 6469 6e67 2069 6e66 6f72  "Providing infor
+0002d5e0: 6d61 7469 6f6e 2061 626f 7574 2070 6c61  mation about pla
+0002d5f0: 6e20 7b70 6c61 6e7d 2229 0a20 2020 2020  n {plan}").     
+0002d600: 2020 206b 203d 2073 656c 662e 6b0a 2020     k = self.k.  
+0002d610: 2020 2020 2020 7265 7375 6c74 7320 3d20        results = 
+0002d620: 5b5d 0a20 2020 2020 2020 2066 6f72 2076  [].        for v
+0002d630: 6d20 696e 206b 2e6c 6973 7428 293a 0a20  m in k.list():. 
+0002d640: 2020 2020 2020 2020 2020 2069 6620 766d             if vm
+0002d650: 2e67 6574 2827 706c 616e 272c 2027 2729  .get('plan', '')
+0002d660: 203d 3d20 706c 616e 3a0a 2020 2020 2020   == plan:.      
+0002d670: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+0002d680: 732e 6170 7065 6e64 2876 6d29 0a20 2020  s.append(vm).   
+0002d690: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
+0002d6a0: 6c74 730a 0a20 2020 2064 6566 2061 7574  lts..    def aut
+0002d6b0: 6f73 6361 6c65 5f63 6c75 7374 6572 2873  oscale_cluster(s
+0002d6c0: 656c 662c 206b 7562 652c 206b 7562 6574  elf, kube, kubet
+0002d6d0: 7970 652c 2077 6f72 6b65 7273 2c20 7468  ype, workers, th
+0002d6e0: 7265 7368 6f6c 642c 2069 646c 6529 3a0a  reshold, idle):.
+0002d6f0: 2020 2020 2020 2020 6966 2074 6872 6573          if thres
+0002d700: 686f 6c64 203e 2039 3939 393a 0a20 2020  hold > 9999:.   
+0002d710: 2020 2020 2020 2020 2070 7072 696e 7428           pprint(
+0002d720: 6622 536b 6970 7069 6e67 2061 7574 6f73  f"Skipping autos
+0002d730: 6361 6c69 6e67 2075 7020 6368 6563 6b73  caling up checks
+0002d740: 2066 6f72 2063 6c75 7374 6572 207b 6b75   for cluster {ku
+0002d750: 6265 7d20 6173 2070 6572 2074 6872 6573  be} as per thres
+0002d760: 686f 6c64 207b 7468 7265 7368 6f6c 647d  hold {threshold}
+0002d770: 2229 0a20 2020 2020 2020 2020 2020 2072  ").            r
+0002d780: 6574 7572 6e20 7b27 7265 7375 6c74 273a  eturn {'result':
+0002d790: 2027 7375 6363 6573 7327 2c20 2777 6f72   'success', 'wor
+0002d7a0: 6b65 7273 273a 2077 6f72 6b65 7273 7d0a  kers': workers}.
+0002d7b0: 2020 2020 2020 2020 6966 2069 646c 6520          if idle 
+0002d7c0: 3c20 313a 0a20 2020 2020 2020 2020 2020  < 1:.           
+0002d7d0: 2070 7072 696e 7428 6622 536b 6970 7069   pprint(f"Skippi
+0002d7e0: 6e67 2061 7574 6f73 6361 6c69 6e67 2064  ng autoscaling d
+0002d7f0: 6f77 6e20 6368 6563 6b73 2066 6f72 2063  own checks for c
+0002d800: 6c75 7374 6572 207b 6b75 6265 7d20 6173  luster {kube} as
+0002d810: 2070 6572 2069 646c 6520 7b69 646c 657d   per idle {idle}
+0002d820: 2229 0a20 2020 2020 2020 2020 2020 2072  ").            r
+0002d830: 6574 7572 6e20 7b27 7265 7375 6c74 273a  eturn {'result':
+0002d840: 2027 7375 6363 6573 7327 2c20 2777 6f72   'success', 'wor
+0002d850: 6b65 7273 273a 2077 6f72 6b65 7273 7d0a  kers': workers}.
+0002d860: 2020 2020 2020 2020 7070 7269 6e74 2866          pprint(f
+0002d870: 2243 6865 636b 696e 6720 6e6f 6e20 7363  "Checking non sc
+0002d880: 6865 6475 6c65 6420 706f 6473 2063 6f75  heduled pods cou
+0002d890: 6e74 206f 6e20 636c 7573 7465 7220 7b6b  nt on cluster {k
+0002d8a0: 7562 657d 2229 0a20 2020 2020 2020 2073  ube}").        s
+0002d8b0: 656c 6563 746f 7220 3d20 2221 6e6f 6465  elector = "!node
+0002d8c0: 2d72 6f6c 652e 6b75 6265 726e 6574 6573  -role.kubernetes
+0002d8d0: 2e69 6f2f 636f 6e74 726f 6c2d 706c 616e  .io/control-plan
+0002d8e0: 652c 6e6f 6465 2d72 6f6c 652e 6b75 6265  e,node-role.kube
+0002d8f0: 726e 6574 6573 2e69 6f2f 776f 726b 6572  rnetes.io/worker
+0002d900: 220a 2020 2020 2020 2020 6375 7272 656e  ".        curren
+0002d910: 7463 6d64 203d 2066 226b 7562 6563 746c  tcmd = f"kubectl
+0002d920: 2067 6574 206e 6f64 6520 2d2d 7365 6c65   get node --sele
+0002d930: 6374 6f72 3d27 7b73 656c 6563 746f 727d  ctor='{selector}
+0002d940: 2722 0a20 2020 2020 2020 2063 7572 7265  '".        curre
+0002d950: 6e74 636d 6420 2b3d 2022 207c 2067 7265  ntcmd += " | gre
+0002d960: 7020 2720 5265 6164 7927 220a 2020 2020  p ' Ready'".    
+0002d970: 2020 2020 776f 726b 6572 7320 3d20 6c65      workers = le
+0002d980: 6e28 6f73 2e70 6f70 656e 2863 7572 7265  n(os.popen(curre
+0002d990: 6e74 636d 6429 2e72 6561 646c 696e 6573  ntcmd).readlines
+0002d9a0: 2829 290a 2020 2020 2020 2020 7065 6e64  ()).        pend
+0002d9b0: 696e 6763 6d64 203d 2022 6b75 6265 6374  ingcmd = "kubect
+0002d9c0: 6c20 6765 7420 706f 6473 202d 4120 2d2d  l get pods -A --
+0002d9d0: 6669 656c 642d 7365 6c65 6374 6f72 3d73  field-selector=s
+0002d9e0: 7461 7475 732e 7068 6173 653d 5065 6e64  tatus.phase=Pend
+0002d9f0: 696e 6720 2d6f 2079 616d 6c22 0a20 2020  ing -o yaml".   
+0002da00: 2020 2020 2070 656e 6469 6e67 5f70 6f64       pending_pod
+0002da10: 7320 3d20 7961 6d6c 2e73 6166 655f 6c6f  s = yaml.safe_lo
+0002da20: 6164 286f 732e 706f 7065 6e28 7065 6e64  ad(os.popen(pend
+0002da30: 696e 6763 6d64 292e 7265 6164 2829 295b  ingcmd).read())[
+0002da40: 2769 7465 6d73 275d 0a20 2020 2020 2020  'items'].       
+0002da50: 2069 6620 6c65 6e28 7065 6e64 696e 675f   if len(pending_
+0002da60: 706f 6473 2920 3e20 7468 7265 7368 6f6c  pods) > threshol
+0002da70: 643a 0a20 2020 2020 2020 2020 2020 2070  d:.            p
+0002da80: 7072 696e 7428 6622 5472 6967 6765 7269  print(f"Triggeri
+0002da90: 6e67 2073 6361 6c69 6e67 2075 7020 666f  ng scaling up fo
+0002daa0: 7220 636c 7573 7465 7220 7b6b 7562 657d  r cluster {kube}
+0002dab0: 2061 7320 7468 6572 6520 6172 6520 7b6c   as there are {l
+0002dac0: 656e 2870 656e 6469 6e67 5f70 6f64 7329  en(pending_pods)
+0002dad0: 7d20 7065 6e64 696e 6720 706f 6473 2229  } pending pods")
+0002dae0: 0a20 2020 2020 2020 2020 2020 2077 6f72  .            wor
+0002daf0: 6b65 7273 202b 3d20 310a 2020 2020 2020  kers += 1.      
+0002db00: 2020 2020 2020 7070 7269 6e74 2822 5363        pprint("Sc
+0002db10: 616c 696e 6720 7570 2063 6c75 7374 6572  aling up cluster
+0002db20: 207b 6b75 6265 7d20 746f 207b 776f 726b   {kube} to {work
+0002db30: 6572 737d 2077 6f72 6b65 7273 2229 0a20  ers} workers"). 
+0002db40: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+0002db50: 7420 3d20 7365 6c66 2e73 6361 6c65 5f6b  t = self.scale_k
+0002db60: 7562 6528 6b75 6265 2c20 6b75 6265 7479  ube(kube, kubety
+0002db70: 7065 2c20 6f76 6572 7269 6465 733d 7b27  pe, overrides={'
+0002db80: 776f 726b 6572 7327 3a20 776f 726b 6572  workers': worker
+0002db90: 737d 290a 2020 2020 2020 2020 2020 2020  s}).            
+0002dba0: 7265 7375 6c74 5b27 776f 726b 6572 7327  result['workers'
+0002dbb0: 5d20 3d20 776f 726b 6572 730a 2020 2020  ] = workers.    
+0002dbc0: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+0002dbd0: 6573 756c 740a 2020 2020 2020 2020 6e6f  esult.        no
+0002dbe0: 6465 7320 3d20 7b7d 0a20 2020 2020 2020  des = {}.       
+0002dbf0: 2063 7572 7265 6e74 636d 6420 3d20 226b   currentcmd = "k
+0002dc00: 7562 6563 746c 2067 6574 2070 6f64 202d  ubectl get pod -
+0002dc10: 4120 2d6f 2079 616d 6c22 0a20 2020 2020  A -o yaml".     
+0002dc20: 2020 2061 6c6c 706f 6473 203d 2079 616d     allpods = yam
+0002dc30: 6c2e 7361 6665 5f6c 6f61 6428 6f73 2e70  l.safe_load(os.p
+0002dc40: 6f70 656e 2863 7572 7265 6e74 636d 6429  open(currentcmd)
+0002dc50: 2e72 6561 6428 2929 5b27 6974 656d 7327  .read())['items'
+0002dc60: 5d0a 2020 2020 2020 2020 666f 7220 706f  ].        for po
+0002dc70: 6420 696e 2061 6c6c 706f 6473 3a0a 2020  d in allpods:.  
+0002dc80: 2020 2020 2020 2020 2020 6e6f 6465 6e61            nodena
+0002dc90: 6d65 203d 2070 6f64 5b27 7370 6563 275d  me = pod['spec']
+0002dca0: 5b27 6e6f 6465 4e61 6d65 275d 0a20 2020  ['nodeName'].   
+0002dcb0: 2020 2020 2020 2020 2073 7461 7475 7320           status 
+0002dcc0: 3d20 706f 645b 2773 7461 7475 7327 5d5b  = pod['status'][
+0002dcd0: 2770 6861 7365 275d 0a20 2020 2020 2020  'phase'].       
+0002dce0: 2020 2020 2069 6620 7374 6174 7573 2021       if status !
+0002dcf0: 3d20 2752 756e 6e69 6e67 273a 0a20 2020  = 'Running':.   
+0002dd00: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
+0002dd10: 7469 6e75 650a 2020 2020 2020 2020 2020  tinue.          
+0002dd20: 2020 6966 206e 6f64 656e 616d 6520 6e6f    if nodename no
+0002dd30: 7420 696e 206e 6f64 6573 3a0a 2020 2020  t in nodes:.    
+0002dd40: 2020 2020 2020 2020 2020 2020 6e6f 6465              node
+0002dd50: 735b 6e6f 6465 6e61 6d65 5d20 3d20 310a  s[nodename] = 1.
+0002dd60: 2020 2020 2020 2020 2020 2020 656c 7365              else
+0002dd70: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0002dd80: 2020 6e6f 6465 735b 6e6f 6465 6e61 6d65    nodes[nodename
+0002dd90: 5d20 2b3d 2031 0a20 2020 2020 2020 2074  ] += 1.        t
+0002dda0: 6f64 656c 6574 6520 3d20 300a 2020 2020  odelete = 0.    
+0002ddb0: 2020 2020 666f 7220 6e6f 6465 2069 6e20      for node in 
+0002ddc0: 6e6f 6465 733a 0a20 2020 2020 2020 2020  nodes:.         
+0002ddd0: 2020 2069 6620 6e6f 6465 735b 6e6f 6465     if nodes[node
+0002dde0: 5d20 3c20 6964 6c65 3a0a 2020 2020 2020  ] < idle:.      
+0002ddf0: 2020 2020 2020 2020 2020 7070 7269 6e74            pprint
+0002de00: 2866 226e 6f64 6520 7b6e 6f64 657d 2074  (f"node {node} t
+0002de10: 6f20 6265 2072 656d 6f76 6564 2073 696e  o be removed sin
+0002de20: 6365 2069 7420 6f6e 6c79 2068 6173 2074  ce it only has t
+0002de30: 6865 2066 6f6c 6c6f 7769 6e67 2070 6f64  he following pod
+0002de40: 733a 207b 6e6f 6465 735b 6e6f 6465 5d7d  s: {nodes[node]}
+0002de50: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
+0002de60: 2020 2074 6f64 656c 6574 6520 2b3d 2031     todelete += 1
+0002de70: 0a20 2020 2020 2020 2069 6620 746f 6465  .        if tode
+0002de80: 6c65 7465 203e 2030 3a0a 2020 2020 2020  lete > 0:.      
+0002de90: 2020 2020 2020 7070 7269 6e74 2866 2254        pprint(f"T
+0002dea0: 7269 6767 6572 696e 6720 7363 616c 696e  riggering scalin
+0002deb0: 6720 646f 776e 2066 6f72 2063 6c75 7374  g down for clust
+0002dec0: 6572 207b 6b75 6265 7d20 6173 2074 6865  er {kube} as the
+0002ded0: 7265 2061 7265 207b 746f 6465 6c65 7465  re are {todelete
+0002dee0: 7d20 6964 6c65 206e 6f64 6573 2229 0a20  } idle nodes"). 
+0002def0: 2020 2020 2020 2020 2020 2077 6f72 6b65             worke
+0002df00: 7273 203d 2077 6f72 6b65 7273 202d 2074  rs = workers - t
+0002df10: 6f64 656c 6574 650a 2020 2020 2020 2020  odelete.        
+0002df20: 2020 2020 7070 7269 6e74 2866 2253 6361      pprint(f"Sca
+0002df30: 6c69 6e67 2064 6f77 6e20 636c 7573 7465  ling down cluste
+0002df40: 7220 7b6b 7562 657d 2074 6f20 7b77 6f72  r {kube} to {wor
+0002df50: 6b65 7273 7d20 776f 726b 6572 7322 290a  kers} workers").
+0002df60: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+0002df70: 6c74 203d 2073 656c 662e 7363 616c 655f  lt = self.scale_
+0002df80: 6b75 6265 286b 7562 652c 206b 7562 6574  kube(kube, kubet
+0002df90: 7970 652c 206f 7665 7272 6964 6573 3d7b  ype, overrides={
+0002dfa0: 2777 6f72 6b65 7273 273a 2077 6f72 6b65  'workers': worke
+0002dfb0: 7273 7d29 0a20 2020 2020 2020 2020 2020  rs}).           
+0002dfc0: 2072 6573 756c 745b 2777 6f72 6b65 7273   result['workers
+0002dfd0: 275d 203d 2077 6f72 6b65 7273 0a20 2020  '] = workers.   
+0002dfe0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0002dff0: 7265 7375 6c74 0a20 2020 2020 2020 2072  result.        r
+0002e000: 6574 7572 6e20 7b27 7265 7375 6c74 273a  eturn {'result':
+0002e010: 2027 7375 6363 6573 7327 2c20 2777 6f72   'success', 'wor
+0002e020: 6b65 7273 273a 2077 6f72 6b65 7273 7d0a  kers': workers}.
+0002e030: 0a20 2020 2064 6566 206c 6f6f 705f 6175  .    def loop_au
+0002e040: 746f 7363 616c 655f 636c 7573 7465 7228  toscale_cluster(
+0002e050: 7365 6c66 2c20 6b75 6265 2c20 6b75 6265  self, kube, kube
+0002e060: 7479 7065 2c20 776f 726b 6572 732c 2074  type, workers, t
+0002e070: 6872 6573 686f 6c64 2c20 6964 6c65 293a  hreshold, idle):
+0002e080: 0a20 2020 2020 2020 2070 7072 696e 7428  .        pprint(
+0002e090: 6622 5374 6172 7469 6e67 2077 6974 6820  f"Starting with 
+0002e0a0: 7b77 6f72 6b65 7273 7d20 776f 726b 6572  {workers} worker
+0002e0b0: 7322 290a 2020 2020 2020 2020 6966 2077  s").        if w
+0002e0c0: 6869 6368 2827 6b75 6265 6374 6c27 2920  hich('kubectl') 
+0002e0d0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+0002e0e0: 2020 2020 2063 6f6d 6d6f 6e2e 6765 745f       common.get_
+0002e0f0: 6b75 6265 6374 6c28 290a 2020 2020 2020  kubectl().      
+0002e100: 2020 2020 2020 6f73 2e65 6e76 6972 6f6e        os.environ
+0002e110: 5b27 5041 5448 275d 202b 3d20 273a 2e27  ['PATH'] += ':.'
+0002e120: 0a20 2020 2020 2020 2077 6869 6c65 2054  .        while T
+0002e130: 7275 653a 0a20 2020 2020 2020 2020 2020  rue:.           
+0002e140: 2073 656c 6563 746f 7220 3d20 2221 6e6f   selector = "!no
+0002e150: 6465 2d72 6f6c 652e 6b75 6265 726e 6574  de-role.kubernet
+0002e160: 6573 2e69 6f2f 636f 6e74 726f 6c2d 706c  es.io/control-pl
+0002e170: 616e 652c 6e6f 6465 2d72 6f6c 652e 6b75  ane,node-role.ku
+0002e180: 6265 726e 6574 6573 2e69 6f2f 776f 726b  bernetes.io/work
+0002e190: 6572 220a 2020 2020 2020 2020 2020 2020  er".            
+0002e1a0: 6375 7272 656e 7463 6d64 203d 2066 226b  currentcmd = f"k
+0002e1b0: 7562 6563 746c 2067 6574 206e 6f64 6520  ubectl get node 
+0002e1c0: 2d2d 7365 6c65 6374 6f72 3d27 7b73 656c  --selector='{sel
+0002e1d0: 6563 746f 727d 2722 0a20 2020 2020 2020  ector}'".       
+0002e1e0: 2020 2020 2063 7572 7265 6e74 636d 6420       currentcmd 
+0002e1f0: 2b3d 2022 207c 2067 7265 7020 2720 5265  += " | grep ' Re
+0002e200: 6164 7927 220a 2020 2020 2020 2020 2020  ady'".          
+0002e210: 2020 6375 7272 656e 746e 6f64 6573 203d    currentnodes =
+0002e220: 206f 732e 706f 7065 6e28 6375 7272 656e   os.popen(curren
+0002e230: 7463 6d64 292e 7265 6164 6c69 6e65 7328  tcmd).readlines(
+0002e240: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+0002e250: 206c 656e 2863 7572 7265 6e74 6e6f 6465   len(currentnode
+0002e260: 7329 2021 3d20 776f 726b 6572 733a 0a20  s) != workers:. 
+0002e270: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0002e280: 7072 696e 7428 6622 4f6e 676f 696e 6720  print(f"Ongoing 
+0002e290: 7363 616c 696e 6720 6f70 6572 6174 696f  scaling operatio
+0002e2a0: 6e20 6f6e 2063 6c75 7374 6572 207b 6b75  n on cluster {ku
+0002e2b0: 6265 7d22 290a 2020 2020 2020 2020 2020  be}").          
+0002e2c0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0002e2d0: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
+0002e2e0: 2073 656c 662e 6175 746f 7363 616c 655f   self.autoscale_
+0002e2f0: 636c 7573 7465 7228 6b75 6265 2c20 6b75  cluster(kube, ku
+0002e300: 6265 7479 7065 2c20 776f 726b 6572 732c  betype, workers,
+0002e310: 2074 6872 6573 686f 6c64 2c20 6964 6c65   threshold, idle
+0002e320: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0002e330: 2020 6966 2072 6573 756c 745b 2772 6573    if result['res
+0002e340: 756c 7427 5d20 213d 2027 7375 6363 6573  ult'] != 'succes
+0002e350: 7327 3a0a 2020 2020 2020 2020 2020 2020  s':.            
+0002e360: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+0002e370: 6573 756c 740a 2020 2020 2020 2020 2020  esult.          
+0002e380: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
 0002e390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002e3a0: 2020 776f 726b 6572 7320 3d20 7265 7375    workers = resu
-0002e3b0: 6c74 5b27 776f 726b 6572 7327 5d0a 2020  lt['workers'].  
+0002e3a0: 776f 726b 6572 7320 3d20 7265 7375 6c74  workers = result
+0002e3b0: 5b27 776f 726b 6572 7327 5d0a 2020 2020  ['workers'].    
 0002e3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002e3d0: 2020 7070 7269 6e74 2866 2243 7572 7265    pprint(f"Curre
-0002e3e0: 6e74 2077 6f72 6b65 7273 206e 756d 6265  nt workers numbe
-0002e3f0: 7220 6465 7369 7265 643a 207b 776f 726b  r desired: {work
-0002e400: 6572 737d 2229 0a20 2020 2020 2020 2020  ers}").         
-0002e410: 2020 2073 6c65 6570 2836 3029 0a0a 2020     sleep(60)..  
-0002e420: 2020 6465 6620 7468 7265 6164 6564 5f77    def threaded_w
-0002e430: 6562 5f63 6f6e 736f 6c65 2873 656c 662c  eb_console(self,
-0002e440: 2070 6f72 742c 206e 616d 6529 3a0a 2020   port, name):.  
-0002e450: 2020 2020 2020 636f 6e73 6f6c 6520 3d20        console = 
-0002e460: 4b6d 696e 6963 6f6e 736f 6c65 2863 6f6e  Kminiconsole(con
-0002e470: 6669 673d 7365 6c66 2c20 706f 7274 3d70  fig=self, port=p
-0002e480: 6f72 742c 206e 616d 653d 6e61 6d65 290a  ort, name=name).
-0002e490: 2020 2020 2020 2020 636f 6e73 6f6c 652e          console.
-0002e4a0: 7275 6e28 290a 0a20 2020 2064 6566 2077  run()..    def w
-0002e4b0: 6562 636f 6e73 6f6c 6528 7365 6c66 2c20  ebconsole(self, 
-0002e4c0: 6e61 6d65 293a 0a20 2020 2020 2020 2070  name):.        p
-0002e4d0: 6f72 7420 3d20 6765 745f 6672 6565 5f70  ort = get_free_p
-0002e4e0: 6f72 7428 290a 2020 2020 2020 2020 7420  ort().        t 
-0002e4f0: 3d20 7468 7265 6164 696e 672e 5468 7265  = threading.Thre
-0002e500: 6164 2874 6172 6765 743d 7365 6c66 2e74  ad(target=self.t
-0002e510: 6872 6561 6465 645f 7765 625f 636f 6e73  hreaded_web_cons
-0002e520: 6f6c 652c 2061 7267 733d 2870 6f72 742c  ole, args=(port,
-0002e530: 206e 616d 652c 2929 0a20 2020 2020 2020   name,)).       
-0002e540: 2074 2e73 7461 7274 2829 0a20 2020 2020   t.start().     
-0002e550: 2020 2077 6562 6272 6f77 7365 722e 6f70     webbrowser.op
-0002e560: 656e 2866 2268 7474 703a 2f2f 3132 372e  en(f"http://127.
-0002e570: 302e 302e 313a 7b70 6f72 747d 222c 206e  0.0.1:{port}", n
-0002e580: 6577 3d32 2c20 6175 746f 7261 6973 653d  ew=2, autoraise=
-0002e590: 5472 7565 290a 0a20 2020 2064 6566 2069  True)..    def i
-0002e5a0: 6e66 6f5f 7370 6563 6966 6963 5f61 6b73  nfo_specific_aks
-0002e5b0: 2873 656c 662c 2063 6c75 7374 6572 293a  (self, cluster):
-0002e5c0: 0a20 2020 2020 2020 2066 726f 6d20 6b76  .        from kv
-0002e5d0: 6972 742e 636c 7573 7465 722e 616b 7320  irt.cluster.aks 
-0002e5e0: 696d 706f 7274 2069 6e66 6f20 6173 2061  import info as a
-0002e5f0: 6b73 5f69 6e66 6f0a 2020 2020 2020 2020  ks_info.        
-0002e600: 7265 7475 726e 2061 6b73 5f69 6e66 6f28  return aks_info(
-0002e610: 7365 6c66 2c20 636c 7573 7465 722c 2073  self, cluster, s
-0002e620: 656c 662e 6465 6275 6729 0a0a 2020 2020  elf.debug)..    
-0002e630: 6465 6620 696e 666f 5f73 7065 6369 6669  def info_specifi
-0002e640: 635f 656b 7328 7365 6c66 2c20 636c 7573  c_eks(self, clus
-0002e650: 7465 7229 3a0a 2020 2020 2020 2020 6672  ter):.        fr
-0002e660: 6f6d 206b 7669 7274 2e63 6c75 7374 6572  om kvirt.cluster
-0002e670: 2e65 6b73 2069 6d70 6f72 7420 696e 666f  .eks import info
-0002e680: 2061 7320 656b 735f 696e 666f 0a20 2020   as eks_info.   
-0002e690: 2020 2020 2072 6574 7572 6e20 656b 735f       return eks_
-0002e6a0: 696e 666f 2873 656c 662c 2063 6c75 7374  info(self, clust
-0002e6b0: 6572 2c20 7365 6c66 2e64 6562 7567 290a  er, self.debug).
-0002e6c0: 0a20 2020 2064 6566 2069 6e66 6f5f 6b75  .    def info_ku
-0002e6d0: 6265 5f61 6b73 2873 656c 662c 2071 7569  be_aks(self, qui
-0002e6e0: 6574 2c20 7765 623d 4661 6c73 6529 3a0a  et, web=False):.
-0002e6f0: 2020 2020 2020 2020 6672 6f6d 206b 7669          from kvi
-0002e700: 7274 2e63 6c75 7374 6572 2069 6d70 6f72  rt.cluster impor
-0002e710: 7420 616b 730a 2020 2020 2020 2020 706c  t aks.        pl
-0002e720: 616e 6469 7220 3d20 6f73 2e70 6174 682e  andir = os.path.
-0002e730: 6469 726e 616d 6528 616b 732e 6372 6561  dirname(aks.crea
-0002e740: 7465 2e5f 5f63 6f64 655f 5f2e 636f 5f66  te.__code__.co_f
-0002e750: 696c 656e 616d 6529 0a20 2020 2020 2020  ilename).       
-0002e760: 2069 6e70 7574 6669 6c65 203d 2066 277b   inputfile = f'{
-0002e770: 706c 616e 6469 727d 2f66 616b 652e 796d  plandir}/fake.ym
-0002e780: 6c27 0a20 2020 2020 2020 2073 656c 662e  l'.        self.
-0002e790: 696e 666f 5f70 6c61 6e28 696e 7075 7466  info_plan(inputf
-0002e7a0: 696c 652c 2071 7569 6574 3d71 7569 6574  ile, quiet=quiet
-0002e7b0: 2c20 7765 623d 7765 6229 0a20 2020 2020  , web=web).     
-0002e7c0: 2020 2061 6b73 2e69 6e66 6f5f 7365 7276     aks.info_serv
-0002e7d0: 6963 6528 7365 6c66 290a 0a20 2020 2064  ice(self)..    d
-0002e7e0: 6566 2069 6e66 6f5f 6b75 6265 5f65 6b73  ef info_kube_eks
-0002e7f0: 2873 656c 662c 2071 7569 6574 2c20 7765  (self, quiet, we
-0002e800: 623d 4661 6c73 6529 3a0a 2020 2020 2020  b=False):.      
-0002e810: 2020 6672 6f6d 206b 7669 7274 2e63 6c75    from kvirt.clu
-0002e820: 7374 6572 2069 6d70 6f72 7420 656b 730a  ster import eks.
-0002e830: 2020 2020 2020 2020 706c 616e 6469 7220          plandir 
-0002e840: 3d20 6f73 2e70 6174 682e 6469 726e 616d  = os.path.dirnam
-0002e850: 6528 656b 732e 6372 6561 7465 2e5f 5f63  e(eks.create.__c
-0002e860: 6f64 655f 5f2e 636f 5f66 696c 656e 616d  ode__.co_filenam
-0002e870: 6529 0a20 2020 2020 2020 2069 6e70 7574  e).        input
-0002e880: 6669 6c65 203d 2066 277b 706c 616e 6469  file = f'{plandi
-0002e890: 727d 2f66 616b 652e 796d 6c27 0a20 2020  r}/fake.yml'.   
-0002e8a0: 2020 2020 2073 656c 662e 696e 666f 5f70       self.info_p
-0002e8b0: 6c61 6e28 696e 7075 7466 696c 652c 2071  lan(inputfile, q
-0002e8c0: 7569 6574 3d71 7569 6574 2c20 7765 623d  uiet=quiet, web=
-0002e8d0: 7765 6229 0a20 2020 2020 2020 2065 6b73  web).        eks
-0002e8e0: 2e69 6e66 6f5f 7365 7276 6963 6528 7365  .info_service(se
-0002e8f0: 6c66 290a 0a20 2020 2064 6566 2069 6e66  lf)..    def inf
-0002e900: 6f5f 7370 6563 6966 6963 5f67 6b65 2873  o_specific_gke(s
-0002e910: 656c 662c 2063 6c75 7374 6572 293a 0a20  elf, cluster):. 
-0002e920: 2020 2020 2020 2066 726f 6d20 6b76 6972         from kvir
-0002e930: 742e 636c 7574 6572 2e67 6b65 2069 6d70  t.cluter.gke imp
-0002e940: 6f72 7420 696e 666f 2061 7320 676b 655f  ort info as gke_
-0002e950: 696e 666f 0a20 2020 2020 2020 2072 6574  info.        ret
-0002e960: 7572 6e20 676b 655f 696e 666f 2873 656c  urn gke_info(sel
-0002e970: 662c 2063 6c75 7374 6572 2c20 7365 6c66  f, cluster, self
-0002e980: 2e64 6562 7567 290a 0a20 2020 2064 6566  .debug)..    def
-0002e990: 2069 6e66 6f5f 6b75 6265 5f67 6b65 2873   info_kube_gke(s
-0002e9a0: 656c 662c 2071 7569 6574 2c20 7765 623d  elf, quiet, web=
-0002e9b0: 4661 6c73 6529 3a0a 2020 2020 2020 2020  False):.        
-0002e9c0: 6672 6f6d 206b 7669 7274 2e63 6c75 7374  from kvirt.clust
-0002e9d0: 6572 2069 6d70 6f72 7420 676b 650a 2020  er import gke.  
-0002e9e0: 2020 2020 2020 706c 616e 6469 7220 3d20        plandir = 
-0002e9f0: 6f73 2e70 6174 682e 6469 726e 616d 6528  os.path.dirname(
-0002ea00: 676b 652e 6372 6561 7465 2e5f 5f63 6f64  gke.create.__cod
-0002ea10: 655f 5f2e 636f 5f66 696c 656e 616d 6529  e__.co_filename)
-0002ea20: 0a20 2020 2020 2020 2069 6e70 7574 6669  .        inputfi
-0002ea30: 6c65 203d 2066 277b 706c 616e 6469 727d  le = f'{plandir}
-0002ea40: 2f66 616b 652e 796d 6c27 0a20 2020 2020  /fake.yml'.     
-0002ea50: 2020 2073 656c 662e 696e 666f 5f70 6c61     self.info_pla
-0002ea60: 6e28 696e 7075 7466 696c 652c 2071 7569  n(inputfile, qui
-0002ea70: 6574 3d71 7569 6574 2c20 7765 623d 7765  et=quiet, web=we
-0002ea80: 6229 0a20 2020 2020 2020 2067 6b65 2e69  b).        gke.i
-0002ea90: 6e66 6f5f 7365 7276 6963 6528 7365 6c66  nfo_service(self
-0002eaa0: 290a                                     ).
+0002e3d0: 7070 7269 6e74 2866 2243 7572 7265 6e74  pprint(f"Current
+0002e3e0: 2077 6f72 6b65 7273 206e 756d 6265 7220   workers number 
+0002e3f0: 6465 7369 7265 643a 207b 776f 726b 6572  desired: {worker
+0002e400: 737d 2229 0a20 2020 2020 2020 2020 2020  s}").           
+0002e410: 2073 6c65 6570 2836 3029 0a0a 2020 2020   sleep(60)..    
+0002e420: 6465 6620 7468 7265 6164 6564 5f77 6562  def threaded_web
+0002e430: 5f63 6f6e 736f 6c65 2873 656c 662c 2070  _console(self, p
+0002e440: 6f72 742c 206e 616d 6529 3a0a 2020 2020  ort, name):.    
+0002e450: 2020 2020 636f 6e73 6f6c 6520 3d20 4b6d      console = Km
+0002e460: 696e 6963 6f6e 736f 6c65 2863 6f6e 6669  iniconsole(confi
+0002e470: 673d 7365 6c66 2c20 706f 7274 3d70 6f72  g=self, port=por
+0002e480: 742c 206e 616d 653d 6e61 6d65 290a 2020  t, name=name).  
+0002e490: 2020 2020 2020 636f 6e73 6f6c 652e 7275        console.ru
+0002e4a0: 6e28 290a 0a20 2020 2064 6566 2077 6562  n()..    def web
+0002e4b0: 636f 6e73 6f6c 6528 7365 6c66 2c20 6e61  console(self, na
+0002e4c0: 6d65 293a 0a20 2020 2020 2020 2070 6f72  me):.        por
+0002e4d0: 7420 3d20 6765 745f 6672 6565 5f70 6f72  t = get_free_por
+0002e4e0: 7428 290a 2020 2020 2020 2020 7420 3d20  t().        t = 
+0002e4f0: 7468 7265 6164 696e 672e 5468 7265 6164  threading.Thread
+0002e500: 2874 6172 6765 743d 7365 6c66 2e74 6872  (target=self.thr
+0002e510: 6561 6465 645f 7765 625f 636f 6e73 6f6c  eaded_web_consol
+0002e520: 652c 2061 7267 733d 2870 6f72 742c 206e  e, args=(port, n
+0002e530: 616d 652c 2929 0a20 2020 2020 2020 2074  ame,)).        t
+0002e540: 2e73 7461 7274 2829 0a20 2020 2020 2020  .start().       
+0002e550: 2077 6562 6272 6f77 7365 722e 6f70 656e   webbrowser.open
+0002e560: 2866 2268 7474 703a 2f2f 3132 372e 302e  (f"http://127.0.
+0002e570: 302e 313a 7b70 6f72 747d 222c 206e 6577  0.1:{port}", new
+0002e580: 3d32 2c20 6175 746f 7261 6973 653d 5472  =2, autoraise=Tr
+0002e590: 7565 290a 0a20 2020 2064 6566 2069 6e66  ue)..    def inf
+0002e5a0: 6f5f 7370 6563 6966 6963 5f61 6b73 2873  o_specific_aks(s
+0002e5b0: 656c 662c 2063 6c75 7374 6572 293a 0a20  elf, cluster):. 
+0002e5c0: 2020 2020 2020 2066 726f 6d20 6b76 6972         from kvir
+0002e5d0: 742e 636c 7573 7465 722e 616b 7320 696d  t.cluster.aks im
+0002e5e0: 706f 7274 2069 6e66 6f20 6173 2061 6b73  port info as aks
+0002e5f0: 5f69 6e66 6f0a 2020 2020 2020 2020 7265  _info.        re
+0002e600: 7475 726e 2061 6b73 5f69 6e66 6f28 7365  turn aks_info(se
+0002e610: 6c66 2c20 636c 7573 7465 722c 2073 656c  lf, cluster, sel
+0002e620: 662e 6465 6275 6729 0a0a 2020 2020 6465  f.debug)..    de
+0002e630: 6620 696e 666f 5f73 7065 6369 6669 635f  f info_specific_
+0002e640: 656b 7328 7365 6c66 2c20 636c 7573 7465  eks(self, cluste
+0002e650: 7229 3a0a 2020 2020 2020 2020 6672 6f6d  r):.        from
+0002e660: 206b 7669 7274 2e63 6c75 7374 6572 2e65   kvirt.cluster.e
+0002e670: 6b73 2069 6d70 6f72 7420 696e 666f 2061  ks import info a
+0002e680: 7320 656b 735f 696e 666f 0a20 2020 2020  s eks_info.     
+0002e690: 2020 2072 6574 7572 6e20 656b 735f 696e     return eks_in
+0002e6a0: 666f 2873 656c 662c 2063 6c75 7374 6572  fo(self, cluster
+0002e6b0: 2c20 7365 6c66 2e64 6562 7567 290a 0a20  , self.debug).. 
+0002e6c0: 2020 2064 6566 2069 6e66 6f5f 6b75 6265     def info_kube
+0002e6d0: 5f61 6b73 2873 656c 662c 2071 7569 6574  _aks(self, quiet
+0002e6e0: 2c20 7765 623d 4661 6c73 6529 3a0a 2020  , web=False):.  
+0002e6f0: 2020 2020 2020 6672 6f6d 206b 7669 7274        from kvirt
+0002e700: 2e63 6c75 7374 6572 2069 6d70 6f72 7420  .cluster import 
+0002e710: 616b 730a 2020 2020 2020 2020 706c 616e  aks.        plan
+0002e720: 6469 7220 3d20 6f73 2e70 6174 682e 6469  dir = os.path.di
+0002e730: 726e 616d 6528 616b 732e 6372 6561 7465  rname(aks.create
+0002e740: 2e5f 5f63 6f64 655f 5f2e 636f 5f66 696c  .__code__.co_fil
+0002e750: 656e 616d 6529 0a20 2020 2020 2020 2069  ename).        i
+0002e760: 6e70 7574 6669 6c65 203d 2066 277b 706c  nputfile = f'{pl
+0002e770: 616e 6469 727d 2f66 616b 652e 796d 6c27  andir}/fake.yml'
+0002e780: 0a20 2020 2020 2020 2073 656c 662e 696e  .        self.in
+0002e790: 666f 5f70 6c61 6e28 696e 7075 7466 696c  fo_plan(inputfil
+0002e7a0: 652c 2071 7569 6574 3d71 7569 6574 2c20  e, quiet=quiet, 
+0002e7b0: 7765 623d 7765 6229 0a20 2020 2020 2020  web=web).       
+0002e7c0: 2061 6b73 2e69 6e66 6f5f 7365 7276 6963   aks.info_servic
+0002e7d0: 6528 7365 6c66 290a 0a20 2020 2064 6566  e(self)..    def
+0002e7e0: 2069 6e66 6f5f 6b75 6265 5f65 6b73 2873   info_kube_eks(s
+0002e7f0: 656c 662c 2071 7569 6574 2c20 7765 623d  elf, quiet, web=
+0002e800: 4661 6c73 6529 3a0a 2020 2020 2020 2020  False):.        
+0002e810: 6672 6f6d 206b 7669 7274 2e63 6c75 7374  from kvirt.clust
+0002e820: 6572 2069 6d70 6f72 7420 656b 730a 2020  er import eks.  
+0002e830: 2020 2020 2020 706c 616e 6469 7220 3d20        plandir = 
+0002e840: 6f73 2e70 6174 682e 6469 726e 616d 6528  os.path.dirname(
+0002e850: 656b 732e 6372 6561 7465 2e5f 5f63 6f64  eks.create.__cod
+0002e860: 655f 5f2e 636f 5f66 696c 656e 616d 6529  e__.co_filename)
+0002e870: 0a20 2020 2020 2020 2069 6e70 7574 6669  .        inputfi
+0002e880: 6c65 203d 2066 277b 706c 616e 6469 727d  le = f'{plandir}
+0002e890: 2f66 616b 652e 796d 6c27 0a20 2020 2020  /fake.yml'.     
+0002e8a0: 2020 2073 656c 662e 696e 666f 5f70 6c61     self.info_pla
+0002e8b0: 6e28 696e 7075 7466 696c 652c 2071 7569  n(inputfile, qui
+0002e8c0: 6574 3d71 7569 6574 2c20 7765 623d 7765  et=quiet, web=we
+0002e8d0: 6229 0a20 2020 2020 2020 2065 6b73 2e69  b).        eks.i
+0002e8e0: 6e66 6f5f 7365 7276 6963 6528 7365 6c66  nfo_service(self
+0002e8f0: 290a 0a20 2020 2064 6566 2069 6e66 6f5f  )..    def info_
+0002e900: 7370 6563 6966 6963 5f67 6b65 2873 656c  specific_gke(sel
+0002e910: 662c 2063 6c75 7374 6572 293a 0a20 2020  f, cluster):.   
+0002e920: 2020 2020 2066 726f 6d20 6b76 6972 742e       from kvirt.
+0002e930: 636c 7574 6572 2e67 6b65 2069 6d70 6f72  cluter.gke impor
+0002e940: 7420 696e 666f 2061 7320 676b 655f 696e  t info as gke_in
+0002e950: 666f 0a20 2020 2020 2020 2072 6574 7572  fo.        retur
+0002e960: 6e20 676b 655f 696e 666f 2873 656c 662c  n gke_info(self,
+0002e970: 2063 6c75 7374 6572 2c20 7365 6c66 2e64   cluster, self.d
+0002e980: 6562 7567 290a 0a20 2020 2064 6566 2069  ebug)..    def i
+0002e990: 6e66 6f5f 6b75 6265 5f67 6b65 2873 656c  nfo_kube_gke(sel
+0002e9a0: 662c 2071 7569 6574 2c20 7765 623d 4661  f, quiet, web=Fa
+0002e9b0: 6c73 6529 3a0a 2020 2020 2020 2020 6672  lse):.        fr
+0002e9c0: 6f6d 206b 7669 7274 2e63 6c75 7374 6572  om kvirt.cluster
+0002e9d0: 2069 6d70 6f72 7420 676b 650a 2020 2020   import gke.    
+0002e9e0: 2020 2020 706c 616e 6469 7220 3d20 6f73      plandir = os
+0002e9f0: 2e70 6174 682e 6469 726e 616d 6528 676b  .path.dirname(gk
+0002ea00: 652e 6372 6561 7465 2e5f 5f63 6f64 655f  e.create.__code_
+0002ea10: 5f2e 636f 5f66 696c 656e 616d 6529 0a20  _.co_filename). 
+0002ea20: 2020 2020 2020 2069 6e70 7574 6669 6c65         inputfile
+0002ea30: 203d 2066 277b 706c 616e 6469 727d 2f66   = f'{plandir}/f
+0002ea40: 616b 652e 796d 6c27 0a20 2020 2020 2020  ake.yml'.       
+0002ea50: 2073 656c 662e 696e 666f 5f70 6c61 6e28   self.info_plan(
+0002ea60: 696e 7075 7466 696c 652c 2071 7569 6574  inputfile, quiet
+0002ea70: 3d71 7569 6574 2c20 7765 623d 7765 6229  =quiet, web=web)
+0002ea80: 0a20 2020 2020 2020 2067 6b65 2e69 6e66  .        gke.inf
+0002ea90: 6f5f 7365 7276 6963 6528 7365 6c66 290a  o_service(self).
```

### Comparing `kcli-99.0.202404122133/kvirt/container/__init__.py` & `kcli-99.0.202404131016/kvirt/container/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/containerconfig.py` & `kcli-99.0.202404131016/kvirt/containerconfig.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/defaults.py` & `kcli-99.0.202404131016/kvirt/defaults.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/ekstoken.py` & `kcli-99.0.202404131016/kvirt/ekstoken.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/examples.py` & `kcli-99.0.202404131016/kvirt/examples.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/expose/__init__.py` & `kcli-99.0.202404131016/kvirt/expose/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/expose/static/css/bootstrap.min.css` & `kcli-99.0.202404131016/kvirt/expose/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/expose/static/css/jquery.dataTables.min.css` & `kcli-99.0.202404131016/kvirt/expose/static/css/jquery.dataTables.min.css`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/expose/static/css/kcli.css` & `kcli-99.0.202404131016/kvirt/expose/static/css/kcli.css`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/expose/static/images/favicon.ico` & `kcli-99.0.202404131016/kvirt/expose/static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/expose/static/images/wheel.gif` & `kcli-99.0.202404131016/kvirt/expose/static/images/wheel.gif`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/expose/static/js/dataTables.checkboxes.min.js` & `kcli-99.0.202404131016/kvirt/expose/static/js/dataTables.checkboxes.min.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/expose/static/js/jquery.dataTables.min.js` & `kcli-99.0.202404131016/kvirt/expose/static/js/jquery.dataTables.min.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/expose/static/js/jquery.min.js` & `kcli-99.0.202404131016/kvirt/expose/static/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/expose/swagger.yml` & `kcli-99.0.202404131016/kvirt/expose/swagger.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/expose/templates/form.html` & `kcli-99.0.202404131016/kvirt/expose/templates/form.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/expose/templates/head.html` & `kcli-99.0.202404131016/kvirt/expose/templates/head.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/expose/templates/infoplan.html` & `kcli-99.0.202404131016/kvirt/expose/templates/infoplan.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/expose/templates/planstable.html` & `kcli-99.0.202404131016/kvirt/expose/templates/planstable.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/expose/templates/result.html` & `kcli-99.0.202404131016/kvirt/expose/templates/result.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/gketoken.py` & `kcli-99.0.202404131016/kvirt/gketoken.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/ignitionmerger.py` & `kcli-99.0.202404131016/kvirt/ignitionmerger.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/internalplans/__init__.py` & `kcli-99.0.202404131016/kvirt/internalplans/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/jinjafilters/jinjafilters.py` & `kcli-99.0.202404131016/kvirt/jinjafilters/jinjafilters.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/keywords.yaml` & `kcli-99.0.202404131016/kvirt/keywords.yaml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/kfish/__init__.py` & `kcli-99.0.202404131016/kvirt/kfish/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/klist.py` & `kcli-99.0.202404131016/kvirt/klist.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/ksushy/__init__.py` & `kcli-99.0.202404131016/kvirt/ksushy/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/ksushy/templates/bios.json` & `kcli-99.0.202404131016/kvirt/ksushy/templates/bios.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/ksushy/templates/manager.json` & `kcli-99.0.202404131016/kvirt/ksushy/templates/manager.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/ksushy/templates/managers.json` & `kcli-99.0.202404131016/kvirt/ksushy/templates/managers.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/ksushy/templates/root.json` & `kcli-99.0.202404131016/kvirt/ksushy/templates/root.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/ksushy/templates/system.json` & `kcli-99.0.202404131016/kvirt/ksushy/templates/system.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/ksushy/templates/virtualmedia_cd.json` & `kcli-99.0.202404131016/kvirt/ksushy/templates/virtualmedia_cd.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/ksushy/templates/virtualmedias.json` & `kcli-99.0.202404131016/kvirt/ksushy/templates/virtualmedias.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/miniconsole/__init__.py` & `kcli-99.0.202404131016/kvirt/miniconsole/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/nameutils/__init__.py` & `kcli-99.0.202404131016/kvirt/nameutils/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/providers/aws/__init__.py` & `kcli-99.0.202404131016/kvirt/providers/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/providers/aws/ctlplane_policy.json` & `kcli-99.0.202404131016/kvirt/providers/aws/ctlplane_policy.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/providers/azure/__init__.py` & `kcli-99.0.202404131016/kvirt/providers/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/providers/gcp/__init__.py` & `kcli-99.0.202404131016/kvirt/providers/gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/providers/ibm/__init__.py` & `kcli-99.0.202404131016/kvirt/providers/ibm/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/providers/kubevirt/__init__.py` & `kcli-99.0.202404131016/kvirt/providers/kubevirt/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/providers/kvm/__init__.py` & `kcli-99.0.202404131016/kvirt/providers/kvm/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/providers/kvm/helpers.py` & `kcli-99.0.202404131016/kvirt/providers/kvm/helpers.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/providers/openstack/__init__.py` & `kcli-99.0.202404131016/kvirt/providers/openstack/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/providers/ovirt/__init__.py` & `kcli-99.0.202404131016/kvirt/providers/ovirt/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/providers/packet/__init__.py` & `kcli-99.0.202404131016/kvirt/providers/packet/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/providers/proxmox/__init__.py` & `kcli-99.0.202404131016/kvirt/providers/proxmox/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/providers/sampleprovider.py` & `kcli-99.0.202404131016/kvirt/providers/sampleprovider.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/providers/vsphere/__init__.py` & `kcli-99.0.202404131016/kvirt/providers/vsphere/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/providers/vsphere/helpers.py` & `kcli-99.0.202404131016/kvirt/providers/vsphere/helpers.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/providers/vsphere/tagging.py` & `kcli-99.0.202404131016/kvirt/providers/vsphere/tagging.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/providers/web/__init__.py` & `kcli-99.0.202404131016/kvirt/providers/web/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/__init__.py` & `kcli-99.0.202404131016/kvirt/web/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/css/bootstrap-theme.min.css` & `kcli-99.0.202404131016/kvirt/web/static/css/bootstrap-theme.min.css`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/css/bootstrap.min.css` & `kcli-99.0.202404131016/kvirt/web/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/css/jquery.dataTables.min.css` & `kcli-99.0.202404131016/kvirt/web/static/css/jquery.dataTables.min.css`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/css/kcli.css` & `kcli-99.0.202404131016/kvirt/web/static/css/kcli.css`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/css/navbar.css` & `kcli-99.0.202404131016/kvirt/web/static/css/navbar.css`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/css/spice.css` & `kcli-99.0.202404131016/kvirt/web/static/css/spice.css`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/fonts/glyphicons-halflings-regular.woff2` & `kcli-99.0.202404131016/kvirt/web/static/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/images/Centos.png` & `kcli-99.0.202404131016/kvirt/web/static/images/Centos.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/images/Fedora.png` & `kcli-99.0.202404131016/kvirt/web/static/images/Fedora.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/images/Redhat.png` & `kcli-99.0.202404131016/kvirt/web/static/images/Redhat.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/images/Suse.png` & `kcli-99.0.202404131016/kvirt/web/static/images/Suse.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/images/Tux.png` & `kcli-99.0.202404131016/kvirt/web/static/images/Tux.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/images/Ubuntu.png` & `kcli-99.0.202404131016/kvirt/web/static/images/Ubuntu.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/images/delete.png` & `kcli-99.0.202404131016/kvirt/web/static/images/delete.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/images/favicon.ico` & `kcli-99.0.202404131016/kvirt/web/static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/images/kcli-small.png` & `kcli-99.0.202404131016/kvirt/web/static/images/kcli-small.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/images/kcli.jpg` & `kcli-99.0.202404131016/kvirt/web/static/images/kcli.jpg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/images/kcli.png` & `kcli-99.0.202404131016/kvirt/web/static/images/kcli.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/images/logo-header.svg` & `kcli-99.0.202404131016/kvirt/web/static/images/logo-header.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/images/logo-main.svg` & `kcli-99.0.202404131016/kvirt/web/static/images/logo-main.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/images/start.png` & `kcli-99.0.202404131016/kvirt/web/static/images/start.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/images/stop.png` & `kcli-99.0.202404131016/kvirt/web/static/images/stop.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/images/wheel.gif` & `kcli-99.0.202404131016/kvirt/web/static/images/wheel.gif`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/js/bootstrap-notify.js` & `kcli-99.0.202404131016/kvirt/web/static/js/bootstrap-notify.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/js/bootstrap.min.js` & `kcli-99.0.202404131016/kvirt/web/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/js/containeraction.js` & `kcli-99.0.202404131016/kvirt/web/static/js/containeraction.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/js/dataTables.checkboxes.min.js` & `kcli-99.0.202404131016/kvirt/web/static/js/dataTables.checkboxes.min.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/js/hostaction.js` & `kcli-99.0.202404131016/kvirt/web/static/js/hostaction.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/js/imageaction.js` & `kcli-99.0.202404131016/kvirt/web/static/js/imageaction.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/js/jquery.dataTables.min.js` & `kcli-99.0.202404131016/kvirt/web/static/js/jquery.dataTables.min.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/js/jquery.min.js` & `kcli-99.0.202404131016/kvirt/web/static/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/js/kcli.js` & `kcli-99.0.202404131016/kvirt/web/static/js/kcli.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/js/kubeaction.js` & `kcli-99.0.202404131016/kvirt/web/static/js/kubeaction.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/js/list.js` & `kcli-99.0.202404131016/kvirt/web/static/js/list.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/js/networkaction.js` & `kcli-99.0.202404131016/kvirt/web/static/js/networkaction.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/js/planaction.js` & `kcli-99.0.202404131016/kvirt/web/static/js/planaction.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/js/poolaction.js` & `kcli-99.0.202404131016/kvirt/web/static/js/poolaction.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/js/productaction.js` & `kcli-99.0.202404131016/kvirt/web/static/js/productaction.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/js/repoaction.js` & `kcli-99.0.202404131016/kvirt/web/static/js/repoaction.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/js/snapshotaction.js` & `kcli-99.0.202404131016/kvirt/web/static/js/snapshotaction.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/js/spice/atKeynames.js` & `kcli-99.0.202404131016/kvirt/web/static/js/spice/atKeynames.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/js/spice/bitmap.js` & `kcli-99.0.202404131016/kvirt/web/static/js/spice/bitmap.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/js/spice/cursor.js` & `kcli-99.0.202404131016/kvirt/web/static/js/spice/cursor.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/js/spice/display.js` & `kcli-99.0.202404131016/kvirt/web/static/js/spice/display.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/js/spice/enums.js` & `kcli-99.0.202404131016/kvirt/web/static/js/spice/enums.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/js/spice/filexfer.js` & `kcli-99.0.202404131016/kvirt/web/static/js/spice/filexfer.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/js/spice/inputs.js` & `kcli-99.0.202404131016/kvirt/web/static/js/spice/inputs.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/js/spice/lz.js` & `kcli-99.0.202404131016/kvirt/web/static/js/spice/lz.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/js/spice/main.js` & `kcli-99.0.202404131016/kvirt/web/static/js/spice/main.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/js/spice/playback.js` & `kcli-99.0.202404131016/kvirt/web/static/js/spice/playback.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/js/spice/png.js` & `kcli-99.0.202404131016/kvirt/web/static/js/spice/png.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/js/spice/port.js` & `kcli-99.0.202404131016/kvirt/web/static/js/spice/port.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/js/spice/quic.js` & `kcli-99.0.202404131016/kvirt/web/static/js/spice/quic.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/js/spice/resize.js` & `kcli-99.0.202404131016/kvirt/web/static/js/spice/resize.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/js/spice/simulatecursor.js` & `kcli-99.0.202404131016/kvirt/web/static/js/spice/simulatecursor.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/js/spice/spicearraybuffer.js` & `kcli-99.0.202404131016/kvirt/web/static/js/spice/spicearraybuffer.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/js/spice/spiceconn.js` & `kcli-99.0.202404131016/kvirt/web/static/js/spice/spiceconn.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/js/spice/spicedataview.js` & `kcli-99.0.202404131016/kvirt/web/static/js/spice/spicedataview.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/js/spice/spicemsg.js` & `kcli-99.0.202404131016/kvirt/web/static/js/spice/spicemsg.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/js/spice/spicetype.js` & `kcli-99.0.202404131016/kvirt/web/static/js/spice/spicetype.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/js/spice/thirdparty/browser-es-module-loader/src/babel-worker.js` & `kcli-99.0.202404131016/kvirt/web/static/js/spice/thirdparty/browser-es-module-loader/src/babel-worker.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/js/spice/thirdparty/browser-es-module-loader/src/browser-es-module-loader.js` & `kcli-99.0.202404131016/kvirt/web/static/js/spice/thirdparty/browser-es-module-loader/src/browser-es-module-loader.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/js/spice/thirdparty/jsbn.js` & `kcli-99.0.202404131016/kvirt/web/static/js/spice/thirdparty/jsbn.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/js/spice/thirdparty/prng4.js` & `kcli-99.0.202404131016/kvirt/web/static/js/spice/thirdparty/prng4.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/js/spice/thirdparty/rng.js` & `kcli-99.0.202404131016/kvirt/web/static/js/spice/thirdparty/rng.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/js/spice/thirdparty/rsa.js` & `kcli-99.0.202404131016/kvirt/web/static/js/spice/thirdparty/rsa.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/js/spice/thirdparty/sha1.js` & `kcli-99.0.202404131016/kvirt/web/static/js/spice/thirdparty/sha1.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/js/spice/ticket.js` & `kcli-99.0.202404131016/kvirt/web/static/js/spice/ticket.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/js/spice/utils.js` & `kcli-99.0.202404131016/kvirt/web/static/js/spice/utils.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/js/spice/webm.js` & `kcli-99.0.202404131016/kvirt/web/static/js/spice/webm.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/js/spice/wire.js` & `kcli-99.0.202404131016/kvirt/web/static/js/spice/wire.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/js/vmaction.js` & `kcli-99.0.202404131016/kvirt/web/static/js/vmaction.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/app/error-handler.js` & `kcli-99.0.202404131016/kvirt/web/static/vnc/app/error-handler.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/alt.svg` & `kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/alt.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/clipboard.svg` & `kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/clipboard.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/connect.svg` & `kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/connect.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/ctrl.svg` & `kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/ctrl.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/ctrlaltdel.svg` & `kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/ctrlaltdel.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/disconnect.svg` & `kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/disconnect.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/drag.svg` & `kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/drag.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/error.svg` & `kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/error.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/esc.svg` & `kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/esc.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/expander.svg` & `kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/expander.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/fullscreen.svg` & `kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/fullscreen.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/handle.svg` & `kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/handle.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/handle_bg.svg` & `kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/handle_bg.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/icons/Makefile` & `kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/icons/Makefile`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/icons/novnc-120x120.png` & `kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/icons/novnc-120x120.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/icons/novnc-144x144.png` & `kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/icons/novnc-144x144.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/icons/novnc-152x152.png` & `kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/icons/novnc-152x152.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/icons/novnc-16x16.png` & `kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/icons/novnc-16x16.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/icons/novnc-192x192.png` & `kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/icons/novnc-192x192.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/icons/novnc-24x24.png` & `kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/icons/novnc-24x24.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/icons/novnc-32x32.png` & `kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/icons/novnc-32x32.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/icons/novnc-48x48.png` & `kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/icons/novnc-48x48.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/icons/novnc-60x60.png` & `kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/icons/novnc-60x60.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/icons/novnc-64x64.png` & `kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/icons/novnc-64x64.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/icons/novnc-72x72.png` & `kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/icons/novnc-72x72.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/icons/novnc-76x76.png` & `kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/icons/novnc-76x76.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/icons/novnc-96x96.png` & `kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/icons/novnc-96x96.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/icons/novnc-icon-sm.svg` & `kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/icons/novnc-icon-sm.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/icons/novnc-icon.svg` & `kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/icons/novnc-icon.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/info.svg` & `kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/info.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/keyboard.svg` & `kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/keyboard.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/mouse_left.svg` & `kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/mouse_left.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/mouse_middle.svg` & `kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/mouse_middle.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/mouse_none.svg` & `kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/mouse_none.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/mouse_right.svg` & `kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/mouse_right.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/power.svg` & `kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/power.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/settings.svg` & `kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/settings.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/tab.svg` & `kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/tab.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/toggleextrakeys.svg` & `kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/toggleextrakeys.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/warning.svg` & `kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/warning.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/app/images/windows.svg` & `kcli-99.0.202404131016/kvirt/web/static/vnc/app/images/windows.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/app/locale/cs.json` & `kcli-99.0.202404131016/kvirt/web/static/vnc/app/locale/cs.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/app/locale/de.json` & `kcli-99.0.202404131016/kvirt/web/static/vnc/app/locale/de.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/app/locale/el.json` & `kcli-99.0.202404131016/kvirt/web/static/vnc/app/locale/el.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/app/locale/es.json` & `kcli-99.0.202404131016/kvirt/web/static/vnc/app/locale/es.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/app/locale/ja.json` & `kcli-99.0.202404131016/kvirt/web/static/vnc/app/locale/ja.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/app/locale/ko.json` & `kcli-99.0.202404131016/kvirt/web/static/vnc/app/locale/ko.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/app/locale/nl.json` & `kcli-99.0.202404131016/kvirt/web/static/vnc/app/locale/nl.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/app/locale/pl.json` & `kcli-99.0.202404131016/kvirt/web/static/vnc/app/locale/pl.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/app/locale/ru.json` & `kcli-99.0.202404131016/kvirt/web/static/vnc/app/locale/ru.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/app/locale/sv.json` & `kcli-99.0.202404131016/kvirt/web/static/vnc/app/locale/sv.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/app/locale/tr.json` & `kcli-99.0.202404131016/kvirt/web/static/vnc/app/locale/tr.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/app/locale/zh_CN.json` & `kcli-99.0.202404131016/kvirt/web/static/vnc/app/locale/zh_CN.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/app/locale/zh_TW.json` & `kcli-99.0.202404131016/kvirt/web/static/vnc/app/locale/zh_TW.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/app/localization.js` & `kcli-99.0.202404131016/kvirt/web/static/vnc/app/localization.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/app/sounds/bell.mp3` & `kcli-99.0.202404131016/kvirt/web/static/vnc/app/sounds/bell.mp3`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/app/sounds/bell.oga` & `kcli-99.0.202404131016/kvirt/web/static/vnc/app/sounds/bell.oga`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/app/styles/Orbitron700.ttf` & `kcli-99.0.202404131016/kvirt/web/static/vnc/app/styles/Orbitron700.ttf`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/app/styles/Orbitron700.woff` & `kcli-99.0.202404131016/kvirt/web/static/vnc/app/styles/Orbitron700.woff`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/app/styles/base.css` & `kcli-99.0.202404131016/kvirt/web/static/vnc/app/styles/base.css`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/app/ui.js` & `kcli-99.0.202404131016/kvirt/web/static/vnc/app/ui.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/app/webutil.js` & `kcli-99.0.202404131016/kvirt/web/static/vnc/app/webutil.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/core/base64.js` & `kcli-99.0.202404131016/kvirt/web/static/vnc/core/base64.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/core/decoders/copyrect.js` & `kcli-99.0.202404131016/kvirt/web/static/vnc/core/decoders/copyrect.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/core/decoders/hextile.js` & `kcli-99.0.202404131016/kvirt/web/static/vnc/core/decoders/hextile.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/core/decoders/raw.js` & `kcli-99.0.202404131016/kvirt/web/static/vnc/core/decoders/raw.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/core/decoders/rre.js` & `kcli-99.0.202404131016/kvirt/web/static/vnc/core/decoders/rre.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/core/decoders/tight.js` & `kcli-99.0.202404131016/kvirt/web/static/vnc/core/decoders/tight.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/core/decoders/tightpng.js` & `kcli-99.0.202404131016/kvirt/web/static/vnc/core/decoders/tightpng.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/core/des.js` & `kcli-99.0.202404131016/kvirt/web/static/vnc/core/des.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/core/display.js` & `kcli-99.0.202404131016/kvirt/web/static/vnc/core/display.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/core/encodings.js` & `kcli-99.0.202404131016/kvirt/web/static/vnc/core/encodings.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/core/inflator.js` & `kcli-99.0.202404131016/kvirt/web/static/vnc/core/inflator.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/core/input/domkeytable.js` & `kcli-99.0.202404131016/kvirt/web/static/vnc/core/input/domkeytable.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/core/input/fixedkeys.js` & `kcli-99.0.202404131016/kvirt/web/static/vnc/core/input/fixedkeys.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/core/input/keyboard.js` & `kcli-99.0.202404131016/kvirt/web/static/vnc/core/input/keyboard.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/core/input/keysym.js` & `kcli-99.0.202404131016/kvirt/web/static/vnc/core/input/keysym.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/core/input/keysymdef.js` & `kcli-99.0.202404131016/kvirt/web/static/vnc/core/input/keysymdef.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/core/input/mouse.js` & `kcli-99.0.202404131016/kvirt/web/static/vnc/core/input/mouse.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/core/input/util.js` & `kcli-99.0.202404131016/kvirt/web/static/vnc/core/input/util.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/core/input/vkeys.js` & `kcli-99.0.202404131016/kvirt/web/static/vnc/core/input/vkeys.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/core/input/xtscancodes.js` & `kcli-99.0.202404131016/kvirt/web/static/vnc/core/input/xtscancodes.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/core/rfb.js` & `kcli-99.0.202404131016/kvirt/web/static/vnc/core/rfb.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/core/util/browser.js` & `kcli-99.0.202404131016/kvirt/web/static/vnc/core/util/browser.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/core/util/cursor.js` & `kcli-99.0.202404131016/kvirt/web/static/vnc/core/util/cursor.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/core/util/events.js` & `kcli-99.0.202404131016/kvirt/web/static/vnc/core/util/events.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/core/util/eventtarget.js` & `kcli-99.0.202404131016/kvirt/web/static/vnc/core/util/eventtarget.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/core/util/logging.js` & `kcli-99.0.202404131016/kvirt/web/static/vnc/core/util/logging.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/core/util/polyfill.js` & `kcli-99.0.202404131016/kvirt/web/static/vnc/core/util/polyfill.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/core/websock.js` & `kcli-99.0.202404131016/kvirt/web/static/vnc/core/websock.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/vendor/browser-es-module-loader/src/babel-worker.js` & `kcli-99.0.202404131016/kvirt/web/static/vnc/vendor/browser-es-module-loader/src/babel-worker.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/vendor/browser-es-module-loader/src/browser-es-module-loader.js` & `kcli-99.0.202404131016/kvirt/web/static/vnc/vendor/browser-es-module-loader/src/browser-es-module-loader.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/vendor/pako/LICENSE` & `kcli-99.0.202404131016/kvirt/web/static/vnc/vendor/pako/LICENSE`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/vendor/pako/lib/utils/common.js` & `kcli-99.0.202404131016/kvirt/web/static/vnc/vendor/pako/lib/utils/common.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/vendor/pako/lib/zlib/adler32.js` & `kcli-99.0.202404131016/kvirt/web/static/vnc/vendor/pako/lib/zlib/adler32.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/vendor/pako/lib/zlib/constants.js` & `kcli-99.0.202404131016/kvirt/web/static/vnc/vendor/pako/lib/zlib/constants.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/vendor/pako/lib/zlib/crc32.js` & `kcli-99.0.202404131016/kvirt/web/static/vnc/vendor/pako/lib/zlib/crc32.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/vendor/pako/lib/zlib/deflate.js` & `kcli-99.0.202404131016/kvirt/web/static/vnc/vendor/pako/lib/zlib/deflate.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/vendor/pako/lib/zlib/gzheader.js` & `kcli-99.0.202404131016/kvirt/web/static/vnc/vendor/pako/lib/zlib/gzheader.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/vendor/pako/lib/zlib/inffast.js` & `kcli-99.0.202404131016/kvirt/web/static/vnc/vendor/pako/lib/zlib/inffast.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/vendor/pako/lib/zlib/inflate.js` & `kcli-99.0.202404131016/kvirt/web/static/vnc/vendor/pako/lib/zlib/inflate.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/vendor/pako/lib/zlib/inftrees.js` & `kcli-99.0.202404131016/kvirt/web/static/vnc/vendor/pako/lib/zlib/inftrees.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/vendor/pako/lib/zlib/messages.js` & `kcli-99.0.202404131016/kvirt/web/static/vnc/vendor/pako/lib/zlib/messages.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/vendor/pako/lib/zlib/trees.js` & `kcli-99.0.202404131016/kvirt/web/static/vnc/vendor/pako/lib/zlib/trees.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/vendor/pako/lib/zlib/zstream.js` & `kcli-99.0.202404131016/kvirt/web/static/vnc/vendor/pako/lib/zlib/zstream.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/static/vnc/vendor/promise.js` & `kcli-99.0.202404131016/kvirt/web/static/vnc/vendor/promise.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/templates/bootstrap.html` & `kcli-99.0.202404131016/kvirt/web/templates/bootstrap.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/templates/console.html` & `kcli-99.0.202404131016/kvirt/web/templates/console.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/templates/containercreate.html` & `kcli-99.0.202404131016/kvirt/web/templates/containercreate.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/templates/containerprofilestable.html` & `kcli-99.0.202404131016/kvirt/web/templates/containerprofilestable.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/templates/containerstable.html` & `kcli-99.0.202404131016/kvirt/web/templates/containerstable.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/templates/head.html` & `kcli-99.0.202404131016/kvirt/web/templates/head.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/templates/hoststable.html` & `kcli-99.0.202404131016/kvirt/web/templates/hoststable.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/templates/imagecreate.html` & `kcli-99.0.202404131016/kvirt/web/templates/imagecreate.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/templates/imagestable.html` & `kcli-99.0.202404131016/kvirt/web/templates/imagestable.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/templates/kubecreate.html` & `kcli-99.0.202404131016/kvirt/web/templates/kubecreate.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/templates/kubeinfo.html` & `kcli-99.0.202404131016/kvirt/web/templates/kubeinfo.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/templates/kubeprofilestable.html` & `kcli-99.0.202404131016/kvirt/web/templates/kubeprofilestable.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/templates/kubestable.html` & `kcli-99.0.202404131016/kvirt/web/templates/kubestable.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/templates/navbar.html` & `kcli-99.0.202404131016/kvirt/web/templates/navbar.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/templates/networkcreate.html` & `kcli-99.0.202404131016/kvirt/web/templates/networkcreate.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/templates/networks.html` & `kcli-99.0.202404131016/kvirt/web/templates/networks.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/templates/networkstable.html` & `kcli-99.0.202404131016/kvirt/web/templates/networkstable.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/templates/plancreate.html` & `kcli-99.0.202404131016/kvirt/web/templates/plancreate.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/templates/planstable.html` & `kcli-99.0.202404131016/kvirt/web/templates/planstable.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/templates/poolcreate.html` & `kcli-99.0.202404131016/kvirt/web/templates/poolcreate.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/templates/poolstable.html` & `kcli-99.0.202404131016/kvirt/web/templates/poolstable.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/templates/productcreate.html` & `kcli-99.0.202404131016/kvirt/web/templates/productcreate.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/templates/productstable.html` & `kcli-99.0.202404131016/kvirt/web/templates/productstable.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/templates/repocreate.html` & `kcli-99.0.202404131016/kvirt/web/templates/repocreate.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/templates/repostable.html` & `kcli-99.0.202404131016/kvirt/web/templates/repostable.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/templates/vmcreate.html` & `kcli-99.0.202404131016/kvirt/web/templates/vmcreate.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/templates/vmprofilestable.html` & `kcli-99.0.202404131016/kvirt/web/templates/vmprofilestable.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/kvirt/web/templates/vmstable.html` & `kcli-99.0.202404131016/kvirt/web/templates/vmstable.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/samples/config.yml` & `kcli-99.0.202404131016/samples/config.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/samples/profiles.yml` & `kcli-99.0.202404131016/samples/profiles.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404122133/setup.py` & `kcli-99.0.202404131016/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 description = 'Provisioner/Manager for Libvirt/Vsphere/Aws/Gcp/Kubevirt/Ovirt/Openstack/IBM Cloud and containers'
 long_description = description
 if os.path.exists('README.rst'):
     long_description = open('README.rst').read()
 
 setup(
     name='kcli',
-    version='99.0.202404122133',
+    version='99.0.202404131016',
     include_package_data=True,
     packages=find_packages(),
     zip_safe=False,
     description=description,
     long_description=long_description,
     url='http://github.com/karmab/kcli',
     author='Karim Boumedhel',
```

### Comparing `kcli-99.0.202404122133/tests/test_kvirt.py` & `kcli-99.0.202404131016/tests/test_kvirt.py`

 * *Files identical despite different names*

