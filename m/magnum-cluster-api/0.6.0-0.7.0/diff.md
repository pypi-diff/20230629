# Comparing `tmp/magnum_cluster_api-0.6.0.tar.gz` & `tmp/magnum_cluster_api-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magnum_cluster_api-0.6.0.tar", max compression
+gzip compressed data, was "magnum_cluster_api-0.7.0.tar", max compression
```

## Comparing `magnum_cluster_api-0.6.0.tar` & `magnum_cluster_api-0.7.0.tar`

### file list

```diff
@@ -1,78 +1,78 @@
--rw-r--r--   0        0        0    10142 2023-06-01 16:40:59.661282 magnum_cluster_api-0.6.0/LICENSE
--rw-r--r--   0        0        0     2795 2023-06-01 16:40:59.661282 magnum_cluster_api-0.6.0/README.md
--rw-r--r--   0        0        0        0 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/__init__.py
--rw-r--r--   0        0        0        0 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/charts/.gitkeep
--rw-r--r--   0        0        0      349 2023-06-01 16:41:00.389285 magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/.helmignore
--rw-r--r--   0        0        0      437 2023-06-01 16:41:00.385285 magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/Chart.yaml
--rw-r--r--   0        0        0    29122 2023-06-01 16:41:00.389285 magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/README.md
--rw-r--r--   0        0        0    14987 2023-06-01 16:41:00.389285 magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/README.md.gotmpl
--rw-r--r--   0        0        0      827 2023-06-01 16:41:00.385285 magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/templates/NOTES.txt
--rw-r--r--   0        0        0     4034 2023-06-01 16:41:00.385285 magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/templates/_helpers.tpl
--rw-r--r--   0        0        0     2982 2023-06-01 16:41:00.393285 magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrole.yaml
--rw-r--r--   0        0        0      534 2023-06-01 16:41:00.385285 magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrolebinding.yaml
--rw-r--r--   0        0        0    13204 2023-06-01 16:41:00.385285 magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/templates/deployment.yaml
--rw-r--r--   0        0        0      508 2023-06-01 16:41:00.385285 magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/templates/pdb.yaml
--rw-r--r--   0        0        0      972 2023-06-01 16:41:00.385285 magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/templates/podsecuritypolicy.yaml
--rw-r--r--   0        0        0      758 2023-06-01 16:41:00.385285 magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/templates/priority-expander-configmap.yaml
--rw-r--r--   0        0        0      564 2023-06-01 16:41:00.385285 magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/templates/prometheusrule.yaml
--rw-r--r--   0        0        0     1807 2023-06-01 16:41:00.385285 magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/templates/role.yaml
--rw-r--r--   0        0        0      527 2023-06-01 16:41:00.385285 magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/templates/rolebinding.yaml
--rw-r--r--   0        0        0      989 2023-06-01 16:41:00.385285 magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/templates/secret.yaml
--rw-r--r--   0        0        0     1180 2023-06-01 16:41:00.385285 magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/templates/service.yaml
--rw-r--r--   0        0        0      528 2023-06-01 16:41:00.385285 magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/templates/serviceaccount.yaml
--rw-r--r--   0        0        0      960 2023-06-01 16:41:00.385285 magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/templates/servicemonitor.yaml
--rw-r--r--   0        0        0      663 2023-06-01 16:41:00.385285 magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/templates/vpa.yaml
--rw-r--r--   0        0        0    18003 2023-06-01 16:41:00.385285 magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/values.yaml
--rw-r--r--   0        0        0     1977 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/clients.py
--rw-r--r--   0        0        0        0 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/cmd/__init__.py
--rw-r--r--   0        0        0     4019 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/cmd/image_builder.py
--rw-r--r--   0        0        0     4714 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/cmd/image_loader.py
--rw-r--r--   0        0        0      956 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/cmd/proxy.py
--rw-r--r--   0        0        0     3278 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/conf.py
--rw-r--r--   0        0        0    11915 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/driver.py
--rw-r--r--   0        0        0     1167 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/exceptions.py
--rw-r--r--   0        0        0     2888 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/helm.py
--rw-r--r--   0        0        0     3464 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/image_utils.py
--rw-r--r--   0        0        0     1116 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/images.py
--rw-r--r--   0        0        0        0 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/manifests/__init__.py
--rw-r--r--   0        0        0     4941 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/manifests/audit/policy.yaml
--rw-r--r--   0        0        0   235191 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/manifests/calico/v3.24.2.yaml
--rw-r--r--   0        0        0      623 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/manifests/ccm/cloud-controller-manager-role-bindings.yaml
--rw-r--r--   0        0        0     1430 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/manifests/ccm/cloud-controller-manager-roles.yaml
--rw-r--r--   0        0        0     2263 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/manifests/ccm/openstack-cloud-controller-manager-ds.yaml
--rw-r--r--   0        0        0     4506 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/manifests/cinder-csi/cinder-csi-controllerplugin-rbac.yaml
--rw-r--r--   0        0        0     4034 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/manifests/cinder-csi/cinder-csi-controllerplugin.yaml
--rw-r--r--   0        0        0      609 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/manifests/cinder-csi/cinder-csi-nodeplugin-rbac.yaml
--rw-r--r--   0        0        0     3307 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/manifests/cinder-csi/cinder-csi-nodeplugin.yaml
--rw-r--r--   0        0        0      194 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/manifests/cinder-csi/csi-cinder-driver.yaml
--rw-r--r--   0        0        0     3377 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/manifests/manila-csi/csi-controllerplugin-rbac.yaml
--rw-r--r--   0        0        0     3944 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/manifests/manila-csi/csi-controllerplugin.yaml
--rw-r--r--   0        0        0     1513 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/manifests/manila-csi/csi-nodeplugin-rbac.yaml
--rw-r--r--   0        0        0     2988 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/manifests/manila-csi/csi-nodeplugin.yaml
--rw-r--r--   0        0        0      143 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/manifests/manila-csi/csidriver.yaml
--rw-r--r--   0        0        0     3127 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/manifests/nfs-csi/csi-nfs-controller.yaml
--rw-r--r--   0        0        0      170 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/manifests/nfs-csi/csi-nfs-driverinfo.yaml
--rw-r--r--   0        0        0     3530 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/manifests/nfs-csi/csi-nfs-node.yaml
--rw-r--r--   0        0        0     1423 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/manifests/nfs-csi/rbac-csi-nfs.yaml
--rw-r--r--   0        0        0     1526 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/monitor.py
--rw-r--r--   0        0        0     5453 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/objects.py
--rw-r--r--   0        0        0      828 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/privsep/__init__.py
--rw-r--r--   0        0        0     1333 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/privsep/haproxy.py
--rw-r--r--   0        0        0    11719 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/proxy/manager.py
--rw-r--r--   0        0        0     3616 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/proxy/structs.py
--rw-r--r--   0        0        0      580 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/proxy/templates/haproxy.cfg.j2
--rw-r--r--   0        0        0     1511 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/proxy/utils.py
--rw-r--r--   0        0        0    78098 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/resources.py
--rw-r--r--   0        0        0     1492 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/service.py
--rw-r--r--   0        0        0     3119 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/tests/functional/conftest.py
--rw-r--r--   0        0        0      666 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/tests/functional/test_clusters.py
--rw-r--r--   0        0        0      942 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/tests/unit/conftest.py
--rw-r--r--   0        0        0     3453 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/tests/unit/test_helm.py
--rw-r--r--   0        0        0     1731 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/tests/unit/test_image_utils.py
--rw-r--r--   0        0        0     2759 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/tests/unit/test_images.py
--rw-r--r--   0        0        0     5366 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/tests/unit/test_objects.py
--rw-r--r--   0        0        0     1717 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/tests/unit/test_resources.py
--rw-r--r--   0        0        0     1192 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/tests/unit/test_utils.py
--rw-r--r--   0        0        0    10350 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/utils.py
--rw-r--r--   0        0        0     1220 2023-06-01 16:40:59.669282 magnum_cluster_api-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     3890 1970-01-01 00:00:00.000000 magnum_cluster_api-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    10142 2023-06-29 14:27:23.846611 magnum_cluster_api-0.7.0/LICENSE
+-rw-r--r--   0        0        0     2795 2023-06-29 14:27:23.846611 magnum_cluster_api-0.7.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-29 14:27:23.846611 magnum_cluster_api-0.7.0/magnum_cluster_api/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-29 14:27:23.846611 magnum_cluster_api-0.7.0/magnum_cluster_api/charts/.gitkeep
+-rw-r--r--   0        0        0      349 2023-06-29 14:27:28.303258 magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/.helmignore
+-rw-r--r--   0        0        0      437 2023-06-29 14:27:28.303258 magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/Chart.yaml
+-rw-r--r--   0        0        0    29122 2023-06-29 14:27:28.303258 magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/README.md
+-rw-r--r--   0        0        0    14987 2023-06-29 14:27:28.303258 magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/README.md.gotmpl
+-rw-r--r--   0        0        0      827 2023-06-29 14:27:28.303258 magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/templates/NOTES.txt
+-rw-r--r--   0        0        0     4034 2023-06-29 14:27:28.303258 magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/templates/_helpers.tpl
+-rw-r--r--   0        0        0     2982 2023-06-29 14:27:28.403267 magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrole.yaml
+-rw-r--r--   0        0        0      534 2023-06-29 14:27:28.303258 magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrolebinding.yaml
+-rw-r--r--   0        0        0    13204 2023-06-29 14:27:28.303258 magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/templates/deployment.yaml
+-rw-r--r--   0        0        0      508 2023-06-29 14:27:28.303258 magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/templates/pdb.yaml
+-rw-r--r--   0        0        0      972 2023-06-29 14:27:28.303258 magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/templates/podsecuritypolicy.yaml
+-rw-r--r--   0        0        0      758 2023-06-29 14:27:28.303258 magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/templates/priority-expander-configmap.yaml
+-rw-r--r--   0        0        0      564 2023-06-29 14:27:28.303258 magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/templates/prometheusrule.yaml
+-rw-r--r--   0        0        0     1807 2023-06-29 14:27:28.303258 magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/templates/role.yaml
+-rw-r--r--   0        0        0      527 2023-06-29 14:27:28.303258 magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/templates/rolebinding.yaml
+-rw-r--r--   0        0        0      989 2023-06-29 14:27:28.303258 magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/templates/secret.yaml
+-rw-r--r--   0        0        0     1180 2023-06-29 14:27:28.303258 magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/templates/service.yaml
+-rw-r--r--   0        0        0      528 2023-06-29 14:27:28.303258 magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/templates/serviceaccount.yaml
+-rw-r--r--   0        0        0      960 2023-06-29 14:27:28.303258 magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/templates/servicemonitor.yaml
+-rw-r--r--   0        0        0      663 2023-06-29 14:27:28.303258 magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/templates/vpa.yaml
+-rw-r--r--   0        0        0    18003 2023-06-29 14:27:28.303258 magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/values.yaml
+-rw-r--r--   0        0        0     1977 2023-06-29 14:27:23.846611 magnum_cluster_api-0.7.0/magnum_cluster_api/clients.py
+-rw-r--r--   0        0        0        0 2023-06-29 14:27:23.846611 magnum_cluster_api-0.7.0/magnum_cluster_api/cmd/__init__.py
+-rw-r--r--   0        0        0     4019 2023-06-29 14:27:23.846611 magnum_cluster_api-0.7.0/magnum_cluster_api/cmd/image_builder.py
+-rw-r--r--   0        0        0     4714 2023-06-29 14:27:23.846611 magnum_cluster_api-0.7.0/magnum_cluster_api/cmd/image_loader.py
+-rw-r--r--   0        0        0      956 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/cmd/proxy.py
+-rw-r--r--   0        0        0     3278 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/conf.py
+-rw-r--r--   0        0        0    14251 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/driver.py
+-rw-r--r--   0        0        0     1219 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/exceptions.py
+-rw-r--r--   0        0        0     2888 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/helm.py
+-rw-r--r--   0        0        0     3464 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/image_utils.py
+-rw-r--r--   0        0        0     1116 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/images.py
+-rw-r--r--   0        0        0        0 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/__init__.py
+-rw-r--r--   0        0        0     4941 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/audit/policy.yaml
+-rw-r--r--   0        0        0   235191 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/calico/v3.24.2.yaml
+-rw-r--r--   0        0        0      623 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/ccm/cloud-controller-manager-role-bindings.yaml
+-rw-r--r--   0        0        0     1430 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/ccm/cloud-controller-manager-roles.yaml
+-rw-r--r--   0        0        0     2263 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/ccm/openstack-cloud-controller-manager-ds.yaml
+-rw-r--r--   0        0        0     4506 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/cinder-csi/cinder-csi-controllerplugin-rbac.yaml
+-rw-r--r--   0        0        0     4034 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/cinder-csi/cinder-csi-controllerplugin.yaml
+-rw-r--r--   0        0        0      609 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/cinder-csi/cinder-csi-nodeplugin-rbac.yaml
+-rw-r--r--   0        0        0     3307 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/cinder-csi/cinder-csi-nodeplugin.yaml
+-rw-r--r--   0        0        0      194 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/cinder-csi/csi-cinder-driver.yaml
+-rw-r--r--   0        0        0     3377 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/manila-csi/csi-controllerplugin-rbac.yaml
+-rw-r--r--   0        0        0     3944 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/manila-csi/csi-controllerplugin.yaml
+-rw-r--r--   0        0        0     1513 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/manila-csi/csi-nodeplugin-rbac.yaml
+-rw-r--r--   0        0        0     2988 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/manila-csi/csi-nodeplugin.yaml
+-rw-r--r--   0        0        0      143 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/manila-csi/csidriver.yaml
+-rw-r--r--   0        0        0     3127 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/nfs-csi/csi-nfs-controller.yaml
+-rw-r--r--   0        0        0      170 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/nfs-csi/csi-nfs-driverinfo.yaml
+-rw-r--r--   0        0        0     3530 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/nfs-csi/csi-nfs-node.yaml
+-rw-r--r--   0        0        0     1423 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/nfs-csi/rbac-csi-nfs.yaml
+-rw-r--r--   0        0        0     1526 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/monitor.py
+-rw-r--r--   0        0        0     5673 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/objects.py
+-rw-r--r--   0        0        0      828 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/privsep/__init__.py
+-rw-r--r--   0        0        0     1333 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/privsep/haproxy.py
+-rw-r--r--   0        0        0    11719 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/proxy/manager.py
+-rw-r--r--   0        0        0     3616 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/proxy/structs.py
+-rw-r--r--   0        0        0      580 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/proxy/templates/haproxy.cfg.j2
+-rw-r--r--   0        0        0     1511 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/proxy/utils.py
+-rw-r--r--   0        0        0    85235 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/resources.py
+-rw-r--r--   0        0        0     1492 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/service.py
+-rw-r--r--   0        0        0     3119 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/tests/functional/conftest.py
+-rw-r--r--   0        0        0      666 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/tests/functional/test_clusters.py
+-rw-r--r--   0        0        0      942 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/tests/unit/conftest.py
+-rw-r--r--   0        0        0     3453 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/tests/unit/test_helm.py
+-rw-r--r--   0        0        0     1731 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/tests/unit/test_image_utils.py
+-rw-r--r--   0        0        0     2759 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/tests/unit/test_images.py
+-rw-r--r--   0        0        0     5366 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/tests/unit/test_objects.py
+-rw-r--r--   0        0        0     1717 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/tests/unit/test_resources.py
+-rw-r--r--   0        0        0     1192 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/tests/unit/test_utils.py
+-rw-r--r--   0        0        0    10474 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/utils.py
+-rw-r--r--   0        0        0     1220 2023-06-29 14:27:23.854614 magnum_cluster_api-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     3890 1970-01-01 00:00:00.000000 magnum_cluster_api-0.7.0/PKG-INFO
```

### Comparing `magnum_cluster_api-0.6.0/LICENSE` & `magnum_cluster_api-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.6.0/README.md` & `magnum_cluster_api-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/README.md` & `magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/README.md`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/README.md.gotmpl` & `magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/README.md.gotmpl`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/templates/NOTES.txt` & `magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/templates/NOTES.txt`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/templates/_helpers.tpl` & `magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrole.yaml` & `magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrole.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrolebinding.yaml` & `magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrolebinding.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/templates/deployment.yaml` & `magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/templates/deployment.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/templates/podsecuritypolicy.yaml` & `magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/templates/podsecuritypolicy.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/templates/priority-expander-configmap.yaml` & `magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/templates/priority-expander-configmap.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/templates/prometheusrule.yaml` & `magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/templates/prometheusrule.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/templates/role.yaml` & `magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/templates/role.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/templates/rolebinding.yaml` & `magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/templates/rolebinding.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/templates/secret.yaml` & `magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/templates/secret.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/templates/service.yaml` & `magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/templates/service.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/templates/serviceaccount.yaml` & `magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/templates/serviceaccount.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/templates/servicemonitor.yaml` & `magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/templates/servicemonitor.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/templates/vpa.yaml` & `magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/templates/vpa.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/values.yaml` & `magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/values.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.6.0/magnum_cluster_api/clients.py` & `magnum_cluster_api-0.7.0/magnum_cluster_api/clients.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.6.0/magnum_cluster_api/cmd/image_builder.py` & `magnum_cluster_api-0.7.0/magnum_cluster_api/cmd/image_builder.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.6.0/magnum_cluster_api/cmd/image_loader.py` & `magnum_cluster_api-0.7.0/magnum_cluster_api/cmd/image_loader.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.6.0/magnum_cluster_api/cmd/proxy.py` & `magnum_cluster_api-0.7.0/magnum_cluster_api/cmd/proxy.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.6.0/magnum_cluster_api/conf.py` & `magnum_cluster_api-0.7.0/magnum_cluster_api/conf.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.6.0/magnum_cluster_api/driver.py` & `magnum_cluster_api-0.7.0/magnum_cluster_api/driver.py`

 * *Files 15% similar despite different names*

