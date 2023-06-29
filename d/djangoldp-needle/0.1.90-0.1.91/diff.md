# Comparing `tmp/djangoldp_needle-0.1.90.tar.gz` & `tmp/djangoldp_needle-0.1.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/djangoldp_needle-0.1.90.tar", last modified: Fri May  5 14:38:48 2023, max compression
+gzip compressed data, was "dist/djangoldp_needle-0.1.91.tar", last modified: Thu Jun 29 08:19:11 2023, max compression
```

## Comparing `djangoldp_needle-0.1.90.tar` & `djangoldp_needle-0.1.91.tar`

### file list

```diff
@@ -1,203 +1,242 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 14:38:48.000000 djangoldp_needle-0.1.90/
--rw-rw-rw-   0 root         (0) root         (0)      278 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 14:38:48.000000 djangoldp_needle-0.1.90/djangoldp_needle/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 14:38:48.000000 djangoldp_needle-0.1.90/djangoldp_needle/tests/
--rw-rw-rw-   0 root         (0) root         (0)      876 2023-05-05 14:38:27.000000 djangoldp_needle-0.1.90/djangoldp_needle/tests/test_first_annotation_on_user_creation.py
--rw-rw-rw-   0 root         (0) root         (0)     3001 2023-05-05 14:38:27.000000 djangoldp_needle-0.1.90/djangoldp_needle/tests/test_user_contact.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-05 14:38:27.000000 djangoldp_needle-0.1.90/djangoldp_needle/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16392 2023-05-05 14:38:27.000000 djangoldp_needle-0.1.90/djangoldp_needle/tests/test_annotation_target_add.py
--rw-rw-rw-   0 root         (0) root         (0)     5325 2023-05-05 14:38:27.000000 djangoldp_needle-0.1.90/djangoldp_needle/tests/test_booklets_list.py
--rw-rw-rw-   0 root         (0) root         (0)     2196 2023-05-05 14:38:27.000000 djangoldp_needle-0.1.90/djangoldp_needle/tests/test_booklets_quit.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 14:38:48.000000 djangoldp_needle-0.1.90/djangoldp_needle/tests/data/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-05 14:38:27.000000 djangoldp_needle-0.1.90/djangoldp_needle/tests/data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 14:38:48.000000 djangoldp_needle-0.1.90/djangoldp_needle/tests/data/target_url/
--rw-rw-rw-   0 root         (0) root         (0)     4305 2023-05-05 14:38:27.000000 djangoldp_needle-0.1.90/djangoldp_needle/tests/data/target_url/links_with_not_found.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-05 14:38:27.000000 djangoldp_needle-0.1.90/djangoldp_needle/tests/data/target_url/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11721 2023-05-05 14:38:27.000000 djangoldp_needle-0.1.90/djangoldp_needle/tests/data/target_url/links_with_dates.py
--rw-rw-rw-   0 root         (0) root         (0)    15329 2023-05-05 14:38:27.000000 djangoldp_needle-0.1.90/djangoldp_needle/tests/data/target_url/links.py
--rw-rw-rw-   0 root         (0) root         (0)      642 2023-05-05 14:38:27.000000 djangoldp_needle-0.1.90/djangoldp_needle/tests/data/target_url/links_with_timeout.py
--rw-rw-rw-   0 root         (0) root         (0)     1747 2023-05-05 14:38:27.000000 djangoldp_needle-0.1.90/djangoldp_needle/tests/data/target_url/realsites.py
--rw-rw-rw-   0 root         (0) root         (0)    17166 2023-05-05 14:38:27.000000 djangoldp_needle-0.1.90/djangoldp_needle/tests/data/target_url/links_with_redirect.py
--rw-rw-rw-   0 root         (0) root         (0)     4538 2023-05-05 14:38:27.000000 djangoldp_needle-0.1.90/djangoldp_needle/tests/data/target_url/links_with_error.py
--rw-rw-rw-   0 root         (0) root         (0)     4184 2023-05-05 14:38:27.000000 djangoldp_needle-0.1.90/djangoldp_needle/tests/data/target_url/needlerealsites.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 14:38:48.000000 djangoldp_needle-0.1.90/djangoldp_needle/tests/data/parsing/
--rw-rw-rw-   0 root         (0) root         (0)      251 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/tests/data/parsing/base_valid.20221103.html
--rw-rw-rw-   0 root         (0) root         (0)   613961 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/tests/data/parsing/lemonde-1.html
--rw-rw-rw-   0 root         (0) root         (0)   289885 2023-05-05 14:38:27.000000 djangoldp_needle-0.1.90/djangoldp_needle/tests/data/parsing/theconversation-1.html
--rw-rw-rw-   0 root         (0) root         (0)   126155 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/tests/data/parsing/internetactu-1.html
--rw-rw-rw-   0 root         (0) root         (0)   306075 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/tests/data/parsing/lemonde.20221103.html
--rw-rw-rw-   0 root         (0) root         (0)   181484 2023-05-05 14:38:27.000000 djangoldp_needle-0.1.90/djangoldp_needle/tests/data/parsing/theconversation.20221103.html
--rw-rw-rw-   0 root         (0) root         (0)   149029 2023-05-05 14:38:27.000000 djangoldp_needle-0.1.90/djangoldp_needle/tests/data/parsing/reporterre-1.html
--rw-rw-rw-   0 root         (0) root         (0)   127161 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/tests/data/parsing/laviedesidees-1.html
--rw-rw-rw-   0 root         (0) root         (0)   369446 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/tests/data/parsing/latribune-1.html
--rw-rw-rw-   0 root         (0) root         (0)       60 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/tests/data/parsing/base_invalid.20221103.html
--rw-rw-rw-   0 root         (0) root         (0)   232761 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/tests/data/parsing/fredcavazza-1.html
--rw-rw-rw-   0 root         (0) root         (0)   118533 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/tests/data/parsing/blogdumoderateur-1.html
--rw-rw-rw-   0 root         (0) root         (0)     2343 2023-05-05 14:38:27.000000 djangoldp_needle-0.1.90/djangoldp_needle/tests/test_date_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     2470 2023-05-05 14:38:27.000000 djangoldp_needle-0.1.90/djangoldp_needle/tests/test_booklets_add.py
--rw-rw-rw-   0 root         (0) root         (0)    10168 2023-05-05 14:38:27.000000 djangoldp_needle-0.1.90/djangoldp_needle/tests/test_annotation_activity.py
--rw-rw-rw-   0 root         (0) root         (0)     2841 2023-05-05 14:38:27.000000 djangoldp_needle-0.1.90/djangoldp_needle/tests/test_annotation_import.py
--rw-rw-rw-   0 root         (0) root         (0)    10327 2023-05-05 14:38:27.000000 djangoldp_needle-0.1.90/djangoldp_needle/tests/test_annotation_intersection.py
--rw-rw-rw-   0 root         (0) root         (0)     8159 2023-05-05 14:38:27.000000 djangoldp_needle-0.1.90/djangoldp_needle/tests/test_annotation_yarn.py
--rw-rw-rw-   0 root         (0) root         (0)     4198 2023-05-05 14:38:27.000000 djangoldp_needle-0.1.90/djangoldp_needle/tests/test_booklets_invitation.py
--rw-rw-rw-   0 root         (0) root         (0)     2117 2023-05-05 14:38:27.000000 djangoldp_needle-0.1.90/djangoldp_needle/tests/runner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 14:38:48.000000 djangoldp_needle-0.1.90/djangoldp_needle/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 14:38:48.000000 djangoldp_needle-0.1.90/djangoldp_needle/templates/registration/
--rw-rw-rw-   0 root         (0) root         (0)       70 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/templates/registration/activation_email_subject.txt
--rw-rw-rw-   0 root         (0) root         (0)      381 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/templates/registration/password_reset_done.html
--rw-rw-rw-   0 root         (0) root         (0)      213 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/templates/registration/password_change_form.html
--rw-rw-rw-   0 root         (0) root         (0)      215 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/templates/registration/password_reset_email.html
--rw-rw-rw-   0 root         (0) root         (0)      329 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/templates/registration/password_reset_confirm.html
--rw-rw-rw-   0 root         (0) root         (0)      134 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/templates/registration/activation_complete.html
--rw-rw-rw-   0 root         (0) root         (0)      918 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/templates/registration/password_reset_form.html
--rw-rw-rw-   0 root         (0) root         (0)      212 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/templates/registration/registration_form.html
--rw-rw-rw-   0 root         (0) root         (0)      209 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/templates/registration/password_reset_complete.html
--rw-rw-rw-   0 root         (0) root         (0)      235 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/templates/registration/activation_email.txt
--rw-rw-rw-   0 root         (0) root         (0)      753 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/templates/registration/lost_user.html
--rw-rw-rw-   0 root         (0) root         (0)      139 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/templates/registration/password_reset_subject.txt
--rw-rw-rw-   0 root         (0) root         (0)      135 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/templates/registration/activate.html
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-05 14:38:27.000000 djangoldp_needle-0.1.90/djangoldp_needle/templates/registration/password_reset_email.txt
--rw-rw-rw-   0 root         (0) root         (0)      145 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/templates/registration/registration_closed.html
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/templates/registration/logout.html
--rw-rw-rw-   0 root         (0) root         (0)     2949 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/templates/registration/login.html
--rw-rw-rw-   0 root         (0) root         (0)      121 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/templates/registration/password_change_done.html
--rw-rw-rw-   0 root         (0) root         (0)      178 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/templates/registration/registration_complete.html
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-05 14:38:27.000000 djangoldp_needle-0.1.90/djangoldp_needle/templates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      881 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/templates/email.html
--rw-rw-rw-   0 root         (0) root         (0)       88 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/templates/email.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 14:38:48.000000 djangoldp_needle-0.1.90/djangoldp_needle/templates/oidc_provider/
--rw-rw-rw-   0 root         (0) root         (0)     1378 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/templates/oidc_provider/authorize.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 14:38:48.000000 djangoldp_needle-0.1.90/djangoldp_needle/templates/password/
--rw-rw-rw-   0 root         (0) root         (0)      621 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/templates/password/email.html
--rw-rw-rw-   0 root         (0) root         (0)      894 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/templates/base.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 14:38:48.000000 djangoldp_needle-0.1.90/djangoldp_needle/templates/django_registration/
--rw-rw-rw-   0 root         (0) root         (0)      119 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/templates/django_registration/activation_email_subject.txt
--rw-rw-rw-   0 root         (0) root         (0)       42 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/templates/django_registration/registration_base.html
--rw-rw-rw-   0 root         (0) root         (0)      604 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/templates/django_registration/activation_email_body.txt
--rw-rw-rw-   0 root         (0) root         (0)      578 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/templates/django_registration/activation_complete.html
--rw-rw-rw-   0 root         (0) root         (0)      576 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/templates/django_registration/registration_form.html
--rw-rw-rw-   0 root         (0) root         (0)     2376 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/templates/django_registration/authorize.html
--rw-rw-rw-   0 root         (0) root         (0)      264 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/templates/django_registration/registration_closed.html
--rw-rw-rw-   0 root         (0) root         (0)      385 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/templates/django_registration/registration_complete.html
--rw-rw-rw-   0 root         (0) root         (0)      364 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/templates/django_registration/activation_failed.html
--rw-rw-rw-   0 root         (0) root         (0)       33 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/admin.py
--rw-rw-rw-   0 root         (0) root         (0)     2346 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/djangoldp_urls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 14:38:48.000000 djangoldp_needle-0.1.90/djangoldp_needle/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-05 14:38:27.000000 djangoldp_needle-0.1.90/djangoldp_needle/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 14:38:48.000000 djangoldp_needle-0.1.90/djangoldp_needle/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)      402 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/management/commands/importneedledata.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-05 14:38:27.000000 djangoldp_needle-0.1.90/djangoldp_needle/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       23 2023-05-05 14:38:46.000000 djangoldp_needle-0.1.90/djangoldp_needle/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 14:38:48.000000 djangoldp_needle-0.1.90/djangoldp_needle/settings/
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/settings/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      280 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/settings/avatar.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 14:38:48.000000 djangoldp_needle-0.1.90/djangoldp_needle/request_parser/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 14:38:48.000000 djangoldp_needle-0.1.90/djangoldp_needle/request_parser/parsers/
--rw-rw-rw-   0 root         (0) root         (0)      799 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/request_parser/parsers/linkIcon.py
--rw-rw-rw-   0 root         (0) root         (0)     2306 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/request_parser/parsers/opengraph.py
--rw-rw-rw-   0 root         (0) root         (0)     1013 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/request_parser/parsers/urlParser.py
--rw-rw-rw-   0 root         (0) root         (0)      357 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/request_parser/parsers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      185 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/request_parser/parsers/abstract_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     2328 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/request_parser/parsers/metaProp.py
--rw-rw-rw-   0 root         (0) root         (0)     3571 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/request_parser/parsers/itemProp.py
--rw-rw-rw-   0 root         (0) root         (0)      632 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/request_parser/parsers/linkCanonicalProp.py
--rw-rw-rw-   0 root         (0) root         (0)    25244 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/request_parser/parsers/jsonld.py
--rw-rw-rw-   0 root         (0) root         (0)      808 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/request_parser/parsers/lastChanceParser.py
--rw-rw-rw-   0 root         (0) root         (0)      611 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/request_parser/parsers/titleTag.py
--rw-rw-rw-   0 root         (0) root         (0)       42 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/request_parser/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1423 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/request_parser/webdriver_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     6029 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/request_parser/request_parser.py
--rw-rw-rw-   0 root         (0) root         (0)      106 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 14:38:48.000000 djangoldp_needle-0.1.90/djangoldp_needle/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 14:38:48.000000 djangoldp_needle-0.1.90/djangoldp_needle/static/images/
--rw-rw-rw-   0 root         (0) root         (0)   798691 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/static/images/background.png
--rw-rw-rw-   0 root         (0) root         (0)      647 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/static/needle.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 14:38:48.000000 djangoldp_needle-0.1.90/djangoldp_needle/views/
--rw-rw-rw-   0 root         (0) root         (0)    12144 2023-05-05 14:38:27.000000 djangoldp_needle-0.1.90/djangoldp_needle/views/annotation.py
--rw-rw-rw-   0 root         (0) root         (0)      461 2023-05-05 14:38:27.000000 djangoldp_needle-0.1.90/djangoldp_needle/views/user.py
--rw-rw-rw-   0 root         (0) root         (0)      748 2023-05-05 14:38:27.000000 djangoldp_needle-0.1.90/djangoldp_needle/views/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      979 2023-05-05 14:38:27.000000 djangoldp_needle-0.1.90/djangoldp_needle/views/annotation_intersections.py
--rw-rw-rw-   0 root         (0) root         (0)       93 2023-05-05 14:38:27.000000 djangoldp_needle-0.1.90/djangoldp_needle/views/needle_user_profile.py
--rw-rw-rw-   0 root         (0) root         (0)      336 2023-05-05 14:38:27.000000 djangoldp_needle-0.1.90/djangoldp_needle/views/avatars.py
--rw-rw-rw-   0 root         (0) root         (0)      188 2023-05-05 14:38:27.000000 djangoldp_needle-0.1.90/djangoldp_needle/views/needle_activity.py
--rw-rw-rw-   0 root         (0) root         (0)      453 2023-05-05 14:38:27.000000 djangoldp_needle-0.1.90/djangoldp_needle/views/contact_message.py
--rw-rw-rw-   0 root         (0) root         (0)     1499 2023-05-05 14:38:27.000000 djangoldp_needle-0.1.90/djangoldp_needle/views/booklet.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2023-05-05 14:38:27.000000 djangoldp_needle-0.1.90/djangoldp_needle/views/annotation_intersection_read.py
--rw-rw-rw-   0 root         (0) root         (0)    10838 2023-05-05 14:38:27.000000 djangoldp_needle-0.1.90/djangoldp_needle/views/annotation_target.py
--rw-rw-rw-   0 root         (0) root         (0)      507 2023-05-05 14:38:27.000000 djangoldp_needle-0.1.90/djangoldp_needle/views/avatar.py
--rw-rw-rw-   0 root         (0) root         (0)      333 2023-05-05 14:38:27.000000 djangoldp_needle-0.1.90/djangoldp_needle/views/needle_user_follow.py
--rw-rw-rw-   0 root         (0) root         (0)      156 2023-05-05 14:38:27.000000 djangoldp_needle-0.1.90/djangoldp_needle/views/tag.py
--rw-rw-rw-   0 root         (0) root         (0)     1002 2023-05-05 14:38:27.000000 djangoldp_needle-0.1.90/djangoldp_needle/views/booklet_invitation.py
--rw-rw-rw-   0 root         (0) root         (0)      824 2023-05-05 14:38:27.000000 djangoldp_needle-0.1.90/djangoldp_needle/views/booklet_quit.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 14:38:48.000000 djangoldp_needle-0.1.90/djangoldp_needle/permissions/
--rw-rw-rw-   0 root         (0) root         (0)      102 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/permissions/annotation.py
--rw-rw-rw-   0 root         (0) root         (0)      569 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/permissions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/permissions/needle_user_profile.py
--rw-rw-rw-   0 root         (0) root         (0)      106 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/permissions/needle_activity.py
--rw-rw-rw-   0 root         (0) root         (0)      106 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/permissions/contact_message.py
--rw-rw-rw-   0 root         (0) root         (0)      221 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/permissions/_base.py
--rw-rw-rw-   0 root         (0) root         (0)      876 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/permissions/booklet.py
--rw-rw-rw-   0 root         (0) root         (0)      118 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/permissions/annotation_intersection_read.py
--rw-rw-rw-   0 root         (0) root         (0)      108 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/permissions/annotation_target.py
--rw-rw-rw-   0 root         (0) root         (0)       98 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/permissions/avatar.py
--rw-rw-rw-   0 root         (0) root         (0)      108 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/permissions/needle_user_follow.py
--rw-rw-rw-   0 root         (0) root         (0)       95 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/permissions/tag.py
--rw-rw-rw-   0 root         (0) root         (0)      190 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/settings.py
--rw-rw-rw-   0 root         (0) root         (0)      411 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/djangoldp_settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 14:38:48.000000 djangoldp_needle-0.1.90/djangoldp_needle/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      413 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/migrations/0004_annotationtarget_image.py
--rw-rw-rw-   0 root         (0) root         (0)      391 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/migrations/0019_auto_20230208_1213.py
--rw-rw-rw-   0 root         (0) root         (0)      422 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/migrations/0012_needleactivity_activity_type.py
--rwxrwxrwx   0 root         (0) root         (0)      798 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/migrations/0032_avatar2.py
--rw-rw-rw-   0 root         (0) root         (0)     2622 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)     1852 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/migrations/0013_needleuserprofile.py
--rw-rw-rw-   0 root         (0) root         (0)      446 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/migrations/0029_auto_20230411_1211.py
--rw-rw-rw-   0 root         (0) root         (0)      402 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/migrations/0009_activity_subtitle.py
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      682 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/migrations/0015_auto_20230112_1339.py
--rw-rw-rw-   0 root         (0) root         (0)      404 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/migrations/0006_auto_20221101_1846.py
--rw-rw-rw-   0 root         (0) root         (0)     1543 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/migrations/0002_tag.py
--rw-rw-rw-   0 root         (0) root         (0)      465 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/migrations/0018_auto_20230129_1617.py
--rw-rw-rw-   0 root         (0) root         (0)      543 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/migrations/0014_auto_20230105_1238.py
--rw-rw-rw-   0 root         (0) root         (0)      408 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/migrations/0022_annotation_annotation_date.py
--rw-rw-rw-   0 root         (0) root         (0)      584 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/migrations/0007_auto_20221114_1643.py
--rw-rw-rw-   0 root         (0) root         (0)     1992 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/migrations/0023_booklet.py
--rw-rw-rw-   0 root         (0) root         (0)     1854 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/migrations/0011_auto_20221125_1015.py
--rw-rw-rw-   0 root         (0) root         (0)      432 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/migrations/0028_annotationtarget_annotation_target_date.py
--rwxrwxrwx   0 root         (0) root         (0)     2452 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/migrations/0032_avatar.py
--rw-rw-rw-   0 root         (0) root         (0)     1846 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/migrations/0017_annotationintersectionread.py
--rw-rw-rw-   0 root         (0) root         (0)     1970 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/migrations/0025_needleuserfollow.py
--rw-rw-rw-   0 root         (0) root         (0)     1699 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/migrations/0019_contactmessage.py
--rw-rw-rw-   0 root         (0) root         (0)      441 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/migrations/0024_auto_20230328_0814.py
--rw-rw-rw-   0 root         (0) root         (0)      513 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/migrations/0020_contactmessage_creation_date.py
--rw-rw-rw-   0 root         (0) root         (0)      302 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/migrations/0021_merge_20230213_1548.py
--rw-rw-rw-   0 root         (0) root         (0)      519 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/migrations/0027_needleuserfollow_creation_date.py
--rw-rw-rw-   0 root         (0) root         (0)      399 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/migrations/0003_annotation_tags.py
--rw-rw-rw-   0 root         (0) root         (0)      420 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/migrations/0005_annotationtarget_title.py
--rw-rw-rw-   0 root         (0) root         (0)     1635 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/migrations/0008_activity.py
--rw-rw-rw-   0 root         (0) root         (0)      396 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/migrations/0010_activity_read.py
--rw-rw-rw-   0 root         (0) root         (0)      436 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/migrations/0026_auto_20230331_1603.py
--rw-rw-rw-   0 root         (0) root         (0)     1129 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/migrations/0016_auto_20230123_1741.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 14:38:48.000000 djangoldp_needle-0.1.90/djangoldp_needle/models/
--rw-rw-rw-   0 root         (0) root         (0)     2885 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/models/annotation.py
--rw-rw-rw-   0 root         (0) root         (0)     8082 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/models/activity_signal_receiver.py
--rw-rw-rw-   0 root         (0) root         (0)      596 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/models/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      875 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/models/needle_user_profile.py
--rw-rw-rw-   0 root         (0) root         (0)     1216 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/models/needle_activity.py
--rw-rw-rw-   0 root         (0) root         (0)     1702 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/models/contact_message.py
--rw-rw-rw-   0 root         (0) root         (0)     1037 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/models/booklet.py
--rw-rw-rw-   0 root         (0) root         (0)     1185 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/models/annotation_intersection_read.py
--rw-rw-rw-   0 root         (0) root         (0)      830 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/models/annotation_target.py
--rwxrwxrwx   0 root         (0) root         (0)     1511 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/models/avatar.py
--rw-rw-rw-   0 root         (0) root         (0)     1346 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/models/needle_user_follow.py
--rw-rw-rw-   0 root         (0) root         (0)      719 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/djangoldp_needle/models/tag.py
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-05-05 14:38:27.000000 djangoldp_needle-0.1.90/setup.py
--rw-rw-rw-   0 root         (0) root         (0)       66 2023-05-05 14:38:26.000000 djangoldp_needle-0.1.90/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)      608 2023-05-05 14:38:48.000000 djangoldp_needle-0.1.90/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      521 2023-05-05 14:38:48.000000 djangoldp_needle-0.1.90/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 14:38:48.000000 djangoldp_needle-0.1.90/djangoldp_needle.egg-info/
--rw-r--r--   0 root         (0) root         (0)      521 2023-05-05 14:38:48.000000 djangoldp_needle-0.1.90/djangoldp_needle.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 14:38:48.000000 djangoldp_needle-0.1.90/djangoldp_needle.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     8950 2023-05-05 14:38:48.000000 djangoldp_needle-0.1.90/djangoldp_needle.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-05-05 14:38:48.000000 djangoldp_needle-0.1.90/djangoldp_needle.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      142 2023-05-05 14:38:48.000000 djangoldp_needle-0.1.90/djangoldp_needle.egg-info/requires.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 08:19:11.000000 djangoldp_needle-0.1.91/
+-rw-rw-rw-   0 root         (0) root         (0)      278 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 08:19:11.000000 djangoldp_needle-0.1.91/djangoldp_needle/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 08:19:11.000000 djangoldp_needle-0.1.91/djangoldp_needle/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      876 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/tests/test_first_annotation_on_user_creation.py
+-rw-rw-rw-   0 root         (0) root         (0)     3001 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/tests/test_user_contact.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16392 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/tests/test_annotation_target_add.py
+-rw-rw-rw-   0 root         (0) root         (0)     7376 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/tests/test_booklet_contributors_delete.py
+-rw-rw-rw-   0 root         (0) root         (0)     4838 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/tests/test_booklets_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     2363 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/tests/test_booklets_quit.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 08:19:11.000000 djangoldp_needle-0.1.91/djangoldp_needle/tests/data/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/tests/data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 08:19:11.000000 djangoldp_needle-0.1.91/djangoldp_needle/tests/data/target_url/
+-rw-rw-rw-   0 root         (0) root         (0)     4305 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/tests/data/target_url/links_with_not_found.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/tests/data/target_url/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11721 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/tests/data/target_url/links_with_dates.py
+-rw-rw-rw-   0 root         (0) root         (0)    15329 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/tests/data/target_url/links.py
+-rw-rw-rw-   0 root         (0) root         (0)      642 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/tests/data/target_url/links_with_timeout.py
+-rw-rw-rw-   0 root         (0) root         (0)     1747 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/tests/data/target_url/realsites.py
+-rw-rw-rw-   0 root         (0) root         (0)    17166 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/tests/data/target_url/links_with_redirect.py
+-rw-rw-rw-   0 root         (0) root         (0)     4538 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/tests/data/target_url/links_with_error.py
+-rw-rw-rw-   0 root         (0) root         (0)     4184 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/tests/data/target_url/needlerealsites.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 08:19:11.000000 djangoldp_needle-0.1.91/djangoldp_needle/tests/data/parsing/
+-rw-rw-rw-   0 root         (0) root         (0)      251 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/tests/data/parsing/base_valid.20221103.html
+-rw-rw-rw-   0 root         (0) root         (0)   613961 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/tests/data/parsing/lemonde-1.html
+-rw-rw-rw-   0 root         (0) root         (0)   289885 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/tests/data/parsing/theconversation-1.html
+-rw-rw-rw-   0 root         (0) root         (0)   126155 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/tests/data/parsing/internetactu-1.html
+-rw-rw-rw-   0 root         (0) root         (0)   306075 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/tests/data/parsing/lemonde.20221103.html
+-rw-rw-rw-   0 root         (0) root         (0)   181484 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/tests/data/parsing/theconversation.20221103.html
+-rw-rw-rw-   0 root         (0) root         (0)   149029 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/tests/data/parsing/reporterre-1.html
+-rw-rw-rw-   0 root         (0) root         (0)   127161 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/tests/data/parsing/laviedesidees-1.html
+-rw-rw-rw-   0 root         (0) root         (0)   369446 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/tests/data/parsing/latribune-1.html
+-rw-rw-rw-   0 root         (0) root         (0)       60 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/tests/data/parsing/base_invalid.20221103.html
+-rw-rw-rw-   0 root         (0) root         (0)   232761 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/tests/data/parsing/fredcavazza-1.html
+-rw-rw-rw-   0 root         (0) root         (0)   118533 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/tests/data/parsing/blogdumoderateur-1.html
+-rw-rw-rw-   0 root         (0) root         (0)     2343 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/tests/test_date_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     6572 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/tests/test_needle_user_contact.py
+-rw-rw-rw-   0 root         (0) root         (0)     2696 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/tests/test_booklets_add.py
+-rw-rw-rw-   0 root         (0) root         (0)    10168 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/tests/test_annotation_activity.py
+-rw-rw-rw-   0 root         (0) root         (0)    10554 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/tests/test_booklet_contributors_patch.py
+-rw-rw-rw-   0 root         (0) root         (0)     2841 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/tests/test_annotation_import.py
+-rw-rw-rw-   0 root         (0) root         (0)    12210 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/tests/test_booklets_add_annotation.py
+-rw-rw-rw-   0 root         (0) root         (0)    10327 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/tests/test_annotation_intersection.py
+-rw-rw-rw-   0 root         (0) root         (0)     8159 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/tests/test_annotation_yarn.py
+-rw-rw-rw-   0 root         (0) root         (0)     6202 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/tests/test_booklet_contributor_pending.py
+-rw-rw-rw-   0 root         (0) root         (0)     5046 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/tests/test_booklets_invitation.py
+-rw-rw-rw-   0 root         (0) root         (0)     4765 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/tests/test_needle_user_contact_pending.py
+-rw-rw-rw-   0 root         (0) root         (0)     4974 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/tests/test_user_serializer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2584 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/tests/runner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 08:19:11.000000 djangoldp_needle-0.1.91/djangoldp_needle/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 08:19:11.000000 djangoldp_needle-0.1.91/djangoldp_needle/templates/registration/
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/templates/registration/activation_email_subject.txt
+-rw-rw-rw-   0 root         (0) root         (0)      381 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/templates/registration/password_reset_done.html
+-rw-rw-rw-   0 root         (0) root         (0)      213 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/templates/registration/password_change_form.html
+-rw-rw-rw-   0 root         (0) root         (0)      364 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/templates/registration/password_reset_email.html
+-rw-rw-rw-   0 root         (0) root         (0)      776 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/templates/registration/activation_email.html
+-rw-rw-rw-   0 root         (0) root         (0)      329 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/templates/registration/password_reset_confirm.html
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/templates/registration/activation_complete.html
+-rw-rw-rw-   0 root         (0) root         (0)      918 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/templates/registration/password_reset_form.html
+-rw-rw-rw-   0 root         (0) root         (0)      212 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/templates/registration/registration_form.html
+-rw-rw-rw-   0 root         (0) root         (0)      209 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/templates/registration/password_reset_complete.html
+-rw-rw-rw-   0 root         (0) root         (0)      299 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/templates/registration/activation_email.txt
+-rw-rw-rw-   0 root         (0) root         (0)      753 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/templates/registration/lost_user.html
+-rw-rw-rw-   0 root         (0) root         (0)      139 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/templates/registration/password_reset_subject.txt
+-rw-rw-rw-   0 root         (0) root         (0)      135 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/templates/registration/activate.html
+-rw-rw-rw-   0 root         (0) root         (0)      214 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/templates/registration/password_reset_email.txt
+-rw-rw-rw-   0 root         (0) root         (0)      145 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/templates/registration/registration_closed.html
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/templates/registration/logout.html
+-rw-rw-rw-   0 root         (0) root         (0)     2949 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/templates/registration/login.html
+-rw-rw-rw-   0 root         (0) root         (0)      121 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/templates/registration/password_change_done.html
+-rw-rw-rw-   0 root         (0) root         (0)      178 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/templates/registration/registration_complete.html
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/templates/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 08:19:11.000000 djangoldp_needle-0.1.91/djangoldp_needle/templates/emails/
+-rw-rw-rw-   0 root         (0) root         (0)     1040 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/templates/emails/booklet_pending.html
+-rw-rw-rw-   0 root         (0) root         (0)     1074 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/templates/emails/invitation.html
+-rw-rw-rw-   0 root         (0) root         (0)      174 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/templates/emails/invitation.txt
+-rw-rw-rw-   0 root         (0) root         (0)       88 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/templates/emails/contact.txt
+-rw-rw-rw-   0 root         (0) root         (0)      192 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/templates/emails/booklet_pending.txt
+-rw-rw-rw-   0 root         (0) root         (0)      164 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/templates/emails/invitation_pending.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1064 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/templates/emails/invitation_pending.html
+-rw-rw-rw-   0 root         (0) root         (0)      881 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/templates/emails/contact.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 08:19:11.000000 djangoldp_needle-0.1.91/djangoldp_needle/templates/oidc_provider/
+-rw-rw-rw-   0 root         (0) root         (0)     1378 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/templates/oidc_provider/authorize.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 08:19:11.000000 djangoldp_needle-0.1.91/djangoldp_needle/templates/password/
+-rw-rw-rw-   0 root         (0) root         (0)      723 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/templates/password/email.html
+-rw-rw-rw-   0 root         (0) root         (0)     1488 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/templates/base.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 08:19:11.000000 djangoldp_needle-0.1.91/djangoldp_needle/templates/django_registration/
+-rw-rw-rw-   0 root         (0) root         (0)      119 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/templates/django_registration/activation_email_subject.txt
+-rw-rw-rw-   0 root         (0) root         (0)       42 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/templates/django_registration/registration_base.html
+-rw-rw-rw-   0 root         (0) root         (0)      776 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/templates/django_registration/activation_email.html
+-rw-rw-rw-   0 root         (0) root         (0)      665 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/templates/django_registration/activation_email_body.txt
+-rw-rw-rw-   0 root         (0) root         (0)      578 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/templates/django_registration/activation_complete.html
+-rw-rw-rw-   0 root         (0) root         (0)      914 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/templates/django_registration/registration_form.html
+-rw-rw-rw-   0 root         (0) root         (0)     2376 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/templates/django_registration/authorize.html
+-rw-rw-rw-   0 root         (0) root         (0)      264 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/templates/django_registration/registration_closed.html
+-rw-rw-rw-   0 root         (0) root         (0)      385 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/templates/django_registration/registration_complete.html
+-rw-rw-rw-   0 root         (0) root         (0)      364 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/templates/django_registration/activation_failed.html
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)     3098 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/djangoldp_urls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 08:19:11.000000 djangoldp_needle-0.1.91/djangoldp_needle/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 08:19:11.000000 djangoldp_needle-0.1.91/djangoldp_needle/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)      402 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/management/commands/importneedledata.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       23 2023-06-29 08:19:09.000000 djangoldp_needle-0.1.91/djangoldp_needle/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 08:19:11.000000 djangoldp_needle-0.1.91/djangoldp_needle/settings/
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/settings/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      280 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/settings/avatar.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 08:19:11.000000 djangoldp_needle-0.1.91/djangoldp_needle/request_parser/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 08:19:11.000000 djangoldp_needle-0.1.91/djangoldp_needle/request_parser/parsers/
+-rw-rw-rw-   0 root         (0) root         (0)      799 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/request_parser/parsers/linkIcon.py
+-rw-rw-rw-   0 root         (0) root         (0)     2306 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/request_parser/parsers/opengraph.py
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/request_parser/parsers/urlParser.py
+-rw-rw-rw-   0 root         (0) root         (0)      357 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/request_parser/parsers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      185 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/request_parser/parsers/abstract_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     2328 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/request_parser/parsers/metaProp.py
+-rw-rw-rw-   0 root         (0) root         (0)     3571 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/request_parser/parsers/itemProp.py
+-rw-rw-rw-   0 root         (0) root         (0)      632 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/request_parser/parsers/linkCanonicalProp.py
+-rw-rw-rw-   0 root         (0) root         (0)    25244 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/request_parser/parsers/jsonld.py
+-rw-rw-rw-   0 root         (0) root         (0)      808 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/request_parser/parsers/lastChanceParser.py
+-rw-rw-rw-   0 root         (0) root         (0)      611 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/request_parser/parsers/titleTag.py
+-rw-rw-rw-   0 root         (0) root         (0)       42 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/request_parser/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1423 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/request_parser/webdriver_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     6029 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/request_parser/request_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)      106 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 08:19:11.000000 djangoldp_needle-0.1.91/djangoldp_needle/form/
+-rw-rw-rw-   0 root         (0) root         (0)       44 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/form/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      522 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/form/needle_user_form.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 08:19:11.000000 djangoldp_needle-0.1.91/djangoldp_needle/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 08:19:11.000000 djangoldp_needle-0.1.91/djangoldp_needle/static/images/
+-rw-rw-rw-   0 root         (0) root         (0)   798691 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/static/images/background.png
+-rw-rw-rw-   0 root         (0) root         (0)      738 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/static/needle.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 08:19:11.000000 djangoldp_needle-0.1.91/djangoldp_needle/views/
+-rw-rw-rw-   0 root         (0) root         (0)    12144 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/views/annotation.py
+-rw-rw-rw-   0 root         (0) root         (0)     2171 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/views/booklet_contributor.py
+-rw-rw-rw-   0 root         (0) root         (0)     1930 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/views/needle_user_contact_pending.py
+-rw-rw-rw-   0 root         (0) root         (0)     1003 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/views/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2248 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/views/booklet_contributor_pending.py
+-rw-rw-rw-   0 root         (0) root         (0)     1065 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/views/annotation_intersections.py
+-rw-rw-rw-   0 root         (0) root         (0)       93 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/views/needle_user_profile.py
+-rw-rw-rw-   0 root         (0) root         (0)      336 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/views/avatars.py
+-rw-rw-rw-   0 root         (0) root         (0)      188 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/views/needle_activity.py
+-rw-rw-rw-   0 root         (0) root         (0)      453 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/views/contact_message.py
+-rw-rw-rw-   0 root         (0) root         (0)     3187 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/views/needle_user_contact.py
+-rw-rw-rw-   0 root         (0) root         (0)     3590 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/views/booklet.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/views/annotation_intersection_read.py
+-rw-rw-rw-   0 root         (0) root         (0)    10838 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/views/annotation_target.py
+-rw-rw-rw-   0 root         (0) root         (0)      507 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/views/avatar.py
+-rw-rw-rw-   0 root         (0) root         (0)      333 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/views/needle_user_follow.py
+-rw-rw-rw-   0 root         (0) root         (0)      156 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/views/tag.py
+-rw-rw-rw-   0 root         (0) root         (0)     1564 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/views/booklet_invitation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1103 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/views/booklet_quit.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 08:19:11.000000 djangoldp_needle-0.1.91/djangoldp_needle/templatetags/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/templatetags/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      258 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/templatetags/settings_value.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 08:19:11.000000 djangoldp_needle-0.1.91/djangoldp_needle/permissions/
+-rw-rw-rw-   0 root         (0) root         (0)      102 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/permissions/annotation.py
+-rw-rw-rw-   0 root         (0) root         (0)      784 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/permissions/booklet_contributor.py
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/permissions/needle_user_contact_pending.py
+-rw-rw-rw-   0 root         (0) root         (0)      849 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/permissions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      117 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/permissions/booklet_contributor_pending.py
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/permissions/needle_user_profile.py
+-rw-rw-rw-   0 root         (0) root         (0)      106 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/permissions/needle_activity.py
+-rw-rw-rw-   0 root         (0) root         (0)      106 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/permissions/contact_message.py
+-rw-rw-rw-   0 root         (0) root         (0)      221 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/permissions/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/permissions/needle_user_contact.py
+-rw-rw-rw-   0 root         (0) root         (0)     1147 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/permissions/booklet.py
+-rw-rw-rw-   0 root         (0) root         (0)      118 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/permissions/annotation_intersection_read.py
+-rw-rw-rw-   0 root         (0) root         (0)      108 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/permissions/annotation_target.py
+-rw-rw-rw-   0 root         (0) root         (0)       98 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/permissions/avatar.py
+-rw-rw-rw-   0 root         (0) root         (0)      108 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/permissions/needle_user_follow.py
+-rw-rw-rw-   0 root         (0) root         (0)       95 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/permissions/tag.py
+-rw-rw-rw-   0 root         (0) root         (0)      152 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)      473 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/djangoldp_settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 08:19:11.000000 djangoldp_needle-0.1.91/djangoldp_needle/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)      413 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/migrations/0004_annotationtarget_image.py
+-rw-rw-rw-   0 root         (0) root         (0)      391 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/migrations/0019_auto_20230208_1213.py
+-rw-rw-rw-   0 root         (0) root         (0)      422 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/migrations/0012_needleactivity_activity_type.py
+-rwxrwxrwx   0 root         (0) root         (0)      798 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/migrations/0032_avatar2.py
+-rw-rw-rw-   0 root         (0) root         (0)     2622 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)     1852 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/migrations/0013_needleuserprofile.py
+-rw-rw-rw-   0 root         (0) root         (0)      446 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/migrations/0029_auto_20230411_1211.py
+-rwxrwxrwx   0 root         (0) root         (0)      718 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/migrations/0034_auto_20230515_1735.py
+-rw-rw-rw-   0 root         (0) root         (0)      402 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/migrations/0009_activity_subtitle.py
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      682 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/migrations/0015_auto_20230112_1339.py
+-rw-rw-rw-   0 root         (0) root         (0)      404 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/migrations/0006_auto_20221101_1846.py
+-rw-rw-rw-   0 root         (0) root         (0)     1543 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/migrations/0002_tag.py
+-rw-rw-rw-   0 root         (0) root         (0)      465 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/migrations/0018_auto_20230129_1617.py
+-rw-rw-rw-   0 root         (0) root         (0)      543 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/migrations/0014_auto_20230105_1238.py
+-rw-rw-rw-   0 root         (0) root         (0)      408 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/migrations/0022_annotation_annotation_date.py
+-rw-rw-rw-   0 root         (0) root         (0)      584 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/migrations/0007_auto_20221114_1643.py
+-rw-rw-rw-   0 root         (0) root         (0)     1992 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/migrations/0023_booklet.py
+-rwxrwxrwx   0 root         (0) root         (0)     4686 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/migrations/0036_auto_20230526_1301.py
+-rw-rw-rw-   0 root         (0) root         (0)     1854 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/migrations/0011_auto_20221125_1015.py
+-rw-rw-rw-   0 root         (0) root         (0)      432 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/migrations/0028_annotationtarget_annotation_target_date.py
+-rwxrwxrwx   0 root         (0) root         (0)     2452 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/migrations/0032_avatar.py
+-rw-rw-rw-   0 root         (0) root         (0)     1846 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/migrations/0017_annotationintersectionread.py
+-rw-rw-rw-   0 root         (0) root         (0)     1970 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/migrations/0025_needleuserfollow.py
+-rw-rw-rw-   0 root         (0) root         (0)     1699 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/migrations/0019_contactmessage.py
+-rw-rw-rw-   0 root         (0) root         (0)      441 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/migrations/0024_auto_20230328_0814.py
+-rw-rw-rw-   0 root         (0) root         (0)     2302 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/migrations/0035_auto_20230525_1351.py
+-rw-rw-rw-   0 root         (0) root         (0)      513 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/migrations/0020_contactmessage_creation_date.py
+-rw-rw-rw-   0 root         (0) root         (0)      302 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/migrations/0021_merge_20230213_1548.py
+-rw-rw-rw-   0 root         (0) root         (0)      519 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/migrations/0027_needleuserfollow_creation_date.py
+-rw-rw-rw-   0 root         (0) root         (0)      399 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/migrations/0003_annotation_tags.py
+-rw-rw-rw-   0 root         (0) root         (0)      420 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/migrations/0005_annotationtarget_title.py
+-rw-rw-rw-   0 root         (0) root         (0)     1635 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/migrations/0008_activity.py
+-rw-rw-rw-   0 root         (0) root         (0)     2082 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/migrations/0037_auto_20230604_1525.py
+-rw-rw-rw-   0 root         (0) root         (0)      396 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/migrations/0010_activity_read.py
+-rwxrwxrwx   0 root         (0) root         (0)     2784 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/migrations/0033_auto_20230509_1434.py
+-rw-rw-rw-   0 root         (0) root         (0)      436 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/migrations/0026_auto_20230331_1603.py
+-rw-rw-rw-   0 root         (0) root         (0)     1129 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/migrations/0016_auto_20230123_1741.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 08:19:11.000000 djangoldp_needle-0.1.91/djangoldp_needle/models/
+-rw-rw-rw-   0 root         (0) root         (0)     2815 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/models/ldp_user.py
+-rw-rw-rw-   0 root         (0) root         (0)     2885 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/models/annotation.py
+-rw-rw-rw-   0 root         (0) root         (0)     8082 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/models/activity_signal_receiver.py
+-rw-rw-rw-   0 root         (0) root         (0)     1507 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/models/booklet_contributor.py
+-rw-rw-rw-   0 root         (0) root         (0)     2544 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/models/needle_user_contact_pending.py
+-rw-rw-rw-   0 root         (0) root         (0)      870 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2149 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/models/booklet_contributor_pending.py
+-rwxrwxrwx   0 root         (0) root         (0)      875 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/models/needle_user_profile.py
+-rw-rw-rw-   0 root         (0) root         (0)     1216 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/models/needle_activity.py
+-rw-rw-rw-   0 root         (0) root         (0)     1720 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/models/contact_message.py
+-rw-rw-rw-   0 root         (0) root         (0)     2046 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/models/needle_user_contact.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/models/booklet.py
+-rw-rw-rw-   0 root         (0) root         (0)     1203 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/models/annotation_intersection_read.py
+-rw-rw-rw-   0 root         (0) root         (0)      830 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/models/annotation_target.py
+-rwxrwxrwx   0 root         (0) root         (0)     1644 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/models/avatar.py
+-rw-rw-rw-   0 root         (0) root         (0)     1356 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/models/needle_user_follow.py
+-rw-rw-rw-   0 root         (0) root         (0)      719 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/djangoldp_needle/models/tag.py
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)       66 2023-06-29 08:18:44.000000 djangoldp_needle-0.1.91/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)      608 2023-06-29 08:19:11.000000 djangoldp_needle-0.1.91/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      521 2023-06-29 08:19:11.000000 djangoldp_needle-0.1.91/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 08:19:11.000000 djangoldp_needle-0.1.91/djangoldp_needle.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      521 2023-06-29 08:19:11.000000 djangoldp_needle-0.1.91/djangoldp_needle.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 08:19:11.000000 djangoldp_needle-0.1.91/djangoldp_needle.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)    10884 2023-06-29 08:19:11.000000 djangoldp_needle-0.1.91/djangoldp_needle.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-06-29 08:19:11.000000 djangoldp_needle-0.1.91/djangoldp_needle.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      142 2023-06-29 08:19:11.000000 djangoldp_needle-0.1.91/djangoldp_needle.egg-info/requires.txt
```

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/tests/test_first_annotation_on_user_creation.py` & `djangoldp_needle-0.1.91/djangoldp_needle/tests/test_first_annotation_on_user_creation.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/tests/test_user_contact.py` & `djangoldp_needle-0.1.91/djangoldp_needle/tests/test_user_contact.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/tests/test_annotation_target_add.py` & `djangoldp_needle-0.1.91/djangoldp_needle/tests/test_annotation_target_add.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/tests/test_booklets_list.py` & `djangoldp_needle-0.1.91/djangoldp_needle/tests/test_booklets_list.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,155 +1,136 @@
-import requests_mock
 from django.db import transaction
 from djangoldp_account.models import LDPUser
 from rest_framework.test import APITestCase, APIClient, APITransactionTestCase
-import json
-import datetime
-from pkg_resources import resource_string
 
-from ..models import Booklet, Annotation
-
-from .data.target_url.realsites import real_sites
-
-from .data.target_url.needlerealsites import needle_real_sites
+from ..models import Booklet, BookletContributor
 
 
 class TestBookletList(APITestCase):
 
     def setUp(self):
         self.client = APIClient()
 
     def buildUser(self, username):
         user = LDPUser(email=username + '@test.startinblox.com', first_name='Test', last_name='Mactest',
                        username=username,
                        password='glass onion')
         user.save()
         return user
 
-    def test_booklet_list_as_owner(self):
-        user1 = self.buildUser('user1')
-        user2 = self.buildUser('user2')
-        self.store_booklet([user1], [user2])
-        self.client.force_authenticate(user1)
+    def test_booklet_list_public_anonymous(self):
+        self.store_booklet(public=True)
 
         response = self.client.get(
             "/booklets/",
             content_type='application/ld+json',
         )
         response_value = response.json()
         self.assertEqual(response.status_code, 200)
         self.assertEqual(len(response_value['ldp:contains']), 1)
 
-    def test_booklet_list_as_contributor(self):
-        user1 = self.buildUser('user1')
-        user2 = self.buildUser('user2')
-        self.store_booklet([user2], [user1])
-        self.client.force_authenticate(user1)
-
-        response = self.client.get(
-            "/booklets/",
-            content_type='application/ld+json',
-        )
-        response_value = response.json()
-        self.assertEqual(response.status_code, 200)
-        self.assertEqual(len(response_value['ldp:contains']), 1)
+    def test_booklet_list_public_user_contributor(self):
+        for role in BookletContributor.ROLE_CHOICES:
+            with transaction.atomic():
+                sid = transaction.savepoint()
+
+                user1 = self.buildUser('user1')
+                booklet = self.store_booklet(public=True)
+                self.store_booklet_contributor(booklet, user1, role[0])
+
+                self.client.force_authenticate(user1)
+                response = self.client.get(
+                    "/booklets/",
+                    content_type='application/ld+json',
+                )
+                response_value = response.json()
+                self.assertEqual(response.status_code, 200)
+                self.assertEqual(len(response_value['ldp:contains']), 1)
 
+                transaction.savepoint_rollback(sid)
 
-    def test_booklet_list_hide_as_non_owner(self):
+    def test_booklet_list_public_user_not_contributor(self):
         user1 = self.buildUser('user1')
-        user2 = self.buildUser('user2')
-        self.store_booklet([user2], [])
-        self.client.force_authenticate(user1)
+        self.store_booklet(public=True)
 
-        response = self.client.get(
-            "/booklets/",
-            content_type='application/ld+json',
-        )
-        response_value = response.json()
-        self.assertEqual(response.status_code, 200)
-        self.assertEqual(len(response_value['ldp:contains']), 0)
-
-    def test_booklet_list_hide_as_non_contributor(self):
-        user1 = self.buildUser('user1')
-        user2 = self.buildUser('user2')
-        self.store_booklet([], [user2])
         self.client.force_authenticate(user1)
-
-        response = self.client.get(
-            "/booklets/",
-            content_type='application/ld+json',
-        )
-        response_value = response.json()
-        self.assertEqual(response.status_code, 200)
-        self.assertEqual(len(response_value['ldp:contains']), 0)
-
-    def test_booklet_list_hide_non_public_for_anonymous(self):
-        user1 = self.buildUser('user1')
-        self.store_booklet([user1], [])
-
-        response = self.client.get(
-            "/booklets/",
-            content_type='application/ld+json',
-        )
-        response_value = response.json()
-        self.assertEqual(response.status_code, 200)
-        self.assertEqual(len(response_value['ldp:contains']), 0)
-
-    def test_booklet_list_show_public_for_anonymous(self):
-        user1 = self.buildUser('user1')
-        self.store_booklet([user1], [], public=True)
-
         response = self.client.get(
             "/booklets/",
             content_type='application/ld+json',
         )
         response_value = response.json()
         self.assertEqual(response.status_code, 200)
         self.assertEqual(len(response_value['ldp:contains']), 1)
 
-    def test_booklet_list_show_collaboration_allowed_no_annotation(self):
-        user1 = self.buildUser('user1')
-        user2 = self.buildUser('user2')
-        self.store_booklet([user1], [], collaboration=True)
+    def test_booklet_list_private_anonymous(self):
+        self.store_booklet(public=False)
 
-        self.client.force_authenticate(user2)
         response = self.client.get(
             "/booklets/",
             content_type='application/ld+json',
         )
         response_value = response.json()
         self.assertEqual(response.status_code, 200)
         self.assertEqual(len(response_value['ldp:contains']), 0)
 
-    def test_booklet_list_show_collaboration_allowed_annotation_added(self):
-        user1 = self.buildUser('user1')
-        user2 = self.buildUser('user2')
-        annotation = Annotation(creator=user2)
-        annotation.save()
-
-        booklet = self.store_booklet([user1], [], collaboration=True)
-        booklet.annotations.add(annotation)
+    def test_booklet_list_private_not_contributor(self):
+        for role in BookletContributor.ROLE_CHOICES:
+            with transaction.atomic():
+                sid = transaction.savepoint()
+
+                user1 = self.buildUser('user1')
+                user2 = self.buildUser('user2')
+                booklet = self.store_booklet(public=False)
+                self.store_booklet_contributor(booklet, user2, role[0])
+
+                self.client.force_authenticate(user1)
+                response = self.client.get(
+                    "/booklets/",
+                    content_type='application/ld+json',
+                )
+                response_value = response.json()
+                self.assertEqual(response.status_code, 200)
+                self.assertEqual(len(response_value['ldp:contains']), 0)
+
+                transaction.savepoint_rollback(sid)
+
+    def test_booklet_list_private_contributor(self):
+        for role in BookletContributor.ROLE_CHOICES:
+            with transaction.atomic():
+                sid = transaction.savepoint()
+
+                user1 = self.buildUser('user1')
+                booklet = self.store_booklet(public=False)
+                self.store_booklet_contributor(booklet, user1, role[0])
+
+                self.client.force_authenticate(user1)
+                response = self.client.get(
+                    "/booklets/",
+                    content_type='application/ld+json',
+                )
+                response_value = response.json()
+                self.assertEqual(response.status_code, 200)
+                self.assertEqual(len(response_value['ldp:contains']), 1)
 
-        self.client.force_authenticate(user2)
-        response = self.client.get(
-            "/booklets/",
-            content_type='application/ld+json',
-        )
-        response_value = response.json()
-        self.assertEqual(response.status_code, 200)
-        self.assertEqual(len(response_value['ldp:contains']), 1)
+                transaction.savepoint_rollback(sid)
 
-    def store_booklet(self, owners, contributors, public = False, collaboration = False):
+    def store_booklet(self, public = False, collaboration = False):
         booklet = Booklet(
             title="title",
             abstract="",
             accessibility_public=public,
             collaboration_allowed=collaboration,
             cover=1,
         )
         booklet.save()
-        for owner in owners:
-            booklet.owners.add(owner)
-        for contributor in contributors:
-            booklet.contributors.add(contributor)
 
         return booklet
+
+    def store_booklet_contributor(self, booklet, user, role):
+        contributor = BookletContributor(
+            booklet=booklet,
+            user=user,
+            role=role
+        )
+        contributor.save()
+
+        return contributor
```

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/tests/test_booklets_quit.py` & `djangoldp_needle-0.1.91/djangoldp_needle/tests/test_booklets_add.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,71 +2,65 @@
 from django.db import transaction
 from djangoldp_account.models import LDPUser
 from rest_framework.test import APITestCase, APIClient, APITransactionTestCase
 import json
 import datetime
 from pkg_resources import resource_string
 
