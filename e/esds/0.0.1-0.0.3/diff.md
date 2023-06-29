# Comparing `tmp/esds-0.0.1.tar.gz` & `tmp/esds-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esds-0.0.1.tar", last modified: Wed May 24 12:46:49 2023, max compression
+gzip compressed data, was "esds-0.0.3.tar", last modified: Thu Jun 29 08:15:13 2023, max compression
```

## Comparing `esds-0.0.1.tar` & `esds-0.0.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 loic      (1000) loic      (1000)        0 2023-05-24 12:46:49.298004 esds-0.0.1/
--rw-r--r--   0 loic      (1000) loic      (1000)     7652 2022-06-10 09:12:54.000000 esds-0.0.1/LICENSE
--rw-r--r--   0 loic      (1000) loic      (1000)      273 2023-05-24 12:46:49.298004 esds-0.0.1/PKG-INFO
--rw-r--r--   0 loic      (1000) loic      (1000)     2008 2022-09-02 08:00:59.000000 esds-0.0.1/README.md
-drwxr-xr-x   0 loic      (1000) loic      (1000)        0 2023-05-24 12:46:49.294670 esds-0.0.1/esds/
--rw-r--r--   0 loic      (1000) loic      (1000)      205 2022-09-12 11:52:41.000000 esds-0.0.1/esds/__init__.py
--rw-r--r--   0 loic      (1000) loic      (1000)     1270 2022-09-13 08:35:49.000000 esds-0.0.1/esds/__main__.py
--rw-r--r--   0 loic      (1000) loic      (1000)     3827 2022-09-10 09:54:46.000000 esds-0.0.1/esds/debug.py
-drwxr-xr-x   0 loic      (1000) loic      (1000)        0 2023-05-24 12:46:49.298004 esds-0.0.1/esds/helpers/
--rw-r--r--   0 loic      (1000) loic      (1000)        0 2022-06-23 08:56:21.000000 esds-0.0.1/esds/helpers/__init__.py
--rw-r--r--   0 loic      (1000) loic      (1000)     2591 2022-06-21 09:01:29.000000 esds-0.0.1/esds/helpers/wireless_area.py
--rw-r--r--   0 loic      (1000) loic      (1000)     9726 2022-09-09 11:00:48.000000 esds-0.0.1/esds/node.py
--rw-r--r--   0 loic      (1000) loic      (1000)     9290 2023-03-31 07:52:22.000000 esds-0.0.1/esds/platform.py
-drwxr-xr-x   0 loic      (1000) loic      (1000)        0 2023-05-24 12:46:49.298004 esds-0.0.1/esds/plugins/
--rw-r--r--   0 loic      (1000) loic      (1000)       44 2022-06-21 09:01:29.000000 esds-0.0.1/esds/plugins/__init__.py
--rw-r--r--   0 loic      (1000) loic      (1000)      971 2022-09-09 07:37:27.000000 esds-0.0.1/esds/plugins/node_plugin.py
--rw-r--r--   0 loic      (1000) loic      (1000)     2038 2022-06-21 09:01:29.000000 esds-0.0.1/esds/plugins/operating_states.py
--rw-r--r--   0 loic      (1000) loic      (1000)     5930 2023-01-23 15:24:36.000000 esds-0.0.1/esds/plugins/power_states.py
--rw-r--r--   0 loic      (1000) loic      (1000)      168 2022-09-14 11:54:19.000000 esds-0.0.1/esds/rcode.py
--rw-r--r--   0 loic      (1000) loic      (1000)    25823 2023-01-23 15:11:22.000000 esds-0.0.1/esds/simulator.py
-drwxr-xr-x   0 loic      (1000) loic      (1000)        0 2023-05-24 12:46:49.298004 esds-0.0.1/esds.egg-info/
--rw-r--r--   0 loic      (1000) loic      (1000)      273 2023-05-24 12:46:49.000000 esds-0.0.1/esds.egg-info/PKG-INFO
--rw-r--r--   0 loic      (1000) loic      (1000)      492 2023-05-24 12:46:49.000000 esds-0.0.1/esds.egg-info/SOURCES.txt
--rw-r--r--   0 loic      (1000) loic      (1000)        1 2023-05-24 12:46:49.000000 esds-0.0.1/esds.egg-info/dependency_links.txt
--rw-r--r--   0 loic      (1000) loic      (1000)       35 2023-05-24 12:46:49.000000 esds-0.0.1/esds.egg-info/entry_points.txt
--rw-r--r--   0 loic      (1000) loic      (1000)       13 2023-05-24 12:46:49.000000 esds-0.0.1/esds.egg-info/requires.txt
--rw-r--r--   0 loic      (1000) loic      (1000)        5 2023-05-24 12:46:49.000000 esds-0.0.1/esds.egg-info/top_level.txt
--rw-r--r--   0 loic      (1000) loic      (1000)      303 2022-09-12 07:44:33.000000 esds-0.0.1/pyproject.toml
--rw-r--r--   0 loic      (1000) loic      (1000)      478 2023-05-24 12:46:49.298004 esds-0.0.1/setup.cfg
+drwxr-xr-x   0 loic      (1000) loic      (1000)        0 2023-06-29 08:15:13.392380 esds-0.0.3/
+-rw-r--r--   0 loic      (1000) loic      (1000)     7652 2022-06-10 09:12:54.000000 esds-0.0.3/LICENSE
+-rw-r--r--   0 loic      (1000) loic      (1000)     2326 2023-06-29 08:15:13.392380 esds-0.0.3/PKG-INFO
+-rw-r--r--   0 loic      (1000) loic      (1000)     2008 2022-09-02 08:00:59.000000 esds-0.0.3/README.md
+drwxr-xr-x   0 loic      (1000) loic      (1000)        0 2023-06-29 08:15:13.392380 esds-0.0.3/esds/
+-rw-r--r--   0 loic      (1000) loic      (1000)      205 2023-06-29 08:14:59.000000 esds-0.0.3/esds/__init__.py
+-rw-r--r--   0 loic      (1000) loic      (1000)     1270 2022-09-13 08:35:49.000000 esds-0.0.3/esds/__main__.py
+-rw-r--r--   0 loic      (1000) loic      (1000)     3827 2022-09-10 09:54:46.000000 esds-0.0.3/esds/debug.py
+drwxr-xr-x   0 loic      (1000) loic      (1000)        0 2023-06-29 08:15:13.392380 esds-0.0.3/esds/helpers/
+-rw-r--r--   0 loic      (1000) loic      (1000)        0 2022-06-23 08:56:21.000000 esds-0.0.3/esds/helpers/__init__.py
+-rw-r--r--   0 loic      (1000) loic      (1000)     2591 2022-06-21 09:01:29.000000 esds-0.0.3/esds/helpers/wireless_area.py
+-rw-r--r--   0 loic      (1000) loic      (1000)     9764 2023-06-28 13:09:49.000000 esds-0.0.3/esds/node.py
+-rw-r--r--   0 loic      (1000) loic      (1000)    10685 2023-06-29 07:38:17.000000 esds-0.0.3/esds/platform.py
+drwxr-xr-x   0 loic      (1000) loic      (1000)        0 2023-06-29 08:15:13.392380 esds-0.0.3/esds/plugins/
+-rw-r--r--   0 loic      (1000) loic      (1000)       44 2022-06-21 09:01:29.000000 esds-0.0.3/esds/plugins/__init__.py
+-rw-r--r--   0 loic      (1000) loic      (1000)      971 2022-09-09 07:37:27.000000 esds-0.0.3/esds/plugins/node_plugin.py
+-rw-r--r--   0 loic      (1000) loic      (1000)     2038 2022-06-21 09:01:29.000000 esds-0.0.3/esds/plugins/operating_states.py
+-rw-r--r--   0 loic      (1000) loic      (1000)     5930 2023-01-23 15:24:36.000000 esds-0.0.3/esds/plugins/power_states.py
+-rw-r--r--   0 loic      (1000) loic      (1000)      168 2022-09-14 11:54:19.000000 esds-0.0.3/esds/rcode.py
+-rw-r--r--   0 loic      (1000) loic      (1000)    26417 2023-06-29 07:38:17.000000 esds-0.0.3/esds/simulator.py
+drwxr-xr-x   0 loic      (1000) loic      (1000)        0 2023-06-29 08:15:13.392380 esds-0.0.3/esds.egg-info/
+-rw-r--r--   0 loic      (1000) loic      (1000)     2326 2023-06-29 08:15:13.000000 esds-0.0.3/esds.egg-info/PKG-INFO
+-rw-r--r--   0 loic      (1000) loic      (1000)      492 2023-06-29 08:15:13.000000 esds-0.0.3/esds.egg-info/SOURCES.txt
+-rw-r--r--   0 loic      (1000) loic      (1000)        1 2023-06-29 08:15:13.000000 esds-0.0.3/esds.egg-info/dependency_links.txt
+-rw-r--r--   0 loic      (1000) loic      (1000)       35 2023-06-29 08:15:13.000000 esds-0.0.3/esds.egg-info/entry_points.txt
+-rw-r--r--   0 loic      (1000) loic      (1000)       13 2023-06-29 08:15:13.000000 esds-0.0.3/esds.egg-info/requires.txt
+-rw-r--r--   0 loic      (1000) loic      (1000)        5 2023-06-29 08:15:13.000000 esds-0.0.3/esds.egg-info/top_level.txt
+-rw-r--r--   0 loic      (1000) loic      (1000)      388 2023-06-29 08:10:38.000000 esds-0.0.3/pyproject.toml
+-rw-r--r--   0 loic      (1000) loic      (1000)      478 2023-06-29 08:15:13.392380 esds-0.0.3/setup.cfg
```

### Comparing `esds-0.0.1/LICENSE` & `esds-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `esds-0.0.1/README.md` & `esds-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `esds-0.0.1/esds/__main__.py` & `esds-0.0.3/esds/__main__.py`

 * *Files identical despite different names*

### Comparing `esds-0.0.1/esds/debug.py` & `esds-0.0.3/esds/debug.py`

 * *Files identical despite different names*

### Comparing `esds-0.0.1/esds/helpers/wireless_area.py` & `esds-0.0.3/esds/helpers/wireless_area.py`

 * *Files identical despite different names*

### Comparing `esds-0.0.1/esds/node.py` & `esds-0.0.3/esds/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import threading,importlib,queue
 from esds.rcode import RCode
 
 class Node:
     available_node_id=0