```diff
@@ -22,14 +22,21 @@
 
 
 class BaseDriver(driver.Driver):
     def __init__(self):
         self.k8s_api = clients.get_pykube_api()
 
     def create_cluster(self, context, cluster, cluster_create_timeout):
+        # NOTE(mnaser): We want to set the `stack_id` as early as possible to
+        #               make sure we can use it in the cluster creation.
+        cluster.stack_id = utils.generate_cluster_api_name(self.k8s_api)
+        cluster.save()
+
+        utils.validate_cluster(cluster)
+
         osc = clients.get_openstack_api(context)
 
         resources.Namespace(self.k8s_api).apply()
 
         credential = osc.keystone().client.application_credentials.create(
             user=cluster.user_id,
             name=cluster.uuid,
@@ -49,14 +56,40 @@
         resources.FrontProxyCertificateAuthoritySecret(self.k8s_api, cluster).apply()
         resources.ServiceAccountCertificateAuthoritySecret(
             self.k8s_api, cluster
         ).apply()
 
         resources.apply_cluster_from_magnum_cluster(context, self.k8s_api, cluster)
 
+    def _get_cluster_status_reason(self, capi_cluster):
+        capi_cluster_status_reason = ""
+        capi_ops_cluster_status_reason = ""
+
+        # Get the latest event message of the CAPI Cluster
+        capi_cluster_events = capi_cluster.events
+        if capi_cluster_events:
+            capi_cluster_status_reason += utils.format_event_message(
+                list(capi_cluster_events)[-1]
+            )
+
+        # Get the latest event message of the CAPI OpenstackCluster
+        capi_ops_cluster_events = []
+        capi_ops_cluster = capi_cluster.openstack_cluster
+        if capi_ops_cluster:
+            capi_ops_cluster_events = capi_ops_cluster.events
+        if capi_ops_cluster_events:
+            capi_ops_cluster_status_reason += utils.format_event_message(
+                list(capi_ops_cluster_events)[-1]
+            )
+
+        return "CAPI Cluster status: %s. CAPI OpenstackCluster status reason: %s" % (
+            capi_cluster_status_reason,
+            capi_ops_cluster_status_reason,
+        )
+
     def update_cluster_status(self, context, cluster, use_admin_ctx=False):
         node_groups = [
             self.update_nodegroup_status(context, cluster, node_group)
             for node_group in cluster.nodegroups
         ]
         # TODO: watch for topology change instead
         osc = clients.get_openstack_api(context)
@@ -76,14 +109,18 @@
             capi_cluster.reload()
             status_map = {
                 c["type"]: c["status"] for c in capi_cluster.obj["status"]["conditions"]
             }
 
             for condition in ("ControlPlaneReady", "InfrastructureReady", "Ready"):
                 if status_map.get(condition) != "True":
+                    cluster.status_reason = self._get_cluster_status_reason(
+                        capi_cluster
+                    )
+                    cluster.save()
                     return
 
             api_endpoint = capi_cluster.obj["spec"]["controlPlaneEndpoint"]
             cluster.api_address = (
                 f"https://{api_endpoint['host']}:{api_endpoint['port']}"
             )
             cluster.coe_version = capi_cluster.obj["spec"]["topology"]["version"]
@@ -91,22 +128,26 @@
             for ng in node_groups:
                 if not ng.status.endswith("_COMPLETE"):
                     return
                 if ng.status == "DELETE_COMPLETE":
                     ng.destroy()
 
             if cluster.status == "CREATE_IN_PROGRESS":
+                cluster.status_reason = None
                 cluster.status = "CREATE_COMPLETE"
             if cluster.status == "UPDATE_IN_PROGRESS":
+                cluster.status_reason = None
                 cluster.status = "UPDATE_COMPLETE"
 
             cluster.save()
 
         if cluster.status == "DELETE_IN_PROGRESS":
             if capi_cluster and capi_cluster.exists():
+                cluster.status_reason = self._get_cluster_status_reason(capi_cluster)
+                cluster.save()
                 return
 
             # NOTE(mnaser): We delete the application credentials at this stage
             #               to make sure CAPI doesn't lose access to OpenStack.
             try:
                 osc.keystone().client.application_credentials.find(
                     name=cluster.uuid,
@@ -121,14 +162,15 @@
             resources.FrontProxyCertificateAuthoritySecret(
                 self.k8s_api, cluster
             ).delete()
             resources.ServiceAccountCertificateAuthoritySecret(
                 self.k8s_api, cluster
             ).delete()
 
+            cluster.status_reason = None
             cluster.status = "DELETE_COMPLETE"
             cluster.save()
 
     def update_cluster(self, context, cluster, scale_manager=None, rollback=False):
         raise NotImplementedError()
 
     def resize_cluster(
@@ -136,24 +178,24 @@
         context,
         cluster,
         resize_manager,
         node_count,
         nodes_to_remove,
         nodegroup=None,
     ):
+        utils.validate_cluster(cluster)
+
         if nodegroup is None:
             nodegroup = cluster.default_ng_worker
 
         if nodes_to_remove:
             machines = objects.Machine.objects(self.k8s_api).filter(
                 namespace="magnum-system",
                 selector={
-                    "cluster.x-k8s.io/cluster-name": utils.get_or_generate_cluster_api_name(
-                        self.k8s_api, cluster
-                    ),
+                    "cluster.x-k8s.io/cluster-name": cluster.stack_id,
                     "topology.cluster.x-k8s.io/deployment-name": nodegroup.name,
                 },
             )
 
             for machine in machines:
                 instance_uuid = machine.obj["spec"]["providerID"].split("/")[-1]
                 if instance_uuid in nodes_to_remove:
@@ -210,14 +252,16 @@
             context, self.k8s_api, cluster
         ).get_observed_generation()
         if old_generation != current_generation:
             return
         raise exceptions.ClusterAPIReconcileTimeout()
 
     def delete_cluster(self, context, cluster):
+        if cluster.stack_id is None:
+            return
         # NOTE(mnaser): This should be removed when this is fixed:
         #
         #               https://github.com/kubernetes-sigs/cluster-api-provider-openstack/issues/842
         #               https://github.com/kubernetes-sigs/cluster-api-provider-openstack/pull/990
         utils.delete_loadbalancers(context, cluster)
 
         resources.ClusterResourceSet(self.k8s_api, cluster).delete()
@@ -278,15 +322,23 @@
         nodegroup.save()
 
         return nodegroup
 
     def update_nodegroup(self, context, cluster, nodegroup):
         # TODO
 
+        # NOTE(okozachenko1203): First we save the nodegroup status because update_cluster_status()
+        #                        could be finished before update_nodegroup().
+        nodegroup.save()
         resources.apply_cluster_from_magnum_cluster(context, self.k8s_api, cluster)
+        # NOTE(okozachenko1203): We set the cluster status as UPDATE_IN_PROGRESS again at the end because
+        #                        update_cluster_status() could be finished and cluster status has been set as
+        #                        UPDATE_COMPLETE before nodegroup_conductor.Handler.nodegroup_update finished.
+        cluster.status = "UPDATE_IN_PROGRESS"
+        cluster.save()
 
     def delete_nodegroup(self, context, cluster, nodegroup):
         nodegroup.status = "DELETE_IN_PROGRESS"
         nodegroup.save()
 
         resources.apply_cluster_from_magnum_cluster(
             context,
```

