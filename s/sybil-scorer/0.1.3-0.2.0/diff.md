# Comparing `tmp/sybil-scorer-0.1.3.tar.gz` & `tmp/sybil-scorer-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sybil-scorer-0.1.3.tar", last modified: Wed Jun  7 16:11:51 2023, max compression
+gzip compressed data, was "sybil-scorer-0.2.0.tar", last modified: Thu Jun 29 10:43:45 2023, max compression
```

## Comparing `sybil-scorer-0.1.3.tar` & `sybil-scorer-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 16:11:50.988542 sybil-scorer-0.1.3/
--rw-rw-rw-   0        0        0     1084 2023-01-29 12:58:09.000000 sybil-scorer-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     9689 2023-06-07 16:11:50.989545 sybil-scorer-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     7755 2023-05-05 09:28:10.000000 sybil-scorer-0.1.3/README.md
--rw-rw-rw-   0        0        0     1142 2023-06-07 16:06:07.000000 sybil-scorer-0.1.3/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-06-07 16:11:50.906542 sybil-scorer-0.1.3/sbscorer/
-drwxrwxrwx   0        0        0        0 2023-06-07 16:11:50.938541 sybil-scorer-0.1.3/sbscorer/sbdata/
--rw-rw-rw-   0        0        0    22880 2023-05-08 09:36:36.000000 sybil-scorer-0.1.3/sbscorer/sbdata/FlipsideApi.py
--rw-rw-rw-   0        0        0        0 2023-01-17 19:51:41.000000 sybil-scorer-0.1.3/sbscorer/sbdata/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 16:11:50.942541 sybil-scorer-0.1.3/sbscorer/sblegos/
--rw-rw-rw-   0        0        0    18460 2023-06-07 16:04:36.000000 sybil-scorer-0.1.3/sbscorer/sblegos/TransactionAnalyser.py
--rw-rw-rw-   0        0        0        0 2023-01-21 08:46:58.000000 sybil-scorer-0.1.3/sbscorer/sblegos/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 16:11:50.946539 sybil-scorer-0.1.3/sbscorer/sbutils/
--rw-rw-rw-   0        0        0     5318 2023-01-30 19:57:35.000000 sybil-scorer-0.1.3/sbscorer/sbutils/LoadData.py
--rw-rw-rw-   0        0        0        0 2023-01-17 19:51:41.000000 sybil-scorer-0.1.3/sbscorer/sbutils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 16:11:50.986542 sybil-scorer-0.1.3/sbscorer/sybil_scorer.egg-info/
--rw-rw-rw-   0        0        0     9689 2023-06-07 16:11:50.000000 sybil-scorer-0.1.3/sbscorer/sybil_scorer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      452 2023-06-07 16:11:50.000000 sybil-scorer-0.1.3/sbscorer/sybil_scorer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 16:11:50.000000 sybil-scorer-0.1.3/sbscorer/sybil_scorer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      150 2023-06-07 16:11:50.000000 sybil-scorer-0.1.3/sbscorer/sybil_scorer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-06-07 16:11:50.000000 sybil-scorer-0.1.3/sbscorer/sybil_scorer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      748 2023-06-07 16:11:51.003541 sybil-scorer-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-29 10:43:45.883710 sybil-scorer-0.2.0/
+-rw-rw-rw-   0        0        0     1084 2023-01-29 12:58:09.000000 sybil-scorer-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     9689 2023-06-29 10:43:45.884708 sybil-scorer-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7755 2023-05-05 09:28:10.000000 sybil-scorer-0.2.0/README.md
+-rw-rw-rw-   0        0        0     1142 2023-06-29 10:38:40.000000 sybil-scorer-0.2.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-06-29 10:43:45.821710 sybil-scorer-0.2.0/sbscorer/
+drwxrwxrwx   0        0        0        0 2023-06-29 10:43:45.836711 sybil-scorer-0.2.0/sbscorer/sbdata/
+-rw-rw-rw-   0        0        0    22880 2023-05-08 09:36:36.000000 sybil-scorer-0.2.0/sbscorer/sbdata/FlipsideApi.py
+-rw-rw-rw-   0        0        0        0 2023-01-17 19:51:41.000000 sybil-scorer-0.2.0/sbscorer/sbdata/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 10:43:45.843711 sybil-scorer-0.2.0/sbscorer/sblegos/
+-rw-rw-rw-   0        0        0    27938 2023-06-29 10:33:57.000000 sybil-scorer-0.2.0/sbscorer/sblegos/TransactionAnalyser.py
+-rw-rw-rw-   0        0        0     9373 2023-06-09 19:15:54.000000 sybil-scorer-0.2.0/sbscorer/sblegos/TransactionAnalyserTest.py
+-rw-rw-rw-   0        0        0        0 2023-01-21 08:46:58.000000 sybil-scorer-0.2.0/sbscorer/sblegos/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 10:43:45.847711 sybil-scorer-0.2.0/sbscorer/sbutils/
+-rw-rw-rw-   0        0        0     5318 2023-01-30 19:57:35.000000 sybil-scorer-0.2.0/sbscorer/sbutils/LoadData.py
+-rw-rw-rw-   0        0        0        0 2023-01-17 19:51:41.000000 sybil-scorer-0.2.0/sbscorer/sbutils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 10:43:45.881708 sybil-scorer-0.2.0/sbscorer/sybil_scorer.egg-info/
+-rw-rw-rw-   0        0        0     9689 2023-06-29 10:43:45.000000 sybil-scorer-0.2.0/sbscorer/sybil_scorer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      496 2023-06-29 10:43:45.000000 sybil-scorer-0.2.0/sbscorer/sybil_scorer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 10:43:45.000000 sybil-scorer-0.2.0/sbscorer/sybil_scorer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      150 2023-06-29 10:43:45.000000 sybil-scorer-0.2.0/sbscorer/sybil_scorer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-06-29 10:43:45.000000 sybil-scorer-0.2.0/sbscorer/sybil_scorer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      748 2023-06-29 10:43:45.894711 sybil-scorer-0.2.0/setup.cfg
```

### Comparing `sybil-scorer-0.1.3/LICENSE` & `sybil-scorer-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sybil-scorer-0.1.3/PKG-INFO` & `sybil-scorer-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sybil-scorer
-Version: 0.1.3
+Version: 0.2.0
 Summary: A sybil scoring tool
 Home-page: https://github.com/poupou-web3/cluster-scorer
 Author: Poupou
 Author-email: Poupou <poupou-web3@protonmail.com>
 License: MIT License
         
         Copyright (c) 2023 Poupou
