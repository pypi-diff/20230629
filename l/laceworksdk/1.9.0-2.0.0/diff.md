# Comparing `tmp/laceworksdk-1.9.0.tar.gz` & `tmp/laceworksdk-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "laceworksdk-1.9.0.tar", last modified: Fri Feb 24 19:19:32 2023, max compression
+gzip compressed data, was "laceworksdk-2.0.0.tar", max compression
```

## Comparing `laceworksdk-1.9.0.tar` & `laceworksdk-2.0.0.tar`

### file list

```diff
@@ -1,282 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 19:19:32.434793 laceworksdk-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 19:19:32.406793 laceworksdk-1.9.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 19:19:32.406793 laceworksdk-1.9.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/.github/workflows/python-test-flaky.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/.github/workflows/python-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/.github/workflows/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5167 2023-02-24 19:19:32.434793 laceworksdk-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 19:19:32.406793 laceworksdk-1.9.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/docs/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 19:19:32.406793 laceworksdk-1.9.0/docs/laceworksdk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 19:19:32.410793 laceworksdk-1.9.0/docs/laceworksdk/api/
--rw-r--r--   0 runner    (1001) docker     (123)   109615 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/docs/laceworksdk/api/base_endpoint.html
--rw-r--r--   0 runner    (1001) docker     (123)   105824 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/docs/laceworksdk/api/crud_endpoint.html
--rw-r--r--   0 runner    (1001) docker     (123)    69307 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/docs/laceworksdk/api/search_endpoint.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 19:19:32.410793 laceworksdk-1.9.0/docs/laceworksdk/api/v1/
--rw-r--r--   0 runner    (1001) docker     (123)    54323 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/docs/laceworksdk/api/v1/account.html
--rw-r--r--   0 runner    (1001) docker     (123)   152158 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/docs/laceworksdk/api/v1/compliance.html
--rw-r--r--   0 runner    (1001) docker     (123)    68313 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/docs/laceworksdk/api/v1/custom_compliance_config.html
--rw-r--r--   0 runner    (1001) docker     (123)    57347 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/docs/laceworksdk/api/v1/download_file.html
--rw-r--r--   0 runner    (1001) docker     (123)    82934 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/docs/laceworksdk/api/v1/events.html
--rw-r--r--   0 runner    (1001) docker     (123)   190081 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/docs/laceworksdk/api/v1/integrations.html
--rw-r--r--   0 runner    (1001) docker     (123)    72534 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/docs/laceworksdk/api/v1/recommendations.html
--rw-r--r--   0 runner    (1001) docker     (123)    87562 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/docs/laceworksdk/api/v1/run_reports.html
--rw-r--r--   0 runner    (1001) docker     (123)    91534 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/docs/laceworksdk/api/v1/suppressions.html
--rw-r--r--   0 runner    (1001) docker     (123)   128143 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/docs/laceworksdk/api/v1/token.html
--rw-r--r--   0 runner    (1001) docker     (123)   266382 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/docs/laceworksdk/api/v1/vulnerability.html
--rw-r--r--   0 runner    (1001) docker     (123)    35203 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/docs/laceworksdk/api/v1.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 19:19:32.414793 laceworksdk-1.9.0/docs/laceworksdk/api/v2/
--rw-r--r--   0 runner    (1001) docker     (123)    77673 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/docs/laceworksdk/api/v2/activities.html
--rw-r--r--   0 runner    (1001) docker     (123)    88036 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/docs/laceworksdk/api/v2/agent_access_tokens.html
--rw-r--r--   0 runner    (1001) docker     (123)    45275 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/docs/laceworksdk/api/v2/agent_info.html
--rw-r--r--   0 runner    (1001) docker     (123)   124179 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/docs/laceworksdk/api/v2/alert_channels.html
--rw-r--r--   0 runner    (1001) docker     (123)   105645 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/docs/laceworksdk/api/v2/alert_profiles.html
--rw-r--r--   0 runner    (1001) docker     (123)   111767 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/docs/laceworksdk/api/v2/alert_rules.html
--rw-r--r--   0 runner    (1001) docker     (123)   111526 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/docs/laceworksdk/api/v2/alerts.html
--rw-r--r--   0 runner    (1001) docker     (123)    69549 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/docs/laceworksdk/api/v2/audit_logs.html
--rw-r--r--   0 runner    (1001) docker     (123)   114369 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/docs/laceworksdk/api/v2/cloud_accounts.html
--rw-r--r--   0 runner    (1001) docker     (123)    93253 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/docs/laceworksdk/api/v2/cloud_activities.html
--rw-r--r--   0 runner    (1001) docker     (123)    54447 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/docs/laceworksdk/api/v2/configs.html
--rw-r--r--   0 runner    (1001) docker     (123)   117797 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/docs/laceworksdk/api/v2/container_registries.html
--rw-r--r--   0 runner    (1001) docker     (123)    56268 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/docs/laceworksdk/api/v2/contract_info.html
--rw-r--r--   0 runner    (1001) docker     (123)    83847 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/docs/laceworksdk/api/v2/datasources.html
--rw-r--r--   0 runner    (1001) docker     (123)   157901 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/docs/laceworksdk/api/v2/entities.html
--rw-r--r--   0 runner    (1001) docker     (123)    48918 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/docs/laceworksdk/api/v2/events.html
--rw-r--r--   0 runner    (1001) docker     (123)    45271 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/docs/laceworksdk/api/v2/inventory.html
--rw-r--r--   0 runner    (1001) docker     (123)    52235 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/docs/laceworksdk/api/v2/organization_info.html
--rw-r--r--   0 runner    (1001) docker     (123)   138017 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/docs/laceworksdk/api/v2/policies.html
--rw-r--r--   0 runner    (1001) docker     (123)   117811 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/docs/laceworksdk/api/v2/policy_exceptions.html
--rw-r--r--   0 runner    (1001) docker     (123)   149560 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/docs/laceworksdk/api/v2/queries.html
--rw-r--r--   0 runner    (1001) docker     (123)   152668 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/docs/laceworksdk/api/v2/report_definitions.html
--rw-r--r--   0 runner    (1001) docker     (123)   113510 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/docs/laceworksdk/api/v2/report_rules.html
--rw-r--r--   0 runner    (1001) docker     (123)    75546 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/docs/laceworksdk/api/v2/reports.html
--rw-r--r--   0 runner    (1001) docker     (123)   106359 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/docs/laceworksdk/api/v2/resource_groups.html
--rw-r--r--   0 runner    (1001) docker     (123)    62352 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/docs/laceworksdk/api/v2/schemas.html
--rw-r--r--   0 runner    (1001) docker     (123)   128744 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/docs/laceworksdk/api/v2/team_members.html
--rw-r--r--   0 runner    (1001) docker     (123)    51575 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/docs/laceworksdk/api/v2/user_profile.html
--rw-r--r--   0 runner    (1001) docker     (123)   127287 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/docs/laceworksdk/api/v2/vulnerabilities.html
--rw-r--r--   0 runner    (1001) docker     (123)   152461 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/docs/laceworksdk/api/v2/vulnerability_exceptions.html
--rw-r--r--   0 runner    (1001) docker     (123)   157633 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/docs/laceworksdk/api/v2/vulnerability_policies.html
--rw-r--r--   0 runner    (1001) docker     (123)    36709 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/docs/laceworksdk/api/v2.html
--rw-r--r--   0 runner    (1001) docker     (123)   161081 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/docs/laceworksdk/api.html
--rw-r--r--   0 runner    (1001) docker     (123)    38099 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/docs/laceworksdk/config.html
--rw-r--r--   0 runner    (1001) docker     (123)    87244 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/docs/laceworksdk/exceptions.html
--rw-r--r--   0 runner    (1001) docker     (123)   254613 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/docs/laceworksdk/http_session.html
--rw-r--r--   0 runner    (1001) docker     (123)    35610 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/docs/laceworksdk/version.html
--rw-r--r--   0 runner    (1001) docker     (123)    36866 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/docs/laceworksdk.html
--rw-r--r--   0 runner    (1001) docker     (123)  1347054 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/docs/search.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 19:19:32.418793 laceworksdk-1.9.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/examples/example_active_container_vulnerabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/examples/example_alert_channels.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/examples/example_alerts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/examples/example_audit_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/examples/example_cloud_accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/examples/example_cloud_activities.py
--rw-r--r--   0 runner    (1001) docker     (123)    10873 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/examples/example_export.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/examples/example_inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/examples/example_query_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/examples/example_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/examples/example_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/examples/example_syscall_query_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/examples/example_tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/examples/example_vulnerabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 19:19:32.418793 laceworksdk-1.9.0/jupyter/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/jupyter/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/jupyter/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 19:19:32.418793 laceworksdk-1.9.0/jupyter/devtools/
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/jupyter/devtools/deploy_to_container.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 19:19:32.418793 laceworksdk-1.9.0/jupyter/docker/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/jupyter/docker/docker-build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/jupyter/docker/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 19:19:32.418793 laceworksdk-1.9.0/jupyter/docker/docker_build/
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/jupyter/docker/docker_build/00-import.py
--rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/jupyter/docker/docker_build/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/jupyter/docker/docker_build/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/jupyter/docker/docker_build/jupyter_notebook_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 19:19:32.418793 laceworksdk-1.9.0/jupyter/docker/docker_build/lacework/
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/jupyter/docker/docker_build/lacework/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/jupyter/docker/docker_build/lacework/lacework.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/jupyter/docker/docker_build/lacework/main.js
--rw-r--r--   0 runner    (1001) docker     (123)    74260 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/jupyter/docker/docker_build/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/jupyter/docker/docker_build/snippets.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 19:19:32.418793 laceworksdk-1.9.0/jupyter/laceworkjupyter/
--rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/jupyter/laceworkjupyter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/jupyter/laceworkjupyter/accessors.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/jupyter/laceworkjupyter/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/jupyter/laceworkjupyter/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 19:19:32.422793 laceworksdk-1.9.0/jupyter/laceworkjupyter/features/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/jupyter/laceworkjupyter/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/jupyter/laceworkjupyter/features/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/jupyter/laceworkjupyter/features/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/jupyter/laceworkjupyter/features/date.py
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/jupyter/laceworkjupyter/features/filters.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/jupyter/laceworkjupyter/features/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8578 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/jupyter/laceworkjupyter/features/hunt.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/jupyter/laceworkjupyter/features/join.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13191 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/jupyter/laceworkjupyter/features/mitre.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/jupyter/laceworkjupyter/features/mitre.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/jupyter/laceworkjupyter/features/policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/jupyter/laceworkjupyter/features/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/jupyter/laceworkjupyter/features/query.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13555 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/jupyter/laceworkjupyter/features/query_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/jupyter/laceworkjupyter/features/tables.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9429 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/jupyter/laceworkjupyter/features/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/jupyter/laceworkjupyter/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/jupyter/laceworkjupyter/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 19:19:32.422793 laceworksdk-1.9.0/jupyter/laceworkjupyter/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/jupyter/laceworkjupyter/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/jupyter/laceworkjupyter/plugins/alert_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/jupyter/laceworkjupyter/plugins/alerts.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/jupyter/laceworkjupyter/plugins/datasources.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/jupyter/laceworkjupyter/plugins/events.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/jupyter/laceworkjupyter/plugins/evidence.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/jupyter/laceworkjupyter/plugins/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5739 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/jupyter/laceworkjupyter/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/jupyter/laceworkjupyter/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 19:19:32.422793 laceworksdk-1.9.0/jupyter/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)    22963 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/jupyter/notebooks/colab_sample.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    16315 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/jupyter/notebooks/sample_notebook.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/jupyter/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/jupyter/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/jupyter/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 19:19:32.422793 laceworksdk-1.9.0/jupyter/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/jupyter/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 19:19:32.422793 laceworksdk-1.9.0/jupyter/tests/laceworkjupyter/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/jupyter/tests/laceworkjupyter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/jupyter/tests/laceworkjupyter/test_accessors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/jupyter/tests/laceworkjupyter/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 19:19:32.422793 laceworksdk-1.9.0/laceworksdk/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/laceworksdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 19:19:32.422793 laceworksdk-1.9.0/laceworksdk/api/
--rw-r--r--   0 runner    (1001) docker     (123)     8303 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/laceworksdk/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/laceworksdk/api/base_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/laceworksdk/api/crud_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/laceworksdk/api/read_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/laceworksdk/api/search_endpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 19:19:32.426793 laceworksdk-1.9.0/laceworksdk/api/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/laceworksdk/api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/laceworksdk/api/v1/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     6630 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/laceworksdk/api/v1/compliance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/laceworksdk/api/v1/custom_compliance_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/laceworksdk/api/v1/download_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/laceworksdk/api/v1/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     7231 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/laceworksdk/api/v1/integrations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/laceworksdk/api/v1/recommendations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/laceworksdk/api/v1/run_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/laceworksdk/api/v1/suppressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/laceworksdk/api/v1/token.py
--rw-r--r--   0 runner    (1001) docker     (123)    12315 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/laceworksdk/api/v1/vulnerability.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 19:19:32.426793 laceworksdk-1.9.0/laceworksdk/api/v2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/laceworksdk/api/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/laceworksdk/api/v2/activities.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/laceworksdk/api/v2/agent_access_tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/laceworksdk/api/v2/agent_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/laceworksdk/api/v2/alert_channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/laceworksdk/api/v2/alert_profiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/laceworksdk/api/v2/alert_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/laceworksdk/api/v2/alerts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/laceworksdk/api/v2/audit_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/laceworksdk/api/v2/cloud_accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/laceworksdk/api/v2/cloud_activities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/laceworksdk/api/v2/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/laceworksdk/api/v2/container_registries.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/laceworksdk/api/v2/contract_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/laceworksdk/api/v2/datasources.py
--rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/laceworksdk/api/v2/entities.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/laceworksdk/api/v2/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/laceworksdk/api/v2/inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/laceworksdk/api/v2/organization_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/laceworksdk/api/v2/policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/laceworksdk/api/v2/policy_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/laceworksdk/api/v2/queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     7183 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/laceworksdk/api/v2/report_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/laceworksdk/api/v2/report_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/laceworksdk/api/v2/reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/laceworksdk/api/v2/resource_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/laceworksdk/api/v2/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/laceworksdk/api/v2/team_members.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/laceworksdk/api/v2/user_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     4921 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/laceworksdk/api/v2/vulnerabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     7086 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/laceworksdk/api/v2/vulnerability_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7094 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/laceworksdk/api/v2/vulnerability_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/laceworksdk/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/laceworksdk/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    14361 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/laceworksdk/http_session.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-02-24 19:19:32.000000 laceworksdk-1.9.0/laceworksdk/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 19:19:32.422793 laceworksdk-1.9.0/laceworksdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5167 2023-02-24 19:19:32.000000 laceworksdk-1.9.0/laceworksdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8867 2023-02-24 19:19:32.000000 laceworksdk-1.9.0/laceworksdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 19:19:32.000000 laceworksdk-1.9.0/laceworksdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-02-24 19:19:32.000000 laceworksdk-1.9.0/laceworksdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-24 19:19:32.000000 laceworksdk-1.9.0/laceworksdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-02-24 19:19:32.434793 laceworksdk-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 19:19:32.426793 laceworksdk-1.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 19:19:32.430793 laceworksdk-1.9.0/tests/api/
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/tests/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/tests/api/test_base_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/tests/api/test_crud_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/tests/api/test_laceworksdk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/tests/api/test_read_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/tests/api/test_search_endpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 19:19:32.430793 laceworksdk-1.9.0/tests/api/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/tests/api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/tests/api/v1/test_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/tests/api/v1/test_compliance.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/tests/api/v1/test_custom_compliance_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/tests/api/v1/test_download_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/tests/api/v1/test_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/tests/api/v1/test_integrations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/tests/api/v1/test_recommendations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/tests/api/v1/test_run_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/tests/api/v1/test_suppressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/tests/api/v1/test_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/tests/api/v1/test_vulnerability.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 19:19:32.434793 laceworksdk-1.9.0/tests/api/v2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/tests/api/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/tests/api/v2/test_activities.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/tests/api/v2/test_agent_access_tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/tests/api/v2/test_agent_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/tests/api/v2/test_alert_channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/tests/api/v2/test_alert_profiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/tests/api/v2/test_alert_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/tests/api/v2/test_alerts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/tests/api/v2/test_audit_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/tests/api/v2/test_cloud_accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/tests/api/v2/test_cloud_activities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/tests/api/v2/test_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/tests/api/v2/test_container_registries.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/tests/api/v2/test_contract_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/tests/api/v2/test_datasources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/tests/api/v2/test_entities.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/tests/api/v2/test_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/tests/api/v2/test_inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/tests/api/v2/test_organization_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/tests/api/v2/test_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/tests/api/v2/test_policy_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/tests/api/v2/test_queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/tests/api/v2/test_report_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/tests/api/v2/test_report_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/tests/api/v2/test_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/tests/api/v2/test_resource_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/tests/api/v2/test_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/tests/api/v2/test_team_members.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/tests/api/v2/test_user_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/tests/api/v2/test_vulnerabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/tests/api/v2/test_vulnerability_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/tests/api/v2/test_vulnerability_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/tests/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-02-24 19:19:20.000000 laceworksdk-1.9.0/tests/test_laceworksdk.py
+-rw-r--r--   0        0        0     1071 2023-06-29 09:44:02.591009 laceworksdk-2.0.0/LICENSE
+-rw-r--r--   0        0        0     3956 2023-06-29 09:44:02.591009 laceworksdk-2.0.0/README.md
+-rw-r--r--   0        0        0      412 2023-06-29 09:44:02.611009 laceworksdk-2.0.0/laceworksdk/__init__.py
+-rw-r--r--   0        0        0     7572 2023-06-29 09:44:02.611009 laceworksdk-2.0.0/laceworksdk/api/__init__.py
+-rw-r--r--   0        0        0     4288 2023-06-29 09:44:02.611009 laceworksdk-2.0.0/laceworksdk/api/base_endpoint.py
+-rw-r--r--   0        0        0     3110 2023-06-29 09:44:02.611009 laceworksdk-2.0.0/laceworksdk/api/crud_endpoint.py
+-rw-r--r--   0        0        0     1330 2023-06-29 09:44:02.611009 laceworksdk-2.0.0/laceworksdk/api/read_endpoint.py
+-rw-r--r--   0        0        0     1612 2023-06-29 09:44:02.611009 laceworksdk-2.0.0/laceworksdk/api/search_endpoint.py
+-rw-r--r--   0        0        0        0 2023-06-29 09:44:02.611009 laceworksdk-2.0.0/laceworksdk/api/v2/__init__.py
+-rw-r--r--   0        0        0     2000 2023-06-29 09:44:02.611009 laceworksdk-2.0.0/laceworksdk/api/v2/activities.py
+-rw-r--r--   0        0        0     2402 2023-06-29 09:44:02.611009 laceworksdk-2.0.0/laceworksdk/api/v2/agent_access_tokens.py
+-rw-r--r--   0        0        0      414 2023-06-29 09:44:02.611009 laceworksdk-2.0.0/laceworksdk/api/v2/agent_info.py
+-rw-r--r--   0        0        0     3834 2023-06-29 09:44:02.611009 laceworksdk-2.0.0/laceworksdk/api/v2/alert_channels.py
+-rw-r--r--   0        0        0     3551 2023-06-29 09:44:02.611009 laceworksdk-2.0.0/laceworksdk/api/v2/alert_profiles.py
+-rw-r--r--   0        0        0     4325 2023-06-29 09:44:02.615008 laceworksdk-2.0.0/laceworksdk/api/v2/alert_rules.py
+-rw-r--r--   0        0        0     4538 2023-06-29 09:44:02.615008 laceworksdk-2.0.0/laceworksdk/api/v2/alerts.py
+-rw-r--r--   0        0        0     1558 2023-06-29 09:44:02.615008 laceworksdk-2.0.0/laceworksdk/api/v2/audit_logs.py
+-rw-r--r--   0        0        0     3484 2023-06-29 09:44:02.615008 laceworksdk-2.0.0/laceworksdk/api/v2/cloud_accounts.py
+-rw-r--r--   0        0        0     2566 2023-06-29 09:44:02.615008 laceworksdk-2.0.0/laceworksdk/api/v2/cloud_activities.py
+-rw-r--r--   0        0        0     1821 2023-06-29 09:44:02.615008 laceworksdk-2.0.0/laceworksdk/api/v2/configs.py
+-rw-r--r--   0        0        0     3549 2023-06-29 09:44:02.615008 laceworksdk-2.0.0/laceworksdk/api/v2/container_registries.py
+-rw-r--r--   0        0        0      900 2023-06-29 09:44:02.615008 laceworksdk-2.0.0/laceworksdk/api/v2/contract_info.py
+-rw-r--r--   0        0        0     2029 2023-06-29 09:44:02.615008 laceworksdk-2.0.0/laceworksdk/api/v2/datasources.py
+-rw-r--r--   0        0        0     5539 2023-06-29 09:44:02.615008 laceworksdk-2.0.0/laceworksdk/api/v2/entities.py
+-rw-r--r--   0        0        0     2861 2023-06-29 09:44:02.615008 laceworksdk-2.0.0/laceworksdk/api/v2/events.py
+-rw-r--r--   0        0        0     1516 2023-06-29 09:44:02.615008 laceworksdk-2.0.0/laceworksdk/api/v2/inventory.py
+-rw-r--r--   0        0        0      654 2023-06-29 09:44:02.615008 laceworksdk-2.0.0/laceworksdk/api/v2/organization_info.py
+-rw-r--r--   0        0        0     7228 2023-06-29 09:44:02.615008 laceworksdk-2.0.0/laceworksdk/api/v2/policies.py
+-rw-r--r--   0        0        0     4127 2023-06-29 09:44:02.615008 laceworksdk-2.0.0/laceworksdk/api/v2/policy_exceptions.py
+-rw-r--r--   0        0        0     5446 2023-06-29 09:44:02.615008 laceworksdk-2.0.0/laceworksdk/api/v2/queries.py
+-rw-r--r--   0        0        0     7183 2023-06-29 09:44:02.615008 laceworksdk-2.0.0/laceworksdk/api/v2/report_definitions.py
+-rw-r--r--   0        0        0     4383 2023-06-29 09:44:02.615008 laceworksdk-2.0.0/laceworksdk/api/v2/report_rules.py
+-rw-r--r--   0        0        0     2250 2023-06-29 09:44:02.615008 laceworksdk-2.0.0/laceworksdk/api/v2/reports.py
+-rw-r--r--   0        0        0     3286 2023-06-29 09:44:02.615008 laceworksdk-2.0.0/laceworksdk/api/v2/resource_groups.py
+-rw-r--r--   0        0        0     1092 2023-06-29 09:44:02.615008 laceworksdk-2.0.0/laceworksdk/api/v2/schemas.py
+-rw-r--r--   0        0        0     5376 2023-06-29 09:44:02.615008 laceworksdk-2.0.0/laceworksdk/api/v2/team_members.py
+-rw-r--r--   0        0        0     3185 2023-06-29 09:44:02.615008 laceworksdk-2.0.0/laceworksdk/api/v2/team_users.py
+-rw-r--r--   0        0        0     1378 2023-06-29 09:44:02.615008 laceworksdk-2.0.0/laceworksdk/api/v2/user_groups.py
+-rw-r--r--   0        0        0      624 2023-06-29 09:44:02.615008 laceworksdk-2.0.0/laceworksdk/api/v2/user_profile.py
+-rw-r--r--   0        0        0     4834 2023-06-29 09:44:02.615008 laceworksdk-2.0.0/laceworksdk/api/v2/vulnerabilities.py
+-rw-r--r--   0        0        0     7086 2023-06-29 09:44:02.615008 laceworksdk-2.0.0/laceworksdk/api/v2/vulnerability_exceptions.py
+-rw-r--r--   0        0        0     7094 2023-06-29 09:44:02.615008 laceworksdk-2.0.0/laceworksdk/api/v2/vulnerability_policies.py
+-rw-r--r--   0        0        0      696 2023-06-29 09:44:02.615008 laceworksdk-2.0.0/laceworksdk/config.py
+-rw-r--r--   0        0        0     2498 2023-06-29 09:44:02.615008 laceworksdk-2.0.0/laceworksdk/exceptions.py
+-rw-r--r--   0        0        0    14468 2023-06-29 09:44:02.615008 laceworksdk-2.0.0/laceworksdk/http_session.py
+-rw-r--r--   0        0        0     1576 2023-06-29 09:44:02.615008 laceworksdk-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     5238 1970-01-01 00:00:00.000000 laceworksdk-2.0.0/PKG-INFO
```

### Comparing `laceworksdk-1.9.0/LICENSE` & `laceworksdk-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `laceworksdk-1.9.0/PKG-INFO` & `laceworksdk-2.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,38 @@
 Metadata-Version: 2.1
 Name: laceworksdk
-Version: 1.9.0
+Version: 2.0.0
 Summary: Community-developed Python SDK for the Lacework APIs
 Home-page: https://github.com/lacework/python-sdk
-Download-URL: https://pypi.python.org/pypi/laceworksdk
-Author: Alan Nix
-Author-email: alan.nix@lacework.net
 License: MIT
-Keywords: lacework,api,sdk,python,api
+Keywords: lacework,api,sdk,python
+Author: Jon Stewart
+Author-email: jon.stewart@lacework.net
+Maintainer: Jon Stewart
+Maintainer-email: jon.stewart@lacework.net
+Requires-Python: >=3.7.16,<4.0.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Topic :: Software Development :: Build Tools
+Requires-Dist: bleach (>=4.1.0,<5.0.0)
+Requires-Dist: configparser (>=5.2.0,<6.0.0)
+Requires-Dist: importlib-metadata (==4.2)
+Requires-Dist: python-dotenv (>=0.20.0,<0.21.0)
+Requires-Dist: requests (>=2.27.1,<3.0.0)
+Requires-Dist: urllib3 (>=1.26.15,<2.0.0)
+Project-URL: Repository, https://github.com/lacework/python-sdk
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 <img src="https://techally-content.s3-us-west-1.amazonaws.com/public-content/lacework_logo_full.png" width="600">
 
 # Lacework Python SDK
 
 ![Build Status](https://github.com/lacework/python-sdk/actions/workflows/python-test.yml/badge.svg)
 [![Downloads](https://pepy.tech/badge/laceworksdk)](https://pepy.tech/project/laceworksdk)
@@ -41,15 +50,20 @@
 
 lw = LaceworkClient() # This would leverage your default Lacework CLI profile.
 lw = LaceworkClient(account="ACCOUNT",
                     subaccount="SUBACCOUNT",
                     api_key="API KEY",
                     api_secret="API SECRET")
 
-events = lw.events.get_for_date_range(start_time=start_time, end_time=end_time)
+events = lw.events.search(json={
+  "timeFilter": {
+    "startTime": start_time,
+    "endTime": end_time
+  }
+})
 
 host_vulns = lw.vulnerabilities.hosts.search(json={
     "timeFilter": {
         "startTime": start_time,
         "endTime": end_time
     }
 })
@@ -118,18 +132,9 @@
 
 `$ pip install laceworksdk --upgrade`
 
 ## Examples
 
 Are you looking for some sample scripts? Check out the [examples](examples/) folder!
 
-### Contributing
+### [Contributing](CONTRIBUTING.md)
 
-To install/configure the necessary requirements for contributing to this project, simply create a virtual environment, install `requirements.txt` and `requirements-dev.txt`, and set up a version file using the commands below:
-
-```sh
-python3 -m venv venv
-source venv/bin/activate
-pip install -r requirements.txt
-pip install -r requirements-dev.txt
-python setup.py --version
-```
```