-from ..models import Booklet
+from ..models import Booklet, BookletContributor
 
 from .data.target_url.realsites import real_sites
 
 from .data.target_url.needlerealsites import needle_real_sites
 
 
-class TestBookletList(APITestCase):
+class TestBookletAdd(APITestCase):
 
     def setUp(self):
         self.client = APIClient()
 
     def buildUser(self, username):
         user = LDPUser(email=username + '@test.startinblox.com', first_name='Test', last_name='Mactest',
                        username=username,
                        password='glass onion')
         user.save()
         return user
 
-    def test_booklet_quit_as_contributor(self):
+    def test_booklet_create(self):
         user1 = self.buildUser('user1')
-        user2 = self.buildUser('user2')
-        booklet = self.store_booklet([user1], [user2])
-        self.client.force_authenticate(user2)
-
-        response = self.client.post(
-            "/booklets/" + str(booklet.pk) + "/quit/",
-            content_type='application/ld+json',
-        )
-
-        self.assertEqual(response.status_code, 200)
-        self.assertEqual(booklet.contributors.count(), 0)
-
-    def test_booklet_quit_as_not_contributor(self):
-        user1 = self.buildUser('user1')
-        user2 = self.buildUser('user2')
-        booklet = self.store_booklet([user1], [user2])
         self.client.force_authenticate(user1)
 
         response = self.client.post(
-            "/booklets/" + str(booklet.pk) + "/quit/",
+            "/booklets/",
             content_type='application/ld+json',
+            data=self._create_booklet('test')
         )
