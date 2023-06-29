# Comparing `tmp/distrax-0.1.3.tar.gz` & `tmp/distrax-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "distrax-0.1.3.tar", last modified: Tue Feb 14 11:03:14 2023, max compression
+gzip compressed data, was "distrax-0.1.4.tar", last modified: Thu Jun 29 14:17:13 2023, max compression
```

## Comparing `distrax-0.1.3.tar` & `distrax-0.1.4.tar`

### file list

```diff
@@ -1,164 +1,164 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 11:03:14.296094 distrax-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-02-14 11:03:02.000000 distrax-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-02-14 11:03:02.000000 distrax-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13001 2023-02-14 11:03:14.296094 distrax-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11984 2023-02-14 11:03:02.000000 distrax-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 11:03:14.272094 distrax-0.1.3/distrax/
--rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 11:03:14.276094 distrax-0.1.3/distrax/_src/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 11:03:14.280094 distrax-0.1.3/distrax/_src/bijectors/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/bijectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7951 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/bijectors/bijector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/bijectors/bijector_from_tfp.py
--rw-r--r--   0 runner    (1001) docker     (123)     9688 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/bijectors/bijector_from_tfp_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/bijectors/bijector_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/bijectors/block.py
--rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/bijectors/block_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/bijectors/chain.py
--rw-r--r--   0 runner    (1001) docker     (123)    10931 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/bijectors/chain_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/bijectors/diag_linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     7510 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/bijectors/diag_linear_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9422 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/bijectors/diag_plus_low_rank_linear.py
--rw-r--r--   0 runner    (1001) docker     (123)    10657 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/bijectors/diag_plus_low_rank_linear_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/bijectors/gumbel_cdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/bijectors/gumbel_cdf_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/bijectors/inverse.py
--rw-r--r--   0 runner    (1001) docker     (123)     9233 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/bijectors/inverse_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/bijectors/lambda_bijector.py
--rw-r--r--   0 runner    (1001) docker     (123)    12894 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/bijectors/lambda_bijector_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/bijectors/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/bijectors/linear_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/bijectors/lower_upper_triangular_affine.py
--rw-r--r--   0 runner    (1001) docker     (123)     8764 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/bijectors/lower_upper_triangular_affine_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/bijectors/masked_coupling.py
--rw-r--r--   0 runner    (1001) docker     (123)    10755 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/bijectors/masked_coupling_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    20159 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/bijectors/rational_quadratic_spline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/bijectors/rational_quadratic_spline_float64_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13180 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/bijectors/rational_quadratic_spline_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/bijectors/scalar_affine.py
--rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/bijectors/scalar_affine_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/bijectors/shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/bijectors/shift_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/bijectors/sigmoid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/bijectors/sigmoid_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/bijectors/split_coupling.py
--rw-r--r--   0 runner    (1001) docker     (123)    10197 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/bijectors/split_coupling_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/bijectors/tanh.py
--rw-r--r--   0 runner    (1001) docker     (123)     6159 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/bijectors/tanh_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9119 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/bijectors/tfp_compatible_bijector.py
--rw-r--r--   0 runner    (1001) docker     (123)    14341 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/bijectors/tfp_compatible_bijector_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/bijectors/triangular_linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/bijectors/triangular_linear_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/bijectors/unconstrained_affine.py
--rw-r--r--   0 runner    (1001) docker     (123)     8199 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/bijectors/unconstrained_affine_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 11:03:14.292094 distrax-0.1.3/distrax/_src/distributions/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/bernoulli.py
--rw-r--r--   0 runner    (1001) docker     (123)    12888 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/bernoulli_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6545 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/beta.py
--rw-r--r--   0 runner    (1001) docker     (123)    10372 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/beta_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7799 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/categorical.py
--rw-r--r--   0 runner    (1001) docker     (123)    22304 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/categorical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5814 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/categorical_uniform.py
--rw-r--r--   0 runner    (1001) docker     (123)    13008 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/categorical_uniform_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5285 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/clipped.py
--rw-r--r--   0 runner    (1001) docker     (123)     7221 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/clipped_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6156 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/deterministic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9858 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/deterministic_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7984 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/dirichlet.py
--rw-r--r--   0 runner    (1001) docker     (123)    10477 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/dirichlet_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/distribution_from_tfp.py
--rw-r--r--   0 runner    (1001) docker     (123)     9828 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/distribution_from_tfp_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10098 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/distribution_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/epsilon_greedy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/epsilon_greedy_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/gamma.py
--rw-r--r--   0 runner    (1001) docker     (123)     8403 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/gamma_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/greedy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/greedy_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/gumbel.py
--rw-r--r--   0 runner    (1001) docker     (123)     9248 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/gumbel_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7106 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/independent.py
--rw-r--r--   0 runner    (1001) docker     (123)    16214 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/independent_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6079 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/joint.py
--rw-r--r--   0 runner    (1001) docker     (123)    18728 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/joint_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/laplace.py
--rw-r--r--   0 runner    (1001) docker     (123)    11436 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/laplace_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/log_stddev_normal.py
--rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/log_stddev_normal_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/logistic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7270 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/logistic_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/mixture_of_two.py
--rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/mixture_of_two_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/mixture_same_family.py
--rw-r--r--   0 runner    (1001) docker     (123)    12708 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/mixture_same_family_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11407 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/multinomial.py
--rw-r--r--   0 runner    (1001) docker     (123)    21199 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/multinomial_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/mvn_diag.py
--rw-r--r--   0 runner    (1001) docker     (123)     8441 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/mvn_diag_plus_low_rank.py
--rw-r--r--   0 runner    (1001) docker     (123)    15802 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/mvn_diag_plus_low_rank_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    17753 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/mvn_diag_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9763 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/mvn_from_bijector.py
--rw-r--r--   0 runner    (1001) docker     (123)    11596 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/mvn_from_bijector_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5028 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/mvn_full_covariance.py
--rw-r--r--   0 runner    (1001) docker     (123)     8854 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/mvn_full_covariance_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5329 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/mvn_kl_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/mvn_tri.py
--rw-r--r--   0 runner    (1001) docker     (123)    10705 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/mvn_tri_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/normal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/normal_float64_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9253 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/normal_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/one_hot_categorical.py
--rw-r--r--   0 runner    (1001) docker     (123)    18970 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/one_hot_categorical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13249 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/quantized.py
--rw-r--r--   0 runner    (1001) docker     (123)    17568 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/quantized_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/softmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/softmax_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/straight_through.py
--rw-r--r--   0 runner    (1001) docker     (123)     6977 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/straight_through_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/tfp_compatible_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)    11323 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/tfp_compatible_distribution_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12304 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/transformed.py
--rw-r--r--   0 runner    (1001) docker     (123)    19258 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/transformed_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/uniform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/uniform_float64_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/uniform_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    16897 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/von_mises.py
--rw-r--r--   0 runner    (1001) docker     (123)    20921 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/distributions/von_mises_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 11:03:14.296094 distrax-0.1.3/distrax/_src/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/utils/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/utils/conversion_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    14657 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/utils/equivalence.py
--rw-r--r--   0 runner    (1001) docker     (123)    11209 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/utils/hmm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/utils/hmm_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/utils/importance_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/utils/importance_sampling_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/utils/jittable.py
--rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/utils/jittable_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/utils/math.py
--rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/utils/math_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/utils/monte_carlo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/utils/monte_carlo_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12689 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/utils/transformations.py
--rw-r--r--   0 runner    (1001) docker     (123)     7340 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/_src/utils/transformations_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-02-14 11:03:02.000000 distrax-0.1.3/distrax/distrax_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 11:03:14.276094 distrax-0.1.3/distrax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13001 2023-02-14 11:03:14.000000 distrax-0.1.3/distrax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-02-14 11:03:14.000000 distrax-0.1.3/distrax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-14 11:03:14.000000 distrax-0.1.3/distrax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-14 11:03:14.000000 distrax-0.1.3/distrax.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-02-14 11:03:14.000000 distrax-0.1.3/distrax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-14 11:03:14.000000 distrax-0.1.3/distrax.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 11:03:14.296094 distrax-0.1.3/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-02-14 11:03:02.000000 distrax-0.1.3/examples/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    10805 2023-02-14 11:03:02.000000 distrax-0.1.3/examples/hmm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-02-14 11:03:02.000000 distrax-0.1.3/examples/vae.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 11:03:14.296094 distrax-0.1.3/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-02-14 11:03:02.000000 distrax-0.1.3/requirements/requirements-examples.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-14 11:03:02.000000 distrax-0.1.3/requirements/requirements-tests.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-02-14 11:03:02.000000 distrax-0.1.3/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-14 11:03:14.296094 distrax-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-02-14 11:03:02.000000 distrax-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:17:13.845530 distrax-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-29 14:17:01.000000 distrax-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-29 14:17:01.000000 distrax-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13001 2023-06-29 14:17:13.845530 distrax-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11984 2023-06-29 14:17:01.000000 distrax-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:17:13.817541 distrax-0.1.4/distrax/
+-rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:17:13.817541 distrax-0.1.4/distrax/_src/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:17:13.825538 distrax-0.1.4/distrax/_src/bijectors/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/bijectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7962 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/bijectors/bijector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/bijectors/bijector_from_tfp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9688 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/bijectors/bijector_from_tfp_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/bijectors/bijector_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/bijectors/block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/bijectors/block_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/bijectors/chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10931 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/bijectors/chain_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/bijectors/diag_linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7510 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/bijectors/diag_linear_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9422 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/bijectors/diag_plus_low_rank_linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10657 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/bijectors/diag_plus_low_rank_linear_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/bijectors/gumbel_cdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/bijectors/gumbel_cdf_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/bijectors/inverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9233 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/bijectors/inverse_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/bijectors/lambda_bijector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12944 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/bijectors/lambda_bijector_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/bijectors/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/bijectors/linear_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/bijectors/lower_upper_triangular_affine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8764 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/bijectors/lower_upper_triangular_affine_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/bijectors/masked_coupling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10755 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/bijectors/masked_coupling_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20159 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/bijectors/rational_quadratic_spline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/bijectors/rational_quadratic_spline_float64_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13180 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/bijectors/rational_quadratic_spline_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/bijectors/scalar_affine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/bijectors/scalar_affine_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/bijectors/shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/bijectors/shift_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/bijectors/sigmoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/bijectors/sigmoid_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/bijectors/split_coupling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10197 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/bijectors/split_coupling_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/bijectors/tanh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/bijectors/tanh_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/bijectors/tfp_compatible_bijector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14341 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/bijectors/tfp_compatible_bijector_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/bijectors/triangular_linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/bijectors/triangular_linear_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/bijectors/unconstrained_affine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8199 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/bijectors/unconstrained_affine_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:17:13.837533 distrax-0.1.4/distrax/_src/distributions/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/bernoulli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12888 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/bernoulli_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/beta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10372 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/beta_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7932 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22304 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/categorical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5844 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/categorical_uniform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13040 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/categorical_uniform_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5316 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/clipped.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7221 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/clipped_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/deterministic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9858 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/deterministic_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8014 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/dirichlet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10477 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/dirichlet_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11822 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/distribution_from_tfp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9828 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/distribution_from_tfp_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10098 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/distribution_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/epsilon_greedy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/epsilon_greedy_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/gamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8403 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/gamma_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/greedy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/greedy_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5251 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/gumbel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9401 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/gumbel_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/independent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16214 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/independent_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6079 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/joint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18728 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/joint_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/laplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11436 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/laplace_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/log_stddev_normal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/log_stddev_normal_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4319 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/logistic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7270 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/logistic_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/mixture_of_two.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/mixture_of_two_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/mixture_same_family.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12708 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/mixture_same_family_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11437 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/multinomial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21199 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/multinomial_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/mvn_diag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8441 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/mvn_diag_plus_low_rank.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15802 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/mvn_diag_plus_low_rank_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17753 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/mvn_diag_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9763 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/mvn_from_bijector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11596 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/mvn_from_bijector_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5028 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/mvn_full_covariance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8854 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/mvn_full_covariance_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5329 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/mvn_kl_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/mvn_tri.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10705 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/mvn_tri_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/normal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/normal_float64_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9253 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/normal_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/one_hot_categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18970 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/one_hot_categorical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13289 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/quantized.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/quantized_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/softmax_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/straight_through.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6977 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/straight_through_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/tfp_compatible_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11323 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/tfp_compatible_distribution_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12331 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/transformed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19258 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/transformed_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/uniform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/uniform_float64_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/uniform_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17000 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/von_mises.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20921 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/distributions/von_mises_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:17:13.841532 distrax-0.1.4/distrax/_src/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/utils/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/utils/conversion_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14630 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/utils/equivalence.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11202 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/utils/hmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/utils/hmm_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/utils/importance_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/utils/importance_sampling_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/utils/jittable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/utils/jittable_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/utils/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/utils/math_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/utils/monte_carlo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/utils/monte_carlo_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12689 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/utils/transformations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7340 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/_src/utils/transformations_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-29 14:17:01.000000 distrax-0.1.4/distrax/distrax_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:17:13.817541 distrax-0.1.4/distrax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13001 2023-06-29 14:17:13.000000 distrax-0.1.4/distrax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-06-29 14:17:13.000000 distrax-0.1.4/distrax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 14:17:13.000000 distrax-0.1.4/distrax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 14:17:13.000000 distrax-0.1.4/distrax.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-29 14:17:13.000000 distrax-0.1.4/distrax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-29 14:17:13.000000 distrax-0.1.4/distrax.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:17:13.841532 distrax-0.1.4/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-06-29 14:17:01.000000 distrax-0.1.4/examples/flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10805 2023-06-29 14:17:01.000000 distrax-0.1.4/examples/hmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-06-29 14:17:01.000000 distrax-0.1.4/examples/vae.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:17:13.841532 distrax-0.1.4/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-29 14:17:01.000000 distrax-0.1.4/requirements/requirements-examples.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-29 14:17:01.000000 distrax-0.1.4/requirements/requirements-tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-29 14:17:01.000000 distrax-0.1.4/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 14:17:13.845530 distrax-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-06-29 14:17:01.000000 distrax-0.1.4/setup.py
```

### Comparing `distrax-0.1.3/LICENSE` & `distrax-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/PKG-INFO` & `distrax-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: distrax
-Version: 0.1.3
+Version: 0.1.4
 Summary: Distrax: Probability distributions in JAX.
 Home-page: https://github.com/deepmind/distrax
 Author: DeepMind
 Author-email: distrax-dev@google.com
 License: Apache 2.0
 Keywords: jax probability distribution python machine learning
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,15 +15,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Distrax
 
 ![CI status](https://github.com/deepmind/distrax/workflows/tests/badge.svg)
 ![pypi](https://img.shields.io/pypi/v/distrax)
```

### Comparing `distrax-0.1.3/README.md` & `distrax-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/__init__.py` & `distrax-0.1.4/distrax/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 from distrax._src.utils.math import multiply_no_nan
 from distrax._src.utils.monte_carlo import estimate_kl_best_effort
 from distrax._src.utils.monte_carlo import mc_estimate_kl
 from distrax._src.utils.monte_carlo import mc_estimate_kl_with_reparameterized
 from distrax._src.utils.monte_carlo import mc_estimate_mode
 from distrax._src.utils.transformations import register_inverse
 
-__version__ = "0.1.3"
+__version__ = "0.1.4"
 
 __all__ = (
     "as_bijector",
     "as_distribution",
     "Bernoulli",
     "Beta",
     "Bijector",
```

### Comparing `distrax-0.1.3/distrax/_src/__init__.py` & `distrax-0.1.4/distrax/_src/__init__.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/bijectors/__init__.py` & `distrax-0.1.4/distrax/_src/bijectors/__init__.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/bijectors/bijector.py` & `distrax-0.1.4/distrax/_src/bijectors/bijector.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,22 +14,23 @@
 # ==============================================================================
 """Bijector abstract base class."""
 
 import abc
 import typing
 from typing import Callable, Optional, Tuple, Union
 
+import chex
 from distrax._src.utils import jittable
 import jax.numpy as jnp
 from tensorflow_probability.substrates import jax as tfp
 
 
 tfb = tfp.bijectors
 
-Array = jnp.ndarray
+Array = chex.Array
 
 
 class Bijector(jittable.Jittable, metaclass=abc.ABCMeta):
   """Differentiable bijection that knows to compute its Jacobian determinant.
 
   A bijector implements a differentiable and bijective transformation `f`, whose
   inverse is also differentiable (`f` is called a "diffeomorphism"). A bijector
```

### Comparing `distrax-0.1.3/distrax/_src/bijectors/bijector_from_tfp.py` & `distrax-0.1.4/distrax/_src/bijectors/bijector_from_tfp.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/bijectors/bijector_from_tfp_test.py` & `distrax-0.1.4/distrax/_src/bijectors/bijector_from_tfp_test.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/bijectors/bijector_test.py` & `distrax-0.1.4/distrax/_src/bijectors/bijector_test.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/bijectors/block.py` & `distrax-0.1.4/distrax/_src/bijectors/block.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/bijectors/block_test.py` & `distrax-0.1.4/distrax/_src/bijectors/block_test.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/bijectors/chain.py` & `distrax-0.1.4/distrax/_src/bijectors/chain.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/bijectors/chain_test.py` & `distrax-0.1.4/distrax/_src/bijectors/chain_test.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/bijectors/diag_linear.py` & `distrax-0.1.4/distrax/_src/bijectors/diag_linear.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/bijectors/diag_linear_test.py` & `distrax-0.1.4/distrax/_src/bijectors/diag_linear_test.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/bijectors/diag_plus_low_rank_linear.py` & `distrax-0.1.4/distrax/_src/bijectors/diag_plus_low_rank_linear.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/bijectors/diag_plus_low_rank_linear_test.py` & `distrax-0.1.4/distrax/_src/bijectors/diag_plus_low_rank_linear_test.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/bijectors/gumbel_cdf.py` & `distrax-0.1.4/distrax/_src/bijectors/gumbel_cdf.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/bijectors/gumbel_cdf_test.py` & `distrax-0.1.4/distrax/_src/bijectors/gumbel_cdf_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,15 +134,15 @@
     tfp_bijector = tfb.GumbelCDF()
 
     x = np.array([-10.0, -3.3, 0.0, 3.3, 10.0], dtype=np.float32)
     fldj = tfp_bijector.forward_log_det_jacobian(x, event_ndims=0)
     fldj_ = self.variant(bijector.forward_log_det_jacobian)(x)
     np.testing.assert_allclose(fldj_, fldj, rtol=RTOL)
 
-    y = bijector.forward(x)
+    y = bijector.forward(x)  # pytype: disable=wrong-arg-types  # jax-ndarray
     ildj = tfp_bijector.inverse_log_det_jacobian(y, event_ndims=0)
     ildj_ = self.variant(bijector.inverse_log_det_jacobian)(y)
     np.testing.assert_allclose(ildj_, ildj, rtol=RTOL)
 
   def test_jittable(self):
     @jax.jit
     def f(x, b):
```

### Comparing `distrax-0.1.3/distrax/_src/bijectors/inverse.py` & `distrax-0.1.4/distrax/_src/bijectors/inverse.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/bijectors/inverse_test.py` & `distrax-0.1.4/distrax/_src/bijectors/inverse_test.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/bijectors/lambda_bijector.py` & `distrax-0.1.4/distrax/_src/bijectors/lambda_bijector.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/bijectors/lambda_bijector_test.py` & `distrax-0.1.4/distrax/_src/bijectors/lambda_bijector_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -244,15 +244,15 @@
     tfp_bijector = tfp_bijector_fn()
 
     x = np.array([0.05, 0.3, 0.45], dtype=np.float32)
     fldj = tfp_bijector.forward_log_det_jacobian(x, event_ndims=0)
     fldj_ = self.variant(bijector.forward_log_det_jacobian)(x)
     np.testing.assert_allclose(fldj_, fldj, rtol=RTOL)
 
-    y = bijector.forward(x)
+    y = bijector.forward(x)  # pytype: disable=wrong-arg-types  # jax-ndarray
     ildj = tfp_bijector.inverse_log_det_jacobian(y, event_ndims=0)
     ildj_ = self.variant(bijector.inverse_log_det_jacobian)(y)
     np.testing.assert_allclose(ildj_, ildj, rtol=RTOL)
 
   @chex.all_variants
   @parameterized.named_parameters(_with_base_dists(
       ('identity', lambda x: x, tfb.Identity),
```

### Comparing `distrax-0.1.3/distrax/_src/bijectors/linear.py` & `distrax-0.1.4/distrax/_src/bijectors/linear.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/bijectors/linear_test.py` & `distrax-0.1.4/distrax/_src/bijectors/linear_test.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/bijectors/lower_upper_triangular_affine.py` & `distrax-0.1.4/distrax/_src/bijectors/lower_upper_triangular_affine.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/bijectors/lower_upper_triangular_affine_test.py` & `distrax-0.1.4/distrax/_src/bijectors/lower_upper_triangular_affine_test.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/bijectors/masked_coupling.py` & `distrax-0.1.4/distrax/_src/bijectors/masked_coupling.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/bijectors/masked_coupling_test.py` & `distrax-0.1.4/distrax/_src/bijectors/masked_coupling_test.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/bijectors/rational_quadratic_spline.py` & `distrax-0.1.4/distrax/_src/bijectors/rational_quadratic_spline.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/bijectors/rational_quadratic_spline_float64_test.py` & `distrax-0.1.4/distrax/_src/bijectors/rational_quadratic_spline_float64_test.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/bijectors/rational_quadratic_spline_test.py` & `distrax-0.1.4/distrax/_src/bijectors/rational_quadratic_spline_test.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/bijectors/scalar_affine.py` & `distrax-0.1.4/distrax/_src/bijectors/scalar_affine.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/bijectors/scalar_affine_test.py` & `distrax-0.1.4/distrax/_src/bijectors/scalar_affine_test.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/bijectors/shift.py` & `distrax-0.1.4/distrax/_src/bijectors/shift.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/bijectors/shift_test.py` & `distrax-0.1.4/distrax/_src/bijectors/shift_test.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/bijectors/sigmoid.py` & `distrax-0.1.4/distrax/_src/bijectors/sigmoid.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/bijectors/sigmoid_test.py` & `distrax-0.1.4/distrax/_src/bijectors/sigmoid_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,15 +133,15 @@
     tfp_bijector = tfb.Sigmoid()
 
     x = np.array([-10.0, -3.3, 0.0, 3.3, 10.0], dtype=np.float32)
     fldj = tfp_bijector.forward_log_det_jacobian(x, event_ndims=0)
     fldj_ = self.variant(bijector.forward_log_det_jacobian)(x)
     np.testing.assert_allclose(fldj_, fldj, rtol=RTOL)
 
-    y = bijector.forward(x)
+    y = bijector.forward(x)  # pytype: disable=wrong-arg-types  # jax-ndarray
     ildj = tfp_bijector.inverse_log_det_jacobian(y, event_ndims=0)
     ildj_ = self.variant(bijector.inverse_log_det_jacobian)(y)
     np.testing.assert_allclose(ildj_, ildj, rtol=RTOL)
 
   def test_jittable(self):
     @jax.jit
     def f(x, b):
```

### Comparing `distrax-0.1.3/distrax/_src/bijectors/split_coupling.py` & `distrax-0.1.4/distrax/_src/bijectors/split_coupling.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/bijectors/split_coupling_test.py` & `distrax-0.1.4/distrax/_src/bijectors/split_coupling_test.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/bijectors/tanh.py` & `distrax-0.1.4/distrax/_src/bijectors/tanh.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/bijectors/tanh_test.py` & `distrax-0.1.4/distrax/_src/bijectors/tanh_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -133,15 +133,15 @@
     tfp_bijector = tfb.Tanh()
 
     x = np.array([-10.0, -3.3, 0.0, 3.3, 10.0], dtype=np.float32)
     fldj = tfp_bijector.forward_log_det_jacobian(x, event_ndims=0)
     fldj_ = self.variant(bijector.forward_log_det_jacobian)(x)
     np.testing.assert_allclose(fldj_, fldj, rtol=RTOL)
 
-    y = bijector.forward(x)
+    y = bijector.forward(x)  # pytype: disable=wrong-arg-types  # jax-ndarray
     ildj = tfp_bijector.inverse_log_det_jacobian(y, event_ndims=0)
     ildj_ = self.variant(bijector.inverse_log_det_jacobian)(y)
     np.testing.assert_allclose(ildj_, ildj, rtol=RTOL)
 
   @chex.all_variants
   @parameterized.named_parameters(
       ('int16', np.array([0, 0], dtype=np.int16)),
```

### Comparing `distrax-0.1.3/distrax/_src/bijectors/tfp_compatible_bijector.py` & `distrax-0.1.4/distrax/_src/bijectors/tfp_compatible_bijector.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
       self.has_static_min_event_ndims = True
       self.forward_min_event_ndims = base_bijector.event_ndims_in
       self.inverse_min_event_ndims = base_bijector.event_ndims_out
 
     def __getattr__(self, name: str):
       return getattr(base_bijector, name)
 
-    def forward_and_log_det(self, x: Array) -> Array:
+    def forward_and_log_det(self, x: Array) -> Tuple[Array, Array]:
       """See `Bijector.forward_and_log_det`."""
       return base_bijector.forward_and_log_det(x)
 
     @property
     def name(self) -> str:
       """The name of the wrapped bijector."""
       return name_ or f"TFPCompatible{base_bijector.name}"
```

### Comparing `distrax-0.1.3/distrax/_src/bijectors/tfp_compatible_bijector_test.py` & `distrax-0.1.4/distrax/_src/bijectors/tfp_compatible_bijector_test.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/bijectors/triangular_linear.py` & `distrax-0.1.4/distrax/_src/bijectors/triangular_linear.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/bijectors/triangular_linear_test.py` & `distrax-0.1.4/distrax/_src/bijectors/triangular_linear_test.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/bijectors/unconstrained_affine.py` & `distrax-0.1.4/distrax/_src/bijectors/unconstrained_affine.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/bijectors/unconstrained_affine_test.py` & `distrax-0.1.4/distrax/_src/bijectors/unconstrained_affine_test.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/distributions/__init__.py` & `distrax-0.1.4/distrax/_src/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/distributions/bernoulli.py` & `distrax-0.1.4/distrax/_src/distributions/bernoulli.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 
 
 tfd = tfp.distributions
 
 Array = chex.Array
 Numeric = chex.Numeric
 PRNGKey = chex.PRNGKey
+EventT = distribution.EventT
 
 
 class Bernoulli(distribution.Distribution):
   """Bernoulli distribution.
 
   Bernoulli distribution with parameter `probs`, the probability of outcome `1`.
   """
@@ -108,37 +109,37 @@
     """See `Distribution._sample_n`."""
     probs = self.probs
     new_shape = (n,) + probs.shape
     uniform = jax.random.uniform(
         key=key, shape=new_shape, dtype=probs.dtype, minval=0., maxval=1.)
     return jnp.less(uniform, probs).astype(self._dtype)
 
-  def log_prob(self, value: Array) -> Array:
+  def log_prob(self, value: EventT) -> Array:
     """See `Distribution.log_prob`."""
     log_probs0, log_probs1 = self._log_probs_parameter()
     return (math.multiply_no_nan(log_probs0, 1 - value) +
             math.multiply_no_nan(log_probs1, value))
 
-  def prob(self, value: Array) -> Array:
+  def prob(self, value: EventT) -> Array:
     """See `Distribution.prob`."""
     probs1 = self.probs
     probs0 = 1 - probs1
     return (math.multiply_no_nan(probs0, 1 - value) +
             math.multiply_no_nan(probs1, value))
 
-  def cdf(self, value: Array) -> Array:
+  def cdf(self, value: EventT) -> Array:
     """See `Distribution.cdf`."""
     # For value < 0 the output should be zero because support = {0, 1}.
     return jnp.where(value < 0,
                      jnp.array(0., dtype=self.probs.dtype),
                      jnp.where(value >= 1,
                                jnp.array(1.0, dtype=self.probs.dtype),
                                1 - self.probs))
 
-  def log_cdf(self, value: Array) -> Array:
+  def log_cdf(self, value: EventT) -> Array:
     """See `Distribution.log_cdf`."""
     return jnp.log(self.cdf(value))
 
   def entropy(self) -> Array:
     """See `Distribution.entropy`."""
     (probs0, probs1,
      log_probs0, log_probs1) = _probs_and_log_probs(self)
@@ -168,16 +169,16 @@
 
 def _probs_and_log_probs(
     dist: Union[Bernoulli, tfd.Bernoulli]
     ) -> Tuple[Array, Array, Array, Array]:
   """Calculates both `probs` and `log_probs`."""
   # pylint: disable=protected-access
   if dist._logits is None:
-    probs0 = 1 - dist._probs
-    probs1 = dist._probs
+    probs0 = 1. - dist._probs
+    probs1 = 1. - probs0
     log_probs0 = jnp.log1p(-1. * dist._probs)
     log_probs1 = jnp.log(dist._probs)
   else:
     probs0 = jax.nn.sigmoid(-1. * dist._logits)
     probs1 = jax.nn.sigmoid(dist._logits)
     log_probs0 = -jax.nn.softplus(dist._logits)
     log_probs1 = -jax.nn.softplus(-1. * dist._logits)
```

### Comparing `distrax-0.1.3/distrax/_src/distributions/bernoulli_test.py` & `distrax-0.1.4/distrax/_src/distributions/bernoulli_test.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/distributions/beta.py` & `distrax-0.1.4/distrax/_src/distributions/beta.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 from tensorflow_probability.substrates import jax as tfp
 
 tfd = tfp.distributions
 
 Array = chex.Array
 Numeric = chex.Numeric
 PRNGKey = chex.PRNGKey
+EventT = distribution.EventT
 
 
 class Beta(distribution.Distribution):
   """Beta distribution with parameters `alpha` and `beta`.
 
   The PDF of a Beta distributed random variable `X` is defined on the interval
   `0 <= X <= 1` and has the form:
@@ -86,31 +87,31 @@
     """See `Distribution._sample_n`."""
     out_shape = (n,) + self.batch_shape
     dtype = jnp.result_type(self._alpha, self._beta)
     rnd = jax.random.beta(
         key, a=self._alpha, b=self._beta, shape=out_shape, dtype=dtype)
     return rnd
 
-  def log_prob(self, value: Array) -> Array:
+  def log_prob(self, value: EventT) -> Array:
     """See `Distribution.log_prob`."""
     result = ((self._alpha - 1.) * jnp.log(value)
               + (self._beta - 1.) * jnp.log(1. - value)
               - self._log_normalization_constant)
     return jnp.where(
         jnp.logical_or(jnp.logical_and(self._alpha == 1., value == 0.),
                        jnp.logical_and(self._beta == 1., value == 1.)),
         -self._log_normalization_constant,
         result
     )
 
-  def cdf(self, value: Array) -> Array:
+  def cdf(self, value: EventT) -> Array:
     """See `Distribution.cdf`."""
     return jax.scipy.special.betainc(self._alpha, self._beta, value)
 
-  def log_cdf(self, value: Array) -> Array:
+  def log_cdf(self, value: EventT) -> Array:
     """See `Distribution.log_cdf`."""
     return jnp.log(self.cdf(value))
 
   def entropy(self) -> Array:
     """Calculates the Shannon entropy (in nats)."""
     return (
         self._log_normalization_constant
```

### Comparing `distrax-0.1.3/distrax/_src/distributions/beta_test.py` & `distrax-0.1.4/distrax/_src/distributions/beta_test.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/distributions/categorical.py` & `distrax-0.1.4/distrax/_src/distributions/categorical.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 import jax.numpy as jnp
 from tensorflow_probability.substrates import jax as tfp
 
 tfd = tfp.distributions
 
 Array = chex.Array
 PRNGKey = chex.PRNGKey
+EventT = distribution.EventT
 
 
 class Categorical(distribution.Distribution):
   """Categorical distribution."""
 
   equiv_tfp_cls = tfd.Categorical
 
@@ -93,26 +94,28 @@
     new_shape = (n,) + self.logits.shape[:-1]
     is_valid = jnp.logical_and(jnp.all(jnp.isfinite(self.probs), axis=-1),
                                jnp.all(self.probs >= 0, axis=-1))
     draws = jax.random.categorical(key=key, logits=self.logits, axis=-1,
                                    shape=new_shape).astype(self._dtype)
     return jnp.where(is_valid, draws, jnp.ones_like(draws) * -1)
 
-  def log_prob(self, value: Array) -> Array:
+  def log_prob(self, value: EventT) -> Array:
     """See `Distribution.log_prob`."""
-    value_one_hot = jax.nn.one_hot(value, self.num_categories)
+    value_one_hot = jax.nn.one_hot(
+        value, self.num_categories, dtype=self.logits.dtype)
     mask_outside_domain = jnp.logical_or(
         value < 0, value > self.num_categories - 1)
     return jnp.where(
         mask_outside_domain, -jnp.inf,
         jnp.sum(math.multiply_no_nan(self.logits, value_one_hot), axis=-1))
 
-  def prob(self, value: Array) -> Array:
+  def prob(self, value: EventT) -> Array:
     """See `Distribution.prob`."""
-    value_one_hot = jax.nn.one_hot(value, self.num_categories)
+    value_one_hot = jax.nn.one_hot(
+        value, self.num_categories, dtype=self.probs.dtype)
     return jnp.sum(math.multiply_no_nan(self.probs, value_one_hot), axis=-1)
 
   def entropy(self) -> Array:
     """See `Distribution.entropy`."""
     if self._logits is None:
       log_probs = jnp.log(self._probs)
     else:
@@ -120,30 +123,31 @@
     return -jnp.sum(math.mul_exp(log_probs, log_probs), axis=-1)
 
   def mode(self) -> Array:
     """See `Distribution.mode`."""
     parameter = self._probs if self._logits is None else self._logits
     return jnp.argmax(parameter, axis=-1).astype(self._dtype)
 
-  def cdf(self, value: Array) -> Array:
+  def cdf(self, value: EventT) -> Array:
     """See `Distribution.cdf`."""
     # For value < 0 the output should be zero because support = {0, ..., K-1}.
     should_be_zero = value < 0
     # For value >= K-1 the output should be one. Explicitly accounting for this
     # case addresses potential numerical issues that may arise when evaluating
     # derived methods (mainly, `log_survival_function`) for `value >= K-1`.
     should_be_one = value >= self.num_categories - 1
     # Will use value as an index below, so clip it to {0, ..., K-1}.
     value = jnp.clip(value, 0, self.num_categories - 1)
-    value_one_hot = jax.nn.one_hot(value, self.num_categories)
+    value_one_hot = jax.nn.one_hot(
+        value, self.num_categories, dtype=self.probs.dtype)
     cdf = jnp.sum(math.multiply_no_nan(
         jnp.cumsum(self.probs, axis=-1), value_one_hot), axis=-1)
     return jnp.where(should_be_zero, 0., jnp.where(should_be_one, 1., cdf))
 
-  def log_cdf(self, value: Array) -> Array:
+  def log_cdf(self, value: EventT) -> Array:
     """See `Distribution.log_cdf`."""
     return jnp.log(self.cdf(value))
 
   def logits_parameter(self) -> Array:
     """Wrapper for `logits` property, for TFP API compatibility."""
     return self.logits
```

### Comparing `distrax-0.1.3/distrax/_src/distributions/categorical_test.py` & `distrax-0.1.4/distrax/_src/distributions/categorical_test.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/distributions/categorical_uniform.py` & `distrax-0.1.4/distrax/_src/distributions/categorical_uniform.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 import jax
 import jax.numpy as jnp
 
 
 Array = chex.Array
 Numeric = chex.Numeric
 PRNGKey = chex.PRNGKey
+EventT = distribution.EventT
 
 
 class CategoricalUniform(distribution.Distribution):
   """Mixture Categorical-Uniform distribution.
 
   Given an interval `[a, b]` and a probability vector `p = [p_1, ..., p_K]`, a
   random variable `x` follows a Categorical-Uniform distribution if its PDF
@@ -82,15 +83,15 @@
         self._low.shape, self._high.shape, self._logits.shape[:-1])
 
   def _sample_n(self, key: PRNGKey, n: int) -> Array:
     """See `Distribution._sample_n`."""
     quantile = jax.random.uniform(key, (n,) + self.batch_shape)
     return self._inverse_cdf(quantile)
 
-  def log_prob(self, value: Array) -> Array:
+  def log_prob(self, value: EventT) -> Array:
     """See `Distribution.log_prob`."""
     return self._get_mixture().log_prob(value)
 
   def entropy(self) -> Array:
     """See `Distribution.entropy`."""
     # The following holds because the components have non-overlapping domains.
     mixture = self._get_mixture()
```

### Comparing `distrax-0.1.3/distrax/_src/distributions/categorical_uniform_test.py` & `distrax-0.1.4/distrax/_src/distributions/categorical_uniform_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,15 +123,17 @@
 )
 
 
 class CategoricalUniformTest(parameterized.TestCase):
 
   def test_raises_on_wrong_logits(self):
     with self.assertRaises(ValueError):
-      categorical_uniform.CategoricalUniform(low=0., high=1., logits=0.)
+      categorical_uniform.CategoricalUniform(
+          low=0.0, high=1.0, logits=jnp.array(0.0)
+      )
 
   @parameterized.named_parameters(*_NAMED_PARAMETERS)
   def test_batch_shape(self, *, low, high, logits, target_batch_shape, **_):
     distribution = categorical_uniform.CategoricalUniform(
         low=low, high=high, logits=logits)
     self.assertEqual(distribution.batch_shape, target_batch_shape)
```

### Comparing `distrax-0.1.3/distrax/_src/distributions/clipped.py` & `distrax-0.1.4/distrax/_src/distributions/clipped.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 import jax.numpy as jnp
 
 
 Array = chex.Array
 PRNGKey = chex.PRNGKey
 Numeric = chex.Numeric
 DistributionLike = base_distribution.DistributionLike
+EventT = base_distribution.EventT
 
 
 class Clipped(base_distribution.Distribution):
   """A clipped distribution."""
 
   def __init__(
       self,
@@ -71,15 +72,15 @@
     return jnp.clip(raw_sample, self._minimum, self._maximum)
 
   def _sample_n_and_log_prob(self, key: PRNGKey, n: int) -> Tuple[Array, Array]:
     """See `Distribution._sample_n_and_log_prob`."""
     samples = self._sample_n(key, n)
     return samples, self.log_prob(samples)
 
-  def log_prob(self, value: Array) -> Array:
+  def log_prob(self, value: EventT) -> Array:
     """See `Distribution.log_prob`."""
     # The log_prob can be used to compute expectations by explicitly integrating
     # over the discrete and continuous elements.
     # Info about mixed distributions:
     # http://www.randomservices.org/random/dist/Mixed.html
     log_prob = jnp.where(
         jnp.equal(value, self._minimum),
@@ -90,19 +91,19 @@
     # Giving -inf log_prob outside the boundaries.
     return jnp.where(
         jnp.logical_or(value < self._minimum, value > self._maximum),
         -jnp.inf,
         log_prob)
 
   @property
-  def minimum(self) -> Numeric:
+  def minimum(self) -> Array:
     return self._minimum
 
   @property
-  def maximum(self) -> Numeric:
+  def maximum(self) -> Array:
     return self._maximum
 
   @property
   def distribution(self) -> DistributionLike:
     return self._distribution
 
   @property
```

### Comparing `distrax-0.1.3/distrax/_src/distributions/clipped_test.py` & `distrax-0.1.4/distrax/_src/distributions/clipped_test.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/distributions/deterministic.py` & `distrax-0.1.4/distrax/_src/distributions/deterministic.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 
 
 tfd = tfp.distributions
 
 Array = chex.Array
 Numeric = chex.Numeric
 PRNGKey = chex.PRNGKey
+EventT = distribution.EventT
 
 
 class Deterministic(distribution.Distribution):
   """Scalar Deterministic distribution on the real line."""
 
   equiv_tfp_cls = tfd.Deterministic
 
@@ -102,19 +103,19 @@
 
   def _sample_n_and_log_prob(self, key: PRNGKey, n: int) -> Tuple[Array, Array]:
     """See `Distribution._sample_n_and_log_prob`."""
     samples = self._sample_n(key, n)
     log_prob = jnp.zeros_like(samples)
     return samples, log_prob
 
-  def log_prob(self, value: Array) -> Array:
+  def log_prob(self, value: EventT) -> Array:
     """See `Distribution.log_prob`."""
     return jnp.log(self.prob(value))
 
-  def prob(self, value: Array) -> Array:
+  def prob(self, value: EventT) -> Array:
     """See `Distribution.prob`."""
     return jnp.where(
         jnp.abs(value - self.loc) <= self.slack, 1., 0.)
 
   def entropy(self) -> Array:
     """Calculates the Shannon entropy (in nats)."""
     return jnp.zeros(self.batch_shape, jnp.float_)
@@ -131,19 +132,19 @@
     """Calculates the variance."""
     return jnp.zeros(self.batch_shape, jnp.float_)
 
   def stddev(self) -> Array:
     """Calculates the standard deviation."""
     return self.variance()
 
-  def log_cdf(self, value: Array) -> Array:
+  def log_cdf(self, value: EventT) -> Array:
     """See `Distribution.log_cdf`."""
     return jnp.log(self.cdf(value))
 
-  def cdf(self, value: Array) -> Array:
+  def cdf(self, value: EventT) -> Array:
     """See `Distribution.cdf`."""
     return jnp.where(value >= self.loc - self.slack, 1., 0.)
 
   def __getitem__(self, index) -> 'Deterministic':
     """See `Distribution.__getitem__`."""
     index = distribution.to_batch_shape_index(self.batch_shape, index)
     return Deterministic(
```

### Comparing `distrax-0.1.3/distrax/_src/distributions/deterministic_test.py` & `distrax-0.1.4/distrax/_src/distributions/deterministic_test.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/distributions/dirichlet.py` & `distrax-0.1.4/distrax/_src/distributions/dirichlet.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 from tensorflow_probability.substrates import jax as tfp
 
 tfd = tfp.distributions
 
 Array = chex.Array
 Numeric = chex.Numeric
 PRNGKey = chex.PRNGKey
+EventT = distribution.EventT
 
 
 class Dirichlet(distribution.Distribution):
   """Dirichlet distribution with concentration parameter `alpha`.
 
   The PDF of a Dirichlet distributed random variable `X`, where `X` lives in the
   simplex `(0, 1)^K` with `sum_{k=1}^{K} X_k = 1`, is given by,
@@ -88,15 +89,15 @@
     """See `Distribution._sample_n`."""
     out_shape = (n,) + self.batch_shape
     dtype = self._concentration.dtype
     rnd = jax.random.dirichlet(
         key, alpha=self._concentration, shape=out_shape, dtype=dtype)
     return rnd
 
-  def log_prob(self, value: Array) -> Array:
+  def log_prob(self, value: EventT) -> Array:
     """See `Distribution.log_prob`."""
     return (jnp.sum((self._concentration - 1.) * jnp.log(value), axis=-1)
             - self._log_normalization_constant)
 
   def entropy(self) -> Array:
     """Calculates the Shannon entropy (in nats)."""
     sum_concentration = jnp.sum(self._concentration, axis=-1)
```

### Comparing `distrax-0.1.3/distrax/_src/distributions/dirichlet_test.py` & `distrax-0.1.4/distrax/_src/distributions/dirichlet_test.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/distributions/distribution.py` & `distrax-0.1.4/distrax/_src/distributions/distribution.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 Array = chex.Array
 PRNGKey = chex.PRNGKey
 IntLike = Union[int, np.int16, np.int32, np.int64]
 # Generic type.
 T = TypeVar('T')
 # Generic nested type.
-NestedT = Union[T, Iterable['NestedT'], Mapping[Any, 'NestedT']]
+NestedT = Union[T, Iterable['NestedT'], Mapping[Any, 'NestedT']]  # pylint: disable=invalid-name
 # Nested types.
 EventT = TypeVar('EventT', bound=NestedT[Array])
 ShapeT = TypeVar('ShapeT', bound=NestedT[Tuple[int, ...]])
 DTypeT = TypeVar('DTypeT', bound=NestedT[jnp.dtype])
 
 
 class Distribution(
@@ -315,15 +315,15 @@
 ) -> Tuple[PRNGKey, Tuple[int, ...]]:
   """Shared functionality to ensure that seeds and shapes are the right type."""
 
   if not isinstance(sample_shape, collections.abc.Sequence):
     sample_shape = (sample_shape,)
   sample_shape = tuple(map(int, sample_shape))
 
-  if isinstance(seed, IntLike.__args__):
+  if isinstance(seed, (int, np.signedinteger)):
     rng = jax.random.PRNGKey(seed)
   else:  # key is of type PRNGKey
     rng = seed
 
   return rng, sample_shape
```

### Comparing `distrax-0.1.3/distrax/_src/distributions/distribution_from_tfp.py` & `distrax-0.1.4/distrax/_src/distributions/distribution_from_tfp.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from tensorflow_probability.substrates import jax as tfp
 
 tfd = tfp.distributions
 
 Array = chex.Array
 PRNGKey = chex.PRNGKey
 DistributionT = distribution.DistributionT
+EventT = distribution.EventT
 
 
 def distribution_from_tfp(tfp_distribution: tfd.Distribution) -> DistributionT:
   """Create a Distrax distribution from a TFP distribution.
 
   Given a TFP distribution `tfp_distribution`, this method returns a
   distribution of a class that inherits from the class of `tfp_distribution`.
@@ -65,19 +66,19 @@
 
     def _sample_n(self, key: PRNGKey, n: int):
       """See `Distribution._sample_n`."""
       return jnp.asarray(
           tfp_distribution.sample(seed=key, sample_shape=(n,)),
           dtype=tfp_distribution.dtype)
 
-    def log_prob(self, value: Array) -> Array:
+    def log_prob(self, value: EventT) -> Array:
       """See `Distribution.log_prob`."""
       return jnp.asarray(tfp_distribution.log_prob(value))
 
-    def prob(self, value: Array) -> Array:
+    def prob(self, value: EventT) -> Array:
       """See `Distribution.prob`."""
       return jnp.asarray(tfp_distribution.prob(value))
 
     @property
     def event_shape(self) -> Tuple[int, ...]:
       """See `Distribution.event_shape`."""
       return tuple(tfp_distribution.event_shape)
@@ -102,19 +103,19 @@
       return jnp.asarray(
           tfd.kullback_leibler.kl_divergence(self, other_dist, *args, **kwargs))
 
     def entropy(self) -> Array:
       """See `Distribution.entropy`."""
       return jnp.asarray(tfp_distribution.entropy())
 
-    def log_cdf(self, value: Array) -> Array:
+    def log_cdf(self, value: EventT) -> Array:
       """See `Distribution.log_cdf`."""
       return jnp.asarray(tfp_distribution.log_cdf(value))
 
-    def cdf(self, value: Array) -> Array:
+    def cdf(self, value: EventT) -> Array:
       """See `Distribution.cdf`."""
       return jnp.asarray(tfp_distribution.cdf(value))
 
     def mean(self) -> Array:
       """See `Distribution.mean`."""
       return jnp.asarray(tfp_distribution.mean())
```

### Comparing `distrax-0.1.3/distrax/_src/distributions/distribution_from_tfp_test.py` & `distrax-0.1.4/distrax/_src/distributions/distribution_from_tfp_test.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/distributions/distribution_test.py` & `distrax-0.1.4/distrax/_src/distributions/distribution_test.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/distributions/epsilon_greedy.py` & `distrax-0.1.4/distrax/_src/distributions/epsilon_greedy.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/distributions/epsilon_greedy_test.py` & `distrax-0.1.4/distrax/_src/distributions/epsilon_greedy_test.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/distributions/gamma.py` & `distrax-0.1.4/distrax/_src/distributions/gamma.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 from tensorflow_probability.substrates import jax as tfp
 
 tfd = tfp.distributions
 
 Array = chex.Array
 Numeric = chex.Numeric
 PRNGKey = chex.PRNGKey
+EventT = distribution.EventT
 
 
 class Gamma(distribution.Distribution):
   """Gamma distribution with parameters `concentration` and `rate`."""
 
   equiv_tfp_cls = tfd.Gamma
 
@@ -76,15 +77,15 @@
     )
 
   def _sample_n(self, key: PRNGKey, n: int) -> Array:
     """See `Distribution._sample_n`."""
     rnd = self._sample_from_std_gamma(key, n)
     return rnd / self._rate
 
-  def log_prob(self, value: Array) -> Array:
+  def log_prob(self, value: EventT) -> Array:
     """See `Distribution.log_prob`."""
     return (
         self._concentration * jnp.log(self._rate)
         + (self._concentration - 1) * jnp.log(value)
         - self._rate * value
         - jax.lax.lgamma(self._concentration)
     )
@@ -95,19 +96,19 @@
     return (
         self._concentration
         - log_rate
         + jax.lax.lgamma(self._concentration)
         + (1.0 - self._concentration) * jax.lax.digamma(self._concentration)
     )
 
-  def cdf(self, value: Array) -> Array:
+  def cdf(self, value: EventT) -> Array:
     """See `Distribution.cdf`."""
     return jax.lax.igamma(self._concentration, self._rate * value)
 
-  def log_cdf(self, value: Array) -> Array:
+  def log_cdf(self, value: EventT) -> Array:
     """See `Distribution.log_cdf`."""
     return jnp.log(self.cdf(value))
 
   def mean(self) -> Array:
     """Calculates the mean."""
     return self._concentration / self._rate
```

### Comparing `distrax-0.1.3/distrax/_src/distributions/gamma_test.py` & `distrax-0.1.4/distrax/_src/distributions/gamma_test.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/distributions/greedy.py` & `distrax-0.1.4/distrax/_src/distributions/greedy.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/distributions/greedy_test.py` & `distrax-0.1.4/distrax/_src/distributions/greedy_test.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/distributions/gumbel.py` & `distrax-0.1.4/distrax/_src/distributions/gumbel.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 from tensorflow_probability.substrates import jax as tfp
 
 tfd = tfp.distributions
 
 Array = chex.Array
 Numeric = chex.Numeric
 PRNGKey = chex.PRNGKey
+EventT = distribution.EventT
 
 
 class Gumbel(distribution.Distribution):
   """Gumbel distribution with location `loc` and `scale` parameters."""
 
   equiv_tfp_cls = tfd.Gumbel
 
@@ -69,15 +70,15 @@
     """Scale of the distribution."""
     return jnp.broadcast_to(self._scale, self.batch_shape)
 
   def _standardize(self, value: Array) -> Array:
     """Standardizes the input `value` in location and scale."""
     return (value - self._loc) / self._scale
 
-  def log_prob(self, value: Array) -> Array:
+  def log_prob(self, value: EventT) -> Array:
     """See `Distribution.log_prob`."""
     z = self._standardize(value)
     return -(z + jnp.exp(-z)) - jnp.log(self._scale)
 
   def _sample_from_std_gumbel(self, key: PRNGKey, n: int) -> Array:
     out_shape = (n,) + self.batch_shape
     dtype = jnp.result_type(self._loc, self._scale)
@@ -95,15 +96,15 @@
     log_prob = -(rnd + jnp.exp(-rnd)) - jnp.log(self._scale)
     return samples, log_prob
 
   def entropy(self) -> Array:
     """Calculates the Shannon entropy (in nats)."""
     return jnp.log(self._scale) + 1. + jnp.euler_gamma
 
-  def log_cdf(self, value: Array) -> Array:
+  def log_cdf(self, value: EventT) -> Array:
     """See `Distribution.log_cdf`."""
     z = self._standardize(value)
     return -jnp.exp(-z)
 
   def mean(self) -> Array:
     """Calculates the mean."""
     return self._loc + self._scale * jnp.euler_gamma
```

### Comparing `distrax-0.1.3/distrax/_src/distributions/gumbel_test.py` & `distrax-0.1.4/distrax/_src/distributions/gumbel_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -166,48 +166,52 @@
       ('kl distrax_to_tfp', 'kl_divergence', 'distrax_to_tfp'),
       ('kl tfp_to_distrax', 'kl_divergence', 'tfp_to_distrax'),
       ('cross-ent distrax_to_distrax', 'cross_entropy', 'distrax_to_distrax'),
       ('cross-ent distrax_to_tfp', 'cross_entropy', 'distrax_to_tfp'),
       ('cross-ent tfp_to_distrax', 'cross_entropy', 'tfp_to_distrax')
   )
   def test_with_two_distributions(self, function_string, mode_string):
+    rng = np.random.default_rng(2023)
     super()._test_with_two_distributions(
         attribute_string=function_string,
         mode_string=mode_string,
         dist1_kwargs={
-            'loc': np.array(np.random.randn(4, 1, 2), dtype=np.float32),
+            'loc': rng.normal(size=(4, 1, 2)).astype(np.float32),
             'scale': np.array([[0.8, 0.2], [0.1, 1.2], [1.4, 3.1]],
                               dtype=np.float32),
         },
         dist2_kwargs={
-            'loc': np.array(np.random.randn(3, 2), dtype=np.float32),
-            'scale': 0.1 + np.array(np.random.rand(4, 1, 2), dtype=np.float32),
+            'loc': rng.normal(size=(3, 2)).astype(np.float32),
+            'scale': 0.1 + np.array(rng.uniform(size=(4, 1, 2)),
+                                    dtype=np.float32),
         },
         assertion_fn=self.assertion_fn(rtol=6e-2))
 
   def test_jittable(self):
     super()._test_jittable(
         (0.1, 1.2), assertion_fn=self.assertion_fn(rtol=3e-2))
 
   @parameterized.named_parameters(
       ('single element', 2),
       ('range', slice(-1)),
       ('range_2', (slice(None), slice(-1))),
       ('ellipsis', (Ellipsis, -1)),
   )
   def test_slice(self, slice_):
-    loc = jnp.array(np.random.randn(3, 4, 5))
-    scale = jnp.array(0.1 + np.random.rand(3, 4, 5))
+    rng = np.random.default_rng(2023)
+    loc = jnp.array(rng.normal(size=(3, 4, 5)))
+    scale = jnp.array(0.1 + rng.uniform(size=(3, 4, 5)))
     dist = self.distrax_cls(loc=loc, scale=scale)
     self.assertion_fn(rtol=3e-2)(dist[slice_].loc, loc[slice_])
     self.assertion_fn(rtol=3e-2)(dist[slice_].scale, scale[slice_])
 
   def test_slice_different_parameterization(self):
-    loc = jnp.array(np.random.randn(4))
-    scale = jnp.array(0.1 + np.random.rand(3, 4))
+    rng = np.random.default_rng(2023)
+    loc = jnp.array(rng.normal(size=(4,)))
+    scale = jnp.array(0.1 + rng.uniform(size=(3, 4)))
     dist = self.distrax_cls(loc=loc, scale=scale)
     self.assertion_fn(rtol=3e-2)(dist[0].loc, loc)  # Not slicing loc.
     self.assertion_fn(rtol=3e-2)(dist[0].scale, scale[0])
 
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `distrax-0.1.3/distrax/_src/distributions/independent.py` & `distrax-0.1.4/distrax/_src/distributions/independent.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
 
 tfd = tfp.distributions
 
 Array = chex.Array
 PRNGKey = chex.PRNGKey
 DistributionLike = distrax_distribution.DistributionLike
+EventT = distrax_distribution.EventT
 
 
 class Independent(distrax_distribution.Distribution):
   """Independent distribution obtained from child distributions."""
 
   equiv_tfp_cls = tfd.Independent
 
@@ -101,23 +102,23 @@
   def _sample_n_and_log_prob(self, key: PRNGKey, n: int) -> Tuple[Array, Array]:
     """See `Distribution._sample_n_and_log_prob`."""
     samples, log_prob = self._distribution.sample_and_log_prob(
         seed=key, sample_shape=n)
     log_prob = self._reduce(jnp.sum, log_prob)
     return samples, log_prob
 
-  def log_prob(self, value: Array) -> Array:
+  def log_prob(self, value: EventT) -> Array:
     """See `Distribution.log_prob`."""
     return self._reduce(jnp.sum, self._distribution.log_prob(value))
 
   def entropy(self) -> Array:
     """See `Distribution.entropy`."""
     return self._reduce(jnp.sum, self._distribution.entropy())
 
-  def log_cdf(self, value: Array) -> Array:
+  def log_cdf(self, value: EventT) -> Array:
     """See `Distribution.log_cdf`."""
     return self._reduce(jnp.sum, self._distribution.log_cdf(value))
 
   def mean(self) -> Array:
     """Calculates the mean."""
     return self._distribution.mean()
```

### Comparing `distrax-0.1.3/distrax/_src/distributions/independent_test.py` & `distrax-0.1.4/distrax/_src/distributions/independent_test.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/distributions/joint.py` & `distrax-0.1.4/distrax/_src/distributions/joint.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/distributions/joint_test.py` & `distrax-0.1.4/distrax/_src/distributions/joint_test.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/distributions/laplace.py` & `distrax-0.1.4/distrax/_src/distributions/laplace.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 from tensorflow_probability.substrates import jax as tfp
 
 tfd = tfp.distributions
 
 Array = chex.Array
 Numeric = chex.Numeric
 PRNGKey = chex.PRNGKey
+EventT = distribution.EventT
 
 
 class Laplace(distribution.Distribution):
   """Laplace distribution with location `loc` and `scale` parameters."""
 
   equiv_tfp_cls = tfd.Laplace
 
@@ -82,32 +83,32 @@
   def _sample_n_and_log_prob(self, key: PRNGKey, n: int) -> Tuple[Array, Array]:
     """See `Distribution._sample_n_and_log_prob`."""
     rnd = self._sample_from_std_laplace(key, n)
     samples = self._loc + self._scale * rnd
     log_prob = -jnp.abs(rnd) - math.log(2.) - jnp.log(self._scale)
     return samples, log_prob
 
-  def log_prob(self, value: Array) -> Array:
+  def log_prob(self, value: EventT) -> Array:
     """See `Distribution.log_prob`."""
     norm_value = self._standardize(value)
     return -jnp.abs(norm_value) - math.log(2.) - jnp.log(self._scale)
 
   def entropy(self) -> Array:
     """Calculates the Shannon entropy (in nats)."""
     return math.log(2.) + 1. + jnp.log(self.scale)
 
-  def cdf(self, value: Array) -> Array:
+  def cdf(self, value: EventT) -> Array:
     """See `Distribution.cdf`."""
     norm_value = self._standardize(value)
     return 0.5 - 0.5 * jnp.sign(norm_value) * jnp.expm1(-jnp.abs(norm_value))
 
   def _standardize(self, value: Array) -> Array:
     return (value - self._loc) / self._scale
 
-  def log_cdf(self, value: Array) -> Array:
+  def log_cdf(self, value: EventT) -> Array:
     """See `Distribution.log_cdf`."""
     norm_value = self._standardize(value)
     lower_value = norm_value - math.log(2.)
     exp_neg_norm_value = jnp.exp(-jnp.abs(norm_value))
     upper_value = jnp.log1p(-0.5 * exp_neg_norm_value)
     return jnp.where(jnp.less_equal(norm_value, 0.), lower_value, upper_value)
```

### Comparing `distrax-0.1.3/distrax/_src/distributions/laplace_test.py` & `distrax-0.1.4/distrax/_src/distributions/laplace_test.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/distributions/log_stddev_normal.py` & `distrax-0.1.4/distrax/_src/distributions/log_stddev_normal.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/distributions/log_stddev_normal_test.py` & `distrax-0.1.4/distrax/_src/distributions/log_stddev_normal_test.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/distributions/logistic.py` & `distrax-0.1.4/distrax/_src/distributions/logistic.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 from tensorflow_probability.substrates import jax as tfp
 
 tfd = tfp.distributions
 
 Array = chex.Array
 Numeric = chex.Numeric
 PRNGKey = chex.PRNGKey
+EventT = distribution.EventT
 
 
 class Logistic(distribution.Distribution):
   """The Logistic distribution with location `loc` and `scale` parameters."""
 
   equiv_tfp_cls = tfd.Logistic
 
@@ -80,36 +81,36 @@
         shape=out_shape,
         dtype=dtype,
         minval=jnp.finfo(dtype).tiny,
         maxval=1.)
     rnd = jnp.log(uniform) - jnp.log1p(-uniform)
     return self._scale * rnd + self._loc
 
-  def log_prob(self, value: Array) -> Array:
+  def log_prob(self, value: EventT) -> Array:
     """See `Distribution.log_prob`."""
     z = self._standardize(value)
     return -z - 2. * jax.nn.softplus(-z) - jnp.log(self._scale)
 
   def entropy(self) -> Array:
     """Calculates the Shannon entropy (in Nats)."""
     return 2. + jnp.broadcast_to(jnp.log(self._scale), self.batch_shape)
 
-  def cdf(self, value: Array) -> Array:
+  def cdf(self, value: EventT) -> Array:
     """See `Distribution.cdf`."""
     return jax.nn.sigmoid(self._standardize(value))
 
-  def log_cdf(self, value: Array) -> Array:
+  def log_cdf(self, value: EventT) -> Array:
     """See `Distribution.log_cdf`."""
     return -jax.nn.softplus(-self._standardize(value))
 
-  def survival_function(self, value: Array) -> Array:
+  def survival_function(self, value: EventT) -> Array:
     """See `Distribution.survival_function`."""
     return jax.nn.sigmoid(-self._standardize(value))
 
-  def log_survival_function(self, value: Array) -> Array:
+  def log_survival_function(self, value: EventT) -> Array:
     """See `Distribution.log_survival_function`."""
     return -jax.nn.softplus(self._standardize(value))
 
   def mean(self) -> Array:
     """Calculates the mean."""
     return self.loc
```

### Comparing `distrax-0.1.3/distrax/_src/distributions/logistic_test.py` & `distrax-0.1.4/distrax/_src/distributions/logistic_test.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/distributions/mixture_of_two.py` & `distrax-0.1.4/distrax/_src/distributions/mixture_of_two.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 
 
 tfd = tfp.distributions
 Array = chex.Array
 Numeric = chex.Numeric
 PRNGKey = chex.PRNGKey
 DistributionLike = base_distribution.DistributionLike
+EventT = base_distribution.EventT
 
 
 class MixtureOfTwo(base_distribution.Distribution):
   """A mixture of two distributions."""
 
   def __init__(
       self,
@@ -75,15 +76,15 @@
     key, key_a, key_b, mask_key = jax.random.split(key, num=4)
     mask_from_a = jax.random.bernoulli(mask_key, p=self._prob_a, shape=[n])
     sample_a = self._component_a.sample(seed=key_a, sample_shape=n)
     sample_b = self._component_b.sample(seed=key_b, sample_shape=n)
     mask_from_a = jnp.expand_dims(mask_from_a, tuple(range(1, sample_a.ndim)))
     return jnp.where(mask_from_a, sample_a, sample_b)
 
-  def log_prob(self, value: Array) -> Array:
+  def log_prob(self, value: EventT) -> Array:
     """See `Distribution.log_prob`."""
     logp1 = jnp.log(self._prob_a) + self._component_a.log_prob(value)
     logp2 = jnp.log(1 - self._prob_a) + self._component_b.log_prob(value)
     return jnp.logaddexp(logp1, logp2)
 
   @property
   def event_shape(self) -> Tuple[int, ...]:
```

### Comparing `distrax-0.1.3/distrax/_src/distributions/mixture_of_two_test.py` & `distrax-0.1.4/distrax/_src/distributions/mixture_of_two_test.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/distributions/mixture_same_family.py` & `distrax-0.1.4/distrax/_src/distributions/mixture_same_family.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 
 tfd = tfp.distributions
 
 Array = chex.Array
 PRNGKey = chex.PRNGKey
 DistributionLike = distribution.DistributionLike
 CategoricalLike = categorical.CategoricalLike
+EventT = distribution.EventT
 
 
 class MixtureSameFamily(distribution.Distribution):
   """Mixture with components provided from a single batched distribution."""
 
   equiv_tfp_cls = tfd.MixtureSameFamily
 
@@ -108,15 +109,15 @@
     mask = mask.reshape(mask.shape + (1,) * len(self.event_shape))
 
     # Need to sum over the component axis, which is the last one for scalar
     # components, the second-last one for 1-dim events, etc.
     samples = jnp.sum(samples_all * mask, axis=-1 - len(self.event_shape))
     return samples
 
-  def log_prob(self, value: Array) -> Array:
+  def log_prob(self, value: EventT) -> Array:
     """See `Distribution.log_prob`."""
     # Add component axis to make input broadcast with components distribution.
     expanded = jnp.expand_dims(value, axis=-1 - len(self.event_shape))
     # Compute `log_prob` in every component.
     lp = self.components_distribution.log_prob(expanded)
     # Last batch axis is number of components, i.e. last axis of `lp` below.
     # Last axis of mixture log probs are components, so reduce last axis.
```

### Comparing `distrax-0.1.3/distrax/_src/distributions/mixture_same_family_test.py` & `distrax-0.1.4/distrax/_src/distributions/mixture_same_family_test.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/distributions/multinomial.py` & `distrax-0.1.4/distrax/_src/distributions/multinomial.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 
 
 tfd = tfp.distributions
 
 Array = chex.Array
 Numeric = chex.Numeric
 PRNGKey = chex.PRNGKey
+EventT = distribution.EventT
 
 
 class Multinomial(distribution.Distribution):
   """Multinomial distribution with parameter `probs`."""
 
   equiv_tfp_cls = tfd.Multinomial
 
@@ -135,15 +136,15 @@
     if self._logits is not None:
       # jax.nn.log_softmax was already applied in init to logits.
       return jnp.broadcast_to(self._logits,
                               self.batch_shape + self.event_shape)
     return jnp.broadcast_to(jnp.log(self._probs),
                             self.batch_shape + self.event_shape)
 
-  def log_prob(self, value: Array) -> Array:
+  def log_prob(self, value: EventT) -> Array:
     """See `Distribution.log_prob`."""
     total_permutations = lax.lgamma(self._total_count + 1.)
     counts_factorial = lax.lgamma(value + 1.)
     redundant_permutations = jnp.sum(counts_factorial, axis=-1)
     log_combinations = total_permutations - redundant_permutations
     return log_combinations + jnp.sum(
         math.multiply_no_nan(self.log_of_probs, value), axis=-1)
```

### Comparing `distrax-0.1.3/distrax/_src/distributions/multinomial_test.py` & `distrax-0.1.4/distrax/_src/distributions/multinomial_test.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/distributions/mvn_diag.py` & `distrax-0.1.4/distrax/_src/distributions/mvn_diag.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 import jax
 import jax.numpy as jnp
 from tensorflow_probability.substrates import jax as tfp
 
 tfd = tfp.distributions
 
 Array = chex.Array
+EventT = distribution.EventT
 
 
 def _check_parameters(
     loc: Optional[Array], scale_diag: Optional[Array]) -> None:
   """Checks that the `loc` and `scale_diag` parameters are correct."""
   chex.assert_not_both_none(loc, scale_diag)
   if scale_diag is not None and not scale_diag.shape:
@@ -97,19 +98,19 @@
     """Scale of the distribution."""
     return jnp.broadcast_to(
         self._scale_diag, self.batch_shape + self.event_shape)
 
   def _standardize(self, value: Array) -> Array:
     return (value - self._loc) / self._scale_diag
 
-  def cdf(self, value: Array) -> Array:
+  def cdf(self, value: EventT) -> Array:
     """See `Distribution.cdf`."""
     return jnp.prod(jax.scipy.special.ndtr(self._standardize(value)), axis=-1)
 
-  def log_cdf(self, value: Array) -> Array:
+  def log_cdf(self, value: EventT) -> Array:
     """See `Distribution.log_cdf`."""
     return jnp.sum(
         jax.scipy.special.log_ndtr(self._standardize(value)), axis=-1)
 
   def __getitem__(self, index) -> 'MultivariateNormalDiag':
     """See `Distribution.__getitem__`."""
     index = distribution.to_batch_shape_index(self.batch_shape, index)
```

### Comparing `distrax-0.1.3/distrax/_src/distributions/mvn_diag_plus_low_rank.py` & `distrax-0.1.4/distrax/_src/distributions/mvn_diag_plus_low_rank.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/distributions/mvn_diag_plus_low_rank_test.py` & `distrax-0.1.4/distrax/_src/distributions/mvn_diag_plus_low_rank_test.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/distributions/mvn_diag_test.py` & `distrax-0.1.4/distrax/_src/distributions/mvn_diag_test.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/distributions/mvn_from_bijector.py` & `distrax-0.1.4/distrax/_src/distributions/mvn_from_bijector.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/distributions/mvn_from_bijector_test.py` & `distrax-0.1.4/distrax/_src/distributions/mvn_from_bijector_test.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/distributions/mvn_full_covariance.py` & `distrax-0.1.4/distrax/_src/distributions/mvn_full_covariance.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/distributions/mvn_full_covariance_test.py` & `distrax-0.1.4/distrax/_src/distributions/mvn_full_covariance_test.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/distributions/mvn_kl_test.py` & `distrax-0.1.4/distrax/_src/distributions/mvn_kl_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,13 +114,13 @@
                 dist1_distrax)
           elif mode == 'distrax_to_tfp':
             result1 = self.variant(getattr(dist1_distrax, method))(dist2_tfp)
             result2 = self.variant(getattr(dist2_distrax, method))(dist1_tfp)
           elif mode == 'tfp_to_distrax':
             result1 = self.variant(getattr(dist1_tfp, method))(dist2_distrax)
             result2 = self.variant(getattr(dist2_tfp, method))(dist1_distrax)
-          np.testing.assert_allclose(result1, expected_result1, rtol=0.02)
-          np.testing.assert_allclose(result2, expected_result2, rtol=0.02)
+          np.testing.assert_allclose(result1, expected_result1, rtol=0.03)
+          np.testing.assert_allclose(result2, expected_result2, rtol=0.03)
 
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `distrax-0.1.3/distrax/_src/distributions/mvn_tri.py` & `distrax-0.1.4/distrax/_src/distributions/mvn_tri.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/distributions/mvn_tri_test.py` & `distrax-0.1.4/distrax/_src/distributions/mvn_tri_test.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/distributions/normal.py` & `distrax-0.1.4/distrax/_src/distributions/normal.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 from tensorflow_probability.substrates import jax as tfp
 
 tfd = tfp.distributions
 
 Array = chex.Array
 Numeric = chex.Numeric
 PRNGKey = chex.PRNGKey
+EventT = distribution.EventT
 
 _half_log2pi = 0.5 * math.log(2 * math.pi)
 
 
 class Normal(distribution.Distribution):
   """Normal distribution with location `loc` and `scale` parameters."""
 
@@ -84,37 +85,37 @@
   def _sample_n_and_log_prob(self, key: PRNGKey, n: int) -> Tuple[Array, Array]:
     """See `Distribution._sample_n_and_log_prob`."""
     rnd = self._sample_from_std_normal(key, n)
     samples = self._scale * rnd + self._loc
     log_prob = -0.5 * jnp.square(rnd) - _half_log2pi - jnp.log(self._scale)
     return samples, log_prob
 
-  def log_prob(self, value: Array) -> Array:
+  def log_prob(self, value: EventT) -> Array:
     """See `Distribution.log_prob`."""
     log_unnormalized = -0.5 * jnp.square(self._standardize(value))
     log_normalization = _half_log2pi + jnp.log(self._scale)
     return log_unnormalized - log_normalization
 
-  def cdf(self, value: Array) -> Array:
+  def cdf(self, value: EventT) -> Array:
     """See `Distribution.cdf`."""
     return jax.scipy.special.ndtr(self._standardize(value))
 
-  def log_cdf(self, value: Array) -> Array:
+  def log_cdf(self, value: EventT) -> Array:
     """See `Distribution.log_cdf`."""
     return jax.scipy.special.log_ndtr(self._standardize(value))
 
-  def survival_function(self, value: Array) -> Array:
+  def survival_function(self, value: EventT) -> Array:
     """See `Distribution.survival_function`."""
     return jax.scipy.special.ndtr(-self._standardize(value))
 
-  def log_survival_function(self, value: Array) -> Array:
+  def log_survival_function(self, value: EventT) -> Array:
     """See `Distribution.log_survival_function`."""
     return jax.scipy.special.log_ndtr(-self._standardize(value))
 
-  def _standardize(self, value: Array) -> Array:
+  def _standardize(self, value: EventT) -> Array:
     return (value - self._loc) / self._scale
 
   def entropy(self) -> Array:
     """Calculates the Shannon entropy (in nats)."""
     log_normalization = _half_log2pi + jnp.log(self.scale)
     entropy = 0.5 + log_normalization
     return entropy
```

### Comparing `distrax-0.1.3/distrax/_src/distributions/normal_float64_test.py` & `distrax-0.1.4/distrax/_src/distributions/normal_float64_test.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/distributions/normal_test.py` & `distrax-0.1.4/distrax/_src/distributions/normal_test.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/distributions/one_hot_categorical.py` & `distrax-0.1.4/distrax/_src/distributions/one_hot_categorical.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 from tensorflow_probability.substrates import jax as tfp
 
 
 tfd = tfp.distributions
 
 Array = chex.Array
 PRNGKey = chex.PRNGKey
+EventT = distribution.EventT
 
 
 class OneHotCategorical(categorical.Categorical):
   """OneHotCategorical distribution."""
 
   equiv_tfp_cls = tfd.OneHotCategorical
 
@@ -64,29 +65,29 @@
         jnp.all(self.probs >= 0, axis=-1, keepdims=True))
     draws = jax.random.categorical(
         key=key, logits=self.logits, axis=-1, shape=new_shape)
     draws_one_hot = jax.nn.one_hot(
         draws, num_classes=self.num_categories).astype(self._dtype)
     return jnp.where(is_valid, draws_one_hot, jnp.ones_like(draws_one_hot) * -1)
 
-  def log_prob(self, value: Array) -> Array:
+  def log_prob(self, value: EventT) -> Array:
     """See `Distribution.log_prob`."""
     return jnp.sum(math.multiply_no_nan(self.logits, value), axis=-1)
 
-  def prob(self, value: Array) -> Array:
+  def prob(self, value: EventT) -> Array:
     """See `Distribution.prob`."""
     return jnp.sum(math.multiply_no_nan(self.probs, value), axis=-1)
 
   def mode(self) -> Array:
     """Calculates the mode."""
     preferences = self._probs if self._logits is None else self._logits
     greedy_index = jnp.argmax(preferences, axis=-1)
     return jax.nn.one_hot(greedy_index, self.num_categories).astype(self._dtype)
 
-  def cdf(self, value: Array) -> Array:
+  def cdf(self, value: EventT) -> Array:
     """See `Distribution.cdf`."""
     return jnp.sum(math.multiply_no_nan(
         jnp.cumsum(self.probs, axis=-1), value), axis=-1)
 
   def __getitem__(self, index) -> 'OneHotCategorical':
     """See `Distribution.__getitem__`."""
     index = distribution.to_batch_shape_index(self.batch_shape, index)
```

### Comparing `distrax-0.1.3/distrax/_src/distributions/one_hot_categorical_test.py` & `distrax-0.1.4/distrax/_src/distributions/one_hot_categorical_test.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/distributions/quantized.py` & `distrax-0.1.4/distrax/_src/distributions/quantized.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 tfd = tfp.distributions
 
 Array = chex.Array
 Numeric = chex.Numeric
 PRNGKey = chex.PRNGKey
 DistributionLike = base_distribution.DistributionLike
 DistributionT = base_distribution.DistributionT
+EventT = base_distribution.EventT
 
 
 class Quantized(
     base_distribution.Distribution[Array, Tuple[int, ...], jnp.dtype],):
   """Distribution representing the quantization `Y = ceil(X)`.
 
   Given an input distribution `p(x)` over a univariate random variable `X`,
@@ -147,15 +148,15 @@
     # Use the survival function instead of the CDF when its value is smaller,
     # which happens to the right of the median of the distribution.
     big = jnp.where(log_sf < log_cdf, log_sf_m1, log_cdf)
     small = jnp.where(log_sf < log_cdf, log_sf, log_cdf_m1)
     log_probs = math.log_expbig_minus_expsmall(big, small)
     return samples, log_probs
 
-  def log_prob(self, value: Array) -> Array:
+  def log_prob(self, value: EventT) -> Array:
     """Calculates the log probability of an event.
 
     This implementation differs slightly from the one in TFP, as it returns
     `-jnp.inf` on non-integer values instead of returning the log prob of the
     floor of the input. In addition, this implementation also returns `-jnp.inf`
     on inputs that are outside the support of the distribution (as opposed to
     `nan`, like TFP does). On other integer values, both implementations are
@@ -193,15 +194,15 @@
     # case `value > high` we test whether `log_sf_m1` is finite; `log_cdf` will
     # be `0.` in this regime.
     is_outside = jnp.logical_or(jnp.isinf(log_cdf), jnp.isinf(log_sf_m1))
     log_probs = jnp.where(is_outside, -jnp.inf, log_probs)
 
     return log_probs
 
-  def prob(self, value: Array) -> Array:
+  def prob(self, value: EventT) -> Array:
     """Calculates the probability of an event.
 
     This implementation differs slightly from the one in TFP, as it returns 0
     on non-integer values instead of returning the prob of the floor of the
     input. It is identical for integer values.
 
     Similar to TFP, the probability is computed using either the CDF or the
@@ -223,15 +224,15 @@
     probs = jnp.where(sf < cdf, sf_m1 - sf, cdf - cdf_m1)
 
     # Return 0. when evaluating on non-integer value.
     is_integer = jnp.where(value > jnp.floor(value), False, True)
     probs = jnp.where(is_integer, probs, 0.)
     return probs
 
-  def log_cdf(self, value: Array) -> Array:
+  def log_cdf(self, value: EventT) -> Array:
     """See `Distribution.log_cdf`."""
     # The log CDF of a quantized distribution is piecewise constant on half-open
     # intervals:
     #    ... [n-2   n-1) [n-1   n) [n   n+1) [n+1   n+2) ...
     # with log CDF(n) <= log CDF(n+1), because the distribution only has mass on
     # integer values. Therefore: P[Y <= value] = P[Y <= floor(value)].
     y = jnp.floor(value)
@@ -239,15 +240,15 @@
     # Update result outside of the interval [low, high].
     if self.low is not None:
       result = jnp.where(y < self.low, -jnp.inf, result)
     if self.high is not None:
       result = jnp.where(y < self.high, result, 0.)
     return result
 
-  def cdf(self, value: Array) -> Array:
+  def cdf(self, value: EventT) -> Array:
     """See `Distribution.cdf`."""
     # The CDF of a quantized distribution is piecewise constant on half-open
     # intervals:
     #    ... [n-2   n-1) [n-1   n) [n   n+1) [n+1   n+2) ...
     # with CDF(n) <= CDF(n+1), because the distribution only has mass on integer
     # values. Therefore: P[Y <= value] = P[Y <= floor(value)].
     y = jnp.floor(value)
@@ -255,15 +256,15 @@
     # Update result outside of the interval [low, high].
     if self.low is not None:
       result = jnp.where(y < self.low, 0., result)
     if self.high is not None:
       result = jnp.where(y < self.high, result, 1.)
     return result
 
-  def log_survival_function(self, value: Array) -> Array:
+  def log_survival_function(self, value: EventT) -> Array:
     """Calculates the log of the survival function of an event.
 
     This implementation differs slightly from TFP, in that it returns the
     correct log of the survival function for non-integer values, that is, it
     always equates to `log(1 - CDF(value))`. It is identical for integer values.
 
     Args:
@@ -282,15 +283,15 @@
     # Update result outside of the interval [low, high].
     if self._low is not None:
       result = jnp.where(y < self._low, 0., result)
     if self._high is not None:
       result = jnp.where(y < self._high, result, -jnp.inf)
     return result
 
-  def survival_function(self, value: Array) -> Array:
+  def survival_function(self, value: EventT) -> Array:
     """Calculates the survival function of an event.
 
     This implementation differs slightly from TFP, in that it returns the
     correct survival function for non-integer values, that is, it always
     equates to `1 - CDF(value)`. It is identical for integer values.
 
     Args:
```

### Comparing `distrax-0.1.3/distrax/_src/distributions/quantized_test.py` & `distrax-0.1.4/distrax/_src/distributions/quantized_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -320,15 +320,17 @@
   def test_jittable(self):
     super()._test_jittable((self.tfd_base_distribution, 0., 1.))
 
 
 class QuantizedDistraxUniform2D(QuantizedTFPUniform2D):
 
   def _make_distrax_base_distribution(self):
-    return uniform.Uniform(low=[0., 10.], high=[100., 90.])
+    return uniform.Uniform(
+        low=jnp.array([0.0, 10.0]), high=jnp.array([100.0, 90.0])
+    )
 
   def test_jittable(self):
     super()._test_jittable((self.distrax_base_distribution, 0., 1.))
 
 
 class QuantizedInvalidParams(equivalence.EquivalenceTest):
   """Class to test invalid combinations of the input parameters."""
```

### Comparing `distrax-0.1.3/distrax/_src/distributions/softmax.py` & `distrax-0.1.4/distrax/_src/distributions/softmax.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/distributions/softmax_test.py` & `distrax-0.1.4/distrax/_src/distributions/softmax_test.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/distributions/straight_through.py` & `distrax-0.1.4/distrax/_src/distributions/straight_through.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/distributions/straight_through_test.py` & `distrax-0.1.4/distrax/_src/distributions/straight_through_test.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/distributions/tfp_compatible_distribution.py` & `distrax-0.1.4/distrax/_src/distributions/tfp_compatible_distribution.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 Array = chex.Array
 ArrayNumpy = chex.ArrayNumpy
 Distribution = distribution.Distribution
 IntLike = distribution.IntLike
 PRNGKey = chex.PRNGKey
 tangent_spaces = tfp.experimental.tangent_spaces
 TangentSpace = tangent_spaces.TangentSpace
+EventT = distribution.EventT
 
 
 def tfp_compatible_distribution(
     base_distribution: Distribution,
     name: Optional[str] = None) -> distribution.DistributionT:
   """Create a TFP-compatible distribution from a Distrax distribution.
 
@@ -113,30 +114,30 @@
     def reparameterization_type(self) -> tfd.ReparameterizationType:
       """Proxy for the TFP property `reparameterization_type`.
 
       It always returns `tfd.NOT_REPARAMETERIZED`.
       """
       return tfd.NOT_REPARAMETERIZED
 
-    def _sample_n(self, key: PRNGKey, n: int) -> Array:
+    def _sample_n(self, key: PRNGKey, n: int) -> EventT:
       return base_distribution.sample(seed=key, sample_shape=(n,))
 
-    def log_prob(self, value: Array) -> Array:
+    def log_prob(self, value: EventT) -> Array:
       """See `Distribution.log_prob`."""
       return base_distribution.log_prob(value)
 
     @property
     def parameters(self) -> Dict[str, str]:
       """Returns a dictionary whose key 'name' maps to the distribution name."""
       return {'name': self.name}
 
     def sample(self,
                sample_shape: Union[IntLike, Sequence[IntLike]] = (),
                seed: Optional[Union[int, tfp.util.SeedStream]] = None,
-               **unused_kwargs) -> Array:
+               **unused_kwargs) -> EventT:
       """See `Distribution.sample`."""
       if not np.isscalar(sample_shape):
         sample_shape = tuple(sample_shape)
       return base_distribution.sample(sample_shape=sample_shape, seed=seed)
 
     def experimental_local_measure(
         self,
```

### Comparing `distrax-0.1.3/distrax/_src/distributions/tfp_compatible_distribution_test.py` & `distrax-0.1.4/distrax/_src/distributions/tfp_compatible_distribution_test.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/distributions/transformed.py` & `distrax-0.1.4/distrax/_src/distributions/transformed.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 
 tfd = tfp.distributions
 
 PRNGKey = dist_base.PRNGKey
 Array = dist_base.Array
 DistributionLike = dist_base.DistributionLike
 BijectorLike = bjct_base.BijectorLike
+EventT = dist_base.EventT
 
 
 class Transformed(dist_base.Distribution):
   """Distribution of a random variable transformed by a bijective function.
 
   Let `X` be a continuous random variable and `Y = f(X)` be a random variable
   transformed by a differentiable bijection `f` (a "bijector"). Given the
@@ -149,15 +150,15 @@
   @property
   def batch_shape(self) -> Tuple[int, ...]:
     """See `Distribution.batch_shape`."""
     if self._batch_shape is None:
       self._infer_shapes_and_dtype()
     return self._batch_shape
 
-  def log_prob(self, value: Array) -> Array:
+  def log_prob(self, value: EventT) -> Array:
     """See `Distribution.log_prob`."""
     x, ildj_y = self.bijector.inverse_and_log_det(value)
     lp_x = self.distribution.log_prob(x)
     lp_y = lp_x + ildj_y
     return lp_y
 
   def _sample_n(self, key: PRNGKey, n: int) -> Array:
```

### Comparing `distrax-0.1.3/distrax/_src/distributions/transformed_test.py` & `distrax-0.1.4/distrax/_src/distributions/transformed_test.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/distributions/uniform.py` & `distrax-0.1.4/distrax/_src/distributions/uniform.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 from tensorflow_probability.substrates import jax as tfp
 
 tfd = tfp.distributions
 
 Array = chex.Array
 Numeric = chex.Numeric
 PRNGKey = chex.PRNGKey
+EventT = distribution.EventT
 
 
 class Uniform(distribution.Distribution):
   """Uniform distribution with `low` and `high` parameters."""
 
   equiv_tfp_cls = tfd.Uniform
 
@@ -84,19 +85,19 @@
   def _sample_n_and_log_prob(self, key: PRNGKey, n: int) -> Tuple[Array, Array]:
     """See `Distribution._sample_n_and_log_prob`."""
     samples = self._sample_n(key, n)
     log_prob = -jnp.log(self.range)
     log_prob = jnp.repeat(log_prob[None], n, axis=0)
     return samples, log_prob
 
-  def log_prob(self, value: Array) -> Array:
+  def log_prob(self, value: EventT) -> Array:
     """See `Distribution.log_prob`."""
     return jnp.log(self.prob(value))
 
-  def prob(self, value: Array) -> Array:
+  def prob(self, value: EventT) -> Array:
     """See `Distribution.prob`."""
     return jnp.where(
         jnp.logical_or(value < self.low, value > self.high),
         jnp.zeros_like(value),
         jnp.ones_like(value) / self.range)
 
   def entropy(self) -> Array:
@@ -115,23 +116,23 @@
     """Calculates the standard deviation."""
     return self.range / math.sqrt(12.)
 
   def median(self) -> Array:
     """Calculates the median."""
     return self.mean()
 
-  def cdf(self, value: Array) -> Array:
+  def cdf(self, value: EventT) -> Array:
     """See `Distribution.cdf`."""
     ones = jnp.ones_like(self.range)
     zeros = jnp.zeros_like(ones)
     result_if_not_big = jnp.where(
         value < self.low, zeros, (value - self.low) / self.range)
     return jnp.where(value > self.high, ones, result_if_not_big)
 
-  def log_cdf(self, value: Array) -> Array:
+  def log_cdf(self, value: EventT) -> Array:
     """See `Distribution.log_cdf`."""
     return jnp.log(self.cdf(value))
 
   def __getitem__(self, index) -> 'Uniform':
     """See `Distribution.__getitem__`."""
     index = distribution.to_batch_shape_index(self.batch_shape, index)
     return Uniform(low=self.low[index], high=self.high[index])
```

### Comparing `distrax-0.1.3/distrax/_src/distributions/uniform_float64_test.py` & `distrax-0.1.4/distrax/_src/distributions/uniform_float64_test.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/distributions/uniform_test.py` & `distrax-0.1.4/distrax/_src/distributions/uniform_test.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/distributions/von_mises.py` & `distrax-0.1.4/distrax/_src/distributions/von_mises.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Von Mises distribution."""
 
 import functools
 import math
-from typing import Sequence, Tuple, Union
+from typing import cast, Sequence, Tuple, Union
 
 import chex
 from distrax._src.distributions import distribution
 from distrax._src.distributions import normal
 from distrax._src.utils import conversion
 import jax
 import jax.numpy as jnp
@@ -29,14 +29,15 @@
 
 tfd = tfp.distributions
 
 Array = chex.Array
 Numeric = chex.Numeric
 PRNGKey = chex.PRNGKey
 IntLike = Union[int, np.int16, np.int32, np.int64]
+EventT = distribution.EventT
 
 
 class VonMises(distribution.Distribution):
   """The von Mises distribution over angles.
 
   The von Mises distribution is a distribution over angles. It is the maximum
   entropy distribution on the space of angles, given a circular mean and a
@@ -122,22 +123,22 @@
     return self.loc
 
   def variance(self) -> Array:
     """The circular variance of the distribution."""
     conc = self._concentration
     return 1. - jax.scipy.special.i1e(conc) / jax.scipy.special.i0e(conc)
 
-  def prob(self, value: Array) -> Array:
+  def prob(self, value: EventT) -> Array:
     """The probability of value under the distribution."""
     conc = self._concentration
     unnormalized_prob = jnp.exp(conc * (jnp.cos(value - self._loc) - 1.))
     normalization = (2. * math.pi) * jax.scipy.special.i0e(conc)
     return unnormalized_prob / normalization
 
-  def log_prob(self, value: Array) -> Array:
+  def log_prob(self, value: EventT) -> Array:
     """The logarithm of the probability of value under the distribution."""
     conc = self._concentration
     i_0 = jax.scipy.special.i0(conc)
     return (
         conc * jnp.cos(value - self._loc) - math.log(2 * math.pi) - jnp.log(i_0)
     )
 
@@ -156,15 +157,15 @@
     i1e = jax.scipy.special.i1e(conc)
     return conc * (1 - i1e / i0e) + math.log(2 * math.pi) + jnp.log(i0e)
 
   def mode(self) -> Array:
     """The mode of the distribution."""
     return self.mean()
 
-  def cdf(self, value: Array) -> Array:
+  def cdf(self, value: EventT) -> Array:
     """The CDF of `value` under the distribution.
 
     Note that the CDF takes values of 0. or 1. for values outside of
     [-pi, pi). Note that this behaviour is different from
     `tensorflow_probability.VonMises` or `scipy.stats.vonmises`.
     Args:
       value: the angle evaluated under the distribution.
@@ -176,30 +177,30 @@
     return jnp.clip(
         _von_mises_cdf(value - loc, self._concentration, dtype)
         - _von_mises_cdf(-math.pi - loc, self._concentration, dtype),
         a_min=0.,
         a_max=1.,
     )
 
-  def log_cdf(self, value: Array) -> Array:
+  def log_cdf(self, value: EventT) -> Array:
     """See `Distribution.log_cdf`."""
     return jnp.log(self.cdf(value))
 
-  def survival_function(self, value: Array) -> Array:
+  def survival_function(self, value: EventT) -> Array:
     """See `Distribution.survival_function`."""
     dtype = jnp.result_type(value, self._loc, self._concentration)
     loc = _convert_angle_to_standard(self._loc)
     return jnp.clip(
         _von_mises_cdf(math.pi - loc, self._concentration, dtype)
         - _von_mises_cdf(value - loc, self._concentration, dtype),
         a_min=0.,
         a_max=1.,
     )
 
-  def log_survival_function(self, value: Array) -> Array:
+  def log_survival_function(self, value: EventT) -> Array:
     """See `Distribution.log_survival_function`."""
     return jnp.log(self.survival_function(value))
 
   def __getitem__(self, index) -> 'VonMises':
     index = distribution.to_batch_shape_index(self.batch_shape, index)
     return VonMises(
         loc=self.loc[index],
@@ -297,15 +298,16 @@
       excluded=(2,),
   )
   dcdf_dconcentration = vectorized_grad_cdf(samples, concentration, dtype)
 
   inv_prob = jnp.exp(-concentration * (jnp.cos(samples) - 1.)) * (
       (2. * math.pi) * jax.scipy.special.i0e(concentration)
   )
-  dsamples = dconcentration * (-dcdf_dconcentration * inv_prob)
+  dcdf_dconcentration = cast(chex.Array, dcdf_dconcentration)
+  dsamples = dconcentration * (-inv_prob * dcdf_dconcentration)
   return samples, dsamples
 
 
 @functools.partial(jax.custom_jvp, nondiff_argnums=(2,))
 def _von_mises_cdf(
     value: Array,
     concentration: Array,
```

### Comparing `distrax-0.1.3/distrax/_src/distributions/von_mises_test.py` & `distrax-0.1.4/distrax/_src/distributions/von_mises_test.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/utils/__init__.py` & `distrax-0.1.4/distrax/_src/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/utils/conversion.py` & `distrax-0.1.4/distrax/_src/utils/conversion.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/utils/conversion_test.py` & `distrax-0.1.4/distrax/_src/utils/conversion_test.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/utils/equivalence.py` & `distrax-0.1.4/distrax/_src/utils/equivalence.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,18 +82,19 @@
     self.key = jax.random.PRNGKey(1234)
     self.distrax_cls = distrax_cls
     if hasattr(distrax_cls, 'equiv_tfp_cls'):
       self.tfp_cls = distrax_cls.equiv_tfp_cls
     else:
       self.tfp_cls = get_tfp_equiv(distrax_cls)
 
-  def assertion_fn(self, **kwargs) -> Callable[[Array, Array], None]:
-    def fn(x: Array, y: Array) -> None:
+  def assertion_fn(self, **kwargs) -> Callable[[Any, Any], None]:
+    def f(x, y):
       np.testing.assert_allclose(x, y, **kwargs)
-    return fn
+
+    return f
 
   def _test_attribute(
       self,
       attribute_string: str,
       dist_args: Tuple[Any, ...] = (),
       dist_kwargs: Optional[Dict[str, Any]] = None,
       tfp_dist_args: Optional[Tuple[Any, ...]] = None,
```

### Comparing `distrax-0.1.3/distrax/_src/utils/hmm.py` & `distrax-0.1.4/distrax/_src/utils/hmm.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,15 @@
   @property
   def obs_dist(self) -> distribution.DistributionLike:
     return self._obs_dist
 
   def sample(self,
              *,
              seed: chex.PRNGKey,
-             seq_len: chex.Array) -> Tuple[chex.Array, chex.Array]:
+             seq_len: int) -> Tuple[chex.Array, chex.Array]:
     """Sample from this HMM.
 
     Samples an observation of given length according to this
     Hidden Markov Model and gives the sequence of the hidden states
     as well as the observation.
 
     Args:
```

### Comparing `distrax-0.1.3/distrax/_src/utils/hmm_test.py` & `distrax-0.1.4/distrax/_src/utils/hmm_test.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/utils/importance_sampling.py` & `distrax-0.1.4/distrax/_src/utils/importance_sampling.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/utils/importance_sampling_test.py` & `distrax-0.1.4/distrax/_src/utils/importance_sampling_test.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/utils/jittable.py` & `distrax-0.1.4/distrax/_src/utils/jittable.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/utils/jittable_test.py` & `distrax-0.1.4/distrax/_src/utils/jittable_test.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/utils/math.py` & `distrax-0.1.4/distrax/_src/utils/math.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/utils/math_test.py` & `distrax-0.1.4/distrax/_src/utils/math_test.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/utils/monte_carlo.py` & `distrax-0.1.4/distrax/_src/utils/monte_carlo.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/utils/monte_carlo_test.py` & `distrax-0.1.4/distrax/_src/utils/monte_carlo_test.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/utils/transformations.py` & `distrax-0.1.4/distrax/_src/utils/transformations.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/_src/utils/transformations_test.py` & `distrax-0.1.4/distrax/_src/utils/transformations_test.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax/distrax_test.py` & `distrax-0.1.4/distrax/distrax_test.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/distrax.egg-info/PKG-INFO` & `distrax-0.1.4/distrax.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: distrax
-Version: 0.1.3
+Version: 0.1.4
 Summary: Distrax: Probability distributions in JAX.
 Home-page: https://github.com/deepmind/distrax
 Author: DeepMind
 Author-email: distrax-dev@google.com
 License: Apache 2.0
 Keywords: jax probability distribution python machine learning
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,15 +15,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Distrax
 
 ![CI status](https://github.com/deepmind/distrax/workflows/tests/badge.svg)
 ![pypi](https://img.shields.io/pypi/v/distrax)
```

### Comparing `distrax-0.1.3/distrax.egg-info/SOURCES.txt` & `distrax-0.1.4/distrax.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/examples/flow.py` & `distrax-0.1.4/examples/flow.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/examples/hmm.py` & `distrax-0.1.4/examples/hmm.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/examples/vae.py` & `distrax-0.1.4/examples/vae.py`

 * *Files identical despite different names*

### Comparing `distrax-0.1.3/setup.py` & `distrax-0.1.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     packages=find_namespace_packages(exclude=['*_test.py']),
     install_requires=_parse_requirements(
         os.path.join(_CURRENT_DIR, 'requirements', 'requirements.txt')),
     tests_require=_parse_requirements(
         os.path.join(_CURRENT_DIR, 'requirements', 'requirements-tests.txt')),
     zip_safe=False,  # Required for full installation.
     include_package_data=True,
-    python_requires='>=3.7',
+    python_requires='>=3.9',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Console',
         'Intended Audience :: Science/Research',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent',
```