### Comparing `laceworksdk-1.9.0/README.md` & `laceworksdk-2.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,20 @@
 
 lw = LaceworkClient() # This would leverage your default Lacework CLI profile.
 lw = LaceworkClient(account="ACCOUNT",
                     subaccount="SUBACCOUNT",
                     api_key="API KEY",
                     api_secret="API SECRET")
 
-events = lw.events.get_for_date_range(start_time=start_time, end_time=end_time)
+events = lw.events.search(json={
+  "timeFilter": {
+    "startTime": start_time,
+    "endTime": end_time
+  }
+})
 
 host_vulns = lw.vulnerabilities.hosts.search(json={
     "timeFilter": {
         "startTime": start_time,
         "endTime": end_time
     }
 })
@@ -95,18 +100,8 @@
 
 `$ pip install laceworksdk --upgrade`
 
 ## Examples
 
 Are you looking for some sample scripts? Check out the [examples](examples/) folder!
 
-### Contributing
-
-To install/configure the necessary requirements for contributing to this project, simply create a virtual environment, install `requirements.txt` and `requirements-dev.txt`, and set up a version file using the commands below:
-
-```sh
-python3 -m venv venv
-source venv/bin/activate
-pip install -r requirements.txt
-pip install -r requirements-dev.txt
-python setup.py --version
-```
+### [Contributing](CONTRIBUTING.md)
```

### Comparing `laceworksdk-1.9.0/laceworksdk/api/__init__.py` & `laceworksdk-2.0.0/laceworksdk/api/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,24 +6,14 @@
 import os
 
 from dotenv import load_dotenv
 import configparser
 
 from laceworksdk.http_session import HttpSession
 