### Comparing `magnum_cluster_api-0.6.0/magnum_cluster_api/exceptions.py` & `magnum_cluster_api-0.7.0/magnum_cluster_api/exceptions.py`

 * *Files 12% similar despite different names*

```diff
@@ -43,7 +43,11 @@
 
 class OpenStackClusterSubnetNotReady(OpenStackClusterNotReady):
     pass
 
 
 class ClusterAPIReconcileTimeout(Exception):
     pass
+
+
+class ClusterMasterCountEven(Exception):
+    pass
```

### Comparing `magnum_cluster_api-0.6.0/magnum_cluster_api/helm.py` & `magnum_cluster_api-0.7.0/magnum_cluster_api/helm.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.6.0/magnum_cluster_api/image_utils.py` & `magnum_cluster_api-0.7.0/magnum_cluster_api/image_utils.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.6.0/magnum_cluster_api/images.py` & `magnum_cluster_api-0.7.0/magnum_cluster_api/images.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.6.0/magnum_cluster_api/manifests/audit/policy.yaml` & `magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/audit/policy.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.6.0/magnum_cluster_api/manifests/calico/v3.24.2.yaml` & `magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/calico/v3.24.2.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.6.0/magnum_cluster_api/manifests/ccm/cloud-controller-manager-role-bindings.yaml` & `magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/ccm/cloud-controller-manager-role-bindings.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.6.0/magnum_cluster_api/manifests/ccm/cloud-controller-manager-roles.yaml` & `magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/ccm/cloud-controller-manager-roles.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.6.0/magnum_cluster_api/manifests/ccm/openstack-cloud-controller-manager-ds.yaml` & `magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/ccm/openstack-cloud-controller-manager-ds.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.6.0/magnum_cluster_api/manifests/cinder-csi/cinder-csi-controllerplugin-rbac.yaml` & `magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/cinder-csi/cinder-csi-controllerplugin-rbac.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.6.0/magnum_cluster_api/manifests/cinder-csi/cinder-csi-controllerplugin.yaml` & `magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/cinder-csi/cinder-csi-controllerplugin.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.6.0/magnum_cluster_api/manifests/cinder-csi/cinder-csi-nodeplugin-rbac.yaml` & `magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/cinder-csi/cinder-csi-nodeplugin-rbac.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.6.0/magnum_cluster_api/manifests/cinder-csi/cinder-csi-nodeplugin.yaml` & `magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/cinder-csi/cinder-csi-nodeplugin.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.6.0/magnum_cluster_api/manifests/manila-csi/csi-controllerplugin-rbac.yaml` & `magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/manila-csi/csi-controllerplugin-rbac.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.6.0/magnum_cluster_api/manifests/manila-csi/csi-controllerplugin.yaml` & `magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/manila-csi/csi-controllerplugin.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.6.0/magnum_cluster_api/manifests/manila-csi/csi-nodeplugin-rbac.yaml` & `magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/manila-csi/csi-nodeplugin-rbac.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.6.0/magnum_cluster_api/manifests/manila-csi/csi-nodeplugin.yaml` & `magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/manila-csi/csi-nodeplugin.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.6.0/magnum_cluster_api/manifests/nfs-csi/csi-nfs-controller.yaml` & `magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/nfs-csi/csi-nfs-controller.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.6.0/magnum_cluster_api/manifests/nfs-csi/csi-nfs-node.yaml` & `magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/nfs-csi/csi-nfs-node.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.6.0/magnum_cluster_api/manifests/nfs-csi/rbac-csi-nfs.yaml` & `magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/nfs-csi/rbac-csi-nfs.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.6.0/magnum_cluster_api/monitor.py` & `magnum_cluster_api-0.7.0/magnum_cluster_api/monitor.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.6.0/magnum_cluster_api/objects.py` & `magnum_cluster_api-0.7.0/magnum_cluster_api/objects.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,69 +18,81 @@
 import pykube
 import yaml
 from oslo_serialization import base64
 
 from magnum_cluster_api import exceptions
 
 
