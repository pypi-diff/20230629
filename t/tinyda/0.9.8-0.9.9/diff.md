# Comparing `tmp/tinyda-0.9.8.tar.gz` & `tmp/tinyda-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinyda-0.9.8.tar", max compression
+gzip compressed data, was "tinyda-0.9.9.tar", max compression
```

## Comparing `tinyda-0.9.8.tar` & `tinyda-0.9.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1078 2022-09-02 12:22:03.235162 tinyda-0.9.8/LICENSE
--rw-r--r--   0        0        0     7399 2022-11-23 11:13:31.668787 tinyda-0.9.8/README.md
--rw-r--r--   0        0        0      845 2022-11-23 14:25:13.386429 tinyda-0.9.8/pyproject.toml
--rw-r--r--   0        0        0      379 2022-11-23 11:13:31.824788 tinyda-0.9.8/tinyDA/__init__.py
--rw-r--r--   0        0        0    28766 2022-11-23 11:13:31.832788 tinyda-0.9.8/tinyDA/chain.py
--rw-r--r--   0        0        0     7048 2022-11-23 14:25:13.386429 tinyda-0.9.8/tinyDA/diagnostics.py
--rw-r--r--   0        0        0     7915 2022-09-02 12:22:03.275162 tinyda-0.9.8/tinyDA/distributions.py
--rw-r--r--   0        0        0     1449 2022-11-23 11:13:31.840788 tinyda-0.9.8/tinyDA/link.py
--rw-r--r--   0        0        0     4759 2022-11-23 11:13:31.840788 tinyda-0.9.8/tinyDA/posterior.py
--rw-r--r--   0        0        0    44793 2022-11-23 11:13:31.852788 tinyda-0.9.8/tinyDA/proposal.py
--rw-r--r--   0        0        0    14878 2022-11-23 11:13:31.852788 tinyda-0.9.8/tinyDA/ray.py
--rw-r--r--   0        0        0    16891 2022-11-23 11:13:31.868788 tinyda-0.9.8/tinyDA/sampler.py
--rw-r--r--   0        0        0     2824 2022-11-22 13:35:59.934364 tinyda-0.9.8/tinyDA/umbridge.py
--rw-r--r--   0        0        0     6572 2022-11-23 11:13:31.868788 tinyda-0.9.8/tinyDA/utils.py
--rw-r--r--   0        0        0     8326 1970-01-01 00:00:00.000000 tinyda-0.9.8/setup.py
--rw-r--r--   0        0        0     8416 1970-01-01 00:00:00.000000 tinyda-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0     1078 2022-12-08 12:18:20.793331 tinyda-0.9.9/LICENSE
+-rw-r--r--   0        0        0     7401 2023-06-24 16:22:55.393245 tinyda-0.9.9/README.md
+-rw-r--r--   0        0        0      845 2023-06-24 16:22:55.433244 tinyda-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0      379 2022-12-08 12:18:20.829331 tinyda-0.9.9/tinyDA/__init__.py
+-rw-r--r--   0        0        0    27221 2023-06-24 06:13:52.143272 tinyda-0.9.9/tinyDA/chain.py
+-rw-r--r--   0        0        0     7048 2022-12-08 12:18:20.829331 tinyda-0.9.9/tinyDA/diagnostics.py
+-rw-r--r--   0        0        0     7915 2022-12-08 12:18:20.829331 tinyda-0.9.9/tinyDA/distributions.py
+-rw-r--r--   0        0        0     1449 2023-04-01 16:34:03.541659 tinyda-0.9.9/tinyDA/link.py
+-rw-r--r--   0        0        0     4759 2023-04-01 16:33:53.557865 tinyda-0.9.9/tinyDA/posterior.py
+-rw-r--r--   0        0        0    40659 2023-06-24 16:22:55.437244 tinyda-0.9.9/tinyDA/proposal.py
+-rw-r--r--   0        0        0    14537 2023-06-24 06:13:52.143272 tinyda-0.9.9/tinyDA/ray.py
+-rw-r--r--   0        0        0    16316 2023-06-24 06:13:52.143272 tinyda-0.9.9/tinyDA/sampler.py
+-rw-r--r--   0        0        0     2824 2022-12-08 12:18:20.829331 tinyda-0.9.9/tinyDA/umbridge.py
+-rw-r--r--   0        0        0     6572 2022-12-08 12:18:20.829331 tinyda-0.9.9/tinyDA/utils.py
+-rw-r--r--   0        0        0     8328 1970-01-01 00:00:00.000000 tinyda-0.9.9/setup.py
+-rw-r--r--   0        0        0     8469 1970-01-01 00:00:00.000000 tinyda-0.9.9/PKG-INFO
```

### Comparing `tinyda-0.9.8/LICENSE` & `tinyda-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tinyda-0.9.8/README.md` & `tinyda-0.9.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 * Delayed Acceptance (Christen & Fox, 2005)
 * Multilevel Delayed Acceptance (Lykkegaard et al. 2022)
 
 ### Proposals
 * Random Walk Metropolis Hastings (RWMH) - Metropolis et al. (1953), Hastings (1970)
 * preconditioned Crank-Nicolson (pCN) - Cotter et al. (2013)
 * Adaptive Metropolis (AM) - Haario et al. (2001)
-* Adaptive pCN - Hu and Yao (2016)
+* Operator-weighted pCN - Law (2014)
 * DREAM(Z) - Vrugt (2016)
 * Multiple-Try Metropolis (MTM) - Liu et al. (2000)
 
 ### Adaptive Error Models
 * State independent - Cui et al. (2018)
 * State dependent - Cui et al. (2018)