-from .v1.account import AccountAPI
-from .v1.compliance import ComplianceAPI
-from .v1.custom_compliance_config import CustomComplianceConfigAPI
-from .v1.download_file import DownloadFileAPI
-from .v1.integrations import IntegrationsAPI
-from .v1.recommendations import RecommendationsAPI
-from .v1.run_reports import RunReportsAPI
-from .v1.suppressions import SuppressionsAPI
-from .v1.token import TokenAPI
-
 from .v2.activities import ActivitiesAPI
 from .v2.agent_access_tokens import AgentAccessTokensAPI
 from .v2.agent_info import AgentInfoAPI
 from .v2.alert_channels import AlertChannelsAPI
 from .v2.alert_profiles import AlertProfilesAPI
 from .v2.alert_rules import AlertRulesAPI
 from .v2.alerts import AlertsAPI
@@ -31,26 +21,28 @@
 from .v2.cloud_accounts import CloudAccountsAPI
 from .v2.cloud_activities import CloudActivitiesAPI
 from .v2.configs import ConfigsAPI
 from .v2.container_registries import ContainerRegistriesAPI
 from .v2.contract_info import ContractInfoAPI
 from .v2.datasources import DatasourcesAPI
 from .v2.entities import EntitiesAPI
-from .v2.events import EventsAPIv2
+from .v2.events import EventsAPI
 from .v2.inventory import InventoryAPI
 from .v2.organization_info import OrganizationInfoAPI
 from .v2.policies import PoliciesAPI
 from .v2.policy_exceptions import PolicyExceptionsAPI
 from .v2.queries import QueriesAPI
 from .v2.report_definitions import ReportDefinitionsAPI
 from .v2.report_rules import ReportRulesAPI
 from .v2.reports import ReportsAPI
 from .v2.resource_groups import ResourceGroupsAPI
 from .v2.schemas import SchemasAPI
 from .v2.team_members import TeamMembersAPI