-    def __init__(self,src,interfaces):
+    def __init__(self,src,interfaces,grp):
         """
         self.chest: contains mutex protected data
         """
         self.node_id=Node.available_node_id
+        self.grp=grp # Node group
         Node.available_node_id+=1 # Refresh node id
         self.src=src # Store the node source code
         self.args=None # Store the node arguments (passed through Simulator.create_node()
         self.rargs=None # Store the requests arguments
         self.plugins=list() # Contains all registered node plugins
         self.rqueue=queue.Queue() # Receive simulator acknowledgments
         self.chest={"state":"running", "turned_on":True, "request": None, "interfaces":dict(), "interfaces_queue_size":dict(), "pending_plugin_notify":0}
```

### Comparing `esds-0.0.1/esds/platform.py` & `esds-0.0.3/esds/platform.py`

 * *Files 8% similar despite different names*

```diff
@@ -54,14 +54,16 @@
             "breakpoints_callback": lambda s:None,
             "debug": False,
             "debug_file": "./esds.debug",
             "interferences": True,
             "node_count": 0,
             "implementations": [],
             "arguments": [],
+            "groups": dict(),               # {node_id} => group
+            "nodes_interfaces": dict(),     # {node_id} => [interfaces]
             "interfaces": dict()
         }
 
         with open(file_path) as f:
             self.platform = yaml.load(f, Loader=yaml.FullLoader)
 
         ##### General