```

### Comparing `tinyda-0.9.8/pyproject.toml` & `tinyda-0.9.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tinyda"
-version = "0.9.8"
+version = "0.9.9"
 description = "Delayed Acceptance MCMC Sampler"
 license = "MIT"
 authors = ["Mikkel Bue Lykkegaard <mikkelbue@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/mikkelbue/tinyda"
 documentation = "https://tinyda.readthedocs.io"
 classifiers = [
```

### Comparing `tinyda-0.9.8/tinyDA/chain.py` & `tinyda-0.9.9/tinyDA/chain.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,15 +31,14 @@
     Methods
     -------
     sample(iterations)
         Runs the MCMC for the specified number of iterations.
     """
 
     def __init__(self, posterior, proposal, initial_parameters=None):
-
         """
         Parameters
         ----------
         posterior : tinyDA.Posterior
             A posterior responsible for communation between prior, likelihood
             and model. It also generates instances of tinyDA.Link (sample objects).
         proposal : tinyDA.Proposal
@@ -73,15 +72,14 @@
 
         # setup the proposal
         self.proposal.setup_proposal(
             parameters=self.initial_parameters, posterior=self.posterior
         )
 
     def sample(self, iterations, progressbar=True):
-
         """
         Parameters
         ----------
         iterations : int
             Number of MCMC samples to generate.
         progressbar : bool, optional
             Whether to draw a progressbar, default is True.
@@ -162,16 +160,14 @@
         coarse sampler or not.
     chain_fine : list
         Samples ("Links") in the fine MCMC chain.
     accepted_fine : list
         List of bool, signifying whether a fine proposal was accepted or not.
     adaptive_error_model : str or None
         The adaptive error model, see e.g. Cui et al. (2019).
-    R : numpy.ndarray
-        Restriction matrix for the adaptive error model.
     bias : tinaDA.RecursiveSampleMoments
         A recursive Gaussian error model that computes the sample moments of
         the coarse bias.
 
     Methods
     -------
     sample(iterations)
@@ -182,17 +178,15 @@
         self,
         posterior_coarse,
         posterior_fine,
         proposal,
         subsampling_rate,
         initial_parameters=None,
         adaptive_error_model=None,
-        R=None,
     ):
-
         """
         Parameters
         ----------
         posterior_coarse : tinyDA.Posterior
             A "coarse" posterior responsible for communation between prior,
             likelihood and model.It also generates instances of tinyDA.Link
             (sample objects).
@@ -208,17 +202,14 @@
             Starting point for the MCMC sampler, default is None (random draw
             from prior).
         adaptive_error_model : str or None, optional
             The adaptive error model, see e.g. Cui et al. (2019). Default is
             None (no error model), options are 'state-independent' or
             'state-dependent'. If an error model is used, the likelihood MUST
             have a set_bias() method, use e.g. tinyDA.AdaptiveLogLike.
-        R : numpy.ndarray or None, optional
-            Restriction matrix for the adaptive error model. Default is None
-            (identity matrix).
         """
 
         # internalise posteriors and the proposal
         self.posterior_coarse = posterior_coarse
         self.posterior_fine = posterior_fine
         self.proposal = proposal
         self.subsampling_rate = subsampling_rate
@@ -243,39 +234,30 @@
         self.chain_coarse.append(
             self.posterior_coarse.create_link(self.initial_parameters)
         )
         self.accepted_coarse.append(True)
         self.is_coarse.append(False)
 
         # append a link with the initial parameters to the coarse chain.
-        self.chain_fine.append(
-            self.posterior_fine.create_link(self.initial_parameters)
-        )
+        self.chain_fine.append(self.posterior_fine.create_link(self.initial_parameters))
         self.accepted_fine.append(True)
 
         # setup the proposal
         self.proposal.setup_proposal(
             parameters=self.initial_parameters, posterior=self.posterior_coarse
         )
 
         # set the adaptive error model as an attribute.
         self.adaptive_error_model = adaptive_error_model
 
         # set up the adaptive error model.
         if self.adaptive_error_model is not None:
-
-            if R is None:
-                self.R = np.eye(self.chain_fine[-1].model_output.shape[0])
-            else:
-                self.R = R
-
             # compute the difference between coarse and fine level.
             self.model_diff = (
-                self.R.dot(self.chain_fine[-1].model_output)
-                - self.chain_coarse[-1].model_output
+                self.chain_fine[-1].model_output - self.chain_coarse[-1].model_output
             )
 
             if self.adaptive_error_model == "state-independent":
                 # for the state-independent error model, the bias is
                 # RecursiveSampleMoments, and the corrector is the mean
                 # of all sampled differences.
                 self.bias = RecursiveSampleMoments(
@@ -327,15 +309,14 @@
                         ),
                         np.mean(self.accepted_fine[-100:]),
                     )
                 )
 
             # subsample the coarse model.
             for j in range(self.subsampling_rate):
-
                 # draw a new proposal, given the previous parameters.
                 proposal = self.proposal.make_proposal(self.chain_coarse[-1])
 
                 # create a link from that proposal.
                 proposal_link_coarse = self.posterior_coarse.create_link(proposal)
 
                 # compute the acceptance probability, which is unique to
@@ -377,19 +358,19 @@
                 # previous coarse link.
                 proposal_link_fine = self.posterior_fine.create_link(
                     self.chain_coarse[-1].parameters
                 )
 
                 # compute the delayed acceptance probability.
                 if self.adaptive_error_model == "state-dependent":
-
                     bias_next = (
-                        self.R.dot(proposal_link_fine.model_output)
+                        proposal_link_fine.model_output
                         - self.chain_coarse[-1].model_output
                     )
+
                     coarse_state_biased = self.posterior_coarse.update_link(
                         self.chain_coarse[-(self.subsampling_rate + 1)], bias_next
                     )
 
                     if self.proposal.is_symmetric:
                         q_x_y = q_y_x = 0
                     else:
@@ -434,41 +415,41 @@
                         self.chain_coarse[-(self.subsampling_rate + 1)]
                     )
                     self.accepted_coarse.append(False)
                     self.is_coarse.append(False)
 
             # update the adaptive error model.
             if self.adaptive_error_model is not None:
-
                 if self.adaptive_error_model == "state-independent":
                     # for the state-independent AEM, we simply update the
                     # RecursiveSampleMoments with the difference between
                     # the fine and coarse model output
                     self.model_diff = (
-                        self.R.dot(self.chain_fine[-1].model_output)
+                        self.chain_fine[-1].model_output
                         - self.chain_coarse[-1].model_output
                     )
+
                     self.bias.update(self.model_diff)
 
                     # and update the likelihood in the coarse posterior.
                     self.posterior_coarse.likelihood.set_bias(
                         self.bias.get_mu(), self.bias.get_sigma()
                     )
 
                 elif self.adaptive_error_model == "state-dependent":
                     # for the state-dependent error model, we want the
                     # difference, corrected with the previous difference
                     # to compute the error covariance.
-                    self.model_diff_corrected = self.R.dot(
-                        self.chain_fine[-1].model_output
-                    ) - (self.chain_coarse[-1].model_output + self.model_diff)
+                    self.model_diff_corrected = self.chain_fine[-1].model_output - (
+                        self.chain_coarse[-1].model_output + self.model_diff
+                    )
 
                     # and the "pure" model difference for the offset.
                     self.model_diff = (
-                        self.R.dot(self.chain_fine[-1].model_output)
+                        self.chain_fine[-1].model_output
                         - self.chain_coarse[-1].model_output
                     )
 
                     # update the ZeroMeanRecursiveSampleMoments with the
                     # corrected difference.
                     self.bias.update(self.model_diff_corrected)
 
@@ -509,16 +490,14 @@
         Starting point for the MCMC sampler
     chain : list
         Samples ("Links") in the finest level MCMC chain.
     accepted : list
         List of bool, signifying whether a proposal was accepted or not.
     adaptive_error_model : str or None
         The adaptive error model, see e.g. Cui et al. (2019).
-    R : numpy.ndarray
-        Restriction matrix for the adaptive error model on the finest level.
     bias : tinaDA.RecursiveSampleMoments
         A recursive Gaussian error model that computes the sample moments
         of the next-coarser bias.
 
     Methods
     -------
     sample(iterations)
@@ -528,17 +507,15 @@
     def __init__(
         self,
         posteriors,
         proposal,
         subsampling_rates,
         initial_parameters=None,
         adaptive_error_model=None,
-        R=None,
     ):
-
         """
         Parameters
         ----------
         posteriors : list
             List of instances of tinyDA.Posterior, in increasing order.
         proposal : tinyDA.Proposal
             Transition kernel for coarsest MCMC proposals.
@@ -549,19 +526,14 @@
             Starting point for the MCMC sampler, default is None (random
             draw from prior).
         adaptive_error_model : str or None, optional
             The adaptive error model, see e.g. Cui et al. (2019). Default
             is None (no error model), options are 'state-independent' or
             'state-dependent'. If an error model is used, the likelihood
             MUST have a set_bias() method, use e.g. tinyDA.AdaptiveLogLike.
-        R : list or None, optional
-            Restriction matrices for the adaptive error model. If list of
-            restriction matrices is given, it must have length
-            len(posteriors) - 1 and they must be in increasing order,
-            as the model hierachy. Default is None (identity matrices).
         """
 
         # internalise the finest posterior and set the level.
         self.posterior = posteriors[-1]
         self.level = len(posteriors) - 1
 
         # set the furrent level subsampling rate.
@@ -581,46 +553,31 @@
             self.initial_parameters = self.posterior.prior.rvs()
 
         # append a link with the initial parameters (this will automatically
         # compute the model output, and the relevant probabilties.
         self.chain.append(self.posterior.create_link(self.initial_parameters))
         self.accepted.append(True)
 
-        # make sure R can be passed recursively to MLDA proposal, if MLDAChain
-        # was initialised without tda.sample().
-        if R is None:
-            R = [None] * self.level
-
         # set the effective proposal to MLDA which runs on the next-coarser level.
         self.proposal = MLDA(
             posteriors[:-1],
             proposal,
             subsampling_rates[:-1],
             self.initial_parameters,
             adaptive_error_model,
-            R[:-1],
         )
 
         # set the adative error model as an attribute.
         self.adaptive_error_model = adaptive_error_model
 
         # set up the adaptive error model.
         if self.adaptive_error_model is not None:
-
-            # extract the finest-level restriction matrix from the list.
-            self.R = R[-1]
-
-            # if no restriction matrix was given, create an identity matrix.
-            if self.R is None:
-                self.R = np.eye(self.chain[-1].model_output.shape[0])
-
             # compute the difference between coarse and fine level.
             self.model_diff = (
-                self.R.dot(self.chain[-1].model_output)
-                - self.proposal.chain[-1].model_output
+                self.chain[-1].model_output - self.proposal.chain[-1].model_output
             )
 
             # set up the state-independent adaptive error model.
             if self.adaptive_error_model == "state-independent":
                 # for the state-independent error model, the bias is
                 # RecursiveSampleMoments, and the corrector is the mean
                 # of all sampled differences.
@@ -638,23 +595,21 @@
                 pass
 
             # update the first coarser link with the adaptive error model.
             self.proposal.chain[-1] = self.proposal.posterior.update_link(
                 self.proposal.chain[-1]
             )
 
-            # collect biases and restriction matrices in a list.
+            # collect biases in a list.
             self.biases = [self.bias]
-            self.Rs = [self.R]
 
-            # pass the bias models and restriction levels to the next-coarser level.
-            self.proposal.setup_adaptive_error_model(self.biases, self.Rs)
+            # pass the bias models to the next-coarser level.
+            self.proposal.setup_adaptive_error_model(self.biases)
 
     def sample(self, iterations, progressbar=True):
-
         """
         Parameters
         ----------
         iterations : int
             Number of MCMC samples to generate.
         progressbar : bool, optional
             Whether to draw a progressbar, default is True.
@@ -677,15 +632,14 @@
             proposal = self.proposal.make_proposal(self.subsampling_rate)
 
             if sum(self.proposal.accepted[-self.subsampling_rate :]) == 0:
                 self.chain.append(self.chain[-1])
                 self.accepted.append(False)
 
             else:
-
                 # create a link from that proposal.
                 proposal_link = self.posterior.create_link(proposal)
 
                 # compute the acceptance probability, which is unique to
                 # the proposal.
                 alpha = self.proposal.get_acceptance(
                     proposal_link,
@@ -703,19 +657,18 @@
                     self.accepted.append(False)
 
             # make sure the next-coarser level is aligned.
             self.proposal.align_chain(self.chain[-1].parameters, self.accepted[-1])
 
             # apply the adaptive error model.
             if self.adaptive_error_model is not None:
-
                 # compute the difference between coarse and fine level.
                 if self.accepted[-1]:
                     self.model_diff = (
-                        self.R.dot(self.chain[-1].model_output)
+                        self.chain[-1].model_output
                         - self.proposal.chain[-1].model_output
                     )
 
                 # update the state-independent adaptive error model.
                 if self.adaptive_error_model == "state-independent":
                     # for the state-independent error model, the bias is
                     # RecursiveSampleMoments, and the corrector is the mean
```

### Comparing `tinyda-0.9.8/tinyDA/diagnostics.py` & `tinyda-0.9.9/tinyDA/diagnostics.py`

 * *Files identical despite different names*

### Comparing `tinyda-0.9.8/tinyDA/distributions.py` & `tinyda-0.9.9/tinyDA/distributions.py`

 * *Files identical despite different names*

### Comparing `tinyda-0.9.8/tinyDA/link.py` & `tinyda-0.9.9/tinyDA/link.py`

 * *Files identical despite different names*

### Comparing `tinyda-0.9.8/tinyDA/posterior.py` & `tinyda-0.9.9/tinyDA/posterior.py`

 * *Files identical despite different names*

### Comparing `tinyda-0.9.8/tinyDA/proposal.py` & `tinyda-0.9.9/tinyDA/proposal.py`

 * *Files 5% similar despite different names*

```diff
@@ -83,29 +83,26 @@
     def setup_proposal(self, **kwargs):
         pass
 
     def adapt(self, **kwargs):
         pass
 
     def make_proposal(self, link):
-
         # draw a random sample from the proposal distribution.
         return self.q.rvs(1).flatten()
 
     def get_acceptance(self, proposal_link, previous_link):
-
         q_proposal = self.get_q(None, proposal_link)
         q_previous = self.get_q(None, previous_link)
 
         return np.exp(
             proposal_link.posterior - previous_link.posterior + q_previous - q_proposal
         )
 
     def get_q(self, x_link, y_link):
-
         # get the transition probability.:
         return self.q.logpdf(y_link.parameters)
 
 
 class GaussianRandomWalk(Proposal):
 
     """Standard Random Walk Metropolis Hastings proposal.
@@ -185,38 +182,34 @@
         self.scaling = scaling
 
         # set adaptivity.
         self.adaptive = adaptive
 
         # if adaptive, set some adaptivity parameters
         if self.adaptive:
-
             # adaptivity scaling.
             self.gamma = gamma
             # adaptivity period (delay between adapting)
             self.period = period
             # initialise adaptivity counter for diminishing adaptivity.
             self.k = 0
 
         # initialise counter of how many times, adapt() has been called..
         self.t = 0
 
     def setup_proposal(self, **kwargs):
         pass
 
     def adapt(self, **kwargs):
-
         self.t += 1
 
         # if adaptive, run the adaptivity routines.
         if self.adaptive:
-
             # make sure the periodicity is respected
             if self.t % self.period == 0:
-
                 # compute the acceptance rate during the previous period.
                 acceptance_rate = np.mean(kwargs["accepted"][-self.period :])
                 # set the scaling so that the acceptance rate will converge to 0.24.
                 self.scaling = np.exp(
                     np.log(self.scaling)
                     + self.gamma**-self.k * (acceptance_rate - 0.24)
                 )
@@ -301,27 +294,25 @@
         self.scaling = scaling
 
         # set adaptivity.
         self.adaptive = adaptive
 
         # if adaptive, set some adaptivity parameters
         if self.adaptive:
-
             # adaptivity scaling.
             self.gamma = gamma
             # adaptivity period (delay between adapting)
             self.period = period
             # initialise adaptivity counter for diminishing adaptivity.
             self.k = 0
 
         # initialise counter of how many times, adapt() has been called..
         self.t = 0
 
     def setup_proposal(self, **kwargs):
-
         # set the covariance operator
         self.C = kwargs["posterior"].prior.cov
 
         # extract the dimensionality.
         self.d = self.C.shape[0]
 
         # set the distribution mean to zero.
@@ -394,15 +385,14 @@
         Computes the acceptance probability given a proposal link and the
         previous link.
     """
 
     def __init__(
         self, C0, sd=None, epsilon=1e-6, t0=0, period=100, adaptive=False, gamma=1.01
     ):
-
         """
         Parameters
         ----------
         C0 : np.ndarray
             The initial covariance matrix of the proposal distribution.
         sd : None or float, optional
             The AM scaling parameter. Default is None (compute from target
@@ -460,15 +450,14 @@
         self.period = period
 
         # set adaptivity.
         self.adaptive = adaptive
 
         # if adaptive, set some adaptivity parameters
         if self.adaptive:
-
             # adaptivity scaling.
             self.gamma = gamma
             # initialise adaptivity counter for diminishing adaptivity.
             self.k = 0
 
         # set a counter of how many times, adapt() has been called.
         self.t = 0
@@ -480,52 +469,36 @@
             kwargs["parameters"],
             np.zeros((self.d, self.d)),
             sd=self.sd,
             epsilon=self.epsilon,
         )
 
     def adapt(self, **kwargs):
-
         super().adapt(**kwargs)
 
         # AM is adaptive per definition. update the RecursiveSampleMoments
         # with the given parameters.
         self.AM_recursor.update(kwargs["parameters"])
 
         if self.t >= self.t0 and self.t % self.period == 0:
             self.C = self.AM_recursor.get_sigma()
         else:
             pass
 
 
-class AdaptiveCrankNicolson(CrankNicolson):
+class OperatorWeightedCrankNicolson(CrankNicolson):
 
-    """Adaptive preconditioned Crank-Nicolson proposal, according to Hu and Yao
-    (2016).
+    """Operator-weighted preconditioned Crank-Nicolson proposal (Law 2014).
 
     Attributes
     ----------
-    C : np.ndarray
-        The initial covariance matrix of the proposal distribution.
-    d : int
-        The dimension of the target distribution.
-    scaling : float
-        The global scaling ("beta") of the proposal.
-    J : int
-        The truncation index, i.e. only dimensions below this index will be
-        adapted.
     B : numpy.ndarray
-        The adapted covariance matrix of the proposal distribution.
-    L : numpy.ndarray
-        Precision matrix of the prior, i.e. the inverse of the initial covariance
-        matrix.
-    operator : numpy.ndarray
-        The adaptive pCN scaling operator. To avoid recomputing the scaling
-        operator at each step, this array caches the result of
-        sqrtm(eye(d) - beta**2*np.dot(B, L))
+        The scaling operator of the proposal distribution.
+    scaling : float
+        The global scaling of the proposal.
     t0 : int
         When to start adapting the covariance matrix.
     adaptive : bool
         Whether to adapt the global scaling of the proposal.
     gamma : float
         The adaptivity coefficient for the global adaptive scaling.
     period : int
@@ -546,132 +519,83 @@
         Generates an adaptive pCN proposal from the input link using the
         proposal covariance.
     get_acceptance(proposal_link, previous_link)
         Computes the acceptance probability given a proposal link and the
         previous link.
     """
 
-    def __init__(
-        self, scaling=0.1, J=None, t0=0, period=100, adaptive=False, gamma=1.01
-    ):
+    def __init__(self, B, scaling=1.0, adaptive=False, gamma=1.01, period=100):
         """
         Parameters
         ----------
+        B : numpy.ndarray
+            The scaling operator of the proposal distribution.
         scaling : float, optional
-            The global scaling ("beta") of the proposal. Default is 0.1.
-        J : None or int, optional
-            The truncation index, i.e. only dimensions below this index will
-            be adapted.
-            Default is None (adapt all dimensions).
-        t0 : int, optional
-            When to start adapting the covariance matrix. Default is 0 (start
-            immediately).
-        period : int, optional
-            How often to adapt. Default is 100.
+            The global scaling of the proposal. Default is 1.0.
         adaptive : bool, optional
             Whether to adapt the global scaling of the proposal. Default is
             False.
         gamma : float, optional
             The adaptivity coefficient for the global adaptive scaling.
             Default is 1.01.
+        period : int, optional
+            How often to adapt. Default is 100.
         """
 
+        # set tge scaling operator
+        self.B = B
+
         # set the scaling.
         self.scaling = scaling
 
-        # truncation.
-        self.J = J
-
-        # set the beginning of adaptation (rigidness of initial covariance).
-        self.t0 = t0
-
-        # Set the update period.
-        self.period = period
-
         # set adaptivity.
         self.adaptive = adaptive
 
         # if adaptive, set some adaptivity parameters
         if self.adaptive:
-
             # adaptivity scaling.
             self.gamma = gamma
+            # adaptivity period (delay between adapting)
+            self.period = period
             # initialise adaptivity counter for diminishing adaptivity.
             self.k = 0
 
         # set a counter of how many times, adapt() has been called..
         self.t = 0
 
     def setup_proposal(self, **kwargs):
+        super().setup_proposal(**kwargs)
 
-        # set the initial covariance operator.
-        self.C = kwargs["posterior"].prior.cov
-
-        # extract the dimensionality.
-        self.d = self.C.shape[0]
-
-        # set a zero mean for the random draw.
-        self._mean = np.zeros(self.d)
-
-        # adaptive parameters
-        self.B = self.C.copy()
-        self.L = np.linalg.inv(self.C)
-        self.operator = sqrtm(
-            np.eye(self.d) - self.scaling**2 * np.dot(self.B, self.L)
-        )
-
-        # eigendecomposition of covariance matrix.
-        self.alpha, self.e = np.linalg.eig(self.C)
-        self.lamb = self.alpha.copy()
-
-        # truncation.
-        if self.J is None:
-            self.J = self.d
-
-        u_j = np.inner(kwargs["parameters"], self.e.T)
-        self.x_n = u_j
-        self.lamb_n = (self.x_n - u_j) ** 2
+        self.state_operator = np.real(sqrtm(np.eye(self.d) - self.scaling * self.B))
+        self.noise_operator = np.real(sqrtm(self.scaling * self.B))
 
     def adapt(self, **kwargs):
-
         super().adapt(**kwargs)
 
-        # ApCN is adaptive per definition. update the moments.
-        u_j = np.inner(kwargs["parameters"], self.e.T)
-        self.x_n = self.t / (self.t + 1) * self.x_n + 1 / (self.t + 1) * u_j
-        self.lamb_n = (
-            self.t / (self.t + 1) * self.lamb_n
-            + 1 / (self.t + 1) * (self.x_n - u_j) ** 2
-        )
-
-        # compute the operator, if the initial adaptation is complete and
-        # the period matches.
-        if self.t >= self.t0 and self.t % self.period == 0:
-            self.lamb[: self.J] = self.lamb_n[: self.J]
-            self.lamb[self.lamb > self.alpha] = self.alpha[self.lamb > self.alpha]
-            self.B = np.linalg.multi_dot((self.e, np.diag(self.lamb), self.e.T))
-            self.operator = sqrtm(
-                np.eye(self.d) - self.scaling**2 * np.dot(self.B, self.L)
-            )
-        else:
-            pass
+        if self.adaptive:
+            # make sure the periodicity is respected
+            if self.t % self.period == 0:
+                self.state_operator = np.real(
+                    sqrtm(np.eye(self.d) - self.scaling * self.B)
+                )
+                self.noise_operator = np.real(sqrtm(self.scaling * self.B))
 
     def make_proposal(self, link):
         # only use the adaptive proposal, if the initial time has passed.
 
         # make a proposal
-        return np.dot(
-            self.operator, link.parameters
-        ) + self.scaling * np.random.multivariate_normal(self._mean, self.B)
+        return np.dot(self.state_operator, link.parameters) + np.dot(
+            self.noise_operator, np.random.multivariate_normal(self._mean, self.C)
+        )
 
     def get_q(self, x_link, y_link):
         return stats.multivariate_normal.logpdf(
             y_link.parameters,
-            mean=np.dot(self.operator, x_link.parameters),
-            cov=self.scaling**2 * self.B,
+            mean=np.dot(self.state_operator, x_link.parameters),
+            cov=np.dot(self.scaling * self.B, self.C),
         )
 
 
 class SingleDreamZ(GaussianRandomWalk):
 
     """Dream(Z) proposal, similar to the DREAM(ZS) algorithm (see e.g. Vrugt
     2016).
@@ -735,15 +659,14 @@
         b_star=1e-6,
         Z_method="random",
         nCR=3,
         adaptive=False,
         gamma=1.01,
         period=100,
     ):
-
         """
         Parameters
         ----------
         M0 : np.ndarray
             Size of the initial archive.
         delta : int, optional
             Number of sample pairs from the archive to use to compute the
@@ -800,41 +723,38 @@
         # set crossover distribution.
         self.nCR = nCR
         self.mCR = None
         self.pCR = np.array(self.nCR * [1 / self.nCR])
 
         # if adaptive, set some adaptivity parameters
         if self.adaptive:
-
             # adaptivity scaling.
             self.gamma = gamma
             # adaptivity period (delay between adapting)
             self.period = period
             # initialise adaptivity counter for diminishing adaptivity.
             self.k = 0
 
         self.t = 0
 
     def setup_proposal(self, **kwargs):
-
         prior = kwargs["posterior"].prior
 
         # get the dimension and the initial scaling.
         self.d = prior.dim
 
         # these adaptivity parameters need to be mutable, so are only
         # initialised at setup.
         if self.adaptive:
             # DREAM-specific adaptivity
             self.LCR = np.zeros(self.nCR)
             self.DeltaCR = np.ones(self.nCR)
 
         # draw initial archive with latin hypercube sampling.
         if self.Z_method == "lhs":
-
             try:
                 lhs = stats.qmc.LatinHypercube(d=self.d)
                 self.Z = lhs.random(n=self.M)
                 self.Z = prior.ppf(self.Z)
                 return
 
             except AttributeError:
@@ -854,37 +774,34 @@
                     )
                     pass
 
         # do simple random sampling from the prior.
         self.Z = prior.rvs(self.M)
 
     def adapt(self, **kwargs):
-
         super().adapt(**kwargs)
 
         # extend the archive.
         self.Z = np.vstack((self.Z, kwargs["parameters"]))
         self.M = self.Z.shape[0]
 
         # adaptivity
         if self.adaptive and self.t % self.period == 0:
-
             # compute new multinomial distribution according to the normalised jumping distance.
             self.DeltaCR[self.mCR] = (
                 self.DeltaCR[self.mCR]
                 + (kwargs["jumping_distance"] ** 2 / np.var(self.Z, axis=0)).sum()
             )
             self.LCR[self.mCR] = self.LCR[self.mCR] + 1
 
             if np.all(self.LCR > 0):
                 DeltaCR_mean = self.DeltaCR / self.LCR
                 self.pCR = DeltaCR_mean / DeltaCR_mean.sum()
 
     def make_proposal(self, link):
-
         # initialise the jump vectors.
         Z_r1 = np.zeros(self.d)
         Z_r2 = np.zeros(self.d)
 
         # get jump vector components.
         for i in range(self.delta):
             r1, r2 = np.random.choice(self.M, 2, replace=False)
@@ -943,25 +860,23 @@
     accepted : list
         List of bool, signifying whether a proposal was accepted or not.
     is_local : list
         List of bool, signifying whether a link was created on the current
         level or by correction according to the next-finer level.
     adaptive_error_model : str or None
         The adaptive error model used, see e.g. Cui et al. (2019).
-    R : numpy.ndarray
-        Restriction matrix for the adaptive error model on the current level.
     bias : tinaDA.RecursiveSampleMoments
         A recursive Gaussian error model that computes the sample moments
         of the next-coarser bias.
 
     Methods
     ----------
-    setup_adaptive_error_model(biases, Rs)
-        Sets up the adaptive error model and passes the biases and restriction
-        matrices to the next-coarser level.
+    setup_adaptive_error_model(biases)
+        Sets up the adaptive error model and passes the biases to the
+        next-coarser level.
     align_chain(parameters, accepted)
         Makes sure the first link of the current level subchain is aligned
         with the next-finer level.
     make_mlda_proposal(subsampling_rate)
         Generates a proposal by creating a subchain of length subsampling_rate
         using MLDA and passing the final link to the next-finer level.
     make_base_proposal(subsampling_rate)
@@ -978,17 +893,15 @@
     def __init__(
         self,
         posteriors,
         proposal,
         subsampling_rates,
         initial_parameters,
         adaptive_error_model,
-        R,
     ):
-
         """
         Parameters
         ----------
         posteriors : list
             List of instances of tinyDA.Posterior, in increasing order.
         proposal : tinyDA.Proposal
             Transition kernel for coarsest MCMC proposals.
@@ -999,19 +912,14 @@
             Starting point for the MCMC sampler, default is None (random
             draw from prior).
         adaptive_error_model : str or None, optional
             The adaptive error model, see e.g. Cui et al. (2019). Default
             is None (no error model), options are 'state-independent' or
             'state-dependent'. If an error model is used, the likelihood
             MUST have a set_bias() method, use e.g. tinyDA.AdaptiveLogLike.
-        R : list or None, optional
-            Restriction matrices for the adaptive error model. If list of
-            restriction matrices is given, it must have length
-            len(posteriors) - 1 and they must be in increasing order,
-            as the model hierachy. Default is None (identity matrices).
         """
 
         # internalise the current level posterior and set the level.
         self.posterior = posteriors[-1]
         self.level = len(posteriors) - 1
         self.initial_parameters = initial_parameters
 
@@ -1026,45 +934,34 @@
         self.is_local.append(False)
 
         # set the adaptive error model as an attribute.
         self.adaptive_error_model = adaptive_error_model
 
         # if this level is not the coarsest level.
         if self.level > 0:
-
             # internalise the subsampling rate.
             self.subsampling_rate = subsampling_rates[-1]
 
             # set MDLA as the proposal on the next-coarser level.
             self.proposal = MLDA(
                 posteriors[:-1],
                 proposal,
                 subsampling_rates[:-1],
                 self.initial_parameters,
                 self.adaptive_error_model,
-                R[:-1],
             )
 
             # set the current level make_proposal method to MLDA.
             self.make_proposal = self.make_mlda_proposal
 
             # set up the adaptive error model.
             if self.adaptive_error_model is not None:
-
-                # set the restriction matrix for the current level.
-                self.R = R[-1]
-
-                # if no restriction matrix was given, create an identity matrix.
-                if self.R is None:
-                    self.R = np.eye(self.chain[-1].model_output.shape[0])
-
                 # compute the difference between coarse and fine level.
                 self.model_diff = (
-                    self.R.dot(self.chain[-1].model_output)
-                    - self.proposal.chain[-1].model_output
+                    self.chain[-1].model_output - self.proposal.chain[-1].model_output
                 )
 
                 # set up the state-independent adaptive error model.
                 if self.adaptive_error_model == "state-independent":
                     # for the state-independent error model, the bias is
                     # RecursiveSampleMoments, and the corrector is the mean
                     # of all sampled differences.
@@ -1076,132 +973,99 @@
                 # state-dependent error model has not been implemented, since
                 # it may not be ergodic.
                 elif self.adaptive_error_model == "state-dependent":
                     pass
 
         # if the current level is the coarsest one.
         elif self.level == 0:
-
             # use the coarsest level proposal.
             self.proposal = proposal
 
             # set up the proposal.
             self.proposal.setup_proposal(
                 parameters=self.initial_parameters, posterior=self.posterior
             )
 
             # set the current level make_proposal method to Metropolis-Hastings.
             self.make_proposal = self.make_base_proposal
 
-    def setup_adaptive_error_model(self, biases, Rs):
-
+    def setup_adaptive_error_model(self, biases):
         """
         Parameters
         ----------
         biases : list
             List of instances of tinyDA.RecursiveSampleMoments.
-        Rs: : list
-            List of restriction matrices.
         """
 
         # add the current level bias to the list.
         self.biases = [self.bias] + biases
 
-        # add the current level restriction matrix to the list.
-        self.Rs = [self.R] + Rs
-
-        # set up a list of recursive product of the restriction matrices.
-        self.R_products = [np.eye(self.Rs[0].shape[0])] * len(self.biases)
-
-        # compute the product of restriction matrices, as approptriate
-        # to each bias term.
-        for i, R in enumerate(self.Rs[:-1]):
-            for j in range(i + 1, len(self.Rs)):
-                self.R_products[j] = np.dot(self.R_products[j], R)
-
         # compute the total bias on the current level.
-        mu_bias = np.sum(
-            [np.dot(R, bias.get_mu()) for R, bias in zip(self.R_products, self.biases)],
-            axis=0,
-        )
-        sigma_bias = np.sum(
-            [
-                np.linalg.multi_dot((R, bias.get_sigma(), R.T))
-                for R, bias in zip(self.R_products, self.biases)
-            ],
-            axis=0,
-        )
+        mu_bias = np.sum([bias.get_mu() for bias in self.biases], axis=0)
+        sigma_bias = np.sum([bias.get_sigma() for bias in self.biases], axis=0)
 
         # set the bias on the next-coarser level.
         self.proposal.posterior.likelihood.set_bias(mu_bias, sigma_bias)
 
         # update the first coarser link with the adaptive error model.
         self.proposal.chain[-1] = self.proposal.posterior.update_link(
             self.proposal.chain[-1]
         )
 
-        # pass the list of biases and restriction matrices on the the next level.
+        # pass the list of biases on to the next level.
         if self.level > 1:
-            self.proposal.setup_adaptive_error_model(self.biases, self.Rs)
+            self.proposal.setup_adaptive_error_model(self.biases)
 
     def align_chain(self, parameters, accepted):
-
         """
         Parameters
         ----------
         parameters : numpy.ndarray
             The latest accepted parameters on the next-finer level.
         accepted : bool
             Whether the passed parameters were accepted on the next-higher
             level.
         """
 
         # append the latest link on the current level matching the parameters.
         self.chain.append(
-            next(
-                filter(
-                    lambda link: link.parameters is parameters, self.chain[::-1]
-                )
-            )
+            next(filter(lambda link: link.parameters is parameters, self.chain[::-1]))
         )
 
         # add the acceptance bool to the history.
         self.accepted.append(accepted)
 
         # the appended link is not local.
         self.is_local.append(False)
 
         # perpetuate the correction downward in the model hierachy.
         if self.level > 1:
             self.proposal.align_chain(parameters, accepted)
 
     def make_mlda_proposal(self, subsampling_rate):
-
         """
         Parameters
         ----------
         subsampling rate : int
             The number of samples drawn in the subchain.
         """
 
         # iterate through the subsamples.
         for i in range(subsampling_rate):
-
             # create a proposal from the next-lower level,
             proposal = self.proposal.make_proposal(self.subsampling_rate)
 
             # if there were no acceptances on the next-lower level, repeat previous sample.
             if sum(self.proposal.accepted[-self.subsampling_rate :]) == 0:
                 self.chain.append(self.chain[-1])
                 self.accepted.append(False)
                 self.is_local.append(True)
 
             # otherwise, evaluate the model.
             else:
-
                 # create a link from that proposal.
                 proposal_link = self.posterior.create_link(proposal)
 
                 # compute the MLDA acceptance probability..
                 alpha = self.proposal.get_acceptance(
                     proposal_link,
                     self.chain[-1],
@@ -1220,42 +1084,31 @@
                     self.is_local.append(True)
 
             # make sure the lower level chains are aligned with the current state.
             self.proposal.align_chain(self.chain[-1].parameters, self.accepted[-1])
 
             # apply the adaptive error model.
             if self.adaptive_error_model is not None:
-
                 # compute the difference between coarse and fine level.
                 if self.accepted[-1]:
                     self.model_diff = (
-                        self.R.dot(self.chain[-1].model_output)
+                        self.chain[-1].model_output
                         - self.proposal.chain[-1].model_output
                     )
 
                 if self.adaptive_error_model == "state-independent":
                     # for the state-independent error model, the bias is
                     # RecursiveSampleMoments, and the corrector is the mean
                     # of all sampled differences.
                     self.bias.update(self.model_diff)
 
                     # compute the entire bias correction.
-                    mu_bias = np.sum(
-                        [
-                            np.dot(R, bias.get_mu())
-                            for R, bias in zip(self.R_products, self.biases)
-                        ],
-                        axis=0,
-                    )
+                    mu_bias = np.sum([bias.get_mu() for bias in self.biases], axis=0)
                     sigma_bias = np.sum(
-                        [
-                            np.linalg.multi_dot((R, bias.get_sigma(), R.T))
-                            for R, bias in zip(self.R_products, self.biases)
-                        ],
-                        axis=0,
+                        [bias.get_sigma() for bias in self.biases], axis=0
                     )
 
                     # update the next-coarser likelihood with the bias.
                     self.proposal.posterior.likelihood.set_bias(mu_bias, sigma_bias)
 
                 # state-dependent error model has not been implemented.
                 elif self.adaptive_error_model == "state-dependent":
@@ -1266,18 +1119,16 @@
                     self.proposal.chain[-1]
                 )
 
         # return the latest link.
         return self.chain[-1].parameters
 
     def make_base_proposal(self, subsampling_rate):
-
         # iterate through the subsamples.
         for i in range(subsampling_rate):
-
             # draw a new proposal, given the previous parameters.
             proposal = self.proposal.make_proposal(self.chain[-1])
 
             # create a link from that proposal.
             proposal_link = self.posterior.create_link(proposal)
 
             # compute the acceptance probability, according to the proposal.
```

### Comparing `tinyda-0.9.8/tinyDA/ray.py` & `tinyda-0.9.9/tinyDA/ray.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,16 +120,14 @@
         The subsampling rate for the coarse chain.
     n_chains : int
         Number of parallel chains.
     initial_parameters : list
             Starting points for the MCMC samplers.
     adaptive_error_model : str or None
         The adaptive error model, see e.g. Cui et al. (2019).
-    R : numpy.ndarray
-        Restriction matrix for the adaptive error model.
     remote_chains : list
         List of Ray actors, each running an independent DA MCMC sampler.
     chains : list
         List of lists containing samples ("Links") in the fine MCMC chains.
     accepted : list
         List of lists of bool, signifying whether a proposal was accepted or not.
 
@@ -144,15 +142,14 @@
         posterior_coarse,
         posterior_fine,
         proposal,
         subsampling_rate=1,
         n_chains=2,
         initial_parameters=None,
         adaptive_error_model=None,
-        R=None,
     ):
 
         """
         Parameters
         ----------
         posterior_coarse : tinyDA.Posterior
             A "coarse" posterior responsible for communation between prior,
@@ -173,17 +170,14 @@
             Starting points for the MCMC samplers, default is None (random
             draws from prior).
         adaptive_error_model : str or None, optional
             The adaptive error model, see e.g. Cui et al. (2019). Default
             is None (no error model), options are 'state-independent' or
             'state-dependent'. If an error model is used, the likelihood MUST
             have a set_bias() method, use e.g. tinyDA.AdaptiveLogLike.
-        R : numpy.ndarray, optional
-            Restriction matrix for the adaptive error model. Default is None
-            (identity matrix).
         """
 
         # internalise posteriors, proposal and subsampling rate.
         self.posterior_coarse = posterior_coarse
         self.posterior_fine = posterior_fine
         self.proposal = proposal
         self.subsampling_rate = subsampling_rate
@@ -192,44 +186,41 @@
         self.n_chains = n_chains
 
         # set the initial parameters.
         self.initial_parameters = initial_parameters
 
         # set the adaptive error model
         self.adaptive_error_model = adaptive_error_model
-        self.R = R
 
         # initialise Ray.
         ray.init(ignore_reinit_error=True)
 
         # set up the parallel DA chains as Ray actors.
         self.remote_chains = [
             RemoteDAChain.remote(
                 self.posterior_coarse,
                 self.posterior_fine,
                 self.proposal[i],
                 self.subsampling_rate,
                 self.initial_parameters[i],
                 self.adaptive_error_model,
-                self.R,
             )
             for i in range(self.n_chains)
         ]
 
 
 class ParallelMLDAChain(ParallelChain):
     def __init__(
         self,
         posteriors,
         proposal,
         subsampling_rates=None,
         n_chains=2,
         initial_parameters=None,
         adaptive_error_model=None,
-        R=None,
     ):
 
         # internalise posteriors, proposal and subsampling rate.
         self.posteriors = posteriors
         self.proposal = proposal
         self.subsampling_rates = subsampling_rates
 
@@ -237,28 +228,26 @@
         self.n_chains = n_chains
 
         # set the initial parameters.
         self.initial_parameters = initial_parameters
 
         # set the adaptive error model
         self.adaptive_error_model = adaptive_error_model
-        self.R = R
 
         # initialise Ray.
         ray.init(ignore_reinit_error=True)
 
         # set up the parallel DA chains as Ray actors.
         self.remote_chains = [
             RemoteMLDAChain.remote(
                 self.posteriors,
                 self.proposal[i],
                 self.subsampling_rates,
                 self.initial_parameters[i],
                 self.adaptive_error_model,
-                self.R,
             )
             for i in range(self.n_chains)
         ]
 
 
 @ray.remote
 class RemoteChain(Chain):
```

### Comparing `tinyda-0.9.8/tinyDA/sampler.py` & `tinyda-0.9.9/tinyDA/sampler.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,19 +79,14 @@
         resulting in "classic" DA MCMC for a two-level model.
     adaptive_error_model : str or None, optional
         The adaptive error model, see e.g. Cui et al. (2019). If running
         single-level MCMC, this parameter is ignored. Default is None
         (no error model), options are 'state-independent' or 'state-dependent'.
         If an error model is used, the likelihood MUST have a set_bias()
         method, use e.g. tinyDA.AdaptiveGaussianLogLike.
-    R : list or numpy.ndarray or None, optional
-        Restriction matrix(-ces) for the adaptive error model. If list of
-        restriction matrices is given for MLDA sampler, they must be in
-        increasing order as the model hierachy. If running single-level
-        MCMC, this parameter is ignored. Default is None (identity matrix).
     force_sequential : bool, optional
         Whether to force sequential sampling, even if Ray is installed.
         Default is False.
     force_progress_bar : bool, optional
         Whether to force printing of progress bar for parallel sampling.
         This will result in "messy" progress bar output, unless Ray is
         patched.
@@ -203,62 +198,56 @@
                 posteriors,
                 proposal,
                 iterations,
                 n_chains,
                 initial_parameters,
                 subsampling_rate,
                 adaptive_error_model,
-                R,
             )
         # parallel sampling.
         else:
             samples = _sample_parallel_da(
                 posteriors,
                 proposal,
                 iterations,
                 n_chains,
                 initial_parameters,
                 subsampling_rate,
                 adaptive_error_model,
-                R,
                 force_progress_bar,
             )
 
     elif n_levels > 2:
 
         if isinstance(subsampling_rate, list):
             subsampling_rates = subsampling_rate
         elif isinstance(subsampling_rate, int):
             subsampling_rates = [subsampling_rate] * (len(posteriors) - 1)