+        self.assertEqual(response.status_code, 201)
+        self.assertEqual(1, Booklet.objects.count())
 
-        self.assertEqual(response.status_code, 404)
-        self.assertEqual(booklet.contributors.count(), 1)
-
-
-
-    def store_booklet(self, owners, contributors):
-        booklet = Booklet(
-            title="title",
-            abstract="",
-            accessibility_public=False,
-            collaboration_allowed=False,
-            cover=1,
-        )
-        booklet.save()
-        for owner in owners:
-            booklet.owners.add(owner)
-        for contributor in contributors:
-            booklet.contributors.add(contributor)
+        booklet = Booklet.objects.first()
+        self.assertEqual(1, booklet.contributors.count())
 
-        return booklet
+        contributor = booklet.contributors.first()
+        self.assertEqual(BookletContributor.ROLE_OWNER, contributor.role)
+        self.assertEqual(user1, contributor.user)
+
+
+    def _create_booklet(self, title):
+        return json.dumps({
+            "@context": {"@vocab": "http://happy-dev.fr/owl/#",
+                         "rdf": "http://www.w3.org/1999/02/22-rdf-syntax-ns#",
+                         "rdfs": "http://www.w3.org/2000/01/rdf-schema#", "ldp": "http://www.w3.org/ns/ldp#",
+                         "foaf": "http://xmlns.com/foaf/0.1/", "name": "rdfs:label",
+                         "acl": "http://www.w3.org/ns/auth/acl#", "permissions": "acl:accessControl",
+                         "mode": "acl:mode", "geo": "http://www.w3.org/2003/01/geo/wgs84_pos#", "lat": "geo:lat",
+                         "lng": "geo:long", "entrepreneurProfile": "http://happy-dev.fr/owl/#entrepreneur_profile",
+                         "mentorProfile": "http://happy-dev.fr/owl/#mentor_profile", "account": "hd:account",
+                         "messageSet": "http://happy-dev.fr/owl/#message_set",
+                         "author": "http://happy-dev.fr/owl/#author_user",
+                         "title": "http://happy-dev.fr/owl/#title"},
+            "title": title,
+            "abstract": "",
+            "accessibility_public": False,
+            "collaboration_allowed": False,
+            "cover": 1
+        })
```

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/tests/data/target_url/links_with_not_found.py` & `djangoldp_needle-0.1.91/djangoldp_needle/tests/data/target_url/links_with_not_found.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/tests/data/target_url/links_with_dates.py` & `djangoldp_needle-0.1.91/djangoldp_needle/tests/data/target_url/links_with_dates.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/tests/data/target_url/links.py` & `djangoldp_needle-0.1.91/djangoldp_needle/tests/data/target_url/links.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/tests/data/target_url/links_with_timeout.py` & `djangoldp_needle-0.1.91/djangoldp_needle/tests/data/target_url/links_with_timeout.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/tests/data/target_url/realsites.py` & `djangoldp_needle-0.1.91/djangoldp_needle/tests/data/target_url/realsites.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/tests/data/target_url/links_with_redirect.py` & `djangoldp_needle-0.1.91/djangoldp_needle/tests/data/target_url/links_with_redirect.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/tests/data/target_url/links_with_error.py` & `djangoldp_needle-0.1.91/djangoldp_needle/tests/data/target_url/links_with_error.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/tests/data/target_url/needlerealsites.py` & `djangoldp_needle-0.1.91/djangoldp_needle/tests/data/target_url/needlerealsites.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/tests/data/parsing/lemonde-1.html` & `djangoldp_needle-0.1.91/djangoldp_needle/tests/data/parsing/lemonde-1.html`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/tests/data/parsing/theconversation-1.html` & `djangoldp_needle-0.1.91/djangoldp_needle/tests/data/parsing/theconversation-1.html`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/tests/data/parsing/internetactu-1.html` & `djangoldp_needle-0.1.91/djangoldp_needle/tests/data/parsing/internetactu-1.html`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/tests/data/parsing/lemonde.20221103.html` & `djangoldp_needle-0.1.91/djangoldp_needle/tests/data/parsing/lemonde.20221103.html`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/tests/data/parsing/theconversation.20221103.html` & `djangoldp_needle-0.1.91/djangoldp_needle/tests/data/parsing/theconversation.20221103.html`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/tests/data/parsing/reporterre-1.html` & `djangoldp_needle-0.1.91/djangoldp_needle/tests/data/parsing/reporterre-1.html`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/tests/data/parsing/laviedesidees-1.html` & `djangoldp_needle-0.1.91/djangoldp_needle/tests/data/parsing/laviedesidees-1.html`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/tests/data/parsing/latribune-1.html` & `djangoldp_needle-0.1.91/djangoldp_needle/tests/data/parsing/latribune-1.html`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/tests/data/parsing/fredcavazza-1.html` & `djangoldp_needle-0.1.91/djangoldp_needle/tests/data/parsing/fredcavazza-1.html`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/tests/data/parsing/blogdumoderateur-1.html` & `djangoldp_needle-0.1.91/djangoldp_needle/tests/data/parsing/blogdumoderateur-1.html`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/tests/test_date_parser.py` & `djangoldp_needle-0.1.91/djangoldp_needle/tests/test_date_parser.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/tests/test_annotation_activity.py` & `djangoldp_needle-0.1.91/djangoldp_needle/tests/test_annotation_activity.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/tests/test_annotation_import.py` & `djangoldp_needle-0.1.91/djangoldp_needle/tests/test_annotation_import.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/tests/test_annotation_intersection.py` & `djangoldp_needle-0.1.91/djangoldp_needle/tests/test_annotation_intersection.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/tests/test_annotation_yarn.py` & `djangoldp_needle-0.1.91/djangoldp_needle/tests/test_annotation_yarn.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/tests/test_booklets_invitation.py` & `djangoldp_needle-0.1.91/djangoldp_needle/tests/test_booklets_invitation.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from django.db import transaction
 from djangoldp_account.models import LDPUser
 from rest_framework.test import APITestCase, APIClient, APITransactionTestCase
 import json
 import datetime
 from pkg_resources import resource_string
 
-from ..models import Booklet
+from ..models import Booklet, BookletContributor
 
 from .data.target_url.realsites import real_sites
 
 from .data.target_url.needlerealsites import needle_real_sites
 
 
 class TestBookletInvitation(APITestCase):
@@ -24,54 +24,58 @@
                        password='glass onion')
         user.save()
         return user
 
     def test_invitation_email_exist(self):
         user1 = self.buildUser('user1')
         user2 = self.buildUser('user2')
-        booklet = self.store_booklet([user1], [])
+        booklet = self.store_booklet()
+        self.store_booklet_contributor(booklet, user1, BookletContributor.ROLE_OWNER)
 
         self.client.force_authenticate(user1)
         response = self.client.post(
             "/booklets/" + str(booklet.pk) + "/invitation/",
             content_type='application/ld+json',
             data=self._create_invitation_request('user2@test.startinblox.com')
         )
         self.assertEqual(response.status_code, 201)
-        self.assertEqual(1, len(booklet.contributors.all()))
-        self.assertEqual(user2, booklet.contributors.all()[0])
+        self.assertEqual(2, len(booklet.contributors.all()))
+        self.assertEqual(user2, booklet.contributors.all()[1].user)
 
     def test_invitation_email_not_exist(self):
         user1 = self.buildUser('user1')
         user2 = self.buildUser('user2')
-        booklet = self.store_booklet([user1], [])
+        booklet = self.store_booklet()
+        self.store_booklet_contributor(booklet, user1, BookletContributor.ROLE_OWNER)
 
         self.client.force_authenticate(user1)
         response = self.client.post(
             "/booklets/" + str(booklet.pk) + "/invitation/",
             content_type='application/ld+json',
             data=self._create_invitation_request('invalid@test.startinblox.com')
         )
         self.assertEqual(response.status_code, 400)
-        self.assertEqual(0, len(booklet.contributors.all()))
+        self.assertEqual(1, len(booklet.contributors.all()))
 
     def test_invitation_user_not_owner(self):
         user1 = self.buildUser('user1')
         user2 = self.buildUser('user2')
         user3 = self.buildUser('user3')
-        booklet = self.store_booklet([user1], [])
+        booklet = self.store_booklet()
+        self.store_booklet_contributor(booklet, user1, BookletContributor.ROLE_OWNER)
+        self.store_booklet_contributor(booklet, user2, BookletContributor.ROLE_VISIT)
 
         self.client.force_authenticate(user2)
         response = self.client.post(
             "/booklets/" + str(booklet.pk) + "/invitation/",
             content_type='application/ld+json',
             data=self._create_invitation_request('user3@test.startinblox.com')
         )
         self.assertEqual(response.status_code, 404)
-        self.assertEqual(0, len(booklet.contributors.all()))
+        self.assertEqual(2, len(booklet.contributors.all()))
 
 
     def store_booklet(self, owners, contributors, public = False, collaboration = False):
         booklet = Booklet(
             title="title",
             abstract="",
             accessibility_public=public,
@@ -96,8 +100,30 @@
                          "mode": "acl:mode", "geo": "http://www.w3.org/2003/01/geo/wgs84_pos#", "lat": "geo:lat",
                          "lng": "geo:long", "entrepreneurProfile": "http://happy-dev.fr/owl/#entrepreneur_profile",
                          "mentorProfile": "http://happy-dev.fr/owl/#mentor_profile", "account": "hd:account",
                          "messageSet": "http://happy-dev.fr/owl/#message_set",
                          "author": "http://happy-dev.fr/owl/#author_user",
                          "title": "http://happy-dev.fr/owl/#title"},
             "email": email
-        })
+        })
+
+    def store_booklet(self):
+        booklet = Booklet(
+            title="title",
+            abstract="",
+            accessibility_public=False,
+            collaboration_allowed=False,
+            cover=1,
+        )
+        booklet.save()
+
+        return booklet
+
+    def store_booklet_contributor(self, booklet, user, role):
+        contributor = BookletContributor(
+            booklet=booklet,
+            user=user,
+            role=role
+        )
+        contributor.save()
+
+        return contributor
```

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/tests/runner.py` & `djangoldp_needle-0.1.91/djangoldp_needle/tests/runner.py`

 * *Files 23% similar despite different names*

```diff
@@ -19,14 +19,15 @@
         'REST_FRAMEWORK': {
             'DEFAULT_PAGINATION_CLASS': 'djangoldp.pagination.LDPPagination',
             'PAGE_SIZE': 5
         },
         # map the config of the core settings (avoid asserts to fail)
         'SITE_URL': 'http://happy-dev.fr',
         'BASE_URL': 'http://happy-dev.fr',