```

### Comparing `sybil-scorer-0.1.3/README.md` & `sybil-scorer-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `sybil-scorer-0.1.3/pyproject.toml` & `sybil-scorer-0.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=61.0.0', "wheel"]
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "sybil-scorer"
-version = "0.1.3"
+version = "0.2.0"
 description = "A sybil scoring tool"
 readme = "README.md"
 authors = [{ name = "Poupou", email = "poupou-web3@protonmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `sybil-scorer-0.1.3/sbscorer/sbdata/FlipsideApi.py` & `sybil-scorer-0.2.0/sbscorer/sbdata/FlipsideApi.py`

 * *Files identical despite different names*

### Comparing `sybil-scorer-0.1.3/sbscorer/sblegos/TransactionAnalyser.py` & `sybil-scorer-0.2.0/sbscorer/sblegos/TransactionAnalyser.py`

 * *Files 19% similar despite different names*

```diff
@@ -27,27 +27,38 @@
         Parameters
         ----------
         df_transactions : pd.DataFrame
             The dataframe containing all the transactions of the addresses
         df_address : pd.DataFrame
             The dataframe containing a 'address' column 
         """
-        self.df_transactions = df_transactions
-        # holds a df of address/seed wallet we don't have to create it each time
+        assert isinstance(df_transactions, pd.DataFrame), "The df_transactions should be a pd.DataFrame"
+        assert isinstance(df_address, pd.DataFrame), "The df_address should be a pd.DataFrame"
+        assert 'address' in df_address.columns, "The df_address should contain a column 'address'"
+
+        self.gb_EOA_sorted = None
         self.df_seed_wallet_naive = None
         self.df_seed_wallet = None
-        self.gb_EOA_sorted = None
-        self.df_address = df_address
-        # We use a df address we can load all transactions in memory and then change the address list easily
-        # for example to calculate on a specific project
+        self.details_first_incoming_transaction = None
+        self.details_first_outgoing_transaction = None
+        self.df_transactions = df_transactions
 
         # store the array of string transactions
+        self.dict_add_interacted = None
         self.dict_add_string_tx = None
         self.dict_add_value_string_tx = None
 
+        # set objects
+        self.set_group_by_sorted_EOA()
+        self.set_seed_wallet_naive()
+        self.set_seed_wallet()
+        self.df_address = df_address
+        self.set_details_first_incoming_transaction()
+        self.set_details_first_outgoing_transaction()
+
     def has_same_seed_naive(self, address):
         """
         Return if the address has the same seed wallet as one of the seed wallet of the df_transactions
 
         If the df_seed_wallet is not set, it will set it
         Note df_transaction could contain transactions from multiple network but the seed wallet of the address is
         filtered which prevent unexpected raise of the boolean.
