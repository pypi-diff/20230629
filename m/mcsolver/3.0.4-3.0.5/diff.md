# Comparing `tmp/mcsolver-3.0.4.tar.gz` & `tmp/mcsolver-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mcsolver-3.0.4.tar", last modified: Sat Jun 24 17:47:55 2023, max compression
+gzip compressed data, was "dist\mcsolver-3.0.5.tar", last modified: Thu Jun 29 12:39:50 2023, max compression
```

## Comparing `mcsolver-3.0.4.tar` & `mcsolver-3.0.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 17:47:55.032680 mcsolver-3.0.4/
--rw-rw-rw-   0        0        0    35823 2019-12-13 12:05:28.000000 mcsolver-3.0.4/LICENSE
--rw-rw-rw-   0        0        0       72 2021-05-31 04:17:53.000000 mcsolver-3.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     8459 2023-06-24 17:47:55.031682 mcsolver-3.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     6979 2023-05-24 09:15:09.000000 mcsolver-3.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-24 17:47:55.003681 mcsolver-3.0.4/mcsolver/
--rw-rw-rw-   0        0        0    14449 2023-05-23 15:54:54.000000 mcsolver-3.0.4/mcsolver/Lattice.py
--rw-rw-rw-   0        0        0    18263 2023-05-26 06:04:35.000000 mcsolver-3.0.4/mcsolver/WannierKit.py
--rw-rw-rw-   0        0        0      536 2023-05-23 16:29:59.000000 mcsolver-3.0.4/mcsolver/__init__.py
--rw-rw-rw-   0        0        0     8390 2023-05-22 11:26:05.000000 mcsolver-3.0.4/mcsolver/auxiliary.py
--rw-rw-rw-   0        0        0    13828 2023-05-23 14:42:07.000000 mcsolver-3.0.4/mcsolver/fileio.py
--rw-rw-rw-   0        0        0    18944 2023-05-26 06:02:12.000000 mcsolver-3.0.4/mcsolver/guiMain.py
--rw-rw-rw-   0        0        0    14059 2023-06-05 04:40:28.000000 mcsolver-3.0.4/mcsolver/guiPyQt5.py
--rw-rw-rw-   0        0        0     4020 2023-06-05 04:16:17.000000 mcsolver-3.0.4/mcsolver/guiPyQt5_toolbox.py
--rw-rw-rw-   0        0        0    39878 2023-06-24 15:15:05.000000 mcsolver-3.0.4/mcsolver/heisenbergLib.c
--rw-rw-rw-   0        0        0     1185 2023-06-24 17:02:47.000000 mcsolver-3.0.4/mcsolver/input.py
--rw-rw-rw-   0        0        0    11504 2021-01-21 13:51:41.000000 mcsolver-3.0.4/mcsolver/interface2swt.py
--rw-rw-rw-   0        0        0    25649 2023-06-24 17:10:24.000000 mcsolver-3.0.4/mcsolver/isingLib.c
--rw-rw-rw-   0        0        0    36491 2023-06-24 17:13:23.000000 mcsolver-3.0.4/mcsolver/mcMain.py
--rw-rw-rw-   0        0        0     3540 2019-12-14 04:31:12.000000 mcsolver-3.0.4/mcsolver/toolbox.py
--rw-rw-rw-   0        0        0     8720 2023-06-24 16:02:37.000000 mcsolver-3.0.4/mcsolver/win.py
--rw-rw-rw-   0        0        0    35728 2023-06-24 13:34:21.000000 mcsolver-3.0.4/mcsolver/xyLib.c
-drwxrwxrwx   0        0        0        0 2023-06-24 17:47:55.027682 mcsolver-3.0.4/mcsolver.egg-info/
--rw-rw-rw-   0        0        0     8459 2023-06-24 17:47:54.000000 mcsolver-3.0.4/mcsolver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      556 2023-06-24 17:47:54.000000 mcsolver-3.0.4/mcsolver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 17:47:54.000000 mcsolver-3.0.4/mcsolver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-24 17:47:54.000000 mcsolver-3.0.4/mcsolver.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-24 17:47:54.000000 mcsolver-3.0.4/mcsolver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-24 17:47:55.033686 mcsolver-3.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1384 2023-06-24 17:42:44.000000 mcsolver-3.0.4/setup.py
--rw-rw-rw-   0        0        0      974 2023-06-24 17:45:50.000000 mcsolver-3.0.4/setup2.py
-drwxrwxrwx   0        0        0        0 2023-06-24 17:47:55.029688 mcsolver-3.0.4/test/
--rw-rw-rw-   0        0        0      283 2023-05-25 14:57:33.000000 mcsolver-3.0.4/test/test.py
+drwxrwxrwx   0        0        0        0 2023-06-29 12:39:50.270010 mcsolver-3.0.5/
+-rw-rw-rw-   0        0        0    35823 2019-12-13 12:05:28.000000 mcsolver-3.0.5/LICENSE
+-rw-rw-rw-   0        0        0       72 2021-05-31 04:17:53.000000 mcsolver-3.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     8459 2023-06-29 12:39:50.269009 mcsolver-3.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     6979 2023-05-24 09:15:09.000000 mcsolver-3.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 12:39:50.226011 mcsolver-3.0.5/mcsolver/
+-rw-rw-rw-   0        0        0    14449 2023-05-23 15:54:54.000000 mcsolver-3.0.5/mcsolver/Lattice.py
+-rw-rw-rw-   0        0        0    18263 2023-05-26 06:04:35.000000 mcsolver-3.0.5/mcsolver/WannierKit.py
+-rw-rw-rw-   0        0        0      536 2023-05-23 16:29:59.000000 mcsolver-3.0.5/mcsolver/__init__.py
+-rw-rw-rw-   0        0        0     8390 2023-05-22 11:26:05.000000 mcsolver-3.0.5/mcsolver/auxiliary.py
+-rw-rw-rw-   0        0        0    13828 2023-05-23 14:42:07.000000 mcsolver-3.0.5/mcsolver/fileio.py
+-rw-rw-rw-   0        0        0    18944 2023-05-26 06:02:12.000000 mcsolver-3.0.5/mcsolver/guiMain.py
+-rw-rw-rw-   0        0        0    14059 2023-06-05 04:40:28.000000 mcsolver-3.0.5/mcsolver/guiPyQt5.py
+-rw-rw-rw-   0        0        0     4020 2023-06-05 04:16:17.000000 mcsolver-3.0.5/mcsolver/guiPyQt5_toolbox.py
+-rw-rw-rw-   0        0        0    40306 2023-06-29 11:28:12.000000 mcsolver-3.0.5/mcsolver/heisenbergLib.c
+-rw-rw-rw-   0        0        0     1185 2023-06-24 17:02:47.000000 mcsolver-3.0.5/mcsolver/input.py
+-rw-rw-rw-   0        0        0    11504 2021-01-21 13:51:41.000000 mcsolver-3.0.5/mcsolver/interface2swt.py
+-rw-rw-rw-   0        0        0    25937 2023-06-29 12:13:05.000000 mcsolver-3.0.5/mcsolver/isingLib.c
+-rw-rw-rw-   0        0        0    36491 2023-06-24 17:13:23.000000 mcsolver-3.0.5/mcsolver/mcMain.py
+-rw-rw-rw-   0        0        0     3540 2019-12-14 04:31:12.000000 mcsolver-3.0.5/mcsolver/toolbox.py
+-rw-rw-rw-   0        0        0     8720 2023-06-24 16:02:37.000000 mcsolver-3.0.5/mcsolver/win.py
+-rw-rw-rw-   0        0        0    36085 2023-06-29 11:59:05.000000 mcsolver-3.0.5/mcsolver/xyLib.c
+drwxrwxrwx   0        0        0        0 2023-06-29 12:39:50.258013 mcsolver-3.0.5/mcsolver.egg-info/
+-rw-rw-rw-   0        0        0     8459 2023-06-29 12:39:49.000000 mcsolver-3.0.5/mcsolver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      556 2023-06-29 12:39:50.000000 mcsolver-3.0.5/mcsolver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 12:39:49.000000 mcsolver-3.0.5/mcsolver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-29 12:39:49.000000 mcsolver-3.0.5/mcsolver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-29 12:39:49.000000 mcsolver-3.0.5/mcsolver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-29 12:39:50.270010 mcsolver-3.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1384 2023-06-29 12:22:19.000000 mcsolver-3.0.5/setup.py
+-rw-rw-rw-   0        0        0      974 2023-06-29 12:37:50.000000 mcsolver-3.0.5/setup2.py
+drwxrwxrwx   0        0        0        0 2023-06-29 12:39:50.268007 mcsolver-3.0.5/test/
+-rw-rw-rw-   0        0        0      283 2023-05-25 14:57:33.000000 mcsolver-3.0.5/test/test.py
```

### Comparing `mcsolver-3.0.4/LICENSE` & `mcsolver-3.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mcsolver-3.0.4/PKG-INFO` & `mcsolver-3.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: mcsolver
-Version: 3.0.4
+Version: 3.0.5
 Summary: A user friendly program to do Monte Carlo sims for magnetic systems
 Home-page: https://github.com/golddoushi/mcsolver
 Author: Liang Liu
 Author-email: liangliu@main.sdu.edu.cn
 License: UNKNOWN
 Description: # mcsolver
         A user friendly and efficient tool implementing Monte Carlo simulations to estimate Curie/Neel temperature