+        'INSTANCE_DEFAULT_CLIENT': 'http://front',
 
         'NEEDLE_AVATARS': {
             'chenille': {
                 'name': 'Chenille',
                 'image': 'https://unpkg.com/@startinblox/component-needle/src/img/animals/chenille.png',
                 'selectable': False,
                 'level': 1
@@ -53,15 +54,22 @@
     'djangoldp_needle.tests.test_first_annotation_on_user_creation',
     'djangoldp_needle.tests.test_annotation_target_add',
     'djangoldp_needle.tests.test_annotation_yarn',
     'djangoldp_needle.tests.test_annotation_activity',
     'djangoldp_needle.tests.test_date_parser',
     'djangoldp_needle.tests.test_annotation_intersection',
     'djangoldp_needle.tests.test_user_contact',
+    'djangoldp_needle.tests.test_booklet_contributor_pending',
+    'djangoldp_needle.tests.test_booklet_contributors_patch',
+    'djangoldp_needle.tests.test_booklet_contributors_delete',
     'djangoldp_needle.tests.test_booklets_add',
     'djangoldp_needle.tests.test_booklets_list',
+    'djangoldp_needle.tests.test_booklets_add_annotation',
     'djangoldp_needle.tests.test_booklets_quit',
     'djangoldp_needle.tests.test_booklets_invitation',
+    'djangoldp_needle.tests.test_needle_user_contact',
+    'djangoldp_needle.tests.test_needle_user_contact_pending',
+    'djangoldp_needle.tests.test_user_serializer',
 ])
 if failures:
     sys.exit(failures)