@@ -145,16 +156,14 @@
 
         Returns
         -------
         None
             Set the df_seed_wallet_naive attribute of the class
 
         """
-        if self.gb_EOA_sorted is None:
-            self.set_group_by_sorted_EOA()
         self.df_seed_wallet_naive = self.gb_EOA_sorted.first().loc[:, ['from_address', 'to_address']]
 
     def set_seed_wallet(self):
         """
         Set the df_seed_wallet attribute of the class. It holds the seed wallet of the addresses in 'EOA'
         of df_transactions. It is a non-naive method that look for the first incoming transaction of the address to get
         the seed wallet.
@@ -174,16 +183,50 @@
 
         Returns
         -------
         None
             Set the gb_EOA_sorted attribute of the class
 
         """
-        if self.gb_EOA_sorted is None:
-            self.gb_EOA_sorted = self.df_transactions.sort_values('block_timestamp', ascending=True).groupby('EOA')
+        self.gb_EOA_sorted = self.df_transactions.sort_values('block_timestamp', ascending=True).groupby('EOA')
+
+    def set_details_first_incoming_transaction(self):
+        """
+        Set the details_first_incoming_transaction attribute of the class. It holds the details of the first incoming
+        transaction of the address given in parameter
+        Parameters
+        ----------
+
+        Returns
+        -------
+        None
+            Set the details_first_incoming_transaction attribute of the class
+
+        """
+        df_filtered = self.df_transactions[self.df_transactions['EOA'] == self.df_transactions['to_address']]
+        df_gb = df_filtered.sort_values('block_timestamp', ascending=True).groupby('EOA').first()
+        cols = ['from_address', 'gas_limit', 'gas_used', 'eth_value', 'block_timestamp']
+        df_gb_first = df_gb.loc[:, cols].reset_index()
+        self.details_first_incoming_transaction = df_gb_first.rename(columns=dict(from_address='first_in_tx_from',
+                                                                                  gas_limit='first_in_tx_gas_limit',
+                                                                                  gas_used='first_in_tx_gas_used',
+                                                                                  eth_value='first_in_tx_eth_value',
+                                                                                  block_timestamp='first_in_tx_timestamp'))
+
+    def set_details_first_outgoing_transaction(self):
+
+        df_filtered = self.df_transactions[self.df_transactions['EOA'] == self.df_transactions['from_address']]
+        df_gb = df_filtered.sort_values('block_timestamp', ascending=True).groupby('EOA').first()
+        cols = ['to_address', 'gas_limit', 'gas_used', 'eth_value', 'block_timestamp']
+        df_gb_first = df_gb.loc[:, cols].reset_index()
+        self.details_first_outgoing_transaction = df_gb_first.rename(columns=dict(from_address='first_out_tx_from',
+                                                                                  gas_limit='first_out_tx_gas_limit',
+                                                                                  gas_used='first_out_tx_gas_used',
+                                                                                  eth_value='first_out_tx_eth_value',
+                                                                                  block_timestamp='first_out_tx_timestamp'))
 
     def has_less_than_n_transactions(self, address, n=5):
         """
         Return a boolean whether the address has less than n transactions
         Parameters
         ----------
         address : str