@@ -98,23 +100,34 @@
     def parse_txperf(self,txperf):
         elts=txperf.split()
         return((UnitsParser.node_range(elts[0],self.default["node_count"]),UnitsParser.bandwidth(elts[1]),UnitsParser.latency(elts[2])))
 
     def parse_interfaces(self):
         interfaces=self.platform["interfaces"]
         node_count=self.default["node_count"]
+        ##### Init nodes interfaces
+        for node in range(0,self.default["node_count"]):
+            self.default["nodes_interfaces"][node]=list()
+        ##### Parse interfaces
         for i in interfaces:
             if interfaces[i]["type"] not in ["wireless","wired"]:
                 self.parsing_error("Invalid interface type \""+interfaces[i]["type"]+"\"")
             is_wired=interfaces[i]["type"] == "wired"
             links=list()
             if type(interfaces[i]["links"]) != list:
                 self.parsing_error("Invalide type of links in interface "+i)
             for link in interfaces[i]["links"]:
                 links.append(self.parse_link(link))
+            ##### Assign interfaces to nodes
+            if "nodes" in interfaces[i]:
+                r=UnitsParser.node_range(str(interfaces[i]["nodes"]),self.default["node_count"])
+                for node in r:
+                    self.default["nodes_interfaces"][node].append(i)
+            else:
+                self.parsing_error("missing nodes section on interface "+i)
             ##### Create network matrix
             BW=np.full((node_count,node_count),0)
             LAT=np.full((node_count,node_count),0)
             for link in links:
                 for n1 in link[0]:
                     for n2 in link[3]:
                         BW[n1][n2]=link[1]