-class EndpointSlice(pykube.objects.NamespacedAPIObject):
+class NamespacedAPIObject(pykube.objects.NamespacedAPIObject):
+    @property
+    def events(self):
+        return pykube.Event.objects(self.api, namespace=self.namespace).filter(
+            field_selector={
+                "involvedObject.name": self.name,
+                "involvedObject.apiVersion": self.version,
+                "involvedObject.kind": self.kind,
+            },
+        )
+
+
+class EndpointSlice(NamespacedAPIObject):
     version = "discovery.k8s.io/v1"
     endpoint = "endpointslices"
     kind = "EndpointSlice"
 
 
-class ClusterResourceSet(pykube.objects.NamespacedAPIObject):
+class ClusterResourceSet(NamespacedAPIObject):
     version = "addons.cluster.x-k8s.io/v1beta1"
     endpoint = "clusterresourcesets"
     kind = "ClusterResourceSet"
 
 
-class OpenStackMachineTemplate(pykube.objects.NamespacedAPIObject):
+class OpenStackMachineTemplate(NamespacedAPIObject):
     version = "infrastructure.cluster.x-k8s.io/v1alpha6"
     endpoint = "openstackmachinetemplates"
     kind = "OpenStackMachineTemplate"
 
 
-class KubeadmConfigTemplate(pykube.objects.NamespacedAPIObject):
+class KubeadmConfigTemplate(NamespacedAPIObject):
     version = "bootstrap.cluster.x-k8s.io/v1beta1"
     endpoint = "kubeadmconfigtemplates"
     kind = "KubeadmConfigTemplate"
 
 