```

### Comparing `mcsolver-3.0.4/README.md` & `mcsolver-3.0.5/README.md`

 * *Files identical despite different names*

### Comparing `mcsolver-3.0.4/mcsolver/Lattice.py` & `mcsolver-3.0.5/mcsolver/Lattice.py`

 * *Files identical despite different names*

### Comparing `mcsolver-3.0.4/mcsolver/WannierKit.py` & `mcsolver-3.0.5/mcsolver/WannierKit.py`

 * *Files identical despite different names*

### Comparing `mcsolver-3.0.4/mcsolver/__init__.py` & `mcsolver-3.0.5/mcsolver/__init__.py`

 * *Files identical despite different names*

### Comparing `mcsolver-3.0.4/mcsolver/auxiliary.py` & `mcsolver-3.0.5/mcsolver/auxiliary.py`

 * *Files identical despite different names*

### Comparing `mcsolver-3.0.4/mcsolver/fileio.py` & `mcsolver-3.0.5/mcsolver/fileio.py`

 * *Files identical despite different names*

### Comparing `mcsolver-3.0.4/mcsolver/guiMain.py` & `mcsolver-3.0.5/mcsolver/guiMain.py`

 * *Files identical despite different names*

### Comparing `mcsolver-3.0.4/mcsolver/guiPyQt5.py` & `mcsolver-3.0.5/mcsolver/guiPyQt5.py`

 * *Files identical despite different names*

### Comparing `mcsolver-3.0.4/mcsolver/guiPyQt5_toolbox.py` & `mcsolver-3.0.5/mcsolver/guiPyQt5_toolbox.py`

 * *Files identical despite different names*

### Comparing `mcsolver-3.0.4/mcsolver/heisenbergLib.c` & `mcsolver-3.0.5/mcsolver/heisenbergLib.c`

 * *Files 3% similar despite different names*

```diff
@@ -147,16 +147,16 @@
     int nOrbInCluster;
     struct Orb **orb_cluster;
     
     double h;
 }Orb;
 
 //establishLattice(lattice, totOrbs, initSpin, maxNLinking, nlink, linkStrength);
