# Comparing `tmp/solutions_template-1.10.0.tar.gz` & `tmp/solutions_template-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solutions_template-1.10.0.tar", max compression
+gzip compressed data, was "solutions_template-1.9.0.tar", max compression
```

## Comparing `solutions_template-1.10.0.tar` & `solutions_template-1.9.0.tar`

### file list

```diff
@@ -1,195 +1,146 @@
--rw-r--r--   0        0        0    11358 2022-06-28 21:05:37.723277 solutions_template-1.10.0/LICENSE
--rw-r--r--   0        0        0     4838 2023-06-27 16:32:20.325913 solutions_template-1.10.0/README.md
--rw-r--r--   0        0        0     1132 2023-06-29 19:09:14.201007 solutions_template-1.10.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-15 16:31:59.883150 solutions_template-1.10.0/solutions_template/__init__.py
--rw-r--r--   0        0        0        0 2023-06-21 14:30:18.509259 solutions_template-1.10.0/solutions_template/cli/__init__.py
--rw-r--r--   0        0        0     6031 2023-06-27 18:52:04.573796 solutions_template-1.10.0/solutions_template/cli/cli.py
--rw-r--r--   0        0        0     4199 2023-06-15 16:31:59.883928 solutions_template-1.10.0/solutions_template/cli/cli_utils.py
--rw-r--r--   0        0        0     6046 2023-06-27 16:32:20.328616 solutions_template-1.10.0/solutions_template/cli/component.py
--rw-r--r--   0        0        0     5883 2023-06-20 16:37:06.248359 solutions_template-1.10.0/solutions_template/cli/infra.py
--rw-r--r--   0        0        0     1417 2023-06-27 16:32:20.329088 solutions_template-1.10.0/solutions_template/cli/template.py
--rw-r--r--   0        0        0        0 2023-06-15 16:31:59.884916 solutions_template-1.10.0/solutions_template/copier_extensions/__init__.py
--rw-r--r--   0        0        0     4703 2023-06-21 14:30:18.510643 solutions_template-1.10.0/solutions_template/copier_extensions/st_helpers.py
--rw-r--r--   0        0        0      101 2023-06-27 16:32:20.329504 solutions_template-1.10.0/solutions_template/module_template/.st/module_answers/{{'{{component_name}}'}}.yaml
--rw-r--r--   0        0        0      766 2023-06-27 16:32:20.329809 solutions_template-1.10.0/solutions_template/module_template/README.md
--rw-r--r--   0        0        0      865 2023-06-27 16:32:20.330046 solutions_template-1.10.0/solutions_template/module_template/copier.yaml
--rw-r--r--   0        0        0       89 2023-06-27 16:32:20.330491 solutions_template-1.10.0/solutions_template/module_template/docs/components/{{'{{component_name}}'}}.md
--rw-r--r--   0        0        0     1135 2023-06-27 16:32:20.330828 solutions_template-1.10.0/solutions_template/module_template/template_copier.yaml
--rw-r--r--   0        0        0     3878 2023-06-27 16:32:20.331156 solutions_template-1.10.0/solutions_template/module_template/{{"{{'.github' if use_github_action}}"}}/workflows/{{"unit_test_linter_{{component_name}}"}}.yaml
--rw-r--r--   0        0        0      566 2023-06-27 16:32:20.331543 solutions_template-1.10.0/solutions_template/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/Dockerfile
--rw-r--r--   0        0        0      109 2023-06-27 16:32:20.331896 solutions_template-1.10.0/solutions_template/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/requirements.txt
--rw-r--r--   0        0        0     3204 2023-06-27 18:51:03.011753 solutions_template-1.10.0/solutions_template/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/skaffold.yaml
--rw-r--r--   0        0        0      590 2023-06-27 16:32:20.332297 solutions_template-1.10.0/solutions_template/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/src/main.py
--rw-r--r--   0        0        0       81 2023-06-27 16:32:20.332629 solutions_template-1.10.0/solutions_template/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/st_module.yaml
--rw-r--r--   0        0        0      736 2023-06-27 16:32:20.332955 solutions_template-1.10.0/solutions_template/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/backend.tf
--rw-r--r--   0        0        0      636 2023-06-27 16:32:20.333135 solutions_template-1.10.0/solutions_template/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/main.tf
--rw-r--r--   0        0        0      836 2023-06-27 16:32:20.333605 solutions_template-1.10.0/solutions_template/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/providers.tf
--rw-r--r--   0        0        0      777 2023-06-27 16:32:20.333871 solutions_template-1.10.0/solutions_template/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/terraform.tfvars
--rw-r--r--   0        0        0      858 2023-06-27 16:32:20.334058 solutions_template-1.10.0/solutions_template/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/variables.tf
--rw-r--r--   0        0        0       80 2023-06-15 16:31:59.885841 solutions_template-1.10.0/solutions_template/modules/restful_service/.st/module_answers/{{component_name}}.yaml
--rw-r--r--   0        0        0     1363 2023-06-27 16:32:20.334262 solutions_template-1.10.0/solutions_template/modules/restful_service/README.md
--rw-r--r--   0        0        0      545 2023-06-15 16:31:59.886671 solutions_template-1.10.0/solutions_template/modules/restful_service/components/{{component_name}}/Dockerfile
--rw-r--r--   0        0        0     1258 2023-06-15 16:31:59.886951 solutions_template-1.10.0/solutions_template/modules/restful_service/components/{{component_name}}/README.md
--rw-r--r--   0        0        0      215 2023-06-15 16:31:59.887289 solutions_template-1.10.0/solutions_template/modules/restful_service/components/{{component_name}}/manifests/cloudrun-service.yaml
--rw-r--r--   0        0        0       77 2023-06-15 16:31:59.887400 solutions_template-1.10.0/solutions_template/modules/restful_service/components/{{component_name}}/requirements-test.txt
--rw-r--r--   0        0        0      109 2023-06-15 16:31:59.887740 solutions_template-1.10.0/solutions_template/modules/restful_service/components/{{component_name}}/requirements.txt
--rw-r--r--   0        0        0     3182 2023-06-21 14:30:18.511072 solutions_template-1.10.0/solutions_template/modules/restful_service/components/{{component_name}}/skaffold.yaml
--rw-r--r--   0        0        0      863 2023-06-15 16:31:59.888227 solutions_template-1.10.0/solutions_template/modules/restful_service/components/{{component_name}}/src/config.py
--rw-r--r--   0        0        0     1871 2023-06-18 03:24:24.483534 solutions_template-1.10.0/solutions_template/modules/restful_service/components/{{component_name}}/src/main.py
--rw-r--r--   0        0        0     1664 2023-06-21 14:30:18.511495 solutions_template-1.10.0/solutions_template/modules/restful_service/components/{{component_name}}/src/models/{{data_model}}.py
--rw-r--r--   0        0        0        0 2023-06-15 16:31:59.889165 solutions_template-1.10.0/solutions_template/modules/restful_service/components/{{component_name}}/src/routes/__init__.py
--rw-r--r--   0        0        0     3876 2023-06-21 14:30:18.511914 solutions_template-1.10.0/solutions_template/modules/restful_service/components/{{component_name}}/src/routes/{{data_model_plural}}.py
--rw-r--r--   0        0        0     1222 2023-06-21 14:30:18.512138 solutions_template-1.10.0/solutions_template/modules/restful_service/components/{{component_name}}/src/schemas/{{data_model}}.py
--rw-r--r--   0        0        0        0 2023-06-15 16:31:59.890086 solutions_template-1.10.0/solutions_template/modules/restful_service/components/{{component_name}}/src/utils/__init__.py
--rw-r--r--   0        0        0       81 2023-06-15 16:31:59.890476 solutions_template-1.10.0/solutions_template/modules/restful_service/components/{{component_name}}/st_module.yaml
--rw-r--r--   0        0        0     1191 2023-06-15 16:31:59.890863 solutions_template-1.10.0/solutions_template/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/deployment.yaml
--rw-r--r--   0        0        0      197 2023-06-15 16:31:59.891124 solutions_template-1.10.0/solutions_template/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/kustomization.yaml
--rw-r--r--   0        0        0       60 2023-06-15 16:31:59.891325 solutions_template-1.10.0/solutions_template/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/properties.env
--rw-r--r--   0        0        0      229 2023-06-15 16:31:59.891641 solutions_template-1.10.0/solutions_template/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/service.yaml
--rw-r--r--   0        0        0      421 2023-06-15 16:31:59.891935 solutions_template-1.10.0/solutions_template/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/hpa/hpa.yaml
--rw-r--r--   0        0        0      103 2023-06-15 16:31:59.892130 solutions_template-1.10.0/solutions_template/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/hpa/kustomization.yaml
--rw-r--r--   0        0        0     2305 2023-06-27 16:32:20.334559 solutions_template-1.10.0/solutions_template/modules/restful_service/copier.yaml
--rw-r--r--   0        0        0      120 2023-06-27 16:32:20.334922 solutions_template-1.10.0/solutions_template/modules/restful_service/docs/components/{{component_name}}.md
--rw-r--r--   0        0        0       92 2023-06-15 16:31:59.892900 solutions_template-1.10.0/solutions_template/modules/restful_service/skaffold.yaml.patch
--rw-r--r--   0        0        0      263 2023-06-15 16:31:59.893286 solutions_template-1.10.0/solutions_template/modules/restful_service/terraform/stages/{{'3-httplb-cloudrun' if cloudrun_neg}}/{{component_name}}_neg.tf
--rw-r--r--   0        0        0     3223 2023-06-22 05:56:48.856502 solutions_template-1.10.0/solutions_template/modules/restful_service/tests/e2e/{{component_name}}_e2e_test.py
--rw-r--r--   0        0        0     3269 2023-06-27 16:32:20.335275 solutions_template-1.10.0/solutions_template/modules/restful_service/{{'.github' if use_github_action}}/workflows/unit_test_linter_{{component_name}}.yaml
--rw-r--r--   0        0        0       80 2023-06-27 18:53:22.996020 solutions_template-1.10.0/solutions_template/modules/task_dispatch_service/.st/module_answers/{{component_name}}.yaml
--rw-r--r--   0        0        0      545 2023-06-27 18:53:22.983961 solutions_template-1.10.0/solutions_template/modules/task_dispatch_service/components/{{component_name}}/Dockerfile
--rw-r--r--   0        0        0       77 2023-06-27 18:56:43.842430 solutions_template-1.10.0/solutions_template/modules/task_dispatch_service/components/{{component_name}}/requirements-test.txt
--rw-r--r--   0        0        0      109 2023-06-27 18:53:22.982374 solutions_template-1.10.0/solutions_template/modules/task_dispatch_service/components/{{component_name}}/requirements.txt
--rw-r--r--   0        0        0     3183 2023-06-27 18:53:22.986184 solutions_template-1.10.0/solutions_template/modules/task_dispatch_service/components/{{component_name}}/skaffold.yaml
--rw-r--r--   0        0        0      863 2023-06-27 18:56:43.783992 solutions_template-1.10.0/solutions_template/modules/task_dispatch_service/components/{{component_name}}/src/config.py
--rw-r--r--   0        0        0     1871 2023-06-27 18:56:43.784569 solutions_template-1.10.0/solutions_template/modules/task_dispatch_service/components/{{component_name}}/src/main.py
--rw-r--r--   0        0        0     1661 2023-06-29 06:23:37.552308 solutions_template-1.10.0/solutions_template/modules/task_dispatch_service/components/{{component_name}}/src/models/task.py
--rw-r--r--   0        0        0        0 2023-06-27 18:56:43.787357 solutions_template-1.10.0/solutions_template/modules/task_dispatch_service/components/{{component_name}}/src/routes/__init__.py
--rw-r--r--   0        0        0     3854 2023-06-29 06:32:32.707285 solutions_template-1.10.0/solutions_template/modules/task_dispatch_service/components/{{component_name}}/src/routes/tasks.py
--rw-r--r--   0        0        0     1177 2023-06-29 06:21:35.454197 solutions_template-1.10.0/solutions_template/modules/task_dispatch_service/components/{{component_name}}/src/schemas/task.py
--rw-r--r--   0        0        0        0 2023-06-27 18:56:43.792295 solutions_template-1.10.0/solutions_template/modules/task_dispatch_service/components/{{component_name}}/src/utils/__init__.py
--rw-r--r--   0        0        0      132 2023-06-29 06:27:57.280902 solutions_template-1.10.0/solutions_template/modules/task_dispatch_service/components/{{component_name}}/src/utils/workflow_helper.py
--rw-r--r--   0        0        0     1099 2023-06-29 17:30:59.312607 solutions_template-1.10.0/solutions_template/modules/task_dispatch_service/components/{{component_name}}/src/workflows/example.yaml
--rw-r--r--   0        0        0      265 2023-06-27 18:53:22.980757 solutions_template-1.10.0/solutions_template/modules/task_dispatch_service/components/{{component_name}}/st_module.yaml
--rw-r--r--   0        0        0     2164 2023-06-29 19:00:22.674787 solutions_template-1.10.0/solutions_template/modules/task_dispatch_service/copier.yaml
--rw-r--r--   0        0        0       71 2023-06-27 18:53:22.956323 solutions_template-1.10.0/solutions_template/modules/task_dispatch_service/docs/components/{{component_name}}.md
--rw-r--r--   0        0        0       92 2023-06-29 17:32:25.048001 solutions_template-1.10.0/solutions_template/modules/task_dispatch_service/skaffold.yaml.patch
--rw-r--r--   0        0        0      719 2023-06-27 18:53:22.974873 solutions_template-1.10.0/solutions_template/modules/task_dispatch_service/terraform/stages/3-task-dispatch-service/backend.tf
--rw-r--r--   0        0        0     1718 2023-06-29 18:51:26.974646 solutions_template-1.10.0/solutions_template/modules/task_dispatch_service/terraform/stages/3-task-dispatch-service/main.tf
--rw-r--r--   0        0        0      930 2023-06-29 18:50:02.588881 solutions_template-1.10.0/solutions_template/modules/task_dispatch_service/terraform/stages/3-task-dispatch-service/providers.tf
--rw-r--r--   0        0        0     1266 2023-06-29 18:52:16.709474 solutions_template-1.10.0/solutions_template/modules/task_dispatch_service/terraform/stages/3-task-dispatch-service/terraform.tfvars
--rw-r--r--   0        0        0     1928 2023-06-29 18:51:22.487897 solutions_template-1.10.0/solutions_template/modules/task_dispatch_service/terraform/stages/3-task-dispatch-service/variables.tf
--rw-r--r--   0        0        0     3851 2023-06-27 18:53:22.992863 solutions_template-1.10.0/solutions_template/modules/task_dispatch_service/{{'.github' if use_github_action}}/workflows/unit_test_linter_{{component_name}}.yaml
--rw-r--r--   0        0        0       80 2023-06-21 14:30:18.513363 solutions_template-1.10.0/solutions_template/modules/terraform_gke/.st/module_answers/{{component_name}}.yaml
--rw-r--r--   0        0        0     1271 2023-06-21 14:30:18.513680 solutions_template-1.10.0/solutions_template/modules/terraform_gke/copier.yaml
--rw-r--r--   0        0        0      794 2023-06-27 16:32:20.335672 solutions_template-1.10.0/solutions_template/modules/terraform_gke/docs/components/{{component_name}}.md
--rw-r--r--   0        0        0       63 2023-06-21 14:30:18.514649 solutions_template-1.10.0/solutions_template/modules/terraform_gke/skaffold.yaml.patch
--rw-r--r--   0        0        0      701 2023-06-15 16:31:59.895524 solutions_template-1.10.0/solutions_template/modules/terraform_gke/terraform/stages/2-gke/backend.tf
--rw-r--r--   0        0        0     1568 2023-06-15 16:31:59.895667 solutions_template-1.10.0/solutions_template/modules/terraform_gke/terraform/stages/2-gke/iam.tf
--rw-r--r--   0        0        0     2486 2023-06-21 14:30:18.514915 solutions_template-1.10.0/solutions_template/modules/terraform_gke/terraform/stages/2-gke/main.tf
--rw-r--r--   0        0        0     1783 2023-06-15 16:31:59.895957 solutions_template-1.10.0/solutions_template/modules/terraform_gke/terraform/stages/2-gke/providers.tf
--rw-r--r--   0        0        0      268 2023-06-21 14:30:18.515245 solutions_template-1.10.0/solutions_template/modules/terraform_gke/terraform/stages/2-gke/terraform.tfvars
--rw-r--r--   0        0        0     1553 2023-06-21 14:30:18.515555 solutions_template-1.10.0/solutions_template/modules/terraform_gke/terraform/stages/2-gke/variables.tf
--rw-r--r--   0        0        0       80 2023-06-21 14:30:18.515897 solutions_template-1.10.0/solutions_template/modules/terraform_gke_ingress/.st/module_answers/{{component_name}}.yaml
--rw-r--r--   0        0        0     2170 2023-06-21 14:30:18.516134 solutions_template-1.10.0/solutions_template/modules/terraform_gke_ingress/copier.yaml
--rw-r--r--   0        0        0      180 2023-06-21 14:30:18.516469 solutions_template-1.10.0/solutions_template/modules/terraform_gke_ingress/ingress/kustomize/gke/frontend_config.yaml
--rw-r--r--   0        0        0      658 2023-06-21 14:30:18.516847 solutions_template-1.10.0/solutions_template/modules/terraform_gke_ingress/ingress/kustomize/gke/ingress.yaml
--rw-r--r--   0        0        0      145 2023-06-21 14:30:18.517055 solutions_template-1.10.0/solutions_template/modules/terraform_gke_ingress/ingress/kustomize/gke/kustomization.yaml
--rw-r--r--   0        0        0      185 2023-06-21 14:30:18.517271 solutions_template-1.10.0/solutions_template/modules/terraform_gke_ingress/ingress/kustomize/gke/managed_cert.yaml
--rw-r--r--   0        0        0      378 2023-06-21 14:30:18.517461 solutions_template-1.10.0/solutions_template/modules/terraform_gke_ingress/ingress/skaffold.yaml
--rw-r--r--   0        0        0       59 2023-06-21 14:30:18.517746 solutions_template-1.10.0/solutions_template/modules/terraform_gke_ingress/skaffold.yaml.patch
--rw-r--r--   0        0        0     2420 2023-06-21 14:30:18.518147 solutions_template-1.10.0/solutions_template/modules/terraform_gke_ingress/terraform/modules/ingress_gce/main.tf
--rw-r--r--   0        0        0      670 2023-06-21 14:30:18.518796 solutions_template-1.10.0/solutions_template/modules/terraform_gke_ingress/terraform/modules/ingress_gce/outputs.tf
--rw-r--r--   0        0        0     1264 2023-06-21 14:30:18.519004 solutions_template-1.10.0/solutions_template/modules/terraform_gke_ingress/terraform/modules/ingress_gce/variables.tf
--rw-r--r--   0        0        0      709 2023-06-21 14:30:18.519311 solutions_template-1.10.0/solutions_template/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/backend.tf
--rw-r--r--   0        0        0     1568 2023-06-21 14:30:18.519782 solutions_template-1.10.0/solutions_template/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/iam.tf
--rw-r--r--   0        0        0     1695 2023-06-21 14:30:18.520002 solutions_template-1.10.0/solutions_template/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/main.tf
--rw-r--r--   0        0        0     1877 2023-06-21 14:30:18.520187 solutions_template-1.10.0/solutions_template/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/providers.tf
--rw-r--r--   0        0        0      480 2023-06-21 14:30:18.520341 solutions_template-1.10.0/solutions_template/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/terraform.tfvars
--rw-r--r--   0        0        0     1802 2023-06-21 14:30:18.520745 solutions_template-1.10.0/solutions_template/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/variables.tf
--rw-r--r--   0        0        0       80 2023-06-21 14:30:18.521191 solutions_template-1.10.0/solutions_template/modules/terraform_httplb_cloudrun/.st/module_answers/{{component_name}}.yaml
--rw-r--r--   0        0        0     1032 2023-06-21 14:30:18.521673 solutions_template-1.10.0/solutions_template/modules/terraform_httplb_cloudrun/copier.yaml
--rw-r--r--   0        0        0      834 2023-06-15 16:31:59.898543 solutions_template-1.10.0/solutions_template/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/backend.tf
--rw-r--r--   0        0        0     2760 2023-06-15 16:31:59.898838 solutions_template-1.10.0/solutions_template/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/main.tf
--rw-r--r--   0        0        0      671 2023-06-15 16:31:59.899283 solutions_template-1.10.0/solutions_template/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/outputs.tf
--rw-r--r--   0        0        0     1298 2023-06-15 16:31:59.899651 solutions_template-1.10.0/solutions_template/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/providers.tf
--rw-r--r--   0        0        0       81 2023-06-15 16:31:59.899785 solutions_template-1.10.0/solutions_template/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/st_module.yaml
--rw-r--r--   0        0        0      196 2023-06-15 16:31:59.899968 solutions_template-1.10.0/solutions_template/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/terraform.tfvars
--rw-r--r--   0        0        0     1967 2023-06-15 16:31:59.900160 solutions_template-1.10.0/solutions_template/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/variables.tf
--rw-r--r--   0        0        0       90 2023-06-27 16:32:20.335915 solutions_template-1.10.0/solutions_template/requirements.txt
--rw-r--r--   0        0        0    68957 2023-06-15 16:31:59.901015 solutions_template-1.10.0/solutions_template/template_root/.github/assets/setup_local.png
--rw-r--r--   0        0        0   239307 2023-06-15 16:31:59.902244 solutions_template-1.10.0/solutions_template/template_root/.github/assets/skaffold_dev_terminal.png
--rw-r--r--   0        0        0     2639 2023-06-15 16:31:59.902916 solutions_template-1.10.0/solutions_template/template_root/.github/workflows/deployment_cloudrun_dev.yaml
--rw-r--r--   0        0        0     2690 2023-06-15 16:31:59.903239 solutions_template-1.10.0/solutions_template/template_root/.github/workflows/deployment_gke_dev.yaml
--rw-r--r--   0        0        0     5786 2023-06-15 16:31:59.905439 solutions_template-1.10.0/solutions_template/template_root/.github/workflows/e2e_cloudrun_api_test.yaml
--rw-r--r--   0        0        0     8049 2023-06-15 16:31:59.912323 solutions_template-1.10.0/solutions_template/template_root/.github/workflows/e2e_gke_api_test.yaml
--rw-r--r--   0        0        0     3131 2023-06-15 16:31:59.916647 solutions_template-1.10.0/solutions_template/template_root/.github/workflows/unit_test_linter_common.yaml
--rw-r--r--   0        0        0      471 2023-06-15 16:31:59.917181 solutions_template-1.10.0/solutions_template/template_root/.gitignore
--rw-r--r--   0        0        0    14552 2023-06-15 16:31:59.919314 solutions_template-1.10.0/solutions_template/template_root/.pylintrc
--rw-r--r--   0        0        0      712 2023-06-15 16:31:59.919730 solutions_template-1.10.0/solutions_template/template_root/README.md
--rw-r--r--   0        0        0      398 2023-06-27 16:32:20.336295 solutions_template-1.10.0/solutions_template/template_root/components/README.md
--rw-r--r--   0        0        0      211 2023-06-15 16:31:59.920301 solutions_template-1.10.0/solutions_template/template_root/components/common/Dockerfile
--rw-r--r--   0        0        0      395 2023-06-15 16:31:59.920640 solutions_template-1.10.0/solutions_template/template_root/components/common/Dockerfile.unittest
--rw-r--r--   0        0        0       77 2023-06-15 16:31:59.920716 solutions_template-1.10.0/solutions_template/template_root/components/common/requirements-test.txt
--rw-r--r--   0        0        0      131 2023-06-15 16:31:59.920842 solutions_template-1.10.0/solutions_template/template_root/components/common/requirements.txt
--rw-r--r--   0        0        0      571 2023-06-15 16:31:59.921142 solutions_template-1.10.0/solutions_template/template_root/components/common/skaffold.yaml
--rw-r--r--   0        0        0        0 2023-06-15 16:31:59.921222 solutions_template-1.10.0/solutions_template/template_root/components/common/src/common/__init__.py
--rw-r--r--   0        0        0      832 2023-06-15 16:31:59.921500 solutions_template-1.10.0/solutions_template/template_root/components/common/src/common/config.py
--rw-r--r--   0        0        0      696 2023-06-15 16:31:59.921923 solutions_template-1.10.0/solutions_template/template_root/components/common/src/common/db_client.py
--rw-r--r--   0        0        0       35 2023-06-15 16:31:59.922651 solutions_template-1.10.0/solutions_template/template_root/components/common/src/common/models/README.md
--rw-r--r--   0        0        0       91 2023-06-15 16:31:59.922920 solutions_template-1.10.0/solutions_template/template_root/components/common/src/common/models/__init__.py
--rw-r--r--   0        0        0     1377 2023-06-15 16:31:59.923190 solutions_template-1.10.0/solutions_template/template_root/components/common/src/common/models/example.py
--rw-r--r--   0        0        0        0 2023-06-15 16:31:59.923251 solutions_template-1.10.0/solutions_template/template_root/components/common/src/common/testing/__init__.py
--rw-r--r--   0        0        0      755 2023-06-15 16:31:59.923525 solutions_template-1.10.0/solutions_template/template_root/components/common/src/common/testing/bq_client_fixture.py
--rw-r--r--   0        0        0     1007 2023-06-15 16:31:59.923771 solutions_template-1.10.0/solutions_template/template_root/components/common/src/common/testing/client_with_emulator.py
--rw-r--r--   0        0        0     2244 2023-06-15 16:31:59.924001 solutions_template-1.10.0/solutions_template/template_root/components/common/src/common/testing/firestore_emulator.py
--rw-r--r--   0        0        0        0 2023-06-15 16:31:59.924090 solutions_template-1.10.0/solutions_template/template_root/components/common/src/common/utils/__init__.py
--rw-r--r--   0        0        0     1003 2023-06-15 16:31:59.924293 solutions_template-1.10.0/solutions_template/template_root/components/common/src/common/utils/logging_handler.py
--rw-r--r--   0        0        0     2015 2023-06-20 15:16:57.863068 solutions_template-1.10.0/solutions_template/template_root/copier.yaml
--rw-r--r--   0        0        0       97 2023-06-15 16:31:59.924976 solutions_template-1.10.0/solutions_template/template_root/firebase.json
--rw-r--r--   0        0        0       98 2023-06-15 16:31:59.925120 solutions_template-1.10.0/solutions_template/template_root/setup.cfg
--rw-r--r--   0        0        0      159 2023-06-15 16:31:59.925502 solutions_template-1.10.0/solutions_template/template_root/skaffold.yaml
--rw-r--r--   0        0        0      360 2023-06-15 16:31:59.925681 solutions_template-1.10.0/solutions_template/template_root/st.yaml
--rw-r--r--   0        0        0      921 2023-06-15 16:31:59.925959 solutions_template-1.10.0/solutions_template/template_root/terraform/modules/cloudbuild/main.tf
--rw-r--r--   0        0        0      730 2023-06-15 16:31:59.926143 solutions_template-1.10.0/solutions_template/template_root/terraform/modules/cloudbuild/variables.tf
--rw-r--r--   0        0        0     3585 2023-06-15 16:31:59.926376 solutions_template-1.10.0/solutions_template/template_root/terraform/modules/cloudrun/main.tf
--rw-r--r--   0        0        0     1178 2023-06-15 16:31:59.926551 solutions_template-1.10.0/solutions_template/template_root/terraform/modules/cloudrun/variables.tf
--rw-r--r--   0        0        0     5024 2023-06-15 16:31:59.927017 solutions_template-1.10.0/solutions_template/template_root/terraform/modules/compute_backend/main.tf
--rw-r--r--   0        0        0      190 2023-06-15 16:31:59.927289 solutions_template-1.10.0/solutions_template/template_root/terraform/modules/compute_backend/outputs.tf
--rw-r--r--   0        0        0     1185 2023-06-15 16:31:59.927608 solutions_template-1.10.0/solutions_template/template_root/terraform/modules/compute_backend/providers.tf
--rw-r--r--   0        0        0     1601 2023-06-15 16:31:59.927810 solutions_template-1.10.0/solutions_template/template_root/terraform/modules/compute_backend/variables.tf
--rw-r--r--   0        0        0     2364 2023-06-15 16:31:59.927994 solutions_template-1.10.0/solutions_template/template_root/terraform/modules/firebase/main.tf
--rw-r--r--   0        0        0     1194 2023-06-15 16:31:59.928358 solutions_template-1.10.0/solutions_template/template_root/terraform/modules/firebase/variables.tf
--rw-r--r--   0        0        0     4239 2023-06-21 14:30:18.522355 solutions_template-1.10.0/solutions_template/template_root/terraform/modules/gke/main.tf
--rw-r--r--   0        0        0      832 2023-06-15 16:31:59.928824 solutions_template-1.10.0/solutions_template/template_root/terraform/modules/gke/outputs.tf
--rw-r--r--   0        0        0     2813 2023-06-21 14:30:18.522769 solutions_template-1.10.0/solutions_template/template_root/terraform/modules/gke/variables.tf
--rw-r--r--   0        0        0     2926 2023-06-15 16:31:59.930393 solutions_template-1.10.0/solutions_template/template_root/terraform/modules/ingress_nginx/main.tf
--rw-r--r--   0        0        0      692 2023-06-15 16:31:59.930656 solutions_template-1.10.0/solutions_template/template_root/terraform/modules/ingress_nginx/outputs.tf
--rw-r--r--   0        0        0     1087 2023-06-15 16:31:59.931016 solutions_template-1.10.0/solutions_template/template_root/terraform/modules/ingress_nginx/variables.tf
--rw-r--r--   0        0        0      827 2023-06-15 16:31:59.931291 solutions_template-1.10.0/solutions_template/template_root/terraform/modules/project_services/main.tf
--rw-r--r--   0        0        0      773 2023-06-15 16:31:59.931538 solutions_template-1.10.0/solutions_template/template_root/terraform/modules/project_services/variables.tf
--rw-r--r--   0        0        0      953 2023-06-15 16:31:59.931934 solutions_template-1.10.0/solutions_template/template_root/terraform/modules/service_account/main.tf
--rw-r--r--   0        0        0     1037 2023-06-15 16:31:59.932426 solutions_template-1.10.0/solutions_template/template_root/terraform/modules/service_account/variables.tf
--rw-r--r--   0        0        0     1529 2023-06-15 16:31:59.932733 solutions_template-1.10.0/solutions_template/template_root/terraform/modules/terraform_cicd/main.tf
--rw-r--r--   0        0        0      677 2023-06-15 16:31:59.933018 solutions_template-1.10.0/solutions_template/template_root/terraform/modules/terraform_cicd/variables.tf
--rw-r--r--   0        0        0     1333 2023-06-15 16:31:59.933248 solutions_template-1.10.0/solutions_template/template_root/terraform/modules/vpc_network/main.tf
--rw-r--r--   0        0        0     1269 2023-06-15 16:31:59.933426 solutions_template-1.10.0/solutions_template/template_root/terraform/modules/vpc_network/variables.tf
--rw-r--r--   0        0        0     2193 2023-06-15 16:31:59.933834 solutions_template-1.10.0/solutions_template/template_root/terraform/stages/1-bootstrap/main.tf
--rw-r--r--   0        0        0      730 2023-06-15 16:31:59.934084 solutions_template-1.10.0/solutions_template/template_root/terraform/stages/1-bootstrap/output.tf
--rw-r--r--   0        0        0       66 2023-06-15 16:31:59.934377 solutions_template-1.10.0/solutions_template/template_root/terraform/stages/1-bootstrap/terraform.tfvars
--rw-r--r--   0        0        0     1071 2023-06-15 16:31:59.934790 solutions_template-1.10.0/solutions_template/template_root/terraform/stages/1-bootstrap/variables.tf
--rw-r--r--   0        0        0      826 2023-06-15 16:31:59.935095 solutions_template-1.10.0/solutions_template/template_root/terraform/stages/2-foundation/backend.tf
--rw-r--r--   0        0        0      517 2023-06-15 16:31:59.935395 solutions_template-1.10.0/solutions_template/template_root/terraform/stages/2-foundation/firestore_setup.tf
--rw-r--r--   0        0        0     1568 2023-06-15 16:31:59.935538 solutions_template-1.10.0/solutions_template/template_root/terraform/stages/2-foundation/iam.tf
--rw-r--r--   0        0        0     4307 2023-06-29 18:47:51.748494 solutions_template-1.10.0/solutions_template/template_root/terraform/stages/2-foundation/main.tf
--rw-r--r--   0        0        0      997 2023-06-15 16:31:59.935925 solutions_template-1.10.0/solutions_template/template_root/terraform/stages/2-foundation/outputs.tf
--rw-r--r--   0        0        0      835 2023-06-15 16:31:59.936181 solutions_template-1.10.0/solutions_template/template_root/terraform/stages/2-foundation/providers.tf
--rw-r--r--   0        0        0      606 2023-06-15 16:31:59.936549 solutions_template-1.10.0/solutions_template/template_root/terraform/stages/2-foundation/terraform.tfvars
--rw-r--r--   0        0        0     2546 2023-06-15 16:31:59.936876 solutions_template-1.10.0/solutions_template/template_root/terraform/stages/2-foundation/variables.tf
--rw-r--r--   0        0        0        0 2023-06-15 16:31:59.937992 solutions_template-1.10.0/solutions_template/template_root/tests/__init__.py
--rw-r--r--   0        0        0      825 2023-06-15 16:31:59.938319 solutions_template-1.10.0/solutions_template/template_root/tests/e2e/e2e_utils.py
--rwxr-xr-x   0        0        0      364 2023-06-15 16:31:59.938529 solutions_template-1.10.0/solutions_template/template_root/utils/disable_org_policies.sh
--rwxr-xr-x   0        0        0     1095 2023-06-15 16:31:59.938794 solutions_template-1.10.0/solutions_template/template_root/utils/init_env_vars.sh
--rwxr-xr-x   0        0        0    13137 2023-06-15 16:31:59.939050 solutions_template-1.10.0/solutions_template/template_root/utils/setup_all.sh
--rwxr-xr-x   0        0        0     2835 2023-06-15 16:31:59.939218 solutions_template-1.10.0/solutions_template/template_root/utils/setup_local.sh
--rw-r--r--   0        0        0       81 2023-06-15 16:31:59.939607 solutions_template-1.10.0/solutions_template/template_root/{{_copier_conf.answers_file}}
--rw-r--r--   0        0        0        0 2023-06-15 16:31:59.939700 solutions_template-1.10.0/solutions_template/tests/__init__.py
--rw-r--r--   0        0        0     5869 1970-01-01 00:00:00.000000 solutions_template-1.10.0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2022-06-28 21:05:37.723277 solutions_template-1.9.0/LICENSE
+-rw-r--r--   0        0        0     4839 2023-06-15 18:40:51.230107 solutions_template-1.9.0/README.md
+-rw-r--r--   0        0        0     1105 2023-06-15 18:42:19.667601 solutions_template-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-15 16:31:59.883150 solutions_template-1.9.0/solutions_template/__init__.py
+-rw-r--r--   0        0        0     5659 2023-06-16 02:54:27.663884 solutions_template-1.9.0/solutions_template/cli/cli.py
+-rw-r--r--   0        0        0     4199 2023-06-15 16:31:59.883928 solutions_template-1.9.0/solutions_template/cli/cli_utils.py
+-rw-r--r--   0        0        0     6184 2023-06-16 03:59:18.084087 solutions_template-1.9.0/solutions_template/cli/component.py
+-rw-r--r--   0        0        0     5883 2023-06-15 16:31:59.884617 solutions_template-1.9.0/solutions_template/cli/infra.py
+-rw-r--r--   0        0        0     1072 2023-06-15 16:31:59.884862 solutions_template-1.9.0/solutions_template/cli/tool.py
+-rw-r--r--   0        0        0        0 2023-06-15 16:31:59.884916 solutions_template-1.9.0/solutions_template/copier_extensions/__init__.py
+-rw-r--r--   0        0        0     3561 2023-06-15 16:31:59.885392 solutions_template-1.9.0/solutions_template/copier_extensions/st_helpers.py
+-rw-r--r--   0        0        0       80 2023-06-15 16:31:59.885841 solutions_template-1.9.0/solutions_template/modules/restful_service/.st/module_answers/{{component_name}}.yaml
+-rw-r--r--   0        0        0      545 2023-06-15 16:31:59.886671 solutions_template-1.9.0/solutions_template/modules/restful_service/components/{{component_name}}/Dockerfile
+-rw-r--r--   0        0        0     1258 2023-06-15 16:31:59.886951 solutions_template-1.9.0/solutions_template/modules/restful_service/components/{{component_name}}/README.md
+-rw-r--r--   0        0        0      215 2023-06-15 16:31:59.887289 solutions_template-1.9.0/solutions_template/modules/restful_service/components/{{component_name}}/manifests/cloudrun-service.yaml
+-rw-r--r--   0        0        0       77 2023-06-15 16:31:59.887400 solutions_template-1.9.0/solutions_template/modules/restful_service/components/{{component_name}}/requirements-test.txt
+-rw-r--r--   0        0        0      109 2023-06-15 16:31:59.887740 solutions_template-1.9.0/solutions_template/modules/restful_service/components/{{component_name}}/requirements.txt
+-rw-r--r--   0        0        0     3182 2023-06-16 02:53:26.841584 solutions_template-1.9.0/solutions_template/modules/restful_service/components/{{component_name}}/skaffold.yaml
+-rw-r--r--   0        0        0      863 2023-06-15 16:31:59.888227 solutions_template-1.9.0/solutions_template/modules/restful_service/components/{{component_name}}/src/config.py
+-rw-r--r--   0        0        0     1871 2023-06-15 16:31:59.888781 solutions_template-1.9.0/solutions_template/modules/restful_service/components/{{component_name}}/src/main.py
+-rw-r--r--   0        0        0     1664 2023-06-16 05:03:43.370908 solutions_template-1.9.0/solutions_template/modules/restful_service/components/{{component_name}}/src/models/{{data_model}}.py
+-rw-r--r--   0        0        0        0 2023-06-15 16:31:59.889165 solutions_template-1.9.0/solutions_template/modules/restful_service/components/{{component_name}}/src/routes/__init__.py
+-rw-r--r--   0        0        0     3876 2023-06-16 05:04:41.195170 solutions_template-1.9.0/solutions_template/modules/restful_service/components/{{component_name}}/src/routes/{{data_model_plural}}.py
+-rw-r--r--   0        0        0     1222 2023-06-16 05:08:22.051091 solutions_template-1.9.0/solutions_template/modules/restful_service/components/{{component_name}}/src/schemas/{{data_model}}.py
+-rw-r--r--   0        0        0        0 2023-06-15 16:31:59.890086 solutions_template-1.9.0/solutions_template/modules/restful_service/components/{{component_name}}/src/utils/__init__.py
+-rw-r--r--   0        0        0       81 2023-06-15 16:31:59.890476 solutions_template-1.9.0/solutions_template/modules/restful_service/components/{{component_name}}/st_module.yaml
+-rw-r--r--   0        0        0     1191 2023-06-15 16:31:59.890863 solutions_template-1.9.0/solutions_template/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/deployment.yaml
+-rw-r--r--   0        0        0      197 2023-06-15 16:31:59.891124 solutions_template-1.9.0/solutions_template/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/kustomization.yaml
+-rw-r--r--   0        0        0       60 2023-06-15 16:31:59.891325 solutions_template-1.9.0/solutions_template/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/properties.env
+-rw-r--r--   0        0        0      229 2023-06-15 16:31:59.891641 solutions_template-1.9.0/solutions_template/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/service.yaml
+-rw-r--r--   0        0        0      421 2023-06-15 16:31:59.891935 solutions_template-1.9.0/solutions_template/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/hpa/hpa.yaml
+-rw-r--r--   0        0        0      103 2023-06-15 16:31:59.892130 solutions_template-1.9.0/solutions_template/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/hpa/kustomization.yaml
+-rw-r--r--   0        0        0     2255 2023-06-16 01:17:41.774796 solutions_template-1.9.0/solutions_template/modules/restful_service/copier.yaml
+-rw-r--r--   0        0        0       92 2023-06-15 16:31:59.892900 solutions_template-1.9.0/solutions_template/modules/restful_service/skaffold.yaml.patch
+-rw-r--r--   0        0        0      263 2023-06-15 16:31:59.893286 solutions_template-1.9.0/solutions_template/modules/restful_service/terraform/stages/{{'3-httplb-cloudrun' if cloudrun_neg}}/{{component_name}}_neg.tf
+-rw-r--r--   0        0        0     3461 2023-06-15 16:31:59.893746 solutions_template-1.9.0/solutions_template/modules/restful_service/tests/e2e/{{component_name}}_e2e_test.py
+-rw-r--r--   0        0        0     3269 2023-06-15 16:31:59.894288 solutions_template-1.9.0/solutions_template/modules/restful_service/{{'.github' if use_github_action}}/workflows/unit_test_linter_{{component_name}}.yaml
+-rw-r--r--   0        0        0     1165 2023-06-16 04:09:29.339712 solutions_template-1.9.0/solutions_template/modules/terraform_gke/copier.yaml
+-rw-r--r--   0        0        0      792 2023-06-15 16:31:59.894621 solutions_template-1.9.0/solutions_template/modules/terraform_gke/docs/modules/{{component_name}}.md
+-rw-r--r--   0        0        0      166 2023-06-15 16:31:59.895201 solutions_template-1.9.0/solutions_template/modules/terraform_gke/ingress/skaffold.yaml
+-rw-r--r--   0        0        0      701 2023-06-15 16:31:59.895524 solutions_template-1.9.0/solutions_template/modules/terraform_gke/terraform/stages/2-gke/backend.tf
+-rw-r--r--   0        0        0     1568 2023-06-15 16:31:59.895667 solutions_template-1.9.0/solutions_template/modules/terraform_gke/terraform/stages/2-gke/iam.tf
+-rw-r--r--   0        0        0     2466 2023-06-15 16:31:59.895836 solutions_template-1.9.0/solutions_template/modules/terraform_gke/terraform/stages/2-gke/main.tf
+-rw-r--r--   0        0        0     1783 2023-06-15 16:31:59.895957 solutions_template-1.9.0/solutions_template/modules/terraform_gke/terraform/stages/2-gke/providers.tf
+-rw-r--r--   0        0        0      167 2023-06-15 16:31:59.896270 solutions_template-1.9.0/solutions_template/modules/terraform_gke/terraform/stages/2-gke/terraform.tfvars
+-rw-r--r--   0        0        0     1656 2023-06-15 16:31:59.896449 solutions_template-1.9.0/solutions_template/modules/terraform_gke/terraform/stages/2-gke/variables.tf
+-rw-r--r--   0        0        0      709 2023-06-15 16:31:59.896669 solutions_template-1.9.0/solutions_template/modules/terraform_gke/terraform/stages/3-ingress-gke/backend.tf
+-rw-r--r--   0        0        0     1568 2023-06-15 16:31:59.896852 solutions_template-1.9.0/solutions_template/modules/terraform_gke/terraform/stages/3-ingress-gke/iam.tf
+-rw-r--r--   0        0        0     1765 2023-06-15 16:31:59.897192 solutions_template-1.9.0/solutions_template/modules/terraform_gke/terraform/stages/3-ingress-gke/main.tf
+-rw-r--r--   0        0        0     1838 2023-06-15 16:31:59.897489 solutions_template-1.9.0/solutions_template/modules/terraform_gke/terraform/stages/3-ingress-gke/providers.tf
+-rw-r--r--   0        0        0      327 2023-06-15 16:31:59.897664 solutions_template-1.9.0/solutions_template/modules/terraform_gke/terraform/stages/3-ingress-gke/terraform.tfvars
+-rw-r--r--   0        0        0     1538 2023-06-15 16:31:59.897824 solutions_template-1.9.0/solutions_template/modules/terraform_gke/terraform/stages/3-ingress-gke/variables.tf
+-rw-r--r--   0        0        0     1038 2023-06-15 16:31:59.898140 solutions_template-1.9.0/solutions_template/modules/terraform_httplb_cloudrun/copier.yaml
+-rw-r--r--   0        0        0      834 2023-06-15 16:31:59.898543 solutions_template-1.9.0/solutions_template/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/backend.tf
+-rw-r--r--   0        0        0     2760 2023-06-15 16:31:59.898838 solutions_template-1.9.0/solutions_template/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/main.tf
+-rw-r--r--   0        0        0      671 2023-06-15 16:31:59.899283 solutions_template-1.9.0/solutions_template/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/outputs.tf
+-rw-r--r--   0        0        0     1298 2023-06-15 16:31:59.899651 solutions_template-1.9.0/solutions_template/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/providers.tf
+-rw-r--r--   0        0        0       81 2023-06-15 16:31:59.899785 solutions_template-1.9.0/solutions_template/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/st_module.yaml
+-rw-r--r--   0        0        0      196 2023-06-15 16:31:59.899968 solutions_template-1.9.0/solutions_template/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/terraform.tfvars
+-rw-r--r--   0        0        0     1967 2023-06-15 16:31:59.900160 solutions_template-1.9.0/solutions_template/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/variables.tf
+-rw-r--r--   0        0        0       74 2023-06-15 16:31:59.900522 solutions_template-1.9.0/solutions_template/requirements.txt
+-rw-r--r--   0        0        0    68957 2023-06-15 16:31:59.901015 solutions_template-1.9.0/solutions_template/template_root/.github/assets/setup_local.png
+-rw-r--r--   0        0        0   239307 2023-06-15 16:31:59.902244 solutions_template-1.9.0/solutions_template/template_root/.github/assets/skaffold_dev_terminal.png
+-rw-r--r--   0        0        0     2639 2023-06-15 16:31:59.902916 solutions_template-1.9.0/solutions_template/template_root/.github/workflows/deployment_cloudrun_dev.yaml
+-rw-r--r--   0        0        0     2690 2023-06-15 16:31:59.903239 solutions_template-1.9.0/solutions_template/template_root/.github/workflows/deployment_gke_dev.yaml
+-rw-r--r--   0        0        0     5786 2023-06-15 16:31:59.905439 solutions_template-1.9.0/solutions_template/template_root/.github/workflows/e2e_cloudrun_api_test.yaml
+-rw-r--r--   0        0        0     8049 2023-06-15 16:31:59.912323 solutions_template-1.9.0/solutions_template/template_root/.github/workflows/e2e_gke_api_test.yaml
+-rw-r--r--   0        0        0     3131 2023-06-15 16:31:59.916647 solutions_template-1.9.0/solutions_template/template_root/.github/workflows/unit_test_linter_common.yaml
+-rw-r--r--   0        0        0      471 2023-06-15 16:31:59.917181 solutions_template-1.9.0/solutions_template/template_root/.gitignore
+-rw-r--r--   0        0        0    14552 2023-06-15 16:31:59.919314 solutions_template-1.9.0/solutions_template/template_root/.pylintrc
+-rw-r--r--   0        0        0      712 2023-06-15 16:31:59.919730 solutions_template-1.9.0/solutions_template/template_root/README.md
+-rw-r--r--   0        0        0      396 2023-06-15 16:31:59.920032 solutions_template-1.9.0/solutions_template/template_root/components/README.md
+-rw-r--r--   0        0        0      211 2023-06-15 16:31:59.920301 solutions_template-1.9.0/solutions_template/template_root/components/common/Dockerfile
+-rw-r--r--   0        0        0      395 2023-06-15 16:31:59.920640 solutions_template-1.9.0/solutions_template/template_root/components/common/Dockerfile.unittest
+-rw-r--r--   0        0        0       77 2023-06-15 16:31:59.920716 solutions_template-1.9.0/solutions_template/template_root/components/common/requirements-test.txt
+-rw-r--r--   0        0        0      131 2023-06-15 16:31:59.920842 solutions_template-1.9.0/solutions_template/template_root/components/common/requirements.txt
+-rw-r--r--   0        0        0      571 2023-06-15 16:31:59.921142 solutions_template-1.9.0/solutions_template/template_root/components/common/skaffold.yaml
+-rw-r--r--   0        0        0        0 2023-06-15 16:31:59.921222 solutions_template-1.9.0/solutions_template/template_root/components/common/src/common/__init__.py
+-rw-r--r--   0        0        0      832 2023-06-15 16:31:59.921500 solutions_template-1.9.0/solutions_template/template_root/components/common/src/common/config.py
+-rw-r--r--   0        0        0      696 2023-06-15 16:31:59.921923 solutions_template-1.9.0/solutions_template/template_root/components/common/src/common/db_client.py
+-rw-r--r--   0        0        0       35 2023-06-15 16:31:59.922651 solutions_template-1.9.0/solutions_template/template_root/components/common/src/common/models/README.md
+-rw-r--r--   0        0        0       91 2023-06-15 16:31:59.922920 solutions_template-1.9.0/solutions_template/template_root/components/common/src/common/models/__init__.py
+-rw-r--r--   0        0        0     1377 2023-06-15 16:31:59.923190 solutions_template-1.9.0/solutions_template/template_root/components/common/src/common/models/example.py
+-rw-r--r--   0        0        0        0 2023-06-15 16:31:59.923251 solutions_template-1.9.0/solutions_template/template_root/components/common/src/common/testing/__init__.py
+-rw-r--r--   0        0        0      755 2023-06-15 16:31:59.923525 solutions_template-1.9.0/solutions_template/template_root/components/common/src/common/testing/bq_client_fixture.py
+-rw-r--r--   0        0        0     1007 2023-06-15 16:31:59.923771 solutions_template-1.9.0/solutions_template/template_root/components/common/src/common/testing/client_with_emulator.py
+-rw-r--r--   0        0        0     2244 2023-06-15 16:31:59.924001 solutions_template-1.9.0/solutions_template/template_root/components/common/src/common/testing/firestore_emulator.py
+-rw-r--r--   0        0        0        0 2023-06-15 16:31:59.924090 solutions_template-1.9.0/solutions_template/template_root/components/common/src/common/utils/__init__.py
+-rw-r--r--   0        0        0     1003 2023-06-15 16:31:59.924293 solutions_template-1.9.0/solutions_template/template_root/components/common/src/common/utils/logging_handler.py
+-rw-r--r--   0        0        0     2015 2023-06-15 16:31:59.924591 solutions_template-1.9.0/solutions_template/template_root/copier.yaml
+-rw-r--r--   0        0        0       97 2023-06-15 16:31:59.924976 solutions_template-1.9.0/solutions_template/template_root/firebase.json
+-rw-r--r--   0        0        0       98 2023-06-15 16:31:59.925120 solutions_template-1.9.0/solutions_template/template_root/setup.cfg
+-rw-r--r--   0        0        0      159 2023-06-15 16:31:59.925502 solutions_template-1.9.0/solutions_template/template_root/skaffold.yaml
+-rw-r--r--   0        0        0      360 2023-06-15 16:31:59.925681 solutions_template-1.9.0/solutions_template/template_root/st.yaml
+-rw-r--r--   0        0        0      921 2023-06-15 16:31:59.925959 solutions_template-1.9.0/solutions_template/template_root/terraform/modules/cloudbuild/main.tf
+-rw-r--r--   0        0        0      730 2023-06-15 16:31:59.926143 solutions_template-1.9.0/solutions_template/template_root/terraform/modules/cloudbuild/variables.tf
+-rw-r--r--   0        0        0     3585 2023-06-15 16:31:59.926376 solutions_template-1.9.0/solutions_template/template_root/terraform/modules/cloudrun/main.tf
+-rw-r--r--   0        0        0     1178 2023-06-15 16:31:59.926551 solutions_template-1.9.0/solutions_template/template_root/terraform/modules/cloudrun/variables.tf
+-rw-r--r--   0        0        0     5024 2023-06-15 16:31:59.927017 solutions_template-1.9.0/solutions_template/template_root/terraform/modules/compute_backend/main.tf
+-rw-r--r--   0        0        0      190 2023-06-15 16:31:59.927289 solutions_template-1.9.0/solutions_template/template_root/terraform/modules/compute_backend/outputs.tf
+-rw-r--r--   0        0        0     1185 2023-06-15 16:31:59.927608 solutions_template-1.9.0/solutions_template/template_root/terraform/modules/compute_backend/providers.tf
+-rw-r--r--   0        0        0     1601 2023-06-15 16:31:59.927810 solutions_template-1.9.0/solutions_template/template_root/terraform/modules/compute_backend/variables.tf
+-rw-r--r--   0        0        0     2364 2023-06-15 16:31:59.927994 solutions_template-1.9.0/solutions_template/template_root/terraform/modules/firebase/main.tf
+-rw-r--r--   0        0        0     1194 2023-06-15 16:31:59.928358 solutions_template-1.9.0/solutions_template/template_root/terraform/modules/firebase/variables.tf
+-rw-r--r--   0        0        0     4235 2023-06-15 16:31:59.928596 solutions_template-1.9.0/solutions_template/template_root/terraform/modules/gke/main.tf
+-rw-r--r--   0        0        0      832 2023-06-15 16:31:59.928824 solutions_template-1.9.0/solutions_template/template_root/terraform/modules/gke/outputs.tf
+-rw-r--r--   0        0        0     2739 2023-06-15 16:31:59.929183 solutions_template-1.9.0/solutions_template/template_root/terraform/modules/gke/variables.tf
+-rw-r--r--   0        0        0     2766 2023-06-15 16:31:59.929718 solutions_template-1.9.0/solutions_template/template_root/terraform/modules/ingress_gce/main.tf
+-rw-r--r--   0        0        0      670 2023-06-15 16:31:59.929888 solutions_template-1.9.0/solutions_template/template_root/terraform/modules/ingress_gce/outputs.tf
+-rw-r--r--   0        0        0     1144 2023-06-15 16:31:59.930158 solutions_template-1.9.0/solutions_template/template_root/terraform/modules/ingress_gce/variables.tf
+-rw-r--r--   0        0        0     2926 2023-06-15 16:31:59.930393 solutions_template-1.9.0/solutions_template/template_root/terraform/modules/ingress_nginx/main.tf
+-rw-r--r--   0        0        0      692 2023-06-15 16:31:59.930656 solutions_template-1.9.0/solutions_template/template_root/terraform/modules/ingress_nginx/outputs.tf
+-rw-r--r--   0        0        0     1087 2023-06-15 16:31:59.931016 solutions_template-1.9.0/solutions_template/template_root/terraform/modules/ingress_nginx/variables.tf
+-rw-r--r--   0        0        0      827 2023-06-15 16:31:59.931291 solutions_template-1.9.0/solutions_template/template_root/terraform/modules/project_services/main.tf
+-rw-r--r--   0        0        0      773 2023-06-15 16:31:59.931538 solutions_template-1.9.0/solutions_template/template_root/terraform/modules/project_services/variables.tf
+-rw-r--r--   0        0        0      953 2023-06-15 16:31:59.931934 solutions_template-1.9.0/solutions_template/template_root/terraform/modules/service_account/main.tf
+-rw-r--r--   0        0        0     1037 2023-06-15 16:31:59.932426 solutions_template-1.9.0/solutions_template/template_root/terraform/modules/service_account/variables.tf
+-rw-r--r--   0        0        0     1529 2023-06-15 16:31:59.932733 solutions_template-1.9.0/solutions_template/template_root/terraform/modules/terraform_cicd/main.tf
+-rw-r--r--   0        0        0      677 2023-06-15 16:31:59.933018 solutions_template-1.9.0/solutions_template/template_root/terraform/modules/terraform_cicd/variables.tf
+-rw-r--r--   0        0        0     1333 2023-06-15 16:31:59.933248 solutions_template-1.9.0/solutions_template/template_root/terraform/modules/vpc_network/main.tf
+-rw-r--r--   0        0        0     1269 2023-06-15 16:31:59.933426 solutions_template-1.9.0/solutions_template/template_root/terraform/modules/vpc_network/variables.tf
+-rw-r--r--   0        0        0     2193 2023-06-15 16:31:59.933834 solutions_template-1.9.0/solutions_template/template_root/terraform/stages/1-bootstrap/main.tf
+-rw-r--r--   0        0        0      730 2023-06-15 16:31:59.934084 solutions_template-1.9.0/solutions_template/template_root/terraform/stages/1-bootstrap/output.tf
+-rw-r--r--   0        0        0       66 2023-06-15 16:31:59.934377 solutions_template-1.9.0/solutions_template/template_root/terraform/stages/1-bootstrap/terraform.tfvars
+-rw-r--r--   0        0        0     1071 2023-06-15 16:31:59.934790 solutions_template-1.9.0/solutions_template/template_root/terraform/stages/1-bootstrap/variables.tf
+-rw-r--r--   0        0        0      826 2023-06-15 16:31:59.935095 solutions_template-1.9.0/solutions_template/template_root/terraform/stages/2-foundation/backend.tf
+-rw-r--r--   0        0        0      517 2023-06-15 16:31:59.935395 solutions_template-1.9.0/solutions_template/template_root/terraform/stages/2-foundation/firestore_setup.tf
+-rw-r--r--   0        0        0     1568 2023-06-15 16:31:59.935538 solutions_template-1.9.0/solutions_template/template_root/terraform/stages/2-foundation/iam.tf
+-rw-r--r--   0        0        0     4252 2023-06-15 16:31:59.935804 solutions_template-1.9.0/solutions_template/template_root/terraform/stages/2-foundation/main.tf
+-rw-r--r--   0        0        0      997 2023-06-15 16:31:59.935925 solutions_template-1.9.0/solutions_template/template_root/terraform/stages/2-foundation/outputs.tf
+-rw-r--r--   0        0        0      835 2023-06-15 16:31:59.936181 solutions_template-1.9.0/solutions_template/template_root/terraform/stages/2-foundation/providers.tf
+-rw-r--r--   0        0        0      606 2023-06-15 16:31:59.936549 solutions_template-1.9.0/solutions_template/template_root/terraform/stages/2-foundation/terraform.tfvars
+-rw-r--r--   0        0        0     2546 2023-06-15 16:31:59.936876 solutions_template-1.9.0/solutions_template/template_root/terraform/stages/2-foundation/variables.tf
+-rw-r--r--   0        0        0      826 2023-06-15 16:31:59.937252 solutions_template-1.9.0/solutions_template/template_root/terraform/stages/3-components/backend.tf
+-rw-r--r--   0        0        0      835 2023-06-15 16:31:59.937397 solutions_template-1.9.0/solutions_template/template_root/terraform/stages/3-components/providers.tf
+-rw-r--r--   0        0        0      148 2023-06-15 16:31:59.937688 solutions_template-1.9.0/solutions_template/template_root/terraform/stages/3-components/terraform.tfvars
+-rw-r--r--   0        0        0     1679 2023-06-15 16:31:59.937915 solutions_template-1.9.0/solutions_template/template_root/terraform/stages/3-components/variables.tf
+-rw-r--r--   0        0        0        0 2023-06-15 16:31:59.937992 solutions_template-1.9.0/solutions_template/template_root/tests/__init__.py
+-rw-r--r--   0        0        0      825 2023-06-15 16:31:59.938319 solutions_template-1.9.0/solutions_template/template_root/tests/e2e/e2e_utils.py
+-rwxr-xr-x   0        0        0      364 2023-06-15 16:31:59.938529 solutions_template-1.9.0/solutions_template/template_root/utils/disable_org_policies.sh
+-rwxr-xr-x   0        0        0     1095 2023-06-15 16:31:59.938794 solutions_template-1.9.0/solutions_template/template_root/utils/init_env_vars.sh
+-rwxr-xr-x   0        0        0    13137 2023-06-15 16:31:59.939050 solutions_template-1.9.0/solutions_template/template_root/utils/setup_all.sh
+-rwxr-xr-x   0        0        0     2835 2023-06-15 16:31:59.939218 solutions_template-1.9.0/solutions_template/template_root/utils/setup_local.sh
+-rw-r--r--   0        0        0       81 2023-06-15 16:31:59.939607 solutions_template-1.9.0/solutions_template/template_root/{{_copier_conf.answers_file}}
+-rw-r--r--   0        0        0        0 2023-06-15 16:31:59.939700 solutions_template-1.9.0/solutions_template/tests/__init__.py
+-rw-r--r--   0        0        0     5822 1970-01-01 00:00:00.000000 solutions_template-1.9.0/PKG-INFO
```

### Comparing `solutions_template-1.10.0/LICENSE` & `solutions_template-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `solutions_template-1.10.0/README.md` & `solutions_template-1.9.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -81,17 +81,17 @@
 
 Go to the newly created project folder and initialize the solution.
 ```
 cd my-solution
 st infra init
 ```
 
-Add a RESTful API service with **Todo** data model to this solution.
+Add a RESTful API component with **Todo** data model to this solution.
 ```