@@ -141,14 +154,22 @@
         nodes=self.platform["nodes"]
         if "count" in nodes:
             if not str(nodes["count"]).isnumeric():
                 self.parsing_error("node count should be a number")
             self.default["node_count"]=nodes["count"]
         else:
             self.parsing_error("node count not provided")
+        if "groups" in nodes:
+            if type(nodes["groups"]) != list:
+                self.parsing_error("nodes groups should be a list")
+            for grp in nodes["groups"]:
+                words=grp.split()
+                r=UnitsParser.node_range(words[0],self.default["node_count"])
+                for node in r:
+                    self.default["groups"][node]=words[1]
         if "implementations" in nodes:
             if type(nodes["implementations"]) != list:
                 self.parsing_error("nodes implementations should be a list of file path")
             self.default["implementations"]=[None]*self.default["node_count"]
             for impl in nodes["implementations"]:
                 words=impl.split()
                 r=UnitsParser.node_range(words[0],self.default["node_count"])
@@ -206,15 +227,18 @@
             module, ext=os.path.splitext(self.default["breakpoints_file"])
             imported=importlib.import_module(module)
             callback=getattr(imported, self.default["breakpoints_callback"])
             self.default["breakpoints_callback"]=callback
         ##### Create simulator
         simulator=Simulator(self.default["interfaces"])
         for node_id in range(0,self.default["node_count"]):