-        if R is None:
-            R = [None] * (len(posteriors) - 1)
 
         # sequential sampling.
         if not ray_is_available or n_chains == 1 or force_sequential:
             samples = _sample_sequential_mlda(
                 posteriors,
                 proposal,
                 iterations,
                 n_chains,
                 initial_parameters,
                 subsampling_rates,
                 adaptive_error_model,
-                R,
             )
         # parallel sampling.
         else:
             samples = _sample_parallel_mlda(
                 posteriors,
                 proposal,
                 iterations,
                 n_chains,
                 initial_parameters,
                 subsampling_rates,
                 adaptive_error_model,
-                R,
                 force_progress_bar,
             )
 
     return samples
 
 
 def _sample_sequential(
@@ -307,15 +296,14 @@
     posteriors,
     proposal,
     iterations,
     n_chains,
     initial_parameters,
     subsampling_rate,
     adaptive_error_model,
-    R,
 ):
     """Helper function for tinyDA.sample()"""
 
     # initialise the chains and sample, sequentially.
     chains = []
     for i in range(n_chains):
         print("Sampling chain {}/{}".format(i + 1, n_chains))
@@ -323,15 +311,14 @@
             DAChain(
                 posteriors[0],
                 posteriors[1],
                 proposal[i],
                 subsampling_rate,
                 initial_parameters[i],
                 adaptive_error_model,
-                R,
             )
         )
         chains[i].sample(iterations)
 
     info = {
         "sampler": "DA",
         "n_chains": n_chains,
@@ -355,15 +342,14 @@
     posteriors,
     proposal,
     iterations,
     n_chains,
     initial_parameters,
     subsampling_rate,
     adaptive_error_model,
-    R,
     force_progress_bar,
 ):
     """Helper function for tinyDA.sample()"""
 
     print("Sampling {} chains in parallel".format(n_chains))
 
     # create a parallel sampling instance and sample.