```

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/templates/registration/password_reset_form.html` & `djangoldp_needle-0.1.91/djangoldp_needle/templates/registration/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/templates/registration/lost_user.html` & `djangoldp_needle-0.1.91/djangoldp_needle/templates/registration/lost_user.html`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/templates/registration/login.html` & `djangoldp_needle-0.1.91/djangoldp_needle/templates/registration/login.html`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/templates/email.html` & `djangoldp_needle-0.1.91/djangoldp_needle/templates/emails/contact.html`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/templates/oidc_provider/authorize.html` & `djangoldp_needle-0.1.91/djangoldp_needle/templates/oidc_provider/authorize.html`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/templates/password/email.html` & `djangoldp_needle-0.1.91/djangoldp_needle/templates/password/email.html`

 * *Files 2% similar despite different names*

```diff
@@ -7,12 +7,14 @@
     <p style='font-style:italic;color:#777'>{% trans "Un compte a été créé pour vous" %} {{ on }}</p>
     <p>{% trans "Créez votre mot de passe en " %}<a href='{{ password_link }}'>{%trans "suivant ce lien." %}</a></p>
 </div>
 <div style='margin-top:10px;'>
     <p style='font-size:small;color:#777'>
         --
         <br>
-        {% trans "Ne répondez pas directement à cet e-mail, à la place rendez-vous sur" %} <a href='{{ on }}' target='_blank'>{{ on }}</a>
+        {% trans "Ne répondez pas directement à cet e-mail, à la place rendez-vous sur" %} <a href='{{ on }}'
+                                                                                              target='_blank'>{{ on
+        }}</a>
         <br>
     </p>
 </div>
 {% endblock %}
```

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/templates/django_registration/activation_email_body.txt` & `djangoldp_needle-0.1.91/djangoldp_needle/templates/django_registration/activation_email_body.txt`

 * *Files 18% similar despite different names*

```diff
@@ -8,7 +8,9 @@
 {{ expiration_days }} jours :
 
 http://{{ siteurl }}{{ activation_key_url }}
 
 Bonne journée,
 l'équipe {{ sitename }}
 {% endblocktrans %}
