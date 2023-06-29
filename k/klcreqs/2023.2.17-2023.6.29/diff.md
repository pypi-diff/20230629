# Comparing `tmp/klcreqs-2023.2.17.tar.gz` & `tmp/klcreqs-2023.6.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klcreqs-2023.2.17.tar", last modified: Fri Feb 17 21:34:33 2023, max compression
+gzip compressed data, was "klcreqs-2023.6.29.tar", last modified: Thu Jun 29 20:00:48 2023, max compression
```

## Comparing `klcreqs-2023.2.17.tar` & `klcreqs-2023.6.29.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-02-17 21:34:33.024769 klcreqs-2023.2.17/
--rw-rw-rw-   0        0        0      288 2023-02-17 21:34:33.023787 klcreqs-2023.2.17/PKG-INFO
--rw-rw-rw-   0        0        0     2511 2023-02-17 21:31:23.000000 klcreqs-2023.2.17/README.md
-drwxrwxrwx   0        0        0        0 2023-02-17 21:34:33.012789 klcreqs-2023.2.17/klcreqs/
--rw-rw-rw-   0        0        0       19 2022-10-19 22:05:33.000000 klcreqs-2023.2.17/klcreqs/__init__.py
--rw-rw-rw-   0        0        0     1632 2023-01-05 15:18:58.000000 klcreqs-2023.2.17/klcreqs/constants.py
--rw-rw-rw-   0        0        0    12507 2023-02-17 21:29:45.000000 klcreqs-2023.2.17/klcreqs/core.py
-drwxrwxrwx   0        0        0        0 2023-02-17 21:34:33.022772 klcreqs-2023.2.17/klcreqs.egg-info/
--rw-rw-rw-   0        0        0      288 2023-02-17 21:34:32.000000 klcreqs-2023.2.17/klcreqs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2023-02-17 21:34:32.000000 klcreqs-2023.2.17/klcreqs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-17 21:34:32.000000 klcreqs-2023.2.17/klcreqs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-02-17 21:34:32.000000 klcreqs-2023.2.17/klcreqs.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-02-17 21:34:32.000000 klcreqs-2023.2.17/klcreqs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-17 21:34:33.024769 klcreqs-2023.2.17/setup.cfg
--rw-rw-rw-   0        0        0      576 2023-02-17 21:19:43.000000 klcreqs-2023.2.17/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 20:00:48.626442 klcreqs-2023.6.29/
+-rw-rw-rw-   0        0        0      229 2023-06-29 20:00:48.624447 klcreqs-2023.6.29/PKG-INFO
+-rw-rw-rw-   0        0        0     2587 2023-02-22 21:31:43.000000 klcreqs-2023.6.29/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 20:00:48.607493 klcreqs-2023.6.29/klcreqs/
+-rw-rw-rw-   0        0        0       19 2022-10-19 22:05:31.000000 klcreqs-2023.6.29/klcreqs/__init__.py
+-rw-rw-rw-   0        0        0     1825 2023-04-05 22:48:56.000000 klcreqs-2023.6.29/klcreqs/constants.py
+-rw-rw-rw-   0        0        0    13924 2023-06-14 21:30:54.000000 klcreqs-2023.6.29/klcreqs/core.py
+drwxrwxrwx   0        0        0        0 2023-06-29 20:00:48.619462 klcreqs-2023.6.29/klcreqs.egg-info/
+-rw-rw-rw-   0        0        0      229 2023-06-29 20:00:47.000000 klcreqs-2023.6.29/klcreqs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2023-06-29 20:00:47.000000 klcreqs-2023.6.29/klcreqs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 20:00:47.000000 klcreqs-2023.6.29/klcreqs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-06-29 20:00:47.000000 klcreqs-2023.6.29/klcreqs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-29 20:00:47.000000 klcreqs-2023.6.29/klcreqs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-29 20:00:48.627443 klcreqs-2023.6.29/setup.cfg
+-rw-rw-rw-   0        0        0      576 2023-06-29 19:55:31.000000 klcreqs-2023.6.29/setup.py
```

### Comparing `klcreqs-2023.2.17/README.md` & `klcreqs-2023.6.29/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -37,12 +37,12 @@
 3. delete_symbol(*symbol, **d)
     * deletes specified symbol, can specify date for more precision
     * returns nothing
 4. delete_ofdb()
     * deletes ofdb at url passed in initialization of class
 5. upload(*inp, *method, *parsed, **idx) 
     * inp can be either pandas DataFrame or dict, contains the data to upload, if DataFrame will automatically transform to dict on orient='index', required arg
-    * method is either 'symbol' or 'date', required arg
+    * method is either 'symbol' or 'date', required arg. Dataframe must have the method column (either symbol or date) as the index
     * parsed is Boolean, set to False if you want to pass in a dataframe and have the fxn parse inp itself. Set to True if you have already created a properly constructed dict to pass in as inp, requred arg
     * idx is the index for uploading pre-parsed input, must be either date or symbol value and sets the end-level location in path specification, required when parsed==True
     * returns response text value (r.text)