-st components add restful_service
+st component add restful_service
 ```
 
 Fill details in the prompt:
 - Component name: **todo_service**
 - Resource name: **todo-service**
 - Relative path: **todo-service**
 - GCP region: **us-central1**
```

### Comparing `solutions_template-1.10.0/pyproject.toml` & `solutions_template-1.9.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "solutions-template"
-version = "1.10.0"
+version = "1.9.0"
 description = "A solution framework to generate a project with built-in structure and modules"
 authors = ["Jon Chen <jonchen@google.com>"]
 license = "Apache"
 readme = "README.md"
 homepage = "https://github.com/GoogleCloudPlatform/solutions-template"
 repository = "https://github.com/GoogleCloudPlatform/solutions-template"
 packages = [
@@ -23,15 +23,14 @@
 copier = "^7.2.0"
 pyyaml = "^6.0"
 typer = "^0.9.0"
 jinja2-time = "^0.2.0"
 copier-templates-extensions = "^0.3.0"
 pathlib = "^1.0.1"
 jinja2 = "^3.1.2"
-jinja2-strcase = "^0.0.2"
 
 [tool.poetry.group.dev.dependencies]
 python = ">=3.9,<4.0"
 copier-templates-extensions = "^0.3.0"
 copier = "^7.2.0"
 PyYAML = "^6.0"
 jinja2-time = "^0.2.0"
```

### Comparing `solutions_template-1.10.0/solutions_template/cli/cli.py` & `solutions_template-1.9.0/solutions_template/cli/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,35 +17,28 @@
 import typer, traceback, os
 import importlib.metadata
 from typing import Optional
 from typing_extensions import Annotated
 from copier import run_auto
 from pathlib import Path
 from .component import component_app
+from .tool import tool_app
 from .infra import infra_app
-from .template import template_app
 from .cli_utils import *
 
 __version__ = importlib.metadata.version("solutions-template")
-DEFAULT_DEPLOY_PROFILE = "default-deploy"
 
 app = typer.Typer(
     add_completion=False,
     help=
     "Solutions Template CLI. See https://github.com/GoogleCloudPlatform/solutions-template for details."
 )
-app.add_typer(component_app,
-              name="components",
-              help="Add or update components.")
-app.add_typer(infra_app,
-              name="infra",
-              help="Manage infrastructure (terraform).")
-app.add_typer(template_app,
-              name="template",
-              help="Create or update module templates.")
+app.add_typer(component_app, name="component")
+app.add_typer(tool_app, name="tool")
+app.add_typer(infra_app, name="infra")
 
 
 # Create a new solution
 @app.command()
 def new(folder_name,
         output_dir: Annotated[Optional[str], typer.Argument()] = ".",
         template_path=None,
@@ -112,67 +105,61 @@
   write_yaml(f"{solution_path}/st.yaml", st_yaml)
 
   print_success(f"Complete. Solution folder updated at {solution_path}.\n")
 
 
 # Build and deploy services.
 @app.command()
-def deploy(profile: str = DEFAULT_DEPLOY_PROFILE,
+def deploy(profile: str = "default-deploy",
            component: str = None,
-           dev: Optional[bool] = False,
            solution_path: Annotated[Optional[str],
                                     typer.Argument()] = ".",
            yes: Optional[bool] = False):
   """
   Build and deploy services.
   """
   validate_solution_folder(solution_path)
 
-  st_yaml = read_yaml(f"{solution_path}/st.yaml")
-  project_id = st_yaml["project_id"]
+  solution_yaml_dict = read_yaml(f"{solution_path}/st.yaml")
+  project_id = solution_yaml_dict["project_id"]
 
   if component:
     component_flag = f" -m {component} "
   else:
     component_flag = ""
 
-  if dev:
-    skaffold_command = "skaffold dev"
-  else:
-    skaffold_command = "skaffold run"
-
-  command = f"{skaffold_command} -p {profile} {component_flag} --default-repo=\"gcr.io/{project_id}\""
+  command = f"skaffold run -p {profile} {component_flag} --default-repo=\"gcr.io/{project_id}\""
   print("This will build and deploy all services using the command below:")
   print_highlight(command)
   confirm("\nThis may take a few minutes. Continue?", skip=yes)
   exec_shell(command, working_dir=solution_path)
 
 
 # Destory deployment.
 @app.command()
-def delete(profile: str = DEFAULT_DEPLOY_PROFILE,
-           component: str = None,
-           solution_path: Annotated[Optional[str],
-                                    typer.Argument()] = ".",
-           yes: Optional[bool] = False):
+def destroy(profile: str = "default",
+            component: str = None,
+            solution_path: Annotated[Optional[str],
+                                     typer.Argument()] = ".",
+            yes: Optional[bool] = False):
   """
-  Delete deployment.
+  Destory deployment.
   """
   validate_solution_folder(solution_path)
 
-  st_yaml = read_yaml(f"{solution_path}/st.yaml")
-  project_id = st_yaml["project_id"]
+  solution_yaml_dict = read_yaml(f"{solution_path}/st.yaml")
+  project_id = solution_yaml_dict["project_id"]
 
   if component:
     component_flag = f" -m {component} "
   else:
     component_flag = ""
 
   command = f"skaffold delete -p {profile} {component_flag} --default-repo=\"gcr.io/{project_id}\""
-  print("This will DELETE deployed services using the command below:")
+  print("This will DESTROY deployed services using the command below:")
   print_highlight(command)
   confirm("\nThis may take a few minutes. Continue?", default=False, skip=yes)
   exec_shell(command, working_dir=solution_path)
 
 
 @app.command()
 def version():
```

### Comparing `solutions_template-1.10.0/solutions_template/cli/cli_utils.py` & `solutions_template-1.9.0/solutions_template/cli/cli_utils.py`

 * *Files identical despite different names*

### Comparing `solutions_template-1.10.0/solutions_template/cli/component.py` & `solutions_template-1.9.0/solutions_template/cli/component.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,42 +58,46 @@
   answers_dict = get_answers_dict(answers)
   process_component("update", component_name, solution_path, data=answers_dict)
   print_success(
       f"Complete. Component {component_name} updated to solution at {solution_path}\n"
   )
 
 
-def update_component_to_root_yaml(component_name, answers, solution_path):
+def update_component_to_root_yaml(component_name, details, solution_path):
   # Update Solution root YAML with new component name.
   solution_yaml_dict = read_yaml(f"{solution_path}/st.yaml") or {}
   components = solution_yaml_dict["components"] or {}
-  components[component_name] = answers
+  components[component_name] = details
   solution_yaml_dict["components"] = components
   write_yaml(f"{solution_path}/st.yaml", solution_yaml_dict)
 
 
 def process_component(method, component_name, solution_path, data={}):
   destination_path = "."
   current_dir = os.path.dirname(__file__)
   answers_file = None
 
   # Get basic info from root st.yaml.
   root_st_yaml = read_yaml(f"{solution_path}/st.yaml")
-  component_answers = {}
 
   # If the component name is a Git URL, use the URL as-is in copier.
   if check_git_url(component_name):
     print(f"Loading component from remote Git URL: {component_name}")
     template_path = component_name
 
   # Otherwise, try to locate the component in local modules/ folder.
   else:
 
     if method == "update":
       data["component_name"] = component_name
+      component_path = f"{solution_path}/components/{component_name}"
+      if not os.path.exists(component_path):
+        raise FileNotFoundError(
+            f"Component {component_name} does not exist in './components' folder."
+        )
       if component_name not in root_st_yaml["components"]:
         raise NameError(
             f"Component {component_name} is not defined in the root yaml 'st.yaml' file."
         )
       component_answers = root_st_yaml["components"][component_name]
       component_template = component_answers["component_template"]
       template_path = f"{current_dir}/../modules/{component_template}"
@@ -110,27 +114,26 @@
     copier_dict = get_copier_yaml(template_path)
     destination_path = solution_path + "/" + copier_dict["_metadata"].get(
         "destination_path")
     destination_path = destination_path.replace("//", "/")
 
   data["project_id"] = root_st_yaml["project_id"]
   data["project_number"] = root_st_yaml["project_number"]
-  data["solution_path"] = solution_path
 
   # Run copier with data.
   worker = run_auto(template_path,
                     destination_path,
                     data=data,
                     answers_file=answers_file)
 
   # Get answer values inputed by user.
   answers = worker.answers.user
   for key, value in worker.answers.default.items():
     if key not in answers:
-      answers[key] = component_answers.get(key) or value
+      answers[key] = value
   answers["component_template"] = component_template
   answers["destination_path"] = copier_dict["_metadata"].get(
       "destination_path")
 
   # Update component's answer back to st.yaml.
   update_component_to_root_yaml(answers["component_name"], answers,
                                 solution_path)
@@ -149,20 +152,20 @@
 def list(solution_path: Annotated[Optional[str], typer.Argument()] = ".", ):
   root_st_yaml = read_yaml(f"{solution_path}/st.yaml")
   components = root_st_yaml.get("components", [])
   print("Installed components:\n")
   for component_name, properties in components.items():
     typer.echo(
         typer.style(f"- {component_name} ", fg=typer.colors.WHITE, bold=True) +
-        typer.style(f"(from: {properties['component_template']})",
+        typer.style(f"(module: {properties['component_template']})",
                     fg=typer.colors.BLACK,
                     bold=True))
   print()
 
 
 # List available components to add.
 @component_app.command()
 def available():
   current_dir = os.path.dirname(__file__)
   path = current_dir + "/../modules"
-  print("Available components to add:\n")
+  print("Available modules:\n")
   list_subfolders(path)
```

### Comparing `solutions_template-1.10.0/solutions_template/cli/infra.py` & `solutions_template-1.9.0/solutions_template/cli/infra.py`

 * *Files identical despite different names*

### Comparing `solutions_template-1.10.0/solutions_template/copier_extensions/st_helpers.py` & `solutions_template-1.9.0/solutions_template/copier_extensions/st_helpers.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,26 +10,19 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-import re, os, yaml
+import re
 import subprocess
 from jinja2.ext import Extension
 
 
-# Read YAML file and convert to a dict.
-def read_yaml(filepath):
-  with open(filepath) as f:
-    data = yaml.safe_load(f)
-  return data
-
-
 # Execute shell commands
 def exec_output(command, working_dir=".", stop_when_error=True):
   output = subprocess.check_output(command,
                                    cwd=working_dir,
                                    shell=True,
                                    text=True)
   return output
@@ -63,64 +56,39 @@
   return project_number
 
 
 def get_existing_firestore(project_id):
   """
     Get boolean whether to initialize Firestore.
     """
-  print(f"   (Retrieving Firestore databases list...)")
   command = f"gcloud alpha firestore databases list --format='value(databases[0].name)' --project='{project_id}' --quiet"
   database_name = exec_gcloud_output(command)
   return database_name
 
 
 def get_current_user(project_id):
   """
     Get current authenticated gcloud user.
     """
-  print(f"   (Retrieving current authenticated gcloud user...)")
   command = f"gcloud config list account --format 'value(core.account)' | head -n 1"
   email = exec_gcloud_output(command)
   return email
 
 
 def get_cloud_run_services(project_id):
   """
-    Get all deployed Cloud Run services.
+    Get current authenticated gcloud user.
     """
-  print(f"   (Retrieving existing Cloud Run services for {project_id}...)")
+  print(f"    (Retrieving existing Cloud Run services for {project_id}...)")
   command = f"gcloud run services list --format='value(name)'"
   service_names = exec_gcloud_output(command)
   service_names = re.sub(r"\n", ",", service_names)
   return service_names
 
 
-def get_cluster_value(arguments):
-  """
-    Get a specific GKE cluster value from describe.
-    """
-  key, cluster_name, region = arguments
-  print(f"   (Retrieving {key} from cluster {cluster_name}...)")
-  command = f"gcloud container clusters describe {cluster_name} --region={region} --format='value({key})'"
-  return exec_gcloud_output(command)
-
-
-def get_services_from_yaml(solution_path):
-  """
-    Get the service list from root yaml.
-    """
-  st_yaml = read_yaml(f"{solution_path}/st.yaml")
-  services = []
-  components = st_yaml.get("components", {})
-  for component_name, properties in components.items():
-    if properties.get("service_path"):
-      services.append(properties["resource_name"])
-  return ",".join(services)
-
-
 def convert_resource_name(resource_name):
   """
     Convert to valid resource_name: lower case, alpha-numeric, dash.
     """
   resource_name = re.sub(r"\W+", "", resource_name)
   resource_name = resource_name.replace(" ", "").replace("_", "-")
   resource_name = resource_name.lower()
@@ -138,11 +106,9 @@
 
   def __init__(self, environment):
     super().__init__(environment)
     environment.filters["get_project_number"] = get_project_number
     environment.filters["get_existing_firestore"] = get_existing_firestore
     environment.filters["get_current_user"] = get_current_user
     environment.filters["get_cloud_run_services"] = get_cloud_run_services
-    environment.filters["get_cluster_value"] = get_cluster_value
-    environment.filters["get_services_from_yaml"] = get_services_from_yaml
     environment.filters["convert_resource_name"] = convert_resource_name
     environment.filters["assert_non_empty"] = assert_non_empty
```

### Comparing `solutions_template-1.10.0/solutions_template/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/Dockerfile` & `solutions_template-1.9.0/solutions_template/modules/restful_service/components/{{component_name}}/Dockerfile`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{% raw %}{% if depend_on_common == true -%}
+{% if depend_on_common == true -%}
 ARG COMMON_IMAGE
 FROM ${COMMON_IMAGE}
 {% else %}
 FROM python:3.9-slim
 {%- endif %}
 
 
@@ -21,8 +21,7 @@
 
 # set environment variables
 ENV PYTHONDONTWRITEBYTECODE 1
 ENV PYTHONUNBUFFERED 1
 
 # ENTRYPOINT [ "python", "main.py", "--prod=True" ]
 ENTRYPOINT [ "python", "main.py" ]
-{% endraw %}
```

### Comparing `solutions_template-1.10.0/solutions_template/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/skaffold.yaml` & `solutions_template-1.9.0/solutions_template/modules/restful_service/components/{{component_name}}/skaffold.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{% raw %}apiVersion: skaffold/v4beta1
+apiVersion: skaffold/v4beta1
 kind: Config
 metadata:
   name: {{component_name}}
 
 {% if depend_on_common == true -%}
 # Requires the common image for shared data models or utils.
 requires:
@@ -124,8 +124,7 @@
 {%- endif %}
 
 {% if default_deploy == "gke" -%}
 # The default-deploy profile refer to gke profile above.
 - <<: *gke-profile
   name: default-deploy
 {%- endif %}
-{% endraw %}
```

### Comparing `solutions_template-1.10.0/solutions_template/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/src/main.py` & `solutions_template-1.9.0/solutions_template/template_root/components/common/src/common/testing/bq_client_fixture.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,8 +10,20 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-# TODO: Add main code below.
+"""
+DB Client fixture for re-use in testing
+"""
+
+import pytest
+from google.cloud.bigquery import Client
+
+client = Client()
+
+
+@pytest.fixture(scope="module")
+def client_fixture():
+  yield client
```

### Comparing `solutions_template-1.10.0/solutions_template/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/backend.tf` & `solutions_template-1.9.0/solutions_template/modules/terraform_gke/terraform/stages/2-gke/backend.tf`

 * *Files 5% similar despite different names*

```diff
@@ -13,11 +13,11 @@
  * See the License for the specific language governing permissions and
  * limitations under the License.
  *
  */
 
 terraform {
   backend "gcs" {
-    bucket = {% raw %}"{{project_id}}-tfstate"{% endraw %}
-    prefix = "stage/{{terraform_stage}}"
+    bucket = "{{project_id}}-tfstate"
+    prefix = "stage/2-gke"
   }
 }
```

### Comparing `solutions_template-1.10.0/solutions_template/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/main.tf` & `solutions_template-1.9.0/solutions_template/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/outputs.tf`

 * *Files 11% similar despite different names*

```diff
@@ -11,8 +11,10 @@
  * distributed under the License is distributed on an "AS IS" BASIS,
  * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  * See the License for the specific language governing permissions and
  * limitations under the License.
  *
  */
 
-# TODO: Add Terraform blocks below.
+output "lb_https_ip_address" {
+  value =  module.lb-http.external_ip
+}
```

### Comparing `solutions_template-1.10.0/solutions_template/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/providers.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/stages/2-foundation/providers.tf`

 * *Files 6% similar despite different names*

```diff
@@ -11,22 +11,22 @@
  * distributed under the License is distributed on an "AS IS" BASIS,
  * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  * See the License for the specific language governing permissions and
  * limitations under the License.
  *
  */
 
-# TODO: Update Terraform providers below.
-
 # Terraform Block
 terraform {
   required_providers {
     google = {
       source  = "hashicorp/google"
       version = ">= 4.65.2"
     }
   }
 }
 
 provider "google" {
   project = var.project_id
 }
+
+data "google_client_config" "default" {}
```

### Comparing `solutions_template-1.10.0/solutions_template/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/terraform.tfvars` & `solutions_template-1.9.0/solutions_template/template_root/terraform/modules/ingress_gce/outputs.tf`

 * *Files 14% similar despite different names*

```diff
@@ -11,13 +11,10 @@
  * distributed under the License is distributed on an "AS IS" BASIS,
  * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  * See the License for the specific language governing permissions and
  * limitations under the License.
  *
  */
 
-# TODO: Add Terraform variable with Jinja variables below.
-# Note for modules: Jinja variables are defined in copier.yaml.
-
-{% raw %}
-project_id = "{{project_id}}"
-{% endraw %}
+output "ingress_ip_address" {
+  value = local.global_static_ip_name
+}
```

### Comparing `solutions_template-1.10.0/solutions_template/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/variables.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/stages/1-bootstrap/output.tf`

 * *Files 18% similar despite different names*

```diff
@@ -11,18 +11,14 @@
  * distributed under the License is distributed on an "AS IS" BASIS,
  * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  * See the License for the specific language governing permissions and
  * limitations under the License.
  *
  */
 
-# TODO: Add Terraform blocks below.
-
-variable "project_id" {
-  type        = string
-  description = "GCP Project ID"
+output "project_id" {
+  value = var.project_id
+}
 
-  validation {
-    condition     = length(var.project_id) > 0
-    error_message = "The project_id value must be an non-empty string."
-  }
+output "tfstate-bucket" {
+  value = google_storage_bucket.tfstate-bucket.name
 }
```

### Comparing `solutions_template-1.10.0/solutions_template/modules/restful_service/components/{{component_name}}/README.md` & `solutions_template-1.9.0/solutions_template/modules/restful_service/components/{{component_name}}/README.md`

 * *Files identical despite different names*

### Comparing `solutions_template-1.10.0/solutions_template/modules/restful_service/components/{{component_name}}/src/config.py` & `solutions_template-1.9.0/solutions_template/modules/restful_service/components/{{component_name}}/src/config.py`

 * *Files identical despite different names*

### Comparing `solutions_template-1.10.0/solutions_template/modules/restful_service/components/{{component_name}}/src/main.py` & `solutions_template-1.9.0/solutions_template/modules/restful_service/components/{{component_name}}/src/main.py`

 * *Files identical despite different names*

### Comparing `solutions_template-1.10.0/solutions_template/modules/restful_service/components/{{component_name}}/src/models/{{data_model}}.py` & `solutions_template-1.9.0/solutions_template/modules/restful_service/components/{{component_name}}/src/models/{{data_model}}.py`

 * *Files identical despite different names*

### Comparing `solutions_template-1.10.0/solutions_template/modules/restful_service/components/{{component_name}}/src/routes/{{data_model_plural}}.py` & `solutions_template-1.9.0/solutions_template/modules/restful_service/components/{{component_name}}/src/routes/{{data_model_plural}}.py`

 * *Files identical despite different names*

### Comparing `solutions_template-1.10.0/solutions_template/modules/restful_service/components/{{component_name}}/src/schemas/{{data_model}}.py` & `solutions_template-1.9.0/solutions_template/modules/restful_service/components/{{component_name}}/src/schemas/{{data_model}}.py`

 * *Files identical despite different names*

### Comparing `solutions_template-1.10.0/solutions_template/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/deployment.yaml` & `solutions_template-1.9.0/solutions_template/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/deployment.yaml`

 * *Files identical despite different names*

### Comparing `solutions_template-1.10.0/solutions_template/modules/restful_service/copier.yaml` & `solutions_template-1.9.0/solutions_template/modules/restful_service/copier.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -9,20 +9,20 @@
   help: What is the name of this component (snake_case)?
   default: restful_service
   validator: "{% if not component_name %}Required{% endif %}"
 
 resource_name:
   type: str
   help: Resource name (lower case, alphanumeric characters, '-')?
-  default: "{{ component_name | to_kebab }}"
+  default: "{{ component_name | convert_resource_name }}"
   validator: "{% if not resource_name %}Required{% endif %}"
 
 service_path:
   type: str
-  help: "The relative path used in ingress as http://my-domain/[service_path]"
+  help: "The relative path used in http://my-domain/[service_path]"
   default: "{{resource_name}}"
 
 gcp_region:
   type: str
   help: Which Google Cloud region?
   default: us-central1
 
@@ -81,23 +81,21 @@
 
 _templates_suffix: ""
 
 _patch:
   - "skaffold.yaml"
 
 _exclude:
-  - "README.md"
   - "copier.yaml"
   - "copier_extensions"
   - ".terraform*"
   - ".tmp"
   - ".venv"
   - ".pytest_cache"
   - "__pycache__"
   - "*-debug.log"
   - ".skip"
 
 _jinja_extensions:
   - jinja2_time.TimeExtension
-  - jinja2_strcase.StrcaseExtension
   - copier_templates_extensions.TemplateExtensionLoader
   - ../../copier_extensions/st_helpers.py:SolutionsTemplateHelpersExtension
```

### Comparing `solutions_template-1.10.0/solutions_template/modules/restful_service/tests/e2e/{{component_name}}_e2e_test.py` & `solutions_template-1.9.0/solutions_template/modules/restful_service/tests/e2e/{{component_name}}_e2e_test.py`

 * *Files 15% similar despite different names*

```diff
@@ -29,15 +29,17 @@
       "Authorization": f"Bearer {auth_token}",
       "Accept": "application/json"
   }
   data = {
       "id": test_id,
       "title": "Title",
       "description": "Description",
-      "status": "New",
+      "is_done": False,
+      "created_at": "2023-06-12T19:37:58.151Z",
+      "modified_at": "2023-06-12T19:37:58.151Z"
   }
 
   # Create a new item
   url = service_url + f"/{{resource_name}}/{{data_model}}"
   res = requests.post(url, json=data, headers=headers)
   assert res.status_code == 200
 
@@ -68,28 +70,32 @@
       "Authorization": f"Bearer {auth_token}",
       "Accept": "application/json"
   }
   data = {
       "id": test_id,
       "title": "Title",
       "description": "Description",
-      "status": "New",
+      "is_done": False,
+      "created_at": "2023-06-12T19:37:58.151Z",
+      "modified_at": "2023-06-12T19:37:58.151Z"
   }
 
   # Create a new item
   url = service_url + f"/{{resource_name}}/{{data_model}}"
   res = requests.post(url, json=data, headers=headers)
   assert res.status_code == 200
 
   # Update the item by ID
   data = {
       "id": test_id,
       "title": "Updated Title",
       "description": "Updated description",
-      "status": "In Progress",
+      "is_done": False,
+      "created_at": "2023-06-12T19:37:58.151Z",
+      "modified_at": "2023-06-12T19:37:58.151Z"
   }
   url = service_url + f"/{{resource_name}}/{{data_model}}"
   res = requests.put(url, json=data, headers=headers)
   assert res.status_code == 200
 
   # Get the item by ID
   url = service_url + f"/{{resource_name}}/{{data_model}}/{test_id}"
@@ -98,15 +104,14 @@
   assert res.status_code == 200
 
   # Verify the content
   res_data = res.json()
   assert res_data["id"] == test_id
   assert res_data["title"] == "Updated Title"
   assert res_data["description"] == "Updated description"
-  assert res_data["status"] == "In Progress"
 
   # Clean up
   url = service_url + f"/{{resource_name}}/{{data_model}}/{test_id}"
   res = requests.delete(url, headers=headers)
   assert res.status_code == 200
 
   # Verify if the item is deleted
```

### Comparing `solutions_template-1.10.0/solutions_template/modules/restful_service/{{'.github' if use_github_action}}/workflows/unit_test_linter_{{component_name}}.yaml` & `solutions_template-1.9.0/solutions_template/modules/restful_service/{{'.github' if use_github_action}}/workflows/unit_test_linter_{{component_name}}.yaml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -10,26 +10,26 @@
       - "components/{{component_name}}"
       - ".github/workflows/unit_test_{{component_name}}.yaml"
       - ".pylintrc"
   workflow_dispatch:
 env:
   PROJECT_ID: {{project_id}}
 
+# copier:raw {% raw %}
 jobs:
   unit-test:
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
         python-version: [3.9]
         target-folder: [
             # TODO: Add all microservice folders below.
             components/{{component_name}},
           ]
-# copier:raw {% raw %}
     steps:
       - uses: actions/checkout@v3
 
       # https://github.com/google-github-actions/auth
       - id: "auth"
         name: Auth with Service Account
         uses: "google-github-actions/auth@v1"
```

### Comparing `solutions_template-1.10.0/solutions_template/modules/task_dispatch_service/components/{{component_name}}/src/config.py` & `solutions_template-1.9.0/solutions_template/template_root/components/common/src/common/config.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,16 +11,20 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 """
-  Sample Service config file
+Config module to setup common environment
 """
+
 import os
 
-PORT = os.environ["PORT"] if os.environ.get("PORT") is not None else 80
-PROJECT_ID = os.environ.get("PROJECT_ID") or \
-    os.environ.get("GOOGLE_CLOUD_PROJECT")
+PROJECT_ID = os.environ.get("PROJECT_ID", "")
+
+if PROJECT_ID != "":
+  os.environ["GOOGLE_CLOUD_PROJECT"] = PROJECT_ID
+
 DATABASE_PREFIX = os.getenv("DATABASE_PREFIX", "")
-SERVICE_NAME = os.getenv("SERVICE_NAME")
+
+NEO4J_URI = "bolt://neo4j-neo4j:7687"
```

### Comparing `solutions_template-1.10.0/solutions_template/modules/task_dispatch_service/components/{{component_name}}/src/models/task.py` & `solutions_template-1.9.0/solutions_template/template_root/components/common/src/common/models/example.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,53 +9,45 @@
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
+
 """
-Data model for Task. See https://octabyte.io/FireO/ for details.
+Data model for example list.
 """
 
 import os
 
-from fireo.models import Model
-from fireo.fields import IDField, TextField, DateTime, BooleanField, Field
-from fireo.queries.errors import ReferenceDocNotExist
+from firedantic import Model
+from firedantic.exceptions import ModelNotFoundError
 from datetime import datetime
 
 # GCP project_id from system's environment variable.
 PROJECT_ID = os.environ.get("PROJECT_ID", "")
 
 # Database prefix for integration and e2e test purpose.
 DATABASE_PREFIX = os.getenv("DATABASE_PREFIX", "")
 
 
-# Firebase data model in "{{data_model_plural}}" collection.
-class Task(Model):
-  """Task ORM class"""
-
-  class Meta:
-    ignore_none_field = False
-    collection_name = DATABASE_PREFIX + "{{data_model_plural}}"
-
-  id = IDField()
-  title = TextField()
-  description = TextField()
-  stage = TextField()
-  status = TextField()
-  complete = BooleanField()
-  created_at = DateTime()
-  modified_at = DateTime()
-
-  # Arbitrary data in JSON format.
-  data = Field()
+# Firebase data model in "examples" collection.
+class Example(Model):
+  """Example ORM class"""
+  __collection__ = "examples"
+
+  id: str = "1234"
+  title: str = "Title"
+  description: str = "Description"
+  is_done: bool = False
+  created_at: datetime
+  modified_at: datetime = None
 
   @classmethod
   def find_by_id(cls, id):
     try:
-      task = Task.collection.get(id)
-    except ReferenceDocNotExist:
+      example = Example.get_by_doc_id(id)
+    except ModelNotFoundError:
       return None
 
-    return task
+    return example
```

### Comparing `solutions_template-1.10.0/solutions_template/modules/task_dispatch_service/terraform/stages/3-task-dispatch-service/backend.tf` & `solutions_template-1.9.0/solutions_template/modules/terraform_gke/terraform/stages/3-ingress-gke/backend.tf`

 * *Files 4% similar despite different names*

```diff
@@ -14,10 +14,10 @@
  * limitations under the License.
  *
  */
 
 terraform {
   backend "gcs" {
     bucket = "{{project_id}}-tfstate"
-    prefix = "stage/3-task-dispatch-service"
+    prefix = "stage/2-ingress-gce"
   }
 }
```

### Comparing `solutions_template-1.10.0/solutions_template/modules/task_dispatch_service/terraform/stages/3-task-dispatch-service/providers.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/modules/terraform_cicd/variables.tf`

 * *Files 14% similar despite different names*

```diff
@@ -11,26 +11,11 @@
  * distributed under the License is distributed on an "AS IS" BASIS,
  * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  * See the License for the specific language governing permissions and
  * limitations under the License.
  *
  */
 
-# TODO: Update Terraform providers below.
-
-# Terraform Block
-terraform {
-  required_providers {
-    google = {
-      source  = "hashicorp/google"
-      version = ">= 4.65.2"
-    }
-    google-beta = {
-      source  = "hashicorp/google-beta"
-      version = ">= 4.65.2"
-    }
-  }
-}
-
-provider "google" {
-  project = var.project_id
-}
+variable "project_id" {
+  type        = string
+  description = "project ID"
+}
```

### Comparing `solutions_template-1.10.0/solutions_template/modules/task_dispatch_service/terraform/stages/3-task-dispatch-service/variables.tf` & `solutions_template-1.9.0/solutions_template/modules/terraform_gke/terraform/stages/3-ingress-gke/variables.tf`

 * *Files 18% similar despite different names*

```diff
@@ -11,16 +11,14 @@
  * distributed under the License is distributed on an "AS IS" BASIS,
  * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  * See the License for the specific language governing permissions and
  * limitations under the License.
  *
  */
 
-# TODO: Add Terraform blocks below.
-
 variable "project_id" {
   type        = string
   description = "GCP Project ID"
 
   validation {
     condition     = length(var.project_id) > 0
     error_message = "The project_id value must be an non-empty string."
@@ -34,44 +32,27 @@
 
   validation {
     condition     = length(var.region) > 0
     error_message = "The region value must be an non-empty string."
   }
 }
 
-variable "task_topic" {
-  type        = string
-  description = "Pub/Sub topic for Task"
-}
-
-variable "eventarc_trigger_name" {
-  type         = string
-  descritption = "EventArc trigger name"
-  default      = "trigger-task-pubsub"
-}
-
-variable "eventarc_gke_cluster" {
-  type        = string
-  description = "GKE cluster name used by EventArc"
-}
-
-variable "eventarc_gke_namespace" {
-  type        = string
-  description = "GKE cluster namespace used by EventArc"
-  default     = "default"
+variable "cluster_name" {
+  type    = string
+  default = "main-cluster"
 }
 
-variable "eventarc_gke_path" {
+variable "kubernetes_version" {
   type        = string
-  description = "GKE path used by EventArc"
-  default     = "/"
+  description = "Kubernetes version. See https://cloud.google.com/kubernetes-engine/docs/release-notes-stable"
 }
 
-variable "eventarc_gke_service" {
+variable "cert_issuer_email" {
   type        = string
-  description = "Destination GKE service"
+  description = "Cert Issuer Email"
 }
 
-variable "eventarc_cloudrun_service" {
+variable "api_domain" {
   type        = string
-  description = "Destination Cloud Run service"
+  description = "API endpoint domain, excluding protocol"
+  default     = "localhost"
 }
```

### Comparing `solutions_template-1.10.0/solutions_template/modules/terraform_gke/copier.yaml` & `solutions_template-1.9.0/solutions_template/modules/terraform_gke/copier.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -7,46 +7,36 @@
 component_name:
   type: str
   help: What is the name of this component (snake_case)?
   default: terraform_gke
 
 terraform_stage_name:
   type: str
-  help: Terraform stage name?
+  help: What is the name of this terraform stage?
   default: 2-gke
 
-resource_name:
-  type: str
-  help: Resource name (lower case, alphanumeric characters, '-')?
-  default: gke-ingress
-
 gcp_region:
   type: str
   help: Which Google Cloud region?
   default: us-central1
 
-cluster_name:
-  type: str
-  help: GKE cluster name?
-  default: main-cluster
-
 kubernetes_version:
   type: str
   help: Kubernetes version?
   default: 1.24.11-gke.1000
 
-node_machine_type:
+cors_allow_origins:
   type: str
-  help: GKE Node machine type (Compute Engine)?
-  default: n1-standard-4
+  help: Allow domains for CORS? (comma-seperated)
+  default: "http://localhost:4200,http://localhost:3000"
 
-private_cluster:
-  type: bool
-  help: Private cluster?
-  default: true
+cert_issuer_email:
+  type: str
+  help: Cert Issuer Email
+  default: "{{project_id | get_current_user}}"
 
 _answers_file: ".st/module_answers/{{component_name}}.yaml"
 
 _templates_suffix: ""
 
 _exclude:
   - "copier.yaml"
```

### Comparing `solutions_template-1.10.0/solutions_template/modules/terraform_gke/docs/components/{{component_name}}.md` & `solutions_template-1.9.0/solutions_template/modules/terraform_gke/docs/modules/{{component_name}}.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 This module defines a Terraform GKE setup stage named "2-gke".
 
 Main components after setup:
 - ./terraform/stage/2-gke
 
 ## Setup
 
-Run `st components add [COMPONENT_NAME]` to add this module.
+Run `st component add [COMPONENT_NAME]` to add this module.
 ```
 cd my-solution-folder
-st components add terraform_gke .
+st component add terraform_gke .
 ```
 
 Fill in the variables.
 ```
 🎤 What is the name of this terraform stage?
    2-gke
 🎤 Which Google Cloud region?
```

### Comparing `solutions_template-1.10.0/solutions_template/modules/terraform_gke/terraform/stages/2-gke/backend.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/stages/3-components/backend.tf`

 * *Files 10% similar despite different names*

```diff
@@ -12,12 +12,15 @@
  * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  * See the License for the specific language governing permissions and
  * limitations under the License.
  *
  */
 
 terraform {
+  {% if terraform_backend_gcs == true -%}
   backend "gcs" {
+    # Uncomment below and specify a GCS bucket for TF state.
     bucket = "{{project_id}}-tfstate"
-    prefix = "stage/2-gke"
+    prefix = "stage/3-components"
   }
+  {%- endif %}
 }
```

### Comparing `solutions_template-1.10.0/solutions_template/modules/terraform_gke/terraform/stages/2-gke/iam.tf` & `solutions_template-1.9.0/solutions_template/modules/terraform_gke/terraform/stages/2-gke/iam.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-1.10.0/solutions_template/modules/terraform_gke/terraform/stages/2-gke/main.tf` & `solutions_template-1.9.0/solutions_template/modules/terraform_gke/terraform/stages/2-gke/main.tf`

 * *Files 2% similar despite different names*

```diff
@@ -43,18 +43,18 @@
   namespace                 = "default"
   vpc_network               = local.vpc_network
   vpc_subnetwork            = local.vpc_subnetwork
   region                    = var.region
   secondary_ranges_pods     = local.secondary_ranges_pods
   secondary_ranges_services = local.secondary_ranges_services
   master_ipv4_cidr_block    = local.master_ipv4_cidr_block
-  enable_private_nodes      = var.private_cluster
+  enable_private_nodes      = true
   min_node_count            = 1
   max_node_count            = 10
-  machine_type              = var.node_machine_type
+  machine_type              = var.machine_type
 
   # This service account will be created in both GCP and GKE, and will be
   # used for workload federation in all microservices.
   # See microservices/sample_service/kustomize/base/deployment.yaml for example.
   service_account_name = "gke-sa"
 
   # See latest stable version at https://cloud.google.com/kubernetes-engine/docs/release-notes-stable
```

### Comparing `solutions_template-1.10.0/solutions_template/modules/terraform_gke/terraform/stages/2-gke/providers.tf` & `solutions_template-1.9.0/solutions_template/modules/terraform_gke/terraform/stages/2-gke/providers.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-1.10.0/solutions_template/modules/terraform_gke/terraform/stages/2-gke/variables.tf` & `solutions_template-1.9.0/solutions_template/modules/terraform_gke/terraform/stages/2-gke/variables.tf`

 * *Files 6% similar despite different names*

```diff
@@ -42,18 +42,23 @@
 }
 
 variable "kubernetes_version" {
   type        = string
   description = "Kubernetes version. See https://cloud.google.com/kubernetes-engine/docs/release-notes-stable"
 }
 
-variable "node_machine_type" {
+variable "machine_type" {
   type        = string
   description = "VM machine time"
   default     = "n1-standard-4"
 }
 
-variable "private_cluster" {
-  type        = bool
-  description = "Whether to use private nodes"
-  default     = true
+variable "cert_issuer_email" {
+  type        = string
+  description = "Cert Issuer Email"
+}
+
+variable "api_domain" {
+  type        = string
+  description = "API endpoint domain, excluding protocol"
+  default     = "localhost"
 }
```

### Comparing `solutions_template-1.10.0/solutions_template/modules/terraform_gke_ingress/terraform/modules/ingress_gce/main.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/modules/ingress_gce/main.tf`

 * *Files 18% similar despite different names*

```diff
@@ -35,48 +35,61 @@
     : google_compute_global_address.ingress_ip_address[0].name
   )
 }
 
 resource "google_compute_global_address" "ingress_ip_address" {
   count        = var.external_ip_address == null ? 1 : 0
   project      = var.project_id
-  name         = "gke-ingress-ip"
+  name         = "ingress-ip"
   address_type = "EXTERNAL"
 }
 
 resource "google_compute_managed_ssl_certificate" "managed_certificate" {
   provider = google-beta
 
-  name = var.managed_cert_name
+  name = "${var.cert-name}"
   managed {
-    domains = var.domains
+    domains = ["${var.domain}"]
   }
 }
 
+# resource "kubectl_manifest" "frontend_config" {
+#   yaml_body = <<YAML
+# apiVersion: networking.gke.io/v1beta1
+# kind: FrontendConfig
+# metadata:
+#   name: ingress-security-config
+# spec:
+#   sslPolicy: ${google_compute_ssl_policy.gke-ingress-ssl-policy.name}
+#   redirectToHttps:
+#     enabled: true
+# YAML
+# }
+
 resource "google_compute_ssl_policy" "gke-ingress-ssl-policy" {
   name            = "gke-ingress-ssl-policy"
   profile         = "MODERN"
   min_tls_version = "TLS_1_2"
 }
 
 # resource "kubernetes_ingress_v1" "default_ingress" {
 
 #   metadata {
 #     name = "default-ingress"
 #     annotations = {
 #       "kubernetes.io/ingress.class"                 = "gce"
 #       "kubernetes.io/ingress.global-static-ip-name" = local.global_static_ip_name
-#       "networking.gke.io/managed-certificates"      = var.managed_cert_name
-#       "networking.gke.io/v1beta1.FrontendConfig"    = var.frontend_config_name
+#       "networking.gke.io/managed-certificates"      = kubectl_manifest.managed_certificate.name
+#       "networking.gke.io/v1beta1.FrontendConfig"    = kubectl_manifest.frontend_config.name
 #     }
 #   }
 
 #   spec {
 #     rule {
-#       host = var.domains[0]
+#       host = var.api_domain
 #       http {
 #         # Sample Service
 #         path {
 #           backend {
 #             service {
 #               name = "sample-service"
 #               port {
@@ -86,8 +99,9 @@
 #           }
 #           path_type = "Prefix"
 #           path      = "/sample_service"
 #         }
 #       }
 #     }
 #   }
-# }
+
+}
```

### Comparing `solutions_template-1.10.0/solutions_template/modules/terraform_gke_ingress/terraform/modules/ingress_gce/outputs.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/modules/ingress_nginx/outputs.tf`

 * *Files 15% similar despite different names*

```diff
@@ -12,9 +12,9 @@
  * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  * See the License for the specific language governing permissions and
  * limitations under the License.
  *
  */
 
 output "ingress_ip_address" {
-  value = local.global_static_ip_name
+  value = google_compute_address.ingress_ip_address.address
 }
```

### Comparing `solutions_template-1.10.0/solutions_template/modules/terraform_gke_ingress/terraform/modules/ingress_gce/variables.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/modules/ingress_nginx/variables.tf`

 * *Files 12% similar despite different names*

```diff
@@ -21,29 +21,21 @@
 }
 
 variable "region" {
   type        = string
   description = "GCP region"
 }
 
-variable "external_ip_address" {
-  type    = string
-  default = null
-}
-
-variable "domains" {
-  type        = list(string)
-  description = "DNS domain list, excluding protocol. E.g. api.example.com"
-  default     = []
+variable "cert_issuer_email" {
+  type        = string
+  description = "email of the cert issuer"
 }
 
-variable "managed_cert_name" {
+variable "api_domain" {
   type        = string
-  description = "Managed certificate name"
-  default     = "managed-cert"
+  description = "API domain, excluding protocol. E.g. api.example.com"
 }
 
-variable "frontend_config_name" {
+variable "cors_allow_origins" {
   type        = string
-  description = "HTTP Load balancer frontend config name"
-  default     = "default-frontend-config"
+  description = "CORS allow origins, comma-separated."
 }
```

### Comparing `solutions_template-1.10.0/solutions_template/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/backend.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/modules/project_services/variables.tf`

 * *Files 14% similar despite different names*

```diff
@@ -11,13 +11,16 @@
  * distributed under the License is distributed on an "AS IS" BASIS,
  * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  * See the License for the specific language governing permissions and
  * limitations under the License.
  *
  */
 
-terraform {
-  backend "gcs" {
-    bucket = "{{project_id}}-tfstate"
-    prefix = "stage/3-gke-ingress"
-  }
+variable "project_id" {
+  type        = string
+  description = "project ID"
 }
+
+variable "services" {
+  type        = list(any)
+  description = "List of services to enable"
+}
```

### Comparing `solutions_template-1.10.0/solutions_template/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/iam.tf` & `solutions_template-1.9.0/solutions_template/modules/terraform_gke/terraform/stages/3-ingress-gke/iam.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-1.10.0/solutions_template/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/main.tf` & `solutions_template-1.9.0/solutions_template/modules/terraform_gke/terraform/stages/3-ingress-gke/main.tf`

 * *Files 17% similar despite different names*

```diff
@@ -33,14 +33,18 @@
   config = {
     bucket = "${var.project_id}-tfstate"
     prefix = "stage/2-foundation"
   }
 }
 
 module "ingress_gce" {
-  source               = "../../modules/ingress_gce"
-  project_id           = var.project_id
-  region               = var.region
-  domains              = var.domains
-  managed_cert_name    = var.managed_cert_name
-  frontend_config_name = var.frontend_config_name
+  depends_on = [module.gke]
+
+  source            = "../../modules/ingress_gce"
+  project_id        = var.project_id
+  cert_issuer_email = var.cert_issuer_email
+  region            = var.region
+
+  # API domain, excluding protocols. E.g. example.com.
+  api_domain         = var.api_domain
+  cors_allow_origins = var.cors_allow_origins
 }
```

### Comparing `solutions_template-1.10.0/solutions_template/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/providers.tf` & `solutions_template-1.9.0/solutions_template/modules/terraform_gke/terraform/stages/3-ingress-gke/providers.tf`

 * *Files 10% similar despite different names*

```diff
@@ -41,27 +41,27 @@
   project = var.project_id
 }
 
 data "google_client_config" "default" {}
 
 # Used by module.gke.
 provider "kubernetes" {
-  host                   = "https://${var.cluster_external_endpoint}"
+  host                   = "https://${module.gke.endpoint}"
   token                  = data.google_client_config.default.access_token
-  cluster_ca_certificate = base64decode(var.cluster_ca_certificate)
+  cluster_ca_certificate = base64decode(module.gke.ca_certificate)
 }
 
 # Used by module.ingress.
 provider "kubectl" {
-  host                   = "https://${var.cluster_external_endpoint}"
+  host                   = "https://${module.gke.endpoint}"
   token                  = data.google_client_config.default.access_token
-  cluster_ca_certificate = base64decode(var.cluster_external_endpoint)
+  cluster_ca_certificate = base64decode(module.gke.ca_certificate)
   load_config_file       = false
 }
 
 provider "helm" {
   kubernetes {
-    host                   = "https://${var.cluster_external_endpoint}"
+    host                   = "https://${module.gke.endpoint}"
     token                  = data.google_client_config.default.access_token
-    cluster_ca_certificate = base64decode(var.cluster_external_endpoint)
+    cluster_ca_certificate = base64decode(module.gke.ca_certificate)
   }
 }
```

### Comparing `solutions_template-1.10.0/solutions_template/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/variables.tf` & `solutions_template-1.9.0/solutions_template/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/variables.tf`

 * *Files 16% similar despite different names*

```diff
@@ -24,47 +24,46 @@
     error_message = "The project_id value must be an non-empty string."
   }
 }
 
 variable "region" {
   type        = string
   description = "Default GCP region"
-  default     = "us-central1"
 
   validation {
     condition     = length(var.region) > 0
     error_message = "The region value must be an non-empty string."
   }
 }
 
-variable "cluster_name" {
-  type    = string
-  default = "main-cluster"
+variable "loadbalancer_name" {
+  type = string
+  default = "http-lb"
 }
 
-variable "cluster_external_endpoint" {
-  type        = string
-  description = "Cluster external endpoint IP address"
+variable "domains" {
+  type = string
+  description = "List of domains attached to the LB, comma-separated."
 }
 
-variable "cluster_ca_certificate" {
-  type        = string
-  description = "Cluster CA certificate"
+variable "cloudrun_services" {
+  type = string
+  description = "List of Cloud Run service names, comma-separated."
 }
 
-variable "domains" {
-  type        = list(string)
-  description = "DNS domain list, excluding protocol. E.g. api.example.com"
-  default     = []
+variable "security_policy" {
+  description = "The resource URL for the security policy to associate with the backend service"
+  type        = string
+  default     = null
 }
 
-variable "managed_cert_name" {
+variable "edge_security_policy" {
+  description = "The resource URL for the edge security policy to associate with the backend service"
   type        = string
-  description = "Managed certificate name"
-  default     = "managed-cert"
+  default     = null
 }
 
-variable "frontend_config_name" {
+variable "load_balancing_scheme" {
+  description = "Load balancing scheme type (EXTERNAL for classic external load balancer, EXTERNAL_MANAGED for Envoy-based load balancer, and INTERNAL_SELF_MANAGED for traffic director)"
   type        = string
-  description = "HTTP Load balancer frontend config name"
-  default     = "default-frontend-config"
+  default     = "EXTERNAL"
 }
```

### Comparing `solutions_template-1.10.0/solutions_template/modules/terraform_httplb_cloudrun/copier.yaml` & `solutions_template-1.9.0/solutions_template/modules/terraform_httplb_cloudrun/copier.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 _metadata:
-  module_name: terraform_httplb_cloudrun
+  module_name: terraform_serverless_ingress
   version: 1.0.0
   destination_path: .
 
 # questions
 component_name:
   type: str
   help: What is the name of this component?
-  default: terraform_httplb_cloudrun
+  default: terraform_serverless_ingress
 
 loadbalancer_name:
   type: str
   help: Name of the HTTP load balancer?
   default: httplb-cloudrun
 
 region:
```

### Comparing `solutions_template-1.10.0/solutions_template/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/backend.tf` & `solutions_template-1.9.0/solutions_template/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/backend.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-1.10.0/solutions_template/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/main.tf` & `solutions_template-1.9.0/solutions_template/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-1.10.0/solutions_template/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/outputs.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/modules/project_services/main.tf`

 * *Files 18% similar despite different names*

```diff
@@ -11,10 +11,13 @@
  * distributed under the License is distributed on an "AS IS" BASIS,
  * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  * See the License for the specific language governing permissions and
  * limitations under the License.
  *
  */
 
-output "lb_https_ip_address" {
-  value =  module.lb-http.external_ip
-}
+resource "google_project_service" "project-apis" {
+  for_each                   = toset(var.services)
+  project                    = var.project_id
+  service                    = each.value
+  disable_dependent_services = true
+}
```

### Comparing `solutions_template-1.10.0/solutions_template/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/providers.tf` & `solutions_template-1.9.0/solutions_template/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/providers.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-1.10.0/solutions_template/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/variables.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/modules/compute_backend/variables.tf`

 * *Files 20% similar despite different names*

```diff
@@ -1,69 +1,49 @@
 /**
  * Copyright 2022 Google LLC
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at
  *
- *     https://www.apache.org/licenses/LICENSE-2.0
+ *      http://www.apache.org/licenses/LICENSE-2.0
  *
  * Unless required by applicable law or agreed to in writing, software
  * distributed under the License is distributed on an "AS IS" BASIS,
  * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  * See the License for the specific language governing permissions and
  * limitations under the License.
- *
  */
 
-variable "project_id" {
+variable "project" {
+  description = "The project to deploy to, if not set the default provider project is used."
   type        = string
-  description = "GCP Project ID"
-
-  validation {
-    condition     = length(var.project_id) > 0
-    error_message = "The project_id value must be an non-empty string."
-  }
 }
 
-variable "region" {
+variable "name" {
+  description = "Name for the forwarding rule and prefix for supporting resources"
   type        = string
-  description = "Default GCP region"
-
-  validation {
-    condition     = length(var.region) > 0
-    error_message = "The region value must be an non-empty string."
-  }
-}
-
-variable "loadbalancer_name" {
-  type = string
-  default = "http-lb"
-}
-
-variable "domains" {
-  type = string
-  description = "List of domains attached to the LB, comma-separated."
 }
 
-variable "cloudrun_services" {
-  type = string
-  description = "List of Cloud Run service names, comma-separated."
+variable "backends" {
+  description = "Map backend indices to list of backend maps."
+  type = map(any)
 }
 
-variable "security_policy" {
-  description = "The resource URL for the security policy to associate with the backend service"
+variable "edge_security_policy" {
+  description = "The resource URL for the edge security policy to associate with the backend service"
   type        = string
   default     = null
 }
 
-variable "edge_security_policy" {
-  description = "The resource URL for the edge security policy to associate with the backend service"
+variable "security_policy" {
+  description = "The resource URL for the security policy to associate with the backend service"
   type        = string
   default     = null
 }
 
 variable "load_balancing_scheme" {
   description = "Load balancing scheme type (EXTERNAL for classic external load balancer, EXTERNAL_MANAGED for Envoy-based load balancer, and INTERNAL_SELF_MANAGED for traffic director)"
   type        = string
   default     = "EXTERNAL"
 }
+
```

### Comparing `solutions_template-1.10.0/solutions_template/template_root/.github/assets/setup_local.png` & `solutions_template-1.9.0/solutions_template/template_root/.github/assets/setup_local.png`

 * *Files identical despite different names*

### Comparing `solutions_template-1.10.0/solutions_template/template_root/.github/assets/skaffold_dev_terminal.png` & `solutions_template-1.9.0/solutions_template/template_root/.github/assets/skaffold_dev_terminal.png`

 * *Files identical despite different names*

### Comparing `solutions_template-1.10.0/solutions_template/template_root/.github/workflows/deployment_cloudrun_dev.yaml` & `solutions_template-1.9.0/solutions_template/template_root/.github/workflows/deployment_cloudrun_dev.yaml`

 * *Files identical despite different names*

### Comparing `solutions_template-1.10.0/solutions_template/template_root/.github/workflows/deployment_gke_dev.yaml` & `solutions_template-1.9.0/solutions_template/template_root/.github/workflows/deployment_gke_dev.yaml`

 * *Files identical despite different names*

### Comparing `solutions_template-1.10.0/solutions_template/template_root/.github/workflows/e2e_cloudrun_api_test.yaml` & `solutions_template-1.9.0/solutions_template/template_root/.github/workflows/e2e_cloudrun_api_test.yaml`

 * *Files identical despite different names*

### Comparing `solutions_template-1.10.0/solutions_template/template_root/.github/workflows/e2e_gke_api_test.yaml` & `solutions_template-1.9.0/solutions_template/template_root/.github/workflows/e2e_gke_api_test.yaml`

 * *Files identical despite different names*

### Comparing `solutions_template-1.10.0/solutions_template/template_root/.github/workflows/unit_test_linter_common.yaml` & `solutions_template-1.9.0/solutions_template/template_root/.github/workflows/unit_test_linter_common.yaml`

 * *Files identical despite different names*

### Comparing `solutions_template-1.10.0/solutions_template/template_root/.pylintrc` & `solutions_template-1.9.0/solutions_template/template_root/.pylintrc`

 * *Files identical despite different names*

### Comparing `solutions_template-1.10.0/solutions_template/template_root/README.md` & `solutions_template-1.9.0/solutions_template/template_root/README.md`

 * *Files identical despite different names*

### Comparing `solutions_template-1.10.0/solutions_template/template_root/components/common/skaffold.yaml` & `solutions_template-1.9.0/solutions_template/template_root/components/common/skaffold.yaml`

 * *Files identical despite different names*

### Comparing `solutions_template-1.10.0/solutions_template/template_root/components/common/src/common/config.py` & `solutions_template-1.9.0/solutions_template/template_root/terraform/modules/gke/outputs.tf`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,28 @@
-"""
-Copyright 2022 Google LLC
-
-Licensed under the Apache License, Version 2.0 (the "License");
-you may not use this file except in compliance with the License.
-You may obtain a copy of the License at
-
-    https://www.apache.org/licenses/LICENSE-2.0
-
-Unless required by applicable law or agreed to in writing, software
-distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-See the License for the specific language governing permissions and
-limitations under the License.
-"""
-
-"""
-Config module to setup common environment
-"""
-
-import os
-
-PROJECT_ID = os.environ.get("PROJECT_ID", "")
-
-if PROJECT_ID != "":
-  os.environ["GOOGLE_CLOUD_PROJECT"] = PROJECT_ID
-
-DATABASE_PREFIX = os.getenv("DATABASE_PREFIX", "")
-
-NEO4J_URI = "bolt://neo4j-neo4j:7687"
+/**
+ * Copyright 2022 Google LLC
+ *
+ * Licensed under the Apache License, Version 2.0 (the "License");
+ * you may not use this file except in compliance with the License.
+ * You may obtain a copy of the License at
+ *
+ *     https://www.apache.org/licenses/LICENSE-2.0
+ *
+ * Unless required by applicable law or agreed to in writing, software
+ * distributed under the License is distributed on an "AS IS" BASIS,
+ * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+ * See the License for the specific language governing permissions and
+ * limitations under the License.
+ *
+ */
+
+output "gke_cluster" {
+  value = try(module.gke_cluster.cluster_id, null)
+}
+
+output "endpoint" {
+  value = try(module.gke_cluster.endpoint, null)
+}
+
+output "ca_certificate" {
+  value = try(module.gke_cluster.ca_certificate, null)
+}
```

### Comparing `solutions_template-1.10.0/solutions_template/template_root/components/common/src/common/db_client.py` & `solutions_template-1.9.0/solutions_template/template_root/components/common/src/common/db_client.py`

 * *Files identical despite different names*

### Comparing `solutions_template-1.10.0/solutions_template/template_root/components/common/src/common/testing/bq_client_fixture.py` & `solutions_template-1.9.0/solutions_template/template_root/components/common/src/common/testing/client_with_emulator.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,19 +11,23 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 """
-DB Client fixture for re-use in testing
+  Pytest Fixture for getting testclient from fastapi
 """
 
-import pytest
-from google.cloud.bigquery import Client
+# disabling pylint rules that conflict with pytest fixtures
+# pylint: disable=unused-argument,redefined-outer-name,unused-import
 
-client = Client()
+import pytest
+from .firestore_emulator import clean_firestore
+from fastapi.testclient import TestClient
+from main import app
 
 
-@pytest.fixture(scope="module")
-def client_fixture():
-  yield client
+@pytest.fixture
+def client_with_emulator(clean_firestore, scope="module"):
+  test_client = TestClient(app)
+  yield test_client
```

### Comparing `solutions_template-1.10.0/solutions_template/template_root/components/common/src/common/testing/firestore_emulator.py` & `solutions_template-1.9.0/solutions_template/template_root/components/common/src/common/testing/firestore_emulator.py`

 * *Files identical despite different names*

### Comparing `solutions_template-1.10.0/solutions_template/template_root/components/common/src/common/utils/logging_handler.py` & `solutions_template-1.9.0/solutions_template/template_root/components/common/src/common/utils/logging_handler.py`

 * *Files identical despite different names*

### Comparing `solutions_template-1.10.0/solutions_template/template_root/copier.yaml` & `solutions_template-1.9.0/solutions_template/template_root/copier.yaml`

 * *Files identical despite different names*

### Comparing `solutions_template-1.10.0/solutions_template/template_root/terraform/modules/cloudbuild/main.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/modules/cloudbuild/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-1.10.0/solutions_template/template_root/terraform/modules/cloudbuild/variables.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/modules/cloudbuild/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-1.10.0/solutions_template/template_root/terraform/modules/cloudrun/main.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/modules/cloudrun/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-1.10.0/solutions_template/template_root/terraform/modules/cloudrun/variables.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/modules/cloudrun/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-1.10.0/solutions_template/template_root/terraform/modules/compute_backend/main.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/modules/compute_backend/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-1.10.0/solutions_template/template_root/terraform/modules/compute_backend/providers.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/modules/compute_backend/providers.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-1.10.0/solutions_template/template_root/terraform/modules/firebase/main.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/modules/firebase/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-1.10.0/solutions_template/template_root/terraform/modules/firebase/variables.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/modules/firebase/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-1.10.0/solutions_template/template_root/terraform/modules/gke/main.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/modules/gke/main.tf`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
   http_load_balancing               = true
   identity_namespace                = "enabled"
   horizontal_pod_autoscaling        = true
   remove_default_node_pool          = true
 
   node_pools = [
     {
-      name               = var.node_pool_name
+      name               = "default-pool"
       machine_type       = var.machine_type
       min_count          = var.min_node_count
       max_count          = var.max_node_count
       disk_size_gb       = var.disk_size_gb
       disk_type          = "pd-standard"
       image_type         = "COS_CONTAINERD"
       auto_repair        = true
```

### Comparing `solutions_template-1.10.0/solutions_template/template_root/terraform/modules/gke/outputs.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/stages/1-bootstrap/variables.tf`

 * *Files 25% similar despite different names*

```diff
@@ -11,18 +11,25 @@
  * distributed under the License is distributed on an "AS IS" BASIS,
  * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  * See the License for the specific language governing permissions and
  * limitations under the License.
  *
  */
 
-output "gke_cluster" {
-  value = try(module.gke_cluster.cluster_id, null)
-}
+variable "project_id" {
+  type        = string
+  description = "GCP Project ID"
 
-output "endpoint" {
-  value = try(module.gke_cluster.endpoint, null)
+  validation {
+    condition     = length(var.project_id) > 0
+    error_message = "The project_id value must be an non-empty string."
+  }
 }
 
-output "ca_certificate" {
-  value = try(module.gke_cluster.ca_certificate, null)
+variable "storage_multiregion" {
+  type        = string
+  description = "Storage Region or Multiregion"
+  validation {
+    condition     = length(var.storage_multiregion) > 0
+    error_message = "The region value must be an non-empty string."
+  }
 }
```

### Comparing `solutions_template-1.10.0/solutions_template/template_root/terraform/modules/gke/variables.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/modules/gke/variables.tf`

 * *Files 2% similar despite different names*

```diff
@@ -36,19 +36,14 @@
 }
 
 variable "region" {
   type        = string
   description = "cluster region"
 }
 
-variable "node_pool_name" {
-  type    = str
-  default = "default-pool"
-}
-
 variable "enable_private_nodes" {
   type        = bool
   description = "Whether nodes have internal IP addresses only"
   default     = true
 }
 
 variable "min_node_count" {
```

### Comparing `solutions_template-1.10.0/solutions_template/template_root/terraform/modules/ingress_nginx/main.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/modules/ingress_nginx/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-1.10.0/solutions_template/template_root/terraform/modules/ingress_nginx/outputs.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/modules/service_account/main.tf`

 * *Files 24% similar despite different names*

```diff
@@ -11,10 +11,17 @@
  * distributed under the License is distributed on an "AS IS" BASIS,
  * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  * See the License for the specific language governing permissions and
  * limitations under the License.
  *
  */
 
-output "ingress_ip_address" {
-  value = google_compute_address.ingress_ip_address.address
+module "service_accounts" {
+  source        = "terraform-google-modules/service-accounts/google"
+  version       = "~> 3.0"
+  project_id    = var.project_id
+  names         = ["${var.name}"]
+  display_name  = var.display_name
+  description   = var.description
+  project_roles = [for i in var.roles : "${var.project_id}=>${i}"]
+  generate_keys = false
 }
```

### Comparing `solutions_template-1.10.0/solutions_template/template_root/terraform/modules/ingress_nginx/variables.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/modules/ingress_gce/variables.tf`

 * *Files 10% similar despite different names*

```diff
@@ -21,21 +21,26 @@
 }
 
 variable "region" {
   type        = string
   description = "GCP region"
 }
 
-variable "cert_issuer_email" {
-  type        = string
-  description = "email of the cert issuer"
+variable "external_ip_address" {
+  type    = string
+  default = null
 }
 
-variable "api_domain" {
+variable "domain" {
   type        = string
   description = "API domain, excluding protocol. E.g. api.example.com"
 }
 
-variable "cors_allow_origins" {
+variable "cert_name" {
+  type        = string
+  description = "SSL certificate name"
+}
+
+variable "cors_allow_originss" {
   type        = string
   description = "CORS allow origins, comma-separated."
 }
```

### Comparing `solutions_template-1.10.0/solutions_template/template_root/terraform/modules/service_account/variables.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/modules/service_account/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-1.10.0/solutions_template/template_root/terraform/modules/terraform_cicd/main.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/modules/terraform_cicd/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-1.10.0/solutions_template/template_root/terraform/modules/terraform_cicd/variables.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/stages/2-foundation/outputs.tf`

 * *Files 27% similar despite different names*

```diff
@@ -11,11 +11,30 @@
  * distributed under the License is distributed on an "AS IS" BASIS,
  * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  * See the License for the specific language governing permissions and
  * limitations under the License.
  *
  */
 
-variable "project_id" {
-  type        = string
-  description = "project ID"
-}
+output "vpc_network" {
+  value =  var.vpc_network
+}
+
+output "vpc_subnetwork" {
+  value =  var.vpc_subnetwork
+}
+
+output "ip_cidr_range" {
+  value =  var.ip_cidr_range
+}
+
+output "master_ipv4_cidr_block" {
+  value =  var.master_ipv4_cidr_block
+}
+
+output "secondary_ranges_pods" {
+  value =  var.secondary_ranges_pods
+}
+
+output "secondary_ranges_services" {
+  value =  var.secondary_ranges_services
+}
```

### Comparing `solutions_template-1.10.0/solutions_template/template_root/terraform/modules/vpc_network/main.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/modules/vpc_network/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-1.10.0/solutions_template/template_root/terraform/modules/vpc_network/variables.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/modules/vpc_network/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-1.10.0/solutions_template/template_root/terraform/stages/1-bootstrap/main.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/stages/1-bootstrap/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-1.10.0/solutions_template/template_root/terraform/stages/2-foundation/backend.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/stages/2-foundation/backend.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-1.10.0/solutions_template/template_root/terraform/stages/2-foundation/firestore_setup.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/stages/2-foundation/firestore_setup.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-1.10.0/solutions_template/template_root/terraform/stages/2-foundation/iam.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/stages/2-foundation/iam.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-1.10.0/solutions_template/template_root/terraform/stages/2-foundation/main.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/stages/2-foundation/main.tf`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,14 @@
     "bigquery.googleapis.com",             # BigQuery
     "bigquerydatatransfer.googleapis.com", # BigQuery Data Transfer
     "cloudbuild.googleapis.com",           # Cloud Build
     "compute.googleapis.com",              # Compute Engine
     "container.googleapis.com",            # Google Kubernetes Engine
     "containerregistry.googleapis.com",    # Google Container Registry
     "dataflow.googleapis.com",             # Cloud Dataflow
-    "eventarc.googleapis.com",             # Event Arc
     "firebase.googleapis.com",             # Firebase
     "firestore.googleapis.com",            # Firestore
     "iam.googleapis.com",                  # Cloud IAM
     "logging.googleapis.com",              # Cloud Logging
     "monitoring.googleapis.com",           # Cloud Operations Suite
     "run.googleapis.com",                  # Cloud Run
     "secretmanager.googleapis.com",        # Secret Manager
```

### Comparing `solutions_template-1.10.0/solutions_template/template_root/terraform/stages/2-foundation/providers.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/stages/3-components/providers.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-1.10.0/solutions_template/template_root/terraform/stages/2-foundation/terraform.tfvars` & `solutions_template-1.9.0/solutions_template/template_root/terraform/stages/2-foundation/terraform.tfvars`

 * *Files identical despite different names*

### Comparing `solutions_template-1.10.0/solutions_template/template_root/terraform/stages/2-foundation/variables.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/stages/2-foundation/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-1.10.0/solutions_template/template_root/tests/e2e/e2e_utils.py` & `solutions_template-1.9.0/solutions_template/template_root/tests/e2e/e2e_utils.py`

 * *Files identical despite different names*

### Comparing `solutions_template-1.10.0/solutions_template/template_root/utils/init_env_vars.sh` & `solutions_template-1.9.0/solutions_template/template_root/utils/init_env_vars.sh`

 * *Files identical despite different names*

### Comparing `solutions_template-1.10.0/solutions_template/template_root/utils/setup_all.sh` & `solutions_template-1.9.0/solutions_template/template_root/utils/setup_all.sh`

 * *Files identical despite different names*

### Comparing `solutions_template-1.10.0/solutions_template/template_root/utils/setup_local.sh` & `solutions_template-1.9.0/solutions_template/template_root/utils/setup_local.sh`

 * *Files identical despite different names*

### Comparing `solutions_template-1.10.0/PKG-INFO` & `solutions_template-1.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: solutions-template
-Version: 1.10.0
+Version: 1.9.0
 Summary: A solution framework to generate a project with built-in structure and modules
 Home-page: https://github.com/GoogleCloudPlatform/solutions-template
 License: Apache
 Author: Jon Chen
 Author-email: jonchen@google.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: copier (>=7.2.0,<8.0.0)
 Requires-Dist: copier-templates-extensions (>=0.3.0,<0.4.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
-Requires-Dist: jinja2-strcase (>=0.0.2,<0.0.3)
 Requires-Dist: jinja2-time (>=0.2.0,<0.3.0)
 Requires-Dist: pathlib (>=1.0.1,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
 Project-URL: Repository, https://github.com/GoogleCloudPlatform/solutions-template
 Description-Content-Type: text/markdown
 
@@ -106,17 +105,17 @@
 
 Go to the newly created project folder and initialize the solution.
 ```
 cd my-solution
 st infra init
 ```
 
-Add a RESTful API service with **Todo** data model to this solution.
+Add a RESTful API component with **Todo** data model to this solution.
 ```
-st components add restful_service
+st component add restful_service
 ```
 
 Fill details in the prompt:
 - Component name: **todo_service**
 - Resource name: **todo-service**
 - Relative path: **todo-service**
 - GCP region: **us-central1**
```