+
+Mentions Légales / CGV /CGU : http://{{ site.domain }}/cgu
```

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/templates/django_registration/activation_complete.html` & `djangoldp_needle-0.1.91/djangoldp_needle/templates/django_registration/activation_complete.html`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/templates/django_registration/authorize.html` & `djangoldp_needle-0.1.91/djangoldp_needle/templates/django_registration/authorize.html`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/request_parser/parsers/linkIcon.py` & `djangoldp_needle-0.1.91/djangoldp_needle/request_parser/parsers/linkIcon.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/request_parser/parsers/opengraph.py` & `djangoldp_needle-0.1.91/djangoldp_needle/request_parser/parsers/opengraph.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/request_parser/parsers/urlParser.py` & `djangoldp_needle-0.1.91/djangoldp_needle/request_parser/parsers/urlParser.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/request_parser/parsers/metaProp.py` & `djangoldp_needle-0.1.91/djangoldp_needle/request_parser/parsers/metaProp.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/request_parser/parsers/itemProp.py` & `djangoldp_needle-0.1.91/djangoldp_needle/request_parser/parsers/itemProp.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/request_parser/parsers/linkCanonicalProp.py` & `djangoldp_needle-0.1.91/djangoldp_needle/request_parser/parsers/linkCanonicalProp.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/request_parser/parsers/jsonld.py` & `djangoldp_needle-0.1.91/djangoldp_needle/request_parser/parsers/jsonld.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/request_parser/parsers/lastChanceParser.py` & `djangoldp_needle-0.1.91/djangoldp_needle/request_parser/parsers/lastChanceParser.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/request_parser/parsers/titleTag.py` & `djangoldp_needle-0.1.91/djangoldp_needle/request_parser/parsers/titleTag.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/request_parser/webdriver_utils.py` & `djangoldp_needle-0.1.91/djangoldp_needle/request_parser/webdriver_utils.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/request_parser/request_parser.py` & `djangoldp_needle-0.1.91/djangoldp_needle/request_parser/request_parser.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/static/images/background.png` & `djangoldp_needle-0.1.91/djangoldp_needle/static/images/background.png`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/static/needle.css` & `djangoldp_needle-0.1.91/djangoldp_needle/static/needle.css`

 * *Files 12% similar despite different names*

```diff
@@ -27,8 +27,15 @@
 label[for="id_email"]:after {
     color: var(--text-color);
     position: absolute;
     left: 0;
     top: 0;
     display: block;
     content: 'E-mail :';
+}
+
+.logo {
+    max-width: 250px;
+    max-height: 250px;
+    width: auto;
+    height: auto;
 }
