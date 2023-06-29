# Comparing `tmp/stdatamodels-1.6.0.tar.gz` & `tmp/stdatamodels-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stdatamodels-1.6.0.tar", last modified: Thu Jun 15 17:45:38 2023, max compression
+gzip compressed data, was "stdatamodels-1.7.0.tar", last modified: Thu Jun 29 13:42:15 2023, max compression
```

## Comparing `stdatamodels-1.6.0.tar` & `stdatamodels-1.7.0.tar`

### file list

```diff
@@ -1,442 +1,445 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:38.507204 stdatamodels-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:38.431204 stdatamodels-1.6.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:38.431204 stdatamodels-1.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/.github/workflows/changelog.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/.github/workflows/ci_cron.yml
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-06-15 17:45:38.507204 stdatamodels-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:38.431204 stdatamodels-1.6.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/docs/rtd_environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:38.431204 stdatamodels-1.6.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/docs/source/asdf_in_fits.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:38.427204 stdatamodels-1.6.0/docs/source/jwst/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:38.431204 stdatamodels-1.6.0/docs/source/jwst/datamodels/
--rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/docs/source/jwst/datamodels/attributes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/docs/source/jwst/datamodels/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6856 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/docs/source/jwst/datamodels/metadata.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/docs/source/jwst/datamodels/models.rst
--rw-r--r--   0 runner    (1001) docker     (123)    16199 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/docs/source/jwst/datamodels/new_model.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/docs/source/jwst/datamodels/structure.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:38.431204 stdatamodels-1.6.0/docs/source/jwst/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/docs/source/jwst/transforms/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 17:45:38.507204 stdatamodels-1.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:38.431204 stdatamodels-1.6.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:38.435204 stdatamodels-1.6.0/src/stdatamodels/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-15 17:45:38.000000 stdatamodels-1.6.0/src/stdatamodels/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/asdf_in_fits.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/basic_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/dqflags.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/dynamicdq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/filetype.py
--rw-r--r--   0 runner    (1001) docker     (123)    29344 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/fits_support.py
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/history.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:38.435204 stdatamodels-1.6.0/src/stdatamodels/jwst/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:38.443204 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/
--rw-r--r--   0 runner    (1001) docker     (123)     7010 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/abvega_offset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/amilg.py
--rw-r--r--   0 runner    (1001) docker     (123)     8018 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/apcorr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/asn.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/barshadow.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/combinedspec.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/contrast.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/cube.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/dark.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/darkMIRI.py
--rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/dqflags.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/drizpars.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/drizproduct.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/extract1d_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/extract1dimage.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/flat.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/fringe.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/fringefreq.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/gain.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/gls_rampfit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/guider.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/ifucube.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/ifucubepars.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/ifuimage.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/ipc.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/irs2.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/lastframe.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/level1b.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/linearity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/mask.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:38.443204 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/metaschema/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/metaschema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/metaschema/fits-schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/model_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/mrsptcorr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/mrsxartcorr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/multicombinedspec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/multiexposure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/multiextract1d.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/multiprod.py
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/multislit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/multispec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/nirspec_flat.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/outlierifuoutput.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/outlierpars.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/pathloss.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/persat.py
--rw-r--r--   0 runner    (1001) docker     (123)     8922 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/photom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/pixelarea.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/psfmask.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/quad.py
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/ramp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/rampfitoutput.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/readnoise.py
--rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/reset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/resolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/rscd.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/saturation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9633 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schema.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    57881 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schema_editor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:38.467204 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/abvegaoffset.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/amilg.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/asn.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/barshadow.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/bunit.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/camera.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/cheby.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/collimator.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/combinedspec.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/combinedspectable.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/contrast.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    90805 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/core.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/cube.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/dark.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/darkMIRI.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/disperser.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/distortion.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/distortion_mrs.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/dq_def.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/drizpars.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/extract1difu.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/extract1dimage.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/fgsimg_apcorr.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/fgsimg_photom.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/filteroffset.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/flat.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/flatcorr.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/fore.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/fpa.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/fringe.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/fringe_freq.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/gain.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/gls_rampfit.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/group.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/guider_cal.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/guider_meta.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/guider_raw.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/ifucube.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/ifucubepars.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/ifufore.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/ifuimage.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/ifupost.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/ifuslicer.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/image.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/int_times.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/ipc.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/irs2.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_band.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_channel.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_coronmsk.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_exptype.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_filter.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_gainfact.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_grating.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_groupgap.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_lampmode.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_lampstate.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_module.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_nframes.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_ngroups.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_nints.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_noutputs.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pband.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pchannel.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pdetector.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pexptype.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pfilter.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pgrating.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_photmjsr.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pixelarea.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_ppupil.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_preadpatt.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_psubarray.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pupil.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_readpatt.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_tsovisit.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/lastframe.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/level1b.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/linearity.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/mask.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/miri_ifucubepars.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/miri_mrsptcorr.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/miri_mrsxartcorr.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/miri_resolution.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/mirimg_apcorr.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/mirimg_photom.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/mirlrs_apcorr.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/mirlrs_pathloss.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/mirlrs_photom.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/mirmrs_apcorr.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/mirmrs_extract1d.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/mirmrs_photom.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/moving_target.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/msa.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8494 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/msatargacq.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/multicombinedspec.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/multiexposure.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/multiextract1d.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/multislit.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/multispec.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nirspec_area_ifu.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nirspec_area_mos.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nirspec_area_slit.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nirspec_flat.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nirspec_ifucubepars.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nirspec_quad_flat.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nisimg_apcorr.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nisimg_photom.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nissoss_photom.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/niswfss_apcorr.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/niswfss_photom.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nrcimg_apcorr.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nrcimg_photom.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nrcwfss_apcorr.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nrcwfss_photom.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nrsfs_apcorr.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nrsfs_photom.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nrsifu_apcorr.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nrsmos_apcorr.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nrsmos_photom.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/ote.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/outlierifuoutput.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/outlierpars.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/pathloss.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/pathlosscorr.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/persat.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/photomcorr.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/photometry.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/pixelarea.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/psfmask.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/quad.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/ramp.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/rampfitoutput.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/readnoise.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/referencecube.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/referencefile.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/referenceimage.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/referencequad.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/regions.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/reset.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/resolution.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/rscd.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/saturation.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/segmap.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/slit.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/slitdata.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/slitmeta.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/sossextractmodel.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/sosswavegrid.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/spec.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/speckernel.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/specprofile.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/specprofilesingle.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/spectable.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/spectrace.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/spectracesingle.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/spectracetable.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/specwcs.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/specwcs_nircam_grism.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/specwcs_niriss_grism.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/straylight.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/subarray.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/superbias.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/throughput.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/trapdensity.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/trappars.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/trapsfilled.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/tsophot.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/variance.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/wavecorr.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/wavelengthrange.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/wavemap.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/wavemapsingle.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    27691 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/wcsinfo.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/wfssbkg.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/segmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/slit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/sossextractmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/sosswavegrid.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/speckernel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/specprofile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/spectrace.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/straylight.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/superbias.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:38.467204 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:38.483204 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/data/association.json
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/data/association_w_cat.json
--rw-r--r--   0 runner    (1001) docker     (123)    34560 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/data/headers.fits
--rw-r--r--   0 runner    (1001) docker     (123) 16801920 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/data/jwst_nircam_mask_ref.fits
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/data/nircam_abvega_offset.asdf
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/data/nonstandard_primary_array.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/data/nonstandard_primary_array.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/data/sip.fits
--rw-r--r--   0 runner    (1001) docker     (123)  5405760 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/data/test.fits
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/test_fits.py
--rw-r--r--   0 runner    (1001) docker     (123)    14868 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/test_multislit.py
--rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/test_open.py
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/test_schema_against_crds.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/test_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/test_wcs.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/throughput.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/trapdensity.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/trappars.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/trapsfilled.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tsophot.py
--rw-r--r--   0 runner    (1001) docker     (123)    15840 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/wavemap.py
--rw-r--r--   0 runner    (1001) docker     (123)    30980 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/wcs_ref_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/wfssbkg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:38.491204 stdatamodels-1.6.0/src/stdatamodels/jwst/library/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/library/basic_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:38.491204 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:38.491204 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/converters/
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12457 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/converters/jwst_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:38.491204 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/converters/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/converters/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:38.491204 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/converters/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/converters/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/converters/tests/data/niriss_soss.asdf
--rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/converters/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    62822 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:38.491204 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:38.491204 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/manifests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/manifests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/manifests/jwst_transforms-0.7.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/manifests/jwst_transforms-1.0.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:38.427204 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:38.427204 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:38.495204 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/coords-0.7.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/coords-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/grating_equation-0.7.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/grating_equation-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/gwa_to_slit-0.7.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/gwa_to_slit-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/logical-0.7.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/logical-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/miri_ab2slice-0.7.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/miri_ab2slice-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/nircam_grism_dispersion-0.7.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/nircam_grism_dispersion-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/niriss_grism_dispersion-0.7.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/niriss_grism_dispersion-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/niriss_soss-0.7.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/niriss_soss-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/refraction_index_from_prism-0.7.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/refraction_index_from_prism-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/rotation_sequence-0.7.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/rotation_sequence-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/slit_to_msa-0.7.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/slit_to_msa-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/snell-0.7.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/snell-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/v23tosky-0.7.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:38.495204 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/tests/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    38513 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/model_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    18349 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    10059 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:38.435204 stdatamodels-1.6.0/src/stdatamodels.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-06-15 17:45:38.000000 stdatamodels-1.6.0/src/stdatamodels.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22454 2023-06-15 17:45:38.000000 stdatamodels-1.6.0/src/stdatamodels.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 17:45:38.000000 stdatamodels-1.6.0/src/stdatamodels.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-15 17:45:38.000000 stdatamodels-1.6.0/src/stdatamodels.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-15 17:45:38.000000 stdatamodels-1.6.0/src/stdatamodels.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-15 17:45:38.000000 stdatamodels-1.6.0/src/stdatamodels.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 17:45:37.000000 stdatamodels-1.6.0/src/stdatamodels.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:38.499204 stdatamodels-1.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:38.499204 stdatamodels-1.6.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/tests/data/association.json
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/tests/data/association_w_cat.json
--rw-r--r--   0 runner    (1001) docker     (123)    34560 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/tests/data/headers.fits
--rw-r--r--   0 runner    (1001) docker     (123)   501120 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/tests/data/jwst_image.fits
--rw-r--r--   0 runner    (1001) docker     (123)    14400 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/tests/data/mask.fits
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/tests/data/nircam_abvega_offset.asdf
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/tests/data/nonstandard_primary_array.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/tests/data/nonstandard_primary_array.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/tests/data/sip.fits
--rw-r--r--   0 runner    (1001) docker     (123)  5405760 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/tests/data/test.fits
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/tests/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:38.507204 stdatamodels-1.6.0/tests/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/tests/schemas/anyof_model.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/tests/schemas/basic_model.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/tests/schemas/core_metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/tests/schemas/deprecated_model.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/tests/schemas/fits_model.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/tests/schemas/required_model.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/tests/schemas/table_model.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/tests/schemas/transform_model.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/tests/schemas/validation_model.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/tests/test_asdf_in_fits.py
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/tests/test_dq.py
--rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/tests/test_embedded_asdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/tests/test_filetype.py
--rw-r--r--   0 runner    (1001) docker     (123)    20748 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/tests/test_fits.py
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/tests/test_history.py
--rw-r--r--   0 runner    (1001) docker     (123)    10494 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/tests/test_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/tests/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     8493 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    13467 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/tests/test_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:42:15.872050 stdatamodels-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:42:15.796048 stdatamodels-1.7.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:42:15.796048 stdatamodels-1.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/.github/workflows/changelog.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/.github/workflows/ci_cron.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6228 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-06-29 13:42:15.872050 stdatamodels-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:42:15.796048 stdatamodels-1.7.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/docs/rtd_environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:42:15.796048 stdatamodels-1.7.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/docs/source/asdf_in_fits.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:42:15.792047 stdatamodels-1.7.0/docs/source/jwst/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:42:15.796048 stdatamodels-1.7.0/docs/source/jwst/datamodels/
+-rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/docs/source/jwst/datamodels/attributes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/docs/source/jwst/datamodels/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6856 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/docs/source/jwst/datamodels/metadata.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/docs/source/jwst/datamodels/models.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    16199 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/docs/source/jwst/datamodels/new_model.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/docs/source/jwst/datamodels/structure.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:42:15.796048 stdatamodels-1.7.0/docs/source/jwst/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/docs/source/jwst/transforms/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 13:42:15.872050 stdatamodels-1.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:42:15.796048 stdatamodels-1.7.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:42:15.800048 stdatamodels-1.7.0/src/stdatamodels/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-29 13:42:15.000000 stdatamodels-1.7.0/src/stdatamodels/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/asdf_in_fits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/basic_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/dqflags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/dynamicdq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/filetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29344 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/fits_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/history.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:42:15.800048 stdatamodels-1.7.0/src/stdatamodels/jwst/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:42:15.808048 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/
+-rw-r--r--   0 runner    (1001) docker     (123)     7058 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/abvega_offset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/amilg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/amioi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8018 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/apcorr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/asn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/barshadow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/combinedspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/contrast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/cube.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/dark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/darkMIRI.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/dqflags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/drizpars.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/drizproduct.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/extract1d_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/extract1dimage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/flat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/fringe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/fringefreq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/gain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/gls_rampfit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/guider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/ifucube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/ifucubepars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/ifuimage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/ipc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/irs2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/lastframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/level1b.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/linearity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/mask.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:42:15.808048 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/metaschema/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/metaschema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/metaschema/fits-schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/model_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/mrsptcorr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/mrsxartcorr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/multicombinedspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/multiexposure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/multiextract1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/multiprod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/multislit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/multispec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/nirspec_flat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/outlierifuoutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/outlierpars.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/pathloss.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/persat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8922 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/photom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/pixelarea.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/psfmask.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/quad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/ramp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/rampfitoutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/readnoise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/reset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/resolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/rscd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/saturation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9633 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schema.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    57881 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schema_editor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:42:15.832049 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/abvegaoffset.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/amilg.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/amioi.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/asn.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/barshadow.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/bunit.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/camera.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/cheby.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/collimator.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/combinedspec.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/combinedspectable.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/contrast.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    91124 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/core.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/cube.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/dark.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/darkMIRI.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/disperser.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/distortion.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/distortion_mrs.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/dq_def.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/drizpars.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/extract1difu.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/extract1dimage.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/fgsimg_apcorr.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/fgsimg_photom.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/filteroffset.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/flat.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/flatcorr.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/fore.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/fpa.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/fringe.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/fringe_freq.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/gain.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/gls_rampfit.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/group.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/guider_cal.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/guider_meta.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/guider_raw.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/ifucube.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/ifucubepars.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/ifufore.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/ifuimage.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/ifupost.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/ifuslicer.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/image.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/int_times.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/ipc.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/irs2.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/keyword_band.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/keyword_channel.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/keyword_coronmsk.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/keyword_exptype.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/keyword_filter.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/keyword_gainfact.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/keyword_grating.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/keyword_groupgap.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/keyword_lampmode.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/keyword_lampstate.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/keyword_module.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/keyword_nframes.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/keyword_ngroups.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/keyword_nints.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/keyword_noutputs.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pband.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pchannel.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pdetector.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pexptype.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pfilter.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pgrating.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/keyword_photmjsr.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pixelarea.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/keyword_ppupil.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/keyword_preadpatt.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/keyword_psubarray.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pupil.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/keyword_readpatt.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/keyword_tsovisit.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/lastframe.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/level1b.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/linearity.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/mask.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/miri_ifucubepars.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/miri_mrsptcorr.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/miri_mrsxartcorr.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/miri_resolution.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/mirimg_apcorr.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/mirimg_photom.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/mirlrs_apcorr.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/mirlrs_pathloss.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/mirlrs_photom.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/mirmrs_apcorr.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/mirmrs_extract1d.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/mirmrs_photom.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/moving_target.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/msa.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8494 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/msatargacq.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/multicombinedspec.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/multiexposure.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/multiextract1d.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/multislit.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/multispec.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/nirspec_area_ifu.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/nirspec_area_mos.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/nirspec_area_slit.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/nirspec_flat.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/nirspec_ifucubepars.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/nirspec_quad_flat.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/nisimg_apcorr.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/nisimg_photom.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/nissoss_photom.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/niswfss_apcorr.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/niswfss_photom.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/nrcimg_apcorr.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/nrcimg_photom.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/nrcwfss_apcorr.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/nrcwfss_photom.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/nrsfs_apcorr.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/nrsfs_photom.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/nrsifu_apcorr.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/nrsmos_apcorr.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/nrsmos_photom.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    10529 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/oifits.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/ote.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/outlierifuoutput.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/outlierpars.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/pathloss.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/pathlosscorr.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/persat.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/photomcorr.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/photometry.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/pixelarea.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/psfmask.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/quad.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/ramp.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/rampfitoutput.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/readnoise.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/referencecube.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/referencefile.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/referenceimage.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/referencequad.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/regions.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/reset.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/resolution.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/rscd.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/saturation.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/segmap.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/slit.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/slitdata.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/slitmeta.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/sossextractmodel.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/sosswavegrid.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/spec.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/speckernel.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/specprofile.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/specprofilesingle.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/spectable.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/spectrace.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/spectracesingle.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/spectracetable.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/specwcs.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/specwcs_nircam_grism.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/specwcs_niriss_grism.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/straylight.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/subarray.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/superbias.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/throughput.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/trapdensity.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/trappars.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/trapsfilled.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/tsophot.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/variance.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/wavecorr.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/wavelengthrange.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/wavemap.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/wavemapsingle.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    27691 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/wcsinfo.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/wfssbkg.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/segmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/slit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/sossextractmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/sosswavegrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/speckernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/specprofile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/spectrace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/straylight.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/superbias.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:42:15.832049 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:42:15.848049 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/tests/data/association.json
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/tests/data/association_w_cat.json
+-rw-r--r--   0 runner    (1001) docker     (123)    34560 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/tests/data/headers.fits
+-rw-r--r--   0 runner    (1001) docker     (123) 16801920 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/tests/data/jwst_nircam_mask_ref.fits
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/tests/data/nircam_abvega_offset.asdf
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/tests/data/nonstandard_primary_array.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/tests/data/nonstandard_primary_array.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/tests/data/sip.fits
+-rw-r--r--   0 runner    (1001) docker     (123)  5405760 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/tests/data/test.fits
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/tests/test_fits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18983 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/tests/test_multislit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/tests/test_open.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/tests/test_schema_against_crds.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/tests/test_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/tests/test_wcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/throughput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/trapdensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/trappars.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/trapsfilled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/tsophot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15840 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/wavemap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30980 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/wcs_ref_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/wfssbkg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:42:15.856050 stdatamodels-1.7.0/src/stdatamodels/jwst/library/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/library/basic_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:42:15.856050 stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:42:15.856050 stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/converters/
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12457 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/converters/jwst_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:42:15.856050 stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/converters/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/converters/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:42:15.856050 stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/converters/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/converters/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/converters/tests/data/niriss_soss.asdf
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/converters/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62822 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:42:15.856050 stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:42:15.856050 stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/resources/manifests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/resources/manifests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/resources/manifests/jwst_transforms-0.7.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/resources/manifests/jwst_transforms-1.0.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:42:15.792047 stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/resources/schemas/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:42:15.792047 stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:42:15.860050 stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/coords-0.7.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/coords-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/grating_equation-0.7.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/grating_equation-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/gwa_to_slit-0.7.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/gwa_to_slit-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/logical-0.7.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/logical-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/miri_ab2slice-0.7.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/miri_ab2slice-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/nircam_grism_dispersion-0.7.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/nircam_grism_dispersion-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/niriss_grism_dispersion-0.7.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/niriss_grism_dispersion-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/niriss_soss-0.7.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/niriss_soss-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/refraction_index_from_prism-0.7.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/refraction_index_from_prism-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/rotation_sequence-0.7.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/rotation_sequence-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/slit_to_msa-0.7.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/slit_to_msa-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/snell-0.7.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/snell-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/v23tosky-0.7.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:42:15.860050 stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/tests/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38513 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/model_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18807 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10059 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/src/stdatamodels/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:42:15.800048 stdatamodels-1.7.0/src/stdatamodels.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-06-29 13:42:15.000000 stdatamodels-1.7.0/src/stdatamodels.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22615 2023-06-29 13:42:15.000000 stdatamodels-1.7.0/src/stdatamodels.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 13:42:15.000000 stdatamodels-1.7.0/src/stdatamodels.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-29 13:42:15.000000 stdatamodels-1.7.0/src/stdatamodels.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-29 13:42:15.000000 stdatamodels-1.7.0/src/stdatamodels.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-29 13:42:15.000000 stdatamodels-1.7.0/src/stdatamodels.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 13:42:15.000000 stdatamodels-1.7.0/src/stdatamodels.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:42:15.864050 stdatamodels-1.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:42:15.864050 stdatamodels-1.7.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/tests/data/association.json
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/tests/data/association_w_cat.json
+-rw-r--r--   0 runner    (1001) docker     (123)    34560 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/tests/data/headers.fits
+-rw-r--r--   0 runner    (1001) docker     (123)   501120 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/tests/data/jwst_image.fits
+-rw-r--r--   0 runner    (1001) docker     (123)    14400 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/tests/data/mask.fits
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/tests/data/nircam_abvega_offset.asdf
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/tests/data/nonstandard_primary_array.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/tests/data/nonstandard_primary_array.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/tests/data/sip.fits
+-rw-r--r--   0 runner    (1001) docker     (123)  5405760 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/tests/data/test.fits
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/tests/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:42:15.872050 stdatamodels-1.7.0/tests/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/tests/schemas/anyof_model.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/tests/schemas/basic_model.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/tests/schemas/core_metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/tests/schemas/deprecated_model.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/tests/schemas/fits_model.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/tests/schemas/required_model.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/tests/schemas/table_model.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/tests/schemas/transform_model.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/tests/schemas/validation_model.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/tests/test_asdf_in_fits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/tests/test_dq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/tests/test_embedded_asdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/tests/test_filetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20748 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/tests/test_fits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/tests/test_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10494 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/tests/test_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8493 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13467 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/tests/test_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-29 13:42:05.000000 stdatamodels-1.7.0/tox.ini
```

### Comparing `stdatamodels-1.6.0/.github/pull_request_template.md` & `stdatamodels-1.7.0/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/.github/workflows/ci.yml` & `stdatamodels-1.7.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/.github/workflows/ci_cron.yml` & `stdatamodels-1.7.0/.github/workflows/ci_cron.yml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/.github/workflows/publish-to-pypi.yml` & `stdatamodels-1.7.0/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/.gitignore` & `stdatamodels-1.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/CHANGES.rst` & `stdatamodels-1.7.0/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,20 @@
-1.6.1 (unreleased)
+1.7.0 (2023-06-29)
 ==================
 