```

### Comparing `klcreqs-2023.2.17/klcreqs/core.py` & `klcreqs-2023.6.29/klcreqs/core.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 
         # print(r.text)
         
         try:
             self.response = json.loads(r.text)
         except:
             self.response = r
-            # print(type(r))
 
     def __request_handling(self):
         # send request as defined
         req = formula_api.make_request(self)
         # print(req.status_code)
 
         # if request returns an error and bof is set to true, override endpoint, batch settings and resend as batch
@@ -47,47 +46,39 @@
         if self.status_code == 429 and self.batch == True:
             self.ep = 'ts'
             self.batch = True
             formula_api.switch_auth(self)
             # print('batch failed, resubmitting with authswitch')
             req = formula_api.__request_handling(self)
             
-        # if batching, call batch handling fxn, print message if something is wrong(req.text doesnt exist)
         try:
             keys = json.loads(req.text)['data'].keys()
         except:
             keys = ['not']
-        # print(keys)
-        if self.batch == True and type(json.loads(req.text)['data']) == dict and 'id' in keys:
-           req = formula_api.__poll_return_batch(self, req) 
+
+        with open('log.txt', 'w') as f:
+            f.writelines(req.text)
+
+        # verifies the response status is in the usual format and calls batch processing function
+        if self.batch == True and 'id' in keys: # and type(json.loads(req.text)['data']) == dict: this wouldnt work b/c 'data' is a list that holds dicts
+           req = formula_api.__poll_return_batch(self, req)
         
         self.ft = time.time()
         return req 
         
     
     def __poll_return_batch(self, req):
         sleep(5)
 
         res = json.loads(req.text)
         try:
             batch_id = res['data']['id']
         except:
-            # print(res['data'])
-            # print('batch skipped')
-            # print('e')
             return req
 
-        # try:
-        #     res = json.loads(req.text)
-        #     batch_id = res['data'][0]['id']
-        # except:
-        #     print('failed batch_id_request')
-        #     print('type', type(req))
-        #     print('len', len(req))
-        #     return req
 
 
         batch_id_request_json = json.dumps({"data": {"id": batch_id}})
 
         while True:
             batch_status = requests.post(url=status_endpoint,
                                                   data=batch_id_request_json,
@@ -113,47 +104,34 @@
                                                     verify=False)
                 
                 if batch_result.status_code == 200:
                     return batch_result
                 elif batch_result.status_code >= 400:
                     print('error retrieving batch_result_response')
                     print(batch_result.status_code)
-                    print(batch_result)
-                    # print(batch_result_response.text)
+                    # print(batch_result)
                     return
             elif batch_status_response['data']['status'] != 'DONE':
                 pass
 
     def make_request(self):
-
-        # if self.acount >= 4:
-        #     sleep(600)
-        #     self.acount = 0
-        # else:
-        #     pass
-
         request_json = formula_api.__create_request_json(self)
         if self.ep in ['ts', 'time', 'timeseries', 'time_series', 'time series']:
             req = formula_api.time_series_request(
                 self,
                 request_json=request_json
             )
         elif self.ep in ['cs', 'cross', 'crosssectional', 'cross_sectional', 'cross sectional']:
             req =  formula_api.cross_sectional_request(
                 self,
                 request_json=request_json
             )
         else:
             raise Exception('Exception no valid endpoint provided, use \"ts\" or \"cs\"')
-        # print(type(req))
-        if type(req) == type(tuple):
-            print(req)
-            print(type(req))
         self.status_code = req.status_code