-class KubeadmControlPlane(pykube.objects.NamespacedAPIObject):
+class KubeadmControlPlane(NamespacedAPIObject):
     version = "controlplane.cluster.x-k8s.io/v1beta1"
     endpoint = "kubeadmcontrolplanes"
     kind = "KubeadmControlPlane"
 
 
-class KubeadmControlPlaneTemplate(pykube.objects.NamespacedAPIObject):
+class KubeadmControlPlaneTemplate(NamespacedAPIObject):
     version = "controlplane.cluster.x-k8s.io/v1beta1"
     endpoint = "kubeadmcontrolplanetemplates"
     kind = "KubeadmControlPlaneTemplate"
 
 
-class MachineDeployment(pykube.objects.NamespacedAPIObject):
+class MachineDeployment(NamespacedAPIObject):
     version = "cluster.x-k8s.io/v1beta1"
     endpoint = "machinedeployments"
     kind = "MachineDeployment"
 
 
-class Machine(pykube.objects.NamespacedAPIObject):
+class Machine(NamespacedAPIObject):
     version = "cluster.x-k8s.io/v1beta1"
     endpoint = "machines"
     kind = "Machine"
 
 
-class OpenStackClusterTemplate(pykube.objects.NamespacedAPIObject):
+class OpenStackClusterTemplate(NamespacedAPIObject):
     version = "infrastructure.cluster.x-k8s.io/v1alpha6"
     endpoint = "openstackclustertemplates"
     kind = "OpenStackClusterTemplate"
 
 