-- 
+Other
+-----
+
+- Update the allocation of the ZEROFRAME array for the RampModel. [#176]
+
+- Added two new header keywords to the JWST core schema exposure section: PRIMECRS and
+  EXTNCRS, which are used to record the rate of primary cosmic rays and extended cosmic
+  rays (Snowballs and Showers). [#173]
+
+- Add OIFITS compatible schema and ``AmiOIModel`` [#174] 
 
 1.6.0 (2023-06-15)
 ==================
 
 Other
 -----
```

### Comparing `stdatamodels-1.6.0/CODE_OF_CONDUCT.md` & `stdatamodels-1.7.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/CONTRIBUTING.md` & `stdatamodels-1.7.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/LICENSE` & `stdatamodels-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/PKG-INFO` & `stdatamodels-1.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stdatamodels
-Version: 1.6.0
+Version: 1.7.0
 Summary: Core support for DataModel classes used in calibration pipelines
 Author: STScI
 License: Copyright (C) 2020 Association of Universities for Research in Astronomy (AURA)
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `stdatamodels-1.6.0/README.md` & `stdatamodels-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/docs/Makefile` & `stdatamodels-1.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/docs/source/asdf_in_fits.rst` & `stdatamodels-1.7.0/docs/source/asdf_in_fits.rst`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/docs/source/conf.py` & `stdatamodels-1.7.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/docs/source/jwst/datamodels/attributes.rst` & `stdatamodels-1.7.0/docs/source/jwst/datamodels/attributes.rst`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/docs/source/jwst/datamodels/metadata.rst` & `stdatamodels-1.7.0/docs/source/jwst/datamodels/metadata.rst`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/docs/source/jwst/datamodels/models.rst` & `stdatamodels-1.7.0/docs/source/jwst/datamodels/models.rst`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/docs/source/jwst/datamodels/new_model.rst` & `stdatamodels-1.7.0/docs/source/jwst/datamodels/new_model.rst`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/docs/source/jwst/datamodels/structure.rst` & `stdatamodels-1.7.0/docs/source/jwst/datamodels/structure.rst`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/docs/source/jwst/transforms/index.rst` & `stdatamodels-1.7.0/docs/source/jwst/transforms/index.rst`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/pyproject.toml` & `stdatamodels-1.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/asdf_in_fits.py` & `stdatamodels-1.7.0/src/stdatamodels/asdf_in_fits.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/basic_utils.py` & `stdatamodels-1.7.0/src/stdatamodels/basic_utils.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/dqflags.py` & `stdatamodels-1.7.0/src/stdatamodels/dqflags.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/dynamicdq.py` & `stdatamodels-1.7.0/src/stdatamodels/dynamicdq.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/filetype.py` & `stdatamodels-1.7.0/src/stdatamodels/filetype.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/fits_support.py` & `stdatamodels-1.7.0/src/stdatamodels/fits_support.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/history.py` & `stdatamodels-1.7.0/src/stdatamodels/history.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/__init__.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from .model_base import JwstDataModel, DataModel
 from .abvega_offset import ABVegaOffsetModel
 from .amilg import AmiLgModel
+from .amioi import AmiOIModel
 from .apcorr import FgsImgApcorrModel, MirImgApcorrModel
 from .apcorr import NrcImgApcorrModel, NisImgApcorrModel
 from .apcorr import MirLrsApcorrModel, MirMrsApcorrModel
 from .apcorr import NrcWfssApcorrModel, NisWfssApcorrModel
 from .apcorr import NrsMosApcorrModel, NrsIfuApcorrModel, NrsFsApcorrModel
 from .asn import AsnModel
 from .barshadow import BarshadowModel
@@ -89,14 +90,15 @@
 
 
 __all__ = [
     'open',
     'DataModel', 'JwstDataModel',
     'ABVegaOffsetModel',
     'AmiLgModel',
+    'AmiOIModel',
     'FgsImgApcorrModel', 'MirImgApcorrModel', 'NrcImgApcorrModel', 'NisImgApcorrModel',
     'MirLrsApcorrModel', 'MirMrsApcorrModel', 'NrcWfssApcorrModel', 'NisWfssApcorrModel',
     'NrsMosApcorrModel', 'NrsFsApcorrModel', 'NrsIfuApcorrModel',
     'AsnModel',
     'BarshadowModel', 'CameraModel', 'CollimatorModel',
     'CombinedSpecModel', 'ContrastModel', 'CubeModel',
     'DarkModel', 'DarkMIRIModel',
```

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/abvega_offset.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/abvega_offset.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/amilg.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/amilg.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/apcorr.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/apcorr.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/asn.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/asn.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/barshadow.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/barshadow.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/cube.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/cube.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/dark.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/dark.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/darkMIRI.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/darkMIRI.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/dqflags.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/dqflags.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/extract1d_spec.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/extract1d_spec.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/flat.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/flat.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/fringe.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/fringe.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/gls_rampfit.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/gls_rampfit.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/guider.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/guider.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/ifucube.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/ifucube.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/ifucubepars.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/ifucubepars.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/ifuimage.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/ifuimage.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/image.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/image.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/integration.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/integration.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/irs2.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/irs2.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/lastframe.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/lastframe.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/level1b.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/level1b.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/linearity.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/linearity.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/mask.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/mask.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/model_base.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/model_base.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/mrsptcorr.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/mrsptcorr.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/mrsxartcorr.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/mrsxartcorr.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/multicombinedspec.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/multicombinedspec.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/multiexposure.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/multiexposure.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/multiextract1d.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/multiextract1d.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/multislit.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/multislit.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/multispec.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/multispec.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/nirspec_flat.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/nirspec_flat.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/outlierifuoutput.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/outlierifuoutput.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/pathloss.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/pathloss.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/persat.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/persat.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/photom.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/photom.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/pixelarea.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/pixelarea.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/quad.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/quad.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/ramp.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/ramp.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import numpy as np
-
 from .model_base import JwstDataModel
 from stdatamodels.jwst.library.basic_utils import deprecate_class
 
 __all__ = ['RampModel', 'MIRIRampModel']
 
 
 class RampModel(JwstDataModel):
@@ -40,24 +38,14 @@
         super(RampModel, self).__init__(init=init, **kwargs)
 
         # Implicitly create arrays
         self.pixeldq = self.pixeldq
         self.groupdq = self.groupdq
         self.err = self.err
 
-        if isinstance(init, tuple) or self.meta.exposure.zero_frame is True:
-            try:
-                self.getarray_noinit("zeroframe")
-            except AttributeError:
-                # If "zeroframe" is not in the instance, create a zero array with
-                # the correct dimensions.
-                nints, ngroups, nrows, ncols = self.data.shape
-                dims = (nints, nrows, ncols)
-                self.zeroframe = np.zeros(dims, dtype=self.data.dtype)
-
 
 @deprecate_class(RampModel)
 class MIRIRampModel:
     """A data model for 4D MIRI ramps.
 
     This model has been deprecated. Please use `RampModel` instead.
     """
```

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/rampfitoutput.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/rampfitoutput.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/reference.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/reference.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/reset.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/reset.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/resolution.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/resolution.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/rscd.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/rscd.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/saturation.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/saturation.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schema.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schema.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schema_editor.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schema_editor.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/abvegaoffset.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/abvegaoffset.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/amilg.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/amilg.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/barshadow.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/barshadow.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/bunit.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/bunit.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/camera.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/camera.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/cheby.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/cheby.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/collimator.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/collimator.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/combinedspec.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/combinedspec.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/core.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/core.schema.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -923,14 +923,22 @@
             fits_keyword: IS_PSF
             blend_table: True
           self_reference_survey:
             title: self-referencing PSF
             type: boolean
             fits_keyword: SELFREF
             blend_table: True
+          primary_cosmic_rays:
+            title: Cosmic Ray rate per thousand pixels per second
+            type: number
+            fits_keyword: PRIMECRS
+          extended_emission_events:
+            title: Snowballs/showers per million pixels per second
+            type: number
+            fits_keyword: EXTNCRS
       subarray:
         title: Subarray parameters
         type: object
         properties:
           name:
             title: Subarray used
             type: string
```

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/cube.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/cube.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/dark.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/dark.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/darkMIRI.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/darkMIRI.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/disperser.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/disperser.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/distortion.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/distortion.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/distortion_mrs.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/distortion_mrs.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/drizpars.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/drizpars.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/extract1difu.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/extract1difu.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/extract1dimage.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/extract1dimage.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/fgsimg_apcorr.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/fgsimg_apcorr.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/fgsimg_photom.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/fgsimg_photom.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/filteroffset.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/filteroffset.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/flat.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/flat.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/fore.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/fore.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/fpa.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/fpa.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/fringe.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/fringe.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/fringe_freq.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/fringe_freq.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/gls_rampfit.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/gls_rampfit.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/group.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/group.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/guider_cal.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/guider_cal.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/guider_meta.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/guider_meta.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/guider_raw.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/guider_raw.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/ifucube.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/ifucube.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/ifucubepars.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/ifucubepars.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/ifufore.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/ifufore.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/ifuimage.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/ifuimage.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/ifupost.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/ifupost.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/ifuslicer.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/ifuslicer.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/image.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/image.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/int_times.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/int_times.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/irs2.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/irs2.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_band.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/keyword_band.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_coronmsk.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/keyword_coronmsk.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_exptype.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/keyword_exptype.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_filter.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/keyword_filter.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_lampstate.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/keyword_lampstate.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pband.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pband.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pdetector.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pdetector.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pexptype.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pexptype.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pfilter.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pfilter.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pixelarea.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pixelarea.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_ppupil.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/keyword_ppupil.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_preadpatt.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/keyword_preadpatt.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_psubarray.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/keyword_psubarray.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pupil.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pupil.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_readpatt.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/keyword_readpatt.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/lastframe.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/lastframe.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/level1b.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/level1b.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/linearity.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/linearity.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/miri_ifucubepars.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/miri_ifucubepars.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/miri_mrsptcorr.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/miri_mrsptcorr.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/miri_mrsxartcorr.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/miri_mrsxartcorr.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/miri_resolution.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/miri_resolution.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/mirimg_apcorr.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/mirimg_apcorr.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/mirimg_photom.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/mirimg_photom.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/mirlrs_apcorr.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/mirlrs_apcorr.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/mirlrs_pathloss.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/mirlrs_pathloss.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/mirlrs_photom.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/mirlrs_photom.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/mirmrs_apcorr.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/mirmrs_apcorr.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/mirmrs_extract1d.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/mirmrs_extract1d.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/mirmrs_photom.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/mirmrs_photom.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/moving_target.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/moving_target.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/msa.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/msa.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/msatargacq.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/msatargacq.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/multicombinedspec.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/multicombinedspec.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/multiextract1d.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/multiextract1d.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/multispec.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/multispec.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nirspec_area_ifu.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/nirspec_area_ifu.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nirspec_area_mos.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/nirspec_area_mos.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nirspec_area_slit.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/nirspec_area_slit.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nirspec_flat.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/nirspec_flat.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nirspec_ifucubepars.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/nirspec_ifucubepars.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nirspec_quad_flat.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/nirspec_quad_flat.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nisimg_apcorr.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/nisimg_apcorr.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nisimg_photom.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/nisimg_photom.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nissoss_photom.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/nissoss_photom.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/niswfss_apcorr.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/niswfss_apcorr.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/niswfss_photom.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/niswfss_photom.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nrcimg_apcorr.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/nrcimg_apcorr.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nrcimg_photom.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/nrcimg_photom.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nrcwfss_apcorr.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/nrcwfss_apcorr.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nrcwfss_photom.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/nrcwfss_photom.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nrsfs_apcorr.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/nrsfs_apcorr.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nrsfs_photom.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/nrsfs_photom.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nrsifu_apcorr.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/nrsifu_apcorr.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nrsmos_apcorr.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/nrsmos_apcorr.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nrsmos_photom.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/nrsmos_photom.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/ote.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/ote.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/outlierifuoutput.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/outlierifuoutput.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/outlierpars.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/outlierpars.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/pathloss.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/pathloss.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/persat.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/persat.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/photometry.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/photometry.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/quad.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/quad.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/ramp.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/ramp.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/rampfitoutput.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/rampfitoutput.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/referencecube.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/referencecube.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/referencefile.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/referencefile.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/referenceimage.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/referenceimage.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/referencequad.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/referencequad.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/reset.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/reset.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/rscd.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/rscd.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/saturation.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/saturation.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/slitdata.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/slitdata.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/slitmeta.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/slitmeta.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/sossextractmodel.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/sossextractmodel.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/speckernel.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/speckernel.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/specprofilesingle.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/specprofilesingle.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/spectable.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/spectable.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/specwcs.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/specwcs.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/specwcs_nircam_grism.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/specwcs_nircam_grism.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/specwcs_niriss_grism.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/specwcs_niriss_grism.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/subarray.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/subarray.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/superbias.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/superbias.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/trappars.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/trappars.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/tsophot.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/tsophot.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/variance.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/variance.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/wavecorr.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/wavecorr.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/wavelengthrange.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/wavelengthrange.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/wavemapsingle.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/wavemapsingle.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/wcsinfo.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/wcsinfo.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/wfssbkg.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/schemas/wfssbkg.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/slit.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/slit.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/sossextractmodel.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/sossextractmodel.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/specprofile.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/specprofile.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/spectrace.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/spectrace.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/superbias.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/superbias.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/data/association.json` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/tests/data/association.json`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/data/association_w_cat.json` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/tests/data/association_w_cat.json`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/data/headers.fits` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/tests/data/headers.fits`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/data/jwst_nircam_mask_ref.fits` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/tests/data/jwst_nircam_mask_ref.fits`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/data/nircam_abvega_offset.asdf` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/tests/data/nircam_abvega_offset.asdf`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/data/nonstandard_primary_array.schema.json` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/tests/data/nonstandard_primary_array.schema.json`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/data/nonstandard_primary_array.schema.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/tests/data/nonstandard_primary_array.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/data/sip.fits` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/tests/data/sip.fits`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/data/test.fits` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/tests/data/test.fits`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/test_fits.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/tests/test_fits.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/test_models.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/tests/test_models.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import warnings
 
+from asdf.exceptions import ValidationError
 from astropy.io import fits
 from astropy.table import Table
 from astropy.time import Time
 from numpy.testing import assert_allclose, assert_array_equal
 import numpy as np
 import pytest
 
@@ -370,14 +371,130 @@
     dims = (nints, ngroups, nrows, ncols)
     zdims = (nints, nrows, ncols)
 
     with datamodels.RampModel(dims) as ramp:
         assert ramp.zeroframe.shape == zdims
 
 
+@pytest.fixture
+def oifits_ami_model():
+    m = datamodels.AmiOIModel()
+    m.meta.telescope = 'JWST'
+    m.meta.origin = 'STScI'
+    m.meta.instrument.name = 'NIRISS'
+    m.meta.program.pi_name = 'UNKNOWN'
+    m.meta.target.proposer_name = 'AB DOR'
+    m.meta.observation.date = '2022-06-05'
+    m.meta.oifits.array_name = 'g7s6'
+    m.meta.oifits.instrument_mode = 'NRM'
+
+    m.array = [
+        (
+            'A1', 'A1', 1, 0.,
+            [ 2.64000000e+00, -1.61653377e-16,  0.00000000e+00], 5.04539835,
+            'RADIUS', [ 2.60973996, -0.39856915]
+        ),
+        (
+            'A2', 'A2', 2, 0.,
+            [ 1.39996111e-16,  2.28631000e+00,  0.00000000e+00], 5.04539835,
+            'RADIUS', [-0.34517145, -2.260104  ]
+        ),
+        (
+            'A3', 'A3', 3, 0.,
+            [ 1.32000010e+00, -2.28631000e+00,  0.00000000e+00], 5.04539835,
+            'RADIUS', [ 1.65004153,  2.06081941]
+        )
+    ]
+    m.target = [(
+        1, 'AB DOR', 82.18704833, -65.44869139, 2000., 0., 0., 0., 'UNKNOWN',
+        'OPTICAL', 29.15, 164.421, 0., 0., 65.3199, 0., 'K0V')]
+    m.t3 = [
+        (
+            1, 0., 59735., 0.3772, 0.71125417, 0.73752607, -1.81575411, 0.73752607,
+            1.86153485, 2.9549114, -4.32092341, -1.99521297, [1, 2, 3],  0
+        ),
+    ]
+    m.vis = [
+        (
+            1, 0., 59735., 0.3772, 0.84231787, 0.00669874, -10.57082496, 1.89098664,
+            1.86153485,  2.9549114 , [1, 2],  0
+        ),
+        (
+            1, 0., 59735., 0.3772, 0.91448467, 0.00621287, -22.26334374, 1.27637574,
+            -2.45938856,  0.95969843, [1, 3],  0
+        )
+    ]
+    m.vis2 = [
+        (1, 0., 59735., 0.3772, 0.70949939, 0.01131277,  1.86153485, 2.9549114 , [1, 2],  0),
+        (1, 0., 59735., 0.3772, 0.8362822 , 0.0113618 , -2.45938856, 0.95969843, [1, 3],  0)
+    ]
+    m.wavelength = [(4.817e-06, 2.98e-07)]
+    return m
+
+
+def test_amioi_model_oifits_compliance(tmp_path, oifits_ami_model):
+    """
+    This test cannot fully test oifits compliance but the schema for the model
+    provides some checks. This test checks that the model in the oifits_ami_model
+    fixture provides a 'passable' OIFITS file.
+    """
+    fn = tmp_path / "test.fits"
+    oifits_ami_model.save(fn)
+
+
+@pytest.mark.parametrize('attr',
+                         [
+                             'meta.telescope',
+                             'meta.origin',
+                             'meta.instrument.name',
+                             'meta.program.pi_name',
+                             'meta.target.proposer_name',
+                             'meta.observation.date',
+                             'meta.oifits.array_name',
+                             'meta.oifits.instrument_mode',
+                             'array',
+                             'target',
+                             'wavelength',
+                         ])
+def test_amioi_model_oifits_keyword_validation(tmp_path, oifits_ami_model, attr):
+    """
+    Remove some critical keywords or tables and make sure the model fails to
+    save/validate This test cannot fully test oifits compliance but at least
+    does some sanity checks that a file produced using AmiOiModel produces a
+    file containing items that should make it oifits compliant
+    """
+    fn = tmp_path / "test.fits"
+
+    node = oifits_ami_model
+    *branches, leaf = attr.split('.')
+    for branch in branches:
+        node = getattr(node, branch)
+    delattr(node, leaf)
+
+    with pytest.raises(ValidationError):
+        oifits_ami_model.save(fn)
+
+
+@pytest.mark.parametrize('keep', ['vis', 'vis2', 't3'])
+def test_amioi_model_oifits_datatable(tmp_path, oifits_ami_model, keep):
+    fn = tmp_path / "test.fits"
+    for table in ('vis', 'vis2', 't3'):
+        if table == keep:
+            continue
+        delattr(oifits_ami_model, table)
+
+    # since we have 1 data table, this should pass
+    oifits_ami_model.save(fn)
+
+    # removing the data table should cause saving to fail
+    delattr(oifits_ami_model, keep)
+    with pytest.raises(ValidationError):
+        oifits_ami_model.save(fn)
+
+
 def test_dq_def_roundtrip(tmp_path):
     """
     Open a MaskModel with a defined DQ array and dq_def that modifies the
     DQ array on open.  Save the model to a new name.  Open the new model
     to verify the DQ array is equal to the original DQ array.  This validates
     that the dynamic_mask is invertible and computes the same values.
     """
```

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/test_multislit.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/tests/test_multislit.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/test_open.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/tests/test_open.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/test_schema.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/test_schema_against_crds.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/tests/test_schema_against_crds.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/test_validation.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/test_wcs.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/tests/test_wcs.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/trapdensity.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/trapdensity.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/trappars.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/trappars.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tsophot.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/tsophot.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/util.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/util.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/wavemap.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/wavemap.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/wcs_ref_models.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/wcs_ref_models.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/wfssbkg.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/datamodels/wfssbkg.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/library/basic_utils.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/library/basic_utils.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/converters/__init__.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/converters/__init__.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/converters/jwst_models.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/converters/jwst_models.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/converters/tests/data/niriss_soss.asdf` & `stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/converters/tests/data/niriss_soss.asdf`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/converters/tests/test_models.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/converters/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/extensions.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/extensions.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/integration.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/integration.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/models.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/models.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/manifests/jwst_transforms-0.7.0.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/resources/manifests/jwst_transforms-0.7.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/manifests/jwst_transforms-1.0.0.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/resources/manifests/jwst_transforms-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/coords-0.7.0.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/coords-0.7.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/coords-1.0.0.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/coords-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/grating_equation-0.7.0.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/grating_equation-0.7.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/grating_equation-1.0.0.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/grating_equation-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/gwa_to_slit-0.7.0.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/gwa_to_slit-0.7.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/gwa_to_slit-1.0.0.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/gwa_to_slit-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/logical-0.7.0.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/logical-0.7.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/logical-1.0.0.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/logical-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/miri_ab2slice-0.7.0.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/miri_ab2slice-0.7.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/miri_ab2slice-1.0.0.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/miri_ab2slice-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/nircam_grism_dispersion-0.7.0.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/nircam_grism_dispersion-0.7.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/nircam_grism_dispersion-1.0.0.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/nircam_grism_dispersion-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/niriss_grism_dispersion-0.7.0.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/niriss_grism_dispersion-0.7.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/niriss_grism_dispersion-1.0.0.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/niriss_grism_dispersion-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/niriss_soss-0.7.0.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/niriss_soss-0.7.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/niriss_soss-1.0.0.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/niriss_soss-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/refraction_index_from_prism-0.7.0.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/refraction_index_from_prism-0.7.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/refraction_index_from_prism-1.0.0.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/refraction_index_from_prism-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/rotation_sequence-0.7.0.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/rotation_sequence-0.7.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/rotation_sequence-1.0.0.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/rotation_sequence-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/slit_to_msa-0.7.0.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/slit_to_msa-0.7.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/slit_to_msa-1.0.0.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/slit_to_msa-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/snell-0.7.0.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/snell-0.7.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/snell-1.0.0.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/snell-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/v23tosky-0.7.0.yaml` & `stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/v23tosky-0.7.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/tests/tests.py` & `stdatamodels-1.7.0/src/stdatamodels/jwst/transforms/tests/tests.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/model_base.py` & `stdatamodels-1.7.0/src/stdatamodels/model_base.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/properties.py` & `stdatamodels-1.7.0/src/stdatamodels/properties.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,15 +173,23 @@
                 primary_array = getattr(ctx, primary_array_name, None)
                 has_primary_array_shape = primary_array is not None
 
             if has_primary_array_shape:
                 if ndim is None:
                     shape = primary_array.shape
                 else:
-                    shape = primary_array.shape[-ndim:]
+                    if attr == "zeroframe":
+                        dims = primary_array.shape
+                        if len(dims) != 4:
+                            error_msg = "To allocate ZEROFRAME, the primary array must "
+                            error_msg += f"have 4 dimensions, but has {len(dims)}."
+                            raise IndexError(error_msg)
+                        shape = (dims[0], dims[2], dims[3])
+                    else:
+                        shape = primary_array.shape[-ndim:]
             elif ndim is None:
                 shape = (0,)
             else:
                 shape = tuple([0] * ndim)
 
     array = np.empty(shape, dtype=dtype)
     if default is not None:
@@ -310,14 +318,15 @@
             if part == "..":
                 node = node._parent
             else:
                 node = getattr(node, part)
         return node, parts[-1]
 
     def __getattr__(self, attr):
+
         if attr.startswith('_'):
             raise AttributeError('No attribute {0}'.format(attr))
 
         if self._is_deprecated(attr):
             self._warn_deprecated_attr(attr)
             node, new_attr = self._get_deprecated(attr)
             return getattr(node, new_attr)
```

### Comparing `stdatamodels-1.6.0/src/stdatamodels/schema.py` & `stdatamodels-1.7.0/src/stdatamodels/schema.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/util.py` & `stdatamodels-1.7.0/src/stdatamodels/util.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels/validate.py` & `stdatamodels-1.7.0/src/stdatamodels/validate.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/src/stdatamodels.egg-info/PKG-INFO` & `stdatamodels-1.7.0/src/stdatamodels.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stdatamodels
-Version: 1.6.0
+Version: 1.7.0
 Summary: Core support for DataModel classes used in calibration pipelines
 Author: STScI
 License: Copyright (C) 2020 Association of Universities for Research in Astronomy (AURA)
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `stdatamodels-1.6.0/src/stdatamodels.egg-info/SOURCES.txt` & `stdatamodels-1.7.0/src/stdatamodels.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 src/stdatamodels.egg-info/requires.txt
 src/stdatamodels.egg-info/top_level.txt
 src/stdatamodels.egg-info/zip-safe
 src/stdatamodels/jwst/__init__.py
 src/stdatamodels/jwst/datamodels/__init__.py
 src/stdatamodels/jwst/datamodels/abvega_offset.py
 src/stdatamodels/jwst/datamodels/amilg.py
+src/stdatamodels/jwst/datamodels/amioi.py
 src/stdatamodels/jwst/datamodels/apcorr.py
 src/stdatamodels/jwst/datamodels/asn.py
 src/stdatamodels/jwst/datamodels/barshadow.py
 src/stdatamodels/jwst/datamodels/combinedspec.py
 src/stdatamodels/jwst/datamodels/conftest.py
 src/stdatamodels/jwst/datamodels/contrast.py
 src/stdatamodels/jwst/datamodels/cube.py
@@ -134,14 +135,15 @@
 src/stdatamodels/jwst/datamodels/wcs_ref_models.py
 src/stdatamodels/jwst/datamodels/wfssbkg.py
 src/stdatamodels/jwst/datamodels/metaschema/__init__.py
 src/stdatamodels/jwst/datamodels/metaschema/fits-schema.yaml
 src/stdatamodels/jwst/datamodels/schemas/__init__.py
 src/stdatamodels/jwst/datamodels/schemas/abvegaoffset.schema.yaml
 src/stdatamodels/jwst/datamodels/schemas/amilg.schema.yaml
+src/stdatamodels/jwst/datamodels/schemas/amioi.schema.yaml
 src/stdatamodels/jwst/datamodels/schemas/asn.schema.yaml
 src/stdatamodels/jwst/datamodels/schemas/barshadow.schema.yaml
 src/stdatamodels/jwst/datamodels/schemas/bunit.schema.yaml
 src/stdatamodels/jwst/datamodels/schemas/camera.schema.yaml
 src/stdatamodels/jwst/datamodels/schemas/cheby.schema.yaml
 src/stdatamodels/jwst/datamodels/schemas/collimator.schema.yaml
 src/stdatamodels/jwst/datamodels/schemas/combinedspec.schema.yaml
@@ -252,14 +254,15 @@
 src/stdatamodels/jwst/datamodels/schemas/nrcwfss_apcorr.schema.yaml
 src/stdatamodels/jwst/datamodels/schemas/nrcwfss_photom.schema.yaml
 src/stdatamodels/jwst/datamodels/schemas/nrsfs_apcorr.schema.yaml
 src/stdatamodels/jwst/datamodels/schemas/nrsfs_photom.schema.yaml
 src/stdatamodels/jwst/datamodels/schemas/nrsifu_apcorr.schema.yaml
 src/stdatamodels/jwst/datamodels/schemas/nrsmos_apcorr.schema.yaml
 src/stdatamodels/jwst/datamodels/schemas/nrsmos_photom.schema.yaml
+src/stdatamodels/jwst/datamodels/schemas/oifits.schema.yaml
 src/stdatamodels/jwst/datamodels/schemas/ote.schema.yaml
 src/stdatamodels/jwst/datamodels/schemas/outlierifuoutput.schema.yaml
 src/stdatamodels/jwst/datamodels/schemas/outlierpars.schema.yaml
 src/stdatamodels/jwst/datamodels/schemas/pathloss.schema.yaml
 src/stdatamodels/jwst/datamodels/schemas/pathlosscorr.schema.yaml
 src/stdatamodels/jwst/datamodels/schemas/persat.schema.yaml
 src/stdatamodels/jwst/datamodels/schemas/photomcorr.schema.yaml
```

### Comparing `stdatamodels-1.6.0/tests/conftest.py` & `stdatamodels-1.7.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/tests/data/association.json` & `stdatamodels-1.7.0/tests/data/association.json`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/tests/data/association_w_cat.json` & `stdatamodels-1.7.0/tests/data/association_w_cat.json`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/tests/data/headers.fits` & `stdatamodels-1.7.0/tests/data/headers.fits`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/tests/data/jwst_image.fits` & `stdatamodels-1.7.0/tests/data/jwst_image.fits`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/tests/data/mask.fits` & `stdatamodels-1.7.0/tests/data/mask.fits`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/tests/data/nircam_abvega_offset.asdf` & `stdatamodels-1.7.0/tests/data/nircam_abvega_offset.asdf`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/tests/data/nonstandard_primary_array.schema.json` & `stdatamodels-1.7.0/tests/data/nonstandard_primary_array.schema.json`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/tests/data/nonstandard_primary_array.schema.yaml` & `stdatamodels-1.7.0/tests/data/nonstandard_primary_array.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/tests/data/sip.fits` & `stdatamodels-1.7.0/tests/data/sip.fits`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/tests/data/test.fits` & `stdatamodels-1.7.0/tests/data/test.fits`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/tests/models.py` & `stdatamodels-1.7.0/tests/models.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/tests/schemas/basic_model.yaml` & `stdatamodels-1.7.0/tests/schemas/basic_model.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/tests/schemas/deprecated_model.yaml` & `stdatamodels-1.7.0/tests/schemas/deprecated_model.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/tests/schemas/fits_model.yaml` & `stdatamodels-1.7.0/tests/schemas/fits_model.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/tests/schemas/table_model.yaml` & `stdatamodels-1.7.0/tests/schemas/table_model.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/tests/schemas/validation_model.yaml` & `stdatamodels-1.7.0/tests/schemas/validation_model.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/tests/test_asdf_in_fits.py` & `stdatamodels-1.7.0/tests/test_asdf_in_fits.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/tests/test_dq.py` & `stdatamodels-1.7.0/tests/test_dq.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/tests/test_embedded_asdf.py` & `stdatamodels-1.7.0/tests/test_embedded_asdf.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/tests/test_filetype.py` & `stdatamodels-1.7.0/tests/test_filetype.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/tests/test_fits.py` & `stdatamodels-1.7.0/tests/test_fits.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/tests/test_history.py` & `stdatamodels-1.7.0/tests/test_history.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/tests/test_models.py` & `stdatamodels-1.7.0/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/tests/test_resources.py` & `stdatamodels-1.7.0/tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/tests/test_schema.py` & `stdatamodels-1.7.0/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/tests/test_util.py` & `stdatamodels-1.7.0/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/tests/test_validation.py` & `stdatamodels-1.7.0/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.6.0/tox.ini` & `stdatamodels-1.7.0/tox.ini`

 * *Files identical despite different names*