```

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/views/annotation.py` & `djangoldp_needle-0.1.91/djangoldp_needle/views/annotation.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/views/__init__.py` & `djangoldp_needle-0.1.91/djangoldp_needle/views/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,13 +3,16 @@
 from .annotation_target import AnnotationTargetViewset
 from .annotation_intersections import AnnotationIntersectionsViewset
 from .needle_activity import NeedleActivityViewset
 from .needle_user_profile import NeedleUserProfileViewset
 from .annotation_intersection_read import AnnotationIntersectionReadViewset
 from .contact_message import ContactMessageView
 from .booklet import BookletViewset
+from .booklet_contributor import BookletContributorViewset
+from .booklet_contributor_pending import BookletContributorPendingViewset
 from .booklet_invitation import BookletInvitationViewset
 from .booklet_quit import BookletQuitViewset
 from .needle_user_follow import NeedleUserFollowViewset
-from .user import UserViewset
+from .needle_user_contact import NeedleUserContactViewset, validate_invitation
+from .needle_user_contact_pending import NeedleUserContactPendingViewset
 from .avatars import avatars_animals_list, avatars_quality_list
 from .avatar import AvatarViewset
```

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/views/annotation_intersections.py` & `djangoldp_needle-0.1.91/djangoldp_needle/views/annotation_intersections.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 from rest_framework import serializers
 import base64
 
 from ..models import AnnotationTarget, Annotation
 
 class AnnotationIntersectionsViewset(LDPViewSet):
     def get_queryset(self, *args, **kwargs):
+        if self.request.user.is_anonymous:
+            return super().get_queryset()
+
         targets = self.request.data['targets']
         if not isinstance(targets, list):
             targets = [targets]
 
         res = Annotation\
             .objects \
             .select_related('target') \
```

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/views/annotation_intersection_read.py` & `djangoldp_needle-0.1.91/djangoldp_needle/views/annotation_intersection_read.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/views/annotation_target.py` & `djangoldp_needle-0.1.91/djangoldp_needle/views/annotation_target.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/views/booklet_invitation.py` & `djangoldp_needle-0.1.91/djangoldp_needle/views/booklet_invitation.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,26 +3,46 @@
 from djangoldp.views import LDPViewSet
 from django.conf import settings
 from djangoldp_account.models import LDPUser
 
 from rest_framework import status
 from rest_framework.exceptions import ValidationError, NotFound
 from rest_framework.response import Response
-from ..models import Booklet
+from ..models import Booklet, BookletContributor
 
 
 class BookletInvitationViewset(LDPViewSet):
     def create(self, request, *args, **kwargs):
         booklet = Booklet.objects.get(pk=kwargs['pk'])
-        if request.user not in booklet.owners.all():
+
+        user_is_owner = BookletContributor.objects.filter(
+            booklet=booklet,
+            user=request.user,
+            role=BookletContributor.ROLE_OWNER
+        ).count() > 0
+
+        if not user_is_owner:
             raise NotFound()
         try:
             target = LDPUser.objects.get(email=request.data['email'])
         except LDPUser.DoesNotExist as e:
             raise ValidationError(detail="Invalid email")
-        booklet.contributors.add(target)
+
+        target_is_contributor = BookletContributor.objects.filter(
+            booklet=booklet,
+            user=target,
+        ).count() > 0
+        if target_is_contributor:
+            raise ValidationError(detail="Target exist")
+
+        contributor = BookletContributor(
+            booklet=booklet,
+            user=target,
+            role=BookletContributor.ROLE_VISIT
+        )
+        contributor.save()
 
         response_serializer = self.get_serializer()
         data = response_serializer.to_representation(booklet)
         headers = self.get_success_headers(data)
         return Response(data, status=status.HTTP_201_CREATED, headers=headers)
```

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/views/booklet_quit.py` & `djangoldp_needle-0.1.91/djangoldp_needle/views/booklet_quit.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,35 @@
 import json
 
+from django.core.exceptions import ObjectDoesNotExist
 from djangoldp.views import LDPViewSet
 from django.conf import settings
 from djangoldp_account.models import LDPUser
 
 from rest_framework import status
 from rest_framework.exceptions import ValidationError, NotFound
 from rest_framework.response import Response
-from ..models import Booklet
+from ..models import Booklet, BookletContributor
 
 
 class BookletQuitViewset(LDPViewSet):
     def create(self, request, *args, **kwargs):
-        booklet = Booklet.objects.get(pk=kwargs['pk'])
-        if request.user not in booklet.contributors.all():
+        try:
+            booklet = Booklet.objects.get(pk=kwargs['pk'])
+        except ObjectDoesNotExist:
             raise NotFound()
 
-        booklet.contributors.remove(request.user)
+        try:
+            booklet_contributor = BookletContributor.objects.get(
+                booklet=booklet,
+                user=request.user
+            )
+        except ObjectDoesNotExist:
+            raise NotFound()
+
+        booklet_contributor.delete()
 
         response_serializer = self.get_serializer()
         data = response_serializer.to_representation(booklet)
         headers = self.get_success_headers(data)
         return Response(data, status=status.HTTP_200_OK, headers=headers)
```

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/migrations/0032_avatar2.py` & `djangoldp_needle-0.1.91/djangoldp_needle/migrations/0032_avatar2.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/migrations/0001_initial.py` & `djangoldp_needle-0.1.91/djangoldp_needle/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/migrations/0013_needleuserprofile.py` & `djangoldp_needle-0.1.91/djangoldp_needle/migrations/0013_needleuserprofile.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/migrations/0015_auto_20230112_1339.py` & `djangoldp_needle-0.1.91/djangoldp_needle/migrations/0015_auto_20230112_1339.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/migrations/0002_tag.py` & `djangoldp_needle-0.1.91/djangoldp_needle/migrations/0002_tag.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/migrations/0014_auto_20230105_1238.py` & `djangoldp_needle-0.1.91/djangoldp_needle/migrations/0014_auto_20230105_1238.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/migrations/0007_auto_20221114_1643.py` & `djangoldp_needle-0.1.91/djangoldp_needle/migrations/0007_auto_20221114_1643.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/migrations/0023_booklet.py` & `djangoldp_needle-0.1.91/djangoldp_needle/migrations/0023_booklet.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/migrations/0011_auto_20221125_1015.py` & `djangoldp_needle-0.1.91/djangoldp_needle/migrations/0011_auto_20221125_1015.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/migrations/0032_avatar.py` & `djangoldp_needle-0.1.91/djangoldp_needle/migrations/0032_avatar.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/migrations/0017_annotationintersectionread.py` & `djangoldp_needle-0.1.91/djangoldp_needle/migrations/0017_annotationintersectionread.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/migrations/0025_needleuserfollow.py` & `djangoldp_needle-0.1.91/djangoldp_needle/migrations/0025_needleuserfollow.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/migrations/0019_contactmessage.py` & `djangoldp_needle-0.1.91/djangoldp_needle/migrations/0019_contactmessage.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/migrations/0020_contactmessage_creation_date.py` & `djangoldp_needle-0.1.91/djangoldp_needle/migrations/0020_contactmessage_creation_date.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/migrations/0027_needleuserfollow_creation_date.py` & `djangoldp_needle-0.1.91/djangoldp_needle/migrations/0027_needleuserfollow_creation_date.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/migrations/0008_activity.py` & `djangoldp_needle-0.1.91/djangoldp_needle/migrations/0008_activity.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/migrations/0016_auto_20230123_1741.py` & `djangoldp_needle-0.1.91/djangoldp_needle/migrations/0016_auto_20230123_1741.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/models/annotation.py` & `djangoldp_needle-0.1.91/djangoldp_needle/models/annotation.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/models/activity_signal_receiver.py` & `djangoldp_needle-0.1.91/djangoldp_needle/models/activity_signal_receiver.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/models/__init__.py` & `djangoldp_needle-0.1.91/djangoldp_needle/models/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,17 @@
+from .needle_user_contact import NeedleUserContact
+from .needle_user_contact_pending import NeedleUserContactPending
 from .avatar import Avatar
 from .tag import Tag
 from .annotation import Annotation
 from .annotation_target import AnnotationTarget
 from .needle_activity import NeedleActivity, ACTIVITY_TYPE_NEW_USER, ACTIVITY_TYPE_FIRST_ANNOTATION_WITH_CONNECTIONS, ACTIVITY_TYPE_FIRST_ANNOTATION_WITHOUT_CONNECTIONS
 from .needle_user_profile import  NeedleUserProfile
 from .annotation_intersection_read import AnnotationIntersectionRead
 from .activity_signal_receiver import post_save_user
 from .contact_message import ContactMessage
 from .booklet import Booklet
+from .booklet_contributor import BookletContributor
+from .booklet_contributor_pending import BookletContributorPending
 from .needle_user_follow import NeedleUserFollow
+
+from .ldp_user import UserSerializer
```

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/models/needle_user_profile.py` & `djangoldp_needle-0.1.91/djangoldp_needle/models/needle_user_profile.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/models/needle_activity.py` & `djangoldp_needle-0.1.91/djangoldp_needle/models/needle_activity.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/models/contact_message.py` & `djangoldp_needle-0.1.91/djangoldp_needle/models/contact_message.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,24 +33,24 @@
         return
 
     email_from = getattr(settings, 'DEFAULT_FROM_EMAIL', False)
     if not email_from:
         return
 
     message = loader.render_to_string(
-        'email.txt',
+        'emails/contact.txt',
         {
             'source': instance.source.email,
             'message': instance.message
         }
     )
 
 
     html_message =  loader.render_to_string(
-        'email.html',
+        'emails/contact.html',
         {
             'source': instance.source.email,
             'message': instance.message
         }
     )
 
     send_mail(
```

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/models/booklet.py` & `djangoldp_needle-0.1.91/djangoldp_needle/models/tag.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 from django.conf import settings
 from django.db import models
 from djangoldp.models import Model
-from . import Annotation, Tag
-from ..permissions import BookletPermissions
 
+from ..permissions import TagPermissions
 
-class Booklet(Model):
-    owners = models.ManyToManyField(settings.AUTH_USER_MODEL, related_name="boolket_owner")
-    contributors = models.ManyToManyField(settings.AUTH_USER_MODEL, related_name="boolket_contributor")
-    annotations = models.ManyToManyField(Annotation, related_name="booklets")
-    title = models.CharField(max_length=160)
-    abstract = models.CharField(max_length=4096, null=True)
-    accessibility_public = models.BooleanField()
-    collaboration_allowed = models.BooleanField()
-    tags = models.ManyToManyField(Tag)
-    cover = models.IntegerField()
+
+class Tag(Model):
+    creator = models.ForeignKey(settings.AUTH_USER_MODEL,
+                                related_name='tags',
+                                null=True,
+                                on_delete=models.SET_NULL
+                                )
+    creation_date = models.DateTimeField(auto_now_add=True)
+    name = models.CharField(max_length=64)
 
     class Meta(Model.Meta):
-        rdf_type = 'hd:annotation'
-        #rdf_context = 'https://www.w3.org/ns/anno.jsonld'
-        owner_field = "owners"
-        owner_perms = []
-        authenticated_perms = []
-        anonymous_perms = []
-        permission_classes = [BookletPermissions]
+        rdf_type = 'hd:tag'
+        authenticated_perms = ['add', 'view']
+        owner_field = 'creator'
+        owner_perms = ['view']
+        permission_classes = [TagPermissions]
```

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/models/annotation_intersection_read.py` & `djangoldp_needle-0.1.91/djangoldp_needle/models/annotation_intersection_read.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,14 +13,15 @@
                                 )
     annotation = models.ForeignKey(Annotation, on_delete=models.CASCADE)
     creation_date = models.DateTimeField(auto_now_add=True)
 
     class Meta(Model.Meta):
         rdf_type = 'hd:annotation_intersection_read'
         #rdf_context = 'https://www.w3.org/ns/anno.jsonld'