+from .v2.team_users import TeamUsersAPI
+from .v2.user_groups import UserGroupsAPI
 from .v2.user_profile import UserProfileAPI
 from .v2.vulnerabilities import VulnerabilitiesAPI
 from .v2.vulnerability_exceptions import VulnerabilityExceptionsAPI
 from .v2.vulnerability_policies import VulnerabilityPoliciesAPI
 
 from laceworksdk.config import (
     DEFAULT_BASE_DOMAIN,
@@ -139,50 +131,43 @@
             self._subaccount,
             self._api_key,
             self._api_secret,
             self._base_domain
         )
 
         # API Wrappers
-        self.account = AccountAPI(self._session)
         self.activities = ActivitiesAPI(self._session)
         self.agent_access_tokens = AgentAccessTokensAPI(self._session)
         self.agent_info = AgentInfoAPI(self._session)
         self.alert_channels = AlertChannelsAPI(self._session)
         self.alert_profiles = AlertProfilesAPI(self._session)
         self.alert_rules = AlertRulesAPI(self._session)
         self.alerts = AlertsAPI(self._session)
         self.audit_logs = AuditLogsAPI(self._session)
         self.cloud_accounts = CloudAccountsAPI(self._session)
         self.cloud_activities = CloudActivitiesAPI(self._session)