@@ -371,15 +357,14 @@
         posteriors[0],
         posteriors[1],
         proposal,
         subsampling_rate,
         n_chains,
         initial_parameters,
         adaptive_error_model,
-        R,
     )
     chains.sample(iterations, force_progress_bar)
 
     info = {
         "sampler": "DA",
         "n_chains": n_chains,
         "iterations": iterations + 1,
@@ -401,15 +386,14 @@
     posteriors,
     proposal,
     iterations,
     n_chains,
     initial_parameters,
     subsampling_rates,
     adaptive_error_model,
-    R,
 ):
     """Helper function for tinyDA.sample()"""
 
     levels = len(posteriors)
 
     # initialise the chains and sample, sequentially.
     chains = []
@@ -418,15 +402,14 @@
         chains.append(
             MLDAChain(
                 posteriors,
                 proposal[i],
                 subsampling_rates,
                 initial_parameters[i],
                 adaptive_error_model,
-                R,
             )
         )
         chains[i].sample(iterations)
 
     info = {
         "sampler": "MLDA",
         "n_chains": n_chains,
@@ -460,15 +443,14 @@
     posteriors,
     proposal,
     iterations,
     n_chains,
     initial_parameters,
     subsampling_rates,
     adaptive_error_model,
-    R,
     force_progress_bar,
 ):
     """Helper function for tinyDA.sample()"""
 
     levels = len(posteriors)
 
     print("Sampling {} chains in parallel".format(n_chains))