-void establishLattice(Orb *lattice, int totOrbs, double initSpin[totOrbs], double initD[totOrbs][3], double h, double flunc, int maxNLinking, int nlink[totOrbs], double linkStrength[totOrbs][maxNLinking][9],
-                      int totOrb_rnorm, int nOrbInCluster, int rOrb[totOrb_rnorm], int rOrbCluster[totOrb_rnorm][nOrbInCluster]){
+void establishLattice(Orb *lattice, int totOrbs, double initSpin[totOrbs], double initD[totOrbs*3], double h, double flunc, int maxNLinking, int nlink[totOrbs], double linkStrength[totOrbs*maxNLinking*9],
+                      int totOrb_rnorm, int nOrbInCluster, int rOrb[totOrb_rnorm], int rOrbCluster[totOrb_rnorm*nOrbInCluster]){
     //printf("establishing whole lattice with %d orbs and %d linkings for each orb\n",totOrbs,maxNLinking);
     for(int i=0;i<totOrbs;i++){
         //printf("check point-1, entering setting %d",i);
         lattice[i].id=i;
         lattice[i].S=initSpin[i];
         //lattice[i].spin.coor=(double*)malloc(3*sizeof(double));  // allocate spin vector for each orb
         lattice[i].spin.x=initSpin[i];
@@ -167,17 +167,17 @@
         Vec *fluncSpin=generateRandomVec();
         cTimes(fluncSpin, flunc);
         plusEqual(&lattice[i].spin,*fluncSpin);
         normalize(&lattice[i].spin);
         cTimes(&lattice[i].spin,fabs(initSpin[i]));
         free(fluncSpin);
         //printf("%.3f %.3f \n",lattice[i].spin.x, fabs(initSpin[i]));
-        lattice[i].onsiteAnisotropy.x=initD[i][0];
-        lattice[i].onsiteAnisotropy.y=initD[i][1];
-        lattice[i].onsiteAnisotropy.z=initD[i][2];
+        lattice[i].onsiteAnisotropy.x=initD[i*3+0];
+        lattice[i].onsiteAnisotropy.y=initD[i*3+1];
+        lattice[i].onsiteAnisotropy.z=initD[i*3+2];
 
         lattice[i].h=h;
         //printf("orb %d spin: %.3f %.3f %.3f\n",i,lattice[i].spin.coor[0],lattice[i].spin.coor[1],lattice[i].spin.coor[2]);
         lattice[i].transSpin.x=0;  // allocate trans spin vector for each orb
         lattice[i].transSpin.y=0;
         lattice[i].transSpin.z=0;
         lattice[i].perpenSpin.x=0;
@@ -186,55 +186,55 @@
         lattice[i].nlink=nlink[i];
         //printf("check point 1, orb: %d\n",lattice[i].id);
         lattice[i].linkStrength=(Vec9*)malloc(nlink[i]*sizeof(Vec9)); // allocate strength for each linking
         //printf("check point 2, total links:%d\n",nlink[i]);
         for(int j=0;j<nlink[i];j++){
             //lattice[i].linkStrength[j].coor=(double*)malloc(3*sizeof(double));
             //printf("check point 3\n");
-            lattice[i].linkStrength[j].xx=linkStrength[i][j][0];
-            lattice[i].linkStrength[j].yy=linkStrength[i][j][1];
-            lattice[i].linkStrength[j].zz=linkStrength[i][j][2];
-            lattice[i].linkStrength[j].xy=linkStrength[i][j][3];
-            lattice[i].linkStrength[j].xz=linkStrength[i][j][4];
-            lattice[i].linkStrength[j].yz=linkStrength[i][j][5];
-            lattice[i].linkStrength[j].yx=linkStrength[i][j][6];
-            lattice[i].linkStrength[j].zx=linkStrength[i][j][7];
-            lattice[i].linkStrength[j].zy=linkStrength[i][j][8];
+            lattice[i].linkStrength[j].xx=linkStrength[i*maxNLinking*9+j*9+0];
+            lattice[i].linkStrength[j].yy=linkStrength[i*maxNLinking*9+j*9+1];
+            lattice[i].linkStrength[j].zz=linkStrength[i*maxNLinking*9+j*9+2];
+            lattice[i].linkStrength[j].xy=linkStrength[i*maxNLinking*9+j*9+3];
+            lattice[i].linkStrength[j].xz=linkStrength[i*maxNLinking*9+j*9+4];
+            lattice[i].linkStrength[j].yz=linkStrength[i*maxNLinking*9+j*9+5];
+            lattice[i].linkStrength[j].yx=linkStrength[i*maxNLinking*9+j*9+6];
+            lattice[i].linkStrength[j].zx=linkStrength[i*maxNLinking*9+j*9+7];
+            lattice[i].linkStrength[j].zy=linkStrength[i*maxNLinking*9+j*9+8];
             //printf("check point 4, link:%d, strength: %.3f %.3f %.3f\n",j,lattice[i].linkStrength[j].coor[0],lattice[i].linkStrength[j].coor[1],lattice[i].linkStrength[j].coor[2]);
         }
         lattice[i].chosen=0;
     }
     //printf("now checking the orb cluster\n");
     for(int i=0;i<totOrb_rnorm;i++){
         int id=rOrb[i];
         lattice[id].chosen=1;
         lattice[id].nOrbInCluster=nOrbInCluster;
         lattice[id].orb_cluster=(Orb**)malloc(nOrbInCluster*sizeof(Orb*));
         //printf("orb%d is chosen to be the center of cluster, involving %d orbs in total:\n",lattice[id].id,lattice[id].nOrbInCluster);
         for(int iorb=0;iorb<nOrbInCluster;iorb++){
-            lattice[id].orb_cluster[iorb]=lattice+rOrbCluster[i][iorb];
+            lattice[id].orb_cluster[iorb]=lattice+rOrbCluster[i*nOrbInCluster+iorb];
             //printf("    from input id=%d orb%d\n",rOrbCluster[id][iorb],lattice[id].orb_cluster[iorb]->id);
         }
     }
     //printf("orbitals successfully built\n");
 }
 
-void establishLinking(Orb *lattice, int totOrbs, int maxNLinking, int nlink[totOrbs], int linkedOrb[totOrbs][maxNLinking],
-                      int totOrb_rnorm, int rOrb[totOrb_rnorm], int linkedOrb_rnorm[totOrb_rnorm][maxNLinking]){
+void establishLinking(Orb *lattice, int totOrbs, int maxNLinking, int nlink[totOrbs], int linkedOrb[totOrbs*maxNLinking],
+                      int totOrb_rnorm, int rOrb[totOrb_rnorm], int linkedOrb_rnorm[totOrb_rnorm*maxNLinking]){
     for(int iorb=0;iorb<totOrbs;iorb++){
         lattice[iorb].linkedOrb=(Orb**)malloc(nlink[iorb]*sizeof(Orb*));
         for(int ilink=0;ilink<nlink[iorb];ilink++){
-            lattice[iorb].linkedOrb[ilink]=lattice+linkedOrb[iorb][ilink];
+            lattice[iorb].linkedOrb[ilink]=lattice+linkedOrb[iorb*maxNLinking+ilink];
         }
     }
     for(int i=0;i<totOrb_rnorm;i++){
         int iorb=rOrb[i];
         lattice[iorb].linkedOrb_rnorm=(Orb**)malloc(nlink[iorb]*sizeof(Orb*));
         for(int ilink=0;ilink<nlink[iorb];ilink++){
-            lattice[iorb].linkedOrb_rnorm[ilink]=lattice+linkedOrb_rnorm[i][ilink];
+            lattice[iorb].linkedOrb_rnorm[ilink]=lattice+linkedOrb_rnorm[i*maxNLinking+ilink];
         }
     }
 }
 
 double getCorrEnergy(Orb *source){
     //printf("start calc corr. energy\n");
     double corr=0;
@@ -518,31 +518,31 @@
     int nsweep=(int)PyLong_AsLong(py_nsweep);
     int maxNLinking=(int)PyLong_AsLong(py_maxNLinking);
     int ninterval=(int)PyLong_AsLong(py_ninterval);
     int spinFrame=(int)PyLong_AsLong(py_spinFrame);
     int ignoreNonDiagonalJ=(int)PyLong_AsLong(py_ignoreNonDiagonalJ);
 
     int totOrbs=(int)PyTuple_Size(py_initSpin);
-    double initSpin[totOrbs];
+    double *initSpin=(double*)malloc(totOrbs*sizeof(double));
     for(int iorb=0;iorb<totOrbs;iorb++)initSpin[iorb]=PyFloat_AsDouble(PyTuple_GetItem(py_initSpin,iorb));
 
-    double initD[totOrbs][3];
+    double *initD=(double*)malloc(totOrbs*3*sizeof(double));
     for(int iorb=0;iorb<totOrbs;iorb++)for(int idir=0;idir<3;idir++)
-        initD[iorb][idir]=PyFloat_AsDouble(PyTuple_GetItem(py_initD,iorb*3+idir));
+        initD[iorb*3+idir]=PyFloat_AsDouble(PyTuple_GetItem(py_initD,iorb*3+idir));
     
     
-    int nlink[totOrbs];
-    double linkStrength[totOrbs][maxNLinking][9];
-    int linkedOrb[totOrbs][maxNLinking];
+    int *nlink=(int*)malloc(totOrbs*sizeof(int));
+    double *linkStrength=(double*)malloc(totOrbs*maxNLinking*9*sizeof(double));
+    int *linkedOrb=(int*)malloc(totOrbs*maxNLinking*sizeof(int));
     for(int iorb=0;iorb<totOrbs;iorb++){
         nlink[iorb]=(int)PyLong_AsLong(PyTuple_GetItem(py_nlink,iorb));
         for(int ilink=0;ilink<maxNLinking;ilink++){
-            linkedOrb[iorb][ilink]=(int)PyLong_AsLong(PyTuple_GetItem(py_linkedOrb,iorb*maxNLinking+ilink));
+            linkedOrb[iorb*maxNLinking+ilink]=(int)PyLong_AsLong(PyTuple_GetItem(py_linkedOrb,iorb*maxNLinking+ilink));
             for(int icomp=0;icomp<9;icomp++)
-            linkStrength[iorb][ilink][icomp]=PyFloat_AsDouble(PyTuple_GetItem(py_linkStrength,iorb*maxNLinking*9+ilink*9+icomp));
+            linkStrength[iorb*maxNLinking*9+ilink*9+icomp]=PyFloat_AsDouble(PyTuple_GetItem(py_linkStrength,iorb*maxNLinking*9+ilink*9+icomp));
         }
     }
     //printf("totOrbs=%d s0=%f D0x=%f nther=%d nst=%d tau=%d maxLink=%d link0=%d J0x=%f\n",totOrbs,initSpin[0],initD[0][0],nthermal,nsweep,ninterval,maxNLinking,nlink[0],linkStrength[0][0][0]);
     //printf("spinFrame: %d only diagonal: %d\n",spinFrame,ignoreNonDiagonalJ);
     //for(int iorb=0;iorb<nlink[0];iorb++)printf("orb0-orb%d\n",linkedOrb[0][iorb]);
     
     int nLocalCircuits=(int)PyTuple_Size(py_localCircuits)/3;
@@ -570,23 +570,23 @@
     double flunc = PyFloat_AsDouble(py_flunc);
     double h = PyFloat_AsDouble(py_h);
     //printf("flunc=%f h=%f\n",flunc,h);
 
     int totOrb_rnorm=(int)PyTuple_Size(py_rOrb);
     int nOrbInCluster=(int)PyTuple_Size(py_rOrbCluster)/totOrb_rnorm;
     //printf("totOrb renorm=%d grain size=%d\n",totOrb_rnorm,nOrbInCluster);
-    int rOrb[totOrb_rnorm];
-    int rOrbCluster[totOrb_rnorm][nOrbInCluster];
-    int linkedOrb_rnorm[totOrb_rnorm][maxNLinking];
+    int *rOrb=(int*)malloc(totOrb_rnorm*sizeof(int));
+    int *rOrbCluster=(int*)malloc(totOrb_rnorm*nOrbInCluster*sizeof(int));
+    int *linkedOrb_rnorm=(int*)malloc(totOrb_rnorm*maxNLinking*sizeof(int));
     for(int iorb=0;iorb<totOrb_rnorm;iorb++){
         rOrb[iorb]=(int)PyLong_AsLong(PyTuple_GetItem(py_rOrb,iorb));
         for(int iorb_cluster=0;iorb_cluster<nOrbInCluster;iorb_cluster++)
-            rOrbCluster[iorb][iorb_cluster]=(int)PyLong_AsLong(PyTuple_GetItem(py_rOrbCluster,iorb*nOrbInCluster+iorb_cluster));
+            rOrbCluster[iorb*nOrbInCluster+iorb_cluster]=(int)PyLong_AsLong(PyTuple_GetItem(py_rOrbCluster,iorb*nOrbInCluster+iorb_cluster));
         for(int ilink=0;ilink<maxNLinking;ilink++)
-            linkedOrb_rnorm[iorb][ilink]=(int)PyLong_AsLong(PyTuple_GetItem(py_linkedOrb_rnorm,iorb*maxNLinking+ilink));
+            linkedOrb_rnorm[iorb*maxNLinking+ilink]=(int)PyLong_AsLong(PyTuple_GetItem(py_linkedOrb_rnorm,iorb*maxNLinking+ilink));
     }    
     
     // set algorithm
     p_mcUpdate=localUpdate;
     if (algorithm==1) p_mcUpdate=blockUpdate;
 
     // set diagonal dot version
```

### Comparing `mcsolver-3.0.4/mcsolver/input.py` & `mcsolver-3.0.5/mcsolver/input.py`

 * *Files identical despite different names*

### Comparing `mcsolver-3.0.4/mcsolver/interface2swt.py` & `mcsolver-3.0.5/mcsolver/interface2swt.py`

 * *Files identical despite different names*

### Comparing `mcsolver-3.0.4/mcsolver/isingLib.c` & `mcsolver-3.0.5/mcsolver/isingLib.c`

 * *Files 10% similar despite different names*

```diff
@@ -15,21 +15,21 @@
 
     int chosen;
     struct Orb **linkedOrb_rnorm;
     int nOrbInCluster;
     struct Orb **orb_cluster;
 }Orb;
 
-void establishLattice(Orb *lattice, int totOrbs, double initSpin[totOrbs], int maxNLinking, int nlink[maxNLinking], double linkStrength[totOrbs][maxNLinking],
-                   int totOrb_rnorm, int nOrbInCluster, int rOrb[totOrb_rnorm], int rOrbCluster[totOrb_rnorm][nOrbInCluster]){
+void establishLattice(Orb *lattice, int totOrbs, double initSpin[totOrbs], int maxNLinking, int nlink[maxNLinking], double linkStrength[totOrbs*maxNLinking],
+                   int totOrb_rnorm, int nOrbInCluster, int rOrb[totOrb_rnorm], int rOrbCluster[totOrb_rnorm*nOrbInCluster]){
     for(int i=0;i<totOrbs;i++){
         lattice[i].id=i;
         lattice[i].spin=initSpin[i];
         lattice[i].nlink=nlink[i];
-        lattice[i].linkStrength=linkStrength[i];
+        lattice[i].linkStrength=linkStrength+i;
         lattice[i].chosen=0;
     }
     //printf("verify lattice\n");
     //for(int i=0;i<totOrbs;i++){
     //    printf("orb%d spin: %.3f nlink: %d\n",lattice[i].id,lattice[i].spin,lattice[i].nlink);
     //    for(int j=0;j<nlink[i];j++) printf(" coupling%d: %.6f\n",j,lattice[i].linkStrength[j]);
     //}
@@ -37,80 +37,80 @@
     for(int i=0;i<totOrb_rnorm;i++){
         int id=rOrb[i];
         lattice[id].chosen=1;
         lattice[id].nOrbInCluster=nOrbInCluster;
         lattice[id].orb_cluster=(Orb**)malloc(nOrbInCluster*sizeof(Orb*));
         //printf("orb%d is chosen to be the center of cluster, involving %d orbs in total:\n",lattice[id].id,lattice[id].nOrbInCluster);
         for(int iorb=0;iorb<nOrbInCluster;iorb++){
-            lattice[id].orb_cluster[iorb]=lattice+rOrbCluster[i][iorb];
+            lattice[id].orb_cluster[iorb]=lattice+rOrbCluster[i*nOrbInCluster+iorb];
             //printf("    from input id=%d orb%d\n",rOrbCluster[id][iorb],lattice[id].orb_cluster[iorb]->id);
         }
     }
 }
 
-void establishLinking(Orb *lattice, int totOrbs, int maxNLinking, int nlink[maxNLinking], int linkedOrb[totOrbs][maxNLinking],
-                   int totOrb_rnorm, int rOrb[totOrb_rnorm], int linkedOrb_rnorm[totOrb_rnorm][maxNLinking]){
+void establishLinking(Orb *lattice, int totOrbs, int maxNLinking, int nlink[maxNLinking], int linkedOrb[totOrbs*maxNLinking],
+                   int totOrb_rnorm, int rOrb[totOrb_rnorm], int linkedOrb_rnorm[totOrb_rnorm*maxNLinking]){
     for(int iorb=0;iorb<totOrbs;iorb++){
         lattice[iorb].linkedOrb=(Orb**)malloc(nlink[iorb]*sizeof(Orb*));
         for(int ilink=0;ilink<nlink[iorb];ilink++){
-            lattice[iorb].linkedOrb[ilink]=lattice+linkedOrb[iorb][ilink];
+            lattice[iorb].linkedOrb[ilink]=lattice+linkedOrb[iorb*maxNLinking+ilink];
         }
     }
     //printf("verify linking\n");
     //for(int iorb=0;iorb<totOrbs;iorb++){
     //    for(int ilink=0;ilink<nlink[iorb];ilink++){
     //        lattice[iorb].linkedOrb[ilink]=lattice+linkedOrb[iorb][ilink];
     //        printf("orb%d ~ orb%d strength: %.6f\n",lattice[iorb].id,lattice[iorb].linkedOrb[ilink]->id,lattice[iorb].linkStrength[ilink]);
     //    }
     //}
     for(int i=0;i<totOrb_rnorm;i++){
         int iorb=rOrb[i];
         lattice[iorb].linkedOrb_rnorm=(Orb**)malloc(nlink[iorb]*sizeof(Orb*));
         for(int ilink=0;ilink<nlink[iorb];ilink++){
-            lattice[iorb].linkedOrb_rnorm[ilink]=lattice+linkedOrb_rnorm[i][ilink];
+            lattice[iorb].linkedOrb_rnorm[ilink]=lattice+linkedOrb_rnorm[i*maxNLinking+ilink];
         }
     }
 }
 
-void establishLatticeWithGhost(Orb *lattice, int totOrbs, double initSpin[totOrbs], int maxNLinking, int nlink[maxNLinking], double linkStrength[totOrbs][maxNLinking], double h,
+void establishLatticeWithGhost(Orb *lattice, int totOrbs, double initSpin[totOrbs], int maxNLinking, int nlink[maxNLinking], double linkStrength[totOrbs*maxNLinking], double h,
                    int totOrb_rnorm, int rOrb[totOrb_rnorm]){
     for(int i=0;i<totOrbs-1;i++){
         lattice[i].id=i;
         lattice[i].spin=initSpin[i];
         lattice[i].nlink=nlink[i]+1;
         lattice[i].linkStrength=(double*)malloc(lattice[i].nlink*sizeof(double));
-        for(int j=0;j<lattice[i].nlink-1;j++)lattice[i].linkStrength[j]=linkStrength[i][j];
+        for(int j=0;j<lattice[i].nlink-1;j++)lattice[i].linkStrength[j]=linkStrength[i*maxNLinking+j];
         lattice[i].linkStrength[lattice[i].nlink-1]=1;
         lattice[i].chosen=0;
     }
     for(int i=0;i<totOrb_rnorm;i++){
         lattice[rOrb[i]].chosen=1;
     }
     lattice[totOrbs-1].id=totOrbs-1;
     lattice[totOrbs-1].spin=h;
     lattice[totOrbs-1].nlink=totOrbs-1;
     lattice[totOrbs-1].linkStrength=(double*)malloc((totOrbs-1)*sizeof(double));
     for(int i=0;i<totOrbs-1;i++) lattice[totOrbs-1].linkStrength[i]=1;
 }
 
-void establishLinkingWithGhost(Orb *lattice, int totOrbs, int maxNLinking, int nlink[maxNLinking], int linkedOrb[totOrbs][maxNLinking],
-                   int totOrb_rnorm, int rOrb[totOrb_rnorm], int linkedOrb_rnorm[totOrb_rnorm][maxNLinking]){
+void establishLinkingWithGhost(Orb *lattice, int totOrbs, int maxNLinking, int nlink[maxNLinking], int linkedOrb[totOrbs*maxNLinking],
+                   int totOrb_rnorm, int rOrb[totOrb_rnorm], int linkedOrb_rnorm[totOrb_rnorm*maxNLinking]){
     for(int iorb=0;iorb<totOrbs-1;iorb++){
         lattice[iorb].linkedOrb=(Orb**)malloc(lattice[iorb].nlink*sizeof(Orb*));
         for(int ilink=0;ilink<lattice[iorb].nlink-1;ilink++){
-            lattice[iorb].linkedOrb[ilink]=lattice+linkedOrb[iorb][ilink];
+            lattice[iorb].linkedOrb[ilink]=lattice+linkedOrb[iorb*maxNLinking+ilink];
         }
         lattice[iorb].linkedOrb[lattice[iorb].nlink-1]=lattice+totOrbs-1;
     }
     for(int i=0;i<totOrb_rnorm;i++){
         int iorb=rOrb[i];
         //printf("step %d, In renormalized lattice, orb%d is involved by %d bonds\n",i,lattice[iorb].id, nlink[iorb]);
         lattice[iorb].linkedOrb_rnorm=(Orb**)malloc(nlink[iorb]*sizeof(Orb*));
         for(int ilink=0;ilink<nlink[iorb];ilink++){
-            lattice[iorb].linkedOrb_rnorm[ilink]=lattice+linkedOrb_rnorm[i][ilink];
+            lattice[iorb].linkedOrb_rnorm[ilink]=lattice+linkedOrb_rnorm[i*maxNLinking+ilink];
             //printf("%d\n",linkedOrb_rnorm[i][ilink]);
             //printf("orb%d with strength %.3f\n",lattice[iorb].linkedOrb_rnorm[ilink]->id,lattice[iorb].linkStrength[ilink]);
         }
     }
     lattice[totOrbs-1].linkedOrb=(Orb**)malloc((totOrbs-1)*sizeof(Orb*));
     for(int i=0;i<totOrbs-1;i++) lattice[totOrbs-1].linkedOrb[i]=lattice+i;
 }
@@ -233,17 +233,17 @@
         *p_totSpin+=(lattice[seedID].spin*2);
         *p_energy-=corr;
     }
     //printf("local update finished\n");
 }
  
 PyObject * blockUpdateMC(int totOrbs, double initSpin[totOrbs], int nthermal, int nsweep, 
-                   int maxNLinking, int nlink[totOrbs], double linkStrength[totOrbs][maxNLinking], int linkedOrb[totOrbs][maxNLinking],
+                   int maxNLinking, int nlink[totOrbs], double linkStrength[totOrbs*maxNLinking], int linkedOrb[totOrbs*maxNLinking],
                    int ninterval, int nLat, int corrOrbPair[nLat][2], double h,
-                   int renormOn, int totOrb_rnorm, int nOrbInCluster, int rOrb[totOrb_rnorm], int rOrbCluster[totOrb_rnorm][nOrbInCluster], int linkedOrb_rnorm[totOrb_rnorm][maxNLinking],
+                   int renormOn, int totOrb_rnorm, int nOrbInCluster, int rOrb[totOrb_rnorm], int rOrbCluster[totOrb_rnorm*nOrbInCluster], int linkedOrb_rnorm[totOrb_rnorm*maxNLinking],
                    int spinFrame){
     //printf("hello block algorithm!\n");
     // initialize lattice including one ghost spin
     //totOrbs+=1;
     Orb lattice[totOrbs];
     //establishLatticeWithGhost(lattice, totOrbs, initSpin, maxNLinking, nlink, linkStrength, h, totOrb_rnorm, rOrb);
     //establishLinkingWithGhost(lattice, totOrbs, maxNLinking, nlink, linkedOrb, totOrb_rnorm, rOrb, linkedOrb_rnorm);
@@ -360,17 +360,17 @@
     PyTuple_SetItem(Data, 8, PyFloat_FromDouble(U4));
     PyTuple_SetItem(Data, 9, PyFloat_FromDouble(spin_tot/nsweep/nLat));
     PyTuple_SetItem(Data, 10, spinFrameData);
     return Data;
 }
 
 PyObject * localUpdateMC(int totOrbs, double initSpin[totOrbs], int nthermal, int nsweep, 
-                   int maxNLinking, int nlink[totOrbs], double linkStrength[totOrbs][maxNLinking], int linkedOrb[totOrbs][maxNLinking],
+                   int maxNLinking, int nlink[totOrbs], double linkStrength[totOrbs*maxNLinking], int linkedOrb[totOrbs*maxNLinking],
                    int ninterval, int nLat, int corrOrbPair[nLat][2], double h,
-                   int renormOn, int totOrb_rnorm, int nOrbInCluster, int rOrb[totOrb_rnorm], int rOrbCluster[totOrb_rnorm][nOrbInCluster], int linkedOrb_rnorm[totOrb_rnorm][maxNLinking],
+                   int renormOn, int totOrb_rnorm, int nOrbInCluster, int rOrb[totOrb_rnorm], int rOrbCluster[totOrb_rnorm*nOrbInCluster], int linkedOrb_rnorm[totOrb_rnorm*maxNLinking],
                    int spinFrame){
     // initialize lattice 
     Orb lattice[totOrbs];
     establishLattice(lattice, totOrbs, initSpin, maxNLinking, nlink, linkStrength, totOrb_rnorm, nOrbInCluster, rOrb, rOrbCluster);
     establishLinking(lattice, totOrbs, maxNLinking, nlink, linkedOrb, totOrb_rnorm, rOrb, linkedOrb_rnorm);
 
     // initialize measurement
@@ -512,25 +512,25 @@
     int nthermal=(int)PyLong_AsLong(py_nthermal);
     int nsweep=(int)PyLong_AsLong(py_nsweep);
     int maxNLinking=(int)PyLong_AsLong(py_maxNLinking);
     int ninterval=(int)PyLong_AsLong(py_ninterval);
     int spinFrame=(int)PyLong_AsLong(py_spinFrame);
 
     int totOrbs=(int)PyTuple_Size(py_initSpin);
-    double initSpin[totOrbs];
+    double *initSpin=(double*)malloc(totOrbs*sizeof(double));
     for(int iorb=0;iorb<totOrbs;iorb++)initSpin[iorb]=PyFloat_AsDouble(PyTuple_GetItem(py_initSpin,iorb));
     
-    int nlink[totOrbs];
-    double linkStrength[totOrbs][maxNLinking];
-    int linkedOrb[totOrbs][maxNLinking];
+    int *nlink=(int*)malloc(totOrbs*sizeof(int));
+    double *linkStrength=(double*)malloc(totOrbs*maxNLinking*sizeof(double));
+    int *linkedOrb=(int*)malloc(totOrbs*maxNLinking*sizeof(int));
     for(int iorb=0;iorb<totOrbs;iorb++){
         nlink[iorb]=(int)PyLong_AsLong(PyTuple_GetItem(py_nlink,iorb));
         for(int ilink=0;ilink<maxNLinking;ilink++){
-            linkedOrb[iorb][ilink]=(int)PyLong_AsLong(PyTuple_GetItem(py_linkedOrb,iorb*maxNLinking+ilink));
-            linkStrength[iorb][ilink]=PyFloat_AsDouble(PyTuple_GetItem(py_linkStrength,iorb*maxNLinking+ilink));
+            linkedOrb[iorb*maxNLinking+ilink]=(int)PyLong_AsLong(PyTuple_GetItem(py_linkedOrb,iorb*maxNLinking+ilink));
+            linkStrength[iorb*maxNLinking+ilink]=PyFloat_AsDouble(PyTuple_GetItem(py_linkStrength,iorb*maxNLinking+ilink));
         }
     }
     //printf("totOrbs=%d s0=%f nther=%d nst=%d tau=%d maxLink=%d link0=%d J=%f\n",totOrbs,initSpin[0],nthermal,nsweep,ninterval,maxNLinking,nlink[0],linkStrength[0][0]);
     //printf("spinFrame: %d\n",spinFrame);
     //for(int iorb=0;iorb<nlink[0];iorb++)printf("orb0-orb%d\n",linkedOrb[0][iorb]);
 
     int nLat=(int)PyTuple_Size(py_corrOrbPair)/2;
@@ -543,23 +543,23 @@
     
     double h = PyFloat_AsDouble(py_h);
     //printf("flunc=%f h=%f\n",flunc,h);
 
     int totOrb_rnorm=(int)PyTuple_Size(py_rOrb);
     int nOrbInCluster=(int)PyTuple_Size(py_rOrbCluster)/totOrb_rnorm;
     //printf("totOrb renorm=%d grain size=%d\n",totOrb_rnorm,nOrbInCluster);
-    int rOrb[totOrb_rnorm];
-    int rOrbCluster[totOrb_rnorm][nOrbInCluster];
-    int linkedOrb_rnorm[totOrb_rnorm][maxNLinking];
+    int *rOrb=(int*)malloc(totOrb_rnorm*sizeof(int));
+    int *rOrbCluster=(int*)malloc(totOrb_rnorm*nOrbInCluster*sizeof(int));
+    int *linkedOrb_rnorm=(int*)malloc(totOrb_rnorm*maxNLinking*sizeof(int));
     for(int iorb=0;iorb<totOrb_rnorm;iorb++){
         rOrb[iorb]=(int)PyLong_AsLong(PyTuple_GetItem(py_rOrb,iorb));
         for(int iorb_cluster=0;iorb_cluster<nOrbInCluster;iorb_cluster++)
-            rOrbCluster[iorb][iorb_cluster]=(int)PyLong_AsLong(PyTuple_GetItem(py_rOrbCluster,iorb*nOrbInCluster+iorb_cluster));
+            rOrbCluster[iorb*nOrbInCluster+iorb_cluster]=(int)PyLong_AsLong(PyTuple_GetItem(py_rOrbCluster,iorb*nOrbInCluster+iorb_cluster));
         for(int ilink=0;ilink<maxNLinking;ilink++)
-            linkedOrb_rnorm[iorb][ilink]=(int)PyLong_AsLong(PyTuple_GetItem(py_linkedOrb_rnorm,iorb*maxNLinking+ilink));
+            linkedOrb_rnorm[iorb*maxNLinking+ilink]=(int)PyLong_AsLong(PyTuple_GetItem(py_linkedOrb_rnorm,iorb*maxNLinking+ilink));
     }
 
     if(algorithm==0){
         return localUpdateMC(totOrbs, initSpin, nthermal, nsweep, 
                    maxNLinking, nlink, linkStrength, linkedOrb,
                    ninterval, nLat, corrOrbPair, h,
                    1, totOrb_rnorm, nOrbInCluster, rOrb, rOrbCluster, linkedOrb_rnorm,
```

### Comparing `mcsolver-3.0.4/mcsolver/mcMain.py` & `mcsolver-3.0.5/mcsolver/mcMain.py`

 * *Files identical despite different names*

### Comparing `mcsolver-3.0.4/mcsolver/toolbox.py` & `mcsolver-3.0.5/mcsolver/toolbox.py`

 * *Files identical despite different names*

### Comparing `mcsolver-3.0.4/mcsolver/win.py` & `mcsolver-3.0.5/mcsolver/win.py`

 * *Files identical despite different names*

### Comparing `mcsolver-3.0.4/mcsolver/xyLib.c` & `mcsolver-3.0.5/mcsolver/xyLib.c`

 * *Files 5% similar despite different names*

```diff
@@ -109,16 +109,16 @@
     struct Orb **orb_cluster;
 
     double h;
     
 }Orb;
 
 //establishLattice(lattice, totOrbs, initSpin, maxNLinking, nlink, linkStrength);
-void establishLattice(Orb *lattice, int totOrbs, double initSpin[totOrbs], double initD[totOrbs][3], double flunc, int maxNLinking, int nlink[totOrbs], double linkStrength[totOrbs][maxNLinking][9], double h,
-                      int totOrb_rnorm, int nOrbInCluster, int rOrb[totOrb_rnorm], int rOrbCluster[totOrb_rnorm][nOrbInCluster]){
+void establishLattice(Orb *lattice, int totOrbs, double initSpin[totOrbs], double initD[totOrbs*3], double flunc, int maxNLinking, int nlink[totOrbs], double linkStrength[totOrbs*maxNLinking*9], double h,
+                      int totOrb_rnorm, int nOrbInCluster, int rOrb[totOrb_rnorm], int rOrbCluster[totOrb_rnorm*nOrbInCluster]){
     //printf("establishing whole lattice with %d orbs and %d linkings for each orb\n",totOrbs,maxNLinking);
     int i;
     for(i=0;i<totOrbs;i++){
         //printf("check point-1, entering setting %d",i);
         lattice[i].id=i;
         lattice[i].S=initSpin[i];
         lattice[i].spin.x=initSpin[i];
@@ -127,66 +127,66 @@
         Vec *fluncSpin=generateRandomVec();
         cTimes(fluncSpin, flunc);
         plusEqual(&lattice[i].spin,*fluncSpin);
         normalize(&lattice[i].spin);
         cTimes(&lattice[i].spin,fabs(initSpin[i]));
         free(fluncSpin);
 
-        lattice[i].onsiteAnisotropy.x=initD[i][0];
-        lattice[i].onsiteAnisotropy.y=initD[i][1];
+        lattice[i].onsiteAnisotropy.x=initD[i*3+0];
+        lattice[i].onsiteAnisotropy.y=initD[i*3+1];
 
         lattice[i].h=h;
         //printf("orb %d spin: %.3f %.3f %.3f\n",i,lattice[i].spin.coor[0],lattice[i].spin.coor[1],lattice[i].spin.coor[2]);
         lattice[i].transSpin.x=0;  // allocate trans spin vector for each orb
         lattice[i].transSpin.y=0;
         lattice[i].perpenSpin.x=0;
         lattice[i].perpenSpin.y=0;
         lattice[i].nlink=nlink[i];
         //printf("check point 1, orb: %d\n",lattice[i].id);
         lattice[i].linkStrength=(Vec4*)malloc(lattice[i].nlink*sizeof(Vec4)); // allocate strength for each linking
         //printf("check point 2, total links:%d\n",nlink[i]);
         for(int j=0;j<nlink[i];j++){
             //lattice[i].linkStrength[j].coor=(double*)malloc(3*sizeof(double));
             //printf("check point 3\n");
-            lattice[i].linkStrength[j].xx=linkStrength[i][j][0];
-            lattice[i].linkStrength[j].yy=linkStrength[i][j][1];
-            lattice[i].linkStrength[j].xy=linkStrength[i][j][3];
-            lattice[i].linkStrength[j].yx=linkStrength[i][j][6];
+            lattice[i].linkStrength[j].xx=linkStrength[i*maxNLinking*9+j*9+0];
+            lattice[i].linkStrength[j].yy=linkStrength[i*maxNLinking*9+j*9+1];
+            lattice[i].linkStrength[j].xy=linkStrength[i*maxNLinking*9+j*9+3];
+            lattice[i].linkStrength[j].yx=linkStrength[i*maxNLinking*9+j*9+6];
             //printf("check point 4, link:%d, strength: %.3f %.3f\n",j,lattice[i].linkStrength[j].x,lattice[i].linkStrength[j].y);
         }
         lattice[i].chosen=0;
     }
     //printf("now checking the orb cluster\n");
     for(int i=0;i<totOrb_rnorm;i++){
         int id=rOrb[i];
         lattice[id].chosen=1;
         lattice[id].nOrbInCluster=nOrbInCluster;
         lattice[id].orb_cluster=(Orb**)malloc(nOrbInCluster*sizeof(Orb*));
         //printf("orb%d is chosen to be the center of cluster, involving %d orbs in total:\n",lattice[id].id,lattice[id].nOrbInCluster);
         for(int iorb=0;iorb<nOrbInCluster;iorb++){
-            lattice[id].orb_cluster[iorb]=lattice+rOrbCluster[i][iorb];
+            lattice[id].orb_cluster[iorb]=lattice+rOrbCluster[i*nOrbInCluster+iorb];
             //printf("    from input id=%d orb%d\n",rOrbCluster[id][iorb],lattice[id].orb_cluster[iorb]->id);
         }
     }
     //printf("orbitals successfully built\n");
 }
 
-void establishLinking(Orb *lattice, int totOrbs, int maxNLinking, int nlink[totOrbs], int linkedOrb[totOrbs][maxNLinking],
-                      int totOrb_rnorm, int rOrb[totOrb_rnorm], int linkedOrb_rnorm[totOrb_rnorm][maxNLinking]){
+void establishLinking(Orb *lattice, int totOrbs, int maxNLinking, int nlink[totOrbs], int linkedOrb[totOrbs*maxNLinking],
+                      int totOrb_rnorm, int rOrb[totOrb_rnorm], int linkedOrb_rnorm[totOrb_rnorm*maxNLinking]){
     for(int iorb=0;iorb<totOrbs;iorb++){
         lattice[iorb].linkedOrb=(Orb**)malloc(lattice[iorb].nlink*sizeof(Orb*));
         for(int ilink=0;ilink<nlink[iorb];ilink++){
-            lattice[iorb].linkedOrb[ilink]=lattice+linkedOrb[iorb][ilink];
+            lattice[iorb].linkedOrb[ilink]=lattice+linkedOrb[iorb*maxNLinking+ilink];
         }
     }
     for(int i=0;i<totOrb_rnorm;i++){
         int iorb=rOrb[i];
         lattice[iorb].linkedOrb_rnorm=(Orb**)malloc(nlink[iorb]*sizeof(Orb*));
         for(int ilink=0;ilink<nlink[iorb];ilink++){
-            lattice[iorb].linkedOrb_rnorm[ilink]=lattice+linkedOrb_rnorm[i][ilink];
+            lattice[iorb].linkedOrb_rnorm[ilink]=lattice+linkedOrb_rnorm[i*maxNLinking+ilink];
         }
     }
     //printf("bonds successfully built\n");
 }
 
 double getCorrEnergy(Orb *source){
     double corr=0;
@@ -457,31 +457,31 @@
     int nsweep=(int)PyLong_AsLong(py_nsweep);
     int maxNLinking=(int)PyLong_AsLong(py_maxNLinking);
     int ninterval=(int)PyLong_AsLong(py_ninterval);
     int spinFrame=(int)PyLong_AsLong(py_spinFrame);
     int ignoreNonDiagonalJ=(int)PyLong_AsLong(py_ignoreNonDiagonalJ);
 
     int totOrbs=(int)PyTuple_Size(py_initSpin);
-    double initSpin[totOrbs];
+    double *initSpin=(double*)malloc(totOrbs*sizeof(double));
     for(int iorb=0;iorb<totOrbs;iorb++)initSpin[iorb]=PyFloat_AsDouble(PyTuple_GetItem(py_initSpin,iorb));
 
-    double initD[totOrbs][3];
+    double *initD=(double*)malloc(totOrbs*3*sizeof(double));
     for(int iorb=0;iorb<totOrbs;iorb++)for(int idir=0;idir<3;idir++)
-        initD[iorb][idir]=PyFloat_AsDouble(PyTuple_GetItem(py_initD,iorb*3+idir));
+        initD[iorb*3+idir]=PyFloat_AsDouble(PyTuple_GetItem(py_initD,iorb*3+idir));
     
     
-    int nlink[totOrbs];
-    double linkStrength[totOrbs][maxNLinking][9];
-    int linkedOrb[totOrbs][maxNLinking];
+    int *nlink=(int*)malloc(totOrbs*sizeof(int));
+    double *linkStrength=(double*)malloc(totOrbs*maxNLinking*9*sizeof(double));
+    int *linkedOrb=(int*)malloc(totOrbs*maxNLinking*sizeof(int));
     for(int iorb=0;iorb<totOrbs;iorb++){
         nlink[iorb]=(int)PyLong_AsLong(PyTuple_GetItem(py_nlink,iorb));
         for(int ilink=0;ilink<maxNLinking;ilink++){
-            linkedOrb[iorb][ilink]=(int)PyLong_AsLong(PyTuple_GetItem(py_linkedOrb,iorb*maxNLinking+ilink));
+            linkedOrb[iorb*maxNLinking+ilink]=(int)PyLong_AsLong(PyTuple_GetItem(py_linkedOrb,iorb*maxNLinking+ilink));
             for(int icomp=0;icomp<9;icomp++)
-            linkStrength[iorb][ilink][icomp]=PyFloat_AsDouble(PyTuple_GetItem(py_linkStrength,iorb*maxNLinking*9+ilink*9+icomp));
+            linkStrength[iorb*maxNLinking*9+ilink*9+icomp]=PyFloat_AsDouble(PyTuple_GetItem(py_linkStrength,iorb*maxNLinking*9+ilink*9+icomp));
         }
     }
     //printf("totOrbs=%d s0=%f D0x=%f nther=%d nst=%d tau=%d maxLink=%d link0=%d J0x=%f\n",totOrbs,initSpin[0],initD[0][0],nthermal,nsweep,ninterval,maxNLinking,nlink[0],linkStrength[0][0][0]);
     //printf("spinFrame: %d only diagonal: %d\n",spinFrame,ignoreNonDiagonalJ);
     //for(int iorb=0;iorb<nlink[0];iorb++)printf("orb0-orb%d\n",linkedOrb[0][iorb]);
     
     int nLocalCircuits=(int)PyTuple_Size(py_localCircuits)/3;
@@ -509,23 +509,23 @@
     double flunc = PyFloat_AsDouble(py_flunc);
     double h = PyFloat_AsDouble(py_h);
     //printf("flunc=%f h=%f\n",flunc,h);
 
     int totOrb_rnorm=(int)PyTuple_Size(py_rOrb);
     int nOrbInCluster=(int)PyTuple_Size(py_rOrbCluster)/totOrb_rnorm;
     //printf("totOrb renorm=%d grain size=%d\n",totOrb_rnorm,nOrbInCluster);
-    int rOrb[totOrb_rnorm];
-    int rOrbCluster[totOrb_rnorm][nOrbInCluster];
-    int linkedOrb_rnorm[totOrb_rnorm][maxNLinking];
+    int *rOrb=(int*)malloc(totOrb_rnorm*sizeof(int));
+    int *rOrbCluster=(int*)malloc(totOrb_rnorm*nOrbInCluster*sizeof(int));
+    int *linkedOrb_rnorm=(int*)malloc(totOrb_rnorm*maxNLinking*sizeof(int));
     for(int iorb=0;iorb<totOrb_rnorm;iorb++){
         rOrb[iorb]=(int)PyLong_AsLong(PyTuple_GetItem(py_rOrb,iorb));
         for(int iorb_cluster=0;iorb_cluster<nOrbInCluster;iorb_cluster++)
-            rOrbCluster[iorb][iorb_cluster]=(int)PyLong_AsLong(PyTuple_GetItem(py_rOrbCluster,iorb*nOrbInCluster+iorb_cluster));
+            rOrbCluster[iorb*nOrbInCluster+iorb_cluster]=(int)PyLong_AsLong(PyTuple_GetItem(py_rOrbCluster,iorb*nOrbInCluster+iorb_cluster));
         for(int ilink=0;ilink<maxNLinking;ilink++)
-            linkedOrb_rnorm[iorb][ilink]=(int)PyLong_AsLong(PyTuple_GetItem(py_linkedOrb_rnorm,iorb*maxNLinking+ilink));
+            linkedOrb_rnorm[iorb*maxNLinking+ilink]=(int)PyLong_AsLong(PyTuple_GetItem(py_linkedOrb_rnorm,iorb*maxNLinking+ilink));
     }
 
     // set algorithm
     p_mcUpdate=localUpdate;
     if(algorithm==1) p_mcUpdate=blockUpdate;
 
     // set diagonal dot function
```

### Comparing `mcsolver-3.0.4/mcsolver.egg-info/PKG-INFO` & `mcsolver-3.0.5/mcsolver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: mcsolver
-Version: 3.0.4
+Version: 3.0.5
 Summary: A user friendly program to do Monte Carlo sims for magnetic systems
 Home-page: https://github.com/golddoushi/mcsolver
 Author: Liang Liu
 Author-email: liangliu@main.sdu.edu.cn
 License: UNKNOWN
 Description: # mcsolver
         A user friendly and efficient tool implementing Monte Carlo simulations to estimate Curie/Neel temperature
```

### Comparing `mcsolver-3.0.4/mcsolver.egg-info/SOURCES.txt` & `mcsolver-3.0.5/mcsolver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mcsolver-3.0.4/setup.py` & `mcsolver-3.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 isingLib=Extension('isinglib',sources=['./mcsolver/isingLib.c'],language='c',extra_compile_args=['-std=c99','-fPIC','-O3'])
 xyLib=Extension('xylib',sources=['./mcsolver/xyLib.c'],language='c',extra_compile_args=['-std=c99','-fPIC','-O3'])
 heisenbergLib=Extension('heisenberglib',sources=['./mcsolver/heisenbergLib.c'],language='c',extra_compile_args=['-std=c99','-fPIC','-O3'])
 
 setup(
     name="mcsolver",
-    version="3.0.4",
+    version="3.0.5",
     author="Liang Liu",
     author_email="liangliu@main.sdu.edu.cn",
     description="A user friendly program to do Monte Carlo sims for magnetic systems",
     long_description=long_description,
     #long_description_content_type="text/markdown",
     url="https://github.com/golddoushi/mcsolver",
     packages=["mcsolver"],
```

### Comparing `mcsolver-3.0.4/setup2.py` & `mcsolver-3.0.5/setup2.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mcsolver",
-    version="3.0.4",
+    version="3.0.5",
     author="Liang Liu",
     author_email="liangliu@main.sdu.edu.cn",
     description="A user friendly program to do Monte Carlo sims for magnetic systems",
     long_description=long_description,
     python_requires='>=3.7',
     install_requires = ['matplotlib','numpy'],
     url="https://github.com/golddoushi/mcsolver",
```