-        self.compliance = ComplianceAPI(self._session)
-        self.compliance.config = CustomComplianceConfigAPI(self._session)
         self.configs = ConfigsAPI(self._session)
         self.container_registries = ContainerRegistriesAPI(self._session)
         self.contract_info = ContractInfoAPI(self._session)
         self.datasources = DatasourcesAPI(self._session)
         self.entities = EntitiesAPI(self._session)
-        self.events = EventsAPIv2(self._session)
-        self.files = DownloadFileAPI(self._session)
+        self.events = EventsAPI(self._session)
         self.inventory = InventoryAPI(self._session)
-        self.integrations = IntegrationsAPI(self._session)
         self.organization_info = OrganizationInfoAPI(self._session)
         self.policies = PoliciesAPI(self._session)
         self.policy_exceptions = PolicyExceptionsAPI(self._session)
         self.queries = QueriesAPI(self._session)
-        self.recommendations = RecommendationsAPI(self._session)
         self.report_definitions = ReportDefinitionsAPI(self._session)
         self.report_rules = ReportRulesAPI(self._session)
         self.reports = ReportsAPI(self._session)
         self.resource_groups = ResourceGroupsAPI(self._session)
-        self.run_reports = RunReportsAPI(self._session)
         self.schemas = SchemasAPI(self._session)