-        
         return req
 
 
     def time_series_request(self, request_json):
         return formula_api.__http_post(
             self,
             URL=formula_api.time_series_url,
@@ -201,24 +179,35 @@
         except Exception as e:
             return False, str(e)
 
     def status_code(self):
         return self.status_code
 
     def df(self):
-        try:
-            self.df = pd.json_normalize(self.response['data'])
-        except:
-            try:
-                self.df = pd.DataFrame(self.response[0]['data'], index=range(math.ceil(len(list(self.response.values()))/len(list(self.response.keys())))))
-            except:
-                print(self.response)
-                self.df = pd.DataFrame(self.response['data'])
+        # print(self.response.keys())
+        if 'data' in list(self.response.keys()):
+            df = pd.DataFrame(self.response['data'])
+        else:
+            print(self.response.keys())
+            print(self.response)
+        return df
+
+        # try:
+        #     self.df = pd.json_normalize(self.response['data'])
+        # except:
+        #     try:
+        #         self.df = pd.DataFrame(self.response[0]['data'], index=range(math.ceil(len(list(self.response.values()))/len(list(self.response.keys())))))
+        #     except:
+        #         try:
+        #             self.df = pd.DataFrame(self.response)
+        #         except:
+        #             with open('logee.txt', 'w') as f:
+        #                 f.writelines(self.response)
                 
-        return self.df
+        # return df
             
 
     @property
     def runtime(self):
         self.rt = (self.ft - self.st)
         return self.rt
 
@@ -259,17 +248,33 @@
     def get_dates(self):
         url = f'{self.host}{self.uri}/dates'
         r = requests.get(url, auth=authorization, headers=headers)
         if r.status_code >= 400:
             print(r)
             print(r.text)
             return
-        response = json.loads(r.text)
+        sleep(5)
+        response = json.loads(r.text)['data']
+        return response
+    
+    
+
+    def get_symbols_for_date(self, d):
+        url = f'{self.host}{self.uri}/dates/{d}/symbols'
+        r = requests.get(url, auth=authorization, headers=headers)
+        if r.status_code >= 400:
+            print(r)
+            print(r.text)
+            return
+        sleep(5)
+        response = json.loads(r.text)['data']
         return response
 
+
+
     def delete_date(self, d):
         url = f"{self.host}{self.uri}/dates/{d}"
         r = requests.delete(url, auth=authorization, headers=headers)
         if r.status_code >= 400:
             print(r)
             print(r.text)
         return
@@ -283,26 +288,32 @@
         if r.status_code > 204:
             print(r)
             print(r.text)
         return
 
     def delete_ofdb(self):
         url = f'{self.host}{self.uri}'
-        conf = input(f'type confirm to confirm deletion of {url}: ')
+        conf = input(f'type \"confirm\" to confirm deletion of {url}: ')
         if conf != 'confirm':
             return
         else:
             r = requests.delete(url, auth=authorization, headers=headers)
             if r.status_code > 204:
                 # print(r)
                 # print(r.text)
                 sleep(30)
                 r = requests.delete
             return
 
+    def get_fields(self):
+        url = f'{self.host}{self.uri}/fields'
+        r = requests.get(url, auth=authorization, headers=headers)
+        return r
+
+
 
     @staticmethod
     def __parse(df, orient):
         if orient not in ['date', 'symbol']:
             raise Exception('invalid orient arg. acceptable values: date, symbol')
             return
         df.fillna(0, inplace=True)
@@ -312,16 +323,16 @@
         except:
             pass
 
         dct = df.to_dict(orient='index')
         bodies = []
         for i, j in dct.items():
             body = {'data': []}
-            body['data'][orient] = i
-            body['data']['content'] = j
+            body['data'].append({orient: i})
+            body['data'].append({'content': j})
             bodies.append(body)
         return bodies
 
     def upload(self, inp, method, parsed, idx):
         if method not in ['symbol', 'date']:
             raise Exception('invalid method arg. must be symbol or date')
         if type(inp) not in (pd.DataFrame, list):
@@ -330,26 +341,56 @@
         parsed = parsed
         orient = method        
         url = f'{self.host}{self.uri}/{orient}s'
 
         if parsed == False:
             self.bodies = ofdb_api.__parse(inp, orient)
             for i in self.bodies:
-                body = json.dumps(i)
+                body = i
+                body['data'][0]['content'] = [{k: None if v == 'nan' else v for k,v in i.items()} for i in body['data'][0]['content']]
+                body = json.dumps(body)
                 r = requests.post(url, auth=authorization, headers=headers, data=body)
+
                 if r.status_code >= 400:
                     print('error in upload')
-                    # print(r)
+                    with open('json_dump.txt', 'w') as f:
+                        f.writelines(body)
+                    # print(body)
                     print(r.text)
+                    return r
 
         elif parsed == True:
             if type(idx) not in (str, int):
                 raise Exception('pre-parsed input must have only 1 index of type int or str')
-            self.body = {'data': [{orient: idx, 'content': inp}]}
-            body = json.dumps(self.body)
-            # r = requests.post(url, auth=authorization, headers=headers, data=body)
+            body = {'data': [{orient: idx, 'content': inp}]}
+            
+            body['data'][0]['content'] = [{k: None if v == 'nan' else v for k,v in i.items()} for i in body['data'][0]['content']]
+            # body = {k: None if v=="nan" else v for k, v in body.items() }
+            
+            
+            
+            body = json.dumps(body)
+            r = requests.post(url, auth=authorization, headers=headers, data=body)
             if r.status_code >= 400:
                 print('error in upload')
-                # print(r)
+                with open('json_dump.txt', 'w') as f:
+                    f.writelines(body)
+                # print(body)
+                print(r)
+                print(r.status_code)
                 print(r.text)
-        return r.text
-                
+        return r
+    
+    ''' in development '''
+
+    # def change_date(self, d):
+    #     url = f"{self.host}{self.uri}/dates/{d}"
+    #     dates_in = self.get_dates(self)
+    #     if d in dates_in:
+    #         raise Exception('date already exists in ofdb')
+    #     fields_in = self.get_fields(self)
+    #     r = formula_api(
+
+    #     )
+        
+
+
```

### Comparing `klcreqs-2023.2.17/setup.py` & `klcreqs-2023.6.29/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 if __name__ == "__main__":
     setup(
         name="klcreqs",
-        version="2023.02.17",
+        version="2023.06.29",
         description="library for streamlining api requests",
         long_description="coming soon",
         readme="README.md",
         author='Thomas Nemechek',
         author_email='tnemechek@klcapital.com',
         classifiers=["Programming Language :: Python"],
         packages=['klcreqs'],
```