+        depth = 1
         anonymous_perms = []
         authenticated_perms = ['add']
         auto_author = 'creator'
         owner_field = 'creator'
         owner_perms = ['view', 'delete']
         constraints = [
             models.UniqueConstraint(
```

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/models/annotation_target.py` & `djangoldp_needle-0.1.91/djangoldp_needle/models/annotation_target.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/models/avatar.py` & `djangoldp_needle-0.1.91/djangoldp_needle/models/avatar.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         avatarConfig = getattr(settings, 'NEEDLE_AVATARS', {})
 
         try:
             rep['avatar_url'] = avatarConfig[rep['name_avatar']]['image']
         except:
             rep['avatar_url'] = None
 
-        rep['full_name'] = (avatarConfig[rep['name_avatar']]['name'] or '')+ " " + (obj.name_quality or '') + "#" + obj.name_number
+        rep['full_name'] = obj.get_full_name()
 
         return rep
 
 class Avatar(Model):
     creator = models.OneToOneField(settings.AUTH_USER_MODEL,
                                    related_name='avatar',
                                    on_delete=models.CASCADE,
@@ -32,14 +32,18 @@
 
     name = models.CharField(max_length=16)
 
     @classmethod
     def get_serializer_class(cls):
         return AvatarSerializer
 
+    def get_full_name(self):
+        avatarConfig = getattr(settings, 'NEEDLE_AVATARS', {})
+        return (avatarConfig[self.name_avatar]['name'] or '')+ " " + (self.name_quality or '') + "#" + str(self.name_number)
+
     class Meta(Model.Meta):
         rdf_type = 'hd:avatar'
         owner_field = 'creator'
         authenticated_perms = ['view']
         anonymous_perms = ['view']
         owner_perms = ['view', 'change']
         permission_classes = [AvatarPermissions]
```

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle/models/needle_user_follow.py` & `djangoldp_needle-0.1.91/djangoldp_needle/models/needle_user_follow.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,14 @@
 
     class Meta(Model.Meta):
         rdf_type = 'hd:annotation'
         #rdf_context = 'https://www.w3.org/ns/anno.jsonld'
         authenticated_perms = ['add']
         auto_author = 'follow_from'
         owner_field = 'follow_from'
-        owner_perms = ['view', 'delete']
+        owner_perms = ['view', 'change', 'delete']
         constraints = [
             models.UniqueConstraint(
                 fields=["follow_from", "follow_to"], name="unique_follow"
             )
         ]
         permission_classes = [NeedleUserFollowPermissions]
```

### Comparing `djangoldp_needle-0.1.90/setup.cfg` & `djangoldp_needle-0.1.91/setup.cfg`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.90/PKG-INFO` & `djangoldp_needle-0.1.91/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangoldp_needle
-Version: 0.1.90
+Version: 0.1.91
 Summary: Needle backend
 Home-page: UNKNOWN
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Provides-Extra: include_package_data
 Provides-Extra: dev
```

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle.egg-info/PKG-INFO` & `djangoldp_needle-0.1.91/djangoldp_needle.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangoldp-needle
-Version: 0.1.90
+Version: 0.1.91
 Summary: Needle backend
 Home-page: UNKNOWN
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Provides-Extra: include_package_data
 Provides-Extra: dev
```

### Comparing `djangoldp_needle-0.1.90/djangoldp_needle.egg-info/SOURCES.txt` & `djangoldp_needle-0.1.91/djangoldp_needle.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 djangoldp_needle/djangoldp_urls.py
 djangoldp_needle/settings.py
 djangoldp_needle.egg-info/PKG-INFO
 djangoldp_needle.egg-info/SOURCES.txt
 djangoldp_needle.egg-info/dependency_links.txt
 djangoldp_needle.egg-info/requires.txt
 djangoldp_needle.egg-info/top_level.txt
+djangoldp_needle/form/__init__.py
+djangoldp_needle/form/needle_user_form.py
 djangoldp_needle/management/__init__.py
 djangoldp_needle/management/commands/__init__.py
 djangoldp_needle/management/commands/importneedledata.py
 djangoldp_needle/migrations/0001_initial.py
 djangoldp_needle/migrations/0002_tag.py
 djangoldp_needle/migrations/0003_annotation_tags.py
 djangoldp_needle/migrations/0004_annotationtarget_image.py
@@ -44,36 +46,50 @@
 djangoldp_needle/migrations/0025_needleuserfollow.py
 djangoldp_needle/migrations/0026_auto_20230331_1603.py
 djangoldp_needle/migrations/0027_needleuserfollow_creation_date.py
 djangoldp_needle/migrations/0028_annotationtarget_annotation_target_date.py
 djangoldp_needle/migrations/0029_auto_20230411_1211.py
 djangoldp_needle/migrations/0032_avatar.py
 djangoldp_needle/migrations/0032_avatar2.py
+djangoldp_needle/migrations/0033_auto_20230509_1434.py
+djangoldp_needle/migrations/0034_auto_20230515_1735.py
+djangoldp_needle/migrations/0035_auto_20230525_1351.py
+djangoldp_needle/migrations/0036_auto_20230526_1301.py
+djangoldp_needle/migrations/0037_auto_20230604_1525.py
 djangoldp_needle/migrations/__init__.py
 djangoldp_needle/models/__init__.py
 djangoldp_needle/models/activity_signal_receiver.py
 djangoldp_needle/models/annotation.py
 djangoldp_needle/models/annotation_intersection_read.py
 djangoldp_needle/models/annotation_target.py
 djangoldp_needle/models/avatar.py
 djangoldp_needle/models/booklet.py
+djangoldp_needle/models/booklet_contributor.py
+djangoldp_needle/models/booklet_contributor_pending.py
 djangoldp_needle/models/contact_message.py
+djangoldp_needle/models/ldp_user.py
 djangoldp_needle/models/needle_activity.py
+djangoldp_needle/models/needle_user_contact.py
+djangoldp_needle/models/needle_user_contact_pending.py
 djangoldp_needle/models/needle_user_follow.py
 djangoldp_needle/models/needle_user_profile.py
 djangoldp_needle/models/tag.py
 djangoldp_needle/permissions/__init__.py
 djangoldp_needle/permissions/_base.py
 djangoldp_needle/permissions/annotation.py
 djangoldp_needle/permissions/annotation_intersection_read.py
 djangoldp_needle/permissions/annotation_target.py
 djangoldp_needle/permissions/avatar.py
 djangoldp_needle/permissions/booklet.py
+djangoldp_needle/permissions/booklet_contributor.py
+djangoldp_needle/permissions/booklet_contributor_pending.py
 djangoldp_needle/permissions/contact_message.py
 djangoldp_needle/permissions/needle_activity.py
+djangoldp_needle/permissions/needle_user_contact.py
+djangoldp_needle/permissions/needle_user_contact_pending.py
 djangoldp_needle/permissions/needle_user_follow.py
 djangoldp_needle/permissions/needle_user_profile.py
 djangoldp_needle/permissions/tag.py
 djangoldp_needle/request_parser/__init__.py
 djangoldp_needle/request_parser/request_parser.py
 djangoldp_needle/request_parser/webdriver_utils.py
 djangoldp_needle/request_parser/parsers/__init__.py
@@ -89,29 +105,37 @@
 djangoldp_needle/request_parser/parsers/urlParser.py
 djangoldp_needle/settings/__init__.py
 djangoldp_needle/settings/avatar.py
 djangoldp_needle/static/needle.css
 djangoldp_needle/static/images/background.png
 djangoldp_needle/templates/__init__.py
 djangoldp_needle/templates/base.html
-djangoldp_needle/templates/email.html
-djangoldp_needle/templates/email.txt
 djangoldp_needle/templates/django_registration/activation_complete.html
+djangoldp_needle/templates/django_registration/activation_email.html
 djangoldp_needle/templates/django_registration/activation_email_body.txt
 djangoldp_needle/templates/django_registration/activation_email_subject.txt
 djangoldp_needle/templates/django_registration/activation_failed.html
 djangoldp_needle/templates/django_registration/authorize.html
 djangoldp_needle/templates/django_registration/registration_base.html
 djangoldp_needle/templates/django_registration/registration_closed.html
 djangoldp_needle/templates/django_registration/registration_complete.html
 djangoldp_needle/templates/django_registration/registration_form.html
+djangoldp_needle/templates/emails/booklet_pending.html
+djangoldp_needle/templates/emails/booklet_pending.txt
+djangoldp_needle/templates/emails/contact.html
+djangoldp_needle/templates/emails/contact.txt
+djangoldp_needle/templates/emails/invitation.html
+djangoldp_needle/templates/emails/invitation.txt
+djangoldp_needle/templates/emails/invitation_pending.html
+djangoldp_needle/templates/emails/invitation_pending.txt
 djangoldp_needle/templates/oidc_provider/authorize.html
 djangoldp_needle/templates/password/email.html
 djangoldp_needle/templates/registration/activate.html
 djangoldp_needle/templates/registration/activation_complete.html
+djangoldp_needle/templates/registration/activation_email.html
 djangoldp_needle/templates/registration/activation_email.txt
 djangoldp_needle/templates/registration/activation_email_subject.txt
 djangoldp_needle/templates/registration/login.html
 djangoldp_needle/templates/registration/logout.html
 djangoldp_needle/templates/registration/lost_user.html
 djangoldp_needle/templates/registration/password_change_done.html
 djangoldp_needle/templates/registration/password_change_form.html
@@ -121,28 +145,37 @@
 djangoldp_needle/templates/registration/password_reset_email.html
 djangoldp_needle/templates/registration/password_reset_email.txt
 djangoldp_needle/templates/registration/password_reset_form.html
 djangoldp_needle/templates/registration/password_reset_subject.txt
 djangoldp_needle/templates/registration/registration_closed.html
 djangoldp_needle/templates/registration/registration_complete.html
 djangoldp_needle/templates/registration/registration_form.html
+djangoldp_needle/templatetags/__init__.py
+djangoldp_needle/templatetags/settings_value.py
 djangoldp_needle/tests/__init__.py
 djangoldp_needle/tests/runner.py
 djangoldp_needle/tests/test_annotation_activity.py
 djangoldp_needle/tests/test_annotation_import.py
 djangoldp_needle/tests/test_annotation_intersection.py
 djangoldp_needle/tests/test_annotation_target_add.py
 djangoldp_needle/tests/test_annotation_yarn.py
+djangoldp_needle/tests/test_booklet_contributor_pending.py
+djangoldp_needle/tests/test_booklet_contributors_delete.py
+djangoldp_needle/tests/test_booklet_contributors_patch.py
 djangoldp_needle/tests/test_booklets_add.py
+djangoldp_needle/tests/test_booklets_add_annotation.py
 djangoldp_needle/tests/test_booklets_invitation.py
 djangoldp_needle/tests/test_booklets_list.py
 djangoldp_needle/tests/test_booklets_quit.py
 djangoldp_needle/tests/test_date_parser.py
 djangoldp_needle/tests/test_first_annotation_on_user_creation.py
+djangoldp_needle/tests/test_needle_user_contact.py
+djangoldp_needle/tests/test_needle_user_contact_pending.py
 djangoldp_needle/tests/test_user_contact.py
+djangoldp_needle/tests/test_user_serializer.py
 djangoldp_needle/tests/data/__init__.py
 djangoldp_needle/tests/data/parsing/base_invalid.20221103.html
 djangoldp_needle/tests/data/parsing/base_valid.20221103.html
 djangoldp_needle/tests/data/parsing/blogdumoderateur-1.html
 djangoldp_needle/tests/data/parsing/fredcavazza-1.html
 djangoldp_needle/tests/data/parsing/internetactu-1.html
 djangoldp_needle/tests/data/parsing/latribune-1.html
@@ -165,15 +198,18 @@
 djangoldp_needle/views/annotation.py
 djangoldp_needle/views/annotation_intersection_read.py
 djangoldp_needle/views/annotation_intersections.py
 djangoldp_needle/views/annotation_target.py
 djangoldp_needle/views/avatar.py
 djangoldp_needle/views/avatars.py
 djangoldp_needle/views/booklet.py
+djangoldp_needle/views/booklet_contributor.py
+djangoldp_needle/views/booklet_contributor_pending.py
 djangoldp_needle/views/booklet_invitation.py
 djangoldp_needle/views/booklet_quit.py
 djangoldp_needle/views/contact_message.py
 djangoldp_needle/views/needle_activity.py
+djangoldp_needle/views/needle_user_contact.py
+djangoldp_needle/views/needle_user_contact_pending.py
 djangoldp_needle/views/needle_user_follow.py
 djangoldp_needle/views/needle_user_profile.py
-djangoldp_needle/views/tag.py
-djangoldp_needle/views/user.py
+djangoldp_needle/views/tag.py
```