-class OpenStackCluster(pykube.objects.NamespacedAPIObject):
+class OpenStackCluster(NamespacedAPIObject):
     version = "infrastructure.cluster.x-k8s.io/v1alpha6"
     endpoint = "openstackclusters"
     kind = "OpenStackCluster"
 
     @property
     def identity_ref(self):
         return self.obj["spec"]["identityRef"]
@@ -144,21 +156,21 @@
 
         fd = io.StringIO()
         config.write(fd)
 
         return fd.getvalue()
 
 
-class ClusterClass(pykube.objects.NamespacedAPIObject):
+class ClusterClass(NamespacedAPIObject):
     version = "cluster.x-k8s.io/v1beta1"
     endpoint = "clusterclasses"
     kind = "ClusterClass"
 
 
-class Cluster(pykube.objects.NamespacedAPIObject):
+class Cluster(NamespacedAPIObject):
     version = "cluster.x-k8s.io/v1beta1"
     endpoint = "clusters"
     kind = "Cluster"
 
     @property
     def openstack_cluster(self):
         filtered_clusters = (
@@ -166,14 +178,14 @@
             .filter(selector={"cluster.x-k8s.io/cluster-name": self.name})
             .all()
         )
 
         if len(filtered_clusters) == 0:
             raise exceptions.OpenStackClusterNotCreated()
 
-        return filtered_clusters[0]
+        return list(filtered_clusters)[0]
 
 
 class StorageClass(pykube.objects.APIObject):
     version = "storage.k8s.io/v1"
     endpoint = "storageclasses"
     kind = "StorageClass"