@@ -192,40 +235,121 @@
             The number of transactions
 
         Returns
         -------
         has_less_than_n_transactions : bool
             True if the address has less than n transactions
         """
-        self.set_group_by_sorted_EOA()
-        return self.gb_EOA_sorted.get_group(address).shape[0] < n
+        return self.count_transactions(address) < n
+
+    def count_transactions(self, address):
+        """
+        Return the number of transactions of the address
+        Parameters
+        ----------
+        address : str
+            The address to check
+
+        Returns
+        -------
+        count_transactions : int
+            The number of transactions of the address
+        """
+        return self.gb_EOA_sorted.get_group(address).shape[0]
+
+    def set_dict_add_interacted(self):
+        """
+        Set the dict_add_interacted attribute of the class. It holds a dictionary of address as key and the list of
+        address interacted with as value.
+        Returns None
+        -------
+
+        """
+        if self.dict_add_interacted is None:
+            dict_add_interacted = {}
+            contributors = self.get_contributors()
+            for address in contributors:
+                df = self.gb_EOA_sorted.get_group(address)
+                add_interacted = np.append(df['to_address'].to_numpy(), df['from_address'].to_numpy())
+                add_interacted = add_interacted.astype('str')
+                unique_add_interacted = np.unique(add_interacted)
+                unique_add_interacted = unique_add_interacted[unique_add_interacted != address]
+                dict_add_interacted[address] = unique_add_interacted
+            self.dict_add_interacted = dict_add_interacted
+
+    def count_interaction_with_other_contributor(self, address):
+        """
+        Return the number of interactions of the address with other contributor (not itself)
+        Parameters
+        ----------
+        address : str
+            The address to check
+
+        Returns
+        -------
+        count_interaction_with_other_contributor : int
+            The number of interactions of the address with other contributor (not itself)
+        """
+        self.set_dict_add_interacted()
+        contributors = self.get_contributors()
+        other_contributors = contributors[contributors != address]
+
+        return self.count_interaction_any(address, other_contributors)
 
     def has_interacted_with_other_contributor(self, address):
         """
         Return a boolean whether the address has interacted with other contributor (not itself)
         Parameters
         ----------
         address : str
             The address to check
 
         Returns
         -------
         has_interacted_with_other_contributor : bool
             True if the address has interacted with one or more contributor of the grant
         """
-        self.set_group_by_sorted_EOA()
-        contributors = self.get_contributors()
-        other_contributors = contributors[contributors != address]
+        return self.count_interaction_with_other_contributor(address) > 0
+
+    def count_interaction_any(self, address, array_address):
+        """
+        Return an integer of the number of interactions with the addresses in the array_address
+        Parameters
+        ----------
+        address : str
+            The address to check
+        array_address : narray
+            The array of addresses to check
+
+        Returns
+        -------
+        count_interaction_with_any : int
+            The number of interactions with the addresses in the array_address
+        """
 
-        df = self.gb_EOA_sorted.get_group(address)
-        add_interacted = np.append(df['to_address'].to_numpy(), df['from_address'].to_numpy())
-        add_interacted = add_interacted.astype('str')
-        unique_add_interacted = np.unique(add_interacted)
-        unique_add_interacted = unique_add_interacted[unique_add_interacted != address]
-        return np.isin(unique_add_interacted, other_contributors).any()
+        unique_add_interacted = self.dict_add_interacted[address]
+        return np.isin(unique_add_interacted, array_address).sum()
+
+    def has_interacted_with_any(self, address, array_address):
+        """
+        Return a boolean whether the address has interacted with any address in the array_address
+        Parameters
+        ----------
+        address : str
+            The address to check
+        array_address : narray
+            The array of addresses to check
+
+        Returns
+        -------
+        has_interacted_with_any : bool
+            True if the address has interacted with one or more of the addresses in the array_address
+        """
+        count_interaction_with_any = self.count_interaction_any(address, array_address)
+        return count_interaction_with_any > 0
 
     def get_contributors(self):
         """
         Return a list of contributors of the grant
         Returns
         -------
         contributors : narray
