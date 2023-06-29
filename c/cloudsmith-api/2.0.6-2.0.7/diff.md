# Comparing `tmp/cloudsmith_api-2.0.6-py2.py3-none-any.whl.zip` & `tmp/cloudsmith_api-2.0.7-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,417 +1,485 @@
-Zip file size: 734820 bytes, number of entries: 415
--rw-r--r--  2.0 unx    16073 b- defN 23-Jun-02 14:23 cloudsmith_api/__init__.py
--rw-r--r--  2.0 unx    25067 b- defN 23-Jun-02 14:23 cloudsmith_api/api_client.py
--rw-r--r--  2.0 unx     8390 b- defN 23-Jun-02 14:23 cloudsmith_api/configuration.py
--rw-r--r--  2.0 unx    13166 b- defN 23-Jun-02 14:23 cloudsmith_api/rest.py
--rw-r--r--  2.0 unx     1131 b- defN 23-Jun-02 14:23 cloudsmith_api/api/__init__.py
--rw-r--r--  2.0 unx    11039 b- defN 23-Jun-02 14:23 cloudsmith_api/api/audit_log_api.py
--rw-r--r--  2.0 unx    11425 b- defN 23-Jun-02 14:23 cloudsmith_api/api/badges_api.py
--rw-r--r--  2.0 unx     7978 b- defN 23-Jun-02 14:23 cloudsmith_api/api/distros_api.py
--rw-r--r--  2.0 unx    54786 b- defN 23-Jun-02 14:23 cloudsmith_api/api/entitlements_api.py
--rw-r--r--  2.0 unx    26620 b- defN 23-Jun-02 14:23 cloudsmith_api/api/files_api.py
--rw-r--r--  2.0 unx     7930 b- defN 23-Jun-02 14:23 cloudsmith_api/api/formats_api.py
--rw-r--r--  2.0 unx    19214 b- defN 23-Jun-02 14:23 cloudsmith_api/api/metrics_api.py
--rw-r--r--  2.0 unx     8514 b- defN 23-Jun-02 14:23 cloudsmith_api/api/namespaces_api.py
--rw-r--r--  2.0 unx   199931 b- defN 23-Jun-02 14:23 cloudsmith_api/api/orgs_api.py
--rw-r--r--  2.0 unx   294424 b- defN 23-Jun-02 14:23 cloudsmith_api/api/packages_api.py
--rw-r--r--  2.0 unx    16386 b- defN 23-Jun-02 14:23 cloudsmith_api/api/quota_api.py
--rw-r--r--  2.0 unx     4157 b- defN 23-Jun-02 14:23 cloudsmith_api/api/rates_api.py
--rw-r--r--  2.0 unx    98642 b- defN 23-Jun-02 14:23 cloudsmith_api/api/repos_api.py
--rw-r--r--  2.0 unx     4118 b- defN 23-Jun-02 14:23 cloudsmith_api/api/status_api.py
--rw-r--r--  2.0 unx     8075 b- defN 23-Jun-02 14:23 cloudsmith_api/api/storage_regions_api.py
--rw-r--r--  2.0 unx     7631 b- defN 23-Jun-02 14:23 cloudsmith_api/api/user_api.py
--rw-r--r--  2.0 unx     4706 b- defN 23-Jun-02 14:23 cloudsmith_api/api/users_api.py
--rw-r--r--  2.0 unx    22091 b- defN 23-Jun-02 14:23 cloudsmith_api/api/vulnerabilities_api.py
--rw-r--r--  2.0 unx    26050 b- defN 23-Jun-02 14:23 cloudsmith_api/api/webhooks_api.py
--rw-r--r--  2.0 unx    14876 b- defN 23-Jun-02 14:23 cloudsmith_api/models/__init__.py
--rw-r--r--  2.0 unx     7305 b- defN 23-Jun-02 14:23 cloudsmith_api/models/allocated_limit.py
--rw-r--r--  2.0 unx     5410 b- defN 23-Jun-02 14:23 cloudsmith_api/models/allocated_limit_raw.py
--rw-r--r--  2.0 unx    58771 b- defN 23-Jun-02 14:23 cloudsmith_api/models/alpine_package_upload.py
--rw-r--r--  2.0 unx     7437 b- defN 23-Jun-02 14:23 cloudsmith_api/models/alpine_package_upload_request.py
--rw-r--r--  2.0 unx     4748 b- defN 23-Jun-02 14:23 cloudsmith_api/models/architecture.py
--rw-r--r--  2.0 unx    58494 b- defN 23-Jun-02 14:23 cloudsmith_api/models/cargo_package_upload.py
--rw-r--r--  2.0 unx     6177 b- defN 23-Jun-02 14:23 cloudsmith_api/models/cargo_package_upload_request.py
--rw-r--r--  2.0 unx    59602 b- defN 23-Jun-02 14:23 cloudsmith_api/models/cocoapods_package_upload.py
--rw-r--r--  2.0 unx     6245 b- defN 23-Jun-02 14:23 cloudsmith_api/models/cocoapods_package_upload_request.py
--rw-r--r--  2.0 unx     6052 b- defN 23-Jun-02 14:23 cloudsmith_api/models/common_bandwidth_metrics.py
--rw-r--r--  2.0 unx     5636 b- defN 23-Jun-02 14:23 cloudsmith_api/models/common_bandwidth_metrics_value.py
--rw-r--r--  2.0 unx     6052 b- defN 23-Jun-02 14:23 cloudsmith_api/models/common_downloads_metrics.py
--rw-r--r--  2.0 unx     3526 b- defN 23-Jun-02 14:23 cloudsmith_api/models/common_downloads_metrics_value.py
--rw-r--r--  2.0 unx     6129 b- defN 23-Jun-02 14:23 cloudsmith_api/models/common_metrics.py
--rw-r--r--  2.0 unx    59325 b- defN 23-Jun-02 14:23 cloudsmith_api/models/composer_package_upload.py
--rw-r--r--  2.0 unx     6228 b- defN 23-Jun-02 14:23 cloudsmith_api/models/composer_package_upload_request.py
--rw-r--r--  2.0 unx    61539 b- defN 23-Jun-02 14:23 cloudsmith_api/models/conan_package_upload.py
--rw-r--r--  2.0 unx    14491 b- defN 23-Jun-02 14:23 cloudsmith_api/models/conan_package_upload_request.py
--rw-r--r--  2.0 unx    58494 b- defN 23-Jun-02 14:23 cloudsmith_api/models/conda_package_upload.py
--rw-r--r--  2.0 unx     6177 b- defN 23-Jun-02 14:23 cloudsmith_api/models/conda_package_upload_request.py
--rw-r--r--  2.0 unx    58217 b- defN 23-Jun-02 14:23 cloudsmith_api/models/cran_package_upload.py
--rw-r--r--  2.0 unx     6160 b- defN 23-Jun-02 14:23 cloudsmith_api/models/cran_package_upload_request.py
--rw-r--r--  2.0 unx    58217 b- defN 23-Jun-02 14:23 cloudsmith_api/models/dart_package_upload.py
--rw-r--r--  2.0 unx     6160 b- defN 23-Jun-02 14:23 cloudsmith_api/models/dart_package_upload_request.py
--rw-r--r--  2.0 unx    57940 b- defN 23-Jun-02 14:23 cloudsmith_api/models/deb_package_upload.py
--rw-r--r--  2.0 unx     9690 b- defN 23-Jun-02 14:23 cloudsmith_api/models/deb_package_upload_request.py
--rw-r--r--  2.0 unx     6159 b- defN 23-Jun-02 14:23 cloudsmith_api/models/distribution.py
--rw-r--r--  2.0 unx     8542 b- defN 23-Jun-02 14:23 cloudsmith_api/models/distribution_full.py
--rw-r--r--  2.0 unx     4497 b- defN 23-Jun-02 14:23 cloudsmith_api/models/distribution_version.py
--rw-r--r--  2.0 unx    58771 b- defN 23-Jun-02 14:23 cloudsmith_api/models/docker_package_upload.py
--rw-r--r--  2.0 unx     6194 b- defN 23-Jun-02 14:23 cloudsmith_api/models/docker_package_upload_request.py
--rw-r--r--  2.0 unx     3541 b- defN 23-Jun-02 14:23 cloudsmith_api/models/entitlement_usage_metrics.py
--rw-r--r--  2.0 unx     3729 b- defN 23-Jun-02 14:23 cloudsmith_api/models/error_detail.py
--rw-r--r--  2.0 unx     5458 b- defN 23-Jun-02 14:23 cloudsmith_api/models/eula.py
--rw-r--r--  2.0 unx    11287 b- defN 23-Jun-02 14:23 cloudsmith_api/models/format.py
--rw-r--r--  2.0 unx     7319 b- defN 23-Jun-02 14:23 cloudsmith_api/models/format_support.py
--rw-r--r--  2.0 unx     8615 b- defN 23-Jun-02 14:23 cloudsmith_api/models/geo_ip_location.py
--rw-r--r--  2.0 unx    57663 b- defN 23-Jun-02 14:23 cloudsmith_api/models/go_package_upload.py
--rw-r--r--  2.0 unx     6126 b- defN 23-Jun-02 14:23 cloudsmith_api/models/go_package_upload_request.py
--rw-r--r--  2.0 unx    58217 b- defN 23-Jun-02 14:23 cloudsmith_api/models/helm_package_upload.py
--rw-r--r--  2.0 unx     7480 b- defN 23-Jun-02 14:23 cloudsmith_api/models/helm_package_upload_request.py
--rw-r--r--  2.0 unx    57940 b- defN 23-Jun-02 14:23 cloudsmith_api/models/hex_package_upload.py
--rw-r--r--  2.0 unx     6143 b- defN 23-Jun-02 14:23 cloudsmith_api/models/hex_package_upload_request.py
--rw-r--r--  2.0 unx     7028 b- defN 23-Jun-02 14:23 cloudsmith_api/models/history.py
--rw-r--r--  2.0 unx     5168 b- defN 23-Jun-02 14:23 cloudsmith_api/models/history_fieldset.py
--rw-r--r--  2.0 unx     5246 b- defN 23-Jun-02 14:23 cloudsmith_api/models/history_fieldset_raw.py
--rw-r--r--  2.0 unx    59325 b- defN 23-Jun-02 14:23 cloudsmith_api/models/luarocks_package_upload.py
--rw-r--r--  2.0 unx     6228 b- defN 23-Jun-02 14:23 cloudsmith_api/models/luarocks_package_upload_request.py
--rw-r--r--  2.0 unx    63607 b- defN 23-Jun-02 14:23 cloudsmith_api/models/maven_package_upload.py
--rw-r--r--  2.0 unx    17576 b- defN 23-Jun-02 14:23 cloudsmith_api/models/maven_package_upload_request.py
--rw-r--r--  2.0 unx     5806 b- defN 23-Jun-02 14:23 cloudsmith_api/models/namespace.py
--rw-r--r--  2.0 unx    18223 b- defN 23-Jun-02 14:23 cloudsmith_api/models/namespace_audit_log.py
--rw-r--r--  2.0 unx    11620 b- defN 23-Jun-02 14:23 cloudsmith_api/models/nested_license_policy.py
--rw-r--r--  2.0 unx    12280 b- defN 23-Jun-02 14:23 cloudsmith_api/models/nested_vulnerability_policy.py
--rw-r--r--  2.0 unx     9527 b- defN 23-Jun-02 14:23 cloudsmith_api/models/nested_vulnerability_scan_results.py
--rw-r--r--  2.0 unx    57940 b- defN 23-Jun-02 14:23 cloudsmith_api/models/npm_package_upload.py
--rw-r--r--  2.0 unx     7663 b- defN 23-Jun-02 14:23 cloudsmith_api/models/npm_package_upload_request.py
--rw-r--r--  2.0 unx    58494 b- defN 23-Jun-02 14:23 cloudsmith_api/models/nuget_package_upload.py
--rw-r--r--  2.0 unx     7272 b- defN 23-Jun-02 14:23 cloudsmith_api/models/nuget_package_upload_request.py
--rw-r--r--  2.0 unx     7918 b- defN 23-Jun-02 14:23 cloudsmith_api/models/organization.py
--rw-r--r--  2.0 unx     8391 b- defN 23-Jun-02 14:23 cloudsmith_api/models/organization_group_sync.py
--rw-r--r--  2.0 unx     8223 b- defN 23-Jun-02 14:23 cloudsmith_api/models/organization_group_sync_request.py
--rw-r--r--  2.0 unx    10169 b- defN 23-Jun-02 14:23 cloudsmith_api/models/organization_invite.py
--rw-r--r--  2.0 unx    10519 b- defN 23-Jun-02 14:23 cloudsmith_api/models/organization_invite_extend.py
--rw-r--r--  2.0 unx     5661 b- defN 23-Jun-02 14:23 cloudsmith_api/models/organization_invite_request.py
--rw-r--r--  2.0 unx     3821 b- defN 23-Jun-02 14:23 cloudsmith_api/models/organization_invite_update.py
--rw-r--r--  2.0 unx     3929 b- defN 23-Jun-02 14:23 cloudsmith_api/models/organization_invite_update_request_patch.py
--rw-r--r--  2.0 unx    12300 b- defN 23-Jun-02 14:23 cloudsmith_api/models/organization_membership.py
--rw-r--r--  2.0 unx    12219 b- defN 23-Jun-02 14:23 cloudsmith_api/models/organization_package_license_policy.py
--rw-r--r--  2.0 unx     9666 b- defN 23-Jun-02 14:23 cloudsmith_api/models/organization_package_license_policy_request.py
--rw-r--r--  2.0 unx     9539 b- defN 23-Jun-02 14:23 cloudsmith_api/models/organization_package_license_policy_request_patch.py
--rw-r--r--  2.0 unx    12855 b- defN 23-Jun-02 14:23 cloudsmith_api/models/organization_package_vulnerability_policy.py
--rw-r--r--  2.0 unx    10230 b- defN 23-Jun-02 14:23 cloudsmith_api/models/organization_package_vulnerability_policy_request.py
--rw-r--r--  2.0 unx    10245 b- defN 23-Jun-02 14:23 cloudsmith_api/models/organization_package_vulnerability_policy_request_patch.py
--rw-r--r--  2.0 unx     8110 b- defN 23-Jun-02 14:23 cloudsmith_api/models/organization_team.py
--rw-r--r--  2.0 unx     3669 b- defN 23-Jun-02 14:23 cloudsmith_api/models/organization_team_members.py
--rw-r--r--  2.0 unx     4783 b- defN 23-Jun-02 14:23 cloudsmith_api/models/organization_team_membership.py
--rw-r--r--  2.0 unx     7065 b- defN 23-Jun-02 14:23 cloudsmith_api/models/organization_team_request.py
--rw-r--r--  2.0 unx     7040 b- defN 23-Jun-02 14:23 cloudsmith_api/models/organization_team_request_patch.py
--rw-r--r--  2.0 unx    57663 b- defN 23-Jun-02 14:23 cloudsmith_api/models/p2_package_upload.py
--rw-r--r--  2.0 unx     6126 b- defN 23-Jun-02 14:23 cloudsmith_api/models/p2_package_upload_request.py
--rw-r--r--  2.0 unx    55965 b- defN 23-Jun-02 14:23 cloudsmith_api/models/package.py
--rw-r--r--  2.0 unx    57197 b- defN 23-Jun-02 14:23 cloudsmith_api/models/package_copy.py
--rw-r--r--  2.0 unx     4776 b- defN 23-Jun-02 14:23 cloudsmith_api/models/package_copy_request.py
--rw-r--r--  2.0 unx     3523 b- defN 23-Jun-02 14:23 cloudsmith_api/models/package_dependencies.py
--rw-r--r--  2.0 unx     7227 b- defN 23-Jun-02 14:23 cloudsmith_api/models/package_dependency.py
--rw-r--r--  2.0 unx    12968 b- defN 23-Jun-02 14:23 cloudsmith_api/models/package_file.py
--rw-r--r--  2.0 unx     6108 b- defN 23-Jun-02 14:23 cloudsmith_api/models/package_file_parts_upload.py
--rw-r--r--  2.0 unx     7841 b- defN 23-Jun-02 14:23 cloudsmith_api/models/package_file_upload.py
--rw-r--r--  2.0 unx     7815 b- defN 23-Jun-02 14:23 cloudsmith_api/models/package_file_upload_request.py
--rw-r--r--  2.0 unx     6035 b- defN 23-Jun-02 14:23 cloudsmith_api/models/package_license_policy_violation_log.py
--rw-r--r--  2.0 unx     5198 b- defN 23-Jun-02 14:23 cloudsmith_api/models/package_license_policy_violation_log_cursor_page.py
--rw-r--r--  2.0 unx    57195 b- defN 23-Jun-02 14:23 cloudsmith_api/models/package_move.py
--rw-r--r--  2.0 unx     3820 b- defN 23-Jun-02 14:23 cloudsmith_api/models/package_move_request.py
--rw-r--r--  2.0 unx    58775 b- defN 23-Jun-02 14:23 cloudsmith_api/models/package_quarantine.py
--rw-r--r--  2.0 unx     3527 b- defN 23-Jun-02 14:23 cloudsmith_api/models/package_quarantine_request.py
--rw-r--r--  2.0 unx    57651 b- defN 23-Jun-02 14:23 cloudsmith_api/models/package_resync.py
--rw-r--r--  2.0 unx    15877 b- defN 23-Jun-02 14:23 cloudsmith_api/models/package_status.py
--rw-r--r--  2.0 unx    57199 b- defN 23-Jun-02 14:23 cloudsmith_api/models/package_tag.py
--rw-r--r--  2.0 unx     5352 b- defN 23-Jun-02 14:23 cloudsmith_api/models/package_tag_request.py
--rw-r--r--  2.0 unx     3547 b- defN 23-Jun-02 14:23 cloudsmith_api/models/package_usage_metrics.py
--rw-r--r--  2.0 unx     2740 b- defN 23-Jun-02 14:23 cloudsmith_api/models/package_version_badge.py
--rw-r--r--  2.0 unx     5707 b- defN 23-Jun-02 14:23 cloudsmith_api/models/package_vulnerability.py
--rw-r--r--  2.0 unx     7491 b- defN 23-Jun-02 14:23 cloudsmith_api/models/package_vulnerability_policy_violation_log.py
--rw-r--r--  2.0 unx     5318 b- defN 23-Jun-02 14:23 cloudsmith_api/models/package_vulnerability_policy_violation_log_cursor_page.py
--rw-r--r--  2.0 unx    58771 b- defN 23-Jun-02 14:23 cloudsmith_api/models/python_package_upload.py
--rw-r--r--  2.0 unx     6194 b- defN 23-Jun-02 14:23 cloudsmith_api/models/python_package_upload_request.py
--rw-r--r--  2.0 unx     3358 b- defN 23-Jun-02 14:23 cloudsmith_api/models/quota.py
--rw-r--r--  2.0 unx     3463 b- defN 23-Jun-02 14:23 cloudsmith_api/models/quota_history.py
--rw-r--r--  2.0 unx     7675 b- defN 23-Jun-02 14:23 cloudsmith_api/models/rate_check.py
--rw-r--r--  2.0 unx    58899 b- defN 23-Jun-02 14:23 cloudsmith_api/models/raw_package_upload.py
--rw-r--r--  2.0 unx    11674 b- defN 23-Jun-02 14:23 cloudsmith_api/models/raw_package_upload_request.py
--rw-r--r--  2.0 unx    66229 b- defN 23-Jun-02 14:23 cloudsmith_api/models/repository.py
--rw-r--r--  2.0 unx    14861 b- defN 23-Jun-02 14:23 cloudsmith_api/models/repository_audit_log.py
--rw-r--r--  2.0 unx    67555 b- defN 23-Jun-02 14:23 cloudsmith_api/models/repository_create.py
--rw-r--r--  2.0 unx    52996 b- defN 23-Jun-02 14:23 cloudsmith_api/models/repository_create_request.py
--rw-r--r--  2.0 unx     4365 b- defN 23-Jun-02 14:23 cloudsmith_api/models/repository_geo_ip_cidr.py
--rw-r--r--  2.0 unx     4488 b- defN 23-Jun-02 14:23 cloudsmith_api/models/repository_geo_ip_country_code.py
--rw-r--r--  2.0 unx     4424 b- defN 23-Jun-02 14:23 cloudsmith_api/models/repository_geo_ip_rules.py
--rw-r--r--  2.0 unx     4515 b- defN 23-Jun-02 14:23 cloudsmith_api/models/repository_geo_ip_rules_request.py
--rw-r--r--  2.0 unx     4312 b- defN 23-Jun-02 14:23 cloudsmith_api/models/repository_geo_ip_rules_request_patch.py
--rw-r--r--  2.0 unx     3733 b- defN 23-Jun-02 14:23 cloudsmith_api/models/repository_geo_ip_test_address.py
--rw-r--r--  2.0 unx     3906 b- defN 23-Jun-02 14:23 cloudsmith_api/models/repository_geo_ip_test_address_response.py
--rw-r--r--  2.0 unx     7359 b- defN 23-Jun-02 14:23 cloudsmith_api/models/repository_geo_ip_test_address_response_dict.py
--rw-r--r--  2.0 unx     8734 b- defN 23-Jun-02 14:23 cloudsmith_api/models/repository_gpg_key.py
--rw-r--r--  2.0 unx     5133 b- defN 23-Jun-02 14:23 cloudsmith_api/models/repository_gpg_key_create.py
--rw-r--r--  2.0 unx     7702 b- defN 23-Jun-02 14:23 cloudsmith_api/models/repository_privilege_dict.py
--rw-r--r--  2.0 unx     3818 b- defN 23-Jun-02 14:23 cloudsmith_api/models/repository_privilege_input.py
--rw-r--r--  2.0 unx     3881 b- defN 23-Jun-02 14:23 cloudsmith_api/models/repository_privilege_input_request.py
--rw-r--r--  2.0 unx     3790 b- defN 23-Jun-02 14:23 cloudsmith_api/models/repository_privilege_input_request_patch.py
--rw-r--r--  2.0 unx    51807 b- defN 23-Jun-02 14:23 cloudsmith_api/models/repository_request_patch.py
--rw-r--r--  2.0 unx     7753 b- defN 23-Jun-02 14:23 cloudsmith_api/models/repository_rsa_key.py
--rw-r--r--  2.0 unx     5133 b- defN 23-Jun-02 14:23 cloudsmith_api/models/repository_rsa_key_create.py
--rw-r--r--  2.0 unx    40544 b- defN 23-Jun-02 14:23 cloudsmith_api/models/repository_token.py
--rw-r--r--  2.0 unx     2750 b- defN 23-Jun-02 14:23 cloudsmith_api/models/repository_token_action.py
--rw-r--r--  2.0 unx    41541 b- defN 23-Jun-02 14:23 cloudsmith_api/models/repository_token_refresh.py
--rw-r--r--  2.0 unx    21868 b- defN 23-Jun-02 14:23 cloudsmith_api/models/repository_token_refresh_request.py
--rw-r--r--  2.0 unx    22374 b- defN 23-Jun-02 14:23 cloudsmith_api/models/repository_token_request.py
--rw-r--r--  2.0 unx    22569 b- defN 23-Jun-02 14:23 cloudsmith_api/models/repository_token_request_patch.py
--rw-r--r--  2.0 unx     3505 b- defN 23-Jun-02 14:23 cloudsmith_api/models/repository_token_sync.py
--rw-r--r--  2.0 unx     3904 b- defN 23-Jun-02 14:23 cloudsmith_api/models/repository_token_sync_request.py
--rw-r--r--  2.0 unx    30728 b- defN 23-Jun-02 14:23 cloudsmith_api/models/repository_webhook.py
--rw-r--r--  2.0 unx    18912 b- defN 23-Jun-02 14:23 cloudsmith_api/models/repository_webhook_request.py
--rw-r--r--  2.0 unx    18774 b- defN 23-Jun-02 14:23 cloudsmith_api/models/repository_webhook_request_patch.py
--rw-r--r--  2.0 unx     3523 b- defN 23-Jun-02 14:23 cloudsmith_api/models/resources_rate_check.py
--rw-r--r--  2.0 unx     2790 b- defN 23-Jun-02 14:23 cloudsmith_api/models/respository_geo_ip_enable_disable.py
--rw-r--r--  2.0 unx     2825 b- defN 23-Jun-02 14:23 cloudsmith_api/models/respository_geo_ip_enable_disable_request.py
--rw-r--r--  2.0 unx    57940 b- defN 23-Jun-02 14:23 cloudsmith_api/models/rpm_package_upload.py
--rw-r--r--  2.0 unx     7374 b- defN 23-Jun-02 14:23 cloudsmith_api/models/rpm_package_upload_request.py
--rw-r--r--  2.0 unx    58217 b- defN 23-Jun-02 14:23 cloudsmith_api/models/ruby_package_upload.py
--rw-r--r--  2.0 unx     6160 b- defN 23-Jun-02 14:23 cloudsmith_api/models/ruby_package_upload_request.py
--rw-r--r--  2.0 unx     8234 b- defN 23-Jun-02 14:23 cloudsmith_api/models/service.py
--rw-r--r--  2.0 unx     6726 b- defN 23-Jun-02 14:23 cloudsmith_api/models/service_request.py
--rw-r--r--  2.0 unx     6701 b- defN 23-Jun-02 14:23 cloudsmith_api/models/service_request_patch.py
--rw-r--r--  2.0 unx     4951 b- defN 23-Jun-02 14:23 cloudsmith_api/models/service_teams.py
--rw-r--r--  2.0 unx     4584 b- defN 23-Jun-02 14:23 cloudsmith_api/models/status_basic.py
--rw-r--r--  2.0 unx     8478 b- defN 23-Jun-02 14:23 cloudsmith_api/models/storage_allocated_limit.py
--rw-r--r--  2.0 unx     6140 b- defN 23-Jun-02 14:23 cloudsmith_api/models/storage_allocated_limit_raw.py
--rw-r--r--  2.0 unx     4670 b- defN 23-Jun-02 14:23 cloudsmith_api/models/storage_region.py
--rw-r--r--  2.0 unx     6847 b- defN 23-Jun-02 14:23 cloudsmith_api/models/storage_usage.py
--rw-r--r--  2.0 unx     5048 b- defN 23-Jun-02 14:23 cloudsmith_api/models/storage_usage_raw.py
--rw-r--r--  2.0 unx    58865 b- defN 23-Jun-02 14:23 cloudsmith_api/models/swift_package_upload.py
--rw-r--r--  2.0 unx     7279 b- defN 23-Jun-02 14:23 cloudsmith_api/models/swift_package_upload_request.py
--rw-r--r--  2.0 unx     2665 b- defN 23-Jun-02 14:23 cloudsmith_api/models/tags.py
--rw-r--r--  2.0 unx    59602 b- defN 23-Jun-02 14:23 cloudsmith_api/models/terraform_package_upload.py
--rw-r--r--  2.0 unx     6245 b- defN 23-Jun-02 14:23 cloudsmith_api/models/terraform_package_upload_request.py
--rw-r--r--  2.0 unx     5738 b- defN 23-Jun-02 14:23 cloudsmith_api/models/usage.py
--rw-r--r--  2.0 unx     4147 b- defN 23-Jun-02 14:23 cloudsmith_api/models/usage_fieldset.py
--rw-r--r--  2.0 unx     4277 b- defN 23-Jun-02 14:23 cloudsmith_api/models/usage_limits.py
--rw-r--r--  2.0 unx     4334 b- defN 23-Jun-02 14:23 cloudsmith_api/models/usage_limits_raw.py
--rw-r--r--  2.0 unx     4382 b- defN 23-Jun-02 14:23 cloudsmith_api/models/usage_raw.py
--rw-r--r--  2.0 unx     3590 b- defN 23-Jun-02 14:23 cloudsmith_api/models/user_auth_token.py
--rw-r--r--  2.0 unx     4612 b- defN 23-Jun-02 14:23 cloudsmith_api/models/user_auth_token_request.py
--rw-r--r--  2.0 unx     8019 b- defN 23-Jun-02 14:23 cloudsmith_api/models/user_brief.py
--rw-r--r--  2.0 unx    11110 b- defN 23-Jun-02 14:23 cloudsmith_api/models/user_profile.py
--rw-r--r--  2.0 unx    60899 b- defN 23-Jun-02 14:23 cloudsmith_api/models/vagrant_package_upload.py
--rw-r--r--  2.0 unx     9492 b- defN 23-Jun-02 14:23 cloudsmith_api/models/vagrant_package_upload_request.py
--rw-r--r--  2.0 unx    13112 b- defN 23-Jun-02 14:23 cloudsmith_api/models/vulnerability.py
--rw-r--r--  2.0 unx     5400 b- defN 23-Jun-02 14:23 cloudsmith_api/models/vulnerability_scan.py
--rw-r--r--  2.0 unx    10348 b- defN 23-Jun-02 14:23 cloudsmith_api/models/vulnerability_scan_results.py
--rw-r--r--  2.0 unx     9725 b- defN 23-Jun-02 14:23 cloudsmith_api/models/vulnerability_scan_results_list.py
--rw-r--r--  2.0 unx     8443 b- defN 23-Jun-02 14:23 cloudsmith_api/models/vulnerability_scan_version.py
--rw-r--r--  2.0 unx     4751 b- defN 23-Jun-02 14:23 cloudsmith_api/models/webhook_template.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-02 14:23 test/__init__.py
--rw-r--r--  2.0 unx      900 b- defN 23-Jun-02 14:23 test/test_allocated_limit.py
--rw-r--r--  2.0 unx      926 b- defN 23-Jun-02 14:23 test/test_allocated_limit_raw.py
--rw-r--r--  2.0 unx      942 b- defN 23-Jun-02 14:23 test/test_alpine_package_upload.py
--rw-r--r--  2.0 unx     1000 b- defN 23-Jun-02 14:23 test/test_alpine_package_upload_request.py
--rw-r--r--  2.0 unx      882 b- defN 23-Jun-02 14:23 test/test_architecture.py
--rw-r--r--  2.0 unx     1083 b- defN 23-Jun-02 14:23 test/test_audit_log_api.py
--rw-r--r--  2.0 unx      883 b- defN 23-Jun-02 14:23 test/test_badges_api.py
--rw-r--r--  2.0 unx      934 b- defN 23-Jun-02 14:23 test/test_cargo_package_upload.py
--rw-r--r--  2.0 unx      992 b- defN 23-Jun-02 14:23 test/test_cargo_package_upload_request.py
--rw-r--r--  2.0 unx      966 b- defN 23-Jun-02 14:23 test/test_cocoapods_package_upload.py
--rw-r--r--  2.0 unx     1024 b- defN 23-Jun-02 14:23 test/test_cocoapods_package_upload_request.py
--rw-r--r--  2.0 unx      966 b- defN 23-Jun-02 14:23 test/test_common_bandwidth_metrics.py
--rw-r--r--  2.0 unx     1008 b- defN 23-Jun-02 14:23 test/test_common_bandwidth_metrics_value.py
--rw-r--r--  2.0 unx      966 b- defN 23-Jun-02 14:23 test/test_common_downloads_metrics.py
--rw-r--r--  2.0 unx     1008 b- defN 23-Jun-02 14:23 test/test_common_downloads_metrics_value.py
--rw-r--r--  2.0 unx      892 b- defN 23-Jun-02 14:23 test/test_common_metrics.py
--rw-r--r--  2.0 unx      958 b- defN 23-Jun-02 14:23 test/test_composer_package_upload.py
--rw-r--r--  2.0 unx     1016 b- defN 23-Jun-02 14:23 test/test_composer_package_upload_request.py
--rw-r--r--  2.0 unx      934 b- defN 23-Jun-02 14:23 test/test_conan_package_upload.py
--rw-r--r--  2.0 unx      992 b- defN 23-Jun-02 14:23 test/test_conan_package_upload_request.py
--rw-r--r--  2.0 unx      934 b- defN 23-Jun-02 14:23 test/test_conda_package_upload.py
--rw-r--r--  2.0 unx      992 b- defN 23-Jun-02 14:23 test/test_conda_package_upload_request.py
--rw-r--r--  2.0 unx      926 b- defN 23-Jun-02 14:23 test/test_cran_package_upload.py
--rw-r--r--  2.0 unx      984 b- defN 23-Jun-02 14:23 test/test_cran_package_upload_request.py
--rw-r--r--  2.0 unx      926 b- defN 23-Jun-02 14:23 test/test_dart_package_upload.py
--rw-r--r--  2.0 unx      984 b- defN 23-Jun-02 14:23 test/test_dart_package_upload_request.py
--rw-r--r--  2.0 unx      918 b- defN 23-Jun-02 14:23 test/test_deb_package_upload.py
--rw-r--r--  2.0 unx      976 b- defN 23-Jun-02 14:23 test/test_deb_package_upload_request.py
--rw-r--r--  2.0 unx      882 b- defN 23-Jun-02 14:23 test/test_distribution.py
--rw-r--r--  2.0 unx      916 b- defN 23-Jun-02 14:23 test/test_distribution_full.py
--rw-r--r--  2.0 unx      940 b- defN 23-Jun-02 14:23 test/test_distribution_version.py
--rw-r--r--  2.0 unx     1019 b- defN 23-Jun-02 14:23 test/test_distros_api.py
--rw-r--r--  2.0 unx      942 b- defN 23-Jun-02 14:23 test/test_docker_package_upload.py
--rw-r--r--  2.0 unx     1000 b- defN 23-Jun-02 14:23 test/test_docker_package_upload_request.py
--rw-r--r--  2.0 unx      974 b- defN 23-Jun-02 14:23 test/test_entitlement_usage_metrics.py
--rw-r--r--  2.0 unx     2550 b- defN 23-Jun-02 14:23 test/test_entitlements_api.py
--rw-r--r--  2.0 unx      876 b- defN 23-Jun-02 14:23 test/test_error_detail.py
--rw-r--r--  2.0 unx      818 b- defN 23-Jun-02 14:23 test/test_eula.py
--rw-r--r--  2.0 unx     1503 b- defN 23-Jun-02 14:23 test/test_files_api.py
--rw-r--r--  2.0 unx      834 b- defN 23-Jun-02 14:23 test/test_format.py
--rw-r--r--  2.0 unx      892 b- defN 23-Jun-02 14:23 test/test_format_support.py
--rw-r--r--  2.0 unx     1022 b- defN 23-Jun-02 14:23 test/test_formats_api.py
--rw-r--r--  2.0 unx      894 b- defN 23-Jun-02 14:23 test/test_geo_ip_location.py
--rw-r--r--  2.0 unx      910 b- defN 23-Jun-02 14:23 test/test_go_package_upload.py
--rw-r--r--  2.0 unx      968 b- defN 23-Jun-02 14:23 test/test_go_package_upload_request.py
--rw-r--r--  2.0 unx      926 b- defN 23-Jun-02 14:23 test/test_helm_package_upload.py
--rw-r--r--  2.0 unx      984 b- defN 23-Jun-02 14:23 test/test_helm_package_upload_request.py
--rw-r--r--  2.0 unx      918 b- defN 23-Jun-02 14:23 test/test_hex_package_upload.py
--rw-r--r--  2.0 unx      976 b- defN 23-Jun-02 14:23 test/test_hex_package_upload_request.py
--rw-r--r--  2.0 unx      842 b- defN 23-Jun-02 14:23 test/test_history.py
--rw-r--r--  2.0 unx      908 b- defN 23-Jun-02 14:23 test/test_history_fieldset.py
--rw-r--r--  2.0 unx      934 b- defN 23-Jun-02 14:23 test/test_history_fieldset_raw.py
--rw-r--r--  2.0 unx      958 b- defN 23-Jun-02 14:23 test/test_luarocks_package_upload.py
--rw-r--r--  2.0 unx     1016 b- defN 23-Jun-02 14:23 test/test_luarocks_package_upload_request.py
--rw-r--r--  2.0 unx      934 b- defN 23-Jun-02 14:23 test/test_maven_package_upload.py
--rw-r--r--  2.0 unx      992 b- defN 23-Jun-02 14:23 test/test_maven_package_upload_request.py
--rw-r--r--  2.0 unx     1335 b- defN 23-Jun-02 14:23 test/test_metrics_api.py
--rw-r--r--  2.0 unx      858 b- defN 23-Jun-02 14:23 test/test_namespace.py
--rw-r--r--  2.0 unx      926 b- defN 23-Jun-02 14:23 test/test_namespace_audit_log.py
--rw-r--r--  2.0 unx     1051 b- defN 23-Jun-02 14:23 test/test_namespaces_api.py
--rw-r--r--  2.0 unx      942 b- defN 23-Jun-02 14:23 test/test_nested_license_policy.py
--rw-r--r--  2.0 unx      990 b- defN 23-Jun-02 14:23 test/test_nested_vulnerability_policy.py
--rw-r--r--  2.0 unx     1032 b- defN 23-Jun-02 14:23 test/test_nested_vulnerability_scan_results.py
--rw-r--r--  2.0 unx      918 b- defN 23-Jun-02 14:23 test/test_npm_package_upload.py
--rw-r--r--  2.0 unx      976 b- defN 23-Jun-02 14:23 test/test_npm_package_upload_request.py
--rw-r--r--  2.0 unx      934 b- defN 23-Jun-02 14:23 test/test_nuget_package_upload.py
--rw-r--r--  2.0 unx      992 b- defN 23-Jun-02 14:23 test/test_nuget_package_upload_request.py
--rw-r--r--  2.0 unx      882 b- defN 23-Jun-02 14:23 test/test_organization.py
--rw-r--r--  2.0 unx      958 b- defN 23-Jun-02 14:23 test/test_organization_group_sync.py
--rw-r--r--  2.0 unx     1016 b- defN 23-Jun-02 14:23 test/test_organization_group_sync_request.py
--rw-r--r--  2.0 unx      932 b- defN 23-Jun-02 14:23 test/test_organization_invite.py
--rw-r--r--  2.0 unx      982 b- defN 23-Jun-02 14:23 test/test_organization_invite_extend.py
--rw-r--r--  2.0 unx      990 b- defN 23-Jun-02 14:23 test/test_organization_invite_request.py
--rw-r--r--  2.0 unx      982 b- defN 23-Jun-02 14:23 test/test_organization_invite_update.py
--rw-r--r--  2.0 unx     1082 b- defN 23-Jun-02 14:23 test/test_organization_invite_update_request_patch.py
--rw-r--r--  2.0 unx      964 b- defN 23-Jun-02 14:23 test/test_organization_membership.py
--rw-r--r--  2.0 unx     1048 b- defN 23-Jun-02 14:23 test/test_organization_package_license_policy.py
--rw-r--r--  2.0 unx     1106 b- defN 23-Jun-02 14:23 test/test_organization_package_license_policy_request.py
--rw-r--r--  2.0 unx     1148 b- defN 23-Jun-02 14:23 test/test_organization_package_license_policy_request_patch.py
--rw-r--r--  2.0 unx     1096 b- defN 23-Jun-02 14:23 test/test_organization_package_vulnerability_policy.py
--rw-r--r--  2.0 unx     1154 b- defN 23-Jun-02 14:23 test/test_organization_package_vulnerability_policy_request.py
--rw-r--r--  2.0 unx     1196 b- defN 23-Jun-02 14:23 test/test_organization_package_vulnerability_policy_request_patch.py
--rw-r--r--  2.0 unx      916 b- defN 23-Jun-02 14:23 test/test_organization_team.py
--rw-r--r--  2.0 unx      974 b- defN 23-Jun-02 14:23 test/test_organization_team_members.py
--rw-r--r--  2.0 unx      998 b- defN 23-Jun-02 14:23 test/test_organization_team_membership.py
--rw-r--r--  2.0 unx      974 b- defN 23-Jun-02 14:23 test/test_organization_team_request.py
--rw-r--r--  2.0 unx     1016 b- defN 23-Jun-02 14:23 test/test_organization_team_request_patch.py
--rw-r--r--  2.0 unx     8908 b- defN 23-Jun-02 14:23 test/test_orgs_api.py
--rw-r--r--  2.0 unx      910 b- defN 23-Jun-02 14:23 test/test_p2_package_upload.py
--rw-r--r--  2.0 unx      968 b- defN 23-Jun-02 14:23 test/test_p2_package_upload_request.py
--rw-r--r--  2.0 unx      842 b- defN 23-Jun-02 14:23 test/test_package.py
--rw-r--r--  2.0 unx      876 b- defN 23-Jun-02 14:23 test/test_package_copy.py
--rw-r--r--  2.0 unx      934 b- defN 23-Jun-02 14:23 test/test_package_copy_request.py
--rw-r--r--  2.0 unx      940 b- defN 23-Jun-02 14:23 test/test_package_dependencies.py
--rw-r--r--  2.0 unx      924 b- defN 23-Jun-02 14:23 test/test_package_dependency.py
--rw-r--r--  2.0 unx      876 b- defN 23-Jun-02 14:23 test/test_package_file.py
--rw-r--r--  2.0 unx      968 b- defN 23-Jun-02 14:23 test/test_package_file_parts_upload.py
--rw-r--r--  2.0 unx      926 b- defN 23-Jun-02 14:23 test/test_package_file_upload.py
--rw-r--r--  2.0 unx      984 b- defN 23-Jun-02 14:23 test/test_package_file_upload_request.py
--rw-r--r--  2.0 unx     1050 b- defN 23-Jun-02 14:23 test/test_package_license_policy_violation_log.py
--rw-r--r--  2.0 unx     1134 b- defN 23-Jun-02 14:23 test/test_package_license_policy_violation_log_cursor_page.py
--rw-r--r--  2.0 unx      876 b- defN 23-Jun-02 14:23 test/test_package_move.py
--rw-r--r--  2.0 unx      934 b- defN 23-Jun-02 14:23 test/test_package_move_request.py
--rw-r--r--  2.0 unx      924 b- defN 23-Jun-02 14:23 test/test_package_quarantine.py
--rw-r--r--  2.0 unx      982 b- defN 23-Jun-02 14:23 test/test_package_quarantine_request.py
--rw-r--r--  2.0 unx      892 b- defN 23-Jun-02 14:23 test/test_package_resync.py
--rw-r--r--  2.0 unx      892 b- defN 23-Jun-02 14:23 test/test_package_status.py
--rw-r--r--  2.0 unx      868 b- defN 23-Jun-02 14:23 test/test_package_tag.py
--rw-r--r--  2.0 unx      926 b- defN 23-Jun-02 14:23 test/test_package_tag_request.py
--rw-r--r--  2.0 unx      942 b- defN 23-Jun-02 14:23 test/test_package_usage_metrics.py
--rw-r--r--  2.0 unx      942 b- defN 23-Jun-02 14:23 test/test_package_version_badge.py
--rw-r--r--  2.0 unx      948 b- defN 23-Jun-02 14:23 test/test_package_vulnerability.py
--rw-r--r--  2.0 unx     1098 b- defN 23-Jun-02 14:23 test/test_package_vulnerability_policy_violation_log.py
--rw-r--r--  2.0 unx     1182 b- defN 23-Jun-02 14:23 test/test_package_vulnerability_policy_violation_log_cursor_page.py
--rw-r--r--  2.0 unx    11743 b- defN 23-Jun-02 14:23 test/test_packages_api.py
--rw-r--r--  2.0 unx      942 b- defN 23-Jun-02 14:23 test/test_python_package_upload.py
--rw-r--r--  2.0 unx     1000 b- defN 23-Jun-02 14:23 test/test_python_package_upload_request.py
--rw-r--r--  2.0 unx      826 b- defN 23-Jun-02 14:23 test/test_quota.py
--rw-r--r--  2.0 unx     1364 b- defN 23-Jun-02 14:23 test/test_quota_api.py
--rw-r--r--  2.0 unx      884 b- defN 23-Jun-02 14:23 test/test_quota_history.py
--rw-r--r--  2.0 unx      860 b- defN 23-Jun-02 14:23 test/test_rate_check.py
--rw-r--r--  2.0 unx      862 b- defN 23-Jun-02 14:23 test/test_rates_api.py
--rw-r--r--  2.0 unx      918 b- defN 23-Jun-02 14:23 test/test_raw_package_upload.py
--rw-r--r--  2.0 unx      976 b- defN 23-Jun-02 14:23 test/test_raw_package_upload_request.py
--rw-r--r--  2.0 unx     4407 b- defN 23-Jun-02 14:23 test/test_repos_api.py
--rw-r--r--  2.0 unx      866 b- defN 23-Jun-02 14:23 test/test_repository.py
--rw-r--r--  2.0 unx      934 b- defN 23-Jun-02 14:23 test/test_repository_audit_log.py
--rw-r--r--  2.0 unx      916 b- defN 23-Jun-02 14:23 test/test_repository_create.py
--rw-r--r--  2.0 unx      974 b- defN 23-Jun-02 14:23 test/test_repository_create_request.py
--rw-r--r--  2.0 unx      944 b- defN 23-Jun-02 14:23 test/test_repository_geo_ip_cidr.py
--rw-r--r--  2.0 unx     1002 b- defN 23-Jun-02 14:23 test/test_repository_geo_ip_country_code.py
--rw-r--r--  2.0 unx      952 b- defN 23-Jun-02 14:23 test/test_repository_geo_ip_rules.py
--rw-r--r--  2.0 unx     1010 b- defN 23-Jun-02 14:23 test/test_repository_geo_ip_rules_request.py
--rw-r--r--  2.0 unx     1052 b- defN 23-Jun-02 14:23 test/test_repository_geo_ip_rules_request_patch.py
--rw-r--r--  2.0 unx     1002 b- defN 23-Jun-02 14:23 test/test_repository_geo_ip_test_address.py
--rw-r--r--  2.0 unx     1068 b- defN 23-Jun-02 14:23 test/test_repository_geo_ip_test_address_response.py
--rw-r--r--  2.0 unx     1102 b- defN 23-Jun-02 14:23 test/test_repository_geo_ip_test_address_response_dict.py
--rw-r--r--  2.0 unx      918 b- defN 23-Jun-02 14:23 test/test_repository_gpg_key.py
--rw-r--r--  2.0 unx      968 b- defN 23-Jun-02 14:23 test/test_repository_gpg_key_create.py
--rw-r--r--  2.0 unx      974 b- defN 23-Jun-02 14:23 test/test_repository_privilege_dict.py
--rw-r--r--  2.0 unx      982 b- defN 23-Jun-02 14:23 test/test_repository_privilege_input.py
--rw-r--r--  2.0 unx     1040 b- defN 23-Jun-02 14:23 test/test_repository_privilege_input_request.py
--rw-r--r--  2.0 unx     1082 b- defN 23-Jun-02 14:23 test/test_repository_privilege_input_request_patch.py
--rw-r--r--  2.0 unx      966 b- defN 23-Jun-02 14:23 test/test_repository_request_patch.py
--rw-r--r--  2.0 unx      918 b- defN 23-Jun-02 14:23 test/test_repository_rsa_key.py
--rw-r--r--  2.0 unx      968 b- defN 23-Jun-02 14:23 test/test_repository_rsa_key_create.py
--rw-r--r--  2.0 unx      908 b- defN 23-Jun-02 14:23 test/test_repository_token.py
--rw-r--r--  2.0 unx      958 b- defN 23-Jun-02 14:23 test/test_repository_token_action.py
--rw-r--r--  2.0 unx      966 b- defN 23-Jun-02 14:23 test/test_repository_token_refresh.py
--rw-r--r--  2.0 unx     1024 b- defN 23-Jun-02 14:23 test/test_repository_token_refresh_request.py
--rw-r--r--  2.0 unx      966 b- defN 23-Jun-02 14:23 test/test_repository_token_request.py
--rw-r--r--  2.0 unx     1008 b- defN 23-Jun-02 14:23 test/test_repository_token_request_patch.py
--rw-r--r--  2.0 unx      942 b- defN 23-Jun-02 14:23 test/test_repository_token_sync.py
--rw-r--r--  2.0 unx     1000 b- defN 23-Jun-02 14:23 test/test_repository_token_sync_request.py
--rw-r--r--  2.0 unx      924 b- defN 23-Jun-02 14:23 test/test_repository_webhook.py
--rw-r--r--  2.0 unx      982 b- defN 23-Jun-02 14:23 test/test_repository_webhook_request.py
--rw-r--r--  2.0 unx     1024 b- defN 23-Jun-02 14:23 test/test_repository_webhook_request_patch.py
--rw-r--r--  2.0 unx      934 b- defN 23-Jun-02 14:23 test/test_resources_rate_check.py
--rw-r--r--  2.0 unx     1026 b- defN 23-Jun-02 14:23 test/test_respository_geo_ip_enable_disable.py
--rw-r--r--  2.0 unx     1084 b- defN 23-Jun-02 14:23 test/test_respository_geo_ip_enable_disable_request.py
--rw-r--r--  2.0 unx      918 b- defN 23-Jun-02 14:23 test/test_rpm_package_upload.py
--rw-r--r--  2.0 unx      976 b- defN 23-Jun-02 14:23 test/test_rpm_package_upload_request.py
--rw-r--r--  2.0 unx      926 b- defN 23-Jun-02 14:23 test/test_ruby_package_upload.py
--rw-r--r--  2.0 unx      984 b- defN 23-Jun-02 14:23 test/test_ruby_package_upload_request.py
--rw-r--r--  2.0 unx      842 b- defN 23-Jun-02 14:23 test/test_service.py
--rw-r--r--  2.0 unx      900 b- defN 23-Jun-02 14:23 test/test_service_request.py
--rw-r--r--  2.0 unx      942 b- defN 23-Jun-02 14:23 test/test_service_request_patch.py
--rw-r--r--  2.0 unx      884 b- defN 23-Jun-02 14:23 test/test_service_teams.py
--rw-r--r--  2.0 unx      864 b- defN 23-Jun-02 14:23 test/test_status_api.py
--rw-r--r--  2.0 unx      876 b- defN 23-Jun-02 14:23 test/test_status_basic.py
--rw-r--r--  2.0 unx      958 b- defN 23-Jun-02 14:23 test/test_storage_allocated_limit.py
--rw-r--r--  2.0 unx      984 b- defN 23-Jun-02 14:23 test/test_storage_allocated_limit_raw.py
--rw-r--r--  2.0 unx      892 b- defN 23-Jun-02 14:23 test/test_storage_region.py
--rw-r--r--  2.0 unx     1088 b- defN 23-Jun-02 14:23 test/test_storage_regions_api.py
--rw-r--r--  2.0 unx      884 b- defN 23-Jun-02 14:23 test/test_storage_usage.py
--rw-r--r--  2.0 unx      910 b- defN 23-Jun-02 14:23 test/test_storage_usage_raw.py
--rw-r--r--  2.0 unx      934 b- defN 23-Jun-02 14:23 test/test_swift_package_upload.py
--rw-r--r--  2.0 unx      992 b- defN 23-Jun-02 14:23 test/test_swift_package_upload_request.py
--rw-r--r--  2.0 unx      818 b- defN 23-Jun-02 14:23 test/test_tags.py
--rw-r--r--  2.0 unx      966 b- defN 23-Jun-02 14:23 test/test_terraform_package_upload.py
--rw-r--r--  2.0 unx     1024 b- defN 23-Jun-02 14:23 test/test_terraform_package_upload_request.py
--rw-r--r--  2.0 unx      826 b- defN 23-Jun-02 14:23 test/test_usage.py
--rw-r--r--  2.0 unx      892 b- defN 23-Jun-02 14:23 test/test_usage_fieldset.py
--rw-r--r--  2.0 unx      876 b- defN 23-Jun-02 14:23 test/test_usage_limits.py
--rw-r--r--  2.0 unx      902 b- defN 23-Jun-02 14:23 test/test_usage_limits_raw.py
--rw-r--r--  2.0 unx      852 b- defN 23-Jun-02 14:23 test/test_usage_raw.py
--rw-r--r--  2.0 unx     1024 b- defN 23-Jun-02 14:23 test/test_user_api.py
--rw-r--r--  2.0 unx      894 b- defN 23-Jun-02 14:23 test/test_user_auth_token.py
--rw-r--r--  2.0 unx      952 b- defN 23-Jun-02 14:23 test/test_user_auth_token_request.py
--rw-r--r--  2.0 unx      860 b- defN 23-Jun-02 14:23 test/test_user_brief.py
--rw-r--r--  2.0 unx      876 b- defN 23-Jun-02 14:23 test/test_user_profile.py
--rw-r--r--  2.0 unx      865 b- defN 23-Jun-02 14:23 test/test_users_api.py
--rw-r--r--  2.0 unx      950 b- defN 23-Jun-02 14:23 test/test_vagrant_package_upload.py
--rw-r--r--  2.0 unx     1008 b- defN 23-Jun-02 14:23 test/test_vagrant_package_upload_request.py
--rw-r--r--  2.0 unx     1487 b- defN 23-Jun-02 14:23 test/test_vulnerabilities_api.py
--rw-r--r--  2.0 unx      890 b- defN 23-Jun-02 14:23 test/test_vulnerability.py
--rw-r--r--  2.0 unx      924 b- defN 23-Jun-02 14:23 test/test_vulnerability_scan.py
--rw-r--r--  2.0 unx      982 b- defN 23-Jun-02 14:23 test/test_vulnerability_scan_results.py
--rw-r--r--  2.0 unx     1016 b- defN 23-Jun-02 14:23 test/test_vulnerability_scan_results_list.py
--rw-r--r--  2.0 unx      982 b- defN 23-Jun-02 14:23 test/test_vulnerability_scan_version.py
--rw-r--r--  2.0 unx      908 b- defN 23-Jun-02 14:23 test/test_webhook_template.py
--rw-r--r--  2.0 unx     1557 b- defN 23-Jun-02 14:23 test/test_webhooks_api.py
--rw-r--r--  2.0 unx      457 b- defN 23-Jun-02 14:24 cloudsmith_api-2.0.6.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Jun-02 14:24 cloudsmith_api-2.0.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       20 b- defN 23-Jun-02 14:24 cloudsmith_api-2.0.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    40280 b- defN 23-Jun-02 14:24 cloudsmith_api-2.0.6.dist-info/RECORD
-415 files, 4398931 bytes uncompressed, 669752 bytes compressed:  84.8%
+Zip file size: 878668 bytes, number of entries: 483
+-rw-r--r--  2.0 unx    18841 b- defN 23-Jun-29 15:39 cloudsmith_api/__init__.py
+-rw-r--r--  2.0 unx    25067 b- defN 23-Jun-29 15:39 cloudsmith_api/api_client.py
+-rw-r--r--  2.0 unx     8390 b- defN 23-Jun-29 15:39 cloudsmith_api/configuration.py
+-rw-r--r--  2.0 unx    13166 b- defN 23-Jun-29 15:39 cloudsmith_api/rest.py
+-rw-r--r--  2.0 unx     1131 b- defN 23-Jun-29 15:39 cloudsmith_api/api/__init__.py
+-rw-r--r--  2.0 unx    11039 b- defN 23-Jun-29 15:39 cloudsmith_api/api/audit_log_api.py
+-rw-r--r--  2.0 unx    11425 b- defN 23-Jun-29 15:39 cloudsmith_api/api/badges_api.py
+-rw-r--r--  2.0 unx     7978 b- defN 23-Jun-29 15:39 cloudsmith_api/api/distros_api.py
+-rw-r--r--  2.0 unx    54786 b- defN 23-Jun-29 15:39 cloudsmith_api/api/entitlements_api.py
+-rw-r--r--  2.0 unx    26620 b- defN 23-Jun-29 15:39 cloudsmith_api/api/files_api.py
+-rw-r--r--  2.0 unx     7930 b- defN 23-Jun-29 15:39 cloudsmith_api/api/formats_api.py
+-rw-r--r--  2.0 unx    19214 b- defN 23-Jun-29 15:39 cloudsmith_api/api/metrics_api.py
+-rw-r--r--  2.0 unx     8514 b- defN 23-Jun-29 15:39 cloudsmith_api/api/namespaces_api.py
+-rw-r--r--  2.0 unx   232571 b- defN 23-Jun-29 15:39 cloudsmith_api/api/orgs_api.py
+-rw-r--r--  2.0 unx   294424 b- defN 23-Jun-29 15:39 cloudsmith_api/api/packages_api.py
+-rw-r--r--  2.0 unx    16386 b- defN 23-Jun-29 15:39 cloudsmith_api/api/quota_api.py
+-rw-r--r--  2.0 unx     4157 b- defN 23-Jun-29 15:39 cloudsmith_api/api/rates_api.py
+-rw-r--r--  2.0 unx   418673 b- defN 23-Jun-29 15:39 cloudsmith_api/api/repos_api.py
+-rw-r--r--  2.0 unx     4118 b- defN 23-Jun-29 15:39 cloudsmith_api/api/status_api.py
+-rw-r--r--  2.0 unx     8075 b- defN 23-Jun-29 15:39 cloudsmith_api/api/storage_regions_api.py
+-rw-r--r--  2.0 unx     7631 b- defN 23-Jun-29 15:39 cloudsmith_api/api/user_api.py
+-rw-r--r--  2.0 unx     4706 b- defN 23-Jun-29 15:39 cloudsmith_api/api/users_api.py
+-rw-r--r--  2.0 unx    22091 b- defN 23-Jun-29 15:39 cloudsmith_api/api/vulnerabilities_api.py
+-rw-r--r--  2.0 unx    26050 b- defN 23-Jun-29 15:39 cloudsmith_api/api/webhooks_api.py
+-rw-r--r--  2.0 unx    17644 b- defN 23-Jun-29 15:39 cloudsmith_api/models/__init__.py
+-rw-r--r--  2.0 unx     7305 b- defN 23-Jun-29 15:39 cloudsmith_api/models/allocated_limit.py
+-rw-r--r--  2.0 unx     5410 b- defN 23-Jun-29 15:39 cloudsmith_api/models/allocated_limit_raw.py
+-rw-r--r--  2.0 unx    58771 b- defN 23-Jun-29 15:39 cloudsmith_api/models/alpine_package_upload.py
+-rw-r--r--  2.0 unx     7437 b- defN 23-Jun-29 15:39 cloudsmith_api/models/alpine_package_upload_request.py
+-rw-r--r--  2.0 unx     4748 b- defN 23-Jun-29 15:39 cloudsmith_api/models/architecture.py
+-rw-r--r--  2.0 unx    58494 b- defN 23-Jun-29 15:39 cloudsmith_api/models/cargo_package_upload.py
+-rw-r--r--  2.0 unx     6177 b- defN 23-Jun-29 15:39 cloudsmith_api/models/cargo_package_upload_request.py
+-rw-r--r--  2.0 unx    59602 b- defN 23-Jun-29 15:39 cloudsmith_api/models/cocoapods_package_upload.py
+-rw-r--r--  2.0 unx     6245 b- defN 23-Jun-29 15:39 cloudsmith_api/models/cocoapods_package_upload_request.py
+-rw-r--r--  2.0 unx     6052 b- defN 23-Jun-29 15:39 cloudsmith_api/models/common_bandwidth_metrics.py
+-rw-r--r--  2.0 unx     5636 b- defN 23-Jun-29 15:39 cloudsmith_api/models/common_bandwidth_metrics_value.py
+-rw-r--r--  2.0 unx     6052 b- defN 23-Jun-29 15:39 cloudsmith_api/models/common_downloads_metrics.py
+-rw-r--r--  2.0 unx     3526 b- defN 23-Jun-29 15:39 cloudsmith_api/models/common_downloads_metrics_value.py
+-rw-r--r--  2.0 unx     6129 b- defN 23-Jun-29 15:39 cloudsmith_api/models/common_metrics.py
+-rw-r--r--  2.0 unx    59325 b- defN 23-Jun-29 15:39 cloudsmith_api/models/composer_package_upload.py
+-rw-r--r--  2.0 unx     6228 b- defN 23-Jun-29 15:39 cloudsmith_api/models/composer_package_upload_request.py
+-rw-r--r--  2.0 unx    61539 b- defN 23-Jun-29 15:39 cloudsmith_api/models/conan_package_upload.py
+-rw-r--r--  2.0 unx    14491 b- defN 23-Jun-29 15:39 cloudsmith_api/models/conan_package_upload_request.py
+-rw-r--r--  2.0 unx    58494 b- defN 23-Jun-29 15:39 cloudsmith_api/models/conda_package_upload.py
+-rw-r--r--  2.0 unx     6177 b- defN 23-Jun-29 15:39 cloudsmith_api/models/conda_package_upload_request.py
+-rw-r--r--  2.0 unx    58217 b- defN 23-Jun-29 15:39 cloudsmith_api/models/cran_package_upload.py
+-rw-r--r--  2.0 unx     6160 b- defN 23-Jun-29 15:39 cloudsmith_api/models/cran_package_upload_request.py
+-rw-r--r--  2.0 unx    58217 b- defN 23-Jun-29 15:39 cloudsmith_api/models/dart_package_upload.py
+-rw-r--r--  2.0 unx     6160 b- defN 23-Jun-29 15:39 cloudsmith_api/models/dart_package_upload_request.py
+-rw-r--r--  2.0 unx    22261 b- defN 23-Jun-29 15:39 cloudsmith_api/models/dart_upstream.py
+-rw-r--r--  2.0 unx    20036 b- defN 23-Jun-29 15:39 cloudsmith_api/models/dart_upstream_request.py
+-rw-r--r--  2.0 unx    20053 b- defN 23-Jun-29 15:39 cloudsmith_api/models/dart_upstream_request_patch.py
+-rw-r--r--  2.0 unx    57940 b- defN 23-Jun-29 15:39 cloudsmith_api/models/deb_package_upload.py
+-rw-r--r--  2.0 unx     9690 b- defN 23-Jun-29 15:39 cloudsmith_api/models/deb_package_upload_request.py
+-rw-r--r--  2.0 unx    26959 b- defN 23-Jun-29 15:39 cloudsmith_api/models/deb_upstream.py
+-rw-r--r--  2.0 unx    24858 b- defN 23-Jun-29 15:39 cloudsmith_api/models/deb_upstream_request.py
+-rw-r--r--  2.0 unx    24814 b- defN 23-Jun-29 15:39 cloudsmith_api/models/deb_upstream_request_patch.py
+-rw-r--r--  2.0 unx     6159 b- defN 23-Jun-29 15:39 cloudsmith_api/models/distribution.py
+-rw-r--r--  2.0 unx     8542 b- defN 23-Jun-29 15:39 cloudsmith_api/models/distribution_full.py
+-rw-r--r--  2.0 unx     4497 b- defN 23-Jun-29 15:39 cloudsmith_api/models/distribution_version.py
+-rw-r--r--  2.0 unx    58771 b- defN 23-Jun-29 15:39 cloudsmith_api/models/docker_package_upload.py
+-rw-r--r--  2.0 unx     6194 b- defN 23-Jun-29 15:39 cloudsmith_api/models/docker_package_upload_request.py
+-rw-r--r--  2.0 unx    22418 b- defN 23-Jun-29 15:39 cloudsmith_api/models/docker_upstream.py
+-rw-r--r--  2.0 unx    20169 b- defN 23-Jun-29 15:39 cloudsmith_api/models/docker_upstream_request.py
+-rw-r--r--  2.0 unx    20186 b- defN 23-Jun-29 15:39 cloudsmith_api/models/docker_upstream_request_patch.py
+-rw-r--r--  2.0 unx     3541 b- defN 23-Jun-29 15:39 cloudsmith_api/models/entitlement_usage_metrics.py
+-rw-r--r--  2.0 unx     3729 b- defN 23-Jun-29 15:39 cloudsmith_api/models/error_detail.py
+-rw-r--r--  2.0 unx     5458 b- defN 23-Jun-29 15:39 cloudsmith_api/models/eula.py
+-rw-r--r--  2.0 unx    11287 b- defN 23-Jun-29 15:39 cloudsmith_api/models/format.py
+-rw-r--r--  2.0 unx     7319 b- defN 23-Jun-29 15:39 cloudsmith_api/models/format_support.py
+-rw-r--r--  2.0 unx     8615 b- defN 23-Jun-29 15:39 cloudsmith_api/models/geo_ip_location.py
+-rw-r--r--  2.0 unx    57663 b- defN 23-Jun-29 15:39 cloudsmith_api/models/go_package_upload.py
+-rw-r--r--  2.0 unx     6126 b- defN 23-Jun-29 15:39 cloudsmith_api/models/go_package_upload_request.py
+-rw-r--r--  2.0 unx    58217 b- defN 23-Jun-29 15:39 cloudsmith_api/models/helm_package_upload.py
+-rw-r--r--  2.0 unx     7480 b- defN 23-Jun-29 15:39 cloudsmith_api/models/helm_package_upload_request.py
+-rw-r--r--  2.0 unx    22280 b- defN 23-Jun-29 15:39 cloudsmith_api/models/helm_upstream.py
+-rw-r--r--  2.0 unx    20055 b- defN 23-Jun-29 15:39 cloudsmith_api/models/helm_upstream_request.py
+-rw-r--r--  2.0 unx    20072 b- defN 23-Jun-29 15:39 cloudsmith_api/models/helm_upstream_request_patch.py
+-rw-r--r--  2.0 unx    57940 b- defN 23-Jun-29 15:39 cloudsmith_api/models/hex_package_upload.py
+-rw-r--r--  2.0 unx     6143 b- defN 23-Jun-29 15:39 cloudsmith_api/models/hex_package_upload_request.py
+-rw-r--r--  2.0 unx     7028 b- defN 23-Jun-29 15:39 cloudsmith_api/models/history.py
+-rw-r--r--  2.0 unx     5168 b- defN 23-Jun-29 15:39 cloudsmith_api/models/history_fieldset.py
+-rw-r--r--  2.0 unx     5246 b- defN 23-Jun-29 15:39 cloudsmith_api/models/history_fieldset_raw.py
+-rw-r--r--  2.0 unx    59325 b- defN 23-Jun-29 15:39 cloudsmith_api/models/luarocks_package_upload.py
+-rw-r--r--  2.0 unx     6228 b- defN 23-Jun-29 15:39 cloudsmith_api/models/luarocks_package_upload_request.py
+-rw-r--r--  2.0 unx    63607 b- defN 23-Jun-29 15:39 cloudsmith_api/models/maven_package_upload.py
+-rw-r--r--  2.0 unx    17576 b- defN 23-Jun-29 15:39 cloudsmith_api/models/maven_package_upload_request.py
+-rw-r--r--  2.0 unx    22363 b- defN 23-Jun-29 15:39 cloudsmith_api/models/maven_upstream.py
+-rw-r--r--  2.0 unx    20126 b- defN 23-Jun-29 15:39 cloudsmith_api/models/maven_upstream_request.py
+-rw-r--r--  2.0 unx    20143 b- defN 23-Jun-29 15:39 cloudsmith_api/models/maven_upstream_request_patch.py
+-rw-r--r--  2.0 unx     5806 b- defN 23-Jun-29 15:39 cloudsmith_api/models/namespace.py
+-rw-r--r--  2.0 unx    18223 b- defN 23-Jun-29 15:39 cloudsmith_api/models/namespace_audit_log.py
+-rw-r--r--  2.0 unx    11620 b- defN 23-Jun-29 15:39 cloudsmith_api/models/nested_license_policy.py
+-rw-r--r--  2.0 unx    12280 b- defN 23-Jun-29 15:39 cloudsmith_api/models/nested_vulnerability_policy.py
+-rw-r--r--  2.0 unx     9527 b- defN 23-Jun-29 15:39 cloudsmith_api/models/nested_vulnerability_scan_results.py
+-rw-r--r--  2.0 unx    57940 b- defN 23-Jun-29 15:39 cloudsmith_api/models/npm_package_upload.py
+-rw-r--r--  2.0 unx     7663 b- defN 23-Jun-29 15:39 cloudsmith_api/models/npm_package_upload_request.py
+-rw-r--r--  2.0 unx    22220 b- defN 23-Jun-29 15:39 cloudsmith_api/models/npm_upstream.py
+-rw-r--r--  2.0 unx    20007 b- defN 23-Jun-29 15:39 cloudsmith_api/models/npm_upstream_request.py
+-rw-r--r--  2.0 unx    20024 b- defN 23-Jun-29 15:39 cloudsmith_api/models/npm_upstream_request_patch.py
+-rw-r--r--  2.0 unx    58494 b- defN 23-Jun-29 15:39 cloudsmith_api/models/nuget_package_upload.py
+-rw-r--r--  2.0 unx     7272 b- defN 23-Jun-29 15:39 cloudsmith_api/models/nuget_package_upload_request.py
+-rw-r--r--  2.0 unx    22349 b- defN 23-Jun-29 15:39 cloudsmith_api/models/nuget_upstream.py
+-rw-r--r--  2.0 unx    20112 b- defN 23-Jun-29 15:39 cloudsmith_api/models/nuget_upstream_request.py
+-rw-r--r--  2.0 unx    20129 b- defN 23-Jun-29 15:39 cloudsmith_api/models/nuget_upstream_request_patch.py
+-rw-r--r--  2.0 unx     7918 b- defN 23-Jun-29 15:39 cloudsmith_api/models/organization.py
+-rw-r--r--  2.0 unx     8391 b- defN 23-Jun-29 15:39 cloudsmith_api/models/organization_group_sync.py
+-rw-r--r--  2.0 unx     8223 b- defN 23-Jun-29 15:39 cloudsmith_api/models/organization_group_sync_request.py
+-rw-r--r--  2.0 unx    10169 b- defN 23-Jun-29 15:39 cloudsmith_api/models/organization_invite.py
+-rw-r--r--  2.0 unx    10519 b- defN 23-Jun-29 15:39 cloudsmith_api/models/organization_invite_extend.py
+-rw-r--r--  2.0 unx     5661 b- defN 23-Jun-29 15:39 cloudsmith_api/models/organization_invite_request.py
+-rw-r--r--  2.0 unx     3821 b- defN 23-Jun-29 15:39 cloudsmith_api/models/organization_invite_update.py
+-rw-r--r--  2.0 unx     3929 b- defN 23-Jun-29 15:39 cloudsmith_api/models/organization_invite_update_request_patch.py
+-rw-r--r--  2.0 unx    12300 b- defN 23-Jun-29 15:39 cloudsmith_api/models/organization_membership.py
+-rw-r--r--  2.0 unx    12219 b- defN 23-Jun-29 15:39 cloudsmith_api/models/organization_package_license_policy.py
+-rw-r--r--  2.0 unx     9666 b- defN 23-Jun-29 15:39 cloudsmith_api/models/organization_package_license_policy_request.py
+-rw-r--r--  2.0 unx     9539 b- defN 23-Jun-29 15:39 cloudsmith_api/models/organization_package_license_policy_request_patch.py
+-rw-r--r--  2.0 unx    12855 b- defN 23-Jun-29 15:39 cloudsmith_api/models/organization_package_vulnerability_policy.py
+-rw-r--r--  2.0 unx    10230 b- defN 23-Jun-29 15:39 cloudsmith_api/models/organization_package_vulnerability_policy_request.py
+-rw-r--r--  2.0 unx    10245 b- defN 23-Jun-29 15:39 cloudsmith_api/models/organization_package_vulnerability_policy_request_patch.py
+-rw-r--r--  2.0 unx     8110 b- defN 23-Jun-29 15:39 cloudsmith_api/models/organization_team.py
+-rw-r--r--  2.0 unx     3669 b- defN 23-Jun-29 15:39 cloudsmith_api/models/organization_team_members.py
+-rw-r--r--  2.0 unx     4783 b- defN 23-Jun-29 15:39 cloudsmith_api/models/organization_team_membership.py
+-rw-r--r--  2.0 unx     7065 b- defN 23-Jun-29 15:39 cloudsmith_api/models/organization_team_request.py
+-rw-r--r--  2.0 unx     7040 b- defN 23-Jun-29 15:39 cloudsmith_api/models/organization_team_request_patch.py
+-rw-r--r--  2.0 unx    57663 b- defN 23-Jun-29 15:39 cloudsmith_api/models/p2_package_upload.py
+-rw-r--r--  2.0 unx     6126 b- defN 23-Jun-29 15:39 cloudsmith_api/models/p2_package_upload_request.py
+-rw-r--r--  2.0 unx    55965 b- defN 23-Jun-29 15:39 cloudsmith_api/models/package.py
+-rw-r--r--  2.0 unx    57197 b- defN 23-Jun-29 15:39 cloudsmith_api/models/package_copy.py
+-rw-r--r--  2.0 unx     4776 b- defN 23-Jun-29 15:39 cloudsmith_api/models/package_copy_request.py
+-rw-r--r--  2.0 unx     3523 b- defN 23-Jun-29 15:39 cloudsmith_api/models/package_dependencies.py
+-rw-r--r--  2.0 unx     7227 b- defN 23-Jun-29 15:39 cloudsmith_api/models/package_dependency.py
+-rw-r--r--  2.0 unx    12968 b- defN 23-Jun-29 15:39 cloudsmith_api/models/package_file.py
+-rw-r--r--  2.0 unx     6108 b- defN 23-Jun-29 15:39 cloudsmith_api/models/package_file_parts_upload.py
+-rw-r--r--  2.0 unx     7841 b- defN 23-Jun-29 15:39 cloudsmith_api/models/package_file_upload.py
+-rw-r--r--  2.0 unx     7815 b- defN 23-Jun-29 15:39 cloudsmith_api/models/package_file_upload_request.py
+-rw-r--r--  2.0 unx     9164 b- defN 23-Jun-29 15:39 cloudsmith_api/models/package_license_policy_evaluation_request.py
+-rw-r--r--  2.0 unx     2865 b- defN 23-Jun-29 15:39 cloudsmith_api/models/package_license_policy_evaluation_request_request.py
+-rw-r--r--  2.0 unx     6035 b- defN 23-Jun-29 15:39 cloudsmith_api/models/package_license_policy_violation_log.py
+-rw-r--r--  2.0 unx     5198 b- defN 23-Jun-29 15:39 cloudsmith_api/models/package_license_policy_violation_log_cursor_page.py
+-rw-r--r--  2.0 unx    57195 b- defN 23-Jun-29 15:39 cloudsmith_api/models/package_move.py
+-rw-r--r--  2.0 unx     3820 b- defN 23-Jun-29 15:39 cloudsmith_api/models/package_move_request.py
+-rw-r--r--  2.0 unx    58775 b- defN 23-Jun-29 15:39 cloudsmith_api/models/package_quarantine.py
+-rw-r--r--  2.0 unx     3527 b- defN 23-Jun-29 15:39 cloudsmith_api/models/package_quarantine_request.py
+-rw-r--r--  2.0 unx    57651 b- defN 23-Jun-29 15:39 cloudsmith_api/models/package_resync.py
+-rw-r--r--  2.0 unx    15877 b- defN 23-Jun-29 15:39 cloudsmith_api/models/package_status.py
+-rw-r--r--  2.0 unx    57199 b- defN 23-Jun-29 15:39 cloudsmith_api/models/package_tag.py
+-rw-r--r--  2.0 unx     5352 b- defN 23-Jun-29 15:39 cloudsmith_api/models/package_tag_request.py
+-rw-r--r--  2.0 unx     3547 b- defN 23-Jun-29 15:39 cloudsmith_api/models/package_usage_metrics.py
+-rw-r--r--  2.0 unx     2740 b- defN 23-Jun-29 15:39 cloudsmith_api/models/package_version_badge.py
+-rw-r--r--  2.0 unx     5707 b- defN 23-Jun-29 15:39 cloudsmith_api/models/package_vulnerability.py
+-rw-r--r--  2.0 unx     9380 b- defN 23-Jun-29 15:39 cloudsmith_api/models/package_vulnerability_policy_evaluation_request.py
+-rw-r--r--  2.0 unx     2895 b- defN 23-Jun-29 15:39 cloudsmith_api/models/package_vulnerability_policy_evaluation_request_request.py
+-rw-r--r--  2.0 unx     7491 b- defN 23-Jun-29 15:39 cloudsmith_api/models/package_vulnerability_policy_violation_log.py
+-rw-r--r--  2.0 unx     5318 b- defN 23-Jun-29 15:39 cloudsmith_api/models/package_vulnerability_policy_violation_log_cursor_page.py
+-rw-r--r--  2.0 unx    58771 b- defN 23-Jun-29 15:39 cloudsmith_api/models/python_package_upload.py
+-rw-r--r--  2.0 unx     6194 b- defN 23-Jun-29 15:39 cloudsmith_api/models/python_package_upload_request.py
+-rw-r--r--  2.0 unx    22418 b- defN 23-Jun-29 15:39 cloudsmith_api/models/python_upstream.py
+-rw-r--r--  2.0 unx    20169 b- defN 23-Jun-29 15:39 cloudsmith_api/models/python_upstream_request.py
+-rw-r--r--  2.0 unx    20186 b- defN 23-Jun-29 15:39 cloudsmith_api/models/python_upstream_request_patch.py
+-rw-r--r--  2.0 unx     3358 b- defN 23-Jun-29 15:39 cloudsmith_api/models/quota.py
+-rw-r--r--  2.0 unx     3463 b- defN 23-Jun-29 15:39 cloudsmith_api/models/quota_history.py
+-rw-r--r--  2.0 unx     7675 b- defN 23-Jun-29 15:39 cloudsmith_api/models/rate_check.py
+-rw-r--r--  2.0 unx    58899 b- defN 23-Jun-29 15:39 cloudsmith_api/models/raw_package_upload.py
+-rw-r--r--  2.0 unx    11674 b- defN 23-Jun-29 15:39 cloudsmith_api/models/raw_package_upload_request.py
+-rw-r--r--  2.0 unx    66229 b- defN 23-Jun-29 15:39 cloudsmith_api/models/repository.py
+-rw-r--r--  2.0 unx    14861 b- defN 23-Jun-29 15:39 cloudsmith_api/models/repository_audit_log.py
+-rw-r--r--  2.0 unx    67555 b- defN 23-Jun-29 15:39 cloudsmith_api/models/repository_create.py
+-rw-r--r--  2.0 unx    52996 b- defN 23-Jun-29 15:39 cloudsmith_api/models/repository_create_request.py
+-rw-r--r--  2.0 unx     4365 b- defN 23-Jun-29 15:39 cloudsmith_api/models/repository_geo_ip_cidr.py
+-rw-r--r--  2.0 unx     4488 b- defN 23-Jun-29 15:39 cloudsmith_api/models/repository_geo_ip_country_code.py
+-rw-r--r--  2.0 unx     4424 b- defN 23-Jun-29 15:39 cloudsmith_api/models/repository_geo_ip_rules.py
+-rw-r--r--  2.0 unx     4515 b- defN 23-Jun-29 15:39 cloudsmith_api/models/repository_geo_ip_rules_request.py
+-rw-r--r--  2.0 unx     4312 b- defN 23-Jun-29 15:39 cloudsmith_api/models/repository_geo_ip_rules_request_patch.py
+-rw-r--r--  2.0 unx     3733 b- defN 23-Jun-29 15:39 cloudsmith_api/models/repository_geo_ip_test_address.py
+-rw-r--r--  2.0 unx     3906 b- defN 23-Jun-29 15:39 cloudsmith_api/models/repository_geo_ip_test_address_response.py
+-rw-r--r--  2.0 unx     7359 b- defN 23-Jun-29 15:39 cloudsmith_api/models/repository_geo_ip_test_address_response_dict.py
+-rw-r--r--  2.0 unx     8734 b- defN 23-Jun-29 15:39 cloudsmith_api/models/repository_gpg_key.py
+-rw-r--r--  2.0 unx     5133 b- defN 23-Jun-29 15:39 cloudsmith_api/models/repository_gpg_key_create.py
+-rw-r--r--  2.0 unx     7702 b- defN 23-Jun-29 15:39 cloudsmith_api/models/repository_privilege_dict.py
+-rw-r--r--  2.0 unx     3818 b- defN 23-Jun-29 15:39 cloudsmith_api/models/repository_privilege_input.py
+-rw-r--r--  2.0 unx     3881 b- defN 23-Jun-29 15:39 cloudsmith_api/models/repository_privilege_input_request.py
+-rw-r--r--  2.0 unx     3790 b- defN 23-Jun-29 15:39 cloudsmith_api/models/repository_privilege_input_request_patch.py
+-rw-r--r--  2.0 unx    51807 b- defN 23-Jun-29 15:39 cloudsmith_api/models/repository_request_patch.py
+-rw-r--r--  2.0 unx     7753 b- defN 23-Jun-29 15:39 cloudsmith_api/models/repository_rsa_key.py
+-rw-r--r--  2.0 unx     5133 b- defN 23-Jun-29 15:39 cloudsmith_api/models/repository_rsa_key_create.py
+-rw-r--r--  2.0 unx    40544 b- defN 23-Jun-29 15:39 cloudsmith_api/models/repository_token.py
+-rw-r--r--  2.0 unx     2750 b- defN 23-Jun-29 15:39 cloudsmith_api/models/repository_token_action.py
+-rw-r--r--  2.0 unx    41541 b- defN 23-Jun-29 15:39 cloudsmith_api/models/repository_token_refresh.py
+-rw-r--r--  2.0 unx    21868 b- defN 23-Jun-29 15:39 cloudsmith_api/models/repository_token_refresh_request.py
+-rw-r--r--  2.0 unx    22374 b- defN 23-Jun-29 15:39 cloudsmith_api/models/repository_token_request.py
+-rw-r--r--  2.0 unx    22569 b- defN 23-Jun-29 15:39 cloudsmith_api/models/repository_token_request_patch.py
+-rw-r--r--  2.0 unx     3505 b- defN 23-Jun-29 15:39 cloudsmith_api/models/repository_token_sync.py
+-rw-r--r--  2.0 unx     3904 b- defN 23-Jun-29 15:39 cloudsmith_api/models/repository_token_sync_request.py
+-rw-r--r--  2.0 unx    30728 b- defN 23-Jun-29 15:39 cloudsmith_api/models/repository_webhook.py
+-rw-r--r--  2.0 unx    18912 b- defN 23-Jun-29 15:39 cloudsmith_api/models/repository_webhook_request.py
+-rw-r--r--  2.0 unx    18774 b- defN 23-Jun-29 15:39 cloudsmith_api/models/repository_webhook_request_patch.py
+-rw-r--r--  2.0 unx     3523 b- defN 23-Jun-29 15:39 cloudsmith_api/models/resources_rate_check.py
+-rw-r--r--  2.0 unx     2790 b- defN 23-Jun-29 15:39 cloudsmith_api/models/respository_geo_ip_enable_disable.py
+-rw-r--r--  2.0 unx     2825 b- defN 23-Jun-29 15:39 cloudsmith_api/models/respository_geo_ip_enable_disable_request.py
+-rw-r--r--  2.0 unx    57940 b- defN 23-Jun-29 15:39 cloudsmith_api/models/rpm_package_upload.py
+-rw-r--r--  2.0 unx     7374 b- defN 23-Jun-29 15:39 cloudsmith_api/models/rpm_package_upload_request.py
+-rw-r--r--  2.0 unx    24178 b- defN 23-Jun-29 15:39 cloudsmith_api/models/rpm_upstream.py
+-rw-r--r--  2.0 unx    22021 b- defN 23-Jun-29 15:39 cloudsmith_api/models/rpm_upstream_request.py
+-rw-r--r--  2.0 unx    21938 b- defN 23-Jun-29 15:39 cloudsmith_api/models/rpm_upstream_request_patch.py
+-rw-r--r--  2.0 unx    58217 b- defN 23-Jun-29 15:39 cloudsmith_api/models/ruby_package_upload.py
+-rw-r--r--  2.0 unx     6160 b- defN 23-Jun-29 15:39 cloudsmith_api/models/ruby_package_upload_request.py
+-rw-r--r--  2.0 unx    22280 b- defN 23-Jun-29 15:39 cloudsmith_api/models/ruby_upstream.py
+-rw-r--r--  2.0 unx    20055 b- defN 23-Jun-29 15:39 cloudsmith_api/models/ruby_upstream_request.py
+-rw-r--r--  2.0 unx    20072 b- defN 23-Jun-29 15:39 cloudsmith_api/models/ruby_upstream_request_patch.py
+-rw-r--r--  2.0 unx     8234 b- defN 23-Jun-29 15:39 cloudsmith_api/models/service.py
+-rw-r--r--  2.0 unx     6726 b- defN 23-Jun-29 15:39 cloudsmith_api/models/service_request.py
+-rw-r--r--  2.0 unx     6701 b- defN 23-Jun-29 15:39 cloudsmith_api/models/service_request_patch.py
+-rw-r--r--  2.0 unx     4951 b- defN 23-Jun-29 15:39 cloudsmith_api/models/service_teams.py
+-rw-r--r--  2.0 unx     4584 b- defN 23-Jun-29 15:39 cloudsmith_api/models/status_basic.py
+-rw-r--r--  2.0 unx     8478 b- defN 23-Jun-29 15:39 cloudsmith_api/models/storage_allocated_limit.py
+-rw-r--r--  2.0 unx     6140 b- defN 23-Jun-29 15:39 cloudsmith_api/models/storage_allocated_limit_raw.py
+-rw-r--r--  2.0 unx     4670 b- defN 23-Jun-29 15:39 cloudsmith_api/models/storage_region.py
+-rw-r--r--  2.0 unx     6847 b- defN 23-Jun-29 15:39 cloudsmith_api/models/storage_usage.py
+-rw-r--r--  2.0 unx     5048 b- defN 23-Jun-29 15:39 cloudsmith_api/models/storage_usage_raw.py
+-rw-r--r--  2.0 unx    58865 b- defN 23-Jun-29 15:39 cloudsmith_api/models/swift_package_upload.py
+-rw-r--r--  2.0 unx     7279 b- defN 23-Jun-29 15:39 cloudsmith_api/models/swift_package_upload_request.py
+-rw-r--r--  2.0 unx     2665 b- defN 23-Jun-29 15:39 cloudsmith_api/models/tags.py
+-rw-r--r--  2.0 unx    59602 b- defN 23-Jun-29 15:39 cloudsmith_api/models/terraform_package_upload.py
+-rw-r--r--  2.0 unx     6245 b- defN 23-Jun-29 15:39 cloudsmith_api/models/terraform_package_upload_request.py
+-rw-r--r--  2.0 unx     5738 b- defN 23-Jun-29 15:39 cloudsmith_api/models/usage.py
+-rw-r--r--  2.0 unx     4147 b- defN 23-Jun-29 15:39 cloudsmith_api/models/usage_fieldset.py
+-rw-r--r--  2.0 unx     4277 b- defN 23-Jun-29 15:39 cloudsmith_api/models/usage_limits.py
+-rw-r--r--  2.0 unx     4334 b- defN 23-Jun-29 15:39 cloudsmith_api/models/usage_limits_raw.py
+-rw-r--r--  2.0 unx     4382 b- defN 23-Jun-29 15:39 cloudsmith_api/models/usage_raw.py
+-rw-r--r--  2.0 unx     3590 b- defN 23-Jun-29 15:39 cloudsmith_api/models/user_auth_token.py
+-rw-r--r--  2.0 unx     4612 b- defN 23-Jun-29 15:39 cloudsmith_api/models/user_auth_token_request.py
+-rw-r--r--  2.0 unx     8019 b- defN 23-Jun-29 15:39 cloudsmith_api/models/user_brief.py
+-rw-r--r--  2.0 unx    11110 b- defN 23-Jun-29 15:39 cloudsmith_api/models/user_profile.py
+-rw-r--r--  2.0 unx    60899 b- defN 23-Jun-29 15:39 cloudsmith_api/models/vagrant_package_upload.py
+-rw-r--r--  2.0 unx     9492 b- defN 23-Jun-29 15:39 cloudsmith_api/models/vagrant_package_upload_request.py
+-rw-r--r--  2.0 unx    13112 b- defN 23-Jun-29 15:39 cloudsmith_api/models/vulnerability.py
+-rw-r--r--  2.0 unx     5400 b- defN 23-Jun-29 15:39 cloudsmith_api/models/vulnerability_scan.py
+-rw-r--r--  2.0 unx    10348 b- defN 23-Jun-29 15:39 cloudsmith_api/models/vulnerability_scan_results.py
+-rw-r--r--  2.0 unx     9725 b- defN 23-Jun-29 15:39 cloudsmith_api/models/vulnerability_scan_results_list.py
+-rw-r--r--  2.0 unx     8445 b- defN 23-Jun-29 15:39 cloudsmith_api/models/vulnerability_scan_version.py
+-rw-r--r--  2.0 unx     4751 b- defN 23-Jun-29 15:39 cloudsmith_api/models/webhook_template.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-29 15:39 test/__init__.py
+-rw-r--r--  2.0 unx      900 b- defN 23-Jun-29 15:39 test/test_allocated_limit.py
+-rw-r--r--  2.0 unx      926 b- defN 23-Jun-29 15:39 test/test_allocated_limit_raw.py
+-rw-r--r--  2.0 unx      942 b- defN 23-Jun-29 15:39 test/test_alpine_package_upload.py
+-rw-r--r--  2.0 unx     1000 b- defN 23-Jun-29 15:39 test/test_alpine_package_upload_request.py
+-rw-r--r--  2.0 unx      882 b- defN 23-Jun-29 15:39 test/test_architecture.py
+-rw-r--r--  2.0 unx     1083 b- defN 23-Jun-29 15:39 test/test_audit_log_api.py
+-rw-r--r--  2.0 unx      883 b- defN 23-Jun-29 15:39 test/test_badges_api.py
+-rw-r--r--  2.0 unx      934 b- defN 23-Jun-29 15:39 test/test_cargo_package_upload.py
+-rw-r--r--  2.0 unx      992 b- defN 23-Jun-29 15:39 test/test_cargo_package_upload_request.py
+-rw-r--r--  2.0 unx      966 b- defN 23-Jun-29 15:39 test/test_cocoapods_package_upload.py
+-rw-r--r--  2.0 unx     1024 b- defN 23-Jun-29 15:39 test/test_cocoapods_package_upload_request.py
+-rw-r--r--  2.0 unx      966 b- defN 23-Jun-29 15:39 test/test_common_bandwidth_metrics.py
+-rw-r--r--  2.0 unx     1008 b- defN 23-Jun-29 15:39 test/test_common_bandwidth_metrics_value.py
+-rw-r--r--  2.0 unx      966 b- defN 23-Jun-29 15:39 test/test_common_downloads_metrics.py
+-rw-r--r--  2.0 unx     1008 b- defN 23-Jun-29 15:39 test/test_common_downloads_metrics_value.py
+-rw-r--r--  2.0 unx      892 b- defN 23-Jun-29 15:39 test/test_common_metrics.py
+-rw-r--r--  2.0 unx      958 b- defN 23-Jun-29 15:39 test/test_composer_package_upload.py
+-rw-r--r--  2.0 unx     1016 b- defN 23-Jun-29 15:39 test/test_composer_package_upload_request.py
+-rw-r--r--  2.0 unx      934 b- defN 23-Jun-29 15:39 test/test_conan_package_upload.py
+-rw-r--r--  2.0 unx      992 b- defN 23-Jun-29 15:39 test/test_conan_package_upload_request.py
+-rw-r--r--  2.0 unx      934 b- defN 23-Jun-29 15:39 test/test_conda_package_upload.py
+-rw-r--r--  2.0 unx      992 b- defN 23-Jun-29 15:39 test/test_conda_package_upload_request.py
+-rw-r--r--  2.0 unx      926 b- defN 23-Jun-29 15:39 test/test_cran_package_upload.py
+-rw-r--r--  2.0 unx      984 b- defN 23-Jun-29 15:39 test/test_cran_package_upload_request.py
+-rw-r--r--  2.0 unx      926 b- defN 23-Jun-29 15:39 test/test_dart_package_upload.py
+-rw-r--r--  2.0 unx      984 b- defN 23-Jun-29 15:39 test/test_dart_package_upload_request.py
+-rw-r--r--  2.0 unx      884 b- defN 23-Jun-29 15:39 test/test_dart_upstream.py
+-rw-r--r--  2.0 unx      942 b- defN 23-Jun-29 15:39 test/test_dart_upstream_request.py
+-rw-r--r--  2.0 unx      984 b- defN 23-Jun-29 15:39 test/test_dart_upstream_request_patch.py
+-rw-r--r--  2.0 unx      918 b- defN 23-Jun-29 15:39 test/test_deb_package_upload.py
+-rw-r--r--  2.0 unx      976 b- defN 23-Jun-29 15:39 test/test_deb_package_upload_request.py
+-rw-r--r--  2.0 unx      876 b- defN 23-Jun-29 15:39 test/test_deb_upstream.py
+-rw-r--r--  2.0 unx      934 b- defN 23-Jun-29 15:39 test/test_deb_upstream_request.py
+-rw-r--r--  2.0 unx      976 b- defN 23-Jun-29 15:39 test/test_deb_upstream_request_patch.py
+-rw-r--r--  2.0 unx      882 b- defN 23-Jun-29 15:39 test/test_distribution.py
+-rw-r--r--  2.0 unx      916 b- defN 23-Jun-29 15:39 test/test_distribution_full.py
+-rw-r--r--  2.0 unx      940 b- defN 23-Jun-29 15:39 test/test_distribution_version.py
+-rw-r--r--  2.0 unx     1019 b- defN 23-Jun-29 15:39 test/test_distros_api.py
+-rw-r--r--  2.0 unx      942 b- defN 23-Jun-29 15:39 test/test_docker_package_upload.py
+-rw-r--r--  2.0 unx     1000 b- defN 23-Jun-29 15:39 test/test_docker_package_upload_request.py
+-rw-r--r--  2.0 unx      900 b- defN 23-Jun-29 15:39 test/test_docker_upstream.py
+-rw-r--r--  2.0 unx      958 b- defN 23-Jun-29 15:39 test/test_docker_upstream_request.py
+-rw-r--r--  2.0 unx     1000 b- defN 23-Jun-29 15:39 test/test_docker_upstream_request_patch.py
+-rw-r--r--  2.0 unx      974 b- defN 23-Jun-29 15:39 test/test_entitlement_usage_metrics.py
+-rw-r--r--  2.0 unx     2550 b- defN 23-Jun-29 15:39 test/test_entitlements_api.py
+-rw-r--r--  2.0 unx      876 b- defN 23-Jun-29 15:39 test/test_error_detail.py
+-rw-r--r--  2.0 unx      818 b- defN 23-Jun-29 15:39 test/test_eula.py
+-rw-r--r--  2.0 unx     1503 b- defN 23-Jun-29 15:39 test/test_files_api.py
+-rw-r--r--  2.0 unx      834 b- defN 23-Jun-29 15:39 test/test_format.py
+-rw-r--r--  2.0 unx      892 b- defN 23-Jun-29 15:39 test/test_format_support.py
+-rw-r--r--  2.0 unx     1022 b- defN 23-Jun-29 15:39 test/test_formats_api.py
+-rw-r--r--  2.0 unx      894 b- defN 23-Jun-29 15:39 test/test_geo_ip_location.py
+-rw-r--r--  2.0 unx      910 b- defN 23-Jun-29 15:39 test/test_go_package_upload.py
+-rw-r--r--  2.0 unx      968 b- defN 23-Jun-29 15:39 test/test_go_package_upload_request.py
+-rw-r--r--  2.0 unx      926 b- defN 23-Jun-29 15:39 test/test_helm_package_upload.py
+-rw-r--r--  2.0 unx      984 b- defN 23-Jun-29 15:39 test/test_helm_package_upload_request.py
+-rw-r--r--  2.0 unx      884 b- defN 23-Jun-29 15:39 test/test_helm_upstream.py
+-rw-r--r--  2.0 unx      942 b- defN 23-Jun-29 15:39 test/test_helm_upstream_request.py
+-rw-r--r--  2.0 unx      984 b- defN 23-Jun-29 15:39 test/test_helm_upstream_request_patch.py
+-rw-r--r--  2.0 unx      918 b- defN 23-Jun-29 15:39 test/test_hex_package_upload.py
+-rw-r--r--  2.0 unx      976 b- defN 23-Jun-29 15:39 test/test_hex_package_upload_request.py
+-rw-r--r--  2.0 unx      842 b- defN 23-Jun-29 15:39 test/test_history.py
+-rw-r--r--  2.0 unx      908 b- defN 23-Jun-29 15:39 test/test_history_fieldset.py
+-rw-r--r--  2.0 unx      934 b- defN 23-Jun-29 15:39 test/test_history_fieldset_raw.py
+-rw-r--r--  2.0 unx      958 b- defN 23-Jun-29 15:39 test/test_luarocks_package_upload.py
+-rw-r--r--  2.0 unx     1016 b- defN 23-Jun-29 15:39 test/test_luarocks_package_upload_request.py
+-rw-r--r--  2.0 unx      934 b- defN 23-Jun-29 15:39 test/test_maven_package_upload.py
+-rw-r--r--  2.0 unx      992 b- defN 23-Jun-29 15:39 test/test_maven_package_upload_request.py
+-rw-r--r--  2.0 unx      892 b- defN 23-Jun-29 15:39 test/test_maven_upstream.py
+-rw-r--r--  2.0 unx      950 b- defN 23-Jun-29 15:39 test/test_maven_upstream_request.py
+-rw-r--r--  2.0 unx      992 b- defN 23-Jun-29 15:39 test/test_maven_upstream_request_patch.py
+-rw-r--r--  2.0 unx     1335 b- defN 23-Jun-29 15:39 test/test_metrics_api.py
+-rw-r--r--  2.0 unx      858 b- defN 23-Jun-29 15:39 test/test_namespace.py
+-rw-r--r--  2.0 unx      926 b- defN 23-Jun-29 15:39 test/test_namespace_audit_log.py
+-rw-r--r--  2.0 unx     1051 b- defN 23-Jun-29 15:39 test/test_namespaces_api.py
+-rw-r--r--  2.0 unx      942 b- defN 23-Jun-29 15:39 test/test_nested_license_policy.py
+-rw-r--r--  2.0 unx      990 b- defN 23-Jun-29 15:39 test/test_nested_vulnerability_policy.py
+-rw-r--r--  2.0 unx     1032 b- defN 23-Jun-29 15:39 test/test_nested_vulnerability_scan_results.py
+-rw-r--r--  2.0 unx      918 b- defN 23-Jun-29 15:39 test/test_npm_package_upload.py
+-rw-r--r--  2.0 unx      976 b- defN 23-Jun-29 15:39 test/test_npm_package_upload_request.py
+-rw-r--r--  2.0 unx      876 b- defN 23-Jun-29 15:39 test/test_npm_upstream.py
+-rw-r--r--  2.0 unx      934 b- defN 23-Jun-29 15:39 test/test_npm_upstream_request.py
+-rw-r--r--  2.0 unx      976 b- defN 23-Jun-29 15:39 test/test_npm_upstream_request_patch.py
+-rw-r--r--  2.0 unx      934 b- defN 23-Jun-29 15:39 test/test_nuget_package_upload.py
+-rw-r--r--  2.0 unx      992 b- defN 23-Jun-29 15:39 test/test_nuget_package_upload_request.py
+-rw-r--r--  2.0 unx      892 b- defN 23-Jun-29 15:39 test/test_nuget_upstream.py
+-rw-r--r--  2.0 unx      950 b- defN 23-Jun-29 15:39 test/test_nuget_upstream_request.py
+-rw-r--r--  2.0 unx      992 b- defN 23-Jun-29 15:39 test/test_nuget_upstream_request_patch.py
+-rw-r--r--  2.0 unx      882 b- defN 23-Jun-29 15:39 test/test_organization.py
+-rw-r--r--  2.0 unx      958 b- defN 23-Jun-29 15:39 test/test_organization_group_sync.py
+-rw-r--r--  2.0 unx     1016 b- defN 23-Jun-29 15:39 test/test_organization_group_sync_request.py
+-rw-r--r--  2.0 unx      932 b- defN 23-Jun-29 15:39 test/test_organization_invite.py
+-rw-r--r--  2.0 unx      982 b- defN 23-Jun-29 15:39 test/test_organization_invite_extend.py
+-rw-r--r--  2.0 unx      990 b- defN 23-Jun-29 15:39 test/test_organization_invite_request.py
+-rw-r--r--  2.0 unx      982 b- defN 23-Jun-29 15:39 test/test_organization_invite_update.py
+-rw-r--r--  2.0 unx     1082 b- defN 23-Jun-29 15:39 test/test_organization_invite_update_request_patch.py
+-rw-r--r--  2.0 unx      964 b- defN 23-Jun-29 15:39 test/test_organization_membership.py
+-rw-r--r--  2.0 unx     1048 b- defN 23-Jun-29 15:39 test/test_organization_package_license_policy.py
+-rw-r--r--  2.0 unx     1106 b- defN 23-Jun-29 15:39 test/test_organization_package_license_policy_request.py
+-rw-r--r--  2.0 unx     1148 b- defN 23-Jun-29 15:39 test/test_organization_package_license_policy_request_patch.py
+-rw-r--r--  2.0 unx     1096 b- defN 23-Jun-29 15:39 test/test_organization_package_vulnerability_policy.py
+-rw-r--r--  2.0 unx     1154 b- defN 23-Jun-29 15:39 test/test_organization_package_vulnerability_policy_request.py
+-rw-r--r--  2.0 unx     1196 b- defN 23-Jun-29 15:39 test/test_organization_package_vulnerability_policy_request_patch.py
+-rw-r--r--  2.0 unx      916 b- defN 23-Jun-29 15:39 test/test_organization_team.py
+-rw-r--r--  2.0 unx      974 b- defN 23-Jun-29 15:39 test/test_organization_team_members.py
+-rw-r--r--  2.0 unx      998 b- defN 23-Jun-29 15:39 test/test_organization_team_membership.py
+-rw-r--r--  2.0 unx      974 b- defN 23-Jun-29 15:39 test/test_organization_team_request.py
+-rw-r--r--  2.0 unx     1016 b- defN 23-Jun-29 15:39 test/test_organization_team_request_patch.py
+-rw-r--r--  2.0 unx    10220 b- defN 23-Jun-29 15:39 test/test_orgs_api.py
+-rw-r--r--  2.0 unx      910 b- defN 23-Jun-29 15:39 test/test_p2_package_upload.py
+-rw-r--r--  2.0 unx      968 b- defN 23-Jun-29 15:39 test/test_p2_package_upload_request.py
+-rw-r--r--  2.0 unx      842 b- defN 23-Jun-29 15:39 test/test_package.py
+-rw-r--r--  2.0 unx      876 b- defN 23-Jun-29 15:39 test/test_package_copy.py
+-rw-r--r--  2.0 unx      934 b- defN 23-Jun-29 15:39 test/test_package_copy_request.py
+-rw-r--r--  2.0 unx      940 b- defN 23-Jun-29 15:39 test/test_package_dependencies.py
+-rw-r--r--  2.0 unx      924 b- defN 23-Jun-29 15:39 test/test_package_dependency.py
+-rw-r--r--  2.0 unx      876 b- defN 23-Jun-29 15:39 test/test_package_file.py
+-rw-r--r--  2.0 unx      968 b- defN 23-Jun-29 15:39 test/test_package_file_parts_upload.py
+-rw-r--r--  2.0 unx      926 b- defN 23-Jun-29 15:39 test/test_package_file_upload.py
+-rw-r--r--  2.0 unx      984 b- defN 23-Jun-29 15:39 test/test_package_file_upload_request.py
+-rw-r--r--  2.0 unx     1090 b- defN 23-Jun-29 15:39 test/test_package_license_policy_evaluation_request.py
+-rw-r--r--  2.0 unx     1148 b- defN 23-Jun-29 15:39 test/test_package_license_policy_evaluation_request_request.py
+-rw-r--r--  2.0 unx     1050 b- defN 23-Jun-29 15:39 test/test_package_license_policy_violation_log.py
+-rw-r--r--  2.0 unx     1134 b- defN 23-Jun-29 15:39 test/test_package_license_policy_violation_log_cursor_page.py
+-rw-r--r--  2.0 unx      876 b- defN 23-Jun-29 15:39 test/test_package_move.py
+-rw-r--r--  2.0 unx      934 b- defN 23-Jun-29 15:39 test/test_package_move_request.py
+-rw-r--r--  2.0 unx      924 b- defN 23-Jun-29 15:39 test/test_package_quarantine.py
+-rw-r--r--  2.0 unx      982 b- defN 23-Jun-29 15:39 test/test_package_quarantine_request.py
+-rw-r--r--  2.0 unx      892 b- defN 23-Jun-29 15:39 test/test_package_resync.py
+-rw-r--r--  2.0 unx      892 b- defN 23-Jun-29 15:39 test/test_package_status.py
+-rw-r--r--  2.0 unx      868 b- defN 23-Jun-29 15:39 test/test_package_tag.py
+-rw-r--r--  2.0 unx      926 b- defN 23-Jun-29 15:39 test/test_package_tag_request.py
+-rw-r--r--  2.0 unx      942 b- defN 23-Jun-29 15:39 test/test_package_usage_metrics.py
+-rw-r--r--  2.0 unx      942 b- defN 23-Jun-29 15:39 test/test_package_version_badge.py
+-rw-r--r--  2.0 unx      948 b- defN 23-Jun-29 15:39 test/test_package_vulnerability.py
+-rw-r--r--  2.0 unx     1138 b- defN 23-Jun-29 15:39 test/test_package_vulnerability_policy_evaluation_request.py
+-rw-r--r--  2.0 unx     1196 b- defN 23-Jun-29 15:39 test/test_package_vulnerability_policy_evaluation_request_request.py
+-rw-r--r--  2.0 unx     1098 b- defN 23-Jun-29 15:39 test/test_package_vulnerability_policy_violation_log.py
+-rw-r--r--  2.0 unx     1182 b- defN 23-Jun-29 15:39 test/test_package_vulnerability_policy_violation_log_cursor_page.py
+-rw-r--r--  2.0 unx    11743 b- defN 23-Jun-29 15:39 test/test_packages_api.py
+-rw-r--r--  2.0 unx      942 b- defN 23-Jun-29 15:39 test/test_python_package_upload.py
+-rw-r--r--  2.0 unx     1000 b- defN 23-Jun-29 15:39 test/test_python_package_upload_request.py
+-rw-r--r--  2.0 unx      900 b- defN 23-Jun-29 15:39 test/test_python_upstream.py
+-rw-r--r--  2.0 unx      958 b- defN 23-Jun-29 15:39 test/test_python_upstream_request.py
+-rw-r--r--  2.0 unx     1000 b- defN 23-Jun-29 15:39 test/test_python_upstream_request_patch.py
+-rw-r--r--  2.0 unx      826 b- defN 23-Jun-29 15:39 test/test_quota.py
+-rw-r--r--  2.0 unx     1364 b- defN 23-Jun-29 15:39 test/test_quota_api.py
+-rw-r--r--  2.0 unx      884 b- defN 23-Jun-29 15:39 test/test_quota_history.py
+-rw-r--r--  2.0 unx      860 b- defN 23-Jun-29 15:39 test/test_rate_check.py
+-rw-r--r--  2.0 unx      862 b- defN 23-Jun-29 15:39 test/test_rates_api.py
+-rw-r--r--  2.0 unx      918 b- defN 23-Jun-29 15:39 test/test_raw_package_upload.py
+-rw-r--r--  2.0 unx      976 b- defN 23-Jun-29 15:39 test/test_raw_package_upload_request.py
+-rw-r--r--  2.0 unx    16607 b- defN 23-Jun-29 15:39 test/test_repos_api.py
+-rw-r--r--  2.0 unx      866 b- defN 23-Jun-29 15:39 test/test_repository.py
+-rw-r--r--  2.0 unx      934 b- defN 23-Jun-29 15:39 test/test_repository_audit_log.py
+-rw-r--r--  2.0 unx      916 b- defN 23-Jun-29 15:39 test/test_repository_create.py
+-rw-r--r--  2.0 unx      974 b- defN 23-Jun-29 15:39 test/test_repository_create_request.py
+-rw-r--r--  2.0 unx      944 b- defN 23-Jun-29 15:39 test/test_repository_geo_ip_cidr.py
+-rw-r--r--  2.0 unx     1002 b- defN 23-Jun-29 15:39 test/test_repository_geo_ip_country_code.py
+-rw-r--r--  2.0 unx      952 b- defN 23-Jun-29 15:39 test/test_repository_geo_ip_rules.py
+-rw-r--r--  2.0 unx     1010 b- defN 23-Jun-29 15:39 test/test_repository_geo_ip_rules_request.py
+-rw-r--r--  2.0 unx     1052 b- defN 23-Jun-29 15:39 test/test_repository_geo_ip_rules_request_patch.py
+-rw-r--r--  2.0 unx     1002 b- defN 23-Jun-29 15:39 test/test_repository_geo_ip_test_address.py
+-rw-r--r--  2.0 unx     1068 b- defN 23-Jun-29 15:39 test/test_repository_geo_ip_test_address_response.py
+-rw-r--r--  2.0 unx     1102 b- defN 23-Jun-29 15:39 test/test_repository_geo_ip_test_address_response_dict.py
+-rw-r--r--  2.0 unx      918 b- defN 23-Jun-29 15:39 test/test_repository_gpg_key.py
+-rw-r--r--  2.0 unx      968 b- defN 23-Jun-29 15:39 test/test_repository_gpg_key_create.py
+-rw-r--r--  2.0 unx      974 b- defN 23-Jun-29 15:39 test/test_repository_privilege_dict.py
+-rw-r--r--  2.0 unx      982 b- defN 23-Jun-29 15:39 test/test_repository_privilege_input.py
+-rw-r--r--  2.0 unx     1040 b- defN 23-Jun-29 15:39 test/test_repository_privilege_input_request.py
+-rw-r--r--  2.0 unx     1082 b- defN 23-Jun-29 15:39 test/test_repository_privilege_input_request_patch.py
+-rw-r--r--  2.0 unx      966 b- defN 23-Jun-29 15:39 test/test_repository_request_patch.py
+-rw-r--r--  2.0 unx      918 b- defN 23-Jun-29 15:39 test/test_repository_rsa_key.py
+-rw-r--r--  2.0 unx      968 b- defN 23-Jun-29 15:39 test/test_repository_rsa_key_create.py
+-rw-r--r--  2.0 unx      908 b- defN 23-Jun-29 15:39 test/test_repository_token.py
+-rw-r--r--  2.0 unx      958 b- defN 23-Jun-29 15:39 test/test_repository_token_action.py
+-rw-r--r--  2.0 unx      966 b- defN 23-Jun-29 15:39 test/test_repository_token_refresh.py
+-rw-r--r--  2.0 unx     1024 b- defN 23-Jun-29 15:39 test/test_repository_token_refresh_request.py
+-rw-r--r--  2.0 unx      966 b- defN 23-Jun-29 15:39 test/test_repository_token_request.py
+-rw-r--r--  2.0 unx     1008 b- defN 23-Jun-29 15:39 test/test_repository_token_request_patch.py
+-rw-r--r--  2.0 unx      942 b- defN 23-Jun-29 15:39 test/test_repository_token_sync.py
+-rw-r--r--  2.0 unx     1000 b- defN 23-Jun-29 15:39 test/test_repository_token_sync_request.py
+-rw-r--r--  2.0 unx      924 b- defN 23-Jun-29 15:39 test/test_repository_webhook.py
+-rw-r--r--  2.0 unx      982 b- defN 23-Jun-29 15:39 test/test_repository_webhook_request.py
+-rw-r--r--  2.0 unx     1024 b- defN 23-Jun-29 15:39 test/test_repository_webhook_request_patch.py
+-rw-r--r--  2.0 unx      934 b- defN 23-Jun-29 15:39 test/test_resources_rate_check.py
+-rw-r--r--  2.0 unx     1026 b- defN 23-Jun-29 15:39 test/test_respository_geo_ip_enable_disable.py
+-rw-r--r--  2.0 unx     1084 b- defN 23-Jun-29 15:39 test/test_respository_geo_ip_enable_disable_request.py
+-rw-r--r--  2.0 unx      918 b- defN 23-Jun-29 15:39 test/test_rpm_package_upload.py
+-rw-r--r--  2.0 unx      976 b- defN 23-Jun-29 15:39 test/test_rpm_package_upload_request.py
+-rw-r--r--  2.0 unx      876 b- defN 23-Jun-29 15:39 test/test_rpm_upstream.py
+-rw-r--r--  2.0 unx      934 b- defN 23-Jun-29 15:39 test/test_rpm_upstream_request.py
+-rw-r--r--  2.0 unx      976 b- defN 23-Jun-29 15:39 test/test_rpm_upstream_request_patch.py
+-rw-r--r--  2.0 unx      926 b- defN 23-Jun-29 15:39 test/test_ruby_package_upload.py
+-rw-r--r--  2.0 unx      984 b- defN 23-Jun-29 15:39 test/test_ruby_package_upload_request.py
+-rw-r--r--  2.0 unx      884 b- defN 23-Jun-29 15:39 test/test_ruby_upstream.py
+-rw-r--r--  2.0 unx      942 b- defN 23-Jun-29 15:39 test/test_ruby_upstream_request.py
+-rw-r--r--  2.0 unx      984 b- defN 23-Jun-29 15:39 test/test_ruby_upstream_request_patch.py
+-rw-r--r--  2.0 unx      842 b- defN 23-Jun-29 15:39 test/test_service.py
+-rw-r--r--  2.0 unx      900 b- defN 23-Jun-29 15:39 test/test_service_request.py
+-rw-r--r--  2.0 unx      942 b- defN 23-Jun-29 15:39 test/test_service_request_patch.py
+-rw-r--r--  2.0 unx      884 b- defN 23-Jun-29 15:39 test/test_service_teams.py
+-rw-r--r--  2.0 unx      864 b- defN 23-Jun-29 15:39 test/test_status_api.py
+-rw-r--r--  2.0 unx      876 b- defN 23-Jun-29 15:39 test/test_status_basic.py
+-rw-r--r--  2.0 unx      958 b- defN 23-Jun-29 15:39 test/test_storage_allocated_limit.py
+-rw-r--r--  2.0 unx      984 b- defN 23-Jun-29 15:39 test/test_storage_allocated_limit_raw.py
+-rw-r--r--  2.0 unx      892 b- defN 23-Jun-29 15:39 test/test_storage_region.py
+-rw-r--r--  2.0 unx     1088 b- defN 23-Jun-29 15:39 test/test_storage_regions_api.py
+-rw-r--r--  2.0 unx      884 b- defN 23-Jun-29 15:39 test/test_storage_usage.py
+-rw-r--r--  2.0 unx      910 b- defN 23-Jun-29 15:39 test/test_storage_usage_raw.py
+-rw-r--r--  2.0 unx      934 b- defN 23-Jun-29 15:39 test/test_swift_package_upload.py
+-rw-r--r--  2.0 unx      992 b- defN 23-Jun-29 15:39 test/test_swift_package_upload_request.py
+-rw-r--r--  2.0 unx      818 b- defN 23-Jun-29 15:39 test/test_tags.py
+-rw-r--r--  2.0 unx      966 b- defN 23-Jun-29 15:39 test/test_terraform_package_upload.py
+-rw-r--r--  2.0 unx     1024 b- defN 23-Jun-29 15:39 test/test_terraform_package_upload_request.py
+-rw-r--r--  2.0 unx      826 b- defN 23-Jun-29 15:39 test/test_usage.py
+-rw-r--r--  2.0 unx      892 b- defN 23-Jun-29 15:39 test/test_usage_fieldset.py
+-rw-r--r--  2.0 unx      876 b- defN 23-Jun-29 15:39 test/test_usage_limits.py
+-rw-r--r--  2.0 unx      902 b- defN 23-Jun-29 15:39 test/test_usage_limits_raw.py
+-rw-r--r--  2.0 unx      852 b- defN 23-Jun-29 15:39 test/test_usage_raw.py
+-rw-r--r--  2.0 unx     1024 b- defN 23-Jun-29 15:39 test/test_user_api.py
+-rw-r--r--  2.0 unx      894 b- defN 23-Jun-29 15:39 test/test_user_auth_token.py
+-rw-r--r--  2.0 unx      952 b- defN 23-Jun-29 15:39 test/test_user_auth_token_request.py
+-rw-r--r--  2.0 unx      860 b- defN 23-Jun-29 15:39 test/test_user_brief.py
+-rw-r--r--  2.0 unx      876 b- defN 23-Jun-29 15:39 test/test_user_profile.py
+-rw-r--r--  2.0 unx      865 b- defN 23-Jun-29 15:39 test/test_users_api.py
+-rw-r--r--  2.0 unx      950 b- defN 23-Jun-29 15:39 test/test_vagrant_package_upload.py
+-rw-r--r--  2.0 unx     1008 b- defN 23-Jun-29 15:39 test/test_vagrant_package_upload_request.py
+-rw-r--r--  2.0 unx     1487 b- defN 23-Jun-29 15:39 test/test_vulnerabilities_api.py
+-rw-r--r--  2.0 unx      890 b- defN 23-Jun-29 15:39 test/test_vulnerability.py
+-rw-r--r--  2.0 unx      924 b- defN 23-Jun-29 15:39 test/test_vulnerability_scan.py
+-rw-r--r--  2.0 unx      982 b- defN 23-Jun-29 15:39 test/test_vulnerability_scan_results.py
+-rw-r--r--  2.0 unx     1016 b- defN 23-Jun-29 15:39 test/test_vulnerability_scan_results_list.py
+-rw-r--r--  2.0 unx      982 b- defN 23-Jun-29 15:39 test/test_vulnerability_scan_version.py
+-rw-r--r--  2.0 unx      908 b- defN 23-Jun-29 15:39 test/test_webhook_template.py
+-rw-r--r--  2.0 unx     1557 b- defN 23-Jun-29 15:39 test/test_webhooks_api.py
+-rw-r--r--  2.0 unx      413 b- defN 23-Jun-29 15:39 cloudsmith_api-2.0.7.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jun-29 15:39 cloudsmith_api-2.0.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       20 b- defN 23-Jun-29 15:39 cloudsmith_api-2.0.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    47075 b- defN 23-Jun-29 15:39 cloudsmith_api-2.0.7.dist-info/RECORD
+483 files, 5479402 bytes uncompressed, 802604 bytes compressed:  85.4%
```

## zipnote {}

```diff
@@ -141,20 +141,38 @@
 
 Filename: cloudsmith_api/models/dart_package_upload.py
 Comment: 
 
 Filename: cloudsmith_api/models/dart_package_upload_request.py
 Comment: 
 
+Filename: cloudsmith_api/models/dart_upstream.py
+Comment: 
+
+Filename: cloudsmith_api/models/dart_upstream_request.py
+Comment: 
+
+Filename: cloudsmith_api/models/dart_upstream_request_patch.py
+Comment: 
+
 Filename: cloudsmith_api/models/deb_package_upload.py
 Comment: 
 
 Filename: cloudsmith_api/models/deb_package_upload_request.py
 Comment: 
 
+Filename: cloudsmith_api/models/deb_upstream.py
+Comment: 
+
+Filename: cloudsmith_api/models/deb_upstream_request.py
+Comment: 
+
+Filename: cloudsmith_api/models/deb_upstream_request_patch.py
+Comment: 
+
 Filename: cloudsmith_api/models/distribution.py
 Comment: 
 
 Filename: cloudsmith_api/models/distribution_full.py
 Comment: 
 
 Filename: cloudsmith_api/models/distribution_version.py
@@ -162,14 +180,23 @@
 
 Filename: cloudsmith_api/models/docker_package_upload.py
 Comment: 
 
 Filename: cloudsmith_api/models/docker_package_upload_request.py
 Comment: 
 
+Filename: cloudsmith_api/models/docker_upstream.py
+Comment: 
+
+Filename: cloudsmith_api/models/docker_upstream_request.py
+Comment: 
+
+Filename: cloudsmith_api/models/docker_upstream_request_patch.py
+Comment: 
+
 Filename: cloudsmith_api/models/entitlement_usage_metrics.py
 Comment: 
 
 Filename: cloudsmith_api/models/error_detail.py
 Comment: 
 
 Filename: cloudsmith_api/models/eula.py
@@ -192,14 +219,23 @@
 
 Filename: cloudsmith_api/models/helm_package_upload.py
 Comment: 
 
 Filename: cloudsmith_api/models/helm_package_upload_request.py
 Comment: 
 
+Filename: cloudsmith_api/models/helm_upstream.py
+Comment: 
+
+Filename: cloudsmith_api/models/helm_upstream_request.py
+Comment: 
+
+Filename: cloudsmith_api/models/helm_upstream_request_patch.py
+Comment: 
+
 Filename: cloudsmith_api/models/hex_package_upload.py
 Comment: 
 
 Filename: cloudsmith_api/models/hex_package_upload_request.py
 Comment: 
 
 Filename: cloudsmith_api/models/history.py
@@ -219,14 +255,23 @@
 
 Filename: cloudsmith_api/models/maven_package_upload.py
 Comment: 
 
 Filename: cloudsmith_api/models/maven_package_upload_request.py
 Comment: 
 
+Filename: cloudsmith_api/models/maven_upstream.py
+Comment: 
+
+Filename: cloudsmith_api/models/maven_upstream_request.py
+Comment: 
+
+Filename: cloudsmith_api/models/maven_upstream_request_patch.py
+Comment: 
+
 Filename: cloudsmith_api/models/namespace.py
 Comment: 
 
 Filename: cloudsmith_api/models/namespace_audit_log.py
 Comment: 
 
 Filename: cloudsmith_api/models/nested_license_policy.py
@@ -240,20 +285,38 @@
 
 Filename: cloudsmith_api/models/npm_package_upload.py
 Comment: 
 
 Filename: cloudsmith_api/models/npm_package_upload_request.py
 Comment: 
 
+Filename: cloudsmith_api/models/npm_upstream.py
+Comment: 
+
+Filename: cloudsmith_api/models/npm_upstream_request.py
+Comment: 
+
+Filename: cloudsmith_api/models/npm_upstream_request_patch.py
+Comment: 
+
 Filename: cloudsmith_api/models/nuget_package_upload.py
 Comment: 
 
 Filename: cloudsmith_api/models/nuget_package_upload_request.py
 Comment: 
 
+Filename: cloudsmith_api/models/nuget_upstream.py
+Comment: 
+
+Filename: cloudsmith_api/models/nuget_upstream_request.py
+Comment: 
+
+Filename: cloudsmith_api/models/nuget_upstream_request_patch.py
+Comment: 
+
 Filename: cloudsmith_api/models/organization.py
 Comment: 
 
 Filename: cloudsmith_api/models/organization_group_sync.py
 Comment: 
 
 Filename: cloudsmith_api/models/organization_group_sync_request.py
@@ -339,14 +402,20 @@
 
 Filename: cloudsmith_api/models/package_file_upload.py
 Comment: 
 
 Filename: cloudsmith_api/models/package_file_upload_request.py
 Comment: 
 
+Filename: cloudsmith_api/models/package_license_policy_evaluation_request.py
+Comment: 
+
+Filename: cloudsmith_api/models/package_license_policy_evaluation_request_request.py
+Comment: 
+
 Filename: cloudsmith_api/models/package_license_policy_violation_log.py
 Comment: 
 
 Filename: cloudsmith_api/models/package_license_policy_violation_log_cursor_page.py
 Comment: 
 
 Filename: cloudsmith_api/models/package_move.py
@@ -378,26 +447,41 @@
 
 Filename: cloudsmith_api/models/package_version_badge.py
 Comment: 
 
 Filename: cloudsmith_api/models/package_vulnerability.py
 Comment: 
 
+Filename: cloudsmith_api/models/package_vulnerability_policy_evaluation_request.py
+Comment: 
+
+Filename: cloudsmith_api/models/package_vulnerability_policy_evaluation_request_request.py
+Comment: 
+
 Filename: cloudsmith_api/models/package_vulnerability_policy_violation_log.py
 Comment: 
 
 Filename: cloudsmith_api/models/package_vulnerability_policy_violation_log_cursor_page.py
 Comment: 
 
 Filename: cloudsmith_api/models/python_package_upload.py
 Comment: 
 
 Filename: cloudsmith_api/models/python_package_upload_request.py
 Comment: 
 
+Filename: cloudsmith_api/models/python_upstream.py
+Comment: 
+
+Filename: cloudsmith_api/models/python_upstream_request.py
+Comment: 
+
+Filename: cloudsmith_api/models/python_upstream_request_patch.py
+Comment: 
+
 Filename: cloudsmith_api/models/quota.py
 Comment: 
 
 Filename: cloudsmith_api/models/quota_history.py
 Comment: 
 
 Filename: cloudsmith_api/models/rate_check.py
@@ -516,20 +600,38 @@
 
 Filename: cloudsmith_api/models/rpm_package_upload.py
 Comment: 
 
 Filename: cloudsmith_api/models/rpm_package_upload_request.py
 Comment: 
 
+Filename: cloudsmith_api/models/rpm_upstream.py
+Comment: 
+
+Filename: cloudsmith_api/models/rpm_upstream_request.py
+Comment: 
+
+Filename: cloudsmith_api/models/rpm_upstream_request_patch.py
+Comment: 
+
 Filename: cloudsmith_api/models/ruby_package_upload.py
 Comment: 
 
 Filename: cloudsmith_api/models/ruby_package_upload_request.py
 Comment: 
 
+Filename: cloudsmith_api/models/ruby_upstream.py
+Comment: 
+
+Filename: cloudsmith_api/models/ruby_upstream_request.py
+Comment: 
+
+Filename: cloudsmith_api/models/ruby_upstream_request_patch.py
+Comment: 
+
 Filename: cloudsmith_api/models/service.py
 Comment: 
 
 Filename: cloudsmith_api/models/service_request.py
 Comment: 
 
 Filename: cloudsmith_api/models/service_request_patch.py
@@ -699,20 +801,38 @@
 
 Filename: test/test_dart_package_upload.py
 Comment: 
 
 Filename: test/test_dart_package_upload_request.py
 Comment: 
 
+Filename: test/test_dart_upstream.py
+Comment: 
+
+Filename: test/test_dart_upstream_request.py
+Comment: 
+
+Filename: test/test_dart_upstream_request_patch.py
+Comment: 
+
 Filename: test/test_deb_package_upload.py
 Comment: 
 
 Filename: test/test_deb_package_upload_request.py
 Comment: 
 
+Filename: test/test_deb_upstream.py
+Comment: 
+
+Filename: test/test_deb_upstream_request.py
+Comment: 
+
+Filename: test/test_deb_upstream_request_patch.py
+Comment: 
+
 Filename: test/test_distribution.py
 Comment: 
 
 Filename: test/test_distribution_full.py
 Comment: 
 
 Filename: test/test_distribution_version.py
@@ -723,14 +843,23 @@
 
 Filename: test/test_docker_package_upload.py
 Comment: 
 
 Filename: test/test_docker_package_upload_request.py
 Comment: 
 
+Filename: test/test_docker_upstream.py
+Comment: 
+
+Filename: test/test_docker_upstream_request.py
+Comment: 
+
+Filename: test/test_docker_upstream_request_patch.py
+Comment: 
+
 Filename: test/test_entitlement_usage_metrics.py
 Comment: 
 
 Filename: test/test_entitlements_api.py
 Comment: 
 
 Filename: test/test_error_detail.py
@@ -762,14 +891,23 @@
 
 Filename: test/test_helm_package_upload.py
 Comment: 
 
 Filename: test/test_helm_package_upload_request.py
 Comment: 
 
+Filename: test/test_helm_upstream.py
+Comment: 
+
+Filename: test/test_helm_upstream_request.py
+Comment: 
+
+Filename: test/test_helm_upstream_request_patch.py
+Comment: 
+
 Filename: test/test_hex_package_upload.py
 Comment: 
 
 Filename: test/test_hex_package_upload_request.py
 Comment: 
 
 Filename: test/test_history.py
@@ -789,14 +927,23 @@
 
 Filename: test/test_maven_package_upload.py
 Comment: 
 
 Filename: test/test_maven_package_upload_request.py
 Comment: 
 
+Filename: test/test_maven_upstream.py
+Comment: 
+
+Filename: test/test_maven_upstream_request.py
+Comment: 
+
+Filename: test/test_maven_upstream_request_patch.py
+Comment: 
+
 Filename: test/test_metrics_api.py
 Comment: 
 
 Filename: test/test_namespace.py
 Comment: 
 
 Filename: test/test_namespace_audit_log.py
@@ -816,20 +963,38 @@
 
 Filename: test/test_npm_package_upload.py
 Comment: 
 
 Filename: test/test_npm_package_upload_request.py
 Comment: 
 
+Filename: test/test_npm_upstream.py
+Comment: 
+
+Filename: test/test_npm_upstream_request.py
+Comment: 
+
+Filename: test/test_npm_upstream_request_patch.py
+Comment: 
+
 Filename: test/test_nuget_package_upload.py
 Comment: 
 
 Filename: test/test_nuget_package_upload_request.py
 Comment: 
 
+Filename: test/test_nuget_upstream.py
+Comment: 
+
+Filename: test/test_nuget_upstream_request.py
+Comment: 
+
+Filename: test/test_nuget_upstream_request_patch.py
+Comment: 
+
 Filename: test/test_organization.py
 Comment: 
 
 Filename: test/test_organization_group_sync.py
 Comment: 
 
 Filename: test/test_organization_group_sync_request.py
@@ -918,14 +1083,20 @@
 
 Filename: test/test_package_file_upload.py
 Comment: 
 
 Filename: test/test_package_file_upload_request.py
 Comment: 
 
+Filename: test/test_package_license_policy_evaluation_request.py
+Comment: 
+
+Filename: test/test_package_license_policy_evaluation_request_request.py
+Comment: 
+
 Filename: test/test_package_license_policy_violation_log.py
 Comment: 
 
 Filename: test/test_package_license_policy_violation_log_cursor_page.py
 Comment: 
 
 Filename: test/test_package_move.py
@@ -957,14 +1128,20 @@
 
 Filename: test/test_package_version_badge.py
 Comment: 
 
 Filename: test/test_package_vulnerability.py
 Comment: 
 
+Filename: test/test_package_vulnerability_policy_evaluation_request.py
+Comment: 
+
+Filename: test/test_package_vulnerability_policy_evaluation_request_request.py
+Comment: 
+
 Filename: test/test_package_vulnerability_policy_violation_log.py
 Comment: 
 
 Filename: test/test_package_vulnerability_policy_violation_log_cursor_page.py
 Comment: 
 
 Filename: test/test_packages_api.py
@@ -972,14 +1149,23 @@
 
 Filename: test/test_python_package_upload.py
 Comment: 
 
 Filename: test/test_python_package_upload_request.py
 Comment: 
 
+Filename: test/test_python_upstream.py
+Comment: 
+
+Filename: test/test_python_upstream_request.py
+Comment: 
+
+Filename: test/test_python_upstream_request_patch.py
+Comment: 
+
 Filename: test/test_quota.py
 Comment: 
 
 Filename: test/test_quota_api.py
 Comment: 
 
 Filename: test/test_quota_history.py
@@ -1107,20 +1293,38 @@
 
 Filename: test/test_rpm_package_upload.py
 Comment: 
 
 Filename: test/test_rpm_package_upload_request.py
 Comment: 
 
+Filename: test/test_rpm_upstream.py
+Comment: 
+
+Filename: test/test_rpm_upstream_request.py
+Comment: 
+
+Filename: test/test_rpm_upstream_request_patch.py
+Comment: 
+
 Filename: test/test_ruby_package_upload.py
 Comment: 
 
 Filename: test/test_ruby_package_upload_request.py
 Comment: 
 
+Filename: test/test_ruby_upstream.py
+Comment: 
+
+Filename: test/test_ruby_upstream_request.py
+Comment: 
+
+Filename: test/test_ruby_upstream_request_patch.py
+Comment: 
+
 Filename: test/test_service.py
 Comment: 
 
 Filename: test/test_service_request.py
 Comment: 
 
 Filename: test/test_service_request_patch.py
@@ -1227,20 +1431,20 @@
 
 Filename: test/test_webhook_template.py
 Comment: 
 
 Filename: test/test_webhooks_api.py
 Comment: 
 
-Filename: cloudsmith_api-2.0.6.dist-info/METADATA
+Filename: cloudsmith_api-2.0.7.dist-info/METADATA
 Comment: 
 
-Filename: cloudsmith_api-2.0.6.dist-info/WHEEL
+Filename: cloudsmith_api-2.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: cloudsmith_api-2.0.6.dist-info/top_level.txt
+Filename: cloudsmith_api-2.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: cloudsmith_api-2.0.6.dist-info/RECORD
+Filename: cloudsmith_api-2.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cloudsmith_api/__init__.py

```diff
@@ -60,49 +60,70 @@
 from cloudsmith_api.models.conan_package_upload_request import ConanPackageUploadRequest
 from cloudsmith_api.models.conda_package_upload import CondaPackageUpload
 from cloudsmith_api.models.conda_package_upload_request import CondaPackageUploadRequest
 from cloudsmith_api.models.cran_package_upload import CranPackageUpload
 from cloudsmith_api.models.cran_package_upload_request import CranPackageUploadRequest
 from cloudsmith_api.models.dart_package_upload import DartPackageUpload
 from cloudsmith_api.models.dart_package_upload_request import DartPackageUploadRequest
+from cloudsmith_api.models.dart_upstream import DartUpstream
+from cloudsmith_api.models.dart_upstream_request import DartUpstreamRequest
+from cloudsmith_api.models.dart_upstream_request_patch import DartUpstreamRequestPatch
 from cloudsmith_api.models.deb_package_upload import DebPackageUpload
 from cloudsmith_api.models.deb_package_upload_request import DebPackageUploadRequest
+from cloudsmith_api.models.deb_upstream import DebUpstream
+from cloudsmith_api.models.deb_upstream_request import DebUpstreamRequest
+from cloudsmith_api.models.deb_upstream_request_patch import DebUpstreamRequestPatch
 from cloudsmith_api.models.distribution import Distribution
 from cloudsmith_api.models.distribution_full import DistributionFull
 from cloudsmith_api.models.distribution_version import DistributionVersion
 from cloudsmith_api.models.docker_package_upload import DockerPackageUpload
 from cloudsmith_api.models.docker_package_upload_request import DockerPackageUploadRequest
+from cloudsmith_api.models.docker_upstream import DockerUpstream
+from cloudsmith_api.models.docker_upstream_request import DockerUpstreamRequest
+from cloudsmith_api.models.docker_upstream_request_patch import DockerUpstreamRequestPatch
 from cloudsmith_api.models.entitlement_usage_metrics import EntitlementUsageMetrics
 from cloudsmith_api.models.error_detail import ErrorDetail
 from cloudsmith_api.models.eula import Eula
 from cloudsmith_api.models.format import Format
 from cloudsmith_api.models.format_support import FormatSupport
 from cloudsmith_api.models.geo_ip_location import GeoIpLocation
 from cloudsmith_api.models.go_package_upload import GoPackageUpload
 from cloudsmith_api.models.go_package_upload_request import GoPackageUploadRequest
 from cloudsmith_api.models.helm_package_upload import HelmPackageUpload
 from cloudsmith_api.models.helm_package_upload_request import HelmPackageUploadRequest
+from cloudsmith_api.models.helm_upstream import HelmUpstream
+from cloudsmith_api.models.helm_upstream_request import HelmUpstreamRequest
+from cloudsmith_api.models.helm_upstream_request_patch import HelmUpstreamRequestPatch
 from cloudsmith_api.models.hex_package_upload import HexPackageUpload
 from cloudsmith_api.models.hex_package_upload_request import HexPackageUploadRequest
 from cloudsmith_api.models.history import History
 from cloudsmith_api.models.history_fieldset import HistoryFieldset
 from cloudsmith_api.models.history_fieldset_raw import HistoryFieldsetRaw
 from cloudsmith_api.models.luarocks_package_upload import LuarocksPackageUpload
 from cloudsmith_api.models.luarocks_package_upload_request import LuarocksPackageUploadRequest
 from cloudsmith_api.models.maven_package_upload import MavenPackageUpload
 from cloudsmith_api.models.maven_package_upload_request import MavenPackageUploadRequest
+from cloudsmith_api.models.maven_upstream import MavenUpstream
+from cloudsmith_api.models.maven_upstream_request import MavenUpstreamRequest
+from cloudsmith_api.models.maven_upstream_request_patch import MavenUpstreamRequestPatch
 from cloudsmith_api.models.namespace import Namespace
 from cloudsmith_api.models.namespace_audit_log import NamespaceAuditLog
 from cloudsmith_api.models.nested_license_policy import NestedLicensePolicy
 from cloudsmith_api.models.nested_vulnerability_policy import NestedVulnerabilityPolicy
 from cloudsmith_api.models.nested_vulnerability_scan_results import NestedVulnerabilityScanResults
 from cloudsmith_api.models.npm_package_upload import NpmPackageUpload
 from cloudsmith_api.models.npm_package_upload_request import NpmPackageUploadRequest
+from cloudsmith_api.models.npm_upstream import NpmUpstream
+from cloudsmith_api.models.npm_upstream_request import NpmUpstreamRequest
+from cloudsmith_api.models.npm_upstream_request_patch import NpmUpstreamRequestPatch
 from cloudsmith_api.models.nuget_package_upload import NugetPackageUpload
 from cloudsmith_api.models.nuget_package_upload_request import NugetPackageUploadRequest
+from cloudsmith_api.models.nuget_upstream import NugetUpstream
+from cloudsmith_api.models.nuget_upstream_request import NugetUpstreamRequest
+from cloudsmith_api.models.nuget_upstream_request_patch import NugetUpstreamRequestPatch
 from cloudsmith_api.models.organization import Organization
 from cloudsmith_api.models.organization_group_sync import OrganizationGroupSync
 from cloudsmith_api.models.organization_group_sync_request import OrganizationGroupSyncRequest
 from cloudsmith_api.models.organization_invite import OrganizationInvite
 from cloudsmith_api.models.organization_invite_extend import OrganizationInviteExtend
 from cloudsmith_api.models.organization_invite_request import OrganizationInviteRequest
 from cloudsmith_api.models.organization_invite_update import OrganizationInviteUpdate
@@ -126,31 +147,38 @@
 from cloudsmith_api.models.package_copy_request import PackageCopyRequest
 from cloudsmith_api.models.package_dependencies import PackageDependencies
 from cloudsmith_api.models.package_dependency import PackageDependency
 from cloudsmith_api.models.package_file import PackageFile
 from cloudsmith_api.models.package_file_parts_upload import PackageFilePartsUpload
 from cloudsmith_api.models.package_file_upload import PackageFileUpload
 from cloudsmith_api.models.package_file_upload_request import PackageFileUploadRequest
+from cloudsmith_api.models.package_license_policy_evaluation_request import PackageLicensePolicyEvaluationRequest
+from cloudsmith_api.models.package_license_policy_evaluation_request_request import PackageLicensePolicyEvaluationRequestRequest
 from cloudsmith_api.models.package_license_policy_violation_log import PackageLicensePolicyViolationLog
 from cloudsmith_api.models.package_license_policy_violation_log_cursor_page import PackageLicensePolicyViolationLogCursorPage
 from cloudsmith_api.models.package_move import PackageMove
 from cloudsmith_api.models.package_move_request import PackageMoveRequest
 from cloudsmith_api.models.package_quarantine import PackageQuarantine
 from cloudsmith_api.models.package_quarantine_request import PackageQuarantineRequest
 from cloudsmith_api.models.package_resync import PackageResync
 from cloudsmith_api.models.package_status import PackageStatus
 from cloudsmith_api.models.package_tag import PackageTag
 from cloudsmith_api.models.package_tag_request import PackageTagRequest
 from cloudsmith_api.models.package_usage_metrics import PackageUsageMetrics
 from cloudsmith_api.models.package_version_badge import PackageVersionBadge
 from cloudsmith_api.models.package_vulnerability import PackageVulnerability
+from cloudsmith_api.models.package_vulnerability_policy_evaluation_request import PackageVulnerabilityPolicyEvaluationRequest
+from cloudsmith_api.models.package_vulnerability_policy_evaluation_request_request import PackageVulnerabilityPolicyEvaluationRequestRequest
 from cloudsmith_api.models.package_vulnerability_policy_violation_log import PackageVulnerabilityPolicyViolationLog
 from cloudsmith_api.models.package_vulnerability_policy_violation_log_cursor_page import PackageVulnerabilityPolicyViolationLogCursorPage
 from cloudsmith_api.models.python_package_upload import PythonPackageUpload
 from cloudsmith_api.models.python_package_upload_request import PythonPackageUploadRequest
+from cloudsmith_api.models.python_upstream import PythonUpstream
+from cloudsmith_api.models.python_upstream_request import PythonUpstreamRequest
+from cloudsmith_api.models.python_upstream_request_patch import PythonUpstreamRequestPatch
 from cloudsmith_api.models.quota import Quota
 from cloudsmith_api.models.quota_history import QuotaHistory
 from cloudsmith_api.models.rate_check import RateCheck
 from cloudsmith_api.models.raw_package_upload import RawPackageUpload
 from cloudsmith_api.models.raw_package_upload_request import RawPackageUploadRequest
 from cloudsmith_api.models.repository import Repository
 from cloudsmith_api.models.repository_audit_log import RepositoryAuditLog
@@ -185,16 +213,22 @@
 from cloudsmith_api.models.repository_webhook_request import RepositoryWebhookRequest
 from cloudsmith_api.models.repository_webhook_request_patch import RepositoryWebhookRequestPatch
 from cloudsmith_api.models.resources_rate_check import ResourcesRateCheck
 from cloudsmith_api.models.respository_geo_ip_enable_disable import RespositoryGeoIpEnableDisable
 from cloudsmith_api.models.respository_geo_ip_enable_disable_request import RespositoryGeoIpEnableDisableRequest
 from cloudsmith_api.models.rpm_package_upload import RpmPackageUpload
 from cloudsmith_api.models.rpm_package_upload_request import RpmPackageUploadRequest
+from cloudsmith_api.models.rpm_upstream import RpmUpstream
+from cloudsmith_api.models.rpm_upstream_request import RpmUpstreamRequest
+from cloudsmith_api.models.rpm_upstream_request_patch import RpmUpstreamRequestPatch
 from cloudsmith_api.models.ruby_package_upload import RubyPackageUpload
 from cloudsmith_api.models.ruby_package_upload_request import RubyPackageUploadRequest
+from cloudsmith_api.models.ruby_upstream import RubyUpstream
+from cloudsmith_api.models.ruby_upstream_request import RubyUpstreamRequest
+from cloudsmith_api.models.ruby_upstream_request_patch import RubyUpstreamRequestPatch
 from cloudsmith_api.models.service import Service
 from cloudsmith_api.models.service_request import ServiceRequest
 from cloudsmith_api.models.service_request_patch import ServiceRequestPatch
 from cloudsmith_api.models.service_teams import ServiceTeams
 from cloudsmith_api.models.status_basic import StatusBasic
 from cloudsmith_api.models.storage_allocated_limit import StorageAllocatedLimit
 from cloudsmith_api.models.storage_allocated_limit_raw import StorageAllocatedLimitRaw
```

## cloudsmith_api/api_client.py

```diff
@@ -70,15 +70,15 @@
         self._pool = None
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'Swagger-Codegen/2.0.6/python'
+        self.user_agent = 'Swagger-Codegen/2.0.7/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __del__(self):
         if self._pool is not None:
             self._pool.close()
             self._pool.join()
```

## cloudsmith_api/configuration.py

```diff
@@ -254,9 +254,9 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: v1\n"\
-               "SDK Package Version: 2.0.6".\
+               "SDK Package Version: 2.0.7".\
                format(env=sys.platform, pyversion=sys.version)
```

## cloudsmith_api/api/orgs_api.py

```diff
@@ -881,14 +881,355 @@
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def orgs_license_policy_evaluation_create(self, org, policy_slug_perm, **kwargs):  # noqa: E501
+        """Create an evaluation request for this policy.  # noqa: E501
+
+        Create an evaluation request for this policy.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.orgs_license_policy_evaluation_create(org, policy_slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str org: (required)
+        :param str policy_slug_perm: (required)
+        :param PackageLicensePolicyEvaluationRequestRequest data:
+        :return: PackageLicensePolicyEvaluationRequest
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.orgs_license_policy_evaluation_create_with_http_info(org, policy_slug_perm, **kwargs)  # noqa: E501
+        else:
+            (data) = self.orgs_license_policy_evaluation_create_with_http_info(org, policy_slug_perm, **kwargs)  # noqa: E501
+            return data
+
+    def orgs_license_policy_evaluation_create_with_http_info(self, org, policy_slug_perm, **kwargs):  # noqa: E501
+        """Create an evaluation request for this policy.  # noqa: E501
+
+        Create an evaluation request for this policy.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.orgs_license_policy_evaluation_create_with_http_info(org, policy_slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str org: (required)
+        :param str policy_slug_perm: (required)
+        :param PackageLicensePolicyEvaluationRequestRequest data:
+        :return: PackageLicensePolicyEvaluationRequest
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['org', 'policy_slug_perm', 'data']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method orgs_license_policy_evaluation_create" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'org' is set
+        if self.api_client.client_side_validation and ('org' not in params or
+                                                       params['org'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `org` when calling `orgs_license_policy_evaluation_create`")  # noqa: E501
+        # verify the required parameter 'policy_slug_perm' is set
+        if self.api_client.client_side_validation and ('policy_slug_perm' not in params or
+                                                       params['policy_slug_perm'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `policy_slug_perm` when calling `orgs_license_policy_evaluation_create`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'org' in params:
+            path_params['org'] = params['org']  # noqa: E501
+        if 'policy_slug_perm' in params:
+            path_params['policy_slug_perm'] = params['policy_slug_perm']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'data' in params:
+            body_params = params['data']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/orgs/{org}/license-policy/{policy_slug_perm}/evaluation/', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='PackageLicensePolicyEvaluationRequest',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def orgs_license_policy_evaluation_list(self, org, policy_slug_perm, **kwargs):  # noqa: E501
+        """List evaluation requests for this policy.  # noqa: E501
+
+        List evaluation requests for this policy.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.orgs_license_policy_evaluation_list(org, policy_slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str org: (required)
+        :param str policy_slug_perm: (required)
+        :param int page: A page number within the paginated result set.
+        :param int page_size: Number of results to return per page.
+        :return: list[PackageLicensePolicyEvaluationRequest]
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.orgs_license_policy_evaluation_list_with_http_info(org, policy_slug_perm, **kwargs)  # noqa: E501
+        else:
+            (data) = self.orgs_license_policy_evaluation_list_with_http_info(org, policy_slug_perm, **kwargs)  # noqa: E501
+            return data
+
+    def orgs_license_policy_evaluation_list_with_http_info(self, org, policy_slug_perm, **kwargs):  # noqa: E501
+        """List evaluation requests for this policy.  # noqa: E501
+
+        List evaluation requests for this policy.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.orgs_license_policy_evaluation_list_with_http_info(org, policy_slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str org: (required)
+        :param str policy_slug_perm: (required)
+        :param int page: A page number within the paginated result set.
+        :param int page_size: Number of results to return per page.
+        :return: list[PackageLicensePolicyEvaluationRequest]
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['org', 'policy_slug_perm', 'page', 'page_size']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method orgs_license_policy_evaluation_list" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'org' is set
+        if self.api_client.client_side_validation and ('org' not in params or
+                                                       params['org'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `org` when calling `orgs_license_policy_evaluation_list`")  # noqa: E501
+        # verify the required parameter 'policy_slug_perm' is set
+        if self.api_client.client_side_validation and ('policy_slug_perm' not in params or
+                                                       params['policy_slug_perm'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `policy_slug_perm` when calling `orgs_license_policy_evaluation_list`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'org' in params:
+            path_params['org'] = params['org']  # noqa: E501
+        if 'policy_slug_perm' in params:
+            path_params['policy_slug_perm'] = params['policy_slug_perm']  # noqa: E501
+
+        query_params = []
+        if 'page' in params:
+            query_params.append(('page', params['page']))  # noqa: E501
+        if 'page_size' in params:
+            query_params.append(('page_size', params['page_size']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/orgs/{org}/license-policy/{policy_slug_perm}/evaluation/', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='list[PackageLicensePolicyEvaluationRequest]',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def orgs_license_policy_evaluation_read(self, org, policy_slug_perm, slug_perm, **kwargs):  # noqa: E501
+        """Retrieve an evaluation request for this policy.  # noqa: E501
+
+        Retrieve an evaluation request for this policy.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.orgs_license_policy_evaluation_read(org, policy_slug_perm, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str org: (required)
+        :param str policy_slug_perm: (required)
+        :param str slug_perm: (required)
+        :return: PackageLicensePolicyEvaluationRequest
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.orgs_license_policy_evaluation_read_with_http_info(org, policy_slug_perm, slug_perm, **kwargs)  # noqa: E501
+        else:
+            (data) = self.orgs_license_policy_evaluation_read_with_http_info(org, policy_slug_perm, slug_perm, **kwargs)  # noqa: E501
+            return data
+
+    def orgs_license_policy_evaluation_read_with_http_info(self, org, policy_slug_perm, slug_perm, **kwargs):  # noqa: E501
+        """Retrieve an evaluation request for this policy.  # noqa: E501
+
+        Retrieve an evaluation request for this policy.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.orgs_license_policy_evaluation_read_with_http_info(org, policy_slug_perm, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str org: (required)
+        :param str policy_slug_perm: (required)
+        :param str slug_perm: (required)
+        :return: PackageLicensePolicyEvaluationRequest
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['org', 'policy_slug_perm', 'slug_perm']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method orgs_license_policy_evaluation_read" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'org' is set
+        if self.api_client.client_side_validation and ('org' not in params or
+                                                       params['org'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `org` when calling `orgs_license_policy_evaluation_read`")  # noqa: E501
+        # verify the required parameter 'policy_slug_perm' is set
+        if self.api_client.client_side_validation and ('policy_slug_perm' not in params or
+                                                       params['policy_slug_perm'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `policy_slug_perm` when calling `orgs_license_policy_evaluation_read`")  # noqa: E501
+        # verify the required parameter 'slug_perm' is set
+        if self.api_client.client_side_validation and ('slug_perm' not in params or
+                                                       params['slug_perm'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `slug_perm` when calling `orgs_license_policy_evaluation_read`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'org' in params:
+            path_params['org'] = params['org']  # noqa: E501
+        if 'policy_slug_perm' in params:
+            path_params['policy_slug_perm'] = params['policy_slug_perm']  # noqa: E501
+        if 'slug_perm' in params:
+            path_params['slug_perm'] = params['slug_perm']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/orgs/{org}/license-policy/{policy_slug_perm}/evaluation/{slug_perm}/', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='PackageLicensePolicyEvaluationRequest',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def orgs_license_policy_list(self, org, **kwargs):  # noqa: E501
         """Get a list of all package license policies.  # noqa: E501
 
         Get a list of all package license policies.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.orgs_license_policy_list(org, async_req=True)
@@ -4186,14 +4527,355 @@
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def orgs_vulnerability_policy_evaluation_create(self, org, policy_slug_perm, **kwargs):  # noqa: E501
+        """Create an evaluation request for this policy.  # noqa: E501
+
+        Create an evaluation request for this policy.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.orgs_vulnerability_policy_evaluation_create(org, policy_slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str org: (required)
+        :param str policy_slug_perm: (required)
+        :param PackageVulnerabilityPolicyEvaluationRequestRequest data:
+        :return: PackageVulnerabilityPolicyEvaluationRequest
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.orgs_vulnerability_policy_evaluation_create_with_http_info(org, policy_slug_perm, **kwargs)  # noqa: E501
+        else:
+            (data) = self.orgs_vulnerability_policy_evaluation_create_with_http_info(org, policy_slug_perm, **kwargs)  # noqa: E501
+            return data
+
+    def orgs_vulnerability_policy_evaluation_create_with_http_info(self, org, policy_slug_perm, **kwargs):  # noqa: E501
+        """Create an evaluation request for this policy.  # noqa: E501
+
+        Create an evaluation request for this policy.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.orgs_vulnerability_policy_evaluation_create_with_http_info(org, policy_slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str org: (required)
+        :param str policy_slug_perm: (required)
+        :param PackageVulnerabilityPolicyEvaluationRequestRequest data:
+        :return: PackageVulnerabilityPolicyEvaluationRequest
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['org', 'policy_slug_perm', 'data']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method orgs_vulnerability_policy_evaluation_create" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'org' is set
+        if self.api_client.client_side_validation and ('org' not in params or
+                                                       params['org'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `org` when calling `orgs_vulnerability_policy_evaluation_create`")  # noqa: E501
+        # verify the required parameter 'policy_slug_perm' is set
+        if self.api_client.client_side_validation and ('policy_slug_perm' not in params or
+                                                       params['policy_slug_perm'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `policy_slug_perm` when calling `orgs_vulnerability_policy_evaluation_create`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'org' in params:
+            path_params['org'] = params['org']  # noqa: E501
+        if 'policy_slug_perm' in params:
+            path_params['policy_slug_perm'] = params['policy_slug_perm']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'data' in params:
+            body_params = params['data']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/orgs/{org}/vulnerability-policy/{policy_slug_perm}/evaluation/', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='PackageVulnerabilityPolicyEvaluationRequest',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def orgs_vulnerability_policy_evaluation_list(self, org, policy_slug_perm, **kwargs):  # noqa: E501
+        """List evaluation requests for this policy.  # noqa: E501
+
+        List evaluation requests for this policy.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.orgs_vulnerability_policy_evaluation_list(org, policy_slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str org: (required)
+        :param str policy_slug_perm: (required)
+        :param int page: A page number within the paginated result set.
+        :param int page_size: Number of results to return per page.
+        :return: list[PackageVulnerabilityPolicyEvaluationRequest]
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.orgs_vulnerability_policy_evaluation_list_with_http_info(org, policy_slug_perm, **kwargs)  # noqa: E501
+        else:
+            (data) = self.orgs_vulnerability_policy_evaluation_list_with_http_info(org, policy_slug_perm, **kwargs)  # noqa: E501
+            return data
+
+    def orgs_vulnerability_policy_evaluation_list_with_http_info(self, org, policy_slug_perm, **kwargs):  # noqa: E501
+        """List evaluation requests for this policy.  # noqa: E501
+
+        List evaluation requests for this policy.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.orgs_vulnerability_policy_evaluation_list_with_http_info(org, policy_slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str org: (required)
+        :param str policy_slug_perm: (required)
+        :param int page: A page number within the paginated result set.
+        :param int page_size: Number of results to return per page.
+        :return: list[PackageVulnerabilityPolicyEvaluationRequest]
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['org', 'policy_slug_perm', 'page', 'page_size']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method orgs_vulnerability_policy_evaluation_list" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'org' is set
+        if self.api_client.client_side_validation and ('org' not in params or
+                                                       params['org'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `org` when calling `orgs_vulnerability_policy_evaluation_list`")  # noqa: E501
+        # verify the required parameter 'policy_slug_perm' is set
+        if self.api_client.client_side_validation and ('policy_slug_perm' not in params or
+                                                       params['policy_slug_perm'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `policy_slug_perm` when calling `orgs_vulnerability_policy_evaluation_list`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'org' in params:
+            path_params['org'] = params['org']  # noqa: E501
+        if 'policy_slug_perm' in params:
+            path_params['policy_slug_perm'] = params['policy_slug_perm']  # noqa: E501
+
+        query_params = []
+        if 'page' in params:
+            query_params.append(('page', params['page']))  # noqa: E501
+        if 'page_size' in params:
+            query_params.append(('page_size', params['page_size']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/orgs/{org}/vulnerability-policy/{policy_slug_perm}/evaluation/', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='list[PackageVulnerabilityPolicyEvaluationRequest]',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def orgs_vulnerability_policy_evaluation_read(self, org, policy_slug_perm, slug_perm, **kwargs):  # noqa: E501
+        """Retrieve an evaluation request for this policy.  # noqa: E501
+
+        Retrieve an evaluation request for this policy.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.orgs_vulnerability_policy_evaluation_read(org, policy_slug_perm, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str org: (required)
+        :param str policy_slug_perm: (required)
+        :param str slug_perm: (required)
+        :return: PackageVulnerabilityPolicyEvaluationRequest
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.orgs_vulnerability_policy_evaluation_read_with_http_info(org, policy_slug_perm, slug_perm, **kwargs)  # noqa: E501
+        else:
+            (data) = self.orgs_vulnerability_policy_evaluation_read_with_http_info(org, policy_slug_perm, slug_perm, **kwargs)  # noqa: E501
+            return data
+
+    def orgs_vulnerability_policy_evaluation_read_with_http_info(self, org, policy_slug_perm, slug_perm, **kwargs):  # noqa: E501
+        """Retrieve an evaluation request for this policy.  # noqa: E501
+
+        Retrieve an evaluation request for this policy.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.orgs_vulnerability_policy_evaluation_read_with_http_info(org, policy_slug_perm, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str org: (required)
+        :param str policy_slug_perm: (required)
+        :param str slug_perm: (required)
+        :return: PackageVulnerabilityPolicyEvaluationRequest
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['org', 'policy_slug_perm', 'slug_perm']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method orgs_vulnerability_policy_evaluation_read" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'org' is set
+        if self.api_client.client_side_validation and ('org' not in params or
+                                                       params['org'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `org` when calling `orgs_vulnerability_policy_evaluation_read`")  # noqa: E501
+        # verify the required parameter 'policy_slug_perm' is set
+        if self.api_client.client_side_validation and ('policy_slug_perm' not in params or
+                                                       params['policy_slug_perm'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `policy_slug_perm` when calling `orgs_vulnerability_policy_evaluation_read`")  # noqa: E501
+        # verify the required parameter 'slug_perm' is set
+        if self.api_client.client_side_validation and ('slug_perm' not in params or
+                                                       params['slug_perm'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `slug_perm` when calling `orgs_vulnerability_policy_evaluation_read`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'org' in params:
+            path_params['org'] = params['org']  # noqa: E501
+        if 'policy_slug_perm' in params:
+            path_params['policy_slug_perm'] = params['policy_slug_perm']  # noqa: E501
+        if 'slug_perm' in params:
+            path_params['slug_perm'] = params['slug_perm']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/orgs/{org}/vulnerability-policy/{policy_slug_perm}/evaluation/{slug_perm}/', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='PackageVulnerabilityPolicyEvaluationRequest',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def orgs_vulnerability_policy_list(self, org, **kwargs):  # noqa: E501
         """Get a list of all package vulnerability policies.  # noqa: E501
 
         Get a list of all package vulnerability policies.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.orgs_vulnerability_policy_list(org, async_req=True)
```

## cloudsmith_api/api/repos_api.py

```diff
@@ -2213,14 +2213,6954 @@
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def repos_upstream_dart_create(self, owner, identifier, **kwargs):  # noqa: E501
+        """Create a Dart upstream config for this repository.  # noqa: E501
+
+        Create a Dart upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_dart_create(owner, identifier, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param DartUpstreamRequest data:
+        :return: DartUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.repos_upstream_dart_create_with_http_info(owner, identifier, **kwargs)  # noqa: E501
+        else:
+            (data) = self.repos_upstream_dart_create_with_http_info(owner, identifier, **kwargs)  # noqa: E501
+            return data
+
+    def repos_upstream_dart_create_with_http_info(self, owner, identifier, **kwargs):  # noqa: E501
+        """Create a Dart upstream config for this repository.  # noqa: E501
+
+        Create a Dart upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_dart_create_with_http_info(owner, identifier, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param DartUpstreamRequest data:
+        :return: DartUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['owner', 'identifier', 'data']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method repos_upstream_dart_create" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'owner' is set
+        if self.api_client.client_side_validation and ('owner' not in params or
+                                                       params['owner'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `owner` when calling `repos_upstream_dart_create`")  # noqa: E501
+        # verify the required parameter 'identifier' is set
+        if self.api_client.client_side_validation and ('identifier' not in params or
+                                                       params['identifier'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `identifier` when calling `repos_upstream_dart_create`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'owner' in params:
+            path_params['owner'] = params['owner']  # noqa: E501
+        if 'identifier' in params:
+            path_params['identifier'] = params['identifier']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'data' in params:
+            body_params = params['data']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/repos/{owner}/{identifier}/upstream/dart/', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='DartUpstream',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def repos_upstream_dart_delete(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Delete a Dart upstream config for this repository.  # noqa: E501
+
+        Delete a Dart upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_dart_delete(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :return: None
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.repos_upstream_dart_delete_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+        else:
+            (data) = self.repos_upstream_dart_delete_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+            return data
+
+    def repos_upstream_dart_delete_with_http_info(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Delete a Dart upstream config for this repository.  # noqa: E501
+
+        Delete a Dart upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_dart_delete_with_http_info(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :return: None
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['owner', 'identifier', 'slug_perm']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method repos_upstream_dart_delete" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'owner' is set
+        if self.api_client.client_side_validation and ('owner' not in params or
+                                                       params['owner'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `owner` when calling `repos_upstream_dart_delete`")  # noqa: E501
+        # verify the required parameter 'identifier' is set
+        if self.api_client.client_side_validation and ('identifier' not in params or
+                                                       params['identifier'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `identifier` when calling `repos_upstream_dart_delete`")  # noqa: E501
+        # verify the required parameter 'slug_perm' is set
+        if self.api_client.client_side_validation and ('slug_perm' not in params or
+                                                       params['slug_perm'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `slug_perm` when calling `repos_upstream_dart_delete`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'owner' in params:
+            path_params['owner'] = params['owner']  # noqa: E501
+        if 'identifier' in params:
+            path_params['identifier'] = params['identifier']  # noqa: E501
+        if 'slug_perm' in params:
+            path_params['slug_perm'] = params['slug_perm']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/repos/{owner}/{identifier}/upstream/dart/{slug_perm}/', 'DELETE',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type=None,  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def repos_upstream_dart_list(self, owner, identifier, **kwargs):  # noqa: E501
+        """List Dart upstream configs for this repository.  # noqa: E501
+
+        List Dart upstream configs for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_dart_list(owner, identifier, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param int page: A page number within the paginated result set.
+        :param int page_size: Number of results to return per page.
+        :return: list[DartUpstream]
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.repos_upstream_dart_list_with_http_info(owner, identifier, **kwargs)  # noqa: E501
+        else:
+            (data) = self.repos_upstream_dart_list_with_http_info(owner, identifier, **kwargs)  # noqa: E501
+            return data
+
+    def repos_upstream_dart_list_with_http_info(self, owner, identifier, **kwargs):  # noqa: E501
+        """List Dart upstream configs for this repository.  # noqa: E501
+
+        List Dart upstream configs for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_dart_list_with_http_info(owner, identifier, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param int page: A page number within the paginated result set.
+        :param int page_size: Number of results to return per page.
+        :return: list[DartUpstream]
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['owner', 'identifier', 'page', 'page_size']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method repos_upstream_dart_list" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'owner' is set
+        if self.api_client.client_side_validation and ('owner' not in params or
+                                                       params['owner'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `owner` when calling `repos_upstream_dart_list`")  # noqa: E501
+        # verify the required parameter 'identifier' is set
+        if self.api_client.client_side_validation and ('identifier' not in params or
+                                                       params['identifier'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `identifier` when calling `repos_upstream_dart_list`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'owner' in params:
+            path_params['owner'] = params['owner']  # noqa: E501
+        if 'identifier' in params:
+            path_params['identifier'] = params['identifier']  # noqa: E501
+
+        query_params = []
+        if 'page' in params:
+            query_params.append(('page', params['page']))  # noqa: E501
+        if 'page_size' in params:
+            query_params.append(('page_size', params['page_size']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/repos/{owner}/{identifier}/upstream/dart/', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='list[DartUpstream]',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def repos_upstream_dart_partial_update(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Partially update a Dart upstream config for this repository.  # noqa: E501
+
+        Partially update a Dart upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_dart_partial_update(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :param DartUpstreamRequestPatch data:
+        :return: DartUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.repos_upstream_dart_partial_update_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+        else:
+            (data) = self.repos_upstream_dart_partial_update_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+            return data
+
+    def repos_upstream_dart_partial_update_with_http_info(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Partially update a Dart upstream config for this repository.  # noqa: E501
+
+        Partially update a Dart upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_dart_partial_update_with_http_info(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :param DartUpstreamRequestPatch data:
+        :return: DartUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['owner', 'identifier', 'slug_perm', 'data']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method repos_upstream_dart_partial_update" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'owner' is set
+        if self.api_client.client_side_validation and ('owner' not in params or
+                                                       params['owner'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `owner` when calling `repos_upstream_dart_partial_update`")  # noqa: E501
+        # verify the required parameter 'identifier' is set
+        if self.api_client.client_side_validation and ('identifier' not in params or
+                                                       params['identifier'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `identifier` when calling `repos_upstream_dart_partial_update`")  # noqa: E501
+        # verify the required parameter 'slug_perm' is set
+        if self.api_client.client_side_validation and ('slug_perm' not in params or
+                                                       params['slug_perm'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `slug_perm` when calling `repos_upstream_dart_partial_update`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'owner' in params:
+            path_params['owner'] = params['owner']  # noqa: E501
+        if 'identifier' in params:
+            path_params['identifier'] = params['identifier']  # noqa: E501
+        if 'slug_perm' in params:
+            path_params['slug_perm'] = params['slug_perm']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'data' in params:
+            body_params = params['data']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/repos/{owner}/{identifier}/upstream/dart/{slug_perm}/', 'PATCH',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='DartUpstream',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def repos_upstream_dart_read(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Retrieve a Dart upstream config for this repository.  # noqa: E501
+
+        Retrieve a Dart upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_dart_read(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :return: DartUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.repos_upstream_dart_read_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+        else:
+            (data) = self.repos_upstream_dart_read_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+            return data
+
+    def repos_upstream_dart_read_with_http_info(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Retrieve a Dart upstream config for this repository.  # noqa: E501
+
+        Retrieve a Dart upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_dart_read_with_http_info(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :return: DartUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['owner', 'identifier', 'slug_perm']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method repos_upstream_dart_read" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'owner' is set
+        if self.api_client.client_side_validation and ('owner' not in params or
+                                                       params['owner'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `owner` when calling `repos_upstream_dart_read`")  # noqa: E501
+        # verify the required parameter 'identifier' is set
+        if self.api_client.client_side_validation and ('identifier' not in params or
+                                                       params['identifier'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `identifier` when calling `repos_upstream_dart_read`")  # noqa: E501
+        # verify the required parameter 'slug_perm' is set
+        if self.api_client.client_side_validation and ('slug_perm' not in params or
+                                                       params['slug_perm'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `slug_perm` when calling `repos_upstream_dart_read`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'owner' in params:
+            path_params['owner'] = params['owner']  # noqa: E501
+        if 'identifier' in params:
+            path_params['identifier'] = params['identifier']  # noqa: E501
+        if 'slug_perm' in params:
+            path_params['slug_perm'] = params['slug_perm']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/repos/{owner}/{identifier}/upstream/dart/{slug_perm}/', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='DartUpstream',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def repos_upstream_dart_update(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Update a Dart upstream config for this repository.  # noqa: E501
+
+        Update a Dart upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_dart_update(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :param DartUpstreamRequest data:
+        :return: DartUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.repos_upstream_dart_update_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+        else:
+            (data) = self.repos_upstream_dart_update_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+            return data
+
+    def repos_upstream_dart_update_with_http_info(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Update a Dart upstream config for this repository.  # noqa: E501
+
+        Update a Dart upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_dart_update_with_http_info(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :param DartUpstreamRequest data:
+        :return: DartUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['owner', 'identifier', 'slug_perm', 'data']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method repos_upstream_dart_update" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'owner' is set
+        if self.api_client.client_side_validation and ('owner' not in params or
+                                                       params['owner'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `owner` when calling `repos_upstream_dart_update`")  # noqa: E501
+        # verify the required parameter 'identifier' is set
+        if self.api_client.client_side_validation and ('identifier' not in params or
+                                                       params['identifier'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `identifier` when calling `repos_upstream_dart_update`")  # noqa: E501
+        # verify the required parameter 'slug_perm' is set
+        if self.api_client.client_side_validation and ('slug_perm' not in params or
+                                                       params['slug_perm'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `slug_perm` when calling `repos_upstream_dart_update`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'owner' in params:
+            path_params['owner'] = params['owner']  # noqa: E501
+        if 'identifier' in params:
+            path_params['identifier'] = params['identifier']  # noqa: E501
+        if 'slug_perm' in params:
+            path_params['slug_perm'] = params['slug_perm']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'data' in params:
+            body_params = params['data']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/repos/{owner}/{identifier}/upstream/dart/{slug_perm}/', 'PUT',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='DartUpstream',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def repos_upstream_deb_create(self, owner, identifier, **kwargs):  # noqa: E501
+        """Create a Debian upstream config for this repository.  # noqa: E501
+
+        Create a Debian upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_deb_create(owner, identifier, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param DebUpstreamRequest data:
+        :return: DebUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.repos_upstream_deb_create_with_http_info(owner, identifier, **kwargs)  # noqa: E501
+        else:
+            (data) = self.repos_upstream_deb_create_with_http_info(owner, identifier, **kwargs)  # noqa: E501
+            return data
+
+    def repos_upstream_deb_create_with_http_info(self, owner, identifier, **kwargs):  # noqa: E501
+        """Create a Debian upstream config for this repository.  # noqa: E501
+
+        Create a Debian upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_deb_create_with_http_info(owner, identifier, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param DebUpstreamRequest data:
+        :return: DebUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['owner', 'identifier', 'data']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method repos_upstream_deb_create" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'owner' is set
+        if self.api_client.client_side_validation and ('owner' not in params or
+                                                       params['owner'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `owner` when calling `repos_upstream_deb_create`")  # noqa: E501
+        # verify the required parameter 'identifier' is set
+        if self.api_client.client_side_validation and ('identifier' not in params or
+                                                       params['identifier'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `identifier` when calling `repos_upstream_deb_create`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'owner' in params:
+            path_params['owner'] = params['owner']  # noqa: E501
+        if 'identifier' in params:
+            path_params['identifier'] = params['identifier']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'data' in params:
+            body_params = params['data']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/repos/{owner}/{identifier}/upstream/deb/', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='DebUpstream',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def repos_upstream_deb_delete(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Delete a Debian upstream config for this repository.  # noqa: E501
+
+        Delete a Debian upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_deb_delete(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :return: None
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.repos_upstream_deb_delete_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+        else:
+            (data) = self.repos_upstream_deb_delete_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+            return data
+
+    def repos_upstream_deb_delete_with_http_info(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Delete a Debian upstream config for this repository.  # noqa: E501
+
+        Delete a Debian upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_deb_delete_with_http_info(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :return: None
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['owner', 'identifier', 'slug_perm']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method repos_upstream_deb_delete" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'owner' is set
+        if self.api_client.client_side_validation and ('owner' not in params or
+                                                       params['owner'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `owner` when calling `repos_upstream_deb_delete`")  # noqa: E501
+        # verify the required parameter 'identifier' is set
+        if self.api_client.client_side_validation and ('identifier' not in params or
+                                                       params['identifier'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `identifier` when calling `repos_upstream_deb_delete`")  # noqa: E501
+        # verify the required parameter 'slug_perm' is set
+        if self.api_client.client_side_validation and ('slug_perm' not in params or
+                                                       params['slug_perm'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `slug_perm` when calling `repos_upstream_deb_delete`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'owner' in params:
+            path_params['owner'] = params['owner']  # noqa: E501
+        if 'identifier' in params:
+            path_params['identifier'] = params['identifier']  # noqa: E501
+        if 'slug_perm' in params:
+            path_params['slug_perm'] = params['slug_perm']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/repos/{owner}/{identifier}/upstream/deb/{slug_perm}/', 'DELETE',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type=None,  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def repos_upstream_deb_list(self, owner, identifier, **kwargs):  # noqa: E501
+        """List Debian upstream configs for this repository.  # noqa: E501
+
+        List Debian upstream configs for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_deb_list(owner, identifier, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param int page: A page number within the paginated result set.
+        :param int page_size: Number of results to return per page.
+        :return: list[DebUpstream]
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.repos_upstream_deb_list_with_http_info(owner, identifier, **kwargs)  # noqa: E501
+        else:
+            (data) = self.repos_upstream_deb_list_with_http_info(owner, identifier, **kwargs)  # noqa: E501
+            return data
+
+    def repos_upstream_deb_list_with_http_info(self, owner, identifier, **kwargs):  # noqa: E501
+        """List Debian upstream configs for this repository.  # noqa: E501
+
+        List Debian upstream configs for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_deb_list_with_http_info(owner, identifier, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param int page: A page number within the paginated result set.
+        :param int page_size: Number of results to return per page.
+        :return: list[DebUpstream]
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['owner', 'identifier', 'page', 'page_size']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method repos_upstream_deb_list" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'owner' is set
+        if self.api_client.client_side_validation and ('owner' not in params or
+                                                       params['owner'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `owner` when calling `repos_upstream_deb_list`")  # noqa: E501
+        # verify the required parameter 'identifier' is set
+        if self.api_client.client_side_validation and ('identifier' not in params or
+                                                       params['identifier'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `identifier` when calling `repos_upstream_deb_list`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'owner' in params:
+            path_params['owner'] = params['owner']  # noqa: E501
+        if 'identifier' in params:
+            path_params['identifier'] = params['identifier']  # noqa: E501
+
+        query_params = []
+        if 'page' in params:
+            query_params.append(('page', params['page']))  # noqa: E501
+        if 'page_size' in params:
+            query_params.append(('page_size', params['page_size']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/repos/{owner}/{identifier}/upstream/deb/', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='list[DebUpstream]',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def repos_upstream_deb_partial_update(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Partially update a Debian upstream config for this repository.  # noqa: E501
+
+        Partially update a Debian upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_deb_partial_update(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :param DebUpstreamRequestPatch data:
+        :return: DebUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.repos_upstream_deb_partial_update_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+        else:
+            (data) = self.repos_upstream_deb_partial_update_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+            return data
+
+    def repos_upstream_deb_partial_update_with_http_info(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Partially update a Debian upstream config for this repository.  # noqa: E501
+
+        Partially update a Debian upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_deb_partial_update_with_http_info(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :param DebUpstreamRequestPatch data:
+        :return: DebUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['owner', 'identifier', 'slug_perm', 'data']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method repos_upstream_deb_partial_update" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'owner' is set
+        if self.api_client.client_side_validation and ('owner' not in params or
+                                                       params['owner'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `owner` when calling `repos_upstream_deb_partial_update`")  # noqa: E501
+        # verify the required parameter 'identifier' is set
+        if self.api_client.client_side_validation and ('identifier' not in params or
+                                                       params['identifier'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `identifier` when calling `repos_upstream_deb_partial_update`")  # noqa: E501
+        # verify the required parameter 'slug_perm' is set
+        if self.api_client.client_side_validation and ('slug_perm' not in params or
+                                                       params['slug_perm'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `slug_perm` when calling `repos_upstream_deb_partial_update`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'owner' in params:
+            path_params['owner'] = params['owner']  # noqa: E501
+        if 'identifier' in params:
+            path_params['identifier'] = params['identifier']  # noqa: E501
+        if 'slug_perm' in params:
+            path_params['slug_perm'] = params['slug_perm']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'data' in params:
+            body_params = params['data']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/repos/{owner}/{identifier}/upstream/deb/{slug_perm}/', 'PATCH',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='DebUpstream',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def repos_upstream_deb_read(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Retrieve a Debian upstream config for this repository.  # noqa: E501
+
+        Retrieve a Debian upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_deb_read(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :return: DebUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.repos_upstream_deb_read_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+        else:
+            (data) = self.repos_upstream_deb_read_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+            return data
+
+    def repos_upstream_deb_read_with_http_info(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Retrieve a Debian upstream config for this repository.  # noqa: E501
+
+        Retrieve a Debian upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_deb_read_with_http_info(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :return: DebUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['owner', 'identifier', 'slug_perm']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method repos_upstream_deb_read" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'owner' is set
+        if self.api_client.client_side_validation and ('owner' not in params or
+                                                       params['owner'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `owner` when calling `repos_upstream_deb_read`")  # noqa: E501
+        # verify the required parameter 'identifier' is set
+        if self.api_client.client_side_validation and ('identifier' not in params or
+                                                       params['identifier'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `identifier` when calling `repos_upstream_deb_read`")  # noqa: E501
+        # verify the required parameter 'slug_perm' is set
+        if self.api_client.client_side_validation and ('slug_perm' not in params or
+                                                       params['slug_perm'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `slug_perm` when calling `repos_upstream_deb_read`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'owner' in params:
+            path_params['owner'] = params['owner']  # noqa: E501
+        if 'identifier' in params:
+            path_params['identifier'] = params['identifier']  # noqa: E501
+        if 'slug_perm' in params:
+            path_params['slug_perm'] = params['slug_perm']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/repos/{owner}/{identifier}/upstream/deb/{slug_perm}/', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='DebUpstream',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def repos_upstream_deb_update(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Update a Debian upstream config for this repository.  # noqa: E501
+
+        Update a Debian upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_deb_update(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :param DebUpstreamRequest data:
+        :return: DebUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.repos_upstream_deb_update_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+        else:
+            (data) = self.repos_upstream_deb_update_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+            return data
+
+    def repos_upstream_deb_update_with_http_info(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Update a Debian upstream config for this repository.  # noqa: E501
+
+        Update a Debian upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_deb_update_with_http_info(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :param DebUpstreamRequest data:
+        :return: DebUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['owner', 'identifier', 'slug_perm', 'data']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method repos_upstream_deb_update" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'owner' is set
+        if self.api_client.client_side_validation and ('owner' not in params or
+                                                       params['owner'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `owner` when calling `repos_upstream_deb_update`")  # noqa: E501
+        # verify the required parameter 'identifier' is set
+        if self.api_client.client_side_validation and ('identifier' not in params or
+                                                       params['identifier'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `identifier` when calling `repos_upstream_deb_update`")  # noqa: E501
+        # verify the required parameter 'slug_perm' is set
+        if self.api_client.client_side_validation and ('slug_perm' not in params or
+                                                       params['slug_perm'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `slug_perm` when calling `repos_upstream_deb_update`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'owner' in params:
+            path_params['owner'] = params['owner']  # noqa: E501
+        if 'identifier' in params:
+            path_params['identifier'] = params['identifier']  # noqa: E501
+        if 'slug_perm' in params:
+            path_params['slug_perm'] = params['slug_perm']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'data' in params:
+            body_params = params['data']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/repos/{owner}/{identifier}/upstream/deb/{slug_perm}/', 'PUT',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='DebUpstream',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def repos_upstream_docker_create(self, owner, identifier, **kwargs):  # noqa: E501
+        """Create a Docker upstream config for this repository.  # noqa: E501
+
+        Create a Docker upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_docker_create(owner, identifier, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param DockerUpstreamRequest data:
+        :return: DockerUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.repos_upstream_docker_create_with_http_info(owner, identifier, **kwargs)  # noqa: E501
+        else:
+            (data) = self.repos_upstream_docker_create_with_http_info(owner, identifier, **kwargs)  # noqa: E501
+            return data
+
+    def repos_upstream_docker_create_with_http_info(self, owner, identifier, **kwargs):  # noqa: E501
+        """Create a Docker upstream config for this repository.  # noqa: E501
+
+        Create a Docker upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_docker_create_with_http_info(owner, identifier, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param DockerUpstreamRequest data:
+        :return: DockerUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['owner', 'identifier', 'data']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method repos_upstream_docker_create" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'owner' is set
+        if self.api_client.client_side_validation and ('owner' not in params or
+                                                       params['owner'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `owner` when calling `repos_upstream_docker_create`")  # noqa: E501
+        # verify the required parameter 'identifier' is set
+        if self.api_client.client_side_validation and ('identifier' not in params or
+                                                       params['identifier'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `identifier` when calling `repos_upstream_docker_create`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'owner' in params:
+            path_params['owner'] = params['owner']  # noqa: E501
+        if 'identifier' in params:
+            path_params['identifier'] = params['identifier']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'data' in params:
+            body_params = params['data']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/repos/{owner}/{identifier}/upstream/docker/', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='DockerUpstream',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def repos_upstream_docker_delete(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Delete a Docker upstream config for this repository.  # noqa: E501
+
+        Delete a Docker upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_docker_delete(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :return: None
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.repos_upstream_docker_delete_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+        else:
+            (data) = self.repos_upstream_docker_delete_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+            return data
+
+    def repos_upstream_docker_delete_with_http_info(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Delete a Docker upstream config for this repository.  # noqa: E501
+
+        Delete a Docker upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_docker_delete_with_http_info(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :return: None
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['owner', 'identifier', 'slug_perm']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method repos_upstream_docker_delete" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'owner' is set
+        if self.api_client.client_side_validation and ('owner' not in params or
+                                                       params['owner'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `owner` when calling `repos_upstream_docker_delete`")  # noqa: E501
+        # verify the required parameter 'identifier' is set
+        if self.api_client.client_side_validation and ('identifier' not in params or
+                                                       params['identifier'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `identifier` when calling `repos_upstream_docker_delete`")  # noqa: E501
+        # verify the required parameter 'slug_perm' is set
+        if self.api_client.client_side_validation and ('slug_perm' not in params or
+                                                       params['slug_perm'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `slug_perm` when calling `repos_upstream_docker_delete`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'owner' in params:
+            path_params['owner'] = params['owner']  # noqa: E501
+        if 'identifier' in params:
+            path_params['identifier'] = params['identifier']  # noqa: E501
+        if 'slug_perm' in params:
+            path_params['slug_perm'] = params['slug_perm']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/repos/{owner}/{identifier}/upstream/docker/{slug_perm}/', 'DELETE',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type=None,  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def repos_upstream_docker_list(self, owner, identifier, **kwargs):  # noqa: E501
+        """List Docker upstream configs for this repository.  # noqa: E501
+
+        List Docker upstream configs for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_docker_list(owner, identifier, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param int page: A page number within the paginated result set.
+        :param int page_size: Number of results to return per page.
+        :return: list[DockerUpstream]
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.repos_upstream_docker_list_with_http_info(owner, identifier, **kwargs)  # noqa: E501
+        else:
+            (data) = self.repos_upstream_docker_list_with_http_info(owner, identifier, **kwargs)  # noqa: E501
+            return data
+
+    def repos_upstream_docker_list_with_http_info(self, owner, identifier, **kwargs):  # noqa: E501
+        """List Docker upstream configs for this repository.  # noqa: E501
+
+        List Docker upstream configs for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_docker_list_with_http_info(owner, identifier, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param int page: A page number within the paginated result set.
+        :param int page_size: Number of results to return per page.
+        :return: list[DockerUpstream]
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['owner', 'identifier', 'page', 'page_size']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method repos_upstream_docker_list" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'owner' is set
+        if self.api_client.client_side_validation and ('owner' not in params or
+                                                       params['owner'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `owner` when calling `repos_upstream_docker_list`")  # noqa: E501
+        # verify the required parameter 'identifier' is set
+        if self.api_client.client_side_validation and ('identifier' not in params or
+                                                       params['identifier'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `identifier` when calling `repos_upstream_docker_list`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'owner' in params:
+            path_params['owner'] = params['owner']  # noqa: E501
+        if 'identifier' in params:
+            path_params['identifier'] = params['identifier']  # noqa: E501
+
+        query_params = []
+        if 'page' in params:
+            query_params.append(('page', params['page']))  # noqa: E501
+        if 'page_size' in params:
+            query_params.append(('page_size', params['page_size']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/repos/{owner}/{identifier}/upstream/docker/', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='list[DockerUpstream]',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def repos_upstream_docker_partial_update(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Partially update a Docker upstream config for this repository.  # noqa: E501
+
+        Partially update a Docker upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_docker_partial_update(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :param DockerUpstreamRequestPatch data:
+        :return: DockerUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.repos_upstream_docker_partial_update_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+        else:
+            (data) = self.repos_upstream_docker_partial_update_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+            return data
+
+    def repos_upstream_docker_partial_update_with_http_info(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Partially update a Docker upstream config for this repository.  # noqa: E501
+
+        Partially update a Docker upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_docker_partial_update_with_http_info(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :param DockerUpstreamRequestPatch data:
+        :return: DockerUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['owner', 'identifier', 'slug_perm', 'data']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method repos_upstream_docker_partial_update" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'owner' is set
+        if self.api_client.client_side_validation and ('owner' not in params or
+                                                       params['owner'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `owner` when calling `repos_upstream_docker_partial_update`")  # noqa: E501
+        # verify the required parameter 'identifier' is set
+        if self.api_client.client_side_validation and ('identifier' not in params or
+                                                       params['identifier'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `identifier` when calling `repos_upstream_docker_partial_update`")  # noqa: E501
+        # verify the required parameter 'slug_perm' is set
+        if self.api_client.client_side_validation and ('slug_perm' not in params or
+                                                       params['slug_perm'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `slug_perm` when calling `repos_upstream_docker_partial_update`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'owner' in params:
+            path_params['owner'] = params['owner']  # noqa: E501
+        if 'identifier' in params:
+            path_params['identifier'] = params['identifier']  # noqa: E501
+        if 'slug_perm' in params:
+            path_params['slug_perm'] = params['slug_perm']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'data' in params:
+            body_params = params['data']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/repos/{owner}/{identifier}/upstream/docker/{slug_perm}/', 'PATCH',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='DockerUpstream',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def repos_upstream_docker_read(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Retrieve a Docker upstream config for this repository.  # noqa: E501
+
+        Retrieve a Docker upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_docker_read(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :return: DockerUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.repos_upstream_docker_read_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+        else:
+            (data) = self.repos_upstream_docker_read_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+            return data
+
+    def repos_upstream_docker_read_with_http_info(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Retrieve a Docker upstream config for this repository.  # noqa: E501
+
+        Retrieve a Docker upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_docker_read_with_http_info(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :return: DockerUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['owner', 'identifier', 'slug_perm']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method repos_upstream_docker_read" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'owner' is set
+        if self.api_client.client_side_validation and ('owner' not in params or
+                                                       params['owner'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `owner` when calling `repos_upstream_docker_read`")  # noqa: E501
+        # verify the required parameter 'identifier' is set
+        if self.api_client.client_side_validation and ('identifier' not in params or
+                                                       params['identifier'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `identifier` when calling `repos_upstream_docker_read`")  # noqa: E501
+        # verify the required parameter 'slug_perm' is set
+        if self.api_client.client_side_validation and ('slug_perm' not in params or
+                                                       params['slug_perm'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `slug_perm` when calling `repos_upstream_docker_read`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'owner' in params:
+            path_params['owner'] = params['owner']  # noqa: E501
+        if 'identifier' in params:
+            path_params['identifier'] = params['identifier']  # noqa: E501
+        if 'slug_perm' in params:
+            path_params['slug_perm'] = params['slug_perm']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/repos/{owner}/{identifier}/upstream/docker/{slug_perm}/', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='DockerUpstream',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def repos_upstream_docker_update(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Update a Docker upstream config for this repository.  # noqa: E501
+
+        Update a Docker upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_docker_update(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :param DockerUpstreamRequest data:
+        :return: DockerUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.repos_upstream_docker_update_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+        else:
+            (data) = self.repos_upstream_docker_update_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+            return data
+
+    def repos_upstream_docker_update_with_http_info(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Update a Docker upstream config for this repository.  # noqa: E501
+
+        Update a Docker upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_docker_update_with_http_info(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :param DockerUpstreamRequest data:
+        :return: DockerUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['owner', 'identifier', 'slug_perm', 'data']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method repos_upstream_docker_update" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'owner' is set
+        if self.api_client.client_side_validation and ('owner' not in params or
+                                                       params['owner'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `owner` when calling `repos_upstream_docker_update`")  # noqa: E501
+        # verify the required parameter 'identifier' is set
+        if self.api_client.client_side_validation and ('identifier' not in params or
+                                                       params['identifier'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `identifier` when calling `repos_upstream_docker_update`")  # noqa: E501
+        # verify the required parameter 'slug_perm' is set
+        if self.api_client.client_side_validation and ('slug_perm' not in params or
+                                                       params['slug_perm'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `slug_perm` when calling `repos_upstream_docker_update`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'owner' in params:
+            path_params['owner'] = params['owner']  # noqa: E501
+        if 'identifier' in params:
+            path_params['identifier'] = params['identifier']  # noqa: E501
+        if 'slug_perm' in params:
+            path_params['slug_perm'] = params['slug_perm']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'data' in params:
+            body_params = params['data']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/repos/{owner}/{identifier}/upstream/docker/{slug_perm}/', 'PUT',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='DockerUpstream',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def repos_upstream_helm_create(self, owner, identifier, **kwargs):  # noqa: E501
+        """Create a Helm upstream config for this repository.  # noqa: E501
+
+        Create a Helm upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_helm_create(owner, identifier, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param HelmUpstreamRequest data:
+        :return: HelmUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.repos_upstream_helm_create_with_http_info(owner, identifier, **kwargs)  # noqa: E501
+        else:
+            (data) = self.repos_upstream_helm_create_with_http_info(owner, identifier, **kwargs)  # noqa: E501
+            return data
+
+    def repos_upstream_helm_create_with_http_info(self, owner, identifier, **kwargs):  # noqa: E501
+        """Create a Helm upstream config for this repository.  # noqa: E501
+
+        Create a Helm upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_helm_create_with_http_info(owner, identifier, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param HelmUpstreamRequest data:
+        :return: HelmUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['owner', 'identifier', 'data']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method repos_upstream_helm_create" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'owner' is set
+        if self.api_client.client_side_validation and ('owner' not in params or
+                                                       params['owner'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `owner` when calling `repos_upstream_helm_create`")  # noqa: E501
+        # verify the required parameter 'identifier' is set
+        if self.api_client.client_side_validation and ('identifier' not in params or
+                                                       params['identifier'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `identifier` when calling `repos_upstream_helm_create`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'owner' in params:
+            path_params['owner'] = params['owner']  # noqa: E501
+        if 'identifier' in params:
+            path_params['identifier'] = params['identifier']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'data' in params:
+            body_params = params['data']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/repos/{owner}/{identifier}/upstream/helm/', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='HelmUpstream',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def repos_upstream_helm_delete(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Delete a Helm upstream config for this repository.  # noqa: E501
+
+        Delete a Helm upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_helm_delete(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :return: None
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.repos_upstream_helm_delete_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+        else:
+            (data) = self.repos_upstream_helm_delete_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+            return data
+
+    def repos_upstream_helm_delete_with_http_info(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Delete a Helm upstream config for this repository.  # noqa: E501
+
+        Delete a Helm upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_helm_delete_with_http_info(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :return: None
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['owner', 'identifier', 'slug_perm']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method repos_upstream_helm_delete" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'owner' is set
+        if self.api_client.client_side_validation and ('owner' not in params or
+                                                       params['owner'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `owner` when calling `repos_upstream_helm_delete`")  # noqa: E501
+        # verify the required parameter 'identifier' is set
+        if self.api_client.client_side_validation and ('identifier' not in params or
+                                                       params['identifier'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `identifier` when calling `repos_upstream_helm_delete`")  # noqa: E501
+        # verify the required parameter 'slug_perm' is set
+        if self.api_client.client_side_validation and ('slug_perm' not in params or
+                                                       params['slug_perm'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `slug_perm` when calling `repos_upstream_helm_delete`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'owner' in params:
+            path_params['owner'] = params['owner']  # noqa: E501
+        if 'identifier' in params:
+            path_params['identifier'] = params['identifier']  # noqa: E501
+        if 'slug_perm' in params:
+            path_params['slug_perm'] = params['slug_perm']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/repos/{owner}/{identifier}/upstream/helm/{slug_perm}/', 'DELETE',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type=None,  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def repos_upstream_helm_list(self, owner, identifier, **kwargs):  # noqa: E501
+        """List Helm upstream configs for this repository.  # noqa: E501
+
+        List Helm upstream configs for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_helm_list(owner, identifier, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param int page: A page number within the paginated result set.
+        :param int page_size: Number of results to return per page.
+        :return: list[HelmUpstream]
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.repos_upstream_helm_list_with_http_info(owner, identifier, **kwargs)  # noqa: E501
+        else:
+            (data) = self.repos_upstream_helm_list_with_http_info(owner, identifier, **kwargs)  # noqa: E501
+            return data
+
+    def repos_upstream_helm_list_with_http_info(self, owner, identifier, **kwargs):  # noqa: E501
+        """List Helm upstream configs for this repository.  # noqa: E501
+
+        List Helm upstream configs for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_helm_list_with_http_info(owner, identifier, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param int page: A page number within the paginated result set.
+        :param int page_size: Number of results to return per page.
+        :return: list[HelmUpstream]
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['owner', 'identifier', 'page', 'page_size']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method repos_upstream_helm_list" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'owner' is set
+        if self.api_client.client_side_validation and ('owner' not in params or
+                                                       params['owner'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `owner` when calling `repos_upstream_helm_list`")  # noqa: E501
+        # verify the required parameter 'identifier' is set
+        if self.api_client.client_side_validation and ('identifier' not in params or
+                                                       params['identifier'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `identifier` when calling `repos_upstream_helm_list`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'owner' in params:
+            path_params['owner'] = params['owner']  # noqa: E501
+        if 'identifier' in params:
+            path_params['identifier'] = params['identifier']  # noqa: E501
+
+        query_params = []
+        if 'page' in params:
+            query_params.append(('page', params['page']))  # noqa: E501
+        if 'page_size' in params:
+            query_params.append(('page_size', params['page_size']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/repos/{owner}/{identifier}/upstream/helm/', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='list[HelmUpstream]',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def repos_upstream_helm_partial_update(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Partially update a Helm upstream config for this repository.  # noqa: E501
+
+        Partially update a Helm upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_helm_partial_update(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :param HelmUpstreamRequestPatch data:
+        :return: HelmUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.repos_upstream_helm_partial_update_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+        else:
+            (data) = self.repos_upstream_helm_partial_update_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+            return data
+
+    def repos_upstream_helm_partial_update_with_http_info(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Partially update a Helm upstream config for this repository.  # noqa: E501
+
+        Partially update a Helm upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_helm_partial_update_with_http_info(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :param HelmUpstreamRequestPatch data:
+        :return: HelmUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['owner', 'identifier', 'slug_perm', 'data']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method repos_upstream_helm_partial_update" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'owner' is set
+        if self.api_client.client_side_validation and ('owner' not in params or
+                                                       params['owner'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `owner` when calling `repos_upstream_helm_partial_update`")  # noqa: E501
+        # verify the required parameter 'identifier' is set
+        if self.api_client.client_side_validation and ('identifier' not in params or
+                                                       params['identifier'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `identifier` when calling `repos_upstream_helm_partial_update`")  # noqa: E501
+        # verify the required parameter 'slug_perm' is set
+        if self.api_client.client_side_validation and ('slug_perm' not in params or
+                                                       params['slug_perm'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `slug_perm` when calling `repos_upstream_helm_partial_update`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'owner' in params:
+            path_params['owner'] = params['owner']  # noqa: E501
+        if 'identifier' in params:
+            path_params['identifier'] = params['identifier']  # noqa: E501
+        if 'slug_perm' in params:
+            path_params['slug_perm'] = params['slug_perm']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'data' in params:
+            body_params = params['data']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/repos/{owner}/{identifier}/upstream/helm/{slug_perm}/', 'PATCH',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='HelmUpstream',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def repos_upstream_helm_read(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Retrieve a Helm upstream config for this repository.  # noqa: E501
+
+        Retrieve a Helm upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_helm_read(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :return: HelmUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.repos_upstream_helm_read_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+        else:
+            (data) = self.repos_upstream_helm_read_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+            return data
+
+    def repos_upstream_helm_read_with_http_info(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Retrieve a Helm upstream config for this repository.  # noqa: E501
+
+        Retrieve a Helm upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_helm_read_with_http_info(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :return: HelmUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['owner', 'identifier', 'slug_perm']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method repos_upstream_helm_read" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'owner' is set
+        if self.api_client.client_side_validation and ('owner' not in params or
+                                                       params['owner'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `owner` when calling `repos_upstream_helm_read`")  # noqa: E501
+        # verify the required parameter 'identifier' is set
+        if self.api_client.client_side_validation and ('identifier' not in params or
+                                                       params['identifier'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `identifier` when calling `repos_upstream_helm_read`")  # noqa: E501
+        # verify the required parameter 'slug_perm' is set
+        if self.api_client.client_side_validation and ('slug_perm' not in params or
+                                                       params['slug_perm'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `slug_perm` when calling `repos_upstream_helm_read`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'owner' in params:
+            path_params['owner'] = params['owner']  # noqa: E501
+        if 'identifier' in params:
+            path_params['identifier'] = params['identifier']  # noqa: E501
+        if 'slug_perm' in params:
+            path_params['slug_perm'] = params['slug_perm']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/repos/{owner}/{identifier}/upstream/helm/{slug_perm}/', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='HelmUpstream',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def repos_upstream_helm_update(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Update a Helm upstream config for this repository.  # noqa: E501
+
+        Update a Helm upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_helm_update(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :param HelmUpstreamRequest data:
+        :return: HelmUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.repos_upstream_helm_update_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+        else:
+            (data) = self.repos_upstream_helm_update_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+            return data
+
+    def repos_upstream_helm_update_with_http_info(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Update a Helm upstream config for this repository.  # noqa: E501
+
+        Update a Helm upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_helm_update_with_http_info(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :param HelmUpstreamRequest data:
+        :return: HelmUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['owner', 'identifier', 'slug_perm', 'data']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method repos_upstream_helm_update" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'owner' is set
+        if self.api_client.client_side_validation and ('owner' not in params or
+                                                       params['owner'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `owner` when calling `repos_upstream_helm_update`")  # noqa: E501
+        # verify the required parameter 'identifier' is set
+        if self.api_client.client_side_validation and ('identifier' not in params or
+                                                       params['identifier'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `identifier` when calling `repos_upstream_helm_update`")  # noqa: E501
+        # verify the required parameter 'slug_perm' is set
+        if self.api_client.client_side_validation and ('slug_perm' not in params or
+                                                       params['slug_perm'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `slug_perm` when calling `repos_upstream_helm_update`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'owner' in params:
+            path_params['owner'] = params['owner']  # noqa: E501
+        if 'identifier' in params:
+            path_params['identifier'] = params['identifier']  # noqa: E501
+        if 'slug_perm' in params:
+            path_params['slug_perm'] = params['slug_perm']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'data' in params:
+            body_params = params['data']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/repos/{owner}/{identifier}/upstream/helm/{slug_perm}/', 'PUT',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='HelmUpstream',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def repos_upstream_maven_create(self, owner, identifier, **kwargs):  # noqa: E501
+        """Create a Maven upstream config for this repository.  # noqa: E501
+
+        Create a Maven upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_maven_create(owner, identifier, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param MavenUpstreamRequest data:
+        :return: MavenUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.repos_upstream_maven_create_with_http_info(owner, identifier, **kwargs)  # noqa: E501
+        else:
+            (data) = self.repos_upstream_maven_create_with_http_info(owner, identifier, **kwargs)  # noqa: E501
+            return data
+
+    def repos_upstream_maven_create_with_http_info(self, owner, identifier, **kwargs):  # noqa: E501
+        """Create a Maven upstream config for this repository.  # noqa: E501
+
+        Create a Maven upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_maven_create_with_http_info(owner, identifier, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param MavenUpstreamRequest data:
+        :return: MavenUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['owner', 'identifier', 'data']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method repos_upstream_maven_create" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'owner' is set
+        if self.api_client.client_side_validation and ('owner' not in params or
+                                                       params['owner'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `owner` when calling `repos_upstream_maven_create`")  # noqa: E501
+        # verify the required parameter 'identifier' is set
+        if self.api_client.client_side_validation and ('identifier' not in params or
+                                                       params['identifier'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `identifier` when calling `repos_upstream_maven_create`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'owner' in params:
+            path_params['owner'] = params['owner']  # noqa: E501
+        if 'identifier' in params:
+            path_params['identifier'] = params['identifier']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'data' in params:
+            body_params = params['data']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/repos/{owner}/{identifier}/upstream/maven/', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='MavenUpstream',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def repos_upstream_maven_delete(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Delete a Maven upstream config for this repository.  # noqa: E501
+
+        Delete a Maven upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_maven_delete(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :return: None
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.repos_upstream_maven_delete_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+        else:
+            (data) = self.repos_upstream_maven_delete_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+            return data
+
+    def repos_upstream_maven_delete_with_http_info(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Delete a Maven upstream config for this repository.  # noqa: E501
+
+        Delete a Maven upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_maven_delete_with_http_info(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :return: None
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['owner', 'identifier', 'slug_perm']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method repos_upstream_maven_delete" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'owner' is set
+        if self.api_client.client_side_validation and ('owner' not in params or
+                                                       params['owner'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `owner` when calling `repos_upstream_maven_delete`")  # noqa: E501
+        # verify the required parameter 'identifier' is set
+        if self.api_client.client_side_validation and ('identifier' not in params or
+                                                       params['identifier'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `identifier` when calling `repos_upstream_maven_delete`")  # noqa: E501
+        # verify the required parameter 'slug_perm' is set
+        if self.api_client.client_side_validation and ('slug_perm' not in params or
+                                                       params['slug_perm'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `slug_perm` when calling `repos_upstream_maven_delete`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'owner' in params:
+            path_params['owner'] = params['owner']  # noqa: E501
+        if 'identifier' in params:
+            path_params['identifier'] = params['identifier']  # noqa: E501
+        if 'slug_perm' in params:
+            path_params['slug_perm'] = params['slug_perm']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/repos/{owner}/{identifier}/upstream/maven/{slug_perm}/', 'DELETE',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type=None,  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def repos_upstream_maven_list(self, owner, identifier, **kwargs):  # noqa: E501
+        """List Maven upstream configs for this repository.  # noqa: E501
+
+        List Maven upstream configs for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_maven_list(owner, identifier, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param int page: A page number within the paginated result set.
+        :param int page_size: Number of results to return per page.
+        :return: list[MavenUpstream]
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.repos_upstream_maven_list_with_http_info(owner, identifier, **kwargs)  # noqa: E501
+        else:
+            (data) = self.repos_upstream_maven_list_with_http_info(owner, identifier, **kwargs)  # noqa: E501
+            return data
+
+    def repos_upstream_maven_list_with_http_info(self, owner, identifier, **kwargs):  # noqa: E501
+        """List Maven upstream configs for this repository.  # noqa: E501
+
+        List Maven upstream configs for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_maven_list_with_http_info(owner, identifier, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param int page: A page number within the paginated result set.
+        :param int page_size: Number of results to return per page.
+        :return: list[MavenUpstream]
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['owner', 'identifier', 'page', 'page_size']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method repos_upstream_maven_list" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'owner' is set
+        if self.api_client.client_side_validation and ('owner' not in params or
+                                                       params['owner'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `owner` when calling `repos_upstream_maven_list`")  # noqa: E501
+        # verify the required parameter 'identifier' is set
+        if self.api_client.client_side_validation and ('identifier' not in params or
+                                                       params['identifier'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `identifier` when calling `repos_upstream_maven_list`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'owner' in params:
+            path_params['owner'] = params['owner']  # noqa: E501
+        if 'identifier' in params:
+            path_params['identifier'] = params['identifier']  # noqa: E501
+
+        query_params = []
+        if 'page' in params:
+            query_params.append(('page', params['page']))  # noqa: E501
+        if 'page_size' in params:
+            query_params.append(('page_size', params['page_size']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/repos/{owner}/{identifier}/upstream/maven/', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='list[MavenUpstream]',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def repos_upstream_maven_partial_update(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Partially update a Maven upstream config for this repository.  # noqa: E501
+
+        Partially update a Maven upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_maven_partial_update(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :param MavenUpstreamRequestPatch data:
+        :return: MavenUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.repos_upstream_maven_partial_update_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+        else:
+            (data) = self.repos_upstream_maven_partial_update_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+            return data
+
+    def repos_upstream_maven_partial_update_with_http_info(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Partially update a Maven upstream config for this repository.  # noqa: E501
+
+        Partially update a Maven upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_maven_partial_update_with_http_info(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :param MavenUpstreamRequestPatch data:
+        :return: MavenUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['owner', 'identifier', 'slug_perm', 'data']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method repos_upstream_maven_partial_update" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'owner' is set
+        if self.api_client.client_side_validation and ('owner' not in params or
+                                                       params['owner'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `owner` when calling `repos_upstream_maven_partial_update`")  # noqa: E501
+        # verify the required parameter 'identifier' is set
+        if self.api_client.client_side_validation and ('identifier' not in params or
+                                                       params['identifier'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `identifier` when calling `repos_upstream_maven_partial_update`")  # noqa: E501
+        # verify the required parameter 'slug_perm' is set
+        if self.api_client.client_side_validation and ('slug_perm' not in params or
+                                                       params['slug_perm'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `slug_perm` when calling `repos_upstream_maven_partial_update`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'owner' in params:
+            path_params['owner'] = params['owner']  # noqa: E501
+        if 'identifier' in params:
+            path_params['identifier'] = params['identifier']  # noqa: E501
+        if 'slug_perm' in params:
+            path_params['slug_perm'] = params['slug_perm']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'data' in params:
+            body_params = params['data']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/repos/{owner}/{identifier}/upstream/maven/{slug_perm}/', 'PATCH',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='MavenUpstream',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def repos_upstream_maven_read(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Retrieve a Maven upstream config for this repository.  # noqa: E501
+
+        Retrieve a Maven upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_maven_read(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :return: MavenUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.repos_upstream_maven_read_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+        else:
+            (data) = self.repos_upstream_maven_read_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+            return data
+
+    def repos_upstream_maven_read_with_http_info(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Retrieve a Maven upstream config for this repository.  # noqa: E501
+
+        Retrieve a Maven upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_maven_read_with_http_info(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :return: MavenUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['owner', 'identifier', 'slug_perm']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method repos_upstream_maven_read" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'owner' is set
+        if self.api_client.client_side_validation and ('owner' not in params or
+                                                       params['owner'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `owner` when calling `repos_upstream_maven_read`")  # noqa: E501
+        # verify the required parameter 'identifier' is set
+        if self.api_client.client_side_validation and ('identifier' not in params or
+                                                       params['identifier'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `identifier` when calling `repos_upstream_maven_read`")  # noqa: E501
+        # verify the required parameter 'slug_perm' is set
+        if self.api_client.client_side_validation and ('slug_perm' not in params or
+                                                       params['slug_perm'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `slug_perm` when calling `repos_upstream_maven_read`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'owner' in params:
+            path_params['owner'] = params['owner']  # noqa: E501
+        if 'identifier' in params:
+            path_params['identifier'] = params['identifier']  # noqa: E501
+        if 'slug_perm' in params:
+            path_params['slug_perm'] = params['slug_perm']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/repos/{owner}/{identifier}/upstream/maven/{slug_perm}/', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='MavenUpstream',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def repos_upstream_maven_update(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Update a Maven upstream config for this repository.  # noqa: E501
+
+        Update a Maven upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_maven_update(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :param MavenUpstreamRequest data:
+        :return: MavenUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.repos_upstream_maven_update_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+        else:
+            (data) = self.repos_upstream_maven_update_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+            return data
+
+    def repos_upstream_maven_update_with_http_info(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Update a Maven upstream config for this repository.  # noqa: E501
+
+        Update a Maven upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_maven_update_with_http_info(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :param MavenUpstreamRequest data:
+        :return: MavenUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['owner', 'identifier', 'slug_perm', 'data']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method repos_upstream_maven_update" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'owner' is set
+        if self.api_client.client_side_validation and ('owner' not in params or
+                                                       params['owner'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `owner` when calling `repos_upstream_maven_update`")  # noqa: E501
+        # verify the required parameter 'identifier' is set
+        if self.api_client.client_side_validation and ('identifier' not in params or
+                                                       params['identifier'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `identifier` when calling `repos_upstream_maven_update`")  # noqa: E501
+        # verify the required parameter 'slug_perm' is set
+        if self.api_client.client_side_validation and ('slug_perm' not in params or
+                                                       params['slug_perm'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `slug_perm` when calling `repos_upstream_maven_update`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'owner' in params:
+            path_params['owner'] = params['owner']  # noqa: E501
+        if 'identifier' in params:
+            path_params['identifier'] = params['identifier']  # noqa: E501
+        if 'slug_perm' in params:
+            path_params['slug_perm'] = params['slug_perm']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'data' in params:
+            body_params = params['data']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/repos/{owner}/{identifier}/upstream/maven/{slug_perm}/', 'PUT',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='MavenUpstream',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def repos_upstream_npm_create(self, owner, identifier, **kwargs):  # noqa: E501
+        """Create a npm upstream config for this repository.  # noqa: E501
+
+        Create a npm upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_npm_create(owner, identifier, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param NpmUpstreamRequest data:
+        :return: NpmUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.repos_upstream_npm_create_with_http_info(owner, identifier, **kwargs)  # noqa: E501
+        else:
+            (data) = self.repos_upstream_npm_create_with_http_info(owner, identifier, **kwargs)  # noqa: E501
+            return data
+
+    def repos_upstream_npm_create_with_http_info(self, owner, identifier, **kwargs):  # noqa: E501
+        """Create a npm upstream config for this repository.  # noqa: E501
+
+        Create a npm upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_npm_create_with_http_info(owner, identifier, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param NpmUpstreamRequest data:
+        :return: NpmUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['owner', 'identifier', 'data']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method repos_upstream_npm_create" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'owner' is set
+        if self.api_client.client_side_validation and ('owner' not in params or
+                                                       params['owner'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `owner` when calling `repos_upstream_npm_create`")  # noqa: E501
+        # verify the required parameter 'identifier' is set
+        if self.api_client.client_side_validation and ('identifier' not in params or
+                                                       params['identifier'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `identifier` when calling `repos_upstream_npm_create`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'owner' in params:
+            path_params['owner'] = params['owner']  # noqa: E501
+        if 'identifier' in params:
+            path_params['identifier'] = params['identifier']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'data' in params:
+            body_params = params['data']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/repos/{owner}/{identifier}/upstream/npm/', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='NpmUpstream',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def repos_upstream_npm_delete(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Delete a npm upstream config for this repository.  # noqa: E501
+
+        Delete a npm upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_npm_delete(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :return: None
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.repos_upstream_npm_delete_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+        else:
+            (data) = self.repos_upstream_npm_delete_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+            return data
+
+    def repos_upstream_npm_delete_with_http_info(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Delete a npm upstream config for this repository.  # noqa: E501
+
+        Delete a npm upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_npm_delete_with_http_info(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :return: None
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['owner', 'identifier', 'slug_perm']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method repos_upstream_npm_delete" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'owner' is set
+        if self.api_client.client_side_validation and ('owner' not in params or
+                                                       params['owner'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `owner` when calling `repos_upstream_npm_delete`")  # noqa: E501
+        # verify the required parameter 'identifier' is set
+        if self.api_client.client_side_validation and ('identifier' not in params or
+                                                       params['identifier'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `identifier` when calling `repos_upstream_npm_delete`")  # noqa: E501
+        # verify the required parameter 'slug_perm' is set
+        if self.api_client.client_side_validation and ('slug_perm' not in params or
+                                                       params['slug_perm'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `slug_perm` when calling `repos_upstream_npm_delete`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'owner' in params:
+            path_params['owner'] = params['owner']  # noqa: E501
+        if 'identifier' in params:
+            path_params['identifier'] = params['identifier']  # noqa: E501
+        if 'slug_perm' in params:
+            path_params['slug_perm'] = params['slug_perm']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/repos/{owner}/{identifier}/upstream/npm/{slug_perm}/', 'DELETE',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type=None,  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def repos_upstream_npm_list(self, owner, identifier, **kwargs):  # noqa: E501
+        """List npm upstream configs for this repository.  # noqa: E501
+
+        List npm upstream configs for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_npm_list(owner, identifier, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param int page: A page number within the paginated result set.
+        :param int page_size: Number of results to return per page.
+        :return: list[NpmUpstream]
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.repos_upstream_npm_list_with_http_info(owner, identifier, **kwargs)  # noqa: E501
+        else:
+            (data) = self.repos_upstream_npm_list_with_http_info(owner, identifier, **kwargs)  # noqa: E501
+            return data
+
+    def repos_upstream_npm_list_with_http_info(self, owner, identifier, **kwargs):  # noqa: E501
+        """List npm upstream configs for this repository.  # noqa: E501
+
+        List npm upstream configs for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_npm_list_with_http_info(owner, identifier, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param int page: A page number within the paginated result set.
+        :param int page_size: Number of results to return per page.
+        :return: list[NpmUpstream]
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['owner', 'identifier', 'page', 'page_size']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method repos_upstream_npm_list" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'owner' is set
+        if self.api_client.client_side_validation and ('owner' not in params or
+                                                       params['owner'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `owner` when calling `repos_upstream_npm_list`")  # noqa: E501
+        # verify the required parameter 'identifier' is set
+        if self.api_client.client_side_validation and ('identifier' not in params or
+                                                       params['identifier'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `identifier` when calling `repos_upstream_npm_list`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'owner' in params:
+            path_params['owner'] = params['owner']  # noqa: E501
+        if 'identifier' in params:
+            path_params['identifier'] = params['identifier']  # noqa: E501
+
+        query_params = []
+        if 'page' in params:
+            query_params.append(('page', params['page']))  # noqa: E501
+        if 'page_size' in params:
+            query_params.append(('page_size', params['page_size']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/repos/{owner}/{identifier}/upstream/npm/', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='list[NpmUpstream]',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def repos_upstream_npm_partial_update(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Partially update a npm upstream config for this repository.  # noqa: E501
+
+        Partially update a npm upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_npm_partial_update(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :param NpmUpstreamRequestPatch data:
+        :return: NpmUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.repos_upstream_npm_partial_update_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+        else:
+            (data) = self.repos_upstream_npm_partial_update_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+            return data
+
+    def repos_upstream_npm_partial_update_with_http_info(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Partially update a npm upstream config for this repository.  # noqa: E501
+
+        Partially update a npm upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_npm_partial_update_with_http_info(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :param NpmUpstreamRequestPatch data:
+        :return: NpmUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['owner', 'identifier', 'slug_perm', 'data']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method repos_upstream_npm_partial_update" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'owner' is set
+        if self.api_client.client_side_validation and ('owner' not in params or
+                                                       params['owner'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `owner` when calling `repos_upstream_npm_partial_update`")  # noqa: E501
+        # verify the required parameter 'identifier' is set
+        if self.api_client.client_side_validation and ('identifier' not in params or
+                                                       params['identifier'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `identifier` when calling `repos_upstream_npm_partial_update`")  # noqa: E501
+        # verify the required parameter 'slug_perm' is set
+        if self.api_client.client_side_validation and ('slug_perm' not in params or
+                                                       params['slug_perm'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `slug_perm` when calling `repos_upstream_npm_partial_update`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'owner' in params:
+            path_params['owner'] = params['owner']  # noqa: E501
+        if 'identifier' in params:
+            path_params['identifier'] = params['identifier']  # noqa: E501
+        if 'slug_perm' in params:
+            path_params['slug_perm'] = params['slug_perm']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'data' in params:
+            body_params = params['data']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/repos/{owner}/{identifier}/upstream/npm/{slug_perm}/', 'PATCH',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='NpmUpstream',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def repos_upstream_npm_read(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Retrieve a npm upstream config for this repository.  # noqa: E501
+
+        Retrieve a npm upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_npm_read(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :return: NpmUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.repos_upstream_npm_read_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+        else:
+            (data) = self.repos_upstream_npm_read_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+            return data
+
+    def repos_upstream_npm_read_with_http_info(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Retrieve a npm upstream config for this repository.  # noqa: E501
+
+        Retrieve a npm upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_npm_read_with_http_info(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :return: NpmUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['owner', 'identifier', 'slug_perm']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method repos_upstream_npm_read" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'owner' is set
+        if self.api_client.client_side_validation and ('owner' not in params or
+                                                       params['owner'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `owner` when calling `repos_upstream_npm_read`")  # noqa: E501
+        # verify the required parameter 'identifier' is set
+        if self.api_client.client_side_validation and ('identifier' not in params or
+                                                       params['identifier'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `identifier` when calling `repos_upstream_npm_read`")  # noqa: E501
+        # verify the required parameter 'slug_perm' is set
+        if self.api_client.client_side_validation and ('slug_perm' not in params or
+                                                       params['slug_perm'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `slug_perm` when calling `repos_upstream_npm_read`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'owner' in params:
+            path_params['owner'] = params['owner']  # noqa: E501
+        if 'identifier' in params:
+            path_params['identifier'] = params['identifier']  # noqa: E501
+        if 'slug_perm' in params:
+            path_params['slug_perm'] = params['slug_perm']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/repos/{owner}/{identifier}/upstream/npm/{slug_perm}/', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='NpmUpstream',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def repos_upstream_npm_update(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Update a npm upstream config for this repository.  # noqa: E501
+
+        Update a npm upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_npm_update(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :param NpmUpstreamRequest data:
+        :return: NpmUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.repos_upstream_npm_update_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+        else:
+            (data) = self.repos_upstream_npm_update_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+            return data
+
+    def repos_upstream_npm_update_with_http_info(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Update a npm upstream config for this repository.  # noqa: E501
+
+        Update a npm upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_npm_update_with_http_info(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :param NpmUpstreamRequest data:
+        :return: NpmUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['owner', 'identifier', 'slug_perm', 'data']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method repos_upstream_npm_update" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'owner' is set
+        if self.api_client.client_side_validation and ('owner' not in params or
+                                                       params['owner'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `owner` when calling `repos_upstream_npm_update`")  # noqa: E501
+        # verify the required parameter 'identifier' is set
+        if self.api_client.client_side_validation and ('identifier' not in params or
+                                                       params['identifier'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `identifier` when calling `repos_upstream_npm_update`")  # noqa: E501
+        # verify the required parameter 'slug_perm' is set
+        if self.api_client.client_side_validation and ('slug_perm' not in params or
+                                                       params['slug_perm'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `slug_perm` when calling `repos_upstream_npm_update`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'owner' in params:
+            path_params['owner'] = params['owner']  # noqa: E501
+        if 'identifier' in params:
+            path_params['identifier'] = params['identifier']  # noqa: E501
+        if 'slug_perm' in params:
+            path_params['slug_perm'] = params['slug_perm']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'data' in params:
+            body_params = params['data']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/repos/{owner}/{identifier}/upstream/npm/{slug_perm}/', 'PUT',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='NpmUpstream',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def repos_upstream_nuget_create(self, owner, identifier, **kwargs):  # noqa: E501
+        """Create a NuGet upstream config for this repository.  # noqa: E501
+
+        Create a NuGet upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_nuget_create(owner, identifier, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param NugetUpstreamRequest data:
+        :return: NugetUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.repos_upstream_nuget_create_with_http_info(owner, identifier, **kwargs)  # noqa: E501
+        else:
+            (data) = self.repos_upstream_nuget_create_with_http_info(owner, identifier, **kwargs)  # noqa: E501
+            return data
+
+    def repos_upstream_nuget_create_with_http_info(self, owner, identifier, **kwargs):  # noqa: E501
+        """Create a NuGet upstream config for this repository.  # noqa: E501
+
+        Create a NuGet upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_nuget_create_with_http_info(owner, identifier, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param NugetUpstreamRequest data:
+        :return: NugetUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['owner', 'identifier', 'data']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method repos_upstream_nuget_create" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'owner' is set
+        if self.api_client.client_side_validation and ('owner' not in params or
+                                                       params['owner'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `owner` when calling `repos_upstream_nuget_create`")  # noqa: E501
+        # verify the required parameter 'identifier' is set
+        if self.api_client.client_side_validation and ('identifier' not in params or
+                                                       params['identifier'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `identifier` when calling `repos_upstream_nuget_create`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'owner' in params:
+            path_params['owner'] = params['owner']  # noqa: E501
+        if 'identifier' in params:
+            path_params['identifier'] = params['identifier']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'data' in params:
+            body_params = params['data']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/repos/{owner}/{identifier}/upstream/nuget/', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='NugetUpstream',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def repos_upstream_nuget_delete(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Delete a NuGet upstream config for this repository.  # noqa: E501
+
+        Delete a NuGet upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_nuget_delete(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :return: None
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.repos_upstream_nuget_delete_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+        else:
+            (data) = self.repos_upstream_nuget_delete_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+            return data
+
+    def repos_upstream_nuget_delete_with_http_info(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Delete a NuGet upstream config for this repository.  # noqa: E501
+
+        Delete a NuGet upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_nuget_delete_with_http_info(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :return: None
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['owner', 'identifier', 'slug_perm']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method repos_upstream_nuget_delete" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'owner' is set
+        if self.api_client.client_side_validation and ('owner' not in params or
+                                                       params['owner'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `owner` when calling `repos_upstream_nuget_delete`")  # noqa: E501
+        # verify the required parameter 'identifier' is set
+        if self.api_client.client_side_validation and ('identifier' not in params or
+                                                       params['identifier'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `identifier` when calling `repos_upstream_nuget_delete`")  # noqa: E501
+        # verify the required parameter 'slug_perm' is set
+        if self.api_client.client_side_validation and ('slug_perm' not in params or
+                                                       params['slug_perm'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `slug_perm` when calling `repos_upstream_nuget_delete`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'owner' in params:
+            path_params['owner'] = params['owner']  # noqa: E501
+        if 'identifier' in params:
+            path_params['identifier'] = params['identifier']  # noqa: E501
+        if 'slug_perm' in params:
+            path_params['slug_perm'] = params['slug_perm']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/repos/{owner}/{identifier}/upstream/nuget/{slug_perm}/', 'DELETE',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type=None,  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def repos_upstream_nuget_list(self, owner, identifier, **kwargs):  # noqa: E501
+        """List NuGet upstream configs for this repository.  # noqa: E501
+
+        List NuGet upstream configs for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_nuget_list(owner, identifier, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param int page: A page number within the paginated result set.
+        :param int page_size: Number of results to return per page.
+        :return: list[NugetUpstream]
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.repos_upstream_nuget_list_with_http_info(owner, identifier, **kwargs)  # noqa: E501
+        else:
+            (data) = self.repos_upstream_nuget_list_with_http_info(owner, identifier, **kwargs)  # noqa: E501
+            return data
+
+    def repos_upstream_nuget_list_with_http_info(self, owner, identifier, **kwargs):  # noqa: E501
+        """List NuGet upstream configs for this repository.  # noqa: E501
+
+        List NuGet upstream configs for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_nuget_list_with_http_info(owner, identifier, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param int page: A page number within the paginated result set.
+        :param int page_size: Number of results to return per page.
+        :return: list[NugetUpstream]
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['owner', 'identifier', 'page', 'page_size']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method repos_upstream_nuget_list" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'owner' is set
+        if self.api_client.client_side_validation and ('owner' not in params or
+                                                       params['owner'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `owner` when calling `repos_upstream_nuget_list`")  # noqa: E501
+        # verify the required parameter 'identifier' is set
+        if self.api_client.client_side_validation and ('identifier' not in params or
+                                                       params['identifier'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `identifier` when calling `repos_upstream_nuget_list`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'owner' in params:
+            path_params['owner'] = params['owner']  # noqa: E501
+        if 'identifier' in params:
+            path_params['identifier'] = params['identifier']  # noqa: E501
+
+        query_params = []
+        if 'page' in params:
+            query_params.append(('page', params['page']))  # noqa: E501
+        if 'page_size' in params:
+            query_params.append(('page_size', params['page_size']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/repos/{owner}/{identifier}/upstream/nuget/', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='list[NugetUpstream]',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def repos_upstream_nuget_partial_update(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Partially update a NuGet upstream config for this repository.  # noqa: E501
+
+        Partially update a NuGet upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_nuget_partial_update(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :param NugetUpstreamRequestPatch data:
+        :return: NugetUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.repos_upstream_nuget_partial_update_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+        else:
+            (data) = self.repos_upstream_nuget_partial_update_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+            return data
+
+    def repos_upstream_nuget_partial_update_with_http_info(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Partially update a NuGet upstream config for this repository.  # noqa: E501
+
+        Partially update a NuGet upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_nuget_partial_update_with_http_info(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :param NugetUpstreamRequestPatch data:
+        :return: NugetUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['owner', 'identifier', 'slug_perm', 'data']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method repos_upstream_nuget_partial_update" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'owner' is set
+        if self.api_client.client_side_validation and ('owner' not in params or
+                                                       params['owner'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `owner` when calling `repos_upstream_nuget_partial_update`")  # noqa: E501
+        # verify the required parameter 'identifier' is set
+        if self.api_client.client_side_validation and ('identifier' not in params or
+                                                       params['identifier'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `identifier` when calling `repos_upstream_nuget_partial_update`")  # noqa: E501
+        # verify the required parameter 'slug_perm' is set
+        if self.api_client.client_side_validation and ('slug_perm' not in params or
+                                                       params['slug_perm'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `slug_perm` when calling `repos_upstream_nuget_partial_update`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'owner' in params:
+            path_params['owner'] = params['owner']  # noqa: E501
+        if 'identifier' in params:
+            path_params['identifier'] = params['identifier']  # noqa: E501
+        if 'slug_perm' in params:
+            path_params['slug_perm'] = params['slug_perm']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'data' in params:
+            body_params = params['data']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/repos/{owner}/{identifier}/upstream/nuget/{slug_perm}/', 'PATCH',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='NugetUpstream',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def repos_upstream_nuget_read(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Retrieve a NuGet upstream config for this repository.  # noqa: E501
+
+        Retrieve a NuGet upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_nuget_read(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :return: NugetUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.repos_upstream_nuget_read_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+        else:
+            (data) = self.repos_upstream_nuget_read_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+            return data
+
+    def repos_upstream_nuget_read_with_http_info(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Retrieve a NuGet upstream config for this repository.  # noqa: E501
+
+        Retrieve a NuGet upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_nuget_read_with_http_info(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :return: NugetUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['owner', 'identifier', 'slug_perm']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method repos_upstream_nuget_read" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'owner' is set
+        if self.api_client.client_side_validation and ('owner' not in params or
+                                                       params['owner'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `owner` when calling `repos_upstream_nuget_read`")  # noqa: E501
+        # verify the required parameter 'identifier' is set
+        if self.api_client.client_side_validation and ('identifier' not in params or
+                                                       params['identifier'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `identifier` when calling `repos_upstream_nuget_read`")  # noqa: E501
+        # verify the required parameter 'slug_perm' is set
+        if self.api_client.client_side_validation and ('slug_perm' not in params or
+                                                       params['slug_perm'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `slug_perm` when calling `repos_upstream_nuget_read`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'owner' in params:
+            path_params['owner'] = params['owner']  # noqa: E501
+        if 'identifier' in params:
+            path_params['identifier'] = params['identifier']  # noqa: E501
+        if 'slug_perm' in params:
+            path_params['slug_perm'] = params['slug_perm']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/repos/{owner}/{identifier}/upstream/nuget/{slug_perm}/', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='NugetUpstream',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def repos_upstream_nuget_update(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Update a NuGet upstream config for this repository.  # noqa: E501
+
+        Update a NuGet upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_nuget_update(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :param NugetUpstreamRequest data:
+        :return: NugetUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.repos_upstream_nuget_update_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+        else:
+            (data) = self.repos_upstream_nuget_update_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+            return data
+
+    def repos_upstream_nuget_update_with_http_info(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Update a NuGet upstream config for this repository.  # noqa: E501
+
+        Update a NuGet upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_nuget_update_with_http_info(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :param NugetUpstreamRequest data:
+        :return: NugetUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['owner', 'identifier', 'slug_perm', 'data']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method repos_upstream_nuget_update" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'owner' is set
+        if self.api_client.client_side_validation and ('owner' not in params or
+                                                       params['owner'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `owner` when calling `repos_upstream_nuget_update`")  # noqa: E501
+        # verify the required parameter 'identifier' is set
+        if self.api_client.client_side_validation and ('identifier' not in params or
+                                                       params['identifier'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `identifier` when calling `repos_upstream_nuget_update`")  # noqa: E501
+        # verify the required parameter 'slug_perm' is set
+        if self.api_client.client_side_validation and ('slug_perm' not in params or
+                                                       params['slug_perm'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `slug_perm` when calling `repos_upstream_nuget_update`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'owner' in params:
+            path_params['owner'] = params['owner']  # noqa: E501
+        if 'identifier' in params:
+            path_params['identifier'] = params['identifier']  # noqa: E501
+        if 'slug_perm' in params:
+            path_params['slug_perm'] = params['slug_perm']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'data' in params:
+            body_params = params['data']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/repos/{owner}/{identifier}/upstream/nuget/{slug_perm}/', 'PUT',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='NugetUpstream',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def repos_upstream_python_create(self, owner, identifier, **kwargs):  # noqa: E501
+        """Create a Python upstream config for this repository.  # noqa: E501
+
+        Create a Python upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_python_create(owner, identifier, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param PythonUpstreamRequest data:
+        :return: PythonUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.repos_upstream_python_create_with_http_info(owner, identifier, **kwargs)  # noqa: E501
+        else:
+            (data) = self.repos_upstream_python_create_with_http_info(owner, identifier, **kwargs)  # noqa: E501
+            return data
+
+    def repos_upstream_python_create_with_http_info(self, owner, identifier, **kwargs):  # noqa: E501
+        """Create a Python upstream config for this repository.  # noqa: E501
+
+        Create a Python upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_python_create_with_http_info(owner, identifier, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param PythonUpstreamRequest data:
+        :return: PythonUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['owner', 'identifier', 'data']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method repos_upstream_python_create" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'owner' is set
+        if self.api_client.client_side_validation and ('owner' not in params or
+                                                       params['owner'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `owner` when calling `repos_upstream_python_create`")  # noqa: E501
+        # verify the required parameter 'identifier' is set
+        if self.api_client.client_side_validation and ('identifier' not in params or
+                                                       params['identifier'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `identifier` when calling `repos_upstream_python_create`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'owner' in params:
+            path_params['owner'] = params['owner']  # noqa: E501
+        if 'identifier' in params:
+            path_params['identifier'] = params['identifier']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'data' in params:
+            body_params = params['data']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/repos/{owner}/{identifier}/upstream/python/', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='PythonUpstream',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def repos_upstream_python_delete(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Delete a Python upstream config for this repository.  # noqa: E501
+
+        Delete a Python upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_python_delete(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :return: None
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.repos_upstream_python_delete_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+        else:
+            (data) = self.repos_upstream_python_delete_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+            return data
+
+    def repos_upstream_python_delete_with_http_info(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Delete a Python upstream config for this repository.  # noqa: E501
+
+        Delete a Python upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_python_delete_with_http_info(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :return: None
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['owner', 'identifier', 'slug_perm']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method repos_upstream_python_delete" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'owner' is set
+        if self.api_client.client_side_validation and ('owner' not in params or
+                                                       params['owner'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `owner` when calling `repos_upstream_python_delete`")  # noqa: E501
+        # verify the required parameter 'identifier' is set
+        if self.api_client.client_side_validation and ('identifier' not in params or
+                                                       params['identifier'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `identifier` when calling `repos_upstream_python_delete`")  # noqa: E501
+        # verify the required parameter 'slug_perm' is set
+        if self.api_client.client_side_validation and ('slug_perm' not in params or
+                                                       params['slug_perm'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `slug_perm` when calling `repos_upstream_python_delete`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'owner' in params:
+            path_params['owner'] = params['owner']  # noqa: E501
+        if 'identifier' in params:
+            path_params['identifier'] = params['identifier']  # noqa: E501
+        if 'slug_perm' in params:
+            path_params['slug_perm'] = params['slug_perm']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/repos/{owner}/{identifier}/upstream/python/{slug_perm}/', 'DELETE',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type=None,  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def repos_upstream_python_list(self, owner, identifier, **kwargs):  # noqa: E501
+        """List Python upstream configs for this repository.  # noqa: E501
+
+        List Python upstream configs for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_python_list(owner, identifier, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param int page: A page number within the paginated result set.
+        :param int page_size: Number of results to return per page.
+        :return: list[PythonUpstream]
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.repos_upstream_python_list_with_http_info(owner, identifier, **kwargs)  # noqa: E501
+        else:
+            (data) = self.repos_upstream_python_list_with_http_info(owner, identifier, **kwargs)  # noqa: E501
+            return data
+
+    def repos_upstream_python_list_with_http_info(self, owner, identifier, **kwargs):  # noqa: E501
+        """List Python upstream configs for this repository.  # noqa: E501
+
+        List Python upstream configs for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_python_list_with_http_info(owner, identifier, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param int page: A page number within the paginated result set.
+        :param int page_size: Number of results to return per page.
+        :return: list[PythonUpstream]
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['owner', 'identifier', 'page', 'page_size']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method repos_upstream_python_list" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'owner' is set
+        if self.api_client.client_side_validation and ('owner' not in params or
+                                                       params['owner'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `owner` when calling `repos_upstream_python_list`")  # noqa: E501
+        # verify the required parameter 'identifier' is set
+        if self.api_client.client_side_validation and ('identifier' not in params or
+                                                       params['identifier'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `identifier` when calling `repos_upstream_python_list`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'owner' in params:
+            path_params['owner'] = params['owner']  # noqa: E501
+        if 'identifier' in params:
+            path_params['identifier'] = params['identifier']  # noqa: E501
+
+        query_params = []
+        if 'page' in params:
+            query_params.append(('page', params['page']))  # noqa: E501
+        if 'page_size' in params:
+            query_params.append(('page_size', params['page_size']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/repos/{owner}/{identifier}/upstream/python/', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='list[PythonUpstream]',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def repos_upstream_python_partial_update(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Partially update a Python upstream config for this repository.  # noqa: E501
+
+        Partially update a Python upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_python_partial_update(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :param PythonUpstreamRequestPatch data:
+        :return: PythonUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.repos_upstream_python_partial_update_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+        else:
+            (data) = self.repos_upstream_python_partial_update_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+            return data
+
+    def repos_upstream_python_partial_update_with_http_info(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Partially update a Python upstream config for this repository.  # noqa: E501
+
+        Partially update a Python upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_python_partial_update_with_http_info(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :param PythonUpstreamRequestPatch data:
+        :return: PythonUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['owner', 'identifier', 'slug_perm', 'data']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method repos_upstream_python_partial_update" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'owner' is set
+        if self.api_client.client_side_validation and ('owner' not in params or
+                                                       params['owner'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `owner` when calling `repos_upstream_python_partial_update`")  # noqa: E501
+        # verify the required parameter 'identifier' is set
+        if self.api_client.client_side_validation and ('identifier' not in params or
+                                                       params['identifier'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `identifier` when calling `repos_upstream_python_partial_update`")  # noqa: E501
+        # verify the required parameter 'slug_perm' is set
+        if self.api_client.client_side_validation and ('slug_perm' not in params or
+                                                       params['slug_perm'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `slug_perm` when calling `repos_upstream_python_partial_update`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'owner' in params:
+            path_params['owner'] = params['owner']  # noqa: E501
+        if 'identifier' in params:
+            path_params['identifier'] = params['identifier']  # noqa: E501
+        if 'slug_perm' in params:
+            path_params['slug_perm'] = params['slug_perm']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'data' in params:
+            body_params = params['data']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/repos/{owner}/{identifier}/upstream/python/{slug_perm}/', 'PATCH',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='PythonUpstream',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def repos_upstream_python_read(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Retrieve a Python upstream config for this repository.  # noqa: E501
+
+        Retrieve a Python upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_python_read(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :return: PythonUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.repos_upstream_python_read_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+        else:
+            (data) = self.repos_upstream_python_read_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+            return data
+
+    def repos_upstream_python_read_with_http_info(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Retrieve a Python upstream config for this repository.  # noqa: E501
+
+        Retrieve a Python upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_python_read_with_http_info(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :return: PythonUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['owner', 'identifier', 'slug_perm']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method repos_upstream_python_read" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'owner' is set
+        if self.api_client.client_side_validation and ('owner' not in params or
+                                                       params['owner'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `owner` when calling `repos_upstream_python_read`")  # noqa: E501
+        # verify the required parameter 'identifier' is set
+        if self.api_client.client_side_validation and ('identifier' not in params or
+                                                       params['identifier'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `identifier` when calling `repos_upstream_python_read`")  # noqa: E501
+        # verify the required parameter 'slug_perm' is set
+        if self.api_client.client_side_validation and ('slug_perm' not in params or
+                                                       params['slug_perm'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `slug_perm` when calling `repos_upstream_python_read`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'owner' in params:
+            path_params['owner'] = params['owner']  # noqa: E501
+        if 'identifier' in params:
+            path_params['identifier'] = params['identifier']  # noqa: E501
+        if 'slug_perm' in params:
+            path_params['slug_perm'] = params['slug_perm']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/repos/{owner}/{identifier}/upstream/python/{slug_perm}/', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='PythonUpstream',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def repos_upstream_python_update(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Update a Python upstream config for this repository.  # noqa: E501
+
+        Update a Python upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_python_update(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :param PythonUpstreamRequest data:
+        :return: PythonUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.repos_upstream_python_update_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+        else:
+            (data) = self.repos_upstream_python_update_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+            return data
+
+    def repos_upstream_python_update_with_http_info(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Update a Python upstream config for this repository.  # noqa: E501
+
+        Update a Python upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_python_update_with_http_info(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :param PythonUpstreamRequest data:
+        :return: PythonUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['owner', 'identifier', 'slug_perm', 'data']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method repos_upstream_python_update" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'owner' is set
+        if self.api_client.client_side_validation and ('owner' not in params or
+                                                       params['owner'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `owner` when calling `repos_upstream_python_update`")  # noqa: E501
+        # verify the required parameter 'identifier' is set
+        if self.api_client.client_side_validation and ('identifier' not in params or
+                                                       params['identifier'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `identifier` when calling `repos_upstream_python_update`")  # noqa: E501
+        # verify the required parameter 'slug_perm' is set
+        if self.api_client.client_side_validation and ('slug_perm' not in params or
+                                                       params['slug_perm'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `slug_perm` when calling `repos_upstream_python_update`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'owner' in params:
+            path_params['owner'] = params['owner']  # noqa: E501
+        if 'identifier' in params:
+            path_params['identifier'] = params['identifier']  # noqa: E501
+        if 'slug_perm' in params:
+            path_params['slug_perm'] = params['slug_perm']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'data' in params:
+            body_params = params['data']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/repos/{owner}/{identifier}/upstream/python/{slug_perm}/', 'PUT',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='PythonUpstream',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def repos_upstream_rpm_create(self, owner, identifier, **kwargs):  # noqa: E501
+        """Create a RedHat upstream config for this repository.  # noqa: E501
+
+        Create a RedHat upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_rpm_create(owner, identifier, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param RpmUpstreamRequest data:
+        :return: RpmUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.repos_upstream_rpm_create_with_http_info(owner, identifier, **kwargs)  # noqa: E501
+        else:
+            (data) = self.repos_upstream_rpm_create_with_http_info(owner, identifier, **kwargs)  # noqa: E501
+            return data
+
+    def repos_upstream_rpm_create_with_http_info(self, owner, identifier, **kwargs):  # noqa: E501
+        """Create a RedHat upstream config for this repository.  # noqa: E501
+
+        Create a RedHat upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_rpm_create_with_http_info(owner, identifier, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param RpmUpstreamRequest data:
+        :return: RpmUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['owner', 'identifier', 'data']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method repos_upstream_rpm_create" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'owner' is set
+        if self.api_client.client_side_validation and ('owner' not in params or
+                                                       params['owner'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `owner` when calling `repos_upstream_rpm_create`")  # noqa: E501
+        # verify the required parameter 'identifier' is set
+        if self.api_client.client_side_validation and ('identifier' not in params or
+                                                       params['identifier'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `identifier` when calling `repos_upstream_rpm_create`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'owner' in params:
+            path_params['owner'] = params['owner']  # noqa: E501
+        if 'identifier' in params:
+            path_params['identifier'] = params['identifier']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'data' in params:
+            body_params = params['data']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/repos/{owner}/{identifier}/upstream/rpm/', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='RpmUpstream',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def repos_upstream_rpm_delete(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Delete a RedHat upstream config for this repository.  # noqa: E501
+
+        Delete a RedHat upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_rpm_delete(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :return: None
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.repos_upstream_rpm_delete_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+        else:
+            (data) = self.repos_upstream_rpm_delete_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+            return data
+
+    def repos_upstream_rpm_delete_with_http_info(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Delete a RedHat upstream config for this repository.  # noqa: E501
+
+        Delete a RedHat upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_rpm_delete_with_http_info(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :return: None
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['owner', 'identifier', 'slug_perm']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method repos_upstream_rpm_delete" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'owner' is set
+        if self.api_client.client_side_validation and ('owner' not in params or
+                                                       params['owner'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `owner` when calling `repos_upstream_rpm_delete`")  # noqa: E501
+        # verify the required parameter 'identifier' is set
+        if self.api_client.client_side_validation and ('identifier' not in params or
+                                                       params['identifier'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `identifier` when calling `repos_upstream_rpm_delete`")  # noqa: E501
+        # verify the required parameter 'slug_perm' is set
+        if self.api_client.client_side_validation and ('slug_perm' not in params or
+                                                       params['slug_perm'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `slug_perm` when calling `repos_upstream_rpm_delete`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'owner' in params:
+            path_params['owner'] = params['owner']  # noqa: E501
+        if 'identifier' in params:
+            path_params['identifier'] = params['identifier']  # noqa: E501
+        if 'slug_perm' in params:
+            path_params['slug_perm'] = params['slug_perm']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/repos/{owner}/{identifier}/upstream/rpm/{slug_perm}/', 'DELETE',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type=None,  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def repos_upstream_rpm_list(self, owner, identifier, **kwargs):  # noqa: E501
+        """List RedHat upstream configs for this repository.  # noqa: E501
+
+        List RedHat upstream configs for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_rpm_list(owner, identifier, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param int page: A page number within the paginated result set.
+        :param int page_size: Number of results to return per page.
+        :return: list[RpmUpstream]
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.repos_upstream_rpm_list_with_http_info(owner, identifier, **kwargs)  # noqa: E501
+        else:
+            (data) = self.repos_upstream_rpm_list_with_http_info(owner, identifier, **kwargs)  # noqa: E501
+            return data
+
+    def repos_upstream_rpm_list_with_http_info(self, owner, identifier, **kwargs):  # noqa: E501
+        """List RedHat upstream configs for this repository.  # noqa: E501
+
+        List RedHat upstream configs for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_rpm_list_with_http_info(owner, identifier, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param int page: A page number within the paginated result set.
+        :param int page_size: Number of results to return per page.
+        :return: list[RpmUpstream]
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['owner', 'identifier', 'page', 'page_size']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method repos_upstream_rpm_list" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'owner' is set
+        if self.api_client.client_side_validation and ('owner' not in params or
+                                                       params['owner'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `owner` when calling `repos_upstream_rpm_list`")  # noqa: E501
+        # verify the required parameter 'identifier' is set
+        if self.api_client.client_side_validation and ('identifier' not in params or
+                                                       params['identifier'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `identifier` when calling `repos_upstream_rpm_list`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'owner' in params:
+            path_params['owner'] = params['owner']  # noqa: E501
+        if 'identifier' in params:
+            path_params['identifier'] = params['identifier']  # noqa: E501
+
+        query_params = []
+        if 'page' in params:
+            query_params.append(('page', params['page']))  # noqa: E501
+        if 'page_size' in params:
+            query_params.append(('page_size', params['page_size']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/repos/{owner}/{identifier}/upstream/rpm/', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='list[RpmUpstream]',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def repos_upstream_rpm_partial_update(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Partially update a RedHat upstream config for this repository.  # noqa: E501
+
+        Partially update a RedHat upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_rpm_partial_update(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :param RpmUpstreamRequestPatch data:
+        :return: RpmUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.repos_upstream_rpm_partial_update_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+        else:
+            (data) = self.repos_upstream_rpm_partial_update_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+            return data
+
+    def repos_upstream_rpm_partial_update_with_http_info(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Partially update a RedHat upstream config for this repository.  # noqa: E501
+
+        Partially update a RedHat upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_rpm_partial_update_with_http_info(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :param RpmUpstreamRequestPatch data:
+        :return: RpmUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['owner', 'identifier', 'slug_perm', 'data']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method repos_upstream_rpm_partial_update" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'owner' is set
+        if self.api_client.client_side_validation and ('owner' not in params or
+                                                       params['owner'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `owner` when calling `repos_upstream_rpm_partial_update`")  # noqa: E501
+        # verify the required parameter 'identifier' is set
+        if self.api_client.client_side_validation and ('identifier' not in params or
+                                                       params['identifier'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `identifier` when calling `repos_upstream_rpm_partial_update`")  # noqa: E501
+        # verify the required parameter 'slug_perm' is set
+        if self.api_client.client_side_validation and ('slug_perm' not in params or
+                                                       params['slug_perm'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `slug_perm` when calling `repos_upstream_rpm_partial_update`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'owner' in params:
+            path_params['owner'] = params['owner']  # noqa: E501
+        if 'identifier' in params:
+            path_params['identifier'] = params['identifier']  # noqa: E501
+        if 'slug_perm' in params:
+            path_params['slug_perm'] = params['slug_perm']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'data' in params:
+            body_params = params['data']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/repos/{owner}/{identifier}/upstream/rpm/{slug_perm}/', 'PATCH',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='RpmUpstream',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def repos_upstream_rpm_read(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Retrieve a RedHat upstream config for this repository.  # noqa: E501
+
+        Retrieve a RedHat upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_rpm_read(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :return: RpmUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.repos_upstream_rpm_read_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+        else:
+            (data) = self.repos_upstream_rpm_read_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+            return data
+
+    def repos_upstream_rpm_read_with_http_info(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Retrieve a RedHat upstream config for this repository.  # noqa: E501
+
+        Retrieve a RedHat upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_rpm_read_with_http_info(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :return: RpmUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['owner', 'identifier', 'slug_perm']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method repos_upstream_rpm_read" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'owner' is set
+        if self.api_client.client_side_validation and ('owner' not in params or
+                                                       params['owner'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `owner` when calling `repos_upstream_rpm_read`")  # noqa: E501
+        # verify the required parameter 'identifier' is set
+        if self.api_client.client_side_validation and ('identifier' not in params or
+                                                       params['identifier'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `identifier` when calling `repos_upstream_rpm_read`")  # noqa: E501
+        # verify the required parameter 'slug_perm' is set
+        if self.api_client.client_side_validation and ('slug_perm' not in params or
+                                                       params['slug_perm'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `slug_perm` when calling `repos_upstream_rpm_read`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'owner' in params:
+            path_params['owner'] = params['owner']  # noqa: E501
+        if 'identifier' in params:
+            path_params['identifier'] = params['identifier']  # noqa: E501
+        if 'slug_perm' in params:
+            path_params['slug_perm'] = params['slug_perm']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/repos/{owner}/{identifier}/upstream/rpm/{slug_perm}/', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='RpmUpstream',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def repos_upstream_rpm_update(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Update a RedHat upstream config for this repository.  # noqa: E501
+
+        Update a RedHat upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_rpm_update(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :param RpmUpstreamRequest data:
+        :return: RpmUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.repos_upstream_rpm_update_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+        else:
+            (data) = self.repos_upstream_rpm_update_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+            return data
+
+    def repos_upstream_rpm_update_with_http_info(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Update a RedHat upstream config for this repository.  # noqa: E501
+
+        Update a RedHat upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_rpm_update_with_http_info(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :param RpmUpstreamRequest data:
+        :return: RpmUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['owner', 'identifier', 'slug_perm', 'data']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method repos_upstream_rpm_update" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'owner' is set
+        if self.api_client.client_side_validation and ('owner' not in params or
+                                                       params['owner'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `owner` when calling `repos_upstream_rpm_update`")  # noqa: E501
+        # verify the required parameter 'identifier' is set
+        if self.api_client.client_side_validation and ('identifier' not in params or
+                                                       params['identifier'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `identifier` when calling `repos_upstream_rpm_update`")  # noqa: E501
+        # verify the required parameter 'slug_perm' is set
+        if self.api_client.client_side_validation and ('slug_perm' not in params or
+                                                       params['slug_perm'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `slug_perm` when calling `repos_upstream_rpm_update`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'owner' in params:
+            path_params['owner'] = params['owner']  # noqa: E501
+        if 'identifier' in params:
+            path_params['identifier'] = params['identifier']  # noqa: E501
+        if 'slug_perm' in params:
+            path_params['slug_perm'] = params['slug_perm']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'data' in params:
+            body_params = params['data']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/repos/{owner}/{identifier}/upstream/rpm/{slug_perm}/', 'PUT',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='RpmUpstream',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def repos_upstream_ruby_create(self, owner, identifier, **kwargs):  # noqa: E501
+        """Create a Ruby upstream config for this repository.  # noqa: E501
+
+        Create a Ruby upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_ruby_create(owner, identifier, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param RubyUpstreamRequest data:
+        :return: RubyUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.repos_upstream_ruby_create_with_http_info(owner, identifier, **kwargs)  # noqa: E501
+        else:
+            (data) = self.repos_upstream_ruby_create_with_http_info(owner, identifier, **kwargs)  # noqa: E501
+            return data
+
+    def repos_upstream_ruby_create_with_http_info(self, owner, identifier, **kwargs):  # noqa: E501
+        """Create a Ruby upstream config for this repository.  # noqa: E501
+
+        Create a Ruby upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_ruby_create_with_http_info(owner, identifier, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param RubyUpstreamRequest data:
+        :return: RubyUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['owner', 'identifier', 'data']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method repos_upstream_ruby_create" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'owner' is set
+        if self.api_client.client_side_validation and ('owner' not in params or
+                                                       params['owner'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `owner` when calling `repos_upstream_ruby_create`")  # noqa: E501
+        # verify the required parameter 'identifier' is set
+        if self.api_client.client_side_validation and ('identifier' not in params or
+                                                       params['identifier'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `identifier` when calling `repos_upstream_ruby_create`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'owner' in params:
+            path_params['owner'] = params['owner']  # noqa: E501
+        if 'identifier' in params:
+            path_params['identifier'] = params['identifier']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'data' in params:
+            body_params = params['data']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/repos/{owner}/{identifier}/upstream/ruby/', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='RubyUpstream',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def repos_upstream_ruby_delete(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Delete a Ruby upstream config for this repository.  # noqa: E501
+
+        Delete a Ruby upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_ruby_delete(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :return: None
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.repos_upstream_ruby_delete_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+        else:
+            (data) = self.repos_upstream_ruby_delete_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+            return data
+
+    def repos_upstream_ruby_delete_with_http_info(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Delete a Ruby upstream config for this repository.  # noqa: E501
+
+        Delete a Ruby upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_ruby_delete_with_http_info(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :return: None
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['owner', 'identifier', 'slug_perm']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method repos_upstream_ruby_delete" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'owner' is set
+        if self.api_client.client_side_validation and ('owner' not in params or
+                                                       params['owner'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `owner` when calling `repos_upstream_ruby_delete`")  # noqa: E501
+        # verify the required parameter 'identifier' is set
+        if self.api_client.client_side_validation and ('identifier' not in params or
+                                                       params['identifier'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `identifier` when calling `repos_upstream_ruby_delete`")  # noqa: E501
+        # verify the required parameter 'slug_perm' is set
+        if self.api_client.client_side_validation and ('slug_perm' not in params or
+                                                       params['slug_perm'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `slug_perm` when calling `repos_upstream_ruby_delete`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'owner' in params:
+            path_params['owner'] = params['owner']  # noqa: E501
+        if 'identifier' in params:
+            path_params['identifier'] = params['identifier']  # noqa: E501
+        if 'slug_perm' in params:
+            path_params['slug_perm'] = params['slug_perm']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/repos/{owner}/{identifier}/upstream/ruby/{slug_perm}/', 'DELETE',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type=None,  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def repos_upstream_ruby_list(self, owner, identifier, **kwargs):  # noqa: E501
+        """List Ruby upstream configs for this repository.  # noqa: E501
+
+        List Ruby upstream configs for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_ruby_list(owner, identifier, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param int page: A page number within the paginated result set.
+        :param int page_size: Number of results to return per page.
+        :return: list[RubyUpstream]
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.repos_upstream_ruby_list_with_http_info(owner, identifier, **kwargs)  # noqa: E501
+        else:
+            (data) = self.repos_upstream_ruby_list_with_http_info(owner, identifier, **kwargs)  # noqa: E501
+            return data
+
+    def repos_upstream_ruby_list_with_http_info(self, owner, identifier, **kwargs):  # noqa: E501
+        """List Ruby upstream configs for this repository.  # noqa: E501
+
+        List Ruby upstream configs for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_ruby_list_with_http_info(owner, identifier, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param int page: A page number within the paginated result set.
+        :param int page_size: Number of results to return per page.
+        :return: list[RubyUpstream]
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['owner', 'identifier', 'page', 'page_size']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method repos_upstream_ruby_list" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'owner' is set
+        if self.api_client.client_side_validation and ('owner' not in params or
+                                                       params['owner'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `owner` when calling `repos_upstream_ruby_list`")  # noqa: E501
+        # verify the required parameter 'identifier' is set
+        if self.api_client.client_side_validation and ('identifier' not in params or
+                                                       params['identifier'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `identifier` when calling `repos_upstream_ruby_list`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'owner' in params:
+            path_params['owner'] = params['owner']  # noqa: E501
+        if 'identifier' in params:
+            path_params['identifier'] = params['identifier']  # noqa: E501
+
+        query_params = []
+        if 'page' in params:
+            query_params.append(('page', params['page']))  # noqa: E501
+        if 'page_size' in params:
+            query_params.append(('page_size', params['page_size']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/repos/{owner}/{identifier}/upstream/ruby/', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='list[RubyUpstream]',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def repos_upstream_ruby_partial_update(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Partially update a Ruby upstream config for this repository.  # noqa: E501
+
+        Partially update a Ruby upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_ruby_partial_update(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :param RubyUpstreamRequestPatch data:
+        :return: RubyUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.repos_upstream_ruby_partial_update_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+        else:
+            (data) = self.repos_upstream_ruby_partial_update_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+            return data
+
+    def repos_upstream_ruby_partial_update_with_http_info(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Partially update a Ruby upstream config for this repository.  # noqa: E501
+
+        Partially update a Ruby upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_ruby_partial_update_with_http_info(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :param RubyUpstreamRequestPatch data:
+        :return: RubyUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['owner', 'identifier', 'slug_perm', 'data']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method repos_upstream_ruby_partial_update" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'owner' is set
+        if self.api_client.client_side_validation and ('owner' not in params or
+                                                       params['owner'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `owner` when calling `repos_upstream_ruby_partial_update`")  # noqa: E501
+        # verify the required parameter 'identifier' is set
+        if self.api_client.client_side_validation and ('identifier' not in params or
+                                                       params['identifier'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `identifier` when calling `repos_upstream_ruby_partial_update`")  # noqa: E501
+        # verify the required parameter 'slug_perm' is set
+        if self.api_client.client_side_validation and ('slug_perm' not in params or
+                                                       params['slug_perm'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `slug_perm` when calling `repos_upstream_ruby_partial_update`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'owner' in params:
+            path_params['owner'] = params['owner']  # noqa: E501
+        if 'identifier' in params:
+            path_params['identifier'] = params['identifier']  # noqa: E501
+        if 'slug_perm' in params:
+            path_params['slug_perm'] = params['slug_perm']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'data' in params:
+            body_params = params['data']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/repos/{owner}/{identifier}/upstream/ruby/{slug_perm}/', 'PATCH',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='RubyUpstream',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def repos_upstream_ruby_read(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Retrieve a Ruby upstream config for this repository.  # noqa: E501
+
+        Retrieve a Ruby upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_ruby_read(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :return: RubyUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.repos_upstream_ruby_read_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+        else:
+            (data) = self.repos_upstream_ruby_read_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+            return data
+
+    def repos_upstream_ruby_read_with_http_info(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Retrieve a Ruby upstream config for this repository.  # noqa: E501
+
+        Retrieve a Ruby upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_ruby_read_with_http_info(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :return: RubyUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['owner', 'identifier', 'slug_perm']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method repos_upstream_ruby_read" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'owner' is set
+        if self.api_client.client_side_validation and ('owner' not in params or
+                                                       params['owner'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `owner` when calling `repos_upstream_ruby_read`")  # noqa: E501
+        # verify the required parameter 'identifier' is set
+        if self.api_client.client_side_validation and ('identifier' not in params or
+                                                       params['identifier'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `identifier` when calling `repos_upstream_ruby_read`")  # noqa: E501
+        # verify the required parameter 'slug_perm' is set
+        if self.api_client.client_side_validation and ('slug_perm' not in params or
+                                                       params['slug_perm'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `slug_perm` when calling `repos_upstream_ruby_read`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'owner' in params:
+            path_params['owner'] = params['owner']  # noqa: E501
+        if 'identifier' in params:
+            path_params['identifier'] = params['identifier']  # noqa: E501
+        if 'slug_perm' in params:
+            path_params['slug_perm'] = params['slug_perm']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/repos/{owner}/{identifier}/upstream/ruby/{slug_perm}/', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='RubyUpstream',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def repos_upstream_ruby_update(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Update a Ruby upstream config for this repository.  # noqa: E501
+
+        Update a Ruby upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_ruby_update(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :param RubyUpstreamRequest data:
+        :return: RubyUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.repos_upstream_ruby_update_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+        else:
+            (data) = self.repos_upstream_ruby_update_with_http_info(owner, identifier, slug_perm, **kwargs)  # noqa: E501
+            return data
+
+    def repos_upstream_ruby_update_with_http_info(self, owner, identifier, slug_perm, **kwargs):  # noqa: E501
+        """Update a Ruby upstream config for this repository.  # noqa: E501
+
+        Update a Ruby upstream config for this repository.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_upstream_ruby_update_with_http_info(owner, identifier, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param str slug_perm: (required)
+        :param RubyUpstreamRequest data:
+        :return: RubyUpstream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['owner', 'identifier', 'slug_perm', 'data']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method repos_upstream_ruby_update" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'owner' is set
+        if self.api_client.client_side_validation and ('owner' not in params or
+                                                       params['owner'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `owner` when calling `repos_upstream_ruby_update`")  # noqa: E501
+        # verify the required parameter 'identifier' is set
+        if self.api_client.client_side_validation and ('identifier' not in params or
+                                                       params['identifier'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `identifier` when calling `repos_upstream_ruby_update`")  # noqa: E501
+        # verify the required parameter 'slug_perm' is set
+        if self.api_client.client_side_validation and ('slug_perm' not in params or
+                                                       params['slug_perm'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `slug_perm` when calling `repos_upstream_ruby_update`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'owner' in params:
+            path_params['owner'] = params['owner']  # noqa: E501
+        if 'identifier' in params:
+            path_params['identifier'] = params['identifier']  # noqa: E501
+        if 'slug_perm' in params:
+            path_params['slug_perm'] = params['slug_perm']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'data' in params:
+            body_params = params['data']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/repos/{owner}/{identifier}/upstream/ruby/{slug_perm}/', 'PUT',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='RubyUpstream',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def repos_user_list(self, **kwargs):  # noqa: E501
         """Get a list of all repositories associated with current user.  # noqa: E501
 
         Get a list of all repositories associated with current user.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.repos_user_list(async_req=True)
```

## cloudsmith_api/models/__init__.py

```diff
@@ -35,49 +35,70 @@
 from cloudsmith_api.models.conan_package_upload_request import ConanPackageUploadRequest
 from cloudsmith_api.models.conda_package_upload import CondaPackageUpload
 from cloudsmith_api.models.conda_package_upload_request import CondaPackageUploadRequest
 from cloudsmith_api.models.cran_package_upload import CranPackageUpload
 from cloudsmith_api.models.cran_package_upload_request import CranPackageUploadRequest
 from cloudsmith_api.models.dart_package_upload import DartPackageUpload
 from cloudsmith_api.models.dart_package_upload_request import DartPackageUploadRequest
+from cloudsmith_api.models.dart_upstream import DartUpstream
+from cloudsmith_api.models.dart_upstream_request import DartUpstreamRequest
+from cloudsmith_api.models.dart_upstream_request_patch import DartUpstreamRequestPatch
 from cloudsmith_api.models.deb_package_upload import DebPackageUpload
 from cloudsmith_api.models.deb_package_upload_request import DebPackageUploadRequest
+from cloudsmith_api.models.deb_upstream import DebUpstream
+from cloudsmith_api.models.deb_upstream_request import DebUpstreamRequest
+from cloudsmith_api.models.deb_upstream_request_patch import DebUpstreamRequestPatch
 from cloudsmith_api.models.distribution import Distribution
 from cloudsmith_api.models.distribution_full import DistributionFull
 from cloudsmith_api.models.distribution_version import DistributionVersion
 from cloudsmith_api.models.docker_package_upload import DockerPackageUpload
 from cloudsmith_api.models.docker_package_upload_request import DockerPackageUploadRequest
+from cloudsmith_api.models.docker_upstream import DockerUpstream
+from cloudsmith_api.models.docker_upstream_request import DockerUpstreamRequest
+from cloudsmith_api.models.docker_upstream_request_patch import DockerUpstreamRequestPatch
 from cloudsmith_api.models.entitlement_usage_metrics import EntitlementUsageMetrics
 from cloudsmith_api.models.error_detail import ErrorDetail
 from cloudsmith_api.models.eula import Eula
 from cloudsmith_api.models.format import Format
 from cloudsmith_api.models.format_support import FormatSupport
 from cloudsmith_api.models.geo_ip_location import GeoIpLocation
 from cloudsmith_api.models.go_package_upload import GoPackageUpload
 from cloudsmith_api.models.go_package_upload_request import GoPackageUploadRequest
 from cloudsmith_api.models.helm_package_upload import HelmPackageUpload
 from cloudsmith_api.models.helm_package_upload_request import HelmPackageUploadRequest
+from cloudsmith_api.models.helm_upstream import HelmUpstream
+from cloudsmith_api.models.helm_upstream_request import HelmUpstreamRequest
+from cloudsmith_api.models.helm_upstream_request_patch import HelmUpstreamRequestPatch
 from cloudsmith_api.models.hex_package_upload import HexPackageUpload
 from cloudsmith_api.models.hex_package_upload_request import HexPackageUploadRequest
 from cloudsmith_api.models.history import History
 from cloudsmith_api.models.history_fieldset import HistoryFieldset
 from cloudsmith_api.models.history_fieldset_raw import HistoryFieldsetRaw
 from cloudsmith_api.models.luarocks_package_upload import LuarocksPackageUpload
 from cloudsmith_api.models.luarocks_package_upload_request import LuarocksPackageUploadRequest
 from cloudsmith_api.models.maven_package_upload import MavenPackageUpload
 from cloudsmith_api.models.maven_package_upload_request import MavenPackageUploadRequest
+from cloudsmith_api.models.maven_upstream import MavenUpstream
+from cloudsmith_api.models.maven_upstream_request import MavenUpstreamRequest
+from cloudsmith_api.models.maven_upstream_request_patch import MavenUpstreamRequestPatch
 from cloudsmith_api.models.namespace import Namespace
 from cloudsmith_api.models.namespace_audit_log import NamespaceAuditLog
 from cloudsmith_api.models.nested_license_policy import NestedLicensePolicy
 from cloudsmith_api.models.nested_vulnerability_policy import NestedVulnerabilityPolicy
 from cloudsmith_api.models.nested_vulnerability_scan_results import NestedVulnerabilityScanResults
 from cloudsmith_api.models.npm_package_upload import NpmPackageUpload
 from cloudsmith_api.models.npm_package_upload_request import NpmPackageUploadRequest
+from cloudsmith_api.models.npm_upstream import NpmUpstream
+from cloudsmith_api.models.npm_upstream_request import NpmUpstreamRequest
+from cloudsmith_api.models.npm_upstream_request_patch import NpmUpstreamRequestPatch
 from cloudsmith_api.models.nuget_package_upload import NugetPackageUpload
 from cloudsmith_api.models.nuget_package_upload_request import NugetPackageUploadRequest
+from cloudsmith_api.models.nuget_upstream import NugetUpstream
+from cloudsmith_api.models.nuget_upstream_request import NugetUpstreamRequest
+from cloudsmith_api.models.nuget_upstream_request_patch import NugetUpstreamRequestPatch
 from cloudsmith_api.models.organization import Organization
 from cloudsmith_api.models.organization_group_sync import OrganizationGroupSync
 from cloudsmith_api.models.organization_group_sync_request import OrganizationGroupSyncRequest
 from cloudsmith_api.models.organization_invite import OrganizationInvite
 from cloudsmith_api.models.organization_invite_extend import OrganizationInviteExtend
 from cloudsmith_api.models.organization_invite_request import OrganizationInviteRequest
 from cloudsmith_api.models.organization_invite_update import OrganizationInviteUpdate
@@ -101,31 +122,38 @@
 from cloudsmith_api.models.package_copy_request import PackageCopyRequest
 from cloudsmith_api.models.package_dependencies import PackageDependencies
 from cloudsmith_api.models.package_dependency import PackageDependency
 from cloudsmith_api.models.package_file import PackageFile
 from cloudsmith_api.models.package_file_parts_upload import PackageFilePartsUpload
 from cloudsmith_api.models.package_file_upload import PackageFileUpload
 from cloudsmith_api.models.package_file_upload_request import PackageFileUploadRequest
+from cloudsmith_api.models.package_license_policy_evaluation_request import PackageLicensePolicyEvaluationRequest
+from cloudsmith_api.models.package_license_policy_evaluation_request_request import PackageLicensePolicyEvaluationRequestRequest
 from cloudsmith_api.models.package_license_policy_violation_log import PackageLicensePolicyViolationLog
 from cloudsmith_api.models.package_license_policy_violation_log_cursor_page import PackageLicensePolicyViolationLogCursorPage
 from cloudsmith_api.models.package_move import PackageMove
 from cloudsmith_api.models.package_move_request import PackageMoveRequest
 from cloudsmith_api.models.package_quarantine import PackageQuarantine
 from cloudsmith_api.models.package_quarantine_request import PackageQuarantineRequest
 from cloudsmith_api.models.package_resync import PackageResync
 from cloudsmith_api.models.package_status import PackageStatus
 from cloudsmith_api.models.package_tag import PackageTag
 from cloudsmith_api.models.package_tag_request import PackageTagRequest
 from cloudsmith_api.models.package_usage_metrics import PackageUsageMetrics
 from cloudsmith_api.models.package_version_badge import PackageVersionBadge
 from cloudsmith_api.models.package_vulnerability import PackageVulnerability
+from cloudsmith_api.models.package_vulnerability_policy_evaluation_request import PackageVulnerabilityPolicyEvaluationRequest
+from cloudsmith_api.models.package_vulnerability_policy_evaluation_request_request import PackageVulnerabilityPolicyEvaluationRequestRequest
 from cloudsmith_api.models.package_vulnerability_policy_violation_log import PackageVulnerabilityPolicyViolationLog
 from cloudsmith_api.models.package_vulnerability_policy_violation_log_cursor_page import PackageVulnerabilityPolicyViolationLogCursorPage
 from cloudsmith_api.models.python_package_upload import PythonPackageUpload
 from cloudsmith_api.models.python_package_upload_request import PythonPackageUploadRequest
+from cloudsmith_api.models.python_upstream import PythonUpstream
+from cloudsmith_api.models.python_upstream_request import PythonUpstreamRequest
+from cloudsmith_api.models.python_upstream_request_patch import PythonUpstreamRequestPatch
 from cloudsmith_api.models.quota import Quota
 from cloudsmith_api.models.quota_history import QuotaHistory
 from cloudsmith_api.models.rate_check import RateCheck
 from cloudsmith_api.models.raw_package_upload import RawPackageUpload
 from cloudsmith_api.models.raw_package_upload_request import RawPackageUploadRequest
 from cloudsmith_api.models.repository import Repository
 from cloudsmith_api.models.repository_audit_log import RepositoryAuditLog
@@ -160,16 +188,22 @@
 from cloudsmith_api.models.repository_webhook_request import RepositoryWebhookRequest
 from cloudsmith_api.models.repository_webhook_request_patch import RepositoryWebhookRequestPatch
 from cloudsmith_api.models.resources_rate_check import ResourcesRateCheck
 from cloudsmith_api.models.respository_geo_ip_enable_disable import RespositoryGeoIpEnableDisable
 from cloudsmith_api.models.respository_geo_ip_enable_disable_request import RespositoryGeoIpEnableDisableRequest
 from cloudsmith_api.models.rpm_package_upload import RpmPackageUpload
 from cloudsmith_api.models.rpm_package_upload_request import RpmPackageUploadRequest
+from cloudsmith_api.models.rpm_upstream import RpmUpstream
+from cloudsmith_api.models.rpm_upstream_request import RpmUpstreamRequest
+from cloudsmith_api.models.rpm_upstream_request_patch import RpmUpstreamRequestPatch
 from cloudsmith_api.models.ruby_package_upload import RubyPackageUpload
 from cloudsmith_api.models.ruby_package_upload_request import RubyPackageUploadRequest
+from cloudsmith_api.models.ruby_upstream import RubyUpstream
+from cloudsmith_api.models.ruby_upstream_request import RubyUpstreamRequest
+from cloudsmith_api.models.ruby_upstream_request_patch import RubyUpstreamRequestPatch
 from cloudsmith_api.models.service import Service
 from cloudsmith_api.models.service_request import ServiceRequest
 from cloudsmith_api.models.service_request_patch import ServiceRequestPatch
 from cloudsmith_api.models.service_teams import ServiceTeams
 from cloudsmith_api.models.status_basic import StatusBasic
 from cloudsmith_api.models.storage_allocated_limit import StorageAllocatedLimit
 from cloudsmith_api.models.storage_allocated_limit_raw import StorageAllocatedLimitRaw
```

## cloudsmith_api/models/status_basic.py

```diff
@@ -38,15 +38,15 @@
     }
 
     attribute_map = {
         'detail': 'detail',
         'version': 'version'
     }
 
-    def __init__(self, detail='Cloudsmith API is operational.', version='1.283.1', _configuration=None):  # noqa: E501
+    def __init__(self, detail='Cloudsmith API is operational.', version='1.290.2', _configuration=None):  # noqa: E501
         """StatusBasic - a model defined in Swagger"""  # noqa: E501
         if _configuration is None:
             _configuration = Configuration()
         self._configuration = _configuration
 
         self._detail = None
         self._version = None
```

## cloudsmith_api/models/vulnerability_scan_version.py

```diff
@@ -185,16 +185,16 @@
         """Sets the raw_version of this VulnerabilityScanVersion.
 
 
         :param raw_version: The raw_version of this VulnerabilityScanVersion.
         :type: str
         """
         if (self._configuration.client_side_validation and
-                raw_version is not None and len(raw_version) > 128):
-            raise ValueError("Invalid value for `raw_version`, length must be less than or equal to `128`")  # noqa: E501
+                raw_version is not None and len(raw_version) > 1024):
+            raise ValueError("Invalid value for `raw_version`, length must be less than or equal to `1024`")  # noqa: E501
         if (self._configuration.client_side_validation and
                 raw_version is not None and len(raw_version) < 1):
             raise ValueError("Invalid value for `raw_version`, length must be greater than or equal to `1`")  # noqa: E501
 
         self._raw_version = raw_version
 
     @property
```

## test/test_orgs_api.py

```diff
@@ -81,14 +81,35 @@
     def test_orgs_license_policy_delete(self):
         """Test case for orgs_license_policy_delete
 
         Delete a package license policy.  # noqa: E501
         """
         pass
 
+    def test_orgs_license_policy_evaluation_create(self):
+        """Test case for orgs_license_policy_evaluation_create
+
+        Create an evaluation request for this policy.  # noqa: E501
+        """
+        pass
+
+    def test_orgs_license_policy_evaluation_list(self):
+        """Test case for orgs_license_policy_evaluation_list
+
+        List evaluation requests for this policy.  # noqa: E501
+        """
+        pass
+
+    def test_orgs_license_policy_evaluation_read(self):
+        """Test case for orgs_license_policy_evaluation_read
+
+        Retrieve an evaluation request for this policy.  # noqa: E501
+        """
+        pass
+
     def test_orgs_license_policy_list(self):
         """Test case for orgs_license_policy_list
 
         Get a list of all package license policies.  # noqa: E501
         """
         pass
 
@@ -298,14 +319,35 @@
     def test_orgs_vulnerability_policy_delete(self):
         """Test case for orgs_vulnerability_policy_delete
 
         Delete a package vulnerability policy.  # noqa: E501
         """
         pass
 
+    def test_orgs_vulnerability_policy_evaluation_create(self):
+        """Test case for orgs_vulnerability_policy_evaluation_create
+
+        Create an evaluation request for this policy.  # noqa: E501
+        """
+        pass
+
+    def test_orgs_vulnerability_policy_evaluation_list(self):
+        """Test case for orgs_vulnerability_policy_evaluation_list
+
+        List evaluation requests for this policy.  # noqa: E501
+        """
+        pass
+
+    def test_orgs_vulnerability_policy_evaluation_read(self):
+        """Test case for orgs_vulnerability_policy_evaluation_read
+
+        Retrieve an evaluation request for this policy.  # noqa: E501
+        """
+        pass
+
     def test_orgs_vulnerability_policy_list(self):
         """Test case for orgs_vulnerability_policy_list
 
         Get a list of all package vulnerability policies.  # noqa: E501
         """
         pass
```

## test/test_repos_api.py

```diff
@@ -165,14 +165,434 @@
     def test_repos_rsa_regenerate(self):
         """Test case for repos_rsa_regenerate
 
         Regenerate RSA Key for the Repository.  # noqa: E501
         """
         pass
 
+    def test_repos_upstream_dart_create(self):
+        """Test case for repos_upstream_dart_create
+
+        Create a Dart upstream config for this repository.  # noqa: E501
+        """
+        pass
+
+    def test_repos_upstream_dart_delete(self):
+        """Test case for repos_upstream_dart_delete
+
+        Delete a Dart upstream config for this repository.  # noqa: E501
+        """
+        pass
+
+    def test_repos_upstream_dart_list(self):
+        """Test case for repos_upstream_dart_list
+
+        List Dart upstream configs for this repository.  # noqa: E501
+        """
+        pass
+
+    def test_repos_upstream_dart_partial_update(self):
+        """Test case for repos_upstream_dart_partial_update
+
+        Partially update a Dart upstream config for this repository.  # noqa: E501
+        """
+        pass
+
+    def test_repos_upstream_dart_read(self):
+        """Test case for repos_upstream_dart_read
+
+        Retrieve a Dart upstream config for this repository.  # noqa: E501
+        """
+        pass
+
+    def test_repos_upstream_dart_update(self):
+        """Test case for repos_upstream_dart_update
+
+        Update a Dart upstream config for this repository.  # noqa: E501
+        """
+        pass
+
+    def test_repos_upstream_deb_create(self):
+        """Test case for repos_upstream_deb_create
+
+        Create a Debian upstream config for this repository.  # noqa: E501
+        """
+        pass
+
+    def test_repos_upstream_deb_delete(self):
+        """Test case for repos_upstream_deb_delete
+
+        Delete a Debian upstream config for this repository.  # noqa: E501
+        """
+        pass
+
+    def test_repos_upstream_deb_list(self):
+        """Test case for repos_upstream_deb_list
+
+        List Debian upstream configs for this repository.  # noqa: E501
+        """
+        pass
+
+    def test_repos_upstream_deb_partial_update(self):
+        """Test case for repos_upstream_deb_partial_update
+
+        Partially update a Debian upstream config for this repository.  # noqa: E501
+        """
+        pass
+
+    def test_repos_upstream_deb_read(self):
+        """Test case for repos_upstream_deb_read
+
+        Retrieve a Debian upstream config for this repository.  # noqa: E501
+        """
+        pass
+
+    def test_repos_upstream_deb_update(self):
+        """Test case for repos_upstream_deb_update
+
+        Update a Debian upstream config for this repository.  # noqa: E501
+        """
+        pass
+
+    def test_repos_upstream_docker_create(self):
+        """Test case for repos_upstream_docker_create
+
+        Create a Docker upstream config for this repository.  # noqa: E501
+        """
+        pass
+
+    def test_repos_upstream_docker_delete(self):
+        """Test case for repos_upstream_docker_delete
+
+        Delete a Docker upstream config for this repository.  # noqa: E501
+        """
+        pass
+
+    def test_repos_upstream_docker_list(self):
+        """Test case for repos_upstream_docker_list
+
+        List Docker upstream configs for this repository.  # noqa: E501
+        """
+        pass
+
+    def test_repos_upstream_docker_partial_update(self):
+        """Test case for repos_upstream_docker_partial_update
+
+        Partially update a Docker upstream config for this repository.  # noqa: E501
+        """
+        pass
+
+    def test_repos_upstream_docker_read(self):
+        """Test case for repos_upstream_docker_read
+
+        Retrieve a Docker upstream config for this repository.  # noqa: E501
+        """
+        pass
+
+    def test_repos_upstream_docker_update(self):
+        """Test case for repos_upstream_docker_update
+
+        Update a Docker upstream config for this repository.  # noqa: E501
+        """
+        pass
+
+    def test_repos_upstream_helm_create(self):
+        """Test case for repos_upstream_helm_create
+
+        Create a Helm upstream config for this repository.  # noqa: E501
+        """
+        pass
+
+    def test_repos_upstream_helm_delete(self):
+        """Test case for repos_upstream_helm_delete
+
+        Delete a Helm upstream config for this repository.  # noqa: E501
+        """
+        pass
+
+    def test_repos_upstream_helm_list(self):
+        """Test case for repos_upstream_helm_list
+
+        List Helm upstream configs for this repository.  # noqa: E501
+        """
+        pass
+
+    def test_repos_upstream_helm_partial_update(self):
+        """Test case for repos_upstream_helm_partial_update
+
+        Partially update a Helm upstream config for this repository.  # noqa: E501
+        """
+        pass
+
+    def test_repos_upstream_helm_read(self):
+        """Test case for repos_upstream_helm_read
+
+        Retrieve a Helm upstream config for this repository.  # noqa: E501
+        """
+        pass
+
+    def test_repos_upstream_helm_update(self):
+        """Test case for repos_upstream_helm_update
+
+        Update a Helm upstream config for this repository.  # noqa: E501
+        """
+        pass
+
+    def test_repos_upstream_maven_create(self):
+        """Test case for repos_upstream_maven_create
+
+        Create a Maven upstream config for this repository.  # noqa: E501
+        """
+        pass
+
+    def test_repos_upstream_maven_delete(self):
+        """Test case for repos_upstream_maven_delete
+
+        Delete a Maven upstream config for this repository.  # noqa: E501
+        """
+        pass
+
+    def test_repos_upstream_maven_list(self):
+        """Test case for repos_upstream_maven_list
+
+        List Maven upstream configs for this repository.  # noqa: E501
+        """
+        pass
+
+    def test_repos_upstream_maven_partial_update(self):
+        """Test case for repos_upstream_maven_partial_update
+
+        Partially update a Maven upstream config for this repository.  # noqa: E501
+        """
+        pass
+
+    def test_repos_upstream_maven_read(self):
+        """Test case for repos_upstream_maven_read
+
+        Retrieve a Maven upstream config for this repository.  # noqa: E501
+        """
+        pass
+
+    def test_repos_upstream_maven_update(self):
+        """Test case for repos_upstream_maven_update
+
+        Update a Maven upstream config for this repository.  # noqa: E501
+        """
+        pass
+
+    def test_repos_upstream_npm_create(self):
+        """Test case for repos_upstream_npm_create
+
+        Create a npm upstream config for this repository.  # noqa: E501
+        """
+        pass
+
+    def test_repos_upstream_npm_delete(self):
+        """Test case for repos_upstream_npm_delete
+
+        Delete a npm upstream config for this repository.  # noqa: E501
+        """
+        pass
+
+    def test_repos_upstream_npm_list(self):
+        """Test case for repos_upstream_npm_list
+
+        List npm upstream configs for this repository.  # noqa: E501
+        """
+        pass
+
+    def test_repos_upstream_npm_partial_update(self):
+        """Test case for repos_upstream_npm_partial_update
+
+        Partially update a npm upstream config for this repository.  # noqa: E501
+        """
+        pass
+
+    def test_repos_upstream_npm_read(self):
+        """Test case for repos_upstream_npm_read
+
+        Retrieve a npm upstream config for this repository.  # noqa: E501
+        """
+        pass
+
+    def test_repos_upstream_npm_update(self):
+        """Test case for repos_upstream_npm_update
+
+        Update a npm upstream config for this repository.  # noqa: E501
+        """
+        pass
+
+    def test_repos_upstream_nuget_create(self):
+        """Test case for repos_upstream_nuget_create
+
+        Create a NuGet upstream config for this repository.  # noqa: E501
+        """
+        pass
+
+    def test_repos_upstream_nuget_delete(self):
+        """Test case for repos_upstream_nuget_delete
+
+        Delete a NuGet upstream config for this repository.  # noqa: E501
+        """
+        pass
+
+    def test_repos_upstream_nuget_list(self):
+        """Test case for repos_upstream_nuget_list
+
+        List NuGet upstream configs for this repository.  # noqa: E501
+        """
+        pass
+
+    def test_repos_upstream_nuget_partial_update(self):
+        """Test case for repos_upstream_nuget_partial_update
+
+        Partially update a NuGet upstream config for this repository.  # noqa: E501
+        """
+        pass
+
+    def test_repos_upstream_nuget_read(self):
+        """Test case for repos_upstream_nuget_read
+
+        Retrieve a NuGet upstream config for this repository.  # noqa: E501
+        """
+        pass
+
+    def test_repos_upstream_nuget_update(self):
+        """Test case for repos_upstream_nuget_update
+
+        Update a NuGet upstream config for this repository.  # noqa: E501
+        """
+        pass
+
+    def test_repos_upstream_python_create(self):
+        """Test case for repos_upstream_python_create
+
+        Create a Python upstream config for this repository.  # noqa: E501
+        """
+        pass
+
+    def test_repos_upstream_python_delete(self):
+        """Test case for repos_upstream_python_delete
+
+        Delete a Python upstream config for this repository.  # noqa: E501
+        """
+        pass
+
+    def test_repos_upstream_python_list(self):
+        """Test case for repos_upstream_python_list
+
+        List Python upstream configs for this repository.  # noqa: E501
+        """
+        pass
+
+    def test_repos_upstream_python_partial_update(self):
+        """Test case for repos_upstream_python_partial_update
+
+        Partially update a Python upstream config for this repository.  # noqa: E501
+        """
+        pass
+
+    def test_repos_upstream_python_read(self):
+        """Test case for repos_upstream_python_read
+
+        Retrieve a Python upstream config for this repository.  # noqa: E501
+        """
+        pass
+
+    def test_repos_upstream_python_update(self):
+        """Test case for repos_upstream_python_update
+
+        Update a Python upstream config for this repository.  # noqa: E501
+        """
+        pass
+
+    def test_repos_upstream_rpm_create(self):
+        """Test case for repos_upstream_rpm_create
+
+        Create a RedHat upstream config for this repository.  # noqa: E501
+        """
+        pass
+
+    def test_repos_upstream_rpm_delete(self):
+        """Test case for repos_upstream_rpm_delete
+
+        Delete a RedHat upstream config for this repository.  # noqa: E501
+        """
+        pass
+
+    def test_repos_upstream_rpm_list(self):
+        """Test case for repos_upstream_rpm_list
+
+        List RedHat upstream configs for this repository.  # noqa: E501
+        """
+        pass
+
+    def test_repos_upstream_rpm_partial_update(self):
+        """Test case for repos_upstream_rpm_partial_update
+
+        Partially update a RedHat upstream config for this repository.  # noqa: E501
+        """
+        pass
+
+    def test_repos_upstream_rpm_read(self):
+        """Test case for repos_upstream_rpm_read
+
+        Retrieve a RedHat upstream config for this repository.  # noqa: E501
+        """
+        pass
+
+    def test_repos_upstream_rpm_update(self):
+        """Test case for repos_upstream_rpm_update
+
+        Update a RedHat upstream config for this repository.  # noqa: E501
+        """
+        pass
+
+    def test_repos_upstream_ruby_create(self):
+        """Test case for repos_upstream_ruby_create
+
+        Create a Ruby upstream config for this repository.  # noqa: E501
+        """
+        pass
+
+    def test_repos_upstream_ruby_delete(self):
+        """Test case for repos_upstream_ruby_delete
+
+        Delete a Ruby upstream config for this repository.  # noqa: E501
+        """
+        pass
+
+    def test_repos_upstream_ruby_list(self):
+        """Test case for repos_upstream_ruby_list
+
+        List Ruby upstream configs for this repository.  # noqa: E501
+        """
+        pass
+
+    def test_repos_upstream_ruby_partial_update(self):
+        """Test case for repos_upstream_ruby_partial_update
+
+        Partially update a Ruby upstream config for this repository.  # noqa: E501
+        """
+        pass
+
+    def test_repos_upstream_ruby_read(self):
+        """Test case for repos_upstream_ruby_read
+
+        Retrieve a Ruby upstream config for this repository.  # noqa: E501
+        """
+        pass
+
+    def test_repos_upstream_ruby_update(self):
+        """Test case for repos_upstream_ruby_update
+
+        Update a Ruby upstream config for this repository.  # noqa: E501
+        """
+        pass
+
     def test_repos_user_list(self):
         """Test case for repos_user_list
 
         Get a list of all repositories associated with current user.  # noqa: E501
         """
         pass
```

## Comparing `cloudsmith_api-2.0.6.dist-info/RECORD` & `cloudsmith_api-2.0.7.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-cloudsmith_api/__init__.py,sha256=8dyH4Dd5vPZFMamSZyUgDyQ5Bv7umS4wPMFa0LToloc,16073
-cloudsmith_api/api_client.py,sha256=D98rCfXfJkuYBtZfJoZmYrC9al9EsVarW3QnaB5RVKk,25067
-cloudsmith_api/configuration.py,sha256=lhJjML-XpIcCJEzXNEcGb0F7eFSNNZ8g6wfsQmYoyw8,8390
+cloudsmith_api/__init__.py,sha256=0Qepha8d6SMR75TUJES_5Ls8BNZC3H4O0fjvaQpbpnc,18841
+cloudsmith_api/api_client.py,sha256=WsSzKbtc3c6-ZIifuAVTjDXHhlBfbmYsw5LIVU7CQ6Q,25067
+cloudsmith_api/configuration.py,sha256=oFuwZDorudpX5nby-WObhjlyDpthF17rr4Jp-rTYTLg,8390
 cloudsmith_api/rest.py,sha256=IVGz52ALLAOqfC3YGAkqFfFjiLz5mAB_R0mIs51372Y,13166
 cloudsmith_api/api/__init__.py,sha256=oHMaETBtdkm77g6ZMGgBaWJb1Q3a8jlD8Nh02VKZd2U,1131
 cloudsmith_api/api/audit_log_api.py,sha256=cDN0Rsgck9w4qB19hpWzsTETl41Zsm-pk8Wrr14EDGs,11039
 cloudsmith_api/api/badges_api.py,sha256=PF8u5FZiEm1BFP8e52ZEDjzMo9skZVM9Qc7arsPk4vc,11425
 cloudsmith_api/api/distros_api.py,sha256=44C2sU3C43GkhRNPLK-jxlB8KrS8-KFe7Bj7KxAc-cU,7978
 cloudsmith_api/api/entitlements_api.py,sha256=Ao8Zk99xiIDEf-5GTz9YbgyaVig05QDGN0Pc2TpZmmo,54786
 cloudsmith_api/api/files_api.py,sha256=lsuhZ5M3ugbdQoqeci23QCYe15g2zVmJ3nF_nRsljZM,26620
 cloudsmith_api/api/formats_api.py,sha256=7Bv_EKqHBEnSHJIbtQ_oh-5laVu5EmofmZwBJo9h4og,7930
 cloudsmith_api/api/metrics_api.py,sha256=cTqkKtutQn2u-zNS7FHVTkxX-LSc3xRpjgbLDIqsWWc,19214
 cloudsmith_api/api/namespaces_api.py,sha256=2qCN92-asz_tZyASYgXE7gpAPBfL6W13khfmuOYV8CA,8514
-cloudsmith_api/api/orgs_api.py,sha256=1byeUdbyyl0BXEwUxNicCq7JWYizv2qj-aRQZBrgFac,199931
+cloudsmith_api/api/orgs_api.py,sha256=TRFxXQu-v5p_BjsXqErq7KSw3Nyjur9juqMs9WloMbE,232571
 cloudsmith_api/api/packages_api.py,sha256=8RLm6j343dJzWSWNAEUHqmmg86nTY2-UBzRCXb7U1-c,294424
 cloudsmith_api/api/quota_api.py,sha256=cLljkIY1w8-urDPf5Zi31YdaoWsyVrzKKz1t3Qasm_w,16386
 cloudsmith_api/api/rates_api.py,sha256=iVavoIQtWfbFE6C_jPnTQP8uG8wk0YS-ejHztrajZdY,4157
-cloudsmith_api/api/repos_api.py,sha256=9IYStNbWWFqBnTEQfDnB14Dfp4-jrVfMG7Ea0FBnKUo,98642
+cloudsmith_api/api/repos_api.py,sha256=aqFaxOdRNC7qcF63XgwmHuwI_2nMxitAt5LHyJlB8Ug,418673
 cloudsmith_api/api/status_api.py,sha256=Y7fJjz1UeBzgC2y7F8EcnBuJIFUh553zQDdk1oLGOIQ,4118
 cloudsmith_api/api/storage_regions_api.py,sha256=27lr9PVQ8G84depb-1M7z1dJ5srWscFsU776W7SRVpc,8075
 cloudsmith_api/api/user_api.py,sha256=B2_HoP2ZNBYI-2GfmmSEmucylTZV_VhU7GnnP4aYPpE,7631
 cloudsmith_api/api/users_api.py,sha256=fjOMJWnFJ8qx5i5WkiR4cdpsKR2RzdoUT_V0w-TIZVM,4706
 cloudsmith_api/api/vulnerabilities_api.py,sha256=gF5GPsUNONLhHE7bf_MIvqlyNU967AZVm0wHNWmYIoY,22091
 cloudsmith_api/api/webhooks_api.py,sha256=RsnHyob8BKBLbqKHq3U7TizhcFJF-VCkgzJllmTZliw,26050
-cloudsmith_api/models/__init__.py,sha256=Tt-KCq4X7QKa-F8k91JLlPVJ26mf8S9s7bxQq1WBje8,14876
+cloudsmith_api/models/__init__.py,sha256=47DRDQK6OXUcyPNz4SGWflqYGFe7B-eQ6SIyQkMTwAw,17644
 cloudsmith_api/models/allocated_limit.py,sha256=1SlEiDZ2Ozouu8Gg6CrYf47I7pJjyxUOCFtJd7Q0yzA,7305
 cloudsmith_api/models/allocated_limit_raw.py,sha256=p6vlL-y9gGwoER9aLnDeexcM0Ci6W5as9765n74SfRE,5410
 cloudsmith_api/models/alpine_package_upload.py,sha256=IUVVXR1YrQt0d52V93rFkdkHGg5YkymjC4pjUKpcxrQ,58771
 cloudsmith_api/models/alpine_package_upload_request.py,sha256=jrzolgP1mvgRKgLiDfWe6J2VS9hywOudnbpg-8zM3lk,7437
 cloudsmith_api/models/architecture.py,sha256=bzGmeP8O7tYFZfdkboF5_E34LlX-NyN2HU4W9T1Bkds,4748
 cloudsmith_api/models/cargo_package_upload.py,sha256=y6a8rNJxe9H4GWMv72MJkqnCPP-7L3YfGALtFbn8RvI,58494
 cloudsmith_api/models/cargo_package_upload_request.py,sha256=RmfIq722CsU9jPUpsofwJRXdTzjwZ0OG8js66XFUPpQ,6177
@@ -43,49 +43,70 @@
 cloudsmith_api/models/conan_package_upload_request.py,sha256=VHMAAtkEMzK8g9XaRaUdBoNW7m-CGok-g5eaPqe3gWU,14491
 cloudsmith_api/models/conda_package_upload.py,sha256=fWfCXkGnNQeciaQl52-gdjhM8fpIX1KkCO2MxaplHPU,58494
 cloudsmith_api/models/conda_package_upload_request.py,sha256=Yrt_T2OeqI8I0Qv1BcN1GPiLv9Zwu8HvR8FNwC7Idr4,6177
 cloudsmith_api/models/cran_package_upload.py,sha256=Eiz1VzQhaPCsuIWwiY7sSQCOq5BtAi32IshtiwubIeg,58217
 cloudsmith_api/models/cran_package_upload_request.py,sha256=5XexroNqcXb68ksP2fQxpxWcvXZ2vRvYpNaObjATg3E,6160
 cloudsmith_api/models/dart_package_upload.py,sha256=w-q2br5i2nYIRQRgDiVWuMOgtPumSgXbC4cro1nVSCQ,58217
 cloudsmith_api/models/dart_package_upload_request.py,sha256=M1K2ao-1mihv4b6_OMksIalVTPVQb7SVTEzJ7eSQE2o,6160
+cloudsmith_api/models/dart_upstream.py,sha256=CeUmQBOyIWClhMzD--oWcVNRNOzDqUjX1qyCv_PlgcQ,22261
+cloudsmith_api/models/dart_upstream_request.py,sha256=sGmbLrSbVA-aGa_MwMx9vpUSiD50_c9ohe1G8gApim0,20036
+cloudsmith_api/models/dart_upstream_request_patch.py,sha256=6aACCEVcgeOXlK63eIDYpcIRWdPaJj1qqpKXx_EAe-c,20053
 cloudsmith_api/models/deb_package_upload.py,sha256=jNuEFXTcrbM0dGOEesLMZDKMdLRuxl4noCm4PJGCgSk,57940
 cloudsmith_api/models/deb_package_upload_request.py,sha256=G4YEAXXzlhIF5RHG0dVodj3xzZ8IdzIF6a0qVAQJR28,9690
+cloudsmith_api/models/deb_upstream.py,sha256=tqGyNb5U-JKlxCKSL9WI4EkhuixPqwx9vRrbii7VnMM,26959
+cloudsmith_api/models/deb_upstream_request.py,sha256=BGzpEqAjc-s_5bVv6_Jjz5w_OgJIIj3RyU01FBF8j10,24858
+cloudsmith_api/models/deb_upstream_request_patch.py,sha256=ksGs_XvyR-I6RUG9bmxQeuQ-ZYpLCeXhk-MG_2oVfvM,24814
 cloudsmith_api/models/distribution.py,sha256=5mh3fWHu2vQU55xO00F4cEoaq76Dtl9sFAqx_WU8y6U,6159
 cloudsmith_api/models/distribution_full.py,sha256=xtxjZk2KOtB__JUCFv--RslyfXI8Pj_g1VaxhTpMdxU,8542
 cloudsmith_api/models/distribution_version.py,sha256=9EFxXMgzUVHKjvELtjUQThMkfpKiwsGA6ctJ8nVKGAY,4497
 cloudsmith_api/models/docker_package_upload.py,sha256=0wb3UWMXsq4W9heBrBUG9FiKHENK3gUShys80ozqjaI,58771
 cloudsmith_api/models/docker_package_upload_request.py,sha256=ZS0lzh-aryr88n5-tVxU3dFrF4wSHe-xsq8Zn4cTbcg,6194
+cloudsmith_api/models/docker_upstream.py,sha256=DpuleMHNePKwi8mDENM7s0Zwt9Yeg9OaaUzIsX4Y_Ws,22418
+cloudsmith_api/models/docker_upstream_request.py,sha256=7J2vA6he_lfKRo2YKM2fZ-wpGQ8KkLbL_vqypbbUeMM,20169
+cloudsmith_api/models/docker_upstream_request_patch.py,sha256=XjkzZ6o7lsD-pHS-SXK1EHKAhJYGTU7YJKg3oK5jnmA,20186
 cloudsmith_api/models/entitlement_usage_metrics.py,sha256=fC2EAybHNP8Fp5Au-VPsEqvA9UQaB-5I1-zLiq-URVc,3541
 cloudsmith_api/models/error_detail.py,sha256=nUsm2ghwLE3GFYyz48jSjqqCbakBefdXR1PTGKaAelw,3729
 cloudsmith_api/models/eula.py,sha256=_dafCxq6v5Cz8HxaCyjTr0T-ka9oMqsc36vy_QLuAwk,5458
 cloudsmith_api/models/format.py,sha256=w9JIldZS2mRBRKo-4tYyPP9ve-4wdF-xTf9gEBvJMuI,11287
 cloudsmith_api/models/format_support.py,sha256=-TbnGczxma_ziAuD4ss-jwdHSPhE6cAI_za52K_Gbpg,7319
 cloudsmith_api/models/geo_ip_location.py,sha256=w5oOjWMH_GcOQtcUwVo0gWk_dDkPVGwmHJ2IC0RxURY,8615
 cloudsmith_api/models/go_package_upload.py,sha256=Slt7_6-PvfajmCK0wHQOKjbdwBA9qs4EgZf__MtSvFE,57663
 cloudsmith_api/models/go_package_upload_request.py,sha256=UgLfJ7yrqfuch7bEjriI8c151CWwStC21nsgOl3Hw4g,6126
 cloudsmith_api/models/helm_package_upload.py,sha256=1AwH6eg9iLHxOf-VK1lzNuWqof7zGa3D1YXjhx7YnrA,58217
 cloudsmith_api/models/helm_package_upload_request.py,sha256=X4b94ShCVDyD9nsReMyrgvzq6MX8W51xyuC9cqbgQQE,7480
+cloudsmith_api/models/helm_upstream.py,sha256=bbRqmZRIjFrB39ZaixfjbtI6nXL9Pl0iUPQuONi583g,22280
+cloudsmith_api/models/helm_upstream_request.py,sha256=aVqgreYYewlU2KZz226PiBXAPmjrStRez14ANCE6Zmg,20055
+cloudsmith_api/models/helm_upstream_request_patch.py,sha256=R4w9HtOijFDPYWie34ZT9-JmJWg4oIsTn3mLhHETujA,20072
 cloudsmith_api/models/hex_package_upload.py,sha256=cPGtS3VlNKXbKRbuwuDOvM8FTzNOebDym4xM6u9oQ7Y,57940
 cloudsmith_api/models/hex_package_upload_request.py,sha256=q-4Uh4f2OJmPY4CDL-P6YhlMGpOogbakNnMcYUPBNhs,6143
 cloudsmith_api/models/history.py,sha256=17AfMvcTcXVi0L8gkqSdytdMeVbNRrLVSToP9SnWsxE,7028
 cloudsmith_api/models/history_fieldset.py,sha256=Cng-daGoLVr2Hc2tlZ7_lktiEllkIGUcKjcTKG0pU-Q,5168
 cloudsmith_api/models/history_fieldset_raw.py,sha256=EV7mi9q3pTap9fsh1cVuSpTUrHrQxcmUreT-EFoUcq0,5246
 cloudsmith_api/models/luarocks_package_upload.py,sha256=D8VMxUWsIKi-evMg-AJW0r89t3hVfhrlSfa6jDNYMjM,59325
 cloudsmith_api/models/luarocks_package_upload_request.py,sha256=FQc8EpOCyRHBRBOmLC9xAl0TlZihGUnLhCE-hUlnIjk,6228
 cloudsmith_api/models/maven_package_upload.py,sha256=HX5WCoNMd4SfpbZg5gNLbk89tLFNU0fYwyr_6hubhLM,63607
 cloudsmith_api/models/maven_package_upload_request.py,sha256=HjJBJOxKNaM60-mC8b580a_lmQDEKwQEV4TPpkT9pvk,17576
+cloudsmith_api/models/maven_upstream.py,sha256=2dlS160QhjZOB6TZYp1VXfjECINv_sw_x8Ih8OuRinA,22363
+cloudsmith_api/models/maven_upstream_request.py,sha256=6fMu0nnakHLLZ4WqfVOQech6SJp7dUzTpXduqsEQjWE,20126
+cloudsmith_api/models/maven_upstream_request_patch.py,sha256=6wPH2-TqdpuHyZFCCtESSy7zhn2sfiXnZLIKPOoBP68,20143
 cloudsmith_api/models/namespace.py,sha256=pPo1q6hL3GaOyfeMuz85jZtPvZ7NZ5pM7GKt4VQPFfw,5806
 cloudsmith_api/models/namespace_audit_log.py,sha256=WRKsSuHhPThpTFC9aQLbWMIjxXpimne5yzQkxK-VtkU,18223
 cloudsmith_api/models/nested_license_policy.py,sha256=YbHzNrWlplzoXh67Oc_sWEsILyvD8Cui3S1n1dulX-E,11620
 cloudsmith_api/models/nested_vulnerability_policy.py,sha256=fzPV_bEEBmwvbzfQuVJHUe651yw8J3Q9tJlNRVCWJlY,12280
 cloudsmith_api/models/nested_vulnerability_scan_results.py,sha256=qvEo7UgdZvUIvphxs78C6M9ev30XpAGuDwIESAI7AWA,9527
 cloudsmith_api/models/npm_package_upload.py,sha256=IEPmH7bgimdDPVNzVZDpKI03DNtqQYnJW5qFXI1SUHw,57940
 cloudsmith_api/models/npm_package_upload_request.py,sha256=xpqvQTM7dP6S81Ztl89g0PoQoVCTg8QJr1hlZ5wZmR4,7663
+cloudsmith_api/models/npm_upstream.py,sha256=fjaII__2psvmKTTl7cX4X5gbltH3HyB0DVmM9tAr5fk,22220
+cloudsmith_api/models/npm_upstream_request.py,sha256=vTCFvAaAEoyjip4UStBwSSW-iQ_CZYUOXbPBriQ6zwM,20007
+cloudsmith_api/models/npm_upstream_request_patch.py,sha256=QXkhy8gJilogi9bQKQNbjwKusaZHwLpwOvc7V51Uhqk,20024
 cloudsmith_api/models/nuget_package_upload.py,sha256=eExC3CDlMs3F_LvmunNevVqw3H6pTrpz-Bfoc17uW5c,58494
 cloudsmith_api/models/nuget_package_upload_request.py,sha256=_V5hSUOnLmqhcbTKRgYQIaAINNMxtcx2oYRSOXQP4No,7272
+cloudsmith_api/models/nuget_upstream.py,sha256=S9QMlJZoQDYS4xSOen7BbX4fqa6fpBRMOGBIyEKTwGE,22349
+cloudsmith_api/models/nuget_upstream_request.py,sha256=D0hhWMii6T6LBOsRGvActRvQPYYuSIKrNmwOIK7lhMs,20112
+cloudsmith_api/models/nuget_upstream_request_patch.py,sha256=mdetkNvD4FUDBlsXTKqrVM27fNTDhCJpUQbg8B5RF-o,20129
 cloudsmith_api/models/organization.py,sha256=BzOVB7ziaUvwmW8387INoJtf90stbPfxkBZ-XYqhKvQ,7918
 cloudsmith_api/models/organization_group_sync.py,sha256=Z-_Ia7wrql-e4T2lJBQVP1KZs0-9XbXQyEMXOqJV8ZM,8391
 cloudsmith_api/models/organization_group_sync_request.py,sha256=KBOHy5g1JAfcqBqvZRPupOF9huDSiJ2e_p3ZS9M0nfc,8223
 cloudsmith_api/models/organization_invite.py,sha256=Az2o6U-T9A-J39v5rDu-IIVHXkMxypHl79A0llK3_CM,10169
 cloudsmith_api/models/organization_invite_extend.py,sha256=cnrSWvGjyFgoOCYxQls0Zv0ExztcXez-XCT8aJ6mhWY,10519
 cloudsmith_api/models/organization_invite_request.py,sha256=xJLQdrXDXsAeTOKsgenEY5HGpqi18xsAAjRXbv2KA8w,5661
 cloudsmith_api/models/organization_invite_update.py,sha256=xnY-FGOU6_nI4ZRJQoYINB9OlTx8pSc07SxnwzaEVHQ,3821
@@ -109,31 +130,38 @@
 cloudsmith_api/models/package_copy_request.py,sha256=WiROah7GuiROyF-AE7I3O1bZojVOaqL8XqgDckQAdjY,4776
 cloudsmith_api/models/package_dependencies.py,sha256=V20LNJxN8_tUTFEBj6ygX4xzwPjtKRePbXOeRmB_C7g,3523
 cloudsmith_api/models/package_dependency.py,sha256=NB7Ok5msL8gr7b_D9YmdPOdO-YAeho4YnoIOpaFJPEE,7227
 cloudsmith_api/models/package_file.py,sha256=VRhis2DJ8H7yWL0V6Mx5WcD87HphFE5BpnEkGdVt06E,12968
 cloudsmith_api/models/package_file_parts_upload.py,sha256=NUgpfiMxAN2qU6k-gxJigd3e4pxP_XfZaJsK1reiriE,6108
 cloudsmith_api/models/package_file_upload.py,sha256=kLsYBDgujzwrcWa1D5mYSLdizqpu7kfoCrHhpp2xSxI,7841
 cloudsmith_api/models/package_file_upload_request.py,sha256=XJAVe2imaUG-kIOtIvP19RO9yktTFM_Nvcb8SmYaSTk,7815
+cloudsmith_api/models/package_license_policy_evaluation_request.py,sha256=2x6i7H0ezbeqAPW7AzqjIuWKzR91ySPQBhSRNXI73ks,9164
+cloudsmith_api/models/package_license_policy_evaluation_request_request.py,sha256=T5CQqwaOXHU0WhyPTrCUdMK2ArVH9wex4pa7UxnL6TQ,2865
 cloudsmith_api/models/package_license_policy_violation_log.py,sha256=LqfpVo013EdCh4gzs5TJCitgo3vEfqpOOFfDnGmktC8,6035
 cloudsmith_api/models/package_license_policy_violation_log_cursor_page.py,sha256=tx7lA-BDmJ4aEvkhb1HDjOp1M0pll_RWK6cPKBYjpIw,5198
 cloudsmith_api/models/package_move.py,sha256=5Rf9FVxaLol6bIG7DZqNSrMasyx2SkoHWDCrTul0KsM,57195
 cloudsmith_api/models/package_move_request.py,sha256=rH-8TsDTwTLPmwOgJcc51yfyeVSqmFDNggKd0LjPciQ,3820
 cloudsmith_api/models/package_quarantine.py,sha256=lnt1g478Z7cMFBRaPlGwPqyZOBU_WCvrwt2ZApoSR6k,58775
 cloudsmith_api/models/package_quarantine_request.py,sha256=JMaDWKZ7DYOGy3lg8vYQLvIDCeMhIu8rDUiBSZ1LdSY,3527
 cloudsmith_api/models/package_resync.py,sha256=2txwMHIR-tb3jFuODLgE9BFmYKSY1i4KLODsGc-4Lvk,57651
 cloudsmith_api/models/package_status.py,sha256=MnQTlZLtSd-cGfgdjyq-QFVsKiwBeO651RKutDAoGok,15877
 cloudsmith_api/models/package_tag.py,sha256=LCUM6nMFNv5EGbfqKWa_QdygV21WO-KxXpEZK7W1CdY,57199
 cloudsmith_api/models/package_tag_request.py,sha256=VTbLpaU8j_MKE7pjZsusCAHFhRHEpyKg3pUCGioAdU8,5352
 cloudsmith_api/models/package_usage_metrics.py,sha256=M7j46JbJloiqe2D4leVEZIaksx5ftwF6OmQNd0WZs5E,3547
 cloudsmith_api/models/package_version_badge.py,sha256=yhpRbr5Mp1Zs6ZLqP0YvF3ihtT8I5-Srzmy0R2_8Ff8,2740
 cloudsmith_api/models/package_vulnerability.py,sha256=7-UFtdgFtceJ5YClNjsCtknJoYu8QlJ3Q3PGjGdC9XA,5707
+cloudsmith_api/models/package_vulnerability_policy_evaluation_request.py,sha256=cEig3IqSa_DmRGOhAG9rShv6vRP3J_fYglwgNSiODKE,9380
+cloudsmith_api/models/package_vulnerability_policy_evaluation_request_request.py,sha256=bH6fStLBTn6IukoBbeUuVp9YSNEkR3CVAVpl9j7-6IY,2895
 cloudsmith_api/models/package_vulnerability_policy_violation_log.py,sha256=kyMrjsBjqZ9ag-he0Rq1Lv_gqfsS1h0F2XwzNbGwK_g,7491
 cloudsmith_api/models/package_vulnerability_policy_violation_log_cursor_page.py,sha256=FZC3S0q3ZrWXGzdifdBbze_CzGkQQ7NRDAmNm9Y0_TU,5318
 cloudsmith_api/models/python_package_upload.py,sha256=iJw8R4hVX64k8m-OGklH4z-YTFTzj7kdTJW2IJf19Nc,58771
 cloudsmith_api/models/python_package_upload_request.py,sha256=QeQVyHNe16XOY39n5OTJTJ-Nte6XyhIAlycR77VKBu4,6194
+cloudsmith_api/models/python_upstream.py,sha256=LOyil4yiCh7zO487UtVd_CPZufBLYOHnzN5eU38hwmA,22418
+cloudsmith_api/models/python_upstream_request.py,sha256=s-M6ty8WO52VqOYRisnB3nZSR_MOTzGiECkjS9tJ_5k,20169
+cloudsmith_api/models/python_upstream_request_patch.py,sha256=5OfEV4CdchHf1tYKMGhjG4AFf9N8q0HfvPhJzVLaTz0,20186
 cloudsmith_api/models/quota.py,sha256=ylCUfeFqiG_jJVYGuYWgN-Hyrx2jsoYPSjiFraD4H6k,3358
 cloudsmith_api/models/quota_history.py,sha256=MbgL9kyGqCmUugExMsdFuoYxT8UWSY6PqtyfrLDB-G0,3463
 cloudsmith_api/models/rate_check.py,sha256=oZn08kE-_pCwt5X2PapC4Mw6-rG_U6u54UnrOQdLV6w,7675
 cloudsmith_api/models/raw_package_upload.py,sha256=o4zSr0dezpZIB4hJFgJxxTT-IJpwa9j0ArMjoRkOars,58899
 cloudsmith_api/models/raw_package_upload_request.py,sha256=ZZnWmMeBiU6RZs_fmzUoe2S9EXSDwJZQgtK3VDIxwHA,11674
 cloudsmith_api/models/repository.py,sha256=w8bfh1EDaJWgHOKiQI4n1pO5TxlbcoXPcXKkd0qIwvg,66229
 cloudsmith_api/models/repository_audit_log.py,sha256=MUOn8hqKio0KTSVvFCfh6eKoOoCzuj7RMiM6hWGWR6Y,14861
@@ -168,21 +196,27 @@
 cloudsmith_api/models/repository_webhook_request.py,sha256=FbkfdGvrZn7yS2PVFpgxgWDnqpfbknuJZfXluVxu9jk,18912
 cloudsmith_api/models/repository_webhook_request_patch.py,sha256=TbujXUmPBjgatch193r4wqhdoofPhWVrkfZh01GvPj8,18774
 cloudsmith_api/models/resources_rate_check.py,sha256=7LlUfH6WkOYY9J1O26LYHbK0jXnXCPyL206-G19VtWs,3523
 cloudsmith_api/models/respository_geo_ip_enable_disable.py,sha256=oSzM7HSHfh7875ZOr9wbap9ciy2zFeooAVd4ceT1-7w,2790
 cloudsmith_api/models/respository_geo_ip_enable_disable_request.py,sha256=h5cWc3qwFHoh5ckaXmbIdDVAyxBu1xWTtC6hr3LxxZ4,2825
 cloudsmith_api/models/rpm_package_upload.py,sha256=EzTFVTqVaif9B17_0HZMz9sB1n-oQcxT0ng23Mbsl4U,57940
 cloudsmith_api/models/rpm_package_upload_request.py,sha256=dI7_B02n2f4DhzcTl_dClukOTFHbuL2ITWwnTEyZrOM,7374
+cloudsmith_api/models/rpm_upstream.py,sha256=kQIMDMPoV39cRhyWMNoMKGLw7aSdw5CP1IAkNvWpQCk,24178
+cloudsmith_api/models/rpm_upstream_request.py,sha256=N5wfq0otlaX5zBXCTpe7gQsUV869VOR1CIa1GEdoyGg,22021
+cloudsmith_api/models/rpm_upstream_request_patch.py,sha256=gQaYRyWDWGiFRtCqXHO8eN_-AX4IGJKA3klsOQEXor8,21938
 cloudsmith_api/models/ruby_package_upload.py,sha256=cLi1WS4JxzNIRkDjUAMtIM_Fx12s_-Th51ysO_t08Bk,58217
 cloudsmith_api/models/ruby_package_upload_request.py,sha256=pA2MIcN9TvnQBQdh-W3VsQRgkB2VkQg4lWuFalrmHmw,6160
+cloudsmith_api/models/ruby_upstream.py,sha256=2cQ3AM2oSCp20N9mHKKpnKCrDG2ZRT_GbVRq2OQ8-Fk,22280
+cloudsmith_api/models/ruby_upstream_request.py,sha256=lbHPwWkjG6yKYjuUXA7rMoHlcjMff5huUUrHrreUO9A,20055
+cloudsmith_api/models/ruby_upstream_request_patch.py,sha256=qm2a_yXYlv9KYfQfpC8NT-TCT7KCbVnExw5dRTnmdwQ,20072
 cloudsmith_api/models/service.py,sha256=lhEXDlJBEf2h_uhqlb0gLo9fPePbEi9Ayo4aC6Zyo6w,8234
 cloudsmith_api/models/service_request.py,sha256=JOv9I8cUiQqTFOBomiwC3KVnewi8x2Rc6NUpp4wg42g,6726
 cloudsmith_api/models/service_request_patch.py,sha256=G3Kyh4R5MA_qsdxaqygbWco5zFqdRmklQGaW0MfAKGQ,6701
 cloudsmith_api/models/service_teams.py,sha256=JVUDlli2nc2oVtCGZQo29lHNQRuRuEsGKei-ShRyYlA,4951
-cloudsmith_api/models/status_basic.py,sha256=1_kzprGvXky9lt0S3d7Ei__Lk0JwR0L5OQxiYeW-kPE,4584
+cloudsmith_api/models/status_basic.py,sha256=0NYtFZR1UWy2NlctpNF0kw9VRSLolgJaTCoTxa6TgXE,4584
 cloudsmith_api/models/storage_allocated_limit.py,sha256=NkE1HLffx1kwuA0GamS5COBvOE3I0CyNa44Ox2vkTcQ,8478
 cloudsmith_api/models/storage_allocated_limit_raw.py,sha256=EZ2PZeIOBGfue8u0HVjurLNClceuFc5wH2UKoBqdtyQ,6140
 cloudsmith_api/models/storage_region.py,sha256=dx_5FJDAJmHrcNI4cBWiZJ6Jr06fFCA5TWYxGob9BTc,4670
 cloudsmith_api/models/storage_usage.py,sha256=EfRE_skvZ85zdc57ZKXwpacL85QGDSrMiYKf2sBQxMQ,6847
 cloudsmith_api/models/storage_usage_raw.py,sha256=fFnveEKU771hbXtZXfCV262Tm3B3RNJH6-4JPC4QFqA,5048
 cloudsmith_api/models/swift_package_upload.py,sha256=p8cHVupHOLYXRqAbsedWsXBrmRMJQffcLFjajXKZpGA,58865
 cloudsmith_api/models/swift_package_upload_request.py,sha256=9lc6XNXvJylOK71lsz9DizrG_dubk8sLMYm2miTU6wU,7279
@@ -200,15 +234,15 @@
 cloudsmith_api/models/user_profile.py,sha256=R7MrOiT5xeTjkw9W2oo0S0Jr15FoyoWts6ACWJHUNrE,11110
 cloudsmith_api/models/vagrant_package_upload.py,sha256=YHZRrw8Fx5owKP2IxNKjyTgGW7G3iziRUrTkQ0xsExc,60899
 cloudsmith_api/models/vagrant_package_upload_request.py,sha256=QCeUkKr6NXB6wAEbFS5prYiv_2BCHyOpHOd0QNM3gTQ,9492
 cloudsmith_api/models/vulnerability.py,sha256=EhiEvjqjau_YWOJQvHUx8ez_iNK0L62OsooXqlYOe6s,13112
 cloudsmith_api/models/vulnerability_scan.py,sha256=l_c1Fi1f5yWuFpkZJ8b9fnoUT24mR-GymVyOXhyStr4,5400
 cloudsmith_api/models/vulnerability_scan_results.py,sha256=ahAY0NoI56ZhZE7a6a5zC81VuwfKXGObU0KVGNo0b74,10348
 cloudsmith_api/models/vulnerability_scan_results_list.py,sha256=pw3m5ew-YNHR26IhiF8xaoaKZskjaySO53zNH_FbvkY,9725
-cloudsmith_api/models/vulnerability_scan_version.py,sha256=iEIDkLWfEL7Xh6wKKm7-DGY2vzbrrJNiMDzSHOKpKwM,8443
+cloudsmith_api/models/vulnerability_scan_version.py,sha256=cjC3fC9l6y3OufeN5PXJHrMM6vFjYnPcnV1ZB0t1Hhk,8445
 cloudsmith_api/models/webhook_template.py,sha256=7gckCqIgyXL1qtzgJ_ShilhjC4OAj0E5dmfS6bt0MEM,4751
 test/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 test/test_allocated_limit.py,sha256=Z9YkpJvxvcybMcK7lhy2w5WWUnB3sqf4g2YiZOZe11g,900
 test/test_allocated_limit_raw.py,sha256=do3JYGvEItmUtaw3jvSXDqtZZPFq4d8aA-FuB6e6jvE,926
 test/test_alpine_package_upload.py,sha256=WsaGcAtKxDgIqI52TuiTekpdFxTKZPUHXg-AgFcoi7A,942
 test/test_alpine_package_upload_request.py,sha256=uHCsktTOkhnw99LhXnMYfqSIapL_CZk5Bue7JBtPUW0,1000
 test/test_architecture.py,sha256=GWlvnskp29WARHM89Iuobu_NH3Ke-F_UtsQcnvwMXps,882
@@ -229,55 +263,76 @@
 test/test_conan_package_upload_request.py,sha256=fV-DtFgkR-CIjcfRaBcMhGAX_HdOWGHhFCIqQ2_ZzTs,992
 test/test_conda_package_upload.py,sha256=fv2j-s5TepKtP9l3gXpiTBdVfhCOsFyVX1LVKN_uvKs,934
 test/test_conda_package_upload_request.py,sha256=NChGXMpvQFWKXalb3yYUk5wHiR2a4id5M5h4t16p_Sk,992
 test/test_cran_package_upload.py,sha256=XLgsD1S5MEutfy4BXO6kOQ4Bsk8pvyScxR6b-C_2YLc,926
 test/test_cran_package_upload_request.py,sha256=B5Vxunnr_S8jb38rGgao5nhNdyoIj7M63z6TY_Ij65I,984
 test/test_dart_package_upload.py,sha256=EyQ4b5lSsSRhelyo673UrJ3MQ60LaC9Cq97vOUV5aIU,926
 test/test_dart_package_upload_request.py,sha256=jaLQQ0PBNCi2d-IsJleK0AreQ7PBWmPrrBBENcTwiwQ,984
+test/test_dart_upstream.py,sha256=O_CaZ4yuOdroPxsnNH7g8m6w3TDMiaJLdk-iYJb2zm4,884
+test/test_dart_upstream_request.py,sha256=dncpzcfS47VIdSGAUOzWrOmWE_3xS0qn2nOmXrJnUdw,942
+test/test_dart_upstream_request_patch.py,sha256=OcZtnsK25SB6w2hDOeSi2jyhrnnXUg_9P0INuv4s2jA,984
 test/test_deb_package_upload.py,sha256=h6--Ja9hEW6M9YEYrbC26-acfFollwQvNX3Cwy4kC3I,918
 test/test_deb_package_upload_request.py,sha256=Izbhf_nd30M4D8GS7MkYlVjUGO6502QQNxuX0XOwj9U,976
+test/test_deb_upstream.py,sha256=kAzooBB93lkNGALlyR6BAQ7O9mFUk_AF8OtH8aeqI7E,876
+test/test_deb_upstream_request.py,sha256=YmiFQGY8oh1z7-MSGpIKzyYI9u33Euy7-YJAaqu9ork,934
+test/test_deb_upstream_request_patch.py,sha256=p1BR2AaprUT1pRV5zucTp8odRBSAytdHKW2DLU_WcRY,976
 test/test_distribution.py,sha256=TBk_9cMHGZbwVblWzbbckovXucarwhKjziGkuyKDjDg,882
 test/test_distribution_full.py,sha256=u8NNJ9x0I7a0aQnjxwzrRKrnpDP63rboH4dAsyHVvzA,916
 test/test_distribution_version.py,sha256=H_ReHZ6uKX802sYpDHZqQ0hwt_2yvl59d01F6PYATvY,940
 test/test_distros_api.py,sha256=qCxTbfid0jBwEKnRwWT-5QS-4OSWvYm96aMsB5jOZS8,1019
 test/test_docker_package_upload.py,sha256=fxYJZ48bwUIanq9cThBhAkDZTPFLPqOtJFacYHrPhJ0,942
 test/test_docker_package_upload_request.py,sha256=RhSFhfh3Pb-Dc3mrlf46AkJrF_JHkNKpLsFnlpjLFJo,1000
+test/test_docker_upstream.py,sha256=ZCdm9pEArijWFdC_zh6G54yzyJSdmEfIOxhdPSJlavY,900
+test/test_docker_upstream_request.py,sha256=jhh7hEmOV38a0LSkozhh5TgYv4SlyNrm9LsuIWf4Udw,958
+test/test_docker_upstream_request_patch.py,sha256=hUmgyR4wYL1NW50moB7mjdWXp2Ur332oYC0CUinTDYQ,1000
 test/test_entitlement_usage_metrics.py,sha256=5tr4tgE_ByGqobpQw_jvLFnBtYKMH6bVbU29j1FPBkk,974
 test/test_entitlements_api.py,sha256=S57P_1gN-t4a5uYn-urYpVBPUCttDcW1wxpltrKE36k,2550
 test/test_error_detail.py,sha256=iLcXZjvPMpcelmLZu8zjvDsVILdO5NrrOI9wcLZ43zY,876
 test/test_eula.py,sha256=QHClUH-uJJxRl3SQo-wjuZ_Bzs_DUtimKWmS8EzYWh0,818
 test/test_files_api.py,sha256=blwlWgReXY_KLmzFzYJpSAzMP7-ph9ykzIPp1VrAAVY,1503
 test/test_format.py,sha256=Pvd-J3GBqOHSPMZVmygOIw13Kfon3FgR94zUGFLqDVM,834
 test/test_format_support.py,sha256=9Pg-T22EECmGmsSxSoLueanDlajn8gk4ZTTkNU58daM,892
 test/test_formats_api.py,sha256=yIEx4POX4lFZ1bUrXWwKzIUuicJhogOLFbzXwPXrbCM,1022
 test/test_geo_ip_location.py,sha256=emR0Gn9O08c3hIq3Z0AHl1I3lrGFDQtD5xEjbEuI5GM,894
 test/test_go_package_upload.py,sha256=-JNWeb4MtT6zYxdaJ4hSnx3_YnSeF1zLUx-Z1rUCSC4,910
 test/test_go_package_upload_request.py,sha256=NkySpOxmeCFPIQaf6mSFxuE6u1-jSAuGc2do4S46I08,968
 test/test_helm_package_upload.py,sha256=10o8yyxk6c5dgU7c-XUAqtFhyB1xjZaAYxmFgXF6g2U,926
 test/test_helm_package_upload_request.py,sha256=nnG38-2Bl3noBV6PGpbmtF5FagtEUasLwd01B8oO9DM,984
+test/test_helm_upstream.py,sha256=Vrlo9HZiKhzstKfuONwtvgq4FetTUAtFKBeoqBi9iKM,884
+test/test_helm_upstream_request.py,sha256=5iBaD0eJoVMOMC6ylHbDc83gLHX7Xey25mK9zxO3axY,942
+test/test_helm_upstream_request_patch.py,sha256=7_wivYsZ9205JfmJ5YKmQhBq2wZ6C-Bpv7dL-Pf22J0,984
 test/test_hex_package_upload.py,sha256=CSrRr2OYKpSoHiJ07iIr_ihsBjljZzY6QoG4nyexyY8,918
 test/test_hex_package_upload_request.py,sha256=5nHxbziLWQR3Iwy34yoboVTjqJsPrrbXWJ-7FmTGMDQ,976
 test/test_history.py,sha256=KcfXovwetcML_pfkqu-mXgjfORWPwk1RaK8YwkdQWsA,842
 test/test_history_fieldset.py,sha256=Bm7FOpV8w9-Whk32HtjzdUtzYZv4DJARQ6DhczdDmn4,908
 test/test_history_fieldset_raw.py,sha256=47wxdjeecweq3QtbNu6SBptW_MLpYI7q1KM2YLjwMks,934
 test/test_luarocks_package_upload.py,sha256=GYj_FvW7CbegzPRB19VjteBuCeLK5S-TVhN5cSnTkFg,958
 test/test_luarocks_package_upload_request.py,sha256=6xLeA8NDCWrRdfLFtOS3ohBNh0xzJ58CUoJvSB-XusU,1016
 test/test_maven_package_upload.py,sha256=5jSiC-GuZ3BSqByMsDRoi9iGbuOdOlkpycLiY_WFITQ,934
 test/test_maven_package_upload_request.py,sha256=2SF-gjJYFmlNinfiCRDCj0AASmwzr2AsbxluOJTpMkA,992
+test/test_maven_upstream.py,sha256=FqpKjGtV3bT9cjfY2k1TldqtnMgOYio1R30h3cZDN_Y,892
+test/test_maven_upstream_request.py,sha256=m1ZKm4DjHB5ToFMtWiYx02LxnYNpcXHcbSgtP5BBoag,950
+test/test_maven_upstream_request_patch.py,sha256=sjLicVQisFQT6YNsU2gdA1gKFeGUvxwfwjBwZ3aFIJA,992
 test/test_metrics_api.py,sha256=crXuZZhSRBWaJ_3jrZ05GSwQhPBpNEAnvQwkX-cjFX8,1335
 test/test_namespace.py,sha256=r3GlqY-TttleCmnpyM7WyrJ1F_QadGhWBmPdcrkGK_E,858
 test/test_namespace_audit_log.py,sha256=ltgG_bIAYUT6UCiRVIOpv3lUt6JRbCNEiOgC9hTOg58,926
 test/test_namespaces_api.py,sha256=ptdTesyF3xWhFm5tcSL2dcLbKvTA7DgNwgRfyK5Q9vU,1051
 test/test_nested_license_policy.py,sha256=C-n4QFeKPfmApUwzED3FkxQrLAQarQ2JH4lIq-i9taQ,942
 test/test_nested_vulnerability_policy.py,sha256=0lXonQei5aKyKfEPyLEnmXeQ06fg9s2c7t3QFnOSCN8,990
 test/test_nested_vulnerability_scan_results.py,sha256=twIYeQF19uD1pK4KjW_flIOSLaKoMR9gRAaYNFSrBX8,1032
 test/test_npm_package_upload.py,sha256=CGaT4uu2xrFDMbp7JetsB3uQmo0NDUiIBLOUvI1PJMk,918
 test/test_npm_package_upload_request.py,sha256=8IuRpjFC9dU6fOYr_SMkZxWLknG9qCxjl-6GPmUAiW8,976
+test/test_npm_upstream.py,sha256=lG-4_U4Ussxj8C63IJSgEs4AJPBv1_ZkASB4uvLwowI,876
+test/test_npm_upstream_request.py,sha256=GVMpzjrX92hmPoSA1rZe06FDyjKTVEdmyn9E83k4XsY,934
+test/test_npm_upstream_request_patch.py,sha256=cbGIO5BvxpLViMeFrHjlAqvT0r8BUYuIH_Uft3N7Plk,976
 test/test_nuget_package_upload.py,sha256=Bk_B3BFm21nP3R3l3uz-l7IwsfX9F3VwqgP3izBybRQ,934
 test/test_nuget_package_upload_request.py,sha256=cZQpVTJ5-tNAp8kpjjaTNqdeQBLf7xjowOsaxOOCIRU,992
+test/test_nuget_upstream.py,sha256=4C24kzRC9RPQSNav43kj0phzh75gSlhWPFfhfuHyngE,892
+test/test_nuget_upstream_request.py,sha256=iopL4vZkD51K8tnWJ7l7bM3KdG1aSFc4ItUjAycUNac,950
+test/test_nuget_upstream_request_patch.py,sha256=r6sIGBk4nfskChI7Ykr0CfR2hd5gG_LcIz1BwnvNjjg,992
 test/test_organization.py,sha256=eREcOoymQehUxcZOAmmDWXJ9qN9G1R-aerZwO-5JVJo,882
 test/test_organization_group_sync.py,sha256=5-NQtopJCdf8MdUgY1seiJoOIK1fRk-4_fBKy_xRf3A,958
 test/test_organization_group_sync_request.py,sha256=8CV8MJv9lNU3DyYtWDLnR7SwxP-qfxPMhqLvUGXOP9Q,1016
 test/test_organization_invite.py,sha256=s2ZxogC6P1ci60k7B1GtGC7YBkKbu7RuXyqEi3Vb_Bg,932
 test/test_organization_invite_extend.py,sha256=QDT6q7fE4jTbQxEcSiWCo6D0p1eG1unzAH2LsyAAnzs,982
 test/test_organization_invite_request.py,sha256=Ixuvzod4-_UWPMJQEA-bUI8acmvlNzz0b5W5MWphnPI,990
 test/test_organization_invite_update.py,sha256=O0CmoZVVF0HKps7DfvFM4ZJ_FmgbIO-9LDAQb4LpyNo,982
@@ -290,52 +345,59 @@
 test/test_organization_package_vulnerability_policy_request.py,sha256=p--_Ps1cJTbDGxlK1_GhLQTFn-g9NkYvk53hKY1Lpvk,1154
 test/test_organization_package_vulnerability_policy_request_patch.py,sha256=tEx5i9iLkznzWqfZVmNaE2ktVVvL4IeAPm2mzBsidXc,1196
 test/test_organization_team.py,sha256=2v-a-O2QGZHyCKwnQjQZWKpobLK2aZsu_RF7F-CHjq8,916
 test/test_organization_team_members.py,sha256=16WGRziNyDblKTBlhuN-YfFUdPunCbMxC9YrfUg8C1Q,974
 test/test_organization_team_membership.py,sha256=670Vtv_P694fq5RuOXDh_2LjIjL2aVGlUpNWFbGjcFk,998
 test/test_organization_team_request.py,sha256=1C36jTrtUkDS_L8boAIALBiDasZkbjml4-1aikC-dik,974
 test/test_organization_team_request_patch.py,sha256=YkTZUinXN-kN1CZdVD-1vW6ePQYxbLdQw_RpShRsbRg,1016
-test/test_orgs_api.py,sha256=oU0CiL42Jzr1l2CrNVNlwopgLCMEAB3givkRIQ03by8,8908
+test/test_orgs_api.py,sha256=N-2BOeyFtWmS7852tfTVsWZGnrVnjjiIutMOH9NCd0A,10220
 test/test_p2_package_upload.py,sha256=aoiFoPo_ShLLp5GwCfICouWaC-3NBkTE0eJ0qfKU9QM,910
 test/test_p2_package_upload_request.py,sha256=KL2bMTridhweBkiuQBMU2R-fi6B6-3-hT0hthD_JxaI,968
 test/test_package.py,sha256=OulQtuNamdW7P2IH8V4-ZQcUEUrReNgVKsBYQ-jFmMs,842
 test/test_package_copy.py,sha256=7-auHuSlNVA4DGNrhbOOm6-F7URvNpcxh34RJ5Ux4wQ,876
 test/test_package_copy_request.py,sha256=wQeTnFexOXdPjNtBJ2Yiz9FTprSfCNhdDBdPfJ6MrGw,934
 test/test_package_dependencies.py,sha256=ouRcYsVryLKrIk7BKQYTQKlDnh06nPUmvxZ7htW4Uk0,940
 test/test_package_dependency.py,sha256=WJIUENn8yrmhTxuHLDPSmkWu6YFPldabbVGW7CQOvX0,924
 test/test_package_file.py,sha256=A-K2ibsMHN4ozvs1JdZq2sQb7AsDqr3epbt5uMJ_tRc,876
 test/test_package_file_parts_upload.py,sha256=BZ2T1wVk51Duk4Pgf-_83CauVnDWKy-FeUbzyHSgi2w,968
 test/test_package_file_upload.py,sha256=PUZhEifW8GiZTkzK4NRyTRErHlNhvnfhTuzIDGD0irs,926
 test/test_package_file_upload_request.py,sha256=F3XinFmLzOR9Spss5VQ73DSVqGax7J6i1fvSXJoha-c,984
+test/test_package_license_policy_evaluation_request.py,sha256=VDiPcJMfq3KcYHeO6J1FvQ3ZiY6AT12sLTNHCoKJVV4,1090
+test/test_package_license_policy_evaluation_request_request.py,sha256=g4fo6RYbdvofg4SJYl4xTsniDaHdvB2X3jXILwK05zw,1148
 test/test_package_license_policy_violation_log.py,sha256=yTsnfWMCqpZmfEnxckU92rfcJ5CvlFE1aTUVzYVti24,1050
 test/test_package_license_policy_violation_log_cursor_page.py,sha256=2iPxBe6NCMEhqs6BqZRUeInrUUi1NHguRVShnzB-kIg,1134
 test/test_package_move.py,sha256=-wzLMgw5zxCPEdO5WTve6qX7YkSlUwq3DUIlukolLi0,876
 test/test_package_move_request.py,sha256=2NnjT9qkQWbsh5LtNoetHeiNiFx5Hvri_ZBZSLCSa9k,934
 test/test_package_quarantine.py,sha256=sb3rngGqkA1jWOnnAflSwNITyOq7IsjZWHOdMA9MUkk,924
 test/test_package_quarantine_request.py,sha256=DPj9Y30Lb6gpWpZptdZKpbbaHS4mHgYtnAwMDFAIn4s,982
 test/test_package_resync.py,sha256=c5B1GBugA9YkeASHf9mwkICAeTw7Qj5g0olVC1XvzkI,892
 test/test_package_status.py,sha256=rkTkhQpbnl9gIPoyRTILzKl5i0gSnQcmp4t8LiykOd4,892
 test/test_package_tag.py,sha256=BkcYyKWhYR0zx_a940tYo5Pm4bguJW6fnpnIboBQBi4,868
 test/test_package_tag_request.py,sha256=HXsOuuK6Tfv6fqZw8r5-PihQTJekhC5_L8kfmyh2F0w,926
 test/test_package_usage_metrics.py,sha256=SA2_RAqLdmvnXrhKq4rFEMb6jJ0uj1sIZO-WjwU9NrE,942
 test/test_package_version_badge.py,sha256=FceEfshIzpn-tZWImTMJWnhpiHObWejQv2syqoOFJ4s,942
 test/test_package_vulnerability.py,sha256=mTIkCXM1qjoanj2t0zdhGxV6TUzo9mhNmUqI1hzMlTs,948
+test/test_package_vulnerability_policy_evaluation_request.py,sha256=z20FeTYYui9SyZ3hDpJlzptN-HBUzTvV2NR6CL9Qwtc,1138
+test/test_package_vulnerability_policy_evaluation_request_request.py,sha256=TowjoE3ms1TyRzcnX33y8WsKbTlleKVcPKI5rjL7UGo,1196
 test/test_package_vulnerability_policy_violation_log.py,sha256=iIrZ6ABnEq_AmAr3jUd9vR_FQh66W1xB7ztdstyFMY4,1098
 test/test_package_vulnerability_policy_violation_log_cursor_page.py,sha256=W5uSYYF6ZzUruutsT4Jj78KOEnNqzN-HZaIzB2IEn2Y,1182
 test/test_packages_api.py,sha256=wPP9ZmJOcM6ABeA-8q4AzyvfMgdeugeF8PhF1rNkXa0,11743
 test/test_python_package_upload.py,sha256=9TqfbGmuNwLq5E3K2DW3jSTsj3NIUlgmQwPLQWcH3YY,942
 test/test_python_package_upload_request.py,sha256=I2Si5Gxo2QZcYiqnG9rJoKD3_uwa58Kj5XUDVS-IUpw,1000
+test/test_python_upstream.py,sha256=oVdp9T7Z7-ISBhyeLwWbaraEZeQHztIXLgOGuXT2T10,900
+test/test_python_upstream_request.py,sha256=AZD_G_rCZbtYESNmiF_QXfvZx89DKL2jmutpJwE4iWg,958
+test/test_python_upstream_request_patch.py,sha256=97oVYm163MI14pR0_nIRpc5RVoRmviU3Z3xrR3gsLeM,1000
 test/test_quota.py,sha256=MBDyrqP8f-c-sfrwseJSKhJr8n-CHk_RdVWKnzXQVeY,826
 test/test_quota_api.py,sha256=9s116ymseG0AEs5GjlYvA6sZQt3TA8314jiigYyHQ8I,1364
 test/test_quota_history.py,sha256=He4i2YAkLW9vikiNV6RkUOQvs5gUqjRUxgHihqriPAw,884
 test/test_rate_check.py,sha256=3chA15laHCwLu0QXKOyTCdiJKJbOzAQOeUTftcsaGCg,860
 test/test_rates_api.py,sha256=eEs-UjEVTAr5b40hueduthNROAGZfwy6pEx2VQaRaHM,862
 test/test_raw_package_upload.py,sha256=IOnVbqK50WyDhWqIWzscOznwL142-YLa8zv-RnAHZzM,918
 test/test_raw_package_upload_request.py,sha256=p6me4NBLN_3QVoZa8EFCiAgr21KwH2aZeJrKge1TmjQ,976
-test/test_repos_api.py,sha256=qfQT2t-Y-rh6IfjXYb-Sh5IMeBubJTqU_ozmxzJDlYI,4407
+test/test_repos_api.py,sha256=NVA7WXrO0tJtEG2r0GFOHxGWhNbNyQQcmxLM8qsH3Yw,16607
 test/test_repository.py,sha256=Khjg77HHFEGxqCWDfPPU-y1Jb1dzDKdGOMm00kmWBt0,866
 test/test_repository_audit_log.py,sha256=9F9aBPgSLwK34UJrdoduvWAjo4IJpm9GPbxJbxyYJn8,934
 test/test_repository_create.py,sha256=LIA13KpeHw57CGXAXDf3-a3qCdVeM_DnG7aGIzAxwNs,916
 test/test_repository_create_request.py,sha256=egKIFHRgD_DBdb9SFbqrSfw9Y1KDiguii_YMXFIaGEY,974
 test/test_repository_geo_ip_cidr.py,sha256=xejx6E_I_DBzag-DFMUn_9X1q5AfT4uToDeXernxNAc,944
 test/test_repository_geo_ip_country_code.py,sha256=ump9BL4aEShFETmaRX5L2K7ECne-mn98-aBR7NpmipI,1002
 test/test_repository_geo_ip_rules.py,sha256=psSkqPoHGXWi54gPNHX8qp3404Q6iK_LYbClWlUpOQo,952
@@ -365,16 +427,22 @@
 test/test_repository_webhook_request.py,sha256=GoFwoKftbPU5ww8tsZwCxxAsbAcylooblPHsVeqtoB4,982
 test/test_repository_webhook_request_patch.py,sha256=T26xKDug4PM3DybormpBPr-6bxAC09_pZvFcSkDvprM,1024
 test/test_resources_rate_check.py,sha256=6sKARN2PzI439zKMj5LwExw1mYii3oWGJ15H1W8smCc,934
 test/test_respository_geo_ip_enable_disable.py,sha256=oKirww-aJ5PVYFwMOI3_RnwNyk0yMRjc97sHqlYCy0U,1026
 test/test_respository_geo_ip_enable_disable_request.py,sha256=DcpIiUwxt_1cwIh7Qu4vypyc7jBziNAc0AbdOUn-PCE,1084
 test/test_rpm_package_upload.py,sha256=oPTf9f7iJZXSMEUnftoUWrQcj5YH7KWLoa6AlKSApy8,918
 test/test_rpm_package_upload_request.py,sha256=BKwOqvJsWd1DVkQXw64hTFXariDx7Uo_w0pi4aDwV-M,976
+test/test_rpm_upstream.py,sha256=_AnbizqZ1f0WRm7km1UBu7FhHV-wdIpLasQwpiFlIVA,876
+test/test_rpm_upstream_request.py,sha256=M0pFr_zwJlu4F3TGW3IdW5xsss0szeWLUjE7Bq-vYa8,934
+test/test_rpm_upstream_request_patch.py,sha256=U0yjXUz7SVDGwbe86INKu2KxjmG2sp0J86Yed0rhAyk,976
 test/test_ruby_package_upload.py,sha256=8qAZf0Z3nwNudKh0vwbvS0fgETivNi1zilPS4S97Ips,926
 test/test_ruby_package_upload_request.py,sha256=M-3rRvlmDDCTKDCZ1F5JakVks4tLxDzZBt9uWK7eams,984
+test/test_ruby_upstream.py,sha256=R4jAt5Z7Ugi2J718f_kI87Db_-5I2SQ06bAcbbfUkHU,884
+test/test_ruby_upstream_request.py,sha256=NDjWw0jSdDhM3t-icp2WwvlV2lAUiINvPcF4DYckhHQ,942
+test/test_ruby_upstream_request_patch.py,sha256=gq9JKfkED9fII7QYvthiDvAYjeeuo-bxixYGlzSRbF8,984
 test/test_service.py,sha256=5iblPOypOwC59YMu85MUON5Xo2_A6C-ZDLtY7H-CPdQ,842
 test/test_service_request.py,sha256=ax3v4nmwXOMukqNVWVS8BVfnpcmsH105c4tw8YeZxyA,900
 test/test_service_request_patch.py,sha256=Hb93XIoaLRDaUF6vKxI4_ZgYPOSFmecMXa96Zio7wFs,942
 test/test_service_teams.py,sha256=gpukM2U7PtF3qbZtbBMyeTvgt6bexCsbpV-UkMSEZYs,884
 test/test_status_api.py,sha256=FQG73VMU1KsBNF9u3wPmBzlbw6AmlN3Sn9uaaAJUMec,864
 test/test_status_basic.py,sha256=PbQ_cv693ykgjTXcdivquHSHITNicdB8fhxIcsmNsM0,876
 test/test_storage_allocated_limit.py,sha256=bWe-Ylveo3nl-qyRFA8QI3Dy_eZviX22ZU0LrGKeQHQ,958
@@ -405,11 +473,11 @@
 test/test_vulnerability.py,sha256=4QDPIFWXKuHg_oy9PTRqFhO8yvsur5VyUFhDVkQ-Dnc,890
 test/test_vulnerability_scan.py,sha256=mGc0AETJ-UP30jb32rN5LvHeP8KFteXB8afWUED2mfI,924
 test/test_vulnerability_scan_results.py,sha256=8-nfCw6UiVWIOsTyge5XETxWxfCkB4hQf4km2lQ3pVI,982
 test/test_vulnerability_scan_results_list.py,sha256=dtcBvhUgGr6LluGnjA6x7dqQ7bkeSbCuPJpKSdHm1kQ,1016
 test/test_vulnerability_scan_version.py,sha256=hgxu72nwZ8rfEgverNQQ9_DF1A-cxa0kIBXPkEEknuk,982
 test/test_webhook_template.py,sha256=kCtiNGZ65WVUpB0an-VxzQ6-F1k-w7kTmHqdgQLSKDU,908
 test/test_webhooks_api.py,sha256=ujU1QfkYPe4MwlMR0M-p2rEfSVTzPO1Q3uB8VLiDbOg,1557
-cloudsmith_api-2.0.6.dist-info/METADATA,sha256=IculCqgjdnNdXHPx9qQsyHD4ZLii6uH1tB5DDOOGAHw,457
-cloudsmith_api-2.0.6.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-cloudsmith_api-2.0.6.dist-info/top_level.txt,sha256=1t-msgoxqMBhQpKKvO2wukE1NWKEk_yDQh9eXqeDNfk,20
-cloudsmith_api-2.0.6.dist-info/RECORD,,
+cloudsmith_api-2.0.7.dist-info/METADATA,sha256=dm2kG1ZBOzZd0KDzpoRJfr5desbhyw3WQRSKvQmW3C4,413
+cloudsmith_api-2.0.7.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+cloudsmith_api-2.0.7.dist-info/top_level.txt,sha256=1t-msgoxqMBhQpKKvO2wukE1NWKEk_yDQh9eXqeDNfk,20
+cloudsmith_api-2.0.7.dist-info/RECORD,,
```