-        self.suppressions = SuppressionsAPI(self._session)
         self.team_members = TeamMembersAPI(self._session)
-        self.tokens = TokenAPI(self._session)
+        self.team_users = TeamUsersAPI(self._session)
+        self.user_groups = UserGroupsAPI(self._session)
         self.user_profile = UserProfileAPI(self._session)
         self.vulnerabilities = VulnerabilitiesAPI(self._session)
         self.vulnerability_exceptions = VulnerabilityExceptionsAPI(self._session)
         self.vulnerability_policies = VulnerabilityPoliciesAPI(self._session)
 
     @property
     def subaccount(self):
```

### Comparing `laceworksdk-1.9.0/laceworksdk/api/base_endpoint.py` & `laceworksdk-2.0.0/laceworksdk/api/base_endpoint.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-1.9.0/laceworksdk/api/crud_endpoint.py` & `laceworksdk-2.0.0/laceworksdk/api/crud_endpoint.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-1.9.0/laceworksdk/api/read_endpoint.py` & `laceworksdk-2.0.0/laceworksdk/api/read_endpoint.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-1.9.0/laceworksdk/api/search_endpoint.py` & `laceworksdk-2.0.0/laceworksdk/api/search_endpoint.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-1.9.0/laceworksdk/api/v2/activities.py` & `laceworksdk-2.0.0/laceworksdk/api/v2/activities.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-1.9.0/laceworksdk/api/v2/agent_access_tokens.py` & `laceworksdk-2.0.0/laceworksdk/api/v2/agent_access_tokens.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-1.9.0/laceworksdk/api/v2/alert_channels.py` & `laceworksdk-2.0.0/laceworksdk/api/v2/alert_channels.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-1.9.0/laceworksdk/api/v2/alert_profiles.py` & `laceworksdk-2.0.0/laceworksdk/api/v2/alert_profiles.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-1.9.0/laceworksdk/api/v2/alert_rules.py` & `laceworksdk-2.0.0/laceworksdk/api/v2/alert_rules.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-1.9.0/laceworksdk/api/v2/alerts.py` & `laceworksdk-2.0.0/laceworksdk/api/v2/alerts.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-1.9.0/laceworksdk/api/v2/audit_logs.py` & `laceworksdk-2.0.0/laceworksdk/api/v2/audit_logs.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-1.9.0/laceworksdk/api/v2/cloud_accounts.py` & `laceworksdk-2.0.0/laceworksdk/api/v2/cloud_accounts.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-1.9.0/laceworksdk/api/v2/cloud_activities.py` & `laceworksdk-2.0.0/laceworksdk/api/v2/cloud_activities.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-1.9.0/laceworksdk/api/v2/configs.py` & `laceworksdk-2.0.0/laceworksdk/api/v2/configs.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-1.9.0/laceworksdk/api/v2/container_registries.py` & `laceworksdk-2.0.0/laceworksdk/api/v2/container_registries.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-1.9.0/laceworksdk/api/v2/contract_info.py` & `laceworksdk-2.0.0/laceworksdk/api/v2/contract_info.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-1.9.0/laceworksdk/api/v2/datasources.py` & `laceworksdk-2.0.0/laceworksdk/api/v2/datasources.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-1.9.0/laceworksdk/api/v2/entities.py` & `laceworksdk-2.0.0/laceworksdk/api/v2/entities.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-1.9.0/laceworksdk/api/v2/inventory.py` & `laceworksdk-2.0.0/laceworksdk/api/v2/inventory.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-1.9.0/laceworksdk/api/v2/organization_info.py` & `laceworksdk-2.0.0/laceworksdk/api/v2/organization_info.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-1.9.0/laceworksdk/api/v2/policies.py` & `laceworksdk-2.0.0/laceworksdk/api/v2/policies.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-1.9.0/laceworksdk/api/v2/policy_exceptions.py` & `laceworksdk-2.0.0/laceworksdk/api/v2/policy_exceptions.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-1.9.0/laceworksdk/api/v2/queries.py` & `laceworksdk-2.0.0/laceworksdk/api/v2/queries.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-1.9.0/laceworksdk/api/v2/report_definitions.py` & `laceworksdk-2.0.0/laceworksdk/api/v2/report_definitions.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-1.9.0/laceworksdk/api/v2/report_rules.py` & `laceworksdk-2.0.0/laceworksdk/api/v2/report_rules.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-1.9.0/laceworksdk/api/v2/reports.py` & `laceworksdk-2.0.0/laceworksdk/api/v2/reports.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-1.9.0/laceworksdk/api/v2/resource_groups.py` & `laceworksdk-2.0.0/laceworksdk/api/v2/resource_groups.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-1.9.0/laceworksdk/api/v2/schemas.py` & `laceworksdk-2.0.0/laceworksdk/api/v2/schemas.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-1.9.0/laceworksdk/api/v2/team_members.py` & `laceworksdk-2.0.0/laceworksdk/api/v2/team_members.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-1.9.0/laceworksdk/api/v2/user_profile.py` & `laceworksdk-2.0.0/laceworksdk/api/v2/user_profile.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-1.9.0/laceworksdk/api/v2/vulnerabilities.py` & `laceworksdk-2.0.0/laceworksdk/api/v2/vulnerabilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 # -*- coding: utf-8 -*-
 """
 Lacework Vulnerabilities API wrapper.
 """
 
 from laceworksdk.api.base_endpoint import BaseEndpoint
 from laceworksdk.api.search_endpoint import SearchEndpoint