@@ -378,19 +502,15 @@
         df : pd.DataFrame
             The data frame with the transactions of the address
 
         """
         try:
             df = self.gb_EOA_sorted.get_group(address)
         except Exception as e:
-            if self.gb_EOA_sorted is None:
-                self.set_group_by_sorted_EOA()
-                df = self.get_address_transactions(address)
-            else:
-                df = pd.DataFrame()
+            df = pd.DataFrame()
         return df
 
     def get_address_transactions_add(self, df, address):
         """
         Get transactions of an address from a dataframe df
         Parameters
         ----------
@@ -446,7 +566,84 @@
 
     @staticmethod
     def longest_common_sub_string_pylcs(string_target, string_other):
 
         # 1 similar transaction equals to 8 first char of the address + "-" + "x" = 10 char
         lcs = pylcs.lcs_string_length(string_target, string_other)
         return lcs // 10  # quotient of the division
+
+    @staticmethod
+    def get_mean_score_lcs(lcs):
+        if lcs.shape[0] == 0:
+            return 0
+        else:
+            return lcs.reset_index()['score'].mean()
+
+    @staticmethod
+    def get_max_score_lcs(lcs):
+        if lcs.shape[0] == 0:
+            return 0
+        else:
+            return lcs.reset_index()['score'].max()
+
+    def get_df_features(self):
+        df_features = self.gb_EOA_sorted['tx_hash'].count().reset_index().rename(columns={'tx_hash': 'count_tx'})
+        df_features['less_10_tx'] = df_features['count_tx'].apply(lambda x: x < 10)
+        df_features['same_seed'] = df_features['EOA'].apply(lambda x: self.has_same_seed(x))
+        df_features['same_seed_naive'] = df_features['EOA'].apply(lambda x: self.has_same_seed_naive(x))
+        df_features['seed_suspicious'] = df_features.loc[:, 'same_seed'].ne(df_features.loc[:, 'same_seed_naive'])
+        df_features['count_interact_other_ctbt'] = df_features['EOA'].apply(
+            lambda x: self.count_interaction_with_other_contributor(x))
+
+        details_first_incoming_transaction = self.details_first_incoming_transaction
+        details_first_outgoing_transaction = self.details_first_outgoing_transaction
+
+        df_features['lcs'] = 0
+        df_features['cluster_size_lcs'] = 0
+        df_features['mean_score_lcs'] = 0
+        df_features['max_score_lcs'] = 0
+        df_bool_less_10_tx = df_features['less_10_tx']
+
+        if df_bool_less_10_tx.sum() > 0:
+            r = df_features.loc[df_bool_less_10_tx, 'EOA'].apply(
+                lambda x: self.transaction_similitude_pylcs(x, minimum_sim_tx=3))
+            df_features.loc[df_bool_less_10_tx, 'cluster_size_lcs'] = r.apply(lambda x: len(x))
+            df_features.loc[df_bool_less_10_tx, 'mean_score_lcs'] = r.apply(lambda x: self.get_mean_score_lcs(x))
+            df_features.loc[df_bool_less_10_tx, 'max_score_lcs'] = r.apply(lambda x: self.get_max_score_lcs(x))
+
+        df_features['has_lcs'] = df_features['cluster_size_lcs'] > 0
+
+        merge = df_features.merge(details_first_incoming_transaction, on='EOA', how='left')
+        merge = merge.merge(details_first_outgoing_transaction, on='EOA', how='left')
+
+        return merge
+
+    def get_df_features_vectorized(self):
+        df_features = self.gb_EOA_sorted['tx_hash'].count().reset_index().rename(columns={'tx_hash': 'count_tx'})
+        df_features['less_10_tx'] = np.vectorize(lambda x: x < 10)(df_features['count_tx'])
+        df_features['same_seed'] = np.vectorize(self.has_same_seed)(df_features['EOA'])
+        df_features['same_seed_naive'] = np.vectorize(self.has_same_seed_naive)(df_features['EOA'])
+        df_features['seed_suspicious'] = df_features.loc[:, 'same_seed'].ne(df_features.loc[:, 'same_seed_naive'])
+        df_features['count_interact_other_ctbt'] = np.vectorize(self.count_interaction_with_other_contributor)(
+            df_features['EOA'])
+
+        details_first_incoming_transaction = self.details_first_incoming_transaction
+        details_first_outgoing_transaction = self.details_first_outgoing_transaction
+
+        df_features['lcs'] = 0
+        df_features['cluster_size_lcs'] = 0
+        df_features['mean_score_lcs'] = 0
+        df_features['max_score_lcs'] = 0
+
+        df_bool_less_10_tx = df_features['less_10_tx']
+        if df_bool_less_10_tx.sum() > 0:
+            r = np.vectorize(self.transaction_similitude_pylcs)(df_features.loc[df_bool_less_10_tx, 'EOA'])
+            df_features.loc[df_bool_less_10_tx, 'cluster_size_lcs'] = np.vectorize(len)(r)
+            df_features.loc[df_bool_less_10_tx, 'mean_score_lcs'] = np.vectorize(self.get_mean_score_lcs)(r)
+            df_features.loc[df_bool_less_10_tx, 'max_score_lcs'] = np.vectorize(self.get_max_score_lcs)(r)
+
+        df_features['has_lcs'] = df_features['cluster_size_lcs'] > 0
+
+        merge = df_features.merge(details_first_incoming_transaction, on='EOA', how='left')
+        merge = merge.merge(details_first_outgoing_transaction, on='EOA', how='left')
+
+        return merge
```

### Comparing `sybil-scorer-0.1.3/sbscorer/sbutils/LoadData.py` & `sybil-scorer-0.2.0/sbscorer/sbutils/LoadData.py`

 * *Files identical despite different names*

### Comparing `sybil-scorer-0.1.3/sbscorer/sybil_scorer.egg-info/PKG-INFO` & `sybil-scorer-0.2.0/sbscorer/sybil_scorer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sybil-scorer
-Version: 0.1.3
+Version: 0.2.0
 Summary: A sybil scoring tool
 Home-page: https://github.com/poupou-web3/cluster-scorer
 Author: Poupou
 Author-email: Poupou <poupou-web3@protonmail.com>
 License: MIT License
         
         Copyright (c) 2023 Poupou
```

### Comparing `sybil-scorer-0.1.3/setup.cfg` & `sybil-scorer-0.2.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2073 7962 696c 2d73 636f 7265 720d   = sybil-scorer.
-00000020: 0a76 6572 7369 6f6e 203d 2030 2e31 2e33  .version = 0.1.3
+00000020: 0a76 6572 7369 6f6e 203d 2030 2e32 2e30  .version = 0.2.0
 00000030: 0d0a 6175 7468 6f72 203d 2050 6f75 706f  ..author = Poupo
 00000040: 750d 0a61 7574 686f 725f 656d 6169 6c20  u..author_email 
 00000050: 3d20 706f 7570 6f75 2d77 6562 3340 7072  = poupou-web3@pr
 00000060: 6f74 6f6e 6d61 696c 2e63 6f6d 0d0a 6465  otonmail.com..de
 00000070: 7363 7269 7074 696f 6e20 3d20 4120 7379  scription = A sy
 00000080: 6269 6c20 7363 6f72 696e 6720 746f 6f6c  bil scoring tool
 00000090: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
```