-            simulator.create_node(self.default["implementations"][node_id], args=self.default["arguments"][node_id])
+            if node_id in self.default["groups"]:
+                simulator.create_node(self.default["implementations"][node_id],self.default["nodes_interfaces"][node_id], args=self.default["arguments"][node_id],grp=self.default["groups"][node_id])
+            else:
+                simulator.create_node(self.default["implementations"][node_id],self.default["nodes_interfaces"][node_id], args=self.default["arguments"][node_id])
         ##### Run simulation
         simulator.run(
             breakpoints=self.default["breakpoints"],
             breakpoints_every=self.default["breakpoints_every"],
             breakpoint_callback=self.default["breakpoints_callback"],
             debug=self.default["debug"],
             debug_file_path=self.default["debug_file"],
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `esds-0.0.1/esds/plugins/node_plugin.py` & `esds-0.0.3/esds/plugins/node_plugin.py`

 * *Files identical despite different names*

### Comparing `esds-0.0.1/esds/plugins/operating_states.py` & `esds-0.0.3/esds/plugins/operating_states.py`

 * *Files identical despite different names*

### Comparing `esds-0.0.1/esds/plugins/power_states.py` & `esds-0.0.3/esds/plugins/power_states.py`

 * *Files identical despite different names*

### Comparing `esds-0.0.1/esds/simulator.py` & `esds-0.0.3/esds/simulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,26 +71,31 @@
                         else:
                             new_duration=new_datasize_remaining*8/new_bw+new_lat*latency_factor
                         event[1]=self.time+new_duration
                         event[2][6]=new_datasize_remaining
                         event[2][5]=new_duration
         self.netmat=netmat
           
-    def create_node(self, src, args=None):
+    def create_node(self, src, interfaces=[], args=None, grp="def"):
         """
         Create a node thread and run it
         """
-        node=Node(src, self.netmat.keys())
+        for intf in interfaces:
+            if intf not in self.netmat.keys():
+                self.log("Cannot create node "+str(Node.available_node_id)+": interface "+ intf + " unknown")
+                exit(1)
+        node=Node(src, interfaces, grp)
         self.nodes.append(node)
         thread=threading.Thread(target=node.run,args=[args]) # There must be "daemon=True" as a parameter, but we removed it to be compatible with older version of python
         thread.start()
 
     def log(self,msg,node=None):
-        src = "esds" if node is None else "n"+str(node)
-        logline="[t="+str(self.time_truncated)+",src="+src+"] "+msg
+        logline="[t="+str(self.time_truncated)+",src=esds] "+msg
+        if node is not None:
+            logline="[t="+str(self.time_truncated)+",src=n"+str(node.node_id)+",grp="+str(node.grp)+"] "+msg
         if self.debug is not None:
             self.debug.append_log(logline)
         print(logline)
 
     def sort_events(self):
         """
         Sort the events by timestamp and priorities
@@ -114,15 +119,15 @@
                 self.events=self.events[~np.array(selector)]
                 node["state"]="running"
                 node.rqueue.put(("timeout_remove",RCode.SUCCESS))
             elif timeout_remove_only:
                 break
             elif not timeout_remove_only:
                 if node["request"] == "log":
-                    self.log(node.rargs,node=node.node_id)
+                    self.log(node.rargs,node=node)
                     node["state"]="running"
                     node.rqueue.put(("log",RCode.SUCCESS))
                 elif node["request"] == "timeout_add":
                     self.add_event(1,self.time+node.rargs,node.node_id,priority=3)
                     node["state"]="running"
                     node.rqueue.put(("timeout_add",RCode.SUCCESS))
                 elif node["request"] == "notify_add":
@@ -136,15 +141,15 @@
                             selector.append(True)
                         else:
                             selector.append(False)
                     self.events=self.events[~np.array(selector)]
                     node["state"]="running"
                     node.rqueue.put(("notify_remove",RCode.SUCCESS))
                 elif node["request"] == "abort":
-                    self.log("Simulation aborted: "+node.rargs,node=node.node_id)
+                    self.log("Simulation aborted: "+node.rargs,node=node)
                     exit(1)
                 elif node["request"] == "read":
                     node["state"]="running"
                     if node.rargs == "clock":
                         node.rqueue.put(("read",float(self.time)))
                     elif node.rargs[0:5] == "ncom_": # ncom_<interface> register
                         interface=node.rargs[5:]
@@ -155,20 +160,20 @@
                                 count+=1
                         node.rqueue.put(("read",count))
                     else:
                         node.rqueue.put(("read",0)) # Always return 0 if register is unknown
                 elif node["request"] == "turn_on":
                     node["state"]="running"
                     node.rqueue.put(("turn_on",RCode.SUCCESS))
-                    self.log("Turned on",node=node.node_id)
+                    self.log("Turned on",node=node)
                 elif node["request"] == "turn_off":
                     # Update node state after turning off
                     node["state"]="running"
                     node.rqueue.put(("turn_off",RCode.SUCCESS))
-                    self.log("Turned off",node=node.node_id)
+                    self.log("Turned off",node=node)
                     # We cancel communication after node has turned off
                     self.cancel_communications(node.node_id,reason=RCode.RECEIVER_TURNED_OFF)
                 elif node["request"] == "send_cancel":
                     self.cancel_communications(node.node_id)
                     node["state"]="running"
                     node.rqueue.put(("send_cancel",RCode.SUCCESS))
             node.sync()
@@ -277,28 +282,28 @@
                     notify.add(sender)
                 selector.append(select)
             else:
                 selector.append(False)
         if len(selector) != 0:
             self.events=self.events[~np.array(selector)]
             for node in notify:
-                self.log("Interferences on "+interface,node=node)
+                self.log("Interferences on "+interface,node=self.nodes[node])
         return status
     
     def sync_node_blocking(self, node):
         """
         Collect events from the nodes
         """
         if node["state"] == "call_blocking":
             if node["request"] == "send":
                 node["state"]="pending"
                 interface, data, datasize, dst, receiver_required=node.rargs
                 if dst != None: 
                     if not (dst >=0 and dst <=len(self.nodes)):
-                        self.log("Invalid dst used in send() or sendt(), node "+str(dst)+" not found", node=node.node_id)
+                        self.log("Invalid dst used in send() or sendt(), node "+str(dst)+" not found", node=node)
                         exit(1)
                 if not self.communicate(interface, node.node_id, dst, data, datasize,receiver_required):
                     node["state"]="running"
                     node.rqueue.put(("send",RCode.RECEIVER_UNAVAILABLE))
                     # Do not forget to collect the next event (since current event did not happend)
                     # Be careful in node implementation to have no infinite loop when receiver_required=True
                     self.sync_node_non_blocking(node)
@@ -319,38 +324,41 @@
 
     def communicate(self, interface, src, dst, data, datasize,receiver_required):
         """
         Create communication event between src and dst
         """
         nsrc=self.nodes[src]
         if self.netmat[interface]["is_wired"]:
-            self.log("Send "+str(datasize)+" bytes to n"+str(dst)+" on "+interface,node=src)
+            if interface not in self.nodes[dst]["interfaces"]:
+                self.log("Cannot create communication from node "+str(src)+ " to "+str(dst)+", interface "+interface+" not available on node "+str(dst))
+                exit(1)
+            self.log("Send "+str(datasize)+" bytes to n"+str(dst)+" on "+interface,node=nsrc)
             if not self.nodes[dst]["turned_on"] and receiver_required:
                 return(False)
             self.update_sharing(dst,1,interface) # Update sharing first
             # Note that in the following we send more data than expected to handle bandwidth sharing (datasize*8*sharing):
             duration=datasize*8/(self.netmat[interface]["bandwidth"][src,dst]/self.sharing[interface][dst])+self.netmat[interface]["latency"][src,dst]
             self.add_event(0,duration+self.time,(src,dst,interface,data,datasize,duration,datasize,self.time,self.nodes[dst]["turned_on"],receiver_required))
         else:
-            self.log("Send "+str(datasize)+" bytes on "+interface,node=src)
+            self.log("Send "+str(datasize)+" bytes on "+interface,node=nsrc)
             for dst in self.list_receivers(nsrc,interface):
-                if self.nodes[dst]["turned_on"]:
+                if interface in self.nodes[dst]["interfaces"] and self.nodes[dst]["turned_on"]:
                     duration=datasize*8/self.netmat[interface]["bandwidth"][src,dst]+self.netmat[interface]["latency"][src,dst]
                     if src == dst:
                         # This event (where src == dst) is used to notify the sender when data is received!
                         # Correspond to the diagonal of the network matrices (bandwidth and latency)
                         self.add_event(0,duration+self.time,(src,dst,interface,data,datasize,duration,datasize,self.time,True,False))
                     elif not self.interferences:
                         self.add_event(0,duration+self.time,(src,dst,interface,data,datasize,duration,datasize,self.time,True,False))
                     elif not self.handle_interferences(src,dst, interface):
                         self.add_event(0,duration+self.time,(src,dst,interface,data,datasize,duration,datasize,self.time,True,False))
         return(True)
     def list_receivers(self,node,interface):
         """
-        Deduce reachable receivers from the bandwidth matrix
+        Deduce reachable receivers from the bandwidth matrix (sender is included in the list!)
         """
         selector = self.netmat[interface]["bandwidth"][node.node_id,] > 0
         return np.arange(0,selector.shape[0])[selector]
 
     def notify_node_plugins(self,node,callback,args):
         node["pending_plugin_notify"]+=1
         node.rqueue.put(("plugin_notify",callback,self.time,args))
@@ -414,15 +422,15 @@
                     src_id,dst_id,interface, data, datasize,duration,datasize_remaining,start_at,perform_delivery,receiver_required=content
                     src=self.nodes[int(src_id)]
                     dst=self.nodes[int(dst_id)]                    
                     if self.netmat[interface]["is_wired"]:
                         if perform_delivery:
                             dst["interfaces"][interface].put((data,start_at,self.time))
                             dst["interfaces_queue_size"][interface]+=1
-                            self.log("Receive "+str(datasize)+" bytes on "+interface,node=int(dst_id))
+                            self.log("Receive "+str(datasize)+" bytes on "+interface,node=dst)
                             # If node is receiving makes it consume (this way if there is a timeout, it will be removed!)
                             if dst["state"] == "call_blocking" and dst["request"] == "receive":
                                 dst["interfaces_queue_size"][interface]-=1
                                 dst["state"]="running"
                                 dst.rqueue.put(("receive",RCode.SUCCESS))
                                 self.sync_node_non_blocking(dst,timeout_remove_only=True)
                             self.notify_node_plugins(dst, "on_communication_end", event)
@@ -433,15 +441,15 @@
                         self.sync_node_non_blocking(src,timeout_remove_only=True)
                         self.notify_node_plugins(src, "on_communication_end", event)
                     else:
                         if src.node_id != dst.node_id:
                             if perform_delivery:
                                 dst["interfaces"][interface].put((data,start_at,self.time))
                                 dst["interfaces_queue_size"][interface]+=1
-                                self.log("Receive "+str(datasize)+" bytes on "+interface,node=int(dst_id))
+                                self.log("Receive "+str(datasize)+" bytes on "+interface,node=dst)
                                 # If node is receiving makes it consume (this way if there is a timeout, it will be removed!)
                                 if dst["state"] == "call_blocking" and dst["request"] == "receive":
                                     dst["interfaces_queue_size"][interface]-=1
                                     dst["state"]="running"
                                     dst.rqueue.put(("receive",RCode.SUCCESS))
                                     self.sync_node_non_blocking(dst,timeout_remove_only=True)
                                 self.notify_node_plugins(dst, "on_communication_end", event)
```