@@ -477,15 +459,14 @@
     chains = ParallelMLDAChain(
         posteriors,
         proposal,
         subsampling_rates,
         n_chains,
         initial_parameters,
         adaptive_error_model,
-        R,
     )
     chains.sample(iterations, force_progress_bar)
 
     info = {
         "sampler": "MLDA",
         "n_chains": n_chains,
         "iterations": iterations + 1,
```

### Comparing `tinyda-0.9.8/tinyDA/umbridge.py` & `tinyda-0.9.9/tinyDA/umbridge.py`

 * *Files identical despite different names*

### Comparing `tinyda-0.9.8/tinyDA/utils.py` & `tinyda-0.9.9/tinyDA/utils.py`

 * *Files identical despite different names*

### Comparing `tinyda-0.9.8/setup.py` & `tinyda-0.9.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,17 @@
  'matplotlib>=3.5.2,<4.0.0',
  'numpy>=1.23.0,<2.0.0',
  'scipy>=1.8.0,<2.0.0',
  'tqdm>=4.64.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'tinyda',
-    'version': '0.9.8',
+    'version': '0.9.9',
     'description': 'Delayed Acceptance MCMC Sampler',
-    'long_description': "![](https://github.com/mikkelbue/tinyDA/blob/main/misc/tinyDA.png)\n\n# tinyDA\nMultilevel Delayed Acceptance MCMC sampler with finite-length subchain sampling and adaptive error modelling. This is intended as a simple, lightweight implementation, with minimal dependencies, i.e. nothing beyond the SciPy stack and ArviZ. It is fully imperative and easy to use!\n\nFor instructions, have a look at the [documentation](https://tinyda.readthedocs.io/en/latest/), the [examples](https://github.com/mikkelbue/tinyDA/tree/main/examples) or the [usage section below](#usage).\n\n## Installation\ntinyDA can be installed from PyPI:\n```\npip install tinyDA\n```\n\n## Dependencies\n* NumPy\n* SciPy\n* ArviZ\n* tqdm\n* [Ray](https://docs.ray.io/en/master/) (multiprocessing, optional)\n\n## Features\n\n### Samplers\n* Metropolis-Hastings\n* Delayed Acceptance (Christen & Fox, 2005)\n* Multilevel Delayed Acceptance (Lykkegaard et al. 2022)\n\n### Proposals\n* Random Walk Metropolis Hastings (RWMH) - Metropolis et al. (1953), Hastings (1970)\n* preconditioned Crank-Nicolson (pCN) - Cotter et al. (2013)\n* Adaptive Metropolis (AM) - Haario et al. (2001)\n* Adaptive pCN - Hu and Yao (2016)\n* DREAM(Z) - Vrugt (2016)\n* Multiple-Try Metropolis (MTM) - Liu et al. (2000)\n\n### Adaptive Error Models\n* State independent - Cui et al. (2018)\n* State dependent - Cui et al. (2018)\n\n### Diagnostics\n* Convert a tinyDA chain to an ArviZ InferenceData object for near-unlimited diagnostics!\n\n## Usage\nDocumentation is available at [Read the Docs](https://tinyda.readthedocs.io/en/latest/). A few illustrative examples are available as Jupyter Notebooks in the root directory. Below is a short summary of the core features.\n\n### Distributions\nThe prior and likelihood can be defined using standard `scipy.stats` classes:\n```python\nimport tinyDA as tda\n\nfrom scipy.stats import multivariate_normal\n\n# set the prior mean and covariance.\nmean_prior = np.zeros(n_dim)\ncov_prior = np.eye(n_dim)\n\n# set the covariance of the likelihood.\ncov_likelihood = sigma**2*np.eye(data.shape[0])\n\n# initialise the prior distribution and likelihood.\nmy_prior = multivariate_normal(mean_prior, cov_prior)\nmy_loglike = tda.GaussianLogLike(data, cov_likelihood)\n```\nIf using a Gaussian likelihood, we recommend using the `tinyDA` implementation, since it is unnormalised and plays along well with `tda.AdaptiveLogLike` used for the Adaptive Error Model. Home-brew distributions can easily be defined, and must have a `.rvs()` method for drawing random samples and a `logpdf(x)` method for computing the log-likelihood, as per the `SciPy` implementation.\n\n### tinyDA.Posterior\nThe heart of the TinyDA sampler is the `tinyDA.Posterior`, which is responsible for:\n1. Calling the model with some parameters (a proposal) and collecting the model output.\n2. Evaluating the prior density of the parameters, and the likelihood of the data, given the parameters.\n3. Constructing `tda.Link` instances that hold information for each sample.\n\n![](https://github.com/mikkelbue/tinyDA/blob/main/misc/flowchart.png)\n\nThe `tinyDA.Posterior` takes as input the prior, the likelihood, and a forward model. Therefore, a forward model must be defined. This model can be either a function `model_output = my_function(parameters)` or a class instance with a `.__call__(self, parameters)` method. The function or `__call__` method must return either just the model output or a tuple of `(model_output, qoi)`. In this example, we define a class that performs simple linear regression on whatever inputs `x` we have.\n\n```python\nclass MyLinearModel:\n    def __init__(self, x):\n\n        self.x = x\n        \n    def __call__(self, parameters):\n        \n        # the model output is a simple linear regression\n        model_output = parameters[0] + parameters[1]*self.x\n        \n        # no quantity of interest beyond the parameters.\n        qoi = None\n        \n        # return both.\n        return model_output, qoi\n\nmy_model = MyLinearModel(x)\nmy_posterior = tda.Posterior(my_prior, my_loglike, my_model)\n```\n\n### Proposals\nA proposal is simply initialised with its parameters:\n```python\n# set the covariance of the proposal distribution.\nam_cov = np.eye(n_dim)\n\n# set the number of iterations before starting adaptation.\nam_t0 = 1000\n\n# set some adaptive metropolis tuning parameters.\nam_sd = 1\nam_epsilon = 1e-6\n\n# initialise the proposal.\nmy_proposal = tda.AdaptiveMetropolis(C0=am_cov, t0=am_t0, sd=am_sd, epsilon=am_epsilon)\n```\n\n### Sampling\nAfter defining a proposal, a coarse posterior `my_posterior_coarse`, and a fine posterior `my_posterior_fine`, the Delayed Acceptance sampler can be run using `tinyDA.sample()`:\n```python\nmy_chains = tda.sample([my_posterior_coarse, my_posterior_fine], \n                       my_proposal, \n                       iterations=12000, \n                       n_chains=2, \n                       subsampling_rate=10)\n```\n\nIf using a hirarchy with more than two models, a Multilevel Delayed Acceptance sampler can be run by supplying a list of posteriors in ascending order and a correponsing list of subsampling rates:\n```python\nmy_chains = tda.sample([my_posterior_level0, \n                        my_posterior_level1, \n                        my_posterior_level2, \n                        my_posterior_level3], \n                       my_proposal, \n                       iterations=12000, \n                       n_chains=2, \n                       subsampling_rate=[10, 5, 5])\n```\n\n### Postprocessing\nThe entire sampling history is now stored in `my_chains` in the form of a dictionary with tinyDA.Link instances. You can convert the output of `tinyDA.sample()` to an ArviZ InferenceData object with \n```python\nidata = tda.to_inference_data(my_chains, burnin=2000)\n```\nIf you want to have a look at the coarse samples, you can pass an additional argument:\n```python\nidata = tda.to_inference_data(my_chains, level='coarse', burnin=20000)\n```\n\nThe `idata` object can then be used with the ArviZ diagnostics suite to e.g. get MCMC statistics, plot the traces and so on.\n\n## Contributing\nI (mikkelbue) am currently the sole contributor to this package. I have been using it in my own research, and have so far been developing it (mostly) for myself. \n\nIf you feel that it is missing some features, or that something could be improved, please do not hesitate to create a fork and submit a PR! If you want to help me improve the package, please have a look at the [issues](https://github.com/mikkelbue/tinyDA/issues) and consider if something seems doable to you. I am currently working on a scientific paper that I plan to submit to Journal of Statistical Software, and would be happy for other people to get involved.\n\nIf you would like to contribute, please consider the following:\n* I am hoping to keep the list of dependencies **short**, and would rather not include any additional large libraries, unless it is strongly warranted. Great things can be achieved using NumPy!\n* I am pretty good at converting theoretical methods into computer code, but I am not a software engineer. Any kind of CI, tests and improvements to the software infrastructure would be greatly appreciated!\n\n## TODO\n* ~~Parallel multi-chain sampling~~\n* ~~More user-friendly diagnostics~~\n* ~~Multilevel Delayed Acceptance~~\n* Variance Reduction\n* MALA proposal\n* Wrapper for framework-agnostic adaptive coarse model\n* Embedded spaces for hierachical models\n* Tests\n\n\n",
+    'long_description': "![](https://github.com/mikkelbue/tinyDA/blob/main/misc/tinyDA.png)\n\n# tinyDA\nMultilevel Delayed Acceptance MCMC sampler with finite-length subchain sampling and adaptive error modelling. This is intended as a simple, lightweight implementation, with minimal dependencies, i.e. nothing beyond the SciPy stack and ArviZ. It is fully imperative and easy to use!\n\nFor instructions, have a look at the [documentation](https://tinyda.readthedocs.io/en/latest/), the [examples](https://github.com/mikkelbue/tinyDA/tree/main/examples) or the [usage section below](#usage).\n\n## Installation\ntinyDA can be installed from PyPI:\n```\npip install tinyDA\n```\n\n## Dependencies\n* NumPy\n* SciPy\n* ArviZ\n* tqdm\n* [Ray](https://docs.ray.io/en/master/) (multiprocessing, optional)\n\n## Features\n\n### Samplers\n* Metropolis-Hastings\n* Delayed Acceptance (Christen & Fox, 2005)\n* Multilevel Delayed Acceptance (Lykkegaard et al. 2022)\n\n### Proposals\n* Random Walk Metropolis Hastings (RWMH) - Metropolis et al. (1953), Hastings (1970)\n* preconditioned Crank-Nicolson (pCN) - Cotter et al. (2013)\n* Adaptive Metropolis (AM) - Haario et al. (2001)\n* Operator-weighted pCN - Law (2014)\n* DREAM(Z) - Vrugt (2016)\n* Multiple-Try Metropolis (MTM) - Liu et al. (2000)\n\n### Adaptive Error Models\n* State independent - Cui et al. (2018)\n* State dependent - Cui et al. (2018)\n\n### Diagnostics\n* Convert a tinyDA chain to an ArviZ InferenceData object for near-unlimited diagnostics!\n\n## Usage\nDocumentation is available at [Read the Docs](https://tinyda.readthedocs.io/en/latest/). A few illustrative examples are available as Jupyter Notebooks in the root directory. Below is a short summary of the core features.\n\n### Distributions\nThe prior and likelihood can be defined using standard `scipy.stats` classes:\n```python\nimport tinyDA as tda\n\nfrom scipy.stats import multivariate_normal\n\n# set the prior mean and covariance.\nmean_prior = np.zeros(n_dim)\ncov_prior = np.eye(n_dim)\n\n# set the covariance of the likelihood.\ncov_likelihood = sigma**2*np.eye(data.shape[0])\n\n# initialise the prior distribution and likelihood.\nmy_prior = multivariate_normal(mean_prior, cov_prior)\nmy_loglike = tda.GaussianLogLike(data, cov_likelihood)\n```\nIf using a Gaussian likelihood, we recommend using the `tinyDA` implementation, since it is unnormalised and plays along well with `tda.AdaptiveLogLike` used for the Adaptive Error Model. Home-brew distributions can easily be defined, and must have a `.rvs()` method for drawing random samples and a `logpdf(x)` method for computing the log-likelihood, as per the `SciPy` implementation.\n\n### tinyDA.Posterior\nThe heart of the TinyDA sampler is the `tinyDA.Posterior`, which is responsible for:\n1. Calling the model with some parameters (a proposal) and collecting the model output.\n2. Evaluating the prior density of the parameters, and the likelihood of the data, given the parameters.\n3. Constructing `tda.Link` instances that hold information for each sample.\n\n![](https://github.com/mikkelbue/tinyDA/blob/main/misc/flowchart.png)\n\nThe `tinyDA.Posterior` takes as input the prior, the likelihood, and a forward model. Therefore, a forward model must be defined. This model can be either a function `model_output = my_function(parameters)` or a class instance with a `.__call__(self, parameters)` method. The function or `__call__` method must return either just the model output or a tuple of `(model_output, qoi)`. In this example, we define a class that performs simple linear regression on whatever inputs `x` we have.\n\n```python\nclass MyLinearModel:\n    def __init__(self, x):\n\n        self.x = x\n        \n    def __call__(self, parameters):\n        \n        # the model output is a simple linear regression\n        model_output = parameters[0] + parameters[1]*self.x\n        \n        # no quantity of interest beyond the parameters.\n        qoi = None\n        \n        # return both.\n        return model_output, qoi\n\nmy_model = MyLinearModel(x)\nmy_posterior = tda.Posterior(my_prior, my_loglike, my_model)\n```\n\n### Proposals\nA proposal is simply initialised with its parameters:\n```python\n# set the covariance of the proposal distribution.\nam_cov = np.eye(n_dim)\n\n# set the number of iterations before starting adaptation.\nam_t0 = 1000\n\n# set some adaptive metropolis tuning parameters.\nam_sd = 1\nam_epsilon = 1e-6\n\n# initialise the proposal.\nmy_proposal = tda.AdaptiveMetropolis(C0=am_cov, t0=am_t0, sd=am_sd, epsilon=am_epsilon)\n```\n\n### Sampling\nAfter defining a proposal, a coarse posterior `my_posterior_coarse`, and a fine posterior `my_posterior_fine`, the Delayed Acceptance sampler can be run using `tinyDA.sample()`:\n```python\nmy_chains = tda.sample([my_posterior_coarse, my_posterior_fine], \n                       my_proposal, \n                       iterations=12000, \n                       n_chains=2, \n                       subsampling_rate=10)\n```\n\nIf using a hirarchy with more than two models, a Multilevel Delayed Acceptance sampler can be run by supplying a list of posteriors in ascending order and a correponsing list of subsampling rates:\n```python\nmy_chains = tda.sample([my_posterior_level0, \n                        my_posterior_level1, \n                        my_posterior_level2, \n                        my_posterior_level3], \n                       my_proposal, \n                       iterations=12000, \n                       n_chains=2, \n                       subsampling_rate=[10, 5, 5])\n```\n\n### Postprocessing\nThe entire sampling history is now stored in `my_chains` in the form of a dictionary with tinyDA.Link instances. You can convert the output of `tinyDA.sample()` to an ArviZ InferenceData object with \n```python\nidata = tda.to_inference_data(my_chains, burnin=2000)\n```\nIf you want to have a look at the coarse samples, you can pass an additional argument:\n```python\nidata = tda.to_inference_data(my_chains, level='coarse', burnin=20000)\n```\n\nThe `idata` object can then be used with the ArviZ diagnostics suite to e.g. get MCMC statistics, plot the traces and so on.\n\n## Contributing\nI (mikkelbue) am currently the sole contributor to this package. I have been using it in my own research, and have so far been developing it (mostly) for myself. \n\nIf you feel that it is missing some features, or that something could be improved, please do not hesitate to create a fork and submit a PR! If you want to help me improve the package, please have a look at the [issues](https://github.com/mikkelbue/tinyDA/issues) and consider if something seems doable to you. I am currently working on a scientific paper that I plan to submit to Journal of Statistical Software, and would be happy for other people to get involved.\n\nIf you would like to contribute, please consider the following:\n* I am hoping to keep the list of dependencies **short**, and would rather not include any additional large libraries, unless it is strongly warranted. Great things can be achieved using NumPy!\n* I am pretty good at converting theoretical methods into computer code, but I am not a software engineer. Any kind of CI, tests and improvements to the software infrastructure would be greatly appreciated!\n\n## TODO\n* ~~Parallel multi-chain sampling~~\n* ~~More user-friendly diagnostics~~\n* ~~Multilevel Delayed Acceptance~~\n* Variance Reduction\n* MALA proposal\n* Wrapper for framework-agnostic adaptive coarse model\n* Embedded spaces for hierachical models\n* Tests\n\n\n",
     'author': 'Mikkel Bue Lykkegaard',
     'author_email': 'mikkelbue@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/mikkelbue/tinyda',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `tinyda-0.9.8/PKG-INFO` & `tinyda-0.9.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: tinyda
-Version: 0.9.8
+Version: 0.9.9
 Summary: Delayed Acceptance MCMC Sampler
 Home-page: https://github.com/mikkelbue/tinyda
 License: MIT
 Author: Mikkel Bue Lykkegaard
 Author-email: mikkelbue@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: arviz (>=0.12.1,<0.13.0)
 Requires-Dist: matplotlib (>=3.5.2,<4.0.0)
 Requires-Dist: numpy (>=1.23.0,<2.0.0)
 Requires-Dist: scipy (>=1.8.0,<2.0.0)
 Requires-Dist: tqdm (>=4.64.0,<5.0.0)
 Project-URL: Bug Tracker, https://github.com/mikkelbue/tinyDA/issues
@@ -51,15 +52,15 @@
 * Delayed Acceptance (Christen & Fox, 2005)
 * Multilevel Delayed Acceptance (Lykkegaard et al. 2022)
 
 ### Proposals
 * Random Walk Metropolis Hastings (RWMH) - Metropolis et al. (1953), Hastings (1970)
 * preconditioned Crank-Nicolson (pCN) - Cotter et al. (2013)
 * Adaptive Metropolis (AM) - Haario et al. (2001)
-* Adaptive pCN - Hu and Yao (2016)
+* Operator-weighted pCN - Law (2014)
 * DREAM(Z) - Vrugt (2016)
 * Multiple-Try Metropolis (MTM) - Liu et al. (2000)
 
 ### Adaptive Error Models
 * State independent - Cui et al. (2018)
 * State dependent - Cui et al. (2018)
```

