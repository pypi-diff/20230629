# Comparing `tmp/pwl_writer-1.1.2.tar.gz` & `tmp/pwl_writer-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwl_writer-1.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pwl_writer-1.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pwl_writer-1.1.2.tar` & `pwl_writer-1.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1497 2023-06-23 13:23:50.038539 pwl_writer-1.1.2/.gitignore
--rw-r--r--   0        0        0     1111 2023-06-23 12:40:45.054972 pwl_writer-1.1.2/LICENSE
--rw-r--r--   0        0        0     3934 2023-06-24 11:49:16.390169 pwl_writer-1.1.2/README.md
--rw-r--r--   0        0        0   174330 2023-06-29 14:05:01.474403 pwl_writer-1.1.2/docs/pwl_writer.html
--rw-r--r--   0        0        0     7070 2023-06-29 14:05:00.797017 pwl_writer-1.1.2/docs/pycco.css
--rw-r--r--   0        0        0      190 2023-06-29 14:03:53.860903 pwl_writer-1.1.2/pwl_writer/__init__.py
--rw-r--r--   0        0        0    45771 2023-06-29 14:04:33.913005 pwl_writer-1.1.2/pwl_writer/pwl_writer.py
--rw-r--r--   0        0        0      685 2023-06-24 11:51:38.147038 pwl_writer-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     4594 1970-01-01 00:00:00.000000 pwl_writer-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1497 2023-06-23 13:23:50.038539 pwl_writer-1.1.3/.gitignore
+-rw-r--r--   0        0        0     1111 2023-06-23 12:40:45.054972 pwl_writer-1.1.3/LICENSE
+-rw-r--r--   0        0        0     3934 2023-06-24 11:49:16.390169 pwl_writer-1.1.3/README.md
+-rw-r--r--   0        0        0   178465 2023-06-29 14:42:19.179958 pwl_writer-1.1.3/docs/pwl_writer.html
+-rw-r--r--   0        0        0     7070 2023-06-29 14:42:18.865952 pwl_writer-1.1.3/docs/pycco.css
+-rw-r--r--   0        0        0      190 2023-06-29 14:43:14.609223 pwl_writer-1.1.3/pwl_writer/__init__.py
+-rw-r--r--   0        0        0    46836 2023-06-29 14:42:12.360007 pwl_writer-1.1.3/pwl_writer/pwl_writer.py
+-rw-r--r--   0        0        0      685 2023-06-24 11:51:38.147038 pwl_writer-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     4594 1970-01-01 00:00:00.000000 pwl_writer-1.1.3/PKG-INFO
```

### Comparing `pwl_writer-1.1.2/.gitignore` & `pwl_writer-1.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pwl_writer-1.1.2/LICENSE` & `pwl_writer-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pwl_writer-1.1.2/README.md` & `pwl_writer-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pwl_writer-1.1.2/docs/pwl_writer.html` & `pwl_writer-1.1.3/docs/pwl_writer.html`

 * *Files 0% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 <li><a href="#package-summary">Package Summary</a></li>
 <li><a href="#precision-related-exception">Precision Related Exception</a></li>
 <li><a href="#pwl-class">PWL Class</a><ul>
 <li>Dunder Methods<ul>
 <li><a href="#initializer">Initializer</a></li>
 <li><a href="#string-representation">String Representation</a></li>
 <li><a href="#length-calculator">Length Calculator</a></li>
+<li><a href="#object-as-a-callable">Object as a Callable</a></li>
 </ul>
 </li>
 <li>Properties<ul>
 <li><a href="#time-coordinates">Time Coordinates</a></li>
 <li><a href="#dependent-coordinates">Dependent Coordinates</a></li>
 <li><a href="#default-timestep">Default Timestep</a></li>
 <li><a href="#name">Name</a></li>
@@ -275,15 +276,15 @@
 <ul>
 <li><code>t_step</code> (<code>float</code>) : Default timestep for all operations. Should be strictly positive.</li>
 <li><code>name</code> (<code>str</code>, optional) : Name of the <code>PWL</code> object used for verbose output printing. Should not be empty. If not set, automatically generates a name based on already taken names.</li>
 <li><code>verbose</code> (<code>bool</code>, optional) : Flag indicating if verbose output should be printed. If not set, defaults to <code>False</code>.</li>
 </ul>
 <h3>Raises</h3>
 <ul>
-<li><code>TypeError</code> : Raised if any of the arguments has an invalid type.</li>
+<li><code>TypeError</code> : Raised if either <code>t_step</code> is not a real number, <code>name</code> is not a string or <code>verbose</code> is not a boolean.</li>
 <li><code>ValueError</code> : Raised if <code>t_step</code> is not strictly positive or <code>name</code> is empty.</li>
 </ul>
     </div>
     <div class='code'>
       <div class="highlight"><pre>        <span class="k">if</span> <span class="n">name</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
             <span class="n">i</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">0</span>
             <span class="k">while</span> <span class="sa">f</span><span class="s2">&quot;pwl_</span><span class="si">{</span><span class="n">i</span><span class="si">}</span><span class="s2">&quot;</span> <span class="ow">in</span> <span class="n">PWL</span><span class="o">.</span><span class="n">__dict_of_objects</span><span class="p">:</span>
@@ -441,52 +442,62 @@
   </div>
   <div class='clearall'></div>
   <div class='section' id='section-22'>
     <div class='docs'>
       <div class='octowrap'>
         <a class='octothorpe' href='#section-22'>#</a>
       </div>
-      <h2><span id="time-coordinates" href="time-coordinates"> Time Coordinates </span></h2>
+      <h2><span id="object-as-a-callable" href="object-as-a-callable"> Object as a Callable </span></h2>
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
   <div class='section' id='section-23'>
     <div class='docs'>
       <div class='octowrap'>
         <a class='octothorpe' href='#section-23'>#</a>
       </div>
-      <p><strong><code>t_list</code> property of <code>PWL</code> class</strong></p>
+      <p><strong>Dunder method <code>__call__</code> of <code>PWL</code> class</strong></p>
     </div>
     <div class='code'>
-      <div class="highlight"><pre>    <span class="nd">@property</span>
-    <span class="k">def</span> <span class="nf">t_list</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">List</span><span class="p">[</span><span class="nb">float</span><span class="p">]:</span></pre></div>
+      <div class="highlight"><pre>    <span class="k">def</span> <span class="fm">__call__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">t</span><span class="p">:</span> <span class="nb">float</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">float</span><span class="p">:</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
   <div class='section' id='section-24'>
     <div class='docs'>
       <div class='octowrap'>
         <a class='octothorpe' href='#section-24'>#</a>
       </div>
-      <h3>Type</h3>
+      <h3>Summary</h3>
+<p>Call <code>PWL</code> object as a function by linearly interpolating between it&rsquo;s time and dependent coordinates.</p>
+<h3>Arguments</h3>
 <ul>
-<li><code>list[float]</code></li>
+<li><code>t</code> (<code>float</code>) : Time instant to evaluate the object at. If negative, returns zero. If bigger than the duration of the object, returns the object&rsquo;s last dependent coordinate.</li>
+</ul>
+<h3>Returns</h3>
+<ul>
+<li><code>float</code></li>
 </ul>
-<h3>Summary</h3>
-<p>Read only property containing all the time coordinates of a <code>PWL</code> object.</p>
 <h3>Raises</h3>
 <ul>
-<li><code>AttributeError</code> : Raised if assignment was attempetd.</li>
+<li><code>TypeError</code> : Raised if <code>t</code> is not a real number.</li>
 </ul>
     </div>
     <div class='code'>
-      <div class="highlight"><pre>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_t_list</span></pre></div>
+      <div class="highlight"><pre>        <span class="k">if</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">t</span><span class="p">,</span> <span class="n">Real</span><span class="p">):</span>
+            <span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span>
+                <span class="sa">f</span><span class="s2">&quot;Argument &#39;t&#39; should be a real number but has type &#39;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">t</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">&#39;.&quot;</span><span class="p">)</span>
+
+        <span class="n">t_list</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_t_list</span>
+        <span class="n">x_list</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_x_list</span>
+
+        <span class="k">return</span> <span class="n">np</span><span class="o">.</span><span class="n">interp</span><span class="p">(</span><span class="n">x</span><span class="o">=</span><span class="n">t</span><span class="p">,</span> <span class="n">xp</span><span class="o">=</span><span class="n">t_list</span><span class="p">,</span> <span class="n">fp</span><span class="o">=</span><span class="n">x_list</span><span class="p">,</span> <span class="n">left</span><span class="o">=</span><span class="mi">0</span><span class="p">)</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
   <div class='section' id='section-25'>
     <div class='docs'>
       <div class='octowrap'>
         <a class='octothorpe' href='#section-25'>#</a>
@@ -499,52 +510,52 @@
   </div>
   <div class='clearall'></div>
   <div class='section' id='section-26'>
     <div class='docs'>
       <div class='octowrap'>
         <a class='octothorpe' href='#section-26'>#</a>
       </div>
-      <h2><span id="dependent-coordinates" href="dependent-coordinates"> Dependent Coordinates </span></h2>
+      <h2><span id="time-coordinates" href="time-coordinates"> Time Coordinates </span></h2>
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
   <div class='section' id='section-27'>
     <div class='docs'>
       <div class='octowrap'>
         <a class='octothorpe' href='#section-27'>#</a>
       </div>
-      <p><strong><code>x_list</code> property of <code>PWL</code> class</strong></p>
+      <p><strong><code>t_list</code> property of <code>PWL</code> class</strong></p>
     </div>
     <div class='code'>
       <div class="highlight"><pre>    <span class="nd">@property</span>
-    <span class="k">def</span> <span class="nf">x_list</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">List</span><span class="p">[</span><span class="nb">float</span><span class="p">]:</span></pre></div>
+    <span class="k">def</span> <span class="nf">t_list</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">List</span><span class="p">[</span><span class="nb">float</span><span class="p">]:</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
   <div class='section' id='section-28'>
     <div class='docs'>
       <div class='octowrap'>
         <a class='octothorpe' href='#section-28'>#</a>
       </div>
       <h3>Type</h3>
 <ul>
 <li><code>list[float]</code></li>
 </ul>
 <h3>Summary</h3>
-<p>Read only property containing all the dependent coordinates of a <code>PWL</code> object.</p>
+<p>Read only property containing all the time coordinates of a <code>PWL</code> object.</p>
 <h3>Raises</h3>
 <ul>
 <li><code>AttributeError</code> : Raised if assignment was attempetd.</li>
 </ul>
     </div>
     <div class='code'>
-      <div class="highlight"><pre>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_x_list</span></pre></div>
+      <div class="highlight"><pre>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_t_list</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
   <div class='section' id='section-29'>
     <div class='docs'>
       <div class='octowrap'>
         <a class='octothorpe' href='#section-29'>#</a>
@@ -557,41 +568,99 @@
   </div>
   <div class='clearall'></div>
   <div class='section' id='section-30'>
     <div class='docs'>
       <div class='octowrap'>
         <a class='octothorpe' href='#section-30'>#</a>
       </div>
-      <h2><span id="default-timestep" href="default-timestep"> Default Timestep </span></h2>
+      <h2><span id="dependent-coordinates" href="dependent-coordinates"> Dependent Coordinates </span></h2>
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
   <div class='section' id='section-31'>
     <div class='docs'>
       <div class='octowrap'>
         <a class='octothorpe' href='#section-31'>#</a>
       </div>
-      <p><strong><code>t_step</code> property of <code>PWL</code> class</strong></p>
+      <p><strong><code>x_list</code> property of <code>PWL</code> class</strong></p>
     </div>
     <div class='code'>
       <div class="highlight"><pre>    <span class="nd">@property</span>
-    <span class="k">def</span> <span class="nf">t_step</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">float</span><span class="p">:</span></pre></div>
+    <span class="k">def</span> <span class="nf">x_list</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">List</span><span class="p">[</span><span class="nb">float</span><span class="p">]:</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
   <div class='section' id='section-32'>
     <div class='docs'>
       <div class='octowrap'>
         <a class='octothorpe' href='#section-32'>#</a>
       </div>
       <h3>Type</h3>
 <ul>
+<li><code>list[float]</code></li>
+</ul>
+<h3>Summary</h3>
+<p>Read only property containing all the dependent coordinates of a <code>PWL</code> object.</p>
+<h3>Raises</h3>
+<ul>
+<li><code>AttributeError</code> : Raised if assignment was attempetd.</li>
+</ul>
+    </div>
+    <div class='code'>
+      <div class="highlight"><pre>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_x_list</span></pre></div>
+    </div>
+  </div>
+  <div class='clearall'></div>
+  <div class='section' id='section-33'>
+    <div class='docs'>
+      <div class='octowrap'>
+        <a class='octothorpe' href='#section-33'>#</a>
+      </div>
+      <hr />
+    </div>
+    <div class='code'>
+      <div class="highlight"><pre></pre></div>
+    </div>
+  </div>
+  <div class='clearall'></div>
+  <div class='section' id='section-34'>
+    <div class='docs'>
+      <div class='octowrap'>
+        <a class='octothorpe' href='#section-34'>#</a>
+      </div>
+      <h2><span id="default-timestep" href="default-timestep"> Default Timestep </span></h2>
+    </div>
+    <div class='code'>
+      <div class="highlight"><pre></pre></div>
+    </div>
+  </div>
+  <div class='clearall'></div>
+  <div class='section' id='section-35'>
+    <div class='docs'>
+      <div class='octowrap'>
+        <a class='octothorpe' href='#section-35'>#</a>
+      </div>
+      <p><strong><code>t_step</code> property of <code>PWL</code> class</strong></p>
+    </div>
+    <div class='code'>
+      <div class="highlight"><pre>    <span class="nd">@property</span>
+    <span class="k">def</span> <span class="nf">t_step</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">float</span><span class="p">:</span></pre></div>
+    </div>
+  </div>
+  <div class='clearall'></div>
+  <div class='section' id='section-36'>
+    <div class='docs'>
+      <div class='octowrap'>
+        <a class='octothorpe' href='#section-36'>#</a>
+      </div>
+      <h3>Type</h3>
+<ul>
 <li><code>float</code></li>
 </ul>
 <h3>Summary</h3>
 <p>Property defining the default timestep of a <code>PWL</code> object.</p>
 <h3>Raises</h3>
 <ul>
 <li><code>TypeError</code> : Raised if the assigned value is not a real number.</li>
@@ -599,18 +668,18 @@
 </ul>
     </div>
     <div class='code'>
       <div class="highlight"><pre>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_t_step</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-33'>
+  <div class='section' id='section-37'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-33'>#</a>
+        <a class='octothorpe' href='#section-37'>#</a>
       </div>
       
     </div>
     <div class='code'>
       <div class="highlight"><pre>    <span class="nd">@t_step</span><span class="o">.</span><span class="n">setter</span>
     <span class="k">def</span> <span class="nf">t_step</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">new_t_step</span><span class="p">:</span> <span class="nb">float</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span>
         <span class="k">if</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">new_t_step</span><span class="p">,</span> <span class="nb">float</span><span class="p">):</span>
@@ -620,55 +689,55 @@
             <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span>
                 <span class="sa">f</span><span class="s2">&quot;Propety &#39;t_step&#39; should be strictly positive but a value of </span><span class="si">{</span><span class="n">new_t_step</span><span class="si">}</span><span class="s2"> was assigned to it.&quot;</span><span class="p">)</span>
 
         <span class="bp">self</span><span class="o">.</span><span class="n">_t_step</span> <span class="o">=</span> <span class="n">new_t_step</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-34'>
+  <div class='section' id='section-38'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-34'>#</a>
+        <a class='octothorpe' href='#section-38'>#</a>
       </div>
       <hr />
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-35'>
+  <div class='section' id='section-39'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-35'>#</a>
+        <a class='octothorpe' href='#section-39'>#</a>
       </div>
       <h2><span id="name" href="name"> Name </span></h2>
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-36'>
+  <div class='section' id='section-40'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-36'>#</a>
+        <a class='octothorpe' href='#section-40'>#</a>
       </div>
       <p><strong><code>name</code> property of <code>PWL</code> class</strong></p>
     </div>
     <div class='code'>
       <div class="highlight"><pre>    <span class="nd">@property</span>
     <span class="k">def</span> <span class="nf">name</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-37'>
+  <div class='section' id='section-41'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-37'>#</a>
+        <a class='octothorpe' href='#section-41'>#</a>
       </div>
       <h3>Type</h3>
 <ul>
 <li><code>str</code></li>
 </ul>
 <h3>Summary</h3>
 <p>Property defining the name of a <code>PWL</code> object for verbose output printing.</p>
@@ -679,18 +748,18 @@
 </ul>
     </div>
     <div class='code'>
       <div class="highlight"><pre>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_name</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-38'>
+  <div class='section' id='section-42'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-38'>#</a>
+        <a class='octothorpe' href='#section-42'>#</a>
       </div>
       
     </div>
     <div class='code'>
       <div class="highlight"><pre>    <span class="nd">@name</span><span class="o">.</span><span class="n">setter</span>
     <span class="k">def</span> <span class="nf">name</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">new_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span>
         <span class="k">if</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">new_name</span><span class="p">,</span> <span class="nb">str</span><span class="p">):</span>
@@ -705,55 +774,55 @@
 
         <span class="n">PWL</span><span class="o">.</span> <span class="n">__dict_of_objects</span><span class="o">.</span><span class="n">pop</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_name</span><span class="p">)</span>
         <span class="n">PWL</span><span class="o">.</span> <span class="n">__dict_of_objects</span><span class="p">[</span><span class="n">new_name</span><span class="p">]</span> <span class="o">=</span> <span class="bp">self</span>
         <span class="bp">self</span><span class="o">.</span><span class="n">_name</span> <span class="o">=</span> <span class="n">new_name</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-39'>
+  <div class='section' id='section-43'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-39'>#</a>
+        <a class='octothorpe' href='#section-43'>#</a>
       </div>
       <hr />
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-40'>
+  <div class='section' id='section-44'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-40'>#</a>
+        <a class='octothorpe' href='#section-44'>#</a>
       </div>
       <h2><span id="verbose-flag" href="verbose-flag"> Verbose Flag </span></h2>
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-41'>
+  <div class='section' id='section-45'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-41'>#</a>
+        <a class='octothorpe' href='#section-45'>#</a>
       </div>
       <p><strong><code>verbose</code> property of <code>PWL</code> class</strong></p>
     </div>
     <div class='code'>
       <div class="highlight"><pre>    <span class="nd">@property</span>
     <span class="k">def</span> <span class="nf">verbose</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-42'>
+  <div class='section' id='section-46'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-42'>#</a>
+        <a class='octothorpe' href='#section-46'>#</a>
       </div>
       <h3>Type</h3>
 <ul>
 <li><code>bool</code></li>
 </ul>
 <h3>Summary</h3>
 <p>Property defining if verbose output should be printed or not.</p>
@@ -763,73 +832,73 @@
 </ul>
     </div>
     <div class='code'>
       <div class="highlight"><pre>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_verbose</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-43'>
+  <div class='section' id='section-47'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-43'>#</a>
+        <a class='octothorpe' href='#section-47'>#</a>
       </div>
       
     </div>
     <div class='code'>
       <div class="highlight"><pre>    <span class="nd">@verbose</span><span class="o">.</span><span class="n">setter</span>
     <span class="k">def</span> <span class="nf">verbose</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">new_verbose</span><span class="p">:</span> <span class="nb">bool</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span>
 
         <span class="k">if</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">new_verbose</span><span class="p">,</span> <span class="nb">bool</span><span class="p">):</span>
             <span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span>
                 <span class="sa">f</span><span class="s2">&quot;Attribute &#39;verbose&#39; should be a boolean but an object of type &#39;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">new_verbose</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">&#39; was assigned to it.&quot;</span><span class="p">)</span>
         <span class="bp">self</span><span class="o">.</span><span class="n">_verbose</span> <span class="o">=</span> <span class="n">new_verbose</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-44'>
+  <div class='section' id='section-48'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-44'>#</a>
+        <a class='octothorpe' href='#section-48'>#</a>
       </div>
       <hr />
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-45'>
+  <div class='section' id='section-49'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-45'>#</a>
+        <a class='octothorpe' href='#section-49'>#</a>
       </div>
       <h2><span id="plot-enable-flag" href="plot-enable-flag"> Plot Enable Flag </span></h2>
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-46'>
+  <div class='section' id='section-50'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-46'>#</a>
+        <a class='octothorpe' href='#section-50'>#</a>
       </div>
       <p><strong><code>plot_flag</code> property of <code>PWL</code> class</strong></p>
     </div>
     <div class='code'>
       <div class="highlight"><pre>    <span class="nd">@property</span>
     <span class="k">def</span> <span class="nf">plot_flag</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-47'>
+  <div class='section' id='section-51'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-47'>#</a>
+        <a class='octothorpe' href='#section-51'>#</a>
       </div>
       <p><em>Optional feature: Requires matplotlib</em></p>
 <h3>Type</h3>
 <ul>
 <li><code>bool</code></li>
 </ul>
 <h3>Summary</h3>
@@ -848,18 +917,18 @@
             <span class="nb">print</span><span class="p">(</span>
                 <span class="s2">&quot;Optional features deactivated. Using the plot_flag does nothing in this case.&quot;</span><span class="p">)</span>
 
         <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_plot_flag</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-48'>
+  <div class='section' id='section-52'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-48'>#</a>
+        <a class='octothorpe' href='#section-52'>#</a>
       </div>
       
     </div>
     <div class='code'>
       <div class="highlight"><pre>    <span class="nd">@plot_flag</span><span class="o">.</span><span class="n">setter</span>
     <span class="k">def</span> <span class="nf">plot_flag</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">new_plot_flag</span><span class="p">:</span> <span class="nb">bool</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span>
 
@@ -871,54 +940,54 @@
             <span class="nb">print</span><span class="p">(</span>
                 <span class="s2">&quot;Optional features deactivated. Using the plot_flag does nothing in this case.&quot;</span><span class="p">)</span>
 
         <span class="bp">self</span><span class="o">.</span><span class="n">_plot_flag</span> <span class="o">=</span> <span class="n">new_plot_flag</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-49'>
+  <div class='section' id='section-53'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-49'>#</a>
+        <a class='octothorpe' href='#section-53'>#</a>
       </div>
       <hr />
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-50'>
+  <div class='section' id='section-54'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-50'>#</a>
+        <a class='octothorpe' href='#section-54'>#</a>
       </div>
       <h2><span id="last-value-holder" href="last-value-holder"> Last Value Holder </span></h2>
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-51'>
+  <div class='section' id='section-55'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-51'>#</a>
+        <a class='octothorpe' href='#section-55'>#</a>
       </div>
       <p><strong><code>hold</code> method of <code>PWL</code> class</strong></p>
     </div>
     <div class='code'>
       <div class="highlight"><pre>    <span class="k">def</span> <span class="nf">hold</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">duration</span><span class="p">:</span> <span class="nb">float</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-52'>
+  <div class='section' id='section-56'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-52'>#</a>
+        <a class='octothorpe' href='#section-56'>#</a>
       </div>
       <h3>Summary</h3>
 <p>Method that holds the last value from the previous event for a given duration.</p>
 <p>If the <code>PWL</code> object is empty, adds the point <code>(0, 0)</code> and holds that.</p>
 <h3>Parameters</h3>
 <ul>
 <li><code>duration</code> (<code>float</code>) : Duration to hold the last value for. Should be strictly positive.</li>
@@ -950,54 +1019,54 @@
         <span class="n">last_t</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_t_list</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span>
         <span class="n">last_x</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_x_list</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span>
 
         <span class="bp">self</span><span class="o">.</span><span class="n">_add</span><span class="p">(</span><span class="n">last_t</span><span class="o">+</span><span class="n">duration</span><span class="p">,</span> <span class="n">last_x</span><span class="p">)</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-53'>
+  <div class='section' id='section-57'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-53'>#</a>
+        <a class='octothorpe' href='#section-57'>#</a>
       </div>
       <hr />
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-54'>
+  <div class='section' id='section-58'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-54'>#</a>
+        <a class='octothorpe' href='#section-58'>#</a>
       </div>
       <h2><span id="linear-transition" href="linear-transition"> Linear Transition </span></h2>
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-55'>
+  <div class='section' id='section-59'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-55'>#</a>
+        <a class='octothorpe' href='#section-59'>#</a>
       </div>
       <p><strong><code>lin_transition</code> method of <code>PWL</code> class</strong></p>
     </div>
     <div class='code'>
       <div class="highlight"><pre>    <span class="k">def</span> <span class="nf">lin_transition</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">target</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">duration</span><span class="p">:</span> <span class="nb">float</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-56'>
+  <div class='section' id='section-60'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-56'>#</a>
+        <a class='octothorpe' href='#section-60'>#</a>
       </div>
       <h3>Summary</h3>
 <p>Method that generates a linear transition from the last value of the previous event to a given target with a given duration.</p>
 <p>If the <code>PWL</code> object is empty, adds the point <code>(0, 0)</code> and transitions from that.</p>
 <h3>Arguments</h3>
 <ul>
 <li><code>target</code> (<code>float</code>) : Value to transition to.</li>
@@ -1022,54 +1091,54 @@
             <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span>
                 <span class="sa">f</span><span class="s2">&quot;Argument &#39;duration&#39; should be strictly positive but has value of </span><span class="si">{</span><span class="n">duration</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
 
         <span class="bp">self</span><span class="o">.</span><span class="n">_lin_transition</span><span class="p">(</span><span class="n">target</span><span class="p">,</span> <span class="n">duration</span><span class="p">,</span> <span class="mi">0</span><span class="p">)</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-57'>
+  <div class='section' id='section-61'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-57'>#</a>
+        <a class='octothorpe' href='#section-61'>#</a>
       </div>
       <hr />
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-58'>
+  <div class='section' id='section-62'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-58'>#</a>
+        <a class='octothorpe' href='#section-62'>#</a>
       </div>
       <h2><span id="rectangular-pulse" href="rectangular-pulse"> Rectangular Pulse </span></h2>
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-59'>
+  <div class='section' id='section-63'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-59'>#</a>
+        <a class='octothorpe' href='#section-63'>#</a>
       </div>
       <p><strong><code>rect_pulse</code> method of <code>PWL</code> class</strong></p>
     </div>
     <div class='code'>
       <div class="highlight"><pre>    <span class="k">def</span> <span class="nf">rect_pulse</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">duration</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">t_step</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="nb">float</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-60'>
+  <div class='section' id='section-64'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-60'>#</a>
+        <a class='octothorpe' href='#section-64'>#</a>
       </div>
       <h3>Summary</h3>
 <p>Method that generates a rectangular pulse with given amplitude and duration.</p>
 <p>If <code>duration</code> is less than or equal to <code>t_step</code> (<code>self.t_step</code> if <code>t_step</code> is not set), substitutes the pulse by a linear transition from the last value of the previous event to <code>value</code> with duration <code>t_step</code> (<code>self.t_step</code> if <code>t_step</code> is not set).</p>
 <h3>Arguments</h3>
 <ul>
 <li><code>value</code> (<code>float</code>) : Amplitude of the pulse.</li>
@@ -1125,54 +1194,54 @@
             <span class="n">last_t</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_t_list</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">_add</span><span class="p">(</span><span class="n">last_t</span><span class="o">+</span><span class="n">t_step</span><span class="p">,</span> <span class="n">value</span><span class="p">)</span>
 
         <span class="bp">self</span><span class="o">.</span><span class="n">_add</span><span class="p">(</span><span class="n">last_t</span><span class="o">+</span><span class="n">duration</span><span class="p">,</span> <span class="n">value</span><span class="p">)</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-61'>
+  <div class='section' id='section-65'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-61'>#</a>
+        <a class='octothorpe' href='#section-65'>#</a>
       </div>
       <hr />
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-62'>
+  <div class='section' id='section-66'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-62'>#</a>
+        <a class='octothorpe' href='#section-66'>#</a>
       </div>
       <h2><span id="sawtooth-pulse" href="sawtooth-pulse"> Sawtooth Pulse </span></h2>
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-63'>
+  <div class='section' id='section-67'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-63'>#</a>
+        <a class='octothorpe' href='#section-67'>#</a>
       </div>
       <p><strong><code>sawtooth_pulse</code> method of <code>PWL</code> class</strong></p>
     </div>
     <div class='code'>
       <div class="highlight"><pre>    <span class="k">def</span> <span class="nf">sawtooth_pulse</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">start</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">end</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">duration</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">t_step</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="nb">float</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-64'>
+  <div class='section' id='section-68'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-64'>#</a>
+        <a class='octothorpe' href='#section-68'>#</a>
       </div>
       <h3>Summary</h3>
 <p>Method that generates a sawtooth pulse with given starting and ending amplitudes and duration.</p>
 <p>If <code>duration</code> is less than or equal to <code>t_step</code> (<code>self.t_step</code> if <code>t_step</code> is not set), substitutes the pulse by a linear transition from the last value of the previous event to <code>end</code> with duration <code>t_step</code> (<code>self.t_step</code> if <code>t_step</code> is not set).</p>
 <h3>Arguments</h3>
 <ul>
 <li><code>start</code> (<code>float</code>) : Amplitude at the start of the pulse.</li>
@@ -1232,54 +1301,54 @@
             <span class="n">last_t</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_t_list</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">_add</span><span class="p">(</span><span class="n">last_t</span><span class="o">+</span><span class="n">t_step</span><span class="p">,</span> <span class="n">start</span><span class="p">)</span>
 
         <span class="bp">self</span><span class="o">.</span><span class="n">_add</span><span class="p">(</span><span class="n">last_t</span><span class="o">+</span><span class="n">duration</span><span class="p">,</span> <span class="n">end</span><span class="p">)</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-65'>
+  <div class='section' id='section-69'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-65'>#</a>
+        <a class='octothorpe' href='#section-69'>#</a>
       </div>
       <hr />
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-66'>
+  <div class='section' id='section-70'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-66'>#</a>
+        <a class='octothorpe' href='#section-70'>#</a>
       </div>
       <h2><span id="exponential-transition" href="exponential-transition"> Exponential Transition </span></h2>
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-67'>
+  <div class='section' id='section-71'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-67'>#</a>
+        <a class='octothorpe' href='#section-71'>#</a>
       </div>
       <p><strong><code>exp_transition</code> method of <code>PWL</code> class</strong></p>
     </div>
     <div class='code'>
       <div class="highlight"><pre>    <span class="k">def</span> <span class="nf">exp_transition</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">target</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">duration</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">tau</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">t_step</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="nb">float</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-68'>
+  <div class='section' id='section-72'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-68'>#</a>
+        <a class='octothorpe' href='#section-72'>#</a>
       </div>
       <h3>Summary</h3>
 <p>Method that generates an exponential transition from the last value of the previous event to a given target with a given duration.</p>
 <p>If the <code>PWL</code> object is empty, adds the point <code>(0, 0)</code> and transitions from that.</p>
 <p>Let&rsquo;s call <code>x0</code> the last value of the previous event and <code>t0</code> the instant when the transition begins. The transition will follow thw following form:</p>
 <pre><code>f(t) = A + B*exp(-t/tau)
 </code></pre>
@@ -1357,54 +1426,54 @@
         <span class="k">for</span> <span class="n">t</span> <span class="ow">in</span> <span class="n">np</span><span class="o">.</span><span class="n">arange</span><span class="p">(</span><span class="n">last_t</span><span class="o">+</span><span class="n">t_step</span><span class="p">,</span> <span class="n">last_t</span><span class="o">+</span><span class="n">duration</span><span class="p">,</span> <span class="n">t_step</span><span class="p">):</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">_add</span><span class="p">(</span><span class="n">t</span><span class="p">,</span> <span class="n">f</span><span class="p">(</span><span class="n">t</span><span class="p">))</span>
 
         <span class="bp">self</span><span class="o">.</span><span class="n">_add</span><span class="p">(</span><span class="n">last_t</span><span class="o">+</span><span class="n">duration</span><span class="p">,</span> <span class="n">target</span><span class="p">)</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-69'>
+  <div class='section' id='section-73'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-69'>#</a>
+        <a class='octothorpe' href='#section-73'>#</a>
       </div>
       <hr />
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-70'>
+  <div class='section' id='section-74'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-70'>#</a>
+        <a class='octothorpe' href='#section-74'>#</a>
       </div>
       <h2><span id="half-sine-transition" href="half-sine-transition"> Half Sine Transition </span></h2>
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-71'>
+  <div class='section' id='section-75'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-71'>#</a>
+        <a class='octothorpe' href='#section-75'>#</a>
       </div>
       <p><strong><code>sin_transition</code> method of <code>PWL</code> class</strong></p>
     </div>
     <div class='code'>
       <div class="highlight"><pre>    <span class="k">def</span> <span class="nf">sin_transition</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">target</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">duration</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">t_step</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="nb">float</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-72'>
+  <div class='section' id='section-76'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-72'>#</a>
+        <a class='octothorpe' href='#section-76'>#</a>
       </div>
       <h3>Summary</h3>
 <p>Method that generates a half sine transition from the last value of the previous event to a given target with a given duration.</p>
 <p>If the <code>PWL</code> object is empty, adds the point <code>(0, 0)</code> and transitions from that.</p>
 <p>Let&rsquo;s call <code>x0</code> the last value of the previous event and <code>t0</code> the instant when the transition begins. The transition will follow thw following form:</p>
 <pre><code>f(t) = A + B*sin(w*t - phi)
 </code></pre>
@@ -1477,54 +1546,54 @@
         <span class="k">for</span> <span class="n">t</span> <span class="ow">in</span> <span class="n">np</span><span class="o">.</span><span class="n">arange</span><span class="p">(</span><span class="n">last_t</span><span class="o">+</span><span class="n">t_step</span><span class="p">,</span> <span class="n">last_t</span><span class="o">+</span><span class="n">duration</span><span class="p">,</span> <span class="n">t_step</span><span class="p">):</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">_add</span><span class="p">(</span><span class="n">t</span><span class="p">,</span> <span class="n">f</span><span class="p">(</span><span class="n">t</span><span class="p">))</span>
 
         <span class="bp">self</span><span class="o">.</span><span class="n">_add</span><span class="p">(</span><span class="n">last_t</span><span class="o">+</span><span class="n">duration</span><span class="p">,</span> <span class="n">target</span><span class="p">)</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-73'>
+  <div class='section' id='section-77'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-73'>#</a>
+        <a class='octothorpe' href='#section-77'>#</a>
       </div>
       <hr />
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-74'>
+  <div class='section' id='section-78'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-74'>#</a>
+        <a class='octothorpe' href='#section-78'>#</a>
       </div>
       <h2><span id="smoothstep-transition" href="smoothstep-transition"> Smoothstep Transition </span></h2>
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-75'>
+  <div class='section' id='section-79'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-75'>#</a>
+        <a class='octothorpe' href='#section-79'>#</a>
       </div>
       <p><strong><code>smoothstep_transition</code> method of <code>PWL</code> class</strong></p>
     </div>
     <div class='code'>
       <div class="highlight"><pre>    <span class="k">def</span> <span class="nf">smoothstep_transition</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">target</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">duration</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">t_step</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="nb">float</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-76'>
+  <div class='section' id='section-80'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-76'>#</a>
+        <a class='octothorpe' href='#section-80'>#</a>
       </div>
       <h3>Summary</h3>
 <p>Method that generates a smoothstep transition from the last value of the previous event to a given target with a given duration.</p>
 <p>If the <code>PWL</code> object is empty, adds the point <code>(0, 0)</code> and transitions from that.</p>
 <p>Let&rsquo;s call <code>x0</code> the last value of the previous event and <code>t0</code> the instant when the transition begins. The transition will follow thw following form:</p>
 <pre><code>f(t) = A + B*t + C*t^2 + D*t^3
 </code></pre>
@@ -1596,54 +1665,54 @@
         <span class="k">for</span> <span class="n">t</span> <span class="ow">in</span> <span class="n">np</span><span class="o">.</span><span class="n">arange</span><span class="p">(</span><span class="n">last_t</span><span class="o">+</span><span class="n">t_step</span><span class="p">,</span> <span class="n">last_t</span><span class="o">+</span><span class="n">duration</span><span class="p">,</span> <span class="n">t_step</span><span class="p">):</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">_add</span><span class="p">(</span><span class="n">t</span><span class="p">,</span> <span class="n">f</span><span class="p">(</span><span class="n">t</span><span class="p">))</span>
 
         <span class="bp">self</span><span class="o">.</span><span class="n">_add</span><span class="p">(</span><span class="n">last_t</span><span class="o">+</span><span class="n">duration</span><span class="p">,</span> <span class="n">target</span><span class="p">)</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-77'>
+  <div class='section' id='section-81'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-77'>#</a>
+        <a class='octothorpe' href='#section-81'>#</a>
       </div>
       <hr />
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-78'>
+  <div class='section' id='section-82'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-78'>#</a>
+        <a class='octothorpe' href='#section-82'>#</a>
       </div>
       <h2><span id="pwl-file-writer" href="pwl-file-writer"> PWL File Writer </span></h2>
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-79'>
+  <div class='section' id='section-83'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-79'>#</a>
+        <a class='octothorpe' href='#section-83'>#</a>
       </div>
       <p><strong><code>write</code> method of <code>PWL</code> class</strong></p>
     </div>
     <div class='code'>
       <div class="highlight"><pre>    <span class="k">def</span> <span class="nf">write</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">filename</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">precision</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">10</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-80'>
+  <div class='section' id='section-84'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-80'>#</a>
+        <a class='octothorpe' href='#section-84'>#</a>
       </div>
       <h3>Summary</h3>
 <p>Method that takes a <code>PWL</code> object and writes a PWL file with it&rsquo;s <code>(t, x)</code> coordinates in scientific notation.</p>
 <p>If the specified file already exists, overwrites it.</p>
 <h3>Arguments</h3>
 <ul>
 <li><code>filename</code> (<code>str</code>, optional) : Name of file to be created. If not set, uses <code>self.name</code> if an added <code>.txt</code> extension.</li>
@@ -1694,55 +1763,55 @@
                         <span class="s2">&quot;The chosen precision level caused the written time coordinates to not be strictly increasing.&quot;</span><span class="p">)</span>
                 <span class="n">file</span><span class="o">.</span><span class="n">write</span><span class="p">(</span>
                     <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">ti_str</span><span class="si">}</span><span class="s2">    </span><span class="si">{</span><span class="n">xi_str</span><span class="si">}</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
                 <span class="n">last_t</span> <span class="o">=</span> <span class="n">ti_str</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-81'>
+  <div class='section' id='section-85'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-81'>#</a>
+        <a class='octothorpe' href='#section-85'>#</a>
       </div>
       <hr />
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-82'>
+  <div class='section' id='section-86'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-82'>#</a>
+        <a class='octothorpe' href='#section-86'>#</a>
       </div>
       <h2><span id="pwl-plotter" href="pwl-plotter"> PWL Plotter </span></h2>
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-83'>
+  <div class='section' id='section-87'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-83'>#</a>
+        <a class='octothorpe' href='#section-87'>#</a>
       </div>
       <p><strong><code>plot</code> class method of <code>PWL</code> class</strong></p>
     </div>
     <div class='code'>
       <div class="highlight"><pre>    <span class="nd">@classmethod</span>
     <span class="k">def</span> <span class="nf">plot</span><span class="p">(</span><span class="bp">cls</span><span class="p">,</span> <span class="n">merge</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-84'>
+  <div class='section' id='section-88'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-84'>#</a>
+        <a class='octothorpe' href='#section-88'>#</a>
       </div>
       <p><em>Optional feature: Requires matplotlib</em></p>
 <h3>Summary</h3>
 <p>Class method that takes all instances of the <code>PWL</code> class with plot enable flag set to <code>True</code> and plots them on the same time axis.</p>
 <h3>Arguments</h3>
 <ul>
 <li><code>merge</code> (<code>bool</code>, optional) : Flag indicating if all signals should be ploted on the same strip or separeted. If not set, defaults to False.</li>
@@ -1793,78 +1862,78 @@
             <span class="n">ax</span><span class="o">.</span><span class="n">set_ylabel</span><span class="p">(</span><span class="n">label</span><span class="p">)</span>
 
         <span class="n">axs</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">set_xlim</span><span class="p">(</span><span class="n">xmin</span><span class="o">=</span><span class="mi">0</span><span class="p">,</span> <span class="n">xmax</span><span class="o">=</span><span class="n">x_max</span><span class="p">)</span>
         <span class="n">plt</span><span class="o">.</span><span class="n">show</span><span class="p">()</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-85'>
+  <div class='section' id='section-89'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-85'>#</a>
+        <a class='octothorpe' href='#section-89'>#</a>
       </div>
       <h1><span id="private-methods-and-functions" href="private-methods-and-functions"> Private Methods and Functions </span></h1>
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-86'>
+  <div class='section' id='section-90'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-86'>#</a>
+        <a class='octothorpe' href='#section-90'>#</a>
       </div>
       <p>From this point forward, all listed methods and functions are not intended to be used by the user. Brief descriptions will be provided, but documentation will be kept to a minimum.</p>
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-87'>
+  <div class='section' id='section-91'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-87'>#</a>
+        <a class='octothorpe' href='#section-91'>#</a>
       </div>
       <hr />
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-88'>
+  <div class='section' id='section-92'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-88'>#</a>
+        <a class='octothorpe' href='#section-92'>#</a>
       </div>
       <h2><span id="pwl-point-adder" href="pwl-point-adder"> PWL Point Adder </span></h2>
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-89'>
+  <div class='section' id='section-93'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-89'>#</a>
+        <a class='octothorpe' href='#section-93'>#</a>
       </div>
       <p><strong><code>_add</code> private method of <code>PWL</code> class</strong></p>
     </div>
     <div class='code'>
       <div class="highlight"><pre>    <span class="k">def</span> <span class="nf">_add</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">t</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">x</span><span class="p">:</span> <span class="nb">float</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-90'>
+  <div class='section' id='section-94'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-90'>#</a>
+        <a class='octothorpe' href='#section-94'>#</a>
       </div>
       <p>Private method that adds a <code>(t, x)</code> point to a <code>PWL</code> object of any size.</p>
     </div>
     <div class='code'>
       <div class="highlight"><pre>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_t_list</span><span class="p">)</span> <span class="o">&gt;=</span> <span class="mi">1</span> <span class="ow">and</span> <span class="n">t</span> <span class="o">&lt;=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_t_list</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">]:</span>
             <span class="k">raise</span> <span class="n">PrecisionError</span><span class="p">(</span>
                 <span class="sa">f</span><span class="s2">&quot;Internal Python rounding caused the time coordinates to not be strictly increasing when adding points to </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_name</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
@@ -1873,54 +1942,54 @@
             <span class="bp">self</span><span class="o">.</span><span class="n">_t_list</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">t</span><span class="p">)</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">_x_list</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">x</span><span class="p">)</span>
         <span class="k">else</span><span class="p">:</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">_colinear_eliminator</span><span class="p">(</span><span class="n">x</span><span class="p">,</span> <span class="n">t</span><span class="p">)</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-91'>
+  <div class='section' id='section-95'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-91'>#</a>
+        <a class='octothorpe' href='#section-95'>#</a>
       </div>
       <hr />
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-92'>
+  <div class='section' id='section-96'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-92'>#</a>
+        <a class='octothorpe' href='#section-96'>#</a>
       </div>
       <h2><span id="colinear-points-eliminator" href="colinear-points-eliminator"> Colinear Points Eliminator </span></h2>
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-93'>
+  <div class='section' id='section-97'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-93'>#</a>
+        <a class='octothorpe' href='#section-97'>#</a>
       </div>
       <p><strong><code>_colinear_eliminator</code> private method of <code>PWL</code> class</strong></p>
     </div>
     <div class='code'>
       <div class="highlight"><pre>    <span class="k">def</span> <span class="nf">_colinear_eliminator</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">x</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">t</span><span class="p">:</span> <span class="nb">float</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-94'>
+  <div class='section' id='section-98'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-94'>#</a>
+        <a class='octothorpe' href='#section-98'>#</a>
       </div>
       <p>Private method that adds a <code>(t, x)</code> point to a <code>PWL</code> object with 2 or more points without consecutive colinear points.</p>
     </div>
     <div class='code'>
       <div class="highlight"><pre>        <span class="n">t_n_1</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_t_list</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span>
         <span class="n">t_n_2</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_t_list</span><span class="p">[</span><span class="o">-</span><span class="mi">2</span><span class="p">]</span>
 
@@ -1935,54 +2004,54 @@
             <span class="bp">self</span><span class="o">.</span><span class="n">_x_list</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span> <span class="o">=</span> <span class="n">x</span>
         <span class="k">else</span><span class="p">:</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">_t_list</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">t</span><span class="p">)</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">_x_list</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">x</span><span class="p">)</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-95'>
+  <div class='section' id='section-99'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-95'>#</a>
+        <a class='octothorpe' href='#section-99'>#</a>
       </div>
       <hr />
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-96'>
+  <div class='section' id='section-100'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-96'>#</a>
+        <a class='octothorpe' href='#section-100'>#</a>
       </div>
       <h2><span id="nested-linear-transition" href="nested-linear-transition"> Nested Linear Transition </span></h2>
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-97'>
+  <div class='section' id='section-101'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-97'>#</a>
+        <a class='octothorpe' href='#section-101'>#</a>
       </div>
       <p><strong><code>_lin_transition</code> private method of <code>PWL</code> class</strong></p>
     </div>
     <div class='code'>
       <div class="highlight"><pre>    <span class="k">def</span> <span class="nf">_lin_transition</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">target</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">duration</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">n</span><span class="p">:</span> <span class="nb">int</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-98'>
+  <div class='section' id='section-102'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-98'>#</a>
+        <a class='octothorpe' href='#section-102'>#</a>
       </div>
       <p>Private method to generate a linear transition. The difference between this method and the <a href="#linear-transition">public linear transition</a> method is that this method prints indented verbose output when called from within any of the public methods that revert to a linear transition in certain conditions.</p>
     </div>
     <div class='code'>
       <div class="highlight"><pre>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_verbose</span><span class="p">:</span>
             <span class="k">if</span> <span class="n">n</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
                 <span class="nb">print</span><span class="p">(</span>
@@ -1997,222 +2066,222 @@
             <span class="bp">self</span><span class="o">.</span><span class="n">_add</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="mi">0</span><span class="p">)</span>
 
         <span class="n">last_t</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_t_list</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span>
         <span class="bp">self</span><span class="o">.</span><span class="n">_add</span><span class="p">(</span><span class="n">last_t</span><span class="o">+</span><span class="n">duration</span><span class="p">,</span> <span class="n">target</span><span class="p">)</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-99'>
+  <div class='section' id='section-103'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-99'>#</a>
+        <a class='octothorpe' href='#section-103'>#</a>
       </div>
       <hr />
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-100'>
+  <div class='section' id='section-104'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-100'>#</a>
+        <a class='octothorpe' href='#section-104'>#</a>
       </div>
       <h2><span id="exponential-function-generator" href="exponential-function-generator"> Exponential Function Generator </span></h2>
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-101'>
+  <div class='section' id='section-105'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-101'>#</a>
+        <a class='octothorpe' href='#section-105'>#</a>
       </div>
       <p><strong><code>_exp_transition_func</code> private function</strong></p>
     </div>
     <div class='code'>
       <div class="highlight"><pre><span class="k">def</span> <span class="nf">_exp_transition_func</span><span class="p">(</span><span class="n">tau</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">t1</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">f1</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">t2</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">f2</span><span class="p">:</span> <span class="nb">float</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Callable</span><span class="p">[[</span><span class="nb">float</span><span class="p">],</span> <span class="nb">float</span><span class="p">]:</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-102'>
+  <div class='section' id='section-106'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-102'>#</a>
+        <a class='octothorpe' href='#section-106'>#</a>
       </div>
       <p>Private function that generates an exponential function passing trough 2 fixed points.</p>
     </div>
     <div class='code'>
       <div class="highlight"><pre>    <span class="n">A</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="p">(</span><span class="n">f1</span><span class="o">*</span><span class="n">np</span><span class="o">.</span><span class="n">exp</span><span class="p">(</span><span class="n">t1</span><span class="o">/</span><span class="n">tau</span><span class="p">)</span> <span class="o">-</span> <span class="n">f2</span><span class="o">*</span><span class="n">np</span><span class="o">.</span><span class="n">exp</span><span class="p">(</span><span class="n">t2</span><span class="o">/</span><span class="n">tau</span><span class="p">))</span> <span class="o">/</span> \
         <span class="p">(</span><span class="n">np</span><span class="o">.</span><span class="n">exp</span><span class="p">(</span><span class="n">t1</span><span class="o">/</span><span class="n">tau</span><span class="p">)</span> <span class="o">-</span> <span class="n">np</span><span class="o">.</span><span class="n">exp</span><span class="p">(</span><span class="n">t2</span><span class="o">/</span><span class="n">tau</span><span class="p">))</span>
     <span class="n">B</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="p">(</span><span class="n">f1</span> <span class="o">-</span> <span class="n">f2</span><span class="p">)</span><span class="o">/</span><span class="p">(</span><span class="n">np</span><span class="o">.</span><span class="n">exp</span><span class="p">(</span><span class="o">-</span><span class="n">t1</span><span class="o">/</span><span class="n">tau</span><span class="p">)</span> <span class="o">-</span> <span class="n">np</span><span class="o">.</span><span class="n">exp</span><span class="p">(</span><span class="o">-</span><span class="n">t2</span><span class="o">/</span><span class="n">tau</span><span class="p">))</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-103'>
+  <div class='section' id='section-107'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-103'>#</a>
+        <a class='octothorpe' href='#section-107'>#</a>
       </div>
       
     </div>
     <div class='code'>
       <div class="highlight"><pre>    <span class="k">def</span> <span class="nf">f</span><span class="p">(</span><span class="n">t</span><span class="p">:</span> <span class="nb">float</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">float</span><span class="p">:</span>
         <span class="n">result</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="n">A</span> <span class="o">+</span> <span class="n">B</span><span class="o">*</span><span class="n">np</span><span class="o">.</span><span class="n">exp</span><span class="p">(</span><span class="o">-</span><span class="n">t</span><span class="o">/</span><span class="n">tau</span><span class="p">)</span>
         <span class="k">return</span> <span class="n">result</span>
 
     <span class="k">return</span> <span class="n">f</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-104'>
+  <div class='section' id='section-108'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-104'>#</a>
+        <a class='octothorpe' href='#section-108'>#</a>
       </div>
       <hr />
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-105'>
+  <div class='section' id='section-109'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-105'>#</a>
+        <a class='octothorpe' href='#section-109'>#</a>
       </div>
       <h2><span id="sinusoidal-function-generator" href="sinusoidal-function-generator"> Sinusoidal Function Generator </span></h2>
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-106'>
+  <div class='section' id='section-110'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-106'>#</a>
+        <a class='octothorpe' href='#section-110'>#</a>
       </div>
       <p><strong><code>_sin_transition_func</code> private function</strong></p>
     </div>
     <div class='code'>
       <div class="highlight"><pre><span class="k">def</span> <span class="nf">_sin_transition_func</span><span class="p">(</span><span class="n">t1</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">f1</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">t2</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">f2</span><span class="p">:</span> <span class="nb">float</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Callable</span><span class="p">[[</span><span class="nb">float</span><span class="p">],</span> <span class="nb">float</span><span class="p">]:</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-107'>
+  <div class='section' id='section-111'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-107'>#</a>
+        <a class='octothorpe' href='#section-111'>#</a>
       </div>
       <p>Private function that generates a sinusoidal function passing trough 2 fixed points.</p>
     </div>
     <div class='code'>
       <div class="highlight"><pre>    <span class="n">fm</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="p">(</span><span class="n">f1</span><span class="o">+</span><span class="n">f2</span><span class="p">)</span><span class="o">/</span><span class="mi">2</span>
     <span class="n">tm</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="p">(</span><span class="n">t1</span><span class="o">+</span><span class="n">t2</span><span class="p">)</span><span class="o">/</span><span class="mi">2</span>
     <span class="n">T</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="mi">2</span><span class="o">*</span><span class="p">(</span><span class="n">t2</span><span class="o">-</span><span class="n">t1</span><span class="p">)</span>
     <span class="n">w</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="mi">2</span><span class="o">*</span><span class="n">np</span><span class="o">.</span><span class="n">pi</span><span class="o">/</span><span class="n">T</span>
     <span class="n">phi</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="n">w</span><span class="o">*</span><span class="n">tm</span>
     <span class="n">A</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="n">f2</span><span class="o">-</span><span class="n">fm</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-108'>
+  <div class='section' id='section-112'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-108'>#</a>
+        <a class='octothorpe' href='#section-112'>#</a>
       </div>
       
     </div>
     <div class='code'>
       <div class="highlight"><pre>    <span class="k">def</span> <span class="nf">f</span><span class="p">(</span><span class="n">t</span><span class="p">:</span> <span class="nb">float</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">float</span><span class="p">:</span>
         <span class="n">result</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="n">fm</span> <span class="o">+</span> <span class="n">A</span><span class="o">*</span><span class="n">np</span><span class="o">.</span><span class="n">sin</span><span class="p">(</span><span class="n">w</span><span class="o">*</span><span class="n">t</span> <span class="o">-</span> <span class="n">phi</span><span class="p">)</span>
         <span class="k">return</span> <span class="n">result</span>
 
     <span class="k">return</span> <span class="n">f</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-109'>
+  <div class='section' id='section-113'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-109'>#</a>
+        <a class='octothorpe' href='#section-113'>#</a>
       </div>
       <hr />
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-110'>
+  <div class='section' id='section-114'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-110'>#</a>
+        <a class='octothorpe' href='#section-114'>#</a>
       </div>
       <h2><span id="smoothstep-function-generator" href="smoothstep-function-generator"> Smoothstep Function Generator </span></h2>
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-111'>
+  <div class='section' id='section-115'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-111'>#</a>
+        <a class='octothorpe' href='#section-115'>#</a>
       </div>
       <p><strong><code>_smoothstep_transition_func</code> private function</strong></p>
     </div>
     <div class='code'>
       <div class="highlight"><pre><span class="k">def</span> <span class="nf">_smoothstep_transition_func</span><span class="p">(</span><span class="n">t1</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">f1</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">t2</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">f2</span><span class="p">:</span> <span class="nb">float</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Callable</span><span class="p">[[</span><span class="nb">float</span><span class="p">],</span> <span class="nb">float</span><span class="p">]:</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-112'>
+  <div class='section' id='section-116'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-112'>#</a>
+        <a class='octothorpe' href='#section-116'>#</a>
       </div>
       <p>Private function that generates a smoothstep function passing trough 2 fixed points.</p>
     </div>
     <div class='code'>
       <div class="highlight"><pre>    <span class="n">Am</span> <span class="o">=</span> <span class="n">np</span><span class="o">.</span><span class="n">array</span><span class="p">([[</span><span class="mi">1</span><span class="p">,</span> <span class="n">t1</span><span class="p">,</span> <span class="n">t1</span><span class="o">**</span><span class="mi">2</span><span class="p">,</span> <span class="n">t1</span><span class="o">**</span><span class="mi">3</span><span class="p">],</span>
                    <span class="p">[</span><span class="mi">1</span><span class="p">,</span> <span class="n">t2</span><span class="p">,</span> <span class="n">t2</span><span class="o">**</span><span class="mi">2</span><span class="p">,</span> <span class="n">t2</span><span class="o">**</span><span class="mi">3</span><span class="p">],</span>
                    <span class="p">[</span><span class="mi">0</span><span class="p">,</span> <span class="mi">1</span><span class="p">,</span> <span class="mi">2</span><span class="o">*</span><span class="n">t1</span><span class="p">,</span> <span class="mi">3</span><span class="o">*</span><span class="n">t1</span><span class="o">**</span><span class="mi">2</span><span class="p">],</span>
                    <span class="p">[</span><span class="mi">0</span><span class="p">,</span> <span class="mi">1</span><span class="p">,</span> <span class="mi">2</span><span class="o">*</span><span class="n">t2</span><span class="p">,</span> <span class="mi">3</span><span class="o">*</span><span class="n">t2</span><span class="o">**</span><span class="mi">2</span><span class="p">]])</span>
     <span class="n">Bm</span> <span class="o">=</span> <span class="n">np</span><span class="o">.</span><span class="n">array</span><span class="p">([</span><span class="n">f1</span><span class="p">,</span> <span class="n">f2</span><span class="p">,</span> <span class="mi">0</span><span class="p">,</span> <span class="mi">0</span><span class="p">])</span>
     <span class="n">A</span><span class="p">,</span> <span class="n">B</span><span class="p">,</span> <span class="n">C</span><span class="p">,</span> <span class="n">D</span> <span class="o">=</span> <span class="n">np</span><span class="o">.</span><span class="n">linalg</span><span class="o">.</span><span class="n">solve</span><span class="p">(</span><span class="n">Am</span><span class="p">,</span> <span class="n">Bm</span><span class="p">)</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-113'>
+  <div class='section' id='section-117'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-113'>#</a>
+        <a class='octothorpe' href='#section-117'>#</a>
       </div>
       
     </div>
     <div class='code'>
       <div class="highlight"><pre>    <span class="k">def</span> <span class="nf">f</span><span class="p">(</span><span class="n">t</span><span class="p">:</span> <span class="nb">float</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">float</span><span class="p">:</span>
         <span class="n">result</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="n">A</span> <span class="o">+</span> <span class="n">B</span><span class="o">*</span><span class="n">t</span> <span class="o">+</span> <span class="n">C</span><span class="o">*</span><span class="n">t</span><span class="o">**</span><span class="mi">2</span> <span class="o">+</span> <span class="n">D</span><span class="o">*</span><span class="n">t</span><span class="o">**</span><span class="mi">3</span>
         <span class="k">return</span> <span class="n">result</span>
 
     <span class="k">return</span> <span class="n">f</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-114'>
+  <div class='section' id='section-118'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-114'>#</a>
+        <a class='octothorpe' href='#section-118'>#</a>
       </div>
       <hr />
     </div>
     <div class='code'>
       <div class="highlight"><pre><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
     <span class="n">pwl0</span> <span class="o">=</span> <span class="n">PWL</span><span class="p">(</span><span class="mf">0.001</span><span class="p">)</span>
     <span class="n">pwl1</span> <span class="o">=</span> <span class="n">PWL</span><span class="p">(</span><span class="mf">0.001</span><span class="p">)</span>
@@ -2227,14 +2296,15 @@
     <span class="n">pwl1</span><span class="o">.</span><span class="n">hold</span><span class="p">(</span><span class="mi">1</span><span class="p">)</span>
 
     <span class="n">pwl0</span><span class="o">.</span><span class="n">sin_transition</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="mi">1</span><span class="p">)</span>
 
     <span class="n">pwl1</span><span class="o">.</span><span class="n">plot_flag</span> <span class="o">=</span> <span class="kc">False</span>
 
     <span class="n">PWL</span><span class="o">.</span><span class="n">plot</span><span class="p">(</span><span class="n">merge</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span>
+    <span class="nb">print</span><span class="p">(</span><span class="n">pwl0</span><span class="p">(</span><span class="mf">1.5</span><span class="p">))</span>
 
 </pre></div>
     </div>
   </div>
   <div class='clearall'></div>
 </div>
 </body>
```