```

### Comparing `magnum_cluster_api-0.6.0/magnum_cluster_api/privsep/__init__.py` & `magnum_cluster_api-0.7.0/magnum_cluster_api/privsep/__init__.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.6.0/magnum_cluster_api/privsep/haproxy.py` & `magnum_cluster_api-0.7.0/magnum_cluster_api/privsep/haproxy.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.6.0/magnum_cluster_api/proxy/manager.py` & `magnum_cluster_api-0.7.0/magnum_cluster_api/proxy/manager.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.6.0/magnum_cluster_api/proxy/structs.py` & `magnum_cluster_api-0.7.0/magnum_cluster_api/proxy/structs.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.6.0/magnum_cluster_api/proxy/templates/haproxy.cfg.j2` & `magnum_cluster_api-0.7.0/magnum_cluster_api/proxy/templates/haproxy.cfg.j2`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.6.0/magnum_cluster_api/proxy/utils.py` & `magnum_cluster_api-0.7.0/magnum_cluster_api/proxy/utils.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.6.0/magnum_cluster_api/resources.py` & `magnum_cluster_api-0.7.0/magnum_cluster_api/resources.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,48 +47,47 @@
 
 AUTOSCALE_ANNOTATION_MIN = "cluster.x-k8s.io/cluster-api-autoscaler-node-group-min-size"
 AUTOSCALE_ANNOTATION_MAX = "cluster.x-k8s.io/cluster-api-autoscaler-node-group-max-size"
 
 
 class ClusterAutoscalerHelmRelease:
     def __init__(self, api, cluster) -> None:
-        cluster_name = utils.get_or_generate_cluster_api_name(api, cluster)
         image = images.get_cluster_autoscaler_image(
             utils.get_kube_tag(cluster),
         )
         image_repo, image_tag = image.split(":", 1)
 
         self.apply = helm.UpgradeReleaseCommand(
             namespace="magnum-system",
-            release_name=cluster_name,
+            release_name=cluster.stack_id,
             chart_ref=os.path.join(
                 pkg_resources.resource_filename("magnum_cluster_api", "charts"),
                 "cluster-autoscaler/",
             ),
             values={
-                "fullnameOverride": f"{cluster_name}-autoscaler",
+                "fullnameOverride": f"{cluster.stack_id}-autoscaler",
                 "cloudProvider": "clusterapi",
                 "clusterAPIMode": "kubeconfig-incluster",
-                "clusterAPIKubeconfigSecret": f"{cluster_name}-kubeconfig",
+                "clusterAPIKubeconfigSecret": f"{cluster.stack_id}-kubeconfig",
                 "autoDiscovery": {
-                    "clusterName": cluster_name,
+                    "clusterName": cluster.stack_id,
                 },
                 "image": {
                     "repository": image_repo,
                     "tag": image_tag,
                 },
                 "nodeSelector": {
                     "openstack-control-plane": "enabled",
                 },
             },
         )
 
         self.delete = helm.DeleteReleaseCommand(
             namespace="magnum-system",
-            release_name=cluster_name,
+            release_name=cluster.stack_id,
             skip_missing=True,
         )
 
 
 class Base:
     def __init__(self, api: pykube.HTTPClient):
         self.api = api
@@ -380,28 +379,42 @@
                     ],
                 },
             },
         )
 
 
 class CertificateAuthoritySecret(ClusterBase):
+    def delete(self) -> None:
+        resource = self.get_or_none()
+        if resource:
+            resource.delete()
+
+    def get_or_none(self) -> pykube.Secret:
+        return pykube.Secret.objects(self.api, namespace="magnum-system").get_or_none(
+            name=f"{self.cluster.stack_id}-{self.CERT}"
+        )
+
     def get_object(self) -> pykube.Secret:
+        cert_ref = getattr(self.cluster, self.REF)
+        if cert_ref is None:
+            raise Exception("Certificate for %s doesn't exist." % self.REF)
+
         ca_cert = cert_manager.get_backend().CertManager.get_cert(
-            getattr(self.cluster, self.REF),
+            cert_ref,
             resource_ref=self.cluster.uuid,
         )
 
         return pykube.Secret(
             self.api,
             {
                 "apiVersion": pykube.Secret.version,
                 "kind": pykube.Secret.kind,
                 "type": "kubernetes.io/tls",
                 "metadata": {
-                    "name": f"{utils.get_or_generate_cluster_api_name(self.api, self.cluster)}-{self.CERT}",
+                    "name": f"{self.cluster.stack_id}-{self.CERT}",
                     "namespace": "magnum-system",
                 },
                 "stringData": {
                     "tls.crt": encodeutils.safe_decode(ca_cert.get_certificate()),
                     "tls.key": encodeutils.safe_decode(
                         x509.decrypt_key(
                             ca_cert.get_private_key(),
@@ -734,14 +747,51 @@
                                             "type": "boolean",
                                         },
                                     },
                                 },
                             },
                         },
                         {
+                            "name": "openidConnect",
+                            "required": True,
+                            "schema": {
+                                "openAPIV3Schema": {
+                                    "type": "object",
+                                    "required": [
+                                        "issuerUrl",
+                                        "clientId",
+                                        "usernameClaim",
+                                        "usernamePrefix",
+                                        "groupsClaim",
+                                        "groupsPrefix",
+                                    ],
+                                    "properties": {
+                                        "issuerUrl": {
+                                            "type": "string",
+                                        },
+                                        "clientId": {
+                                            "type": "string",
+                                        },
+                                        "usernameClaim": {
+                                            "type": "string",
+                                        },
+                                        "usernamePrefix": {
+                                            "type": "string",
+                                        },
+                                        "groupsClaim": {
+                                            "type": "string",
+                                        },
+                                        "groupsPrefix": {
+                                            "type": "string",
+                                        },
+                                    },
+                                },
+                            },
+                        },
+                        {
                             "name": "auditLog",
                             "required": True,
                             "schema": {
                                 "openAPIV3Schema": {
                                     "type": "object",
                                     "required": [
                                         "enabled",
@@ -983,14 +1033,73 @@
                                             },
                                         },
                                     ],
                                 }
                             ],
                         },
                         {
+                            "name": "openidConnect",
+                            "enabledIf": "{{ if .openidConnect.issuerUrl }}true{{end}}",
+                            "definitions": [
+                                {
+                                    "selector": {
+                                        "apiVersion": objects.KubeadmControlPlaneTemplate.version,
+                                        "kind": objects.KubeadmControlPlaneTemplate.kind,
+                                        "matchResources": {
+                                            "controlPlane": True,
+                                        },
+                                    },
+                                    "jsonPatches": [
+                                        {
+                                            "op": "add",
+                                            "path": "/spec/template/spec/kubeadmConfigSpec/clusterConfiguration/apiServer/extraArgs/oidc-issuer-url",  # noqa: E501
+                                            "valueFrom": {
+                                                "variable": "openidConnect.issuerUrl",
+                                            },
+                                        },
+                                        {
+                                            "op": "add",
+                                            "path": "/spec/template/spec/kubeadmConfigSpec/clusterConfiguration/apiServer/extraArgs/oidc-client-id",  # noqa: E501
+                                            "valueFrom": {
+                                                "variable": "openidConnect.clientId",
+                                            },
+                                        },
+                                        {
+                                            "op": "add",
+                                            "path": "/spec/template/spec/kubeadmConfigSpec/clusterConfiguration/apiServer/extraArgs/oidc-username-claim",  # noqa: E501
+                                            "valueFrom": {
+                                                "variable": "openidConnect.usernameClaim",
+                                            },
+                                        },
+                                        {
+                                            "op": "add",
+                                            "path": "/spec/template/spec/kubeadmConfigSpec/clusterConfiguration/apiServer/extraArgs/oidc-username-prefix",  # noqa: E501
+                                            "valueFrom": {
+                                                "variable": "openidConnect.usernamePrefix",
+                                            },
+                                        },
+                                        {
+                                            "op": "add",
+                                            "path": "/spec/template/spec/kubeadmConfigSpec/clusterConfiguration/apiServer/extraArgs/oidc-groups-claim",  # noqa: E501
+                                            "valueFrom": {
+                                                "variable": "openidConnect.groupsClaim",
+                                            },
+                                        },
+                                        {
+                                            "op": "add",
+                                            "path": "/spec/template/spec/kubeadmConfigSpec/clusterConfiguration/apiServer/extraArgs/oidc-groups-prefix",  # noqa: E501
+                                            "valueFrom": {
+                                                "variable": "openidConnect.groupsPrefix",
+                                            },
+                                        },
+                                    ],
+                                }
+                            ],
+                        },
+                        {
                             "name": "bootVolume",
                             "enabledIf": "{{ if gt .bootVolume.size 0.0 }}true{{end}}",
                             "definitions": [
                                 {
                                     "selector": {
                                         "apiVersion": objects.OpenStackMachineTemplate.version,
                                         "kind": objects.OpenStackMachineTemplate.kind,
@@ -1438,15 +1547,15 @@
             )
             labels["manila-csi-version"] = manila_version
 
         return {**super().labels, **labels}
 
     def get_or_none(self) -> objects.Cluster:
         return objects.Cluster.objects(self.api, namespace="magnum-system").get_or_none(
-            name=utils.get_or_generate_cluster_api_name(self.api, self.cluster)
+            name=self.cluster.stack_id
         )
 
     def get_observed_generation(self) -> int:
         capi_cluster = self.get_or_none()
         if capi_cluster:
             return capi_cluster.obj["status"]["observedGeneration"]
         raise Exception("Cluster doesn't exists.")
@@ -1454,17 +1563,15 @@
     def get_object(self) -> objects.Cluster:
         return objects.Cluster(
             self.api,
             {
                 "apiVersion": objects.Cluster.version,
                 "kind": objects.Cluster.kind,
                 "metadata": {
-                    "name": utils.get_or_generate_cluster_api_name(
-                        self.api, self.cluster
-                    ),
+                    "name": self.cluster.stack_id,
                     "namespace": "magnum-system",
                     "labels": self.labels,
                 },
                 "spec": {
                     "clusterNetwork": {
                         "serviceDomain": utils.get_cluster_label(
                             self.cluster,
@@ -1510,14 +1617,37 @@
                             {
                                 "name": "apiServerLoadBalancer",
                                 "value": {
                                     "enabled": self.cluster.master_lb_enabled,
                                 },
                             },
                             {
+                                "name": "openidConnect",
+                                "value": {
+                                    "clientId": utils.get_cluster_label(
+                                        self.cluster, "oidc_client_id", ""
+                                    ),
+                                    "groupsClaim": utils.get_cluster_label(
+                                        self.cluster, "oidc_groups_claim", ""
+                                    ),
+                                    "groupsPrefix": utils.get_cluster_label(
+                                        self.cluster, "oidc_groups_prefix", ""
+                                    ),
+                                    "issuerUrl": utils.get_cluster_label(
+                                        self.cluster, "oidc_issuer_url", ""
+                                    ),
+                                    "usernameClaim": utils.get_cluster_label(
+                                        self.cluster, "oidc_username_claim", "sub"
+                                    ),
+                                    "usernamePrefix": utils.get_cluster_label(
+                                        self.cluster, "oidc_username_prefix", "-"
+                                    ),
+                                },
+                            },
+                            {
                                 "name": "auditLog",
                                 "value": {
                                     "enabled": utils.get_cluster_label_as_bool(
                                         self.cluster, "audit_log_enabled", False
                                     ),
                                     "maxAge": utils.get_cluster_label(
                                         self.cluster, "audit_log_max_age", "30"
@@ -1652,17 +1782,15 @@
     nodegroup: magnum_objects.NodeGroup,
 ):
     if not utils.get_auto_scaling_enabled(cluster):
         return
     mds = objects.MachineDeployment.objects(api).filter(
         namespace="magnum-system",
         selector={
-            "cluster.x-k8s.io/cluster-name": utils.get_or_generate_cluster_api_name(
-                api, cluster
-            ),
+            "cluster.x-k8s.io/cluster-name": cluster.stack_id,
             "topology.cluster.x-k8s.io/deployment-name": nodegroup.name,
         },
     )
     for md in mds:
         # NOTE(mnaser): The autoscaler will not scale under the minimum number
         #               of nodes, so we do that ourselves here.
         if AUTOSCALE_ANNOTATION_MIN not in md.obj["metadata"]["annotations"]:
@@ -1712,33 +1840,29 @@
 
 
 def get_kubeadm_control_plane(
     api: pykube.HTTPClient, cluster: magnum_objects.Cluster
 ) -> objects.KubeadmControlPlane:
     kcps = objects.KubeadmControlPlane.objects(api, namespace="magnum-system").filter(
         selector={
-            "cluster.x-k8s.io/cluster-name": utils.get_or_generate_cluster_api_name(
-                api, cluster
-            )
+            "cluster.x-k8s.io/cluster-name": cluster.stack_id,
         },
     )
     if len(kcps) == 1:
         return list(kcps)[0]
     return None
 
 
 def get_machine_deployment(
     api: pykube.HTTPClient,
     cluster: magnum_objects.Cluster,
     node_group: magnum_objects.NodeGroup,
 ) -> objects.KubeadmControlPlane:
     mds = objects.MachineDeployment.objects(api, namespace="magnum-system").filter(
         selector={
-            "cluster.x-k8s.io/cluster-name": utils.get_or_generate_cluster_api_name(
-                api, cluster
-            ),
+            "cluster.x-k8s.io/cluster-name": cluster.stack_id,
             "topology.cluster.x-k8s.io/deployment-name": node_group.name,
         },
     )
     if len(mds) == 1:
         return list(mds)[0]
     return None
```