-from laceworksdk.api.v1.vulnerability import VulnerabilityAPI
 
 
-class VulnerabilitiesAPI(VulnerabilityAPI):
+class VulnerabilitiesAPI:
     """A class used to represent the Vulnerabilities API endpoint.
 
     The Vulnerabilities API endpoint is simply a parent for different types of
     vulnerabilities that can be queried.  Due to namespace overlap with the v1
     API, this class is a subclass of VulnerabilityAPI to expose those methods
     and provide backwards compatibility.
 
@@ -30,16 +29,16 @@
         """
         Initializes the VulnerabilitiesAPI object.
 
         :param session: An instance of the HttpSession class
 
         :return VulnerabilitiesAPI object.
         """
+        super().__init__()
 
-        super().__init__(session)
         self._base_path = "Vulnerabilities"
 
         self.containers = ContainerVulnerabilitiesAPI(session, self._base_path)
         self.hosts = HostVulnerabilitiesAPI(session, self._base_path)
         self.packages = SoftwarePackagesAPI(session, self._base_path)
```

### Comparing `laceworksdk-1.9.0/laceworksdk/api/v2/vulnerability_exceptions.py` & `laceworksdk-2.0.0/laceworksdk/api/v2/vulnerability_exceptions.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-1.9.0/laceworksdk/api/v2/vulnerability_policies.py` & `laceworksdk-2.0.0/laceworksdk/api/v2/vulnerability_policies.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-1.9.0/laceworksdk/config.py` & `laceworksdk-2.0.0/laceworksdk/config.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-1.9.0/laceworksdk/exceptions.py` & `laceworksdk-2.0.0/laceworksdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-1.9.0/laceworksdk/http_session.py` & `laceworksdk-2.0.0/laceworksdk/http_session.py`

 * *Files 6% similar despite different names*

```diff
@@ -222,16 +222,19 @@
             domain_end = domain_begin + len(self._base_domain)
             uri = uri[domain_end:]
 
         uri = f"{self._base_url}{uri}"
 
         logger.info(f"{method} request to URI: {uri}")
 
-        if "/api/v1/" in uri:
-            logger.warning("Lacework's v1 APIs are scheduled to be deprecated and will not allow usage of after December 2022.")
+        if "/api/v2/TeamUsers" in uri:
+            logger.warning("TeamUsers APIs is currently experimental and subject to change")
+
+        if "/api/v2/UserGroups" in uri:
+            logger.warning("UserGroups API is currently experimental and subject to change")
 
         # Check for 'org' - if True, make an organization-level API call
         # TODO: Remove this on v1.0 release - this is done for back compat
         org = kwargs.pop("org", None)
         headers = self._get_request_headers(org_access=org)
 
         # Check for 'data' or 'json'
```