#### html2text {}

```diff
@@ -14,14 +14,15 @@
     * Package_Summary
     * Precision_Related_Exception
     * PWL_Class
           o Dunder Methods
                 # Initializer
                 # String_Representation
                 # Length_Calculator
+                # Object_as_a_Callable
           o Properties
                 # Time_Coordinates
                 # Dependent_Coordinates
                 # Default_Timestep
                 # Name
                 # Verbose_Flag
                 # Plot_Enable_Flag (optional feature: requires matplotlib)
@@ -151,15 +152,16 @@
       positive.
     * name (str, optional) : Name of the PWL object used for verbose output
       printing. Should not be empty. If not set, automatically generates a name
       based on already taken names.
     * verbose (bool, optional) : Flag indicating if verbose output should be
       printed. If not set, defaults to False.
 **** Raises ****
-    * TypeError : Raised if any of the arguments has an invalid type.
+    * TypeError : Raised if either t_step is not a real number, name is not a
+      string or verbose is not a boolean.
     * ValueError : Raised if t_step is not strictly positive or name is empty.
         if name is None:
             i: int = 0
             while f"pwl_{i}" in PWL.__dict_of_objects:
                 i += 1
             name = f"pwl_{i}"
 
@@ -223,14 +225,42 @@
 Length of PWL instances defined as the number of (t, x) points they contain.
 **** Returns ****
     * int
         return len(self._t_list)
 #
 ===============================================================================
 #
+***** Object as a Callable *****
+#
+Dunder method __call__ of PWL class
+    def __call__(self, t: float) -> float:
+#
+**** Summary ****
+Call PWL object as a function by linearly interpolating between it’s time and
+dependent coordinates.
+**** Arguments ****
+    * t (float) : Time instant to evaluate the object at. If negative, returns
+      zero. If bigger than the duration of the object, returns the object’s
+      last dependent coordinate.
+**** Returns ****
+    * float
+**** Raises ****
+    * TypeError : Raised if t is not a real number.
+        if not isinstance(t, Real):
+            raise TypeError(
+                f"Argument 't' should be a real number but has type '{type
+(t).__name__}'.")
+
+        t_list = self._t_list
+        x_list = self._x_list
+
+        return np.interp(x=t, xp=t_list, fp=x_list, left=0)
+#
+===============================================================================
+#
 ***** Time Coordinates *****
 #
 t_list property of PWL class
     @property
     def t_list(self) -> List[float]:
 #
 **** Type ****
@@ -1191,7 +1221,8 @@
     pwl1.hold(1)
 
     pwl0.sin_transition(0, 1)
 
     pwl1.plot_flag = False
 
     PWL.plot(merge=False)
+    print(pwl0(1.5))
```