### Comparing `magnum_cluster_api-0.6.0/magnum_cluster_api/service.py` & `magnum_cluster_api-0.7.0/magnum_cluster_api/service.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.6.0/magnum_cluster_api/tests/functional/conftest.py` & `magnum_cluster_api-0.7.0/magnum_cluster_api/tests/functional/conftest.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.6.0/magnum_cluster_api/tests/functional/test_clusters.py` & `magnum_cluster_api-0.7.0/magnum_cluster_api/tests/functional/test_clusters.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.6.0/magnum_cluster_api/tests/unit/conftest.py` & `magnum_cluster_api-0.7.0/magnum_cluster_api/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.6.0/magnum_cluster_api/tests/unit/test_helm.py` & `magnum_cluster_api-0.7.0/magnum_cluster_api/tests/unit/test_helm.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.6.0/magnum_cluster_api/tests/unit/test_image_utils.py` & `magnum_cluster_api-0.7.0/magnum_cluster_api/tests/unit/test_image_utils.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.6.0/magnum_cluster_api/tests/unit/test_images.py` & `magnum_cluster_api-0.7.0/magnum_cluster_api/tests/unit/test_images.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.6.0/magnum_cluster_api/tests/unit/test_objects.py` & `magnum_cluster_api-0.7.0/magnum_cluster_api/tests/unit/test_objects.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.6.0/magnum_cluster_api/tests/unit/test_resources.py` & `magnum_cluster_api-0.7.0/magnum_cluster_api/tests/unit/test_resources.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.6.0/magnum_cluster_api/tests/unit/test_utils.py` & `magnum_cluster_api-0.7.0/magnum_cluster_api/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.6.0/magnum_cluster_api/utils.py` & `magnum_cluster_api-0.7.0/magnum_cluster_api/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,32 +23,25 @@
 from magnum.common import context, exception, octavia
 from magnum.common.keystone import KeystoneClientV3
 from oslo_log import log as logging
 from oslo_serialization import base64
 from oslo_utils import strutils
 from tenacity import retry, retry_if_exception_type
 
-from magnum_cluster_api import clients, image_utils, images, objects
+from magnum_cluster_api import clients
+from magnum_cluster_api import exceptions as mcapi_exceptions
+from magnum_cluster_api import image_utils, images, objects
 
 LOG = logging.getLogger(__name__)
 
 
 def get_or_generate_cluster_api_cloud_config_secret_name(
     api: pykube.HTTPClient, cluster: magnum_objects.Cluster
 ) -> str:
-    return f"{get_or_generate_cluster_api_name(api, cluster)}-cloud-config"
-
-
-def get_or_generate_cluster_api_name(
-    api: pykube.HTTPClient, cluster: magnum_objects.Cluster
-) -> str:
-    if cluster.stack_id is None:
-        cluster.stack_id = generate_cluster_api_name(api)
-        cluster.save()
-    return cluster.stack_id
+    return f"{cluster.stack_id}-cloud-config"
 
 
 @retry(retry=retry_if_exception_type(exception.Conflict))
 def generate_cluster_api_name(
     api: pykube.HTTPClient,
 ) -> str:
     alphabet = string.ascii_lowercase + string.digits
@@ -314,7 +307,20 @@
 
 
 def is_manila_csi_enabled(cluster: magnum_objects.Cluster) -> bool:
     return (
         get_cluster_label_as_bool(cluster, "manila_csi_enabled", True)
         and is_manila_enabled()
     )
+
+
+def format_event_message(event: pykube.Event):
+    return "%s: %s" % (
+        event.obj["reason"],
+        event.obj["message"],
+    )
+
+
+def validate_cluster(cluster: magnum_objects.Cluster):
+    # Check master count
+    if (cluster.master_count % 2) == 0:
+        raise mcapi_exceptions.ClusterMasterCountEven
```

### Comparing `magnum_cluster_api-0.6.0/pyproject.toml` & `magnum_cluster_api-0.7.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "magnum-cluster-api"
-version = "0.6.0"
+version = "0.7.0"
 description = "Cluster API driver for Magnum"
 authors = ["Mohammed Naser <mnaser@vexxhost.com>"]
 readme = "README.md"
 packages = [{include = "magnum_cluster_api"}]
 include = ["magnum_cluster_api/charts/**/*"]
 
 [tool.poetry.dependencies]
```

### Comparing `magnum_cluster_api-0.6.0/PKG-INFO` & `magnum_cluster_api-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magnum-cluster-api
-Version: 0.6.0
+Version: 0.7.0
 Summary: Cluster API driver for Magnum
 Author: Mohammed Naser
 Author-email: mnaser@vexxhost.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