### Comparing `pwl_writer-1.1.2/docs/pycco.css` & `pwl_writer-1.1.3/docs/pycco.css`

 * *Files identical despite different names*

### Comparing `pwl_writer-1.1.2/pwl_writer/pwl_writer.py` & `pwl_writer-1.1.3/pwl_writer/pwl_writer.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 * [Package Summary](#package-summary)
 * [Precision Related Exception](#precision-related-exception)
 * [PWL Class](#pwl-class)
         * Dunder Methods
             * [Initializer](#initializer)
             * [String Representation](#string-representation)
             * [Length Calculator](#length-calculator)
+            * [Object as a Callable](#object-as-a-callable)
         * Properties
             * [Time Coordinates](#time-coordinates)
             * [Dependent Coordinates](#dependent-coordinates)
             * [Default Timestep](#default-timestep)
             * [Name](#name)
             * [Verbose Flag](#verbose-flag)
             * [Plot Enable Flag](#plot-enable-flag) *(optional feature: requires matplotlib)*
@@ -136,15 +137,15 @@
 
         * `t_step` (`float`) : Default timestep for all operations. Should be strictly positive.
         * `name` (`str`, optional) : Name of the `PWL` object used for verbose output printing. Should not be empty. If not set, automatically generates a name based on already taken names.
         * `verbose` (`bool`, optional) : Flag indicating if verbose output should be printed. If not set, defaults to `False`.
 
         ### Raises
 
-        * `TypeError` : Raised if any of the arguments has an invalid type.
+        * `TypeError` : Raised if either `t_step` is not a real number, `name` is not a string or `verbose` is not a boolean.
         * `ValueError` : Raised if `t_step` is not strictly positive or `name` is empty.
         """
 
         if name is None:
             i: int = 0
             while f"pwl_{i}" in PWL.__dict_of_objects:
                 i += 1
@@ -214,14 +215,47 @@
         * `int`
         """
 
         return len(self._t_list)
 
     # ----
 
+    # == Object as a Callable ==
+
+    def __call__(self, t: float) -> float:
+        """**Dunder method `__call__` of `PWL` class**
+
+        ### Summary
+
+        Call `PWL` object as a function by linearly interpolating between it's time and dependent coordinates.
+
+        ### Arguments
+
+        * `t` (`float`) : Time instant to evaluate the object at. If negative, returns zero. If bigger than the duration of the object, returns the object's last dependent coordinate.
+
+        ### Returns
+
+        * `float`
+
+        ### Raises
+
+        * `TypeError` : Raised if `t` is not a real number.
+        """
+
+        if not isinstance(t, Real):
+            raise TypeError(
+                f"Argument 't' should be a real number but has type '{type(t).__name__}'.")
+
+        t_list = self._t_list
+        x_list = self._x_list
+
+        return np.interp(x=t, xp=t_list, fp=x_list, left=0)
+
+    # ----
+
     # == Time Coordinates ==
 
     @property
     def t_list(self) -> List[float]:
         """**`t_list` property of `PWL` class**
 
         ### Type
@@ -1201,7 +1235,8 @@
     pwl1.hold(1)
 
     pwl0.sin_transition(0, 1)
 
     pwl1.plot_flag = False
 
     PWL.plot(merge=False)
+    print(pwl0(1.5))
```

### Comparing `pwl_writer-1.1.2/pyproject.toml` & `pwl_writer-1.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pwl_writer-1.1.2/PKG-INFO` & `pwl_writer-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwl_writer
-Version: 1.1.2
+Version: 1.1.3
 Summary: Package to generate PWL files incrementally using little 'events' like rectangular pulses and exponential rising or falling edges.
 Author-email: "Victor Sabiá P. Carpes" <victorscarpes@gmail.com>
 Requires-Python: >=3.6.6
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: numpy
 Requires-Dist: pycco ; extra == "doc"
```

