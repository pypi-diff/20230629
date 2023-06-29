# Comparing `tmp/OpenRadio-1.0.tar.gz` & `tmp/OpenRadio-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OpenRadio-1.0.tar", last modified: Tue May 23 15:49:44 2023, max compression
+gzip compressed data, was "OpenRadio-1.1.0.tar", last modified: Thu Jun 29 16:12:38 2023, max compression
```

## Comparing `OpenRadio-1.0.tar` & `OpenRadio-1.1.0.tar`

### file list

```diff
@@ -1,390 +1,459 @@
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-05-23 15:49:44.114567 OpenRadio-1.0/
--rw-rw-r--   0 simon     (1000) simon     (1000)    35129 2023-05-11 13:36:22.000000 OpenRadio-1.0/LICENSE.md
--rw-rw-r--   0 simon     (1000) simon     (1000)     7222 2023-05-11 13:46:31.000000 OpenRadio-1.0/LICENSE_Flags.md
--rw-rw-r--   0 simon     (1000) simon     (1000)    31331 2023-05-11 13:55:23.000000 OpenRadio-1.0/LICENSE_Icons.md
--rw-rw-r--   0 simon     (1000) simon     (1000)       75 2023-05-13 16:43:34.000000 OpenRadio-1.0/MANIFEST.in
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-05-23 15:49:44.062567 OpenRadio-1.0/OpenRadio/
--rw-rw-r--   0 simon     (1000) simon     (1000)      500 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/__init__.py
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-05-23 15:49:44.062567 OpenRadio-1.0/OpenRadio/assets/
--rw-rw-r--   0 simon     (1000) simon     (1000)    67646 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/OpenRadio.icon
--rw-rw-r--   0 simon     (1000) simon     (1000)    15563 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/bitmap.png
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-05-23 15:49:44.062567 OpenRadio-1.0/OpenRadio/assets/icons/
--rw-rw-r--   0 simon     (1000) simon     (1000)     1793 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/alarm-symbolic.svg
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-05-23 15:49:44.106567 OpenRadio-1.0/OpenRadio/assets/icons/countries/
--rw-rw-r--   0 simon     (1000) simon     (1000)    92775 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/ad.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      330 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/ae.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)   190468 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/af.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      678 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/ag.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)     4249 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/ai.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)     8675 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/al.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      251 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/am.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)     2273 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/ao.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      283 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/aq.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)     5009 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/ar.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)    49194 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/as.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      217 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/at.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)     1557 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/au.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      408 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/aw.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      412 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/ax.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      593 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/az.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      539 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/ba.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      822 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/bb.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      211 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/bd.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      232 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/be.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      677 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/bf.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      277 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/bg.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      277 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/bh.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      725 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/bi.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      247 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/bj.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      259 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/bl.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)    34544 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/bm.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)    24416 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/bn.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      266 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/bo.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      265 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/bq.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)     5262 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/br.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      239 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/bs.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)    38925 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/bt.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      414 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/bv.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      270 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/bw.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)     1532 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/by.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)    86462 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/bz.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      741 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/ca.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)     4945 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/cc.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      489 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/cd.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      437 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/cf.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      284 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/cg.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      234 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/ch.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      244 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/ci.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)     1272 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/ck.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      351 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/cl.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      487 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/cm.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      665 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/cn.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      371 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/co.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)    72287 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/cr.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      365 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/cu.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)     1329 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/cv.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      716 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/cw.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)     4039 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/cx.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)    11533 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/cy.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      274 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/cz.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      457 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/de.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      410 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/dj.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      214 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/dk.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)    12255 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/dm.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)   184096 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/do.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      338 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/dz.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)   287468 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/ec.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      257 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/ee.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)    20586 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/eg.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      283 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/eh.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)    12302 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/er.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)    63079 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/es.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      919 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/et.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      281 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/fi.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)    55994 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/fj.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)   216962 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/fk.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      817 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/fm.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      394 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/fo.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      259 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/fr.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      250 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/ga.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      665 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/gb.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)     1469 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/gd.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      977 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/ge.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      259 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/gf.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      342 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/gg.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      343 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/gh.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)     5345 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/gi.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      251 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/gl.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      335 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/gm.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      255 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/gn.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)    19946 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/gp.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)     7139 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/gq.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      287 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/gr.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)    65458 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/gs.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)    88758 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/gt.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)    12382 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/gu.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      706 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/gw.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      357 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/gy.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      775 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/hk.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)     1557 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/hm.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      568 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/hn.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)    69237 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/hr.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)   146550 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/ht.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      763 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/hu.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      195 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/id.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      277 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/ie.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      401 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/il.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)     7441 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/im.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)     1113 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/in.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)    78557 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/io.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)     2753 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/iq.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)     1520 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/ir.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      299 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/is.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      278 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/it.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)   172680 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/je.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      362 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/jm.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      456 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/jo.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      212 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/jp.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)     1333 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/ke.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)    16841 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/kg.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)    10668 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/kh.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)     6352 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/ki.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      763 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/km.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      851 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/kn.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      904 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/kp.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      757 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/kr.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      320 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/kw.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)    47530 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/ky.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)    10232 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/kz.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      295 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/la.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)     6065 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/lb.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      353 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/lc.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)    16676 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/li.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)    23952 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/lk.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      810 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/lr.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)     2316 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/ls.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      250 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/lt.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      276 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/lu.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      202 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/lv.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      451 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/ly.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      300 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/ma.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      201 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/mc.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)    46392 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/md.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)    77922 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/me.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      259 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/mf.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      259 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/mg.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      833 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/mh.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      460 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/mk.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      247 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/ml.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      664 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/mm.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)     1583 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/mn.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)     2673 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/mo.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)   455627 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/mp.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      259 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/mq.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      664 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/mr.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)    12017 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/ms.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)   290586 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/mt.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      292 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/mu.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      333 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/mv.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)     1151 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/mw.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)   162396 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/mx.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      720 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/my.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)     3725 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/mz.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      824 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/na.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      259 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/nc.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      311 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/ne.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)    23254 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/nf.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      243 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/ng.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)    26615 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/ni.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      265 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/nl.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      414 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/no.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)     1066 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/np.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      587 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/nr.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)     1283 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/nu.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)     2451 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/nz.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)    16890 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/om.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      374 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/pa.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      337 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/pe.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)     7593 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/pf.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)     3231 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/pg.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      954 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/ph.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      703 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/pk.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      221 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/pl.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)    93537 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/pm.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)    19848 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/pn.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      323 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/pr.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      283 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/ps.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)    13173 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/pt.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      215 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/pw.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)    23661 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/py.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      311 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/qa.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      259 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/re.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      280 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/ro.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)   126627 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/rs.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      277 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/ru.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      804 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/rw.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)    17489 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/sa.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      950 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/sb.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      330 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/sc.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      282 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/sd.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      209 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/se.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)     1248 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/sg.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)    93713 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/sh.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)     3228 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/si.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      283 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/sj.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)     2059 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/sk.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      244 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/sl.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)   125040 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/sm.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      744 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/sn.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      614 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/so.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      381 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/sr.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      564 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/ss.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      782 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/st.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)   274288 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/sv.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)    25918 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/sx.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      364 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/sy.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)     7553 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/sz.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)     6839 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/tc.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      247 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/td.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      921 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/tf.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      716 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/tg.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      278 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/th.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)     1842 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/tj.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)     1403 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/tk.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      454 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/tl.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)    59356 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/tm.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      334 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/tn.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      336 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/to.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      357 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/tr.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      303 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/tt.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)     1492 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/tv.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      548 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/tw.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      503 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/tz.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      223 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/ua.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)     4590 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/ug.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      998 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/um.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)     1676 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/us.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)    10139 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/uy.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)     1465 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/uz.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)    45755 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/va.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      591 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/vc.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)     1047 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/ve.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)    19972 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/vg.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)    25693 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/vi.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      278 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/vn.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)     2774 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/vu.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      259 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/wf.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      734 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/ws.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      229 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/ye.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      259 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/yt.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)      488 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/za.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)     8732 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/zm.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)    26277 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/countries/zw.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)     1653 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/globe-symbolic.svg
--rw-rw-r--   0 simon     (1000) simon     (1000)     3406 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/map-search-outline.png
--rw-rw-r--   0 simon     (1000) simon     (1000)     2631 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/search-web.png
--rw-rw-r--   0 simon     (1000) simon     (1000)     3411 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/star-outline.png
--rw-rw-r--   0 simon     (1000) simon     (1000)     2554 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/star.png
--rw-rw-r--   0 simon     (1000) simon     (1000)     3528 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/assets/icons/tag-search-outline.png
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-05-23 15:49:44.106567 OpenRadio-1.0/OpenRadio/core/
--rw-rw-r--   0 simon     (1000) simon     (1000)    15113 2023-05-22 13:27:42.000000 OpenRadio-1.0/OpenRadio/core/AudioPlayer.py
--rw-rw-r--   0 simon     (1000) simon     (1000)      864 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/core/Core.py
--rw-rw-r--   0 simon     (1000) simon     (1000)       47 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/core/Exceptions.py
--rw-rw-r--   0 simon     (1000) simon     (1000)     5207 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/core/HTTPApi.py
--rw-rw-r--   0 simon     (1000) simon     (1000)     1574 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/core/IconHelper.py
--rw-rw-r--   0 simon     (1000) simon     (1000)     1110 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/core/Localizer.py
--rw-rw-r--   0 simon     (1000) simon     (1000)      382 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/core/ModuleClass.py
--rw-rw-r--   0 simon     (1000) simon     (1000)     2634 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/core/ModuleHandler.py
--rw-rw-r--   0 simon     (1000) simon     (1000)     1417 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/core/Settings.py
--rw-rw-r--   0 simon     (1000) simon     (1000)     5038 2023-05-13 17:22:06.000000 OpenRadio-1.0/OpenRadio/core/Window.py
--rw-rw-r--   0 simon     (1000) simon     (1000)     1375 2023-05-11 14:00:41.000000 OpenRadio-1.0/OpenRadio/core/const.py
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-05-23 15:49:44.058567 OpenRadio-1.0/OpenRadio/locales/
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-05-23 15:49:44.054567 OpenRadio-1.0/OpenRadio/locales/core/
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-05-23 15:49:44.054567 OpenRadio-1.0/OpenRadio/locales/core/de/
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-05-23 15:49:44.106567 OpenRadio-1.0/OpenRadio/locales/core/de/LC_MESSAGES/
--rw-rw-r--   0 simon     (1000) simon     (1000)      415 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/locales/core/de/LC_MESSAGES/core.mo
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-05-23 15:49:44.054567 OpenRadio-1.0/OpenRadio/locales/core/en/
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-05-23 15:49:44.106567 OpenRadio-1.0/OpenRadio/locales/core/en/LC_MESSAGES/
--rw-rw-r--   0 simon     (1000) simon     (1000)      430 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/locales/core/en/LC_MESSAGES/core.mo
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-05-23 15:49:44.058567 OpenRadio-1.0/OpenRadio/locales/modules/
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-05-23 15:49:44.054567 OpenRadio-1.0/OpenRadio/locales/modules/builtin.about/
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-05-23 15:49:44.054567 OpenRadio-1.0/OpenRadio/locales/modules/builtin.about/de/
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-05-23 15:49:44.106567 OpenRadio-1.0/OpenRadio/locales/modules/builtin.about/de/LC_MESSAGES/
--rw-rw-r--   0 simon     (1000) simon     (1000)      898 2023-05-13 16:35:54.000000 OpenRadio-1.0/OpenRadio/locales/modules/builtin.about/de/LC_MESSAGES/builtin.about.mo
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-05-23 15:49:44.054567 OpenRadio-1.0/OpenRadio/locales/modules/builtin.about/en/
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-05-23 15:49:44.106567 OpenRadio-1.0/OpenRadio/locales/modules/builtin.about/en/LC_MESSAGES/
--rw-rw-r--   0 simon     (1000) simon     (1000)      854 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/locales/modules/builtin.about/en/LC_MESSAGES/builtin.about.mo
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-05-23 15:49:44.054567 OpenRadio-1.0/OpenRadio/locales/modules/builtin.clock/
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-05-23 15:49:44.054567 OpenRadio-1.0/OpenRadio/locales/modules/builtin.clock/de/
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-05-23 15:49:44.106567 OpenRadio-1.0/OpenRadio/locales/modules/builtin.clock/de/LC_MESSAGES/
--rw-rw-r--   0 simon     (1000) simon     (1000)      334 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/locales/modules/builtin.clock/de/LC_MESSAGES/builtin.clock.mo
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-05-23 15:49:44.054567 OpenRadio-1.0/OpenRadio/locales/modules/builtin.exit/
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-05-23 15:49:44.054567 OpenRadio-1.0/OpenRadio/locales/modules/builtin.exit/de/
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-05-23 15:49:44.106567 OpenRadio-1.0/OpenRadio/locales/modules/builtin.exit/de/LC_MESSAGES/
--rw-rw-r--   0 simon     (1000) simon     (1000)      334 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/locales/modules/builtin.exit/de/LC_MESSAGES/builtin.exit.mo
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-05-23 15:49:44.058567 OpenRadio-1.0/OpenRadio/locales/modules/builtin.internetradio/
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-05-23 15:49:44.058567 OpenRadio-1.0/OpenRadio/locales/modules/builtin.internetradio/de/
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-05-23 15:49:44.106567 OpenRadio-1.0/OpenRadio/locales/modules/builtin.internetradio/de/LC_MESSAGES/
--rw-rw-r--   0 simon     (1000) simon     (1000)      536 2023-05-13 16:38:27.000000 OpenRadio-1.0/OpenRadio/locales/modules/builtin.internetradio/de/LC_MESSAGES/builtin.internetradio.mo
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-05-23 15:49:44.058567 OpenRadio-1.0/OpenRadio/locales/modules/builtin.internetradio/en/
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-05-23 15:49:44.106567 OpenRadio-1.0/OpenRadio/locales/modules/builtin.internetradio/en/LC_MESSAGES/
--rw-rw-r--   0 simon     (1000) simon     (1000)      534 2023-05-13 16:38:37.000000 OpenRadio-1.0/OpenRadio/locales/modules/builtin.internetradio/en/LC_MESSAGES/builtin.internetradio.mo
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-05-23 15:49:44.058567 OpenRadio-1.0/OpenRadio/locales/modules/builtin.settings/
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-05-23 15:49:44.058567 OpenRadio-1.0/OpenRadio/locales/modules/builtin.settings/de/
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-05-23 15:49:44.110566 OpenRadio-1.0/OpenRadio/locales/modules/builtin.settings/de/LC_MESSAGES/
--rw-rw-r--   0 simon     (1000) simon     (1000)      334 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/locales/modules/builtin.settings/de/LC_MESSAGES/builtin.settings.mo
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-05-23 15:49:44.058567 OpenRadio-1.0/OpenRadio/locales/src/
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-05-23 15:49:44.058567 OpenRadio-1.0/OpenRadio/locales/src/de/
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-05-23 15:49:44.110566 OpenRadio-1.0/OpenRadio/locales/src/de/core/
--rw-rw-r--   0 simon     (1000) simon     (1000)      593 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/locales/src/de/core/core.pot
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-05-23 15:49:44.058567 OpenRadio-1.0/OpenRadio/locales/src/de/modules/
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-05-23 15:49:44.110566 OpenRadio-1.0/OpenRadio/locales/src/de/modules/builtin.about/
--rw-rw-r--   0 simon     (1000) simon     (1000)     1129 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/locales/src/de/modules/builtin.about/builtin.about.pot
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-05-23 15:49:44.110566 OpenRadio-1.0/OpenRadio/locales/src/de/modules/builtin.clock/
--rw-rw-r--   0 simon     (1000) simon     (1000)      474 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/locales/src/de/modules/builtin.clock/builtin.clock.pot
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-05-23 15:49:44.110566 OpenRadio-1.0/OpenRadio/locales/src/de/modules/builtin.demo/
--rw-rw-r--   0 simon     (1000) simon     (1000)      474 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/locales/src/de/modules/builtin.demo/builtin.demo.pot
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-05-23 15:49:44.110566 OpenRadio-1.0/OpenRadio/locales/src/de/modules/builtin.exit/
--rw-rw-r--   0 simon     (1000) simon     (1000)      474 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/locales/src/de/modules/builtin.exit/builtin.exit.pot
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-05-23 15:49:44.110566 OpenRadio-1.0/OpenRadio/locales/src/de/modules/builtin.internetradio/
--rw-rw-r--   0 simon     (1000) simon     (1000)      899 2023-05-13 16:34:31.000000 OpenRadio-1.0/OpenRadio/locales/src/de/modules/builtin.internetradio/builtin.internetradio.pot
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-05-23 15:49:44.110566 OpenRadio-1.0/OpenRadio/locales/src/de/modules/builtin.settings/
--rw-rw-r--   0 simon     (1000) simon     (1000)      474 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/locales/src/de/modules/builtin.settings/builtin.settings.pot
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-05-23 15:49:44.058567 OpenRadio-1.0/OpenRadio/locales/src/en/
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-05-23 15:49:44.110566 OpenRadio-1.0/OpenRadio/locales/src/en/core/
--rw-rw-r--   0 simon     (1000) simon     (1000)      608 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/locales/src/en/core/core.pot
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-05-23 15:49:44.058567 OpenRadio-1.0/OpenRadio/locales/src/en/modules/
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-05-23 15:49:44.110566 OpenRadio-1.0/OpenRadio/locales/src/en/modules/builtin.about/
--rw-rw-r--   0 simon     (1000) simon     (1000)     1085 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/locales/src/en/modules/builtin.about/builtin.about.pot
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-05-23 15:49:44.110566 OpenRadio-1.0/OpenRadio/locales/src/en/modules/builtin.clock/
--rw-rw-r--   0 simon     (1000) simon     (1000)      474 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/locales/src/en/modules/builtin.clock/builtin.clock.pot
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-05-23 15:49:44.110566 OpenRadio-1.0/OpenRadio/locales/src/en/modules/builtin.demo/
--rw-rw-r--   0 simon     (1000) simon     (1000)      474 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/locales/src/en/modules/builtin.demo/builtin.demo.pot
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-05-23 15:49:44.110566 OpenRadio-1.0/OpenRadio/locales/src/en/modules/builtin.exit/
--rw-rw-r--   0 simon     (1000) simon     (1000)      474 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/locales/src/en/modules/builtin.exit/builtin.exit.pot
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-05-23 15:49:44.110566 OpenRadio-1.0/OpenRadio/locales/src/en/modules/builtin.internetradio/
--rw-rw-r--   0 simon     (1000) simon     (1000)      897 2023-05-13 16:34:45.000000 OpenRadio-1.0/OpenRadio/locales/src/en/modules/builtin.internetradio/builtin.internetradio.pot
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-05-23 15:49:44.110566 OpenRadio-1.0/OpenRadio/locales/src/en/modules/builtin.settings/
--rw-rw-r--   0 simon     (1000) simon     (1000)      474 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/locales/src/en/modules/builtin.settings/builtin.settings.pot
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-05-23 15:49:44.058567 OpenRadio-1.0/OpenRadio/locales/templates/
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-05-23 15:49:44.110566 OpenRadio-1.0/OpenRadio/locales/templates/core/
--rw-rw-r--   0 simon     (1000) simon     (1000)      573 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/locales/templates/core/core.pot
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-05-23 15:49:44.058567 OpenRadio-1.0/OpenRadio/locales/templates/modules/
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-05-23 15:49:44.110566 OpenRadio-1.0/OpenRadio/locales/templates/modules/builtin.about/
--rw-rw-r--   0 simon     (1000) simon     (1000)      817 2023-05-13 16:31:44.000000 OpenRadio-1.0/OpenRadio/locales/templates/modules/builtin.about/builtin.about.pot
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-05-23 15:49:44.110566 OpenRadio-1.0/OpenRadio/locales/templates/modules/builtin.clock/
--rw-rw-r--   0 simon     (1000) simon     (1000)      474 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/locales/templates/modules/builtin.clock/builtin.clock.pot
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-05-23 15:49:44.110566 OpenRadio-1.0/OpenRadio/locales/templates/modules/builtin.exit/
--rw-rw-r--   0 simon     (1000) simon     (1000)      474 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/locales/templates/modules/builtin.exit/builtin.exit.pot
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-05-23 15:49:44.110566 OpenRadio-1.0/OpenRadio/locales/templates/modules/builtin.internetradio/
--rw-rw-r--   0 simon     (1000) simon     (1000)      842 2023-05-13 16:45:04.000000 OpenRadio-1.0/OpenRadio/locales/templates/modules/builtin.internetradio/builtin.internetradio.pot
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-05-23 15:49:44.110566 OpenRadio-1.0/OpenRadio/locales/templates/modules/builtin.settings/
--rw-rw-r--   0 simon     (1000) simon     (1000)      587 2023-05-13 16:32:23.000000 OpenRadio-1.0/OpenRadio/locales/templates/modules/builtin.settings/builtin.settings.pot
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-05-23 15:49:44.058567 OpenRadio-1.0/OpenRadio/modules/
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-05-23 15:49:44.110566 OpenRadio-1.0/OpenRadio/modules/About/
--rw-rw-r--   0 simon     (1000) simon     (1000)     1735 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/modules/About/__init__.py
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-05-23 15:49:44.110566 OpenRadio-1.0/OpenRadio/modules/Alarm/
--rw-rw-r--   0 simon     (1000) simon     (1000)     3295 2023-05-13 17:01:19.000000 OpenRadio-1.0/OpenRadio/modules/Alarm/TimeThread.py
--rw-rw-r--   0 simon     (1000) simon     (1000)     1992 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/modules/Alarm/TimeWidget.py
--rw-rw-r--   0 simon     (1000) simon     (1000)    11534 2023-05-13 17:08:25.000000 OpenRadio-1.0/OpenRadio/modules/Alarm/__init__.py
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-05-23 15:49:44.110566 OpenRadio-1.0/OpenRadio/modules/Clock/
--rw-rw-r--   0 simon     (1000) simon     (1000)     2343 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/modules/Clock/__init__.py
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-05-23 15:49:44.110566 OpenRadio-1.0/OpenRadio/modules/Exit/
--rw-rw-r--   0 simon     (1000) simon     (1000)      553 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/modules/Exit/__init__.py
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-05-23 15:49:44.114567 OpenRadio-1.0/OpenRadio/modules/InternetRadio/
--rw-rw-r--   0 simon     (1000) simon     (1000)     2689 2023-05-13 18:02:45.000000 OpenRadio-1.0/OpenRadio/modules/InternetRadio/IconThread.py
--rw-rw-r--   0 simon     (1000) simon     (1000)    15611 2023-05-13 18:03:04.000000 OpenRadio-1.0/OpenRadio/modules/InternetRadio/UI.py
--rw-rw-r--   0 simon     (1000) simon     (1000)     2286 2023-05-13 17:25:34.000000 OpenRadio-1.0/OpenRadio/modules/InternetRadio/__init__.py
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-05-23 15:49:44.114567 OpenRadio-1.0/OpenRadio/modules/Settings/
--rw-rw-r--   0 simon     (1000) simon     (1000)     2655 2023-05-11 13:31:29.000000 OpenRadio-1.0/OpenRadio/modules/Settings/__init__.py
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-05-23 15:49:44.062567 OpenRadio-1.0/OpenRadio.egg-info/
--rw-rw-r--   0 simon     (1000) simon     (1000)     1049 2023-05-23 15:49:44.000000 OpenRadio-1.0/OpenRadio.egg-info/PKG-INFO
--rw-rw-r--   0 simon     (1000) simon     (1000)    13226 2023-05-23 15:49:44.000000 OpenRadio-1.0/OpenRadio.egg-info/SOURCES.txt
--rw-rw-r--   0 simon     (1000) simon     (1000)        1 2023-05-23 15:49:44.000000 OpenRadio-1.0/OpenRadio.egg-info/dependency_links.txt
--rw-rw-r--   0 simon     (1000) simon     (1000)       42 2023-05-23 15:49:44.000000 OpenRadio-1.0/OpenRadio.egg-info/entry_points.txt
--rw-rw-r--   0 simon     (1000) simon     (1000)       58 2023-05-23 15:49:44.000000 OpenRadio-1.0/OpenRadio.egg-info/requires.txt
--rw-rw-r--   0 simon     (1000) simon     (1000)       10 2023-05-23 15:49:44.000000 OpenRadio-1.0/OpenRadio.egg-info/top_level.txt
--rw-rw-r--   0 simon     (1000) simon     (1000)     1049 2023-05-23 15:49:44.114567 OpenRadio-1.0/PKG-INFO
--rw-rw-r--   0 simon     (1000) simon     (1000)      411 2023-05-11 13:31:40.000000 OpenRadio-1.0/README.md
--rw-rw-r--   0 simon     (1000) simon     (1000)      865 2023-05-23 15:35:07.000000 OpenRadio-1.0/pyproject.toml
--rw-rw-r--   0 simon     (1000) simon     (1000)       38 2023-05-23 15:49:44.114567 OpenRadio-1.0/setup.cfg
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.648041 OpenRadio-1.1.0/
+-rw-rw-r--   0 simon     (1000) simon     (1000)    35129 2023-05-11 13:36:22.000000 OpenRadio-1.1.0/LICENSE.md
+-rw-rw-r--   0 simon     (1000) simon     (1000)     7222 2023-05-11 13:46:31.000000 OpenRadio-1.1.0/LICENSE_Flags.md
+-rw-rw-r--   0 simon     (1000) simon     (1000)    32171 2023-06-28 19:46:14.000000 OpenRadio-1.1.0/LICENSE_Icons.md
+-rw-rw-r--   0 simon     (1000) simon     (1000)      148 2023-06-29 15:42:43.000000 OpenRadio-1.1.0/MANIFEST.in
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.588042 OpenRadio-1.1.0/OpenRadio/
+-rw-rw-r--   0 simon     (1000) simon     (1000)      546 2023-06-29 14:02:04.000000 OpenRadio-1.1.0/OpenRadio/__init__.py
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.588042 OpenRadio-1.1.0/OpenRadio/assets/
+-rw-rw-r--   0 simon     (1000) simon     (1000)    67646 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/OpenRadio.icon
+-rw-rw-r--   0 simon     (1000) simon     (1000)    15563 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/OpenRadio.png
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.592042 OpenRadio-1.1.0/OpenRadio/assets/icons/
+-rw-r--r--   0 simon     (1000) simon     (1000)     1792 2023-06-28 19:15:35.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/alarm-symbolic.svg
+-rw-r--r--   0 simon     (1000) simon     (1000)     5237 2023-06-28 19:01:45.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/application-exit.png
+-rw-r--r--   0 simon     (1000) simon     (1000)    24764 2023-06-28 19:01:09.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/applications-internet.png
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.636041 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/
+-rw-rw-r--   0 simon     (1000) simon     (1000)    92775 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/ad.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      330 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/ae.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)   190468 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/af.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      678 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/ag.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)     4249 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/ai.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)     8675 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/al.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      251 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/am.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)     2273 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/ao.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      283 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/aq.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)     5009 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/ar.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)    49194 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/as.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      217 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/at.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)     1557 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/au.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      408 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/aw.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      412 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/ax.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      593 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/az.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      539 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/ba.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      822 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/bb.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      211 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/bd.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      232 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/be.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      677 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/bf.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      277 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/bg.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      277 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/bh.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      725 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/bi.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      247 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/bj.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      259 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/bl.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)    34544 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/bm.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)    24416 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/bn.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      266 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/bo.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      265 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/bq.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)     5262 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/br.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      239 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/bs.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)    38925 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/bt.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      414 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/bv.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      270 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/bw.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)     1532 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/by.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)    86462 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/bz.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      741 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/ca.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)     4945 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/cc.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      489 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/cd.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      437 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/cf.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      284 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/cg.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      234 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/ch.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      244 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/ci.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)     1272 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/ck.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      351 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/cl.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      487 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/cm.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      665 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/cn.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      371 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/co.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)    72287 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/cr.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      365 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/cu.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)     1329 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/cv.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      716 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/cw.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)     4039 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/cx.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)    11533 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/cy.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      274 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/cz.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      457 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/de.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      410 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/dj.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      214 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/dk.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)    12255 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/dm.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)   184096 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/do.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      338 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/dz.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)   287468 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/ec.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      257 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/ee.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)    20586 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/eg.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      283 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/eh.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)    12302 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/er.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)    63079 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/es.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      919 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/et.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      281 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/fi.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)    55994 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/fj.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)   216962 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/fk.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      817 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/fm.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      394 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/fo.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      259 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/fr.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      250 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/ga.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      665 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/gb.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)     1469 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/gd.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      977 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/ge.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      259 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/gf.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      342 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/gg.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      343 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/gh.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)     5345 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/gi.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      251 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/gl.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      335 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/gm.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      255 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/gn.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)    19946 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/gp.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)     7139 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/gq.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      287 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/gr.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)    65458 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/gs.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)    88758 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/gt.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)    12382 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/gu.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      706 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/gw.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      357 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/gy.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      775 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/hk.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)     1557 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/hm.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      568 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/hn.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)    69237 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/hr.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)   146550 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/ht.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      763 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/hu.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      195 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/id.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      277 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/ie.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      401 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/il.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)     7441 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/im.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)     1113 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/in.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)    78557 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/io.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)     2753 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/iq.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)     1520 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/ir.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      299 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/is.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      278 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/it.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)   172680 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/je.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      362 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/jm.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      456 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/jo.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      212 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/jp.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)     1333 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/ke.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)    16841 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/kg.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)    10668 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/kh.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)     6352 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/ki.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      763 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/km.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      851 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/kn.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      904 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/kp.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      757 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/kr.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      320 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/kw.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)    47530 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/ky.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)    10232 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/kz.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      295 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/la.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)     6065 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/lb.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      353 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/lc.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)    16676 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/li.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)    23952 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/lk.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      810 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/lr.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)     2316 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/ls.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      250 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/lt.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      276 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/lu.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      202 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/lv.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      451 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/ly.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      300 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/ma.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      201 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/mc.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)    46392 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/md.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)    77922 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/me.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      259 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/mf.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      259 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/mg.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      833 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/mh.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      460 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/mk.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      247 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/ml.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      664 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/mm.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)     1583 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/mn.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)     2673 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/mo.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)   455627 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/mp.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      259 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/mq.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      664 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/mr.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)    12017 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/ms.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)   290586 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/mt.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      292 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/mu.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      333 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/mv.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)     1151 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/mw.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)   162396 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/mx.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      720 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/my.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)     3725 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/mz.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      824 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/na.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      259 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/nc.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      311 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/ne.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)    23254 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/nf.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      243 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/ng.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)    26615 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/ni.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      265 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/nl.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      414 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/no.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)     1066 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/np.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      587 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/nr.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)     1283 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/nu.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)     2451 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/nz.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)    16890 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/om.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      374 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/pa.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      337 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/pe.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)     7593 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/pf.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)     3231 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/pg.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      954 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/ph.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      703 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/pk.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      221 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/pl.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)    93537 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/pm.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)    19848 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/pn.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      323 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/pr.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      283 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/ps.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)    13173 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/pt.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      215 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/pw.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)    23661 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/py.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      311 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/qa.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      259 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/re.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      280 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/ro.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)   126627 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/rs.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      277 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/ru.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      804 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/rw.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)    17489 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/sa.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      950 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/sb.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      330 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/sc.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      282 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/sd.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      209 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/se.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)     1248 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/sg.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)    93713 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/sh.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)     3228 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/si.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      283 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/sj.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)     2059 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/sk.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      244 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/sl.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)   125040 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/sm.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      744 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/sn.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      614 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/so.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      381 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/sr.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      564 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/ss.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      782 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/st.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)   274288 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/sv.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)    25918 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/sx.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      364 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/sy.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)     7553 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/sz.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)     6839 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/tc.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      247 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/td.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      921 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/tf.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      716 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/tg.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      278 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/th.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)     1842 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/tj.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)     1403 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/tk.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      454 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/tl.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)    59356 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/tm.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      334 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/tn.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      336 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/to.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      357 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/tr.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      303 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/tt.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)     1492 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/tv.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      548 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/tw.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      503 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/tz.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      223 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/ua.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)     4590 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/ug.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      998 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/um.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)     1676 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/us.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)    10139 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/uy.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)     1465 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/uz.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)    45755 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/va.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      591 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/vc.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)     1047 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/ve.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)    19972 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/vg.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)    25693 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/vi.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      278 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/vn.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)     2774 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/vu.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      259 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/wf.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      734 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/ws.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      229 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/ye.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      259 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/yt.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      488 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/za.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)     8732 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/zm.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)    26277 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/countries/zw.svg
+-rw-r--r--   0 simon     (1000) simon     (1000)    13826 2023-06-28 19:00:54.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/dialog-information.png
+-rw-r--r--   0 simon     (1000) simon     (1000)    11830 2023-06-28 19:00:33.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/emblem-system.png
+-rw-r--r--   0 simon     (1000) simon     (1000)     1653 2023-06-28 19:01:21.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/globe-symbolic.svg
+-rw-r--r--   0 simon     (1000) simon     (1000)      490 2023-06-28 19:04:34.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/go-down-symbolic.svg
+-rw-r--r--   0 simon     (1000) simon     (1000)      495 2023-06-28 19:02:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/go-previous-symbolic.svg
+-rw-r--r--   0 simon     (1000) simon     (1000)      489 2023-06-28 19:03:42.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/go-up-symbolic.svg
+-rw-r--r--   0 simon     (1000) simon     (1000)      616 2023-06-28 19:03:31.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/list-add-symbolic.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)     3406 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/map-search-outline.png
+-rw-r--r--   0 simon     (1000) simon     (1000)      572 2023-06-28 19:05:04.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/media-playback-pause-symbolic.svg
+-rw-r--r--   0 simon     (1000) simon     (1000)      162 2023-06-28 19:04:51.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/media-playback-start-symbolic.svg
+-rw-r--r--   0 simon     (1000) simon     (1000)      561 2023-06-28 19:04:58.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/media-playback-stop-symbolic.svg
+-rw-r--r--   0 simon     (1000) simon     (1000)     1633 2023-06-28 19:02:02.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/network-wireless-hotspot-symbolic.svg
+-rw-rw-r--   0 simon     (1000) simon     (1000)     2631 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/search-web.png
+-rw-rw-r--   0 simon     (1000) simon     (1000)     3411 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/star-outline.png
+-rw-rw-r--   0 simon     (1000) simon     (1000)     2554 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/star.png
+-rw-rw-r--   0 simon     (1000) simon     (1000)     3528 2023-05-11 13:31:29.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/tag-search-outline.png
+-rw-r--r--   0 simon     (1000) simon     (1000)      879 2023-06-28 19:05:21.000000 OpenRadio-1.1.0/OpenRadio/assets/icons/user-trash-symbolic.svg
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.636041 OpenRadio-1.1.0/OpenRadio/core/
+-rw-rw-r--   0 simon     (1000) simon     (1000)    14309 2023-06-29 14:02:04.000000 OpenRadio-1.1.0/OpenRadio/core/AudioPlayer.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)      921 2023-06-29 14:02:04.000000 OpenRadio-1.1.0/OpenRadio/core/Core.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)       94 2023-06-29 13:12:07.000000 OpenRadio-1.1.0/OpenRadio/core/Exceptions.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)     5468 2023-06-29 14:02:04.000000 OpenRadio-1.1.0/OpenRadio/core/HTTPApi.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)     2211 2023-06-29 14:02:04.000000 OpenRadio-1.1.0/OpenRadio/core/IconHelper.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)     1032 2023-06-29 14:02:04.000000 OpenRadio-1.1.0/OpenRadio/core/Localizer.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)     1254 2023-06-29 13:21:08.000000 OpenRadio-1.1.0/OpenRadio/core/ModuleClass.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)     3396 2023-06-29 14:02:04.000000 OpenRadio-1.1.0/OpenRadio/core/ModuleHandler.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)     1444 2023-06-29 14:02:04.000000 OpenRadio-1.1.0/OpenRadio/core/Settings.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)     2941 2023-06-29 13:24:59.000000 OpenRadio-1.1.0/OpenRadio/core/UIHelper.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)     5765 2023-06-29 14:02:04.000000 OpenRadio-1.1.0/OpenRadio/core/Window.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)     1501 2023-06-29 12:56:38.000000 OpenRadio-1.1.0/OpenRadio/core/const.py
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.584042 OpenRadio-1.1.0/OpenRadio/locales/
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.580042 OpenRadio-1.1.0/OpenRadio/locales/core/
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.580042 OpenRadio-1.1.0/OpenRadio/locales/core/de/
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.636041 OpenRadio-1.1.0/OpenRadio/locales/core/de/LC_MESSAGES/
+-rw-rw-r--   0 simon     (1000) simon     (1000)      415 2023-06-25 14:41:35.000000 OpenRadio-1.1.0/OpenRadio/locales/core/de/LC_MESSAGES/core.mo
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.580042 OpenRadio-1.1.0/OpenRadio/locales/core/en/
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.636041 OpenRadio-1.1.0/OpenRadio/locales/core/en/LC_MESSAGES/
+-rw-rw-r--   0 simon     (1000) simon     (1000)      430 2023-06-25 14:41:35.000000 OpenRadio-1.1.0/OpenRadio/locales/core/en/LC_MESSAGES/core.mo
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.580042 OpenRadio-1.1.0/OpenRadio/locales/modules/
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.580042 OpenRadio-1.1.0/OpenRadio/locales/modules/builtin.about/
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.580042 OpenRadio-1.1.0/OpenRadio/locales/modules/builtin.about/de/
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.636041 OpenRadio-1.1.0/OpenRadio/locales/modules/builtin.about/de/LC_MESSAGES/
+-rw-rw-r--   0 simon     (1000) simon     (1000)      866 2023-06-25 14:41:35.000000 OpenRadio-1.1.0/OpenRadio/locales/modules/builtin.about/de/LC_MESSAGES/builtin.about.mo
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.580042 OpenRadio-1.1.0/OpenRadio/locales/modules/builtin.about/en/
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.636041 OpenRadio-1.1.0/OpenRadio/locales/modules/builtin.about/en/LC_MESSAGES/
+-rw-rw-r--   0 simon     (1000) simon     (1000)      854 2023-06-25 14:41:35.000000 OpenRadio-1.1.0/OpenRadio/locales/modules/builtin.about/en/LC_MESSAGES/builtin.about.mo
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.580042 OpenRadio-1.1.0/OpenRadio/locales/modules/builtin.alarm/
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.580042 OpenRadio-1.1.0/OpenRadio/locales/modules/builtin.alarm/de/
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.640041 OpenRadio-1.1.0/OpenRadio/locales/modules/builtin.alarm/de/LC_MESSAGES/
+-rw-rw-r--   0 simon     (1000) simon     (1000)      984 2023-06-25 16:04:22.000000 OpenRadio-1.1.0/OpenRadio/locales/modules/builtin.alarm/de/LC_MESSAGES/builtin.alarm.mo
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.580042 OpenRadio-1.1.0/OpenRadio/locales/modules/builtin.alarm/en/
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.640041 OpenRadio-1.1.0/OpenRadio/locales/modules/builtin.alarm/en/LC_MESSAGES/
+-rw-rw-r--   0 simon     (1000) simon     (1000)      960 2023-06-25 16:03:50.000000 OpenRadio-1.1.0/OpenRadio/locales/modules/builtin.alarm/en/LC_MESSAGES/builtin.alarm.mo
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.580042 OpenRadio-1.1.0/OpenRadio/locales/modules/builtin.clock/
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.580042 OpenRadio-1.1.0/OpenRadio/locales/modules/builtin.clock/de/
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.640041 OpenRadio-1.1.0/OpenRadio/locales/modules/builtin.clock/de/LC_MESSAGES/
+-rw-rw-r--   0 simon     (1000) simon     (1000)      334 2023-06-25 14:41:35.000000 OpenRadio-1.1.0/OpenRadio/locales/modules/builtin.clock/de/LC_MESSAGES/builtin.clock.mo
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.580042 OpenRadio-1.1.0/OpenRadio/locales/modules/builtin.clock/en/
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.640041 OpenRadio-1.1.0/OpenRadio/locales/modules/builtin.clock/en/LC_MESSAGES/
+-rw-rw-r--   0 simon     (1000) simon     (1000)      334 2023-06-25 14:41:35.000000 OpenRadio-1.1.0/OpenRadio/locales/modules/builtin.clock/en/LC_MESSAGES/builtin.clock.mo
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.580042 OpenRadio-1.1.0/OpenRadio/locales/modules/builtin.core_settings/
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.580042 OpenRadio-1.1.0/OpenRadio/locales/modules/builtin.core_settings/de/
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.640041 OpenRadio-1.1.0/OpenRadio/locales/modules/builtin.core_settings/de/LC_MESSAGES/
+-rw-rw-r--   0 simon     (1000) simon     (1000)      583 2023-06-28 19:42:21.000000 OpenRadio-1.1.0/OpenRadio/locales/modules/builtin.core_settings/de/LC_MESSAGES/builtin.core_settings.mo
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.580042 OpenRadio-1.1.0/OpenRadio/locales/modules/builtin.core_settings/en/
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.640041 OpenRadio-1.1.0/OpenRadio/locales/modules/builtin.core_settings/en/LC_MESSAGES/
+-rw-rw-r--   0 simon     (1000) simon     (1000)      574 2023-06-28 19:42:22.000000 OpenRadio-1.1.0/OpenRadio/locales/modules/builtin.core_settings/en/LC_MESSAGES/builtin.core_settings.mo
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.580042 OpenRadio-1.1.0/OpenRadio/locales/modules/builtin.dab/
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.580042 OpenRadio-1.1.0/OpenRadio/locales/modules/builtin.dab/de/
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.640041 OpenRadio-1.1.0/OpenRadio/locales/modules/builtin.dab/de/LC_MESSAGES/
+-rw-rw-r--   0 simon     (1000) simon     (1000)      850 2023-06-25 14:56:54.000000 OpenRadio-1.1.0/OpenRadio/locales/modules/builtin.dab/de/LC_MESSAGES/builtin.dab.mo
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.580042 OpenRadio-1.1.0/OpenRadio/locales/modules/builtin.dab/en/
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.640041 OpenRadio-1.1.0/OpenRadio/locales/modules/builtin.dab/en/LC_MESSAGES/
+-rw-rw-r--   0 simon     (1000) simon     (1000)      818 2023-06-25 14:50:23.000000 OpenRadio-1.1.0/OpenRadio/locales/modules/builtin.dab/en/LC_MESSAGES/builtin.dab.mo
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.580042 OpenRadio-1.1.0/OpenRadio/locales/modules/builtin.exit/
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.580042 OpenRadio-1.1.0/OpenRadio/locales/modules/builtin.exit/de/
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.640041 OpenRadio-1.1.0/OpenRadio/locales/modules/builtin.exit/de/LC_MESSAGES/
+-rw-rw-r--   0 simon     (1000) simon     (1000)      334 2023-06-25 14:41:35.000000 OpenRadio-1.1.0/OpenRadio/locales/modules/builtin.exit/de/LC_MESSAGES/builtin.exit.mo
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.580042 OpenRadio-1.1.0/OpenRadio/locales/modules/builtin.exit/en/
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.640041 OpenRadio-1.1.0/OpenRadio/locales/modules/builtin.exit/en/LC_MESSAGES/
+-rw-rw-r--   0 simon     (1000) simon     (1000)      334 2023-06-25 14:41:35.000000 OpenRadio-1.1.0/OpenRadio/locales/modules/builtin.exit/en/LC_MESSAGES/builtin.exit.mo
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.580042 OpenRadio-1.1.0/OpenRadio/locales/modules/builtin.internetradio/
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.580042 OpenRadio-1.1.0/OpenRadio/locales/modules/builtin.internetradio/de/
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.640041 OpenRadio-1.1.0/OpenRadio/locales/modules/builtin.internetradio/de/LC_MESSAGES/
+-rw-rw-r--   0 simon     (1000) simon     (1000)      536 2023-06-25 14:41:35.000000 OpenRadio-1.1.0/OpenRadio/locales/modules/builtin.internetradio/de/LC_MESSAGES/builtin.internetradio.mo
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.580042 OpenRadio-1.1.0/OpenRadio/locales/modules/builtin.internetradio/en/
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.640041 OpenRadio-1.1.0/OpenRadio/locales/modules/builtin.internetradio/en/LC_MESSAGES/
+-rw-rw-r--   0 simon     (1000) simon     (1000)      534 2023-06-25 14:41:35.000000 OpenRadio-1.1.0/OpenRadio/locales/modules/builtin.internetradio/en/LC_MESSAGES/builtin.internetradio.mo
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.580042 OpenRadio-1.1.0/OpenRadio/locales/modules/builtin.settings/
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.580042 OpenRadio-1.1.0/OpenRadio/locales/modules/builtin.settings/de/
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.640041 OpenRadio-1.1.0/OpenRadio/locales/modules/builtin.settings/de/LC_MESSAGES/
+-rw-rw-r--   0 simon     (1000) simon     (1000)      415 2023-06-25 14:41:35.000000 OpenRadio-1.1.0/OpenRadio/locales/modules/builtin.settings/de/LC_MESSAGES/builtin.settings.mo
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.580042 OpenRadio-1.1.0/OpenRadio/locales/modules/builtin.settings/en/
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.640041 OpenRadio-1.1.0/OpenRadio/locales/modules/builtin.settings/en/LC_MESSAGES/
+-rw-rw-r--   0 simon     (1000) simon     (1000)      430 2023-06-25 14:41:35.000000 OpenRadio-1.1.0/OpenRadio/locales/modules/builtin.settings/en/LC_MESSAGES/builtin.settings.mo
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.584042 OpenRadio-1.1.0/OpenRadio/locales/src/
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.580042 OpenRadio-1.1.0/OpenRadio/locales/src/de/
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.640041 OpenRadio-1.1.0/OpenRadio/locales/src/de/core/
+-rw-rw-r--   0 simon     (1000) simon     (1000)      598 2023-06-25 14:41:35.000000 OpenRadio-1.1.0/OpenRadio/locales/src/de/core/core.pot
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.584042 OpenRadio-1.1.0/OpenRadio/locales/src/de/modules/
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.640041 OpenRadio-1.1.0/OpenRadio/locales/src/de/modules/builtin.about/
+-rw-rw-r--   0 simon     (1000) simon     (1000)     1102 2023-06-25 14:41:35.000000 OpenRadio-1.1.0/OpenRadio/locales/src/de/modules/builtin.about/builtin.about.pot
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.640041 OpenRadio-1.1.0/OpenRadio/locales/src/de/modules/builtin.alarm/
+-rw-rw-r--   0 simon     (1000) simon     (1000)     1991 2023-06-25 16:04:14.000000 OpenRadio-1.1.0/OpenRadio/locales/src/de/modules/builtin.alarm/builtin.alarm.pot
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.640041 OpenRadio-1.1.0/OpenRadio/locales/src/de/modules/builtin.clock/
+-rw-rw-r--   0 simon     (1000) simon     (1000)      474 2023-06-25 14:41:35.000000 OpenRadio-1.1.0/OpenRadio/locales/src/de/modules/builtin.clock/builtin.clock.pot
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.640041 OpenRadio-1.1.0/OpenRadio/locales/src/de/modules/builtin.core_settings/
+-rw-rw-r--   0 simon     (1000) simon     (1000)     1020 2023-06-28 19:41:31.000000 OpenRadio-1.1.0/OpenRadio/locales/src/de/modules/builtin.core_settings/builtin.core_settings.pot
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.640041 OpenRadio-1.1.0/OpenRadio/locales/src/de/modules/builtin.dab/
+-rw-rw-r--   0 simon     (1000) simon     (1000)     1330 2023-06-25 14:54:44.000000 OpenRadio-1.1.0/OpenRadio/locales/src/de/modules/builtin.dab/builtin.dab.pot
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.640041 OpenRadio-1.1.0/OpenRadio/locales/src/de/modules/builtin.exit/
+-rw-rw-r--   0 simon     (1000) simon     (1000)      474 2023-06-25 14:41:35.000000 OpenRadio-1.1.0/OpenRadio/locales/src/de/modules/builtin.exit/builtin.exit.pot
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.640041 OpenRadio-1.1.0/OpenRadio/locales/src/de/modules/builtin.internetradio/
+-rw-rw-r--   0 simon     (1000) simon     (1000)      923 2023-06-25 14:41:35.000000 OpenRadio-1.1.0/OpenRadio/locales/src/de/modules/builtin.internetradio/builtin.internetradio.pot
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.640041 OpenRadio-1.1.0/OpenRadio/locales/src/de/modules/builtin.settings/
+-rw-rw-r--   0 simon     (1000) simon     (1000)      612 2023-06-25 14:41:35.000000 OpenRadio-1.1.0/OpenRadio/locales/src/de/modules/builtin.settings/builtin.settings.pot
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.584042 OpenRadio-1.1.0/OpenRadio/locales/src/en/
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.644041 OpenRadio-1.1.0/OpenRadio/locales/src/en/core/
+-rw-rw-r--   0 simon     (1000) simon     (1000)      613 2023-06-25 14:41:35.000000 OpenRadio-1.1.0/OpenRadio/locales/src/en/core/core.pot
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.584042 OpenRadio-1.1.0/OpenRadio/locales/src/en/modules/
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.644041 OpenRadio-1.1.0/OpenRadio/locales/src/en/modules/builtin.about/
+-rw-rw-r--   0 simon     (1000) simon     (1000)     1090 2023-06-25 14:41:35.000000 OpenRadio-1.1.0/OpenRadio/locales/src/en/modules/builtin.about/builtin.about.pot
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.644041 OpenRadio-1.1.0/OpenRadio/locales/src/en/modules/builtin.alarm/
+-rw-rw-r--   0 simon     (1000) simon     (1000)     1968 2023-06-25 16:02:56.000000 OpenRadio-1.1.0/OpenRadio/locales/src/en/modules/builtin.alarm/builtin.alarm.pot
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.644041 OpenRadio-1.1.0/OpenRadio/locales/src/en/modules/builtin.clock/
+-rw-rw-r--   0 simon     (1000) simon     (1000)      474 2023-06-25 14:41:35.000000 OpenRadio-1.1.0/OpenRadio/locales/src/en/modules/builtin.clock/builtin.clock.pot
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.644041 OpenRadio-1.1.0/OpenRadio/locales/src/en/modules/builtin.core_settings/
+-rw-rw-r--   0 simon     (1000) simon     (1000)     1011 2023-06-28 19:42:00.000000 OpenRadio-1.1.0/OpenRadio/locales/src/en/modules/builtin.core_settings/builtin.core_settings.pot
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.644041 OpenRadio-1.1.0/OpenRadio/locales/src/en/modules/builtin.dab/
+-rw-rw-r--   0 simon     (1000) simon     (1000)     1298 2023-06-25 14:50:08.000000 OpenRadio-1.1.0/OpenRadio/locales/src/en/modules/builtin.dab/builtin.dab.pot
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.644041 OpenRadio-1.1.0/OpenRadio/locales/src/en/modules/builtin.exit/
+-rw-rw-r--   0 simon     (1000) simon     (1000)      474 2023-06-25 14:41:35.000000 OpenRadio-1.1.0/OpenRadio/locales/src/en/modules/builtin.exit/builtin.exit.pot
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.644041 OpenRadio-1.1.0/OpenRadio/locales/src/en/modules/builtin.internetradio/
+-rw-rw-r--   0 simon     (1000) simon     (1000)      921 2023-06-25 14:41:35.000000 OpenRadio-1.1.0/OpenRadio/locales/src/en/modules/builtin.internetradio/builtin.internetradio.pot
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.644041 OpenRadio-1.1.0/OpenRadio/locales/src/en/modules/builtin.settings/
+-rw-rw-r--   0 simon     (1000) simon     (1000)      627 2023-06-25 14:41:35.000000 OpenRadio-1.1.0/OpenRadio/locales/src/en/modules/builtin.settings/builtin.settings.pot
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.584042 OpenRadio-1.1.0/OpenRadio/locales/templates/
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.644041 OpenRadio-1.1.0/OpenRadio/locales/templates/core/
+-rw-rw-r--   0 simon     (1000) simon     (1000)      579 2023-06-25 14:41:35.000000 OpenRadio-1.1.0/OpenRadio/locales/templates/core/core.pot
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.584042 OpenRadio-1.1.0/OpenRadio/locales/templates/modules/
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.644041 OpenRadio-1.1.0/OpenRadio/locales/templates/modules/builtin.about/
+-rw-rw-r--   0 simon     (1000) simon     (1000)      823 2023-06-25 14:41:35.000000 OpenRadio-1.1.0/OpenRadio/locales/templates/modules/builtin.about/builtin.about.pot
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.644041 OpenRadio-1.1.0/OpenRadio/locales/templates/modules/builtin.alarm/
+-rw-rw-r--   0 simon     (1000) simon     (1000)     1840 2023-06-25 15:59:15.000000 OpenRadio-1.1.0/OpenRadio/locales/templates/modules/builtin.alarm/builtin.alarm.pot
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.644041 OpenRadio-1.1.0/OpenRadio/locales/templates/modules/builtin.clock/
+-rw-rw-r--   0 simon     (1000) simon     (1000)      474 2023-06-25 14:41:35.000000 OpenRadio-1.1.0/OpenRadio/locales/templates/modules/builtin.clock/builtin.clock.pot
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.644041 OpenRadio-1.1.0/OpenRadio/locales/templates/modules/builtin.core_settings/
+-rw-rw-r--   0 simon     (1000) simon     (1000)      953 2023-06-28 19:38:52.000000 OpenRadio-1.1.0/OpenRadio/locales/templates/modules/builtin.core_settings/builtin.core_settings.pot
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.644041 OpenRadio-1.1.0/OpenRadio/locales/templates/modules/builtin.dab/
+-rw-rw-r--   0 simon     (1000) simon     (1000)     1135 2023-06-25 14:46:56.000000 OpenRadio-1.1.0/OpenRadio/locales/templates/modules/builtin.dab/builtin.dab.pot
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.644041 OpenRadio-1.1.0/OpenRadio/locales/templates/modules/builtin.exit/
+-rw-rw-r--   0 simon     (1000) simon     (1000)      474 2023-06-25 14:41:35.000000 OpenRadio-1.1.0/OpenRadio/locales/templates/modules/builtin.exit/builtin.exit.pot
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.644041 OpenRadio-1.1.0/OpenRadio/locales/templates/modules/builtin.internetradio/
+-rw-rw-r--   0 simon     (1000) simon     (1000)      866 2023-06-25 14:41:35.000000 OpenRadio-1.1.0/OpenRadio/locales/templates/modules/builtin.internetradio/builtin.internetradio.pot
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.644041 OpenRadio-1.1.0/OpenRadio/locales/templates/modules/builtin.settings/
+-rw-rw-r--   0 simon     (1000) simon     (1000)      593 2023-06-25 14:41:35.000000 OpenRadio-1.1.0/OpenRadio/locales/templates/modules/builtin.settings/builtin.settings.pot
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.584042 OpenRadio-1.1.0/OpenRadio/modules/
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.644041 OpenRadio-1.1.0/OpenRadio/modules/About/
+-rw-rw-r--   0 simon     (1000) simon     (1000)     1817 2023-06-29 14:02:04.000000 OpenRadio-1.1.0/OpenRadio/modules/About/__init__.py
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.644041 OpenRadio-1.1.0/OpenRadio/modules/Alarm/
+-rw-rw-r--   0 simon     (1000) simon     (1000)     5289 2023-06-29 14:02:04.000000 OpenRadio-1.1.0/OpenRadio/modules/Alarm/AlarmScheduler.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)     7446 2023-06-29 16:09:04.000000 OpenRadio-1.1.0/OpenRadio/modules/Alarm/AlarmWidget.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)     3145 2023-06-29 14:02:04.000000 OpenRadio-1.1.0/OpenRadio/modules/Alarm/RingUI.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)     3673 2023-06-29 14:02:04.000000 OpenRadio-1.1.0/OpenRadio/modules/Alarm/TimeWidget.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)     6067 2023-06-29 14:02:04.000000 OpenRadio-1.1.0/OpenRadio/modules/Alarm/UI.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)     1403 2023-06-29 14:02:04.000000 OpenRadio-1.1.0/OpenRadio/modules/Alarm/__init__.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)       25 2023-06-25 14:00:14.000000 OpenRadio-1.1.0/OpenRadio/modules/Alarm/const.py
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.644041 OpenRadio-1.1.0/OpenRadio/modules/Clock/
+-rw-rw-r--   0 simon     (1000) simon     (1000)     5055 2023-06-29 14:02:04.000000 OpenRadio-1.1.0/OpenRadio/modules/Clock/__init__.py
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.644041 OpenRadio-1.1.0/OpenRadio/modules/CoreSettings/
+-rw-rw-r--   0 simon     (1000) simon     (1000)     8441 2023-06-29 14:02:04.000000 OpenRadio-1.1.0/OpenRadio/modules/CoreSettings/__init__.py
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.648041 OpenRadio-1.1.0/OpenRadio/modules/DAB/
+-rw-rw-r--   0 simon     (1000) simon     (1000)     5399 2023-06-29 14:02:04.000000 OpenRadio-1.1.0/OpenRadio/modules/DAB/__init__.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)      705 2023-06-29 13:39:28.000000 OpenRadio-1.1.0/OpenRadio/modules/DAB/const.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)     8196 2023-06-29 14:02:04.000000 OpenRadio-1.1.0/OpenRadio/modules/DAB/dab_helper.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)     5752 2023-06-29 14:02:04.000000 OpenRadio-1.1.0/OpenRadio/modules/DAB/player.py
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.648041 OpenRadio-1.1.0/OpenRadio/modules/Exit/
+-rw-rw-r--   0 simon     (1000) simon     (1000)      584 2023-06-29 14:02:04.000000 OpenRadio-1.1.0/OpenRadio/modules/Exit/__init__.py
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.648041 OpenRadio-1.1.0/OpenRadio/modules/InternetRadio/
+-rw-rw-r--   0 simon     (1000) simon     (1000)     2720 2023-06-29 14:02:04.000000 OpenRadio-1.1.0/OpenRadio/modules/InternetRadio/IconThread.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)    16002 2023-06-29 14:02:05.000000 OpenRadio-1.1.0/OpenRadio/modules/InternetRadio/UI.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)     2976 2023-06-29 14:02:04.000000 OpenRadio-1.1.0/OpenRadio/modules/InternetRadio/__init__.py
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.648041 OpenRadio-1.1.0/OpenRadio/modules/Settings/
+-rw-rw-r--   0 simon     (1000) simon     (1000)     2875 2023-06-29 14:02:04.000000 OpenRadio-1.1.0/OpenRadio/modules/Settings/__init__.py
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-29 16:12:38.588042 OpenRadio-1.1.0/OpenRadio.egg-info/
+-rw-rw-r--   0 simon     (1000) simon     (1000)     2254 2023-06-29 16:12:38.000000 OpenRadio-1.1.0/OpenRadio.egg-info/PKG-INFO
+-rw-rw-r--   0 simon     (1000) simon     (1000)    15389 2023-06-29 16:12:38.000000 OpenRadio-1.1.0/OpenRadio.egg-info/SOURCES.txt
+-rw-rw-r--   0 simon     (1000) simon     (1000)        1 2023-06-29 16:12:38.000000 OpenRadio-1.1.0/OpenRadio.egg-info/dependency_links.txt
+-rw-rw-r--   0 simon     (1000) simon     (1000)       42 2023-06-29 16:12:38.000000 OpenRadio-1.1.0/OpenRadio.egg-info/entry_points.txt
+-rw-rw-r--   0 simon     (1000) simon     (1000)      105 2023-06-29 16:12:38.000000 OpenRadio-1.1.0/OpenRadio.egg-info/requires.txt
+-rw-rw-r--   0 simon     (1000) simon     (1000)       10 2023-06-29 16:12:38.000000 OpenRadio-1.1.0/OpenRadio.egg-info/top_level.txt
+-rw-rw-r--   0 simon     (1000) simon     (1000)     2254 2023-06-29 16:12:38.648041 OpenRadio-1.1.0/PKG-INFO
+-rw-rw-r--   0 simon     (1000) simon     (1000)     1614 2023-06-29 16:05:07.000000 OpenRadio-1.1.0/README.md
+-rw-rw-r--   0 simon     (1000) simon     (1000)     1007 2023-06-29 15:56:29.000000 OpenRadio-1.1.0/pyproject.toml
+-rw-rw-r--   0 simon     (1000) simon     (1000)       38 2023-06-29 16:12:38.648041 OpenRadio-1.1.0/setup.cfg
```

### Comparing `OpenRadio-1.0/LICENSE.md` & `OpenRadio-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/LICENSE_Flags.md` & `OpenRadio-1.1.0/LICENSE_Flags.md`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/LICENSE_Icons.md` & `OpenRadio-1.1.0/LICENSE_Icons.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,71 +1,436 @@
-The Icons (alarm-symbolic.svg and globe-symbolic.svg) where taken from the [adwaita](https://gitlab.gnome.org/GNOME/adwaita-icon-theme) project. They are licensed under Commons Attribution-Share Alike 3.0 a copy is provided below.
-The Icons (search-web.png,star-outline.png,star.png,tag-search-outline.png) where taken from the [MaterialDesignIcons] project. They are licensed under Apache 2.0 a copy is provided at the end of this file.
+The Icons (alarm-symbolic.svg,dialog-information.png,go-previous-symbolic.svg,media-playback-pause-symbolic.svg,user-trash-symbolic.svg,application-exit.png,emblem-system.png,go-up-symbolic.svg,media-playback-start-symbolic.svg,applications-internet.png,globe-symbolic.svg,list-add-symbolic.svg,media-playback-stop-symbolic.svg,go-down-symbolic.svg,network-wireless-hotspot-symbolic.svg) where taken from the [yaru](https://github.com/ubuntu/yaru) project. They are licensed under Commons Attribution-Share Alike 4.0 a copy is provided below.
+The Icons (search-web.png,star-outline.png,star.png,tag-search-outline.png) where taken from the [MaterialDesignIcons](https://pictogrammers.com/library/mdi/) project. They are licensed under Apache 2.0 a copy is provided at the end of this file.
 
-# CC-By-3
-THE WORK (AS DEFINED BELOW) IS PROVIDED UNDER THE TERMS OF THIS CREATIVE COMMONS PUBLIC LICENSE ("CCPL" OR "LICENSE"). THE WORK IS PROTECTED BY COPYRIGHT AND/OR OTHER APPLICABLE LAW. ANY USE OF THE WORK OTHER THAN AS AUTHORIZED UNDER THIS LICENSE OR COPYRIGHT LAW IS PROHIBITED.
+# CC-By-4
+Attribution-ShareAlike 4.0 International
 
-BY EXERCISING ANY RIGHTS TO THE WORK PROVIDED HERE, YOU ACCEPT AND AGREE TO BE BOUND BY THE TERMS OF THIS LICENSE. TO THE EXTENT THIS LICENSE MAY BE CONSIDERED TO BE A CONTRACT, THE LICENSOR GRANTS YOU THE RIGHTS CONTAINED HERE IN CONSIDERATION OF YOUR ACCEPTANCE OF SUCH TERMS AND CONDITIONS.
+=======================================================================
 
-1. Definitions
+Creative Commons Corporation ("Creative Commons") is not a law firm and
+does not provide legal services or legal advice. Distribution of
+Creative Commons public licenses does not create a lawyer-client or
+other relationship. Creative Commons makes its licenses and related
+information available on an "as-is" basis. Creative Commons gives no
+warranties regarding its licenses, any material licensed under their
+terms and conditions, or any related information. Creative Commons
+disclaims all liability for damages resulting from their use to the
+fullest extent possible.
+
+Using Creative Commons Public Licenses
+
+Creative Commons public licenses provide a standard set of terms and
+conditions that creators and other rights holders may use to share
+original works of authorship and other material subject to copyright
+and certain other rights specified in the public license below. The
+following considerations are for informational purposes only, are not
+exhaustive, and do not form part of our licenses.
+
+     Considerations for licensors: Our public licenses are
+     intended for use by those authorized to give the public
+     permission to use material in ways otherwise restricted by
+     copyright and certain other rights. Our licenses are
+     irrevocable. Licensors should read and understand the terms
+     and conditions of the license they choose before applying it.
+     Licensors should also secure all rights necessary before
+     applying our licenses so that the public can reuse the
+     material as expected. Licensors should clearly mark any
+     material not subject to the license. This includes other CC-
+     licensed material, or material used under an exception or
+     limitation to copyright. More considerations for licensors:
+	wiki.creativecommons.org/Considerations_for_licensors
+
+     Considerations for the public: By using one of our public
+     licenses, a licensor grants the public permission to use the
+     licensed material under specified terms and conditions. If
+     the licensor's permission is not necessary for any reason--for
+     example, because of any applicable exception or limitation to
+     copyright--then that use is not regulated by the license. Our
+     licenses grant only permissions under copyright and certain
+     other rights that a licensor has authority to grant. Use of
+     the licensed material may still be restricted for other
+     reasons, including because others have copyright or other
+     rights in the material. A licensor may make special requests,
+     such as asking that all changes be marked or described.
+     Although not required by our licenses, you are encouraged to
+     respect those requests where reasonable. More_considerations
+     for the public:
+	wiki.creativecommons.org/Considerations_for_licensees
+
+=======================================================================
+
+Creative Commons Attribution-ShareAlike 4.0 International Public
+License
+
+By exercising the Licensed Rights (defined below), You accept and agree
+to be bound by the terms and conditions of this Creative Commons
+Attribution-ShareAlike 4.0 International Public License ("Public
+License"). To the extent this Public License may be interpreted as a
+contract, You are granted the Licensed Rights in consideration of Your
+acceptance of these terms and conditions, and the Licensor grants You
+such rights in consideration of benefits the Licensor receives from
+making the Licensed Material available under these terms and
+conditions.
+
+
+Section 1 -- Definitions.
+
+  a. Adapted Material means material subject to Copyright and Similar
+     Rights that is derived from or based upon the Licensed Material
+     and in which the Licensed Material is translated, altered,
+     arranged, transformed, or otherwise modified in a manner requiring
+     permission under the Copyright and Similar Rights held by the
+     Licensor. For purposes of this Public License, where the Licensed
+     Material is a musical work, performance, or sound recording,
+     Adapted Material is always produced where the Licensed Material is
+     synched in timed relation with a moving image.
+
+  b. Adapter's License means the license You apply to Your Copyright
+     and Similar Rights in Your contributions to Adapted Material in
+     accordance with the terms and conditions of this Public License.
+
+  c. BY-SA Compatible License means a license listed at
+     creativecommons.org/compatiblelicenses, approved by Creative
+     Commons as essentially the equivalent of this Public License.
+
+  d. Copyright and Similar Rights means copyright and/or similar rights
+     closely related to copyright including, without limitation,
+     performance, broadcast, sound recording, and Sui Generis Database
+     Rights, without regard to how the rights are labeled or
+     categorized. For purposes of this Public License, the rights
+     specified in Section 2(b)(1)-(2) are not Copyright and Similar
+     Rights.
+
+  e. Effective Technological Measures means those measures that, in the
+     absence of proper authority, may not be circumvented under laws
+     fulfilling obligations under Article 11 of the WIPO Copyright
+     Treaty adopted on December 20, 1996, and/or similar international
+     agreements.
+
+  f. Exceptions and Limitations means fair use, fair dealing, and/or
+     any other exception or limitation to Copyright and Similar Rights
+     that applies to Your use of the Licensed Material.
+
+  g. License Elements means the license attributes listed in the name
+     of a Creative Commons Public License. The License Elements of this
+     Public License are Attribution and ShareAlike.
+
+  h. Licensed Material means the artistic or literary work, database,
+     or other material to which the Licensor applied this Public
+     License.
+
+  i. Licensed Rights means the rights granted to You subject to the
+     terms and conditions of this Public License, which are limited to
+     all Copyright and Similar Rights that apply to Your use of the
+     Licensed Material and that the Licensor has authority to license.
+
+  j. Licensor means the individual(s) or entity(ies) granting rights
+     under this Public License.
+
+  k. Share means to provide material to the public by any means or
+     process that requires permission under the Licensed Rights, such
+     as reproduction, public display, public performance, distribution,
+     dissemination, communication, or importation, and to make material
+     available to the public including in ways that members of the
+     public may access the material from a place and at a time
+     individually chosen by them.
+
+  l. Sui Generis Database Rights means rights other than copyright
+     resulting from Directive 96/9/EC of the European Parliament and of
+     the Council of 11 March 1996 on the legal protection of databases,
+     as amended and/or succeeded, as well as other essentially
+     equivalent rights anywhere in the world.
+
+  m. You means the individual or entity exercising the Licensed Rights
+     under this Public License. Your has a corresponding meaning.
+
+
+Section 2 -- Scope.
+
+  a. License grant.
+
+       1. Subject to the terms and conditions of this Public License,
+          the Licensor hereby grants You a worldwide, royalty-free,
+          non-sublicensable, non-exclusive, irrevocable license to
+          exercise the Licensed Rights in the Licensed Material to:
+
+            a. reproduce and Share the Licensed Material, in whole or
+               in part; and
+
+            b. produce, reproduce, and Share Adapted Material.
+
+       2. Exceptions and Limitations. For the avoidance of doubt, where
+          Exceptions and Limitations apply to Your use, this Public
+          License does not apply, and You do not need to comply with
+          its terms and conditions.
+
+       3. Term. The term of this Public License is specified in Section
+          6(a).
+
+       4. Media and formats; technical modifications allowed. The
+          Licensor authorizes You to exercise the Licensed Rights in
+          all media and formats whether now known or hereafter created,
+          and to make technical modifications necessary to do so. The
+          Licensor waives and/or agrees not to assert any right or
+          authority to forbid You from making technical modifications
+          necessary to exercise the Licensed Rights, including
+          technical modifications necessary to circumvent Effective
+          Technological Measures. For purposes of this Public License,
+          simply making modifications authorized by this Section 2(a)
+          (4) never produces Adapted Material.
+
+       5. Downstream recipients.
+
+            a. Offer from the Licensor -- Licensed Material. Every
+               recipient of the Licensed Material automatically
+               receives an offer from the Licensor to exercise the
+               Licensed Rights under the terms and conditions of this
+               Public License.
+
+            b. Additional offer from the Licensor -- Adapted Material.
+               Every recipient of Adapted Material from You
+               automatically receives an offer from the Licensor to
+               exercise the Licensed Rights in the Adapted Material
+               under the conditions of the Adapter's License You apply.
+
+            c. No downstream restrictions. You may not offer or impose
+               any additional or different terms or conditions on, or
+               apply any Effective Technological Measures to, the
+               Licensed Material if doing so restricts exercise of the
+               Licensed Rights by any recipient of the Licensed
+               Material.
+
+       6. No endorsement. Nothing in this Public License constitutes or
+          may be construed as permission to assert or imply that You
+          are, or that Your use of the Licensed Material is, connected
+          with, or sponsored, endorsed, or granted official status by,
+          the Licensor or others designated to receive attribution as
+          provided in Section 3(a)(1)(A)(i).
+
+  b. Other rights.
+
+       1. Moral rights, such as the right of integrity, are not
+          licensed under this Public License, nor are publicity,
+          privacy, and/or other similar personality rights; however, to
+          the extent possible, the Licensor waives and/or agrees not to
+          assert any such rights held by the Licensor to the limited
+          extent necessary to allow You to exercise the Licensed
+          Rights, but not otherwise.
+
+       2. Patent and trademark rights are not licensed under this
+          Public License.
+
+       3. To the extent possible, the Licensor waives any right to
+          collect royalties from You for the exercise of the Licensed
+          Rights, whether directly or through a collecting society
+          under any voluntary or waivable statutory or compulsory
+          licensing scheme. In all other cases the Licensor expressly
+          reserves any right to collect such royalties.
+
+
+Section 3 -- License Conditions.
+
+Your exercise of the Licensed Rights is expressly made subject to the
+following conditions.
+
+  a. Attribution.
+
+       1. If You Share the Licensed Material (including in modified
+          form), You must:
+
+            a. retain the following if it is supplied by the Licensor
+               with the Licensed Material:
+
+                 i. identification of the creator(s) of the Licensed
+                    Material and any others designated to receive
+                    attribution, in any reasonable manner requested by
+                    the Licensor (including by pseudonym if
+                    designated);
+
+                ii. a copyright notice;
+
+               iii. a notice that refers to this Public License;
+
+                iv. a notice that refers to the disclaimer of
+                    warranties;
+
+                 v. a URI or hyperlink to the Licensed Material to the
+                    extent reasonably practicable;
+
+            b. indicate if You modified the Licensed Material and
+               retain an indication of any previous modifications; and
+
+            c. indicate the Licensed Material is licensed under this
+               Public License, and include the text of, or the URI or
+               hyperlink to, this Public License.
+
+       2. You may satisfy the conditions in Section 3(a)(1) in any
+          reasonable manner based on the medium, means, and context in
+          which You Share the Licensed Material. For example, it may be
+          reasonable to satisfy the conditions by providing a URI or
+          hyperlink to a resource that includes the required
+          information.
+
+       3. If requested by the Licensor, You must remove any of the
+          information required by Section 3(a)(1)(A) to the extent
+          reasonably practicable.
+
+  b. ShareAlike.
+
+     In addition to the conditions in Section 3(a), if You Share
+     Adapted Material You produce, the following conditions also apply.
+
+       1. The Adapter's License You apply must be a Creative Commons
+          license with the same License Elements, this version or
+          later, or a BY-SA Compatible License.
+
+       2. You must include the text of, or the URI or hyperlink to, the
+          Adapter's License You apply. You may satisfy this condition
+          in any reasonable manner based on the medium, means, and
+          context in which You Share Adapted Material.
+
+       3. You may not offer or impose any additional or different terms
+          or conditions on, or apply any Effective Technological
+          Measures to, Adapted Material that restrict exercise of the
+          rights granted under the Adapter's License You apply.
+
+
+Section 4 -- Sui Generis Database Rights.
+
+Where the Licensed Rights include Sui Generis Database Rights that
+apply to Your use of the Licensed Material:
+
+  a. for the avoidance of doubt, Section 2(a)(1) grants You the right
+     to extract, reuse, reproduce, and Share all or a substantial
+     portion of the contents of the database;
+
+  b. if You include all or a substantial portion of the database
+     contents in a database in which You have Sui Generis Database
+     Rights, then the database in which You have Sui Generis Database
+     Rights (but not its individual contents) is Adapted Material,
+
+     including for purposes of Section 3(b); and
+  c. You must comply with the conditions in Section 3(a) if You Share
+     all or a substantial portion of the contents of the database.
+
+For the avoidance of doubt, this Section 4 supplements and does not
+replace Your obligations under this Public License where the Licensed
+Rights include other Copyright and Similar Rights.
+
+
+Section 5 -- Disclaimer of Warranties and Limitation of Liability.
+
+  a. UNLESS OTHERWISE SEPARATELY UNDERTAKEN BY THE LICENSOR, TO THE
+     EXTENT POSSIBLE, THE LICENSOR OFFERS THE LICENSED MATERIAL AS-IS
+     AND AS-AVAILABLE, AND MAKES NO REPRESENTATIONS OR WARRANTIES OF
+     ANY KIND CONCERNING THE LICENSED MATERIAL, WHETHER EXPRESS,
+     IMPLIED, STATUTORY, OR OTHER. THIS INCLUDES, WITHOUT LIMITATION,
+     WARRANTIES OF TITLE, MERCHANTABILITY, FITNESS FOR A PARTICULAR
+     PURPOSE, NON-INFRINGEMENT, ABSENCE OF LATENT OR OTHER DEFECTS,
+     ACCURACY, OR THE PRESENCE OR ABSENCE OF ERRORS, WHETHER OR NOT
+     KNOWN OR DISCOVERABLE. WHERE DISCLAIMERS OF WARRANTIES ARE NOT
+     ALLOWED IN FULL OR IN PART, THIS DISCLAIMER MAY NOT APPLY TO YOU.
+
+  b. TO THE EXTENT POSSIBLE, IN NO EVENT WILL THE LICENSOR BE LIABLE
+     TO YOU ON ANY LEGAL THEORY (INCLUDING, WITHOUT LIMITATION,
+     NEGLIGENCE) OR OTHERWISE FOR ANY DIRECT, SPECIAL, INDIRECT,
+     INCIDENTAL, CONSEQUENTIAL, PUNITIVE, EXEMPLARY, OR OTHER LOSSES,
+     COSTS, EXPENSES, OR DAMAGES ARISING OUT OF THIS PUBLIC LICENSE OR
+     USE OF THE LICENSED MATERIAL, EVEN IF THE LICENSOR HAS BEEN
+     ADVISED OF THE POSSIBILITY OF SUCH LOSSES, COSTS, EXPENSES, OR
+     DAMAGES. WHERE A LIMITATION OF LIABILITY IS NOT ALLOWED IN FULL OR
+     IN PART, THIS LIMITATION MAY NOT APPLY TO YOU.
+
+  c. The disclaimer of warranties and limitation of liability provided
+     above shall be interpreted in a manner that, to the extent
+     possible, most closely approximates an absolute disclaimer and
+     waiver of all liability.
+
+
+Section 6 -- Term and Termination.
+
+  a. This Public License applies for the term of the Copyright and
+     Similar Rights licensed here. However, if You fail to comply with
+     this Public License, then Your rights under this Public License
+     terminate automatically.
+
+  b. Where Your right to use the Licensed Material has terminated under
+     Section 6(a), it reinstates:
+
+       1. automatically as of the date the violation is cured, provided
+          it is cured within 30 days of Your discovery of the
+          violation; or
+
+       2. upon express reinstatement by the Licensor.
+
+     For the avoidance of doubt, this Section 6(b) does not affect any
+     right the Licensor may have to seek remedies for Your violations
+     of this Public License.
+
+  c. For the avoidance of doubt, the Licensor may also offer the
+     Licensed Material under separate terms or conditions or stop
+     distributing the Licensed Material at any time; however, doing so
+     will not terminate this Public License.
+
+  d. Sections 1, 5, 6, 7, and 8 survive termination of this Public
+     License.
+
+
+Section 7 -- Other Terms and Conditions.
+
+  a. The Licensor shall not be bound by any additional or different
+     terms or conditions communicated by You unless expressly agreed.
+
+  b. Any arrangements, understandings, or agreements regarding the
+     Licensed Material not stated herein are separate from and
+     independent of the terms and conditions of this Public License.
+
+
+Section 8 -- Interpretation.
+
+  a. For the avoidance of doubt, this Public License does not, and
+     shall not be interpreted to, reduce, limit, restrict, or impose
+     conditions on any use of the Licensed Material that could lawfully
+     be made without permission under this Public License.
+
+  b. To the extent possible, if any provision of this Public License is
+     deemed unenforceable, it shall be automatically reformed to the
+     minimum extent necessary to make it enforceable. If the provision
+     cannot be reformed, it shall be severed from this Public License
+     without affecting the enforceability of the remaining terms and
+     conditions.
+
+  c. No term or condition of this Public License will be waived and no
+     failure to comply consented to unless expressly agreed to by the
+     Licensor.
+
+  d. Nothing in this Public License constitutes or may be interpreted
+     as a limitation upon, or waiver of, any privileges and immunities
+     that apply to the Licensor or You, including from the legal
+     processes of any jurisdiction or authority.
+
+
+=======================================================================
+
+Creative Commons is not a party to its public licenses.
+Notwithstanding, Creative Commons may elect to apply one of its public
+licenses to material it publishes and in those instances will be
+considered the "Licensor." Except for the limited purpose of indicating
+that material is shared under a Creative Commons public license or as
+otherwise permitted by the Creative Commons policies published at
+creativecommons.org/policies, Creative Commons does not authorize the
+use of the trademark "Creative Commons" or any other trademark or logo
+of Creative Commons without its prior written consent including,
+without limitation, in connection with any unauthorized modifications
+to any of its public licenses or any other arrangements,
+understandings, or agreements concerning use of licensed material. For
+the avoidance of doubt, this paragraph does not form part of the public
+licenses.
 
-    "Adaptation" means a work based upon the Work, or upon the Work and other pre-existing works, such as a translation, adaptation, derivative work, arrangement of music or other alterations of a literary or artistic work, or phonogram or performance and includes cinematographic adaptations or any other form in which the Work may be recast, transformed, or adapted including in any form recognizably derived from the original, except that a work that constitutes a Collection will not be considered an Adaptation for the purpose of this License. For the avoidance of doubt, where the Work is a musical work, performance or phonogram, the synchronization of the Work in timed-relation with a moving image ("synching") will be considered an Adaptation for the purpose of this License.
-    "Collection" means a collection of literary or artistic works, such as encyclopedias and anthologies, or performances, phonograms or broadcasts, or other works or subject matter other than works listed in Section 1(f) below, which, by reason of the selection and arrangement of their contents, constitute intellectual creations, in which the Work is included in its entirety in unmodified form along with one or more other contributions, each constituting separate and independent works in themselves, which together are assembled into a collective whole. A work that constitutes a Collection will not be considered an Adaptation (as defined below) for the purposes of this License.
-    "Creative Commons Compatible License" means a license that is listed at https://creativecommons.org/compatiblelicenses that has been approved by Creative Commons as being essentially equivalent to this License, including, at a minimum, because that license: (i) contains terms that have the same purpose, meaning and effect as the License Elements of this License; and, (ii) explicitly permits the relicensing of adaptations of works made available under that license under this License or a Creative Commons jurisdiction license with the same License Elements as this License.
-    "Distribute" means to make available to the public the original and copies of the Work or Adaptation, as appropriate, through sale or other transfer of ownership.
-    "License Elements" means the following high-level license attributes as selected by Licensor and indicated in the title of this License: Attribution, ShareAlike.
-    "Licensor" means the individual, individuals, entity or entities that offer(s) the Work under the terms of this License.
-    "Original Author" means, in the case of a literary or artistic work, the individual, individuals, entity or entities who created the Work or if no individual or entity can be identified, the publisher; and in addition (i) in the case of a performance the actors, singers, musicians, dancers, and other persons who act, sing, deliver, declaim, play in, interpret or otherwise perform literary or artistic works or expressions of folklore; (ii) in the case of a phonogram the producer being the person or legal entity who first fixes the sounds of a performance or other sounds; and, (iii) in the case of broadcasts, the organization that transmits the broadcast.
-    "Work" means the literary and/or artistic work offered under the terms of this License including without limitation any production in the literary, scientific and artistic domain, whatever may be the mode or form of its expression including digital form, such as a book, pamphlet and other writing; a lecture, address, sermon or other work of the same nature; a dramatic or dramatico-musical work; a choreographic work or entertainment in dumb show; a musical composition with or without words; a cinematographic work to which are assimilated works expressed by a process analogous to cinematography; a work of drawing, painting, architecture, sculpture, engraving or lithography; a photographic work to which are assimilated works expressed by a process analogous to photography; a work of applied art; an illustration, map, plan, sketch or three-dimensional work relative to geography, topography, architecture or science; a performance; a broadcast; a phonogram; a compilation of data to the extent it is protected as a copyrightable work; or a work performed by a variety or circus performer to the extent it is not otherwise considered a literary or artistic work.
-    "You" means an individual or entity exercising rights under this License who has not previously violated the terms of this License with respect to the Work, or who has received express permission from the Licensor to exercise rights under this License despite a previous violation.
-    "Publicly Perform" means to perform public recitations of the Work and to communicate to the public those public recitations, by any means or process, including by wire or wireless means or public digital performances; to make available to the public Works in such a way that members of the public may access these Works from a place and at a place individually chosen by them; to perform the Work to the public by any means or process and the communication to the public of the performances of the Work, including by public digital performance; to broadcast and rebroadcast the Work by any means including signs, sounds or images.
-    "Reproduce" means to make copies of the Work by any means including without limitation by sound or visual recordings and the right of fixation and reproducing fixations of the Work, including storage of a protected performance or phonogram in digital form or other electronic medium.
-
-2. Fair Dealing Rights. Nothing in this License is intended to reduce, limit, or restrict any uses free from copyright or rights arising from limitations or exceptions that are provided for in connection with the copyright protection under copyright law or other applicable laws.
-
-3. License Grant. Subject to the terms and conditions of this License, Licensor hereby grants You a worldwide, royalty-free, non-exclusive, perpetual (for the duration of the applicable copyright) license to exercise the rights in the Work as stated below:
-
-    to Reproduce the Work, to incorporate the Work into one or more Collections, and to Reproduce the Work as incorporated in the Collections;
-    to create and Reproduce Adaptations provided that any such Adaptation, including any translation in any medium, takes reasonable steps to clearly label, demarcate or otherwise identify that changes were made to the original Work. For example, a translation could be marked "The original work was translated from English to Spanish," or a modification could indicate "The original work has been modified.";
-    to Distribute and Publicly Perform the Work including as incorporated in Collections; and,
-    to Distribute and Publicly Perform Adaptations.
-
-    For the avoidance of doubt:
-        Non-waivable Compulsory License Schemes. In those jurisdictions in which the right to collect royalties through any statutory or compulsory licensing scheme cannot be waived, the Licensor reserves the exclusive right to collect such royalties for any exercise by You of the rights granted under this License;
-        Waivable Compulsory License Schemes. In those jurisdictions in which the right to collect royalties through any statutory or compulsory licensing scheme can be waived, the Licensor waives the exclusive right to collect such royalties for any exercise by You of the rights granted under this License; and,
-        Voluntary License Schemes. The Licensor waives the right to collect royalties, whether individually or, in the event that the Licensor is a member of a collecting society that administers voluntary licensing schemes, via that society, from any exercise by You of the rights granted under this License.
-
-The above rights may be exercised in all media and formats whether now known or hereafter devised. The above rights include the right to make such modifications as are technically necessary to exercise the rights in other media and formats. Subject to Section 8(f), all rights not expressly granted by Licensor are hereby reserved.
-
-4. Restrictions. The license granted in Section 3 above is expressly made subject to and limited by the following restrictions:
-
-    You may Distribute or Publicly Perform the Work only under the terms of this License. You must include a copy of, or the Uniform Resource Identifier (URI) for, this License with every copy of the Work You Distribute or Publicly Perform. You may not offer or impose any terms on the Work that restrict the terms of this License or the ability of the recipient of the Work to exercise the rights granted to that recipient under the terms of the License. You may not sublicense the Work. You must keep intact all notices that refer to this License and to the disclaimer of warranties with every copy of the Work You Distribute or Publicly Perform. When You Distribute or Publicly Perform the Work, You may not impose any effective technological measures on the Work that restrict the ability of a recipient of the Work from You to exercise the rights granted to that recipient under the terms of the License. This Section 4(a) applies to the Work as incorporated in a Collection, but this does not require the Collection apart from the Work itself to be made subject to the terms of this License. If You create a Collection, upon notice from any Licensor You must, to the extent practicable, remove from the Collection any credit as required by Section 4(c), as requested. If You create an Adaptation, upon notice from any Licensor You must, to the extent practicable, remove from the Adaptation any credit as required by Section 4(c), as requested.
-    You may Distribute or Publicly Perform an Adaptation only under the terms of: (i) this License; (ii) a later version of this License with the same License Elements as this License; (iii) a Creative Commons jurisdiction license (either this or a later license version) that contains the same License Elements as this License (e.g., Attribution-ShareAlike 3.0 US)); (iv) a Creative Commons Compatible License. If you license the Adaptation under one of the licenses mentioned in (iv), you must comply with the terms of that license. If you license the Adaptation under the terms of any of the licenses mentioned in (i), (ii) or (iii) (the "Applicable License"), you must comply with the terms of the Applicable License generally and the following provisions: (I) You must include a copy of, or the URI for, the Applicable License with every copy of each Adaptation You Distribute or Publicly Perform; (II) You may not offer or impose any terms on the Adaptation that restrict the terms of the Applicable License or the ability of the recipient of the Adaptation to exercise the rights granted to that recipient under the terms of the Applicable License; (III) You must keep intact all notices that refer to the Applicable License and to the disclaimer of warranties with every copy of the Work as included in the Adaptation You Distribute or Publicly Perform; (IV) when You Distribute or Publicly Perform the Adaptation, You may not impose any effective technological measures on the Adaptation that restrict the ability of a recipient of the Adaptation from You to exercise the rights granted to that recipient under the terms of the Applicable License. This Section 4(b) applies to the Adaptation as incorporated in a Collection, but this does not require the Collection apart from the Adaptation itself to be made subject to the terms of the Applicable License.
-    If You Distribute, or Publicly Perform the Work or any Adaptations or Collections, You must, unless a request has been made pursuant to Section 4(a), keep intact all copyright notices for the Work and provide, reasonable to the medium or means You are utilizing: (i) the name of the Original Author (or pseudonym, if applicable) if supplied, and/or if the Original Author and/or Licensor designate another party or parties (e.g., a sponsor institute, publishing entity, journal) for attribution ("Attribution Parties") in Licensor's copyright notice, terms of service or by other reasonable means, the name of such party or parties; (ii) the title of the Work if supplied; (iii) to the extent reasonably practicable, the URI, if any, that Licensor specifies to be associated with the Work, unless such URI does not refer to the copyright notice or licensing information for the Work; and (iv) , consistent with Ssection 3(b), in the case of an Adaptation, a credit identifying the use of the Work in the Adaptation (e.g., "French translation of the Work by Original Author," or "Screenplay based on original Work by Original Author"). The credit required by this Section 4(c) may be implemented in any reasonable manner; provided, however, that in the case of a Adaptation or Collection, at a minimum such credit will appear, if a credit for all contributing authors of the Adaptation or Collection appears, then as part of these credits and in a manner at least as prominent as the credits for the other contributing authors. For the avoidance of doubt, You may only use the credit required by this Section for the purpose of attribution in the manner set out above and, by exercising Your rights under this License, You may not implicitly or explicitly assert or imply any connection with, sponsorship or endorsement by the Original Author, Licensor and/or Attribution Parties, as appropriate, of You or Your use of the Work, without the separate, express prior written permission of the Original Author, Licensor and/or Attribution Parties.
-    Except as otherwise agreed in writing by the Licensor or as may be otherwise permitted by applicable law, if You Reproduce, Distribute or Publicly Perform the Work either by itself or as part of any Adaptations or Collections, You must not distort, mutilate, modify or take other derogatory action in relation to the Work which would be prejudicial to the Original Author's honor or reputation. Licensor agrees that in those jurisdictions (e.g. Japan), in which any exercise of the right granted in Section 3(b) of this License (the right to make Adaptations) would be deemed to be a distortion, mutilation, modification or other derogatory action prejudicial to the Original Author's honor and reputation, the Licensor will waive or not assert, as appropriate, this Section, to the fullest extent permitted by the applicable national law, to enable You to reasonably exercise Your right under Section 3(b) of this License (right to make Adaptations) but not otherwise.
-
-5. Representations, Warranties and Disclaimer
-
-UNLESS OTHERWISE MUTUALLY AGREED TO BY THE PARTIES IN WRITING, LICENSOR OFFERS THE WORK AS-IS AND MAKES NO REPRESENTATIONS OR WARRANTIES OF ANY KIND CONCERNING THE WORK, EXPRESS, IMPLIED, STATUTORY OR OTHERWISE, INCLUDING, WITHOUT LIMITATION, WARRANTIES OF TITLE, MERCHANTIBILITY, FITNESS FOR A PARTICULAR PURPOSE, NONINFRINGEMENT, OR THE ABSENCE OF LATENT OR OTHER DEFECTS, ACCURACY, OR THE PRESENCE OF ABSENCE OF ERRORS, WHETHER OR NOT DISCOVERABLE. SOME JURISDICTIONS DO NOT ALLOW THE EXCLUSION OF IMPLIED WARRANTIES, SO SUCH EXCLUSION MAY NOT APPLY TO YOU.
-
-6. Limitation on Liability. EXCEPT TO THE EXTENT REQUIRED BY APPLICABLE LAW, IN NO EVENT WILL LICENSOR BE LIABLE TO YOU ON ANY LEGAL THEORY FOR ANY SPECIAL, INCIDENTAL, CONSEQUENTIAL, PUNITIVE OR EXEMPLARY DAMAGES ARISING OUT OF THIS LICENSE OR THE USE OF THE WORK, EVEN IF LICENSOR HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGES.
-
-7. Termination
-
-    This License and the rights granted hereunder will terminate automatically upon any breach by You of the terms of this License. Individuals or entities who have received Adaptations or Collections from You under this License, however, will not have their licenses terminated provided such individuals or entities remain in full compliance with those licenses. Sections 1, 2, 5, 6, 7, and 8 will survive any termination of this License.
-    Subject to the above terms and conditions, the license granted here is perpetual (for the duration of the applicable copyright in the Work). Notwithstanding the above, Licensor reserves the right to release the Work under different license terms or to stop distributing the Work at any time; provided, however that any such election will not serve to withdraw this License (or any other license that has been, or is required to be, granted under the terms of this License), and this License will continue in full force and effect unless terminated as stated above.
-
-8. Miscellaneous
-
-    Each time You Distribute or Publicly Perform the Work or a Collection, the Licensor offers to the recipient a license to the Work on the same terms and conditions as the license granted to You under this License.
-    Each time You Distribute or Publicly Perform an Adaptation, Licensor offers to the recipient a license to the original Work on the same terms and conditions as the license granted to You under this License.
-    If any provision of this License is invalid or unenforceable under applicable law, it shall not affect the validity or enforceability of the remainder of the terms of this License, and without further action by the parties to this agreement, such provision shall be reformed to the minimum extent necessary to make such provision valid and enforceable.
-    No term or provision of this License shall be deemed waived and no breach consented to unless such waiver or consent shall be in writing and signed by the party to be charged with such waiver or consent.
-    This License constitutes the entire agreement between the parties with respect to the Work licensed here. There are no understandings, agreements or representations with respect to the Work not specified here. Licensor shall not be bound by any additional provisions that may appear in any communication from You. This License may not be modified without the mutual written agreement of the Licensor and You.
-    The rights granted under, and the subject matter referenced, in this License were drafted utilizing the terminology of the Berne Convention for the Protection of Literary and Artistic Works (as amended on September 28, 1979), the Rome Convention of 1961, the WIPO Copyright Treaty of 1996, the WIPO Performances and Phonograms Treaty of 1996 and the Universal Copyright Convention (as revised on July 24, 1971). These rights and subject matter take effect in the relevant jurisdiction in which the License terms are sought to be enforced according to the corresponding provisions of the implementation of those treaty provisions in the applicable national law. If the standard suite of rights granted under applicable copyright law includes additional rights not granted under this License, such additional rights are deemed to be included in the License; this License is not intended to restrict the license of any rights under applicable law.
+Creative Commons may be contacted at creativecommons.org.
 
 # Apache 2.0
                             Apache License
                            Version 2.0, January 2004
                         http://www.apache.org/licenses/
 
    TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `OpenRadio-1.0/OpenRadio/assets/OpenRadio.icon` & `OpenRadio-1.1.0/OpenRadio/assets/OpenRadio.icon`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/bitmap.png` & `OpenRadio-1.1.0/OpenRadio/assets/OpenRadio.png`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/alarm-symbolic.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/alarm-symbolic.svg`

 * *Files 1% similar despite different names*

```diff
@@ -1,113 +1,112 @@
 00000000: 3c73 7667 2076 6965 7742 6f78 3d22 3020  <svg viewBox="0 
 00000010: 3020 3136 2031 3622 2078 6d6c 6e73 3d22  0 16 16" xmlns="
 00000020: 6874 7470 3a2f 2f77 7777 2e77 332e 6f72  http://www.w3.or
 00000030: 672f 3230 3030 2f73 7667 223e 0a20 3c67  g/2000/svg">. <g
-00000040: 2066 696c 6c3d 2277 6869 7465 223e 0a20   fill="white">. 
-00000050: 203c 7061 7468 2064 3d22 4d31 322e 3433   <path d="M12.43
-00000060: 3620 3132 2e37 3036 6330 202e 3030 332e  6 12.706c0 .003.
-00000070: 3031 2e30 3036 2e30 312e 3031 2030 202e  01.006.01.01 0 .
-00000080: 3030 352e 3031 2e30 312e 3031 2e30 3135  005.01.01.01.015
-00000090: 7a4d 332e 3535 3720 3132 2e37 3038 6c2d  zM3.557 12.708l-
-000000a0: 2e30 322e 3032 3663 302d 2e30 3035 2e30  .02.026c0-.005.0
-000000b0: 312d 2e30 312e 3031 2d2e 3031 3520 302d  1-.01.01-.015 0-
-000000c0: 2e30 3033 2e30 312d 2e30 3036 2e30 312d  .003.01-.006.01-
-000000d0: 2e30 317a 2220 666f 6e74 2d66 616d 696c  .01z" font-famil
-000000e0: 793d 2255 6275 6e74 7522 2066 6f6e 742d  y="Ubuntu" font-
-000000f0: 7369 7a65 3d22 3135 2220 666f 6e74 2d77  size="15" font-w
-00000100: 6569 6768 743d 2234 3030 2220 6c65 7474  eight="400" lett
-00000110: 6572 2d73 7061 6369 6e67 3d22 3022 2074  er-spacing="0" t
-00000120: 6578 742d 616e 6368 6f72 3d22 6d69 6464  ext-anchor="midd
-00000130: 6c65 2220 776f 7264 2d73 7061 6369 6e67  le" word-spacing
-00000140: 3d22 3022 2f3e 0a20 203c 7061 7468 2064  ="0"/>.  <path d
-00000150: 3d22 4d38 2030 4333 2e35 3837 2030 2030  ="M8 0C3.587 0 0
-00000160: 2033 2e35 3837 2030 2038 7333 2e35 3837   3.587 0 8s3.587
-00000170: 2038 2038 2038 6334 2e34 3134 2030 2038   8 8 8c4.414 0 8
-00000180: 2d33 2e35 3837 2038 2d38 732d 332e 3538  -3.587 8-8s-3.58
-00000190: 362d 382d 382d 387a 6d30 2031 6137 2037  6-8-8-8zm0 1a7 7
-000001a0: 2030 2030 2031 2037 2037 2037 2037 2030   0 0 1 7 7 7 7 0
-000001b0: 2030 2031 2d37 2037 2037 2037 2030 2030   0 1-7 7 7 7 0 0
-000001c0: 2031 2d37 2d37 2037 2037 2030 2030 2031   1-7-7 7 7 0 0 1
-000001d0: 2037 2d37 7a22 2066 6f6e 742d 6661 6d69   7-7z" font-fami
-000001e0: 6c79 3d22 7361 6e73 2d73 6572 6966 2220  ly="sans-serif" 
-000001f0: 666f 6e74 2d77 6569 6768 743d 2234 3030  font-weight="400
-00000200: 2220 6f76 6572 666c 6f77 3d22 7669 7369  " overflow="visi
-00000210: 626c 6522 2073 7479 6c65 3d22 666f 6e74  ble" style="font
-00000220: 2d66 6561 7475 7265 2d73 6574 7469 6e67  -feature-setting
-00000230: 733a 6e6f 726d 616c 3b66 6f6e 742d 7661  s:normal;font-va
-00000240: 7269 616e 742d 616c 7465 726e 6174 6573  riant-alternates
-00000250: 3a6e 6f72 6d61 6c3b 666f 6e74 2d76 6172  :normal;font-var
-00000260: 6961 6e74 2d63 6170 733a 6e6f 726d 616c  iant-caps:normal
-00000270: 3b66 6f6e 742d 7661 7269 616e 742d 6c69  ;font-variant-li
-00000280: 6761 7475 7265 733a 6e6f 6e65 3b66 6f6e  gatures:none;fon
-00000290: 742d 7661 7269 616e 742d 6e75 6d65 7269  t-variant-numeri
-000002a0: 633a 6e6f 726d 616c 3b66 6f6e 742d 7661  c:normal;font-va
-000002b0: 7269 616e 742d 706f 7369 7469 6f6e 3a6e  riant-position:n
-000002c0: 6f72 6d61 6c3b 6973 6f6c 6174 696f 6e3a  ormal;isolation:
-000002d0: 6175 746f 3b6d 6978 2d62 6c65 6e64 2d6d  auto;mix-blend-m
-000002e0: 6f64 653a 6e6f 726d 616c 3b73 6861 7065  ode:normal;shape
-000002f0: 2d70 6164 6469 6e67 3a30 3b74 6578 742d  -padding:0;text-
-00000300: 6465 636f 7261 7469 6f6e 2d63 6f6c 6f72  decoration-color
-00000310: 3a23 3030 303b 7465 7874 2d64 6563 6f72  :#000;text-decor
-00000320: 6174 696f 6e2d 6c69 6e65 3a6e 6f6e 653b  ation-line:none;
-00000330: 7465 7874 2d64 6563 6f72 6174 696f 6e2d  text-decoration-
-00000340: 7374 796c 653a 736f 6c69 643b 7465 7874  style:solid;text
-00000350: 2d69 6e64 656e 743a 303b 7465 7874 2d74  -indent:0;text-t
-00000360: 7261 6e73 666f 726d 3a6e 6f6e 6522 2077  ransform:none" w
-00000370: 6869 7465 2d73 7061 6365 3d22 6e6f 726d  hite-space="norm
-00000380: 616c 222f 3e0a 2020 3c70 6174 6820 643d  al"/>.  <path d=
-00000390: 224d 3134 2e37 3337 2031 2e32 3633 632d  "M14.737 1.263c-
-000003a0: 312e 3638 342d 312e 3638 342d 322e 3532  1.684-1.684-2.52
-000003b0: 362d 312e 3638 342d 342e 3231 2030 6c2d  6-1.684-4.21 0l-
-000003c0: 2e31 352e 3135 6135 2e39 3534 2035 2e39  .15.15a5.954 5.9
-000003d0: 3534 2030 2030 2031 2032 2e36 3736 2031  54 0 0 1 2.676 1
-000003e0: 2e35 3334 2035 2e39 3536 2035 2e39 3536  .534 5.956 5.956
-000003f0: 2030 2030 2031 2031 2e35 3336 2032 2e36   0 0 1 1.536 2.6
-00000400: 3734 6c2e 3134 382d 2e31 3437 6331 2e36  74l.148-.147c1.6
-00000410: 3834 2d31 2e36 3835 2031 2e36 3834 2d32  84-1.685 1.684-2
-00000420: 2e35 3237 2030 2d34 2e32 317a 4d31 2e32  .527 0-4.21zM1.2
-00000430: 3633 2031 2e32 3633 632d 312e 3638 3420  63 1.263c-1.684 
-00000440: 312e 3638 342d 312e 3638 3420 322e 3532  1.684-1.684 2.52
-00000450: 3620 3020 342e 3231 6c2e 3135 2e31 3561  6 0 4.21l.15.15a
-00000460: 352e 3935 3520 352e 3935 3520 3020 3020  5.955 5.955 0 0 
-00000470: 3120 312e 3533 342d 322e 3637 3620 352e  1 1.534-2.676 5.
-00000480: 3935 3520 352e 3935 3520 3020 3020 3120  955 5.955 0 0 1 
-00000490: 322e 3637 342d 312e 3533 366c 2d2e 3134  2.674-1.536l-.14
-000004a0: 372d 2e31 3438 4333 2e37 392d 2e34 3220  7-.148C3.79-.42 
-000004b0: 322e 3934 372d 2e34 3220 312e 3236 3420  2.947-.42 1.264 
-000004c0: 312e 3236 337a 2220 6f76 6572 666c 6f77  1.263z" overflow
-000004d0: 3d22 7669 7369 626c 6522 2f3e 0a20 203c  ="visible"/>.  <
-000004e0: 7061 7468 2064 3d22 4d37 2e35 2033 7635  path d="M7.5 3v5
-000004f0: 2e32 3037 6c33 2e31 3436 2033 2e31 3437  .207l3.146 3.147
-00000500: 2e37 3037 2d2e 3730 384c 382e 3520 372e  .707-.708L8.5 7.
-00000510: 3739 3356 337a 2220 6669 6c6c 2d72 756c  793V3z" fill-rul
-00000520: 653d 2265 7665 6e6f 6464 2220 666f 6e74  e="evenodd" font
-00000530: 2d66 616d 696c 793d 2273 616e 732d 7365  -family="sans-se
-00000540: 7269 6622 2066 6f6e 742d 7765 6967 6874  rif" font-weight
-00000550: 3d22 3430 3022 206f 7665 7266 6c6f 773d  ="400" overflow=
-00000560: 2276 6973 6962 6c65 2220 7374 796c 653d  "visible" style=
-00000570: 2266 6f6e 742d 6665 6174 7572 652d 7365  "font-feature-se
-00000580: 7474 696e 6773 3a6e 6f72 6d61 6c3b 666f  ttings:normal;fo
-00000590: 6e74 2d76 6172 6961 6e74 2d61 6c74 6572  nt-variant-alter
-000005a0: 6e61 7465 733a 6e6f 726d 616c 3b66 6f6e  nates:normal;fon
-000005b0: 742d 7661 7269 616e 742d 6361 7073 3a6e  t-variant-caps:n
-000005c0: 6f72 6d61 6c3b 666f 6e74 2d76 6172 6961  ormal;font-varia
-000005d0: 6e74 2d6c 6967 6174 7572 6573 3a6e 6f72  nt-ligatures:nor
-000005e0: 6d61 6c3b 666f 6e74 2d76 6172 6961 6e74  mal;font-variant
-000005f0: 2d6e 756d 6572 6963 3a6e 6f72 6d61 6c3b  -numeric:normal;
-00000600: 666f 6e74 2d76 6172 6961 6e74 2d70 6f73  font-variant-pos
-00000610: 6974 696f 6e3a 6e6f 726d 616c 3b69 736f  ition:normal;iso
-00000620: 6c61 7469 6f6e 3a61 7574 6f3b 6d69 782d  lation:auto;mix-
-00000630: 626c 656e 642d 6d6f 6465 3a6e 6f72 6d61  blend-mode:norma
-00000640: 6c3b 7368 6170 652d 7061 6464 696e 673a  l;shape-padding:
-00000650: 303b 7465 7874 2d64 6563 6f72 6174 696f  0;text-decoratio
-00000660: 6e2d 636f 6c6f 723a 2330 3030 3b74 6578  n-color:#000;tex
-00000670: 742d 6465 636f 7261 7469 6f6e 2d6c 696e  t-decoration-lin
-00000680: 653a 6e6f 6e65 3b74 6578 742d 6465 636f  e:none;text-deco
-00000690: 7261 7469 6f6e 2d73 7479 6c65 3a73 6f6c  ration-style:sol
-000006a0: 6964 3b74 6578 742d 696e 6465 6e74 3a30  id;text-indent:0
-000006b0: 3b74 6578 742d 6f72 6965 6e74 6174 696f  ;text-orientatio
-000006c0: 6e3a 6d69 7865 643b 7465 7874 2d74 7261  n:mixed;text-tra
-000006d0: 6e73 666f 726d 3a6e 6f6e 6522 2077 6869  nsform:none" whi
-000006e0: 7465 2d73 7061 6365 3d22 6e6f 726d 616c  te-space="normal
-000006f0: 222f 3e0a 203c 2f67 3e0a 3c2f 7376 673e  "/>. </g>.</svg>
-00000700: 0a                                       .
+00000040: 2066 696c 6c3d 2267 7261 7922 3e0a 2020   fill="gray">.  
+00000050: 3c70 6174 6820 643d 224d 3132 2e34 3336  <path d="M12.436
+00000060: 2031 322e 3730 3663 3020 2e30 3033 2e30   12.706c0 .003.0
+00000070: 312e 3030 362e 3031 2e30 3120 3020 2e30  1.006.01.01 0 .0
+00000080: 3035 2e30 312e 3031 2e30 312e 3031 357a  05.01.01.01.015z
+00000090: 4d33 2e35 3537 2031 322e 3730 386c 2d2e  M3.557 12.708l-.
+000000a0: 3032 2e30 3236 6330 2d2e 3030 352e 3031  02.026c0-.005.01
+000000b0: 2d2e 3031 2e30 312d 2e30 3135 2030 2d2e  -.01.01-.015 0-.
+000000c0: 3030 332e 3031 2d2e 3030 362e 3031 2d2e  003.01-.006.01-.
+000000d0: 3031 7a22 2066 6f6e 742d 6661 6d69 6c79  01z" font-family
+000000e0: 3d22 5562 756e 7475 2220 666f 6e74 2d73  ="Ubuntu" font-s
+000000f0: 697a 653d 2231 3522 2066 6f6e 742d 7765  ize="15" font-we
+00000100: 6967 6874 3d22 3430 3022 206c 6574 7465  ight="400" lette
+00000110: 722d 7370 6163 696e 673d 2230 2220 7465  r-spacing="0" te
+00000120: 7874 2d61 6e63 686f 723d 226d 6964 646c  xt-anchor="middl
+00000130: 6522 2077 6f72 642d 7370 6163 696e 673d  e" word-spacing=
+00000140: 2230 222f 3e0a 2020 3c70 6174 6820 643d  "0"/>.  <path d=
+00000150: 224d 3820 3043 332e 3538 3720 3020 3020  "M8 0C3.587 0 0 
+00000160: 332e 3538 3720 3020 3873 332e 3538 3720  3.587 0 8s3.587 
+00000170: 3820 3820 3863 342e 3431 3420 3020 382d  8 8 8c4.414 0 8-
+00000180: 332e 3538 3720 382d 3873 2d33 2e35 3836  3.587 8-8s-3.586
+00000190: 2d38 2d38 2d38 7a6d 3020 3161 3720 3720  -8-8-8zm0 1a7 7 
+000001a0: 3020 3020 3120 3720 3720 3720 3720 3020  0 0 1 7 7 7 7 0 
+000001b0: 3020 312d 3720 3720 3720 3720 3020 3020  0 1-7 7 7 7 0 0 
+000001c0: 312d 372d 3720 3720 3720 3020 3020 3120  1-7-7 7 7 0 0 1 
+000001d0: 372d 377a 2220 666f 6e74 2d66 616d 696c  7-7z" font-famil
+000001e0: 793d 2273 616e 732d 7365 7269 6622 2066  y="sans-serif" f
+000001f0: 6f6e 742d 7765 6967 6874 3d22 3430 3022  ont-weight="400"
+00000200: 206f 7665 7266 6c6f 773d 2276 6973 6962   overflow="visib
+00000210: 6c65 2220 7374 796c 653d 2266 6f6e 742d  le" style="font-
+00000220: 6665 6174 7572 652d 7365 7474 696e 6773  feature-settings
+00000230: 3a6e 6f72 6d61 6c3b 666f 6e74 2d76 6172  :normal;font-var
+00000240: 6961 6e74 2d61 6c74 6572 6e61 7465 733a  iant-alternates:
+00000250: 6e6f 726d 616c 3b66 6f6e 742d 7661 7269  normal;font-vari
+00000260: 616e 742d 6361 7073 3a6e 6f72 6d61 6c3b  ant-caps:normal;
+00000270: 666f 6e74 2d76 6172 6961 6e74 2d6c 6967  font-variant-lig
+00000280: 6174 7572 6573 3a6e 6f6e 653b 666f 6e74  atures:none;font
+00000290: 2d76 6172 6961 6e74 2d6e 756d 6572 6963  -variant-numeric
+000002a0: 3a6e 6f72 6d61 6c3b 666f 6e74 2d76 6172  :normal;font-var
+000002b0: 6961 6e74 2d70 6f73 6974 696f 6e3a 6e6f  iant-position:no
+000002c0: 726d 616c 3b69 736f 6c61 7469 6f6e 3a61  rmal;isolation:a
+000002d0: 7574 6f3b 6d69 782d 626c 656e 642d 6d6f  uto;mix-blend-mo
+000002e0: 6465 3a6e 6f72 6d61 6c3b 7368 6170 652d  de:normal;shape-
+000002f0: 7061 6464 696e 673a 303b 7465 7874 2d64  padding:0;text-d
+00000300: 6563 6f72 6174 696f 6e2d 636f 6c6f 723a  ecoration-color:
+00000310: 2330 3030 3b74 6578 742d 6465 636f 7261  #000;text-decora
+00000320: 7469 6f6e 2d6c 696e 653a 6e6f 6e65 3b74  tion-line:none;t
+00000330: 6578 742d 6465 636f 7261 7469 6f6e 2d73  ext-decoration-s
+00000340: 7479 6c65 3a73 6f6c 6964 3b74 6578 742d  tyle:solid;text-
+00000350: 696e 6465 6e74 3a30 3b74 6578 742d 7472  indent:0;text-tr
+00000360: 616e 7366 6f72 6d3a 6e6f 6e65 2220 7768  ansform:none" wh
+00000370: 6974 652d 7370 6163 653d 226e 6f72 6d61  ite-space="norma
+00000380: 6c22 2f3e 0a20 203c 7061 7468 2064 3d22  l"/>.  <path d="
+00000390: 4d31 342e 3733 3720 312e 3236 3363 2d31  M14.737 1.263c-1
+000003a0: 2e36 3834 2d31 2e36 3834 2d32 2e35 3236  .684-1.684-2.526
+000003b0: 2d31 2e36 3834 2d34 2e32 3120 306c 2d2e  -1.684-4.21 0l-.
+000003c0: 3135 2e31 3561 352e 3935 3420 352e 3935  15.15a5.954 5.95
+000003d0: 3420 3020 3020 3120 322e 3637 3620 312e  4 0 0 1 2.676 1.
+000003e0: 3533 3420 352e 3935 3620 352e 3935 3620  534 5.956 5.956 
+000003f0: 3020 3020 3120 312e 3533 3620 322e 3637  0 0 1 1.536 2.67
+00000400: 346c 2e31 3438 2d2e 3134 3763 312e 3638  4l.148-.147c1.68
+00000410: 342d 312e 3638 3520 312e 3638 342d 322e  4-1.685 1.684-2.
+00000420: 3532 3720 302d 342e 3231 7a4d 312e 3236  527 0-4.21zM1.26
+00000430: 3320 312e 3236 3363 2d31 2e36 3834 2031  3 1.263c-1.684 1
+00000440: 2e36 3834 2d31 2e36 3834 2032 2e35 3236  .684-1.684 2.526
+00000450: 2030 2034 2e32 316c 2e31 352e 3135 6135   0 4.21l.15.15a5
+00000460: 2e39 3535 2035 2e39 3535 2030 2030 2031  .955 5.955 0 0 1
+00000470: 2031 2e35 3334 2d32 2e36 3736 2035 2e39   1.534-2.676 5.9
+00000480: 3535 2035 2e39 3535 2030 2030 2031 2032  55 5.955 0 0 1 2
+00000490: 2e36 3734 2d31 2e35 3336 6c2d 2e31 3437  .674-1.536l-.147
+000004a0: 2d2e 3134 3843 332e 3739 2d2e 3432 2032  -.148C3.79-.42 2
+000004b0: 2e39 3437 2d2e 3432 2031 2e32 3634 2031  .947-.42 1.264 1
+000004c0: 2e32 3633 7a22 206f 7665 7266 6c6f 773d  .263z" overflow=
+000004d0: 2276 6973 6962 6c65 222f 3e0a 2020 3c70  "visible"/>.  <p
+000004e0: 6174 6820 643d 224d 372e 3520 3376 352e  ath d="M7.5 3v5.
+000004f0: 3230 376c 332e 3134 3620 332e 3134 372e  207l3.146 3.147.
+00000500: 3730 372d 2e37 3038 4c38 2e35 2037 2e37  707-.708L8.5 7.7
+00000510: 3933 5633 7a22 2066 696c 6c2d 7275 6c65  93V3z" fill-rule
+00000520: 3d22 6576 656e 6f64 6422 2066 6f6e 742d  ="evenodd" font-
+00000530: 6661 6d69 6c79 3d22 7361 6e73 2d73 6572  family="sans-ser
+00000540: 6966 2220 666f 6e74 2d77 6569 6768 743d  if" font-weight=
+00000550: 2234 3030 2220 6f76 6572 666c 6f77 3d22  "400" overflow="
+00000560: 7669 7369 626c 6522 2073 7479 6c65 3d22  visible" style="
+00000570: 666f 6e74 2d66 6561 7475 7265 2d73 6574  font-feature-set
+00000580: 7469 6e67 733a 6e6f 726d 616c 3b66 6f6e  tings:normal;fon
+00000590: 742d 7661 7269 616e 742d 616c 7465 726e  t-variant-altern
+000005a0: 6174 6573 3a6e 6f72 6d61 6c3b 666f 6e74  ates:normal;font
+000005b0: 2d76 6172 6961 6e74 2d63 6170 733a 6e6f  -variant-caps:no
+000005c0: 726d 616c 3b66 6f6e 742d 7661 7269 616e  rmal;font-varian
+000005d0: 742d 6c69 6761 7475 7265 733a 6e6f 726d  t-ligatures:norm
+000005e0: 616c 3b66 6f6e 742d 7661 7269 616e 742d  al;font-variant-
+000005f0: 6e75 6d65 7269 633a 6e6f 726d 616c 3b66  numeric:normal;f
+00000600: 6f6e 742d 7661 7269 616e 742d 706f 7369  ont-variant-posi
+00000610: 7469 6f6e 3a6e 6f72 6d61 6c3b 6973 6f6c  tion:normal;isol
+00000620: 6174 696f 6e3a 6175 746f 3b6d 6978 2d62  ation:auto;mix-b
+00000630: 6c65 6e64 2d6d 6f64 653a 6e6f 726d 616c  lend-mode:normal
+00000640: 3b73 6861 7065 2d70 6164 6469 6e67 3a30  ;shape-padding:0
+00000650: 3b74 6578 742d 6465 636f 7261 7469 6f6e  ;text-decoration
+00000660: 2d63 6f6c 6f72 3a23 3030 303b 7465 7874  -color:#000;text
+00000670: 2d64 6563 6f72 6174 696f 6e2d 6c69 6e65  -decoration-line
+00000680: 3a6e 6f6e 653b 7465 7874 2d64 6563 6f72  :none;text-decor
+00000690: 6174 696f 6e2d 7374 796c 653a 736f 6c69  ation-style:soli
+000006a0: 643b 7465 7874 2d69 6e64 656e 743a 303b  d;text-indent:0;
+000006b0: 7465 7874 2d6f 7269 656e 7461 7469 6f6e  text-orientation
+000006c0: 3a6d 6978 6564 3b74 6578 742d 7472 616e  :mixed;text-tran
+000006d0: 7366 6f72 6d3a 6e6f 6e65 2220 7768 6974  sform:none" whit
+000006e0: 652d 7370 6163 653d 226e 6f72 6d61 6c22  e-space="normal"
+000006f0: 2f3e 0a20 3c2f 673e 0a3c 2f73 7667 3e0a  />. </g>.</svg>.
```

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/ad.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/ad.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/af.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/af.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/ag.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/ag.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/ai.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/ai.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/al.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/al.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/ao.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/ao.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/ar.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/ar.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/as.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/as.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/au.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/au.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/az.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/az.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/ba.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/ba.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/bb.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/bb.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/bf.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/bf.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/bi.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/bi.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/bm.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/bm.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/bn.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/bn.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/br.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/br.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/bt.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/bt.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/by.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/by.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/bz.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/bz.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/ca.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/ca.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/cc.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/cc.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/ck.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/ck.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/cn.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/cn.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/cr.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/cr.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/cv.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/cv.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/cw.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/cw.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/cx.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/cx.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/cy.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/cy.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/dm.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/dm.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/do.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/do.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/ec.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/ec.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/eg.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/eg.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/er.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/er.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/es.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/es.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/et.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/et.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/fj.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/fj.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/fk.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/fk.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/fm.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/fm.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/gb.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/gb.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/gd.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/gd.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/ge.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/ge.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/gi.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/gi.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/gp.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/gp.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/gq.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/gq.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/gs.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/gs.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/gt.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/gt.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/gu.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/gu.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/gw.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/gw.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/hk.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/hk.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/hm.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/hm.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/hn.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/hn.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/hr.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/hr.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/ht.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/ht.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/hu.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/hu.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/im.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/im.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/in.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/in.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/io.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/io.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/iq.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/iq.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/ir.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/ir.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/je.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/je.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/ke.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/ke.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/kg.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/kg.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/kh.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/kh.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/ki.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/ki.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/km.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/km.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/kn.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/kn.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/kp.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/kp.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/kr.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/kr.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/ky.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/ky.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/kz.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/kz.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/lb.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/lb.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/li.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/li.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/lk.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/lk.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/lr.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/lr.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/ls.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/ls.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/md.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/md.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/me.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/me.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/mh.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/mh.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/mm.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/mm.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/mn.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/mn.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/mo.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/mo.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/mp.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/mp.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/mr.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/mr.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/ms.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/ms.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/mt.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/mt.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/mw.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/mw.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/mx.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/mx.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/my.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/my.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/mz.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/mz.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/na.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/na.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/nf.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/nf.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/ni.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/ni.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/np.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/np.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/nr.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/nr.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/nu.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/nu.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/nz.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/nz.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/om.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/om.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/pf.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/pf.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/pg.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/pg.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/ph.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/ph.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/pk.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/pk.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/pm.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/pm.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/pn.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/pn.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/pt.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/pt.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/py.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/py.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/rs.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/rs.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/rw.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/rw.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/sa.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/sa.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/sb.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/sb.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/sg.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/sg.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/sh.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/sh.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/si.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/si.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/sk.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/sk.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/sm.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/sm.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/sn.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/sn.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/so.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/so.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/ss.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/ss.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/st.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/st.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/sv.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/sv.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/sx.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/sx.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/sz.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/sz.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/tc.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/tc.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/tf.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/tf.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/tg.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/tg.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/tj.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/tj.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/tk.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/tk.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/tm.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/tm.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/tv.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/tv.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/tw.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/tw.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/ug.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/ug.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/um.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/um.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/us.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/us.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/uy.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/uy.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/uz.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/uz.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/va.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/va.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/vc.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/vc.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/ve.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/ve.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/vg.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/vg.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/vi.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/vi.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/vu.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/vu.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/ws.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/ws.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/zm.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/zm.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/countries/zw.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/countries/zw.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/globe-symbolic.svg` & `OpenRadio-1.1.0/OpenRadio/assets/icons/globe-symbolic.svg`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/map-search-outline.png` & `OpenRadio-1.1.0/OpenRadio/assets/icons/map-search-outline.png`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/search-web.png` & `OpenRadio-1.1.0/OpenRadio/assets/icons/search-web.png`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/star-outline.png` & `OpenRadio-1.1.0/OpenRadio/assets/icons/star-outline.png`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/star.png` & `OpenRadio-1.1.0/OpenRadio/assets/icons/star.png`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/assets/icons/tag-search-outline.png` & `OpenRadio-1.1.0/OpenRadio/assets/icons/tag-search-outline.png`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/core/AudioPlayer.py` & `OpenRadio-1.1.0/OpenRadio/core/AudioPlayer.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,24 +6,24 @@
     DEFAULT_ICON_SIZE,
 )
 import vlc
 import logging
 from gi.repository import Gtk, GLib, GdkPixbuf
 import math
 from time import sleep
-import threading
 import requests
 from requests_file import FileAdapter
 from io import BytesIO
 
 LOGGER = logging.getLogger(__name__)
 LOGGER.setLevel(LOG_LEVEL)
 LOGGER.addHandler(LOG_HANDLER)
 
 
+# This class handles the vlc events
 class event_handler:
     def __init__(self, parent):
         self.parent = parent
         self.source_id = False
 
     def error(self, event, player):
         LOGGER.error("VLC encountered an error.")
@@ -45,34 +45,35 @@
             self.parent.scale.set_range(0, player.get_length())
 
     def update_playing(self, event, player):
         if (
             "show_play_pause" in self.parent.enabled_features
             and self.parent.playing_active
         ):
-            GLib.idle_add(self.parent._set_play_image, "media-playback-pause")
+            GLib.idle_add(self.parent._set_play_image, "media-playback-pause-symbolic")
 
     def update_pause(self, event, player):
         if (
             "show_play_pause" in self.parent.enabled_features
             and self.parent.playing_active
         ):
-            GLib.idle_add(self.parent._set_play_image, "media-playback-start")
+            GLib.idle_add(self.parent._set_play_image, "media-playback-start-symbolic")
 
     def update_stopped(self, event, player):
         self.update_pause(None, player)
 
 
+# Audio player main class
 class AudioPlayer:
     def __init__(self, core):
         self.core = core
-        self.localizer = self.core.Localizer.get_core_translator()
         self.event_handler = event_handler(self)
         self.req_session = requests.Session()
         self.req_session.mount("file://", FileAdapter())
+        self.grid = None
         self.player_event_map = {
             vlc.EventType.MediaPlayerEndReached: self.event_handler.end,
             vlc.EventType.MediaPlayerEncounteredError: self.event_handler.error,
             vlc.EventType.MediaPlayerPositionChanged: self.event_handler.update_position,
             vlc.EventType.MediaPlayerLengthChanged: self.event_handler.update_length,
             vlc.EventType.MediaPlayerPaused: self.event_handler.update_pause,
             vlc.EventType.MediaPlayerStopped: self.event_handler.update_stopped,
@@ -179,36 +180,14 @@
 
     def _skip_back(self, ignore=None):
         self.vlc_list_player.previous()
 
     def _skip_forward(self, ignore=None):
         self.vlc_list_player.next()
 
-    def _favorite_callback(self, button):
-        if self.favorite_butt.get_active():
-            callback = self.favorite_callbacks["set"]
-
-            self.favorite_butt.remove(self.favorite_image)
-            self.favorite_image = self.core.IconHelper.get_icon(
-                "star", size=DEFAULT_ICON_SIZE
-            )
-
-        else:
-            callback = self.favorite_callbacks["remove"]
-
-            self.favorite_butt.remove(self.favorite_image)
-            self.favorite_image = self.core.IconHelper.get_icon(
-                "star-outline", size=DEFAULT_ICON_SIZE
-            )
-
-        callback(*self.favorite_callbacks["args"])
-
-        self.favorite_butt.add(self.favorite_image)
-        self.favorite_butt.show_all()
-
     def _check_kwargs(self, kwargs, is_playlist=False):
         self.enabled_features = []
         row = 0
 
         if kwargs.get("show_title_vlc", False):
             self.enabled_features.append("show_title_vlc")
             self.title_label = Gtk.Label()
@@ -252,33 +231,25 @@
             self._cover_callback = kwargs["show_cover_callback"]
             GLib.timeout_add_seconds(1, self._update_cover, None)
             self.grid.attach(self.cover, 4, row, 1, 1)
 
         row += 1
         if kwargs.get("show_favorite_callbacks", False):
             self.enabled_features.append("show_favorite_callbacks")
-            self.favorite_butt = Gtk.ToggleButton()
-
-            if kwargs["show_favorite_callbacks"]["state"]:
-                self.favorite_image = self.core.IconHelper.get_icon(
-                    "star", size=DEFAULT_ICON_SIZE
-                )
-            else:
-                self.favorite_image = self.core.IconHelper.get_icon(
-                    "star-outline", size=DEFAULT_ICON_SIZE
-                )
-
-            self.favorite_butt.set_active(kwargs["show_favorite_callbacks"]["state"])
-
-            self.favorite_callbacks = kwargs["show_favorite_callbacks"]
-
-            self.favorite_butt.add(self.favorite_image)
-            self.favorite_butt.connect("toggled", self._favorite_callback)
+            set_callback = kwargs["show_favorite_callbacks"]["set"]
+            remove_callback = kwargs["show_favorite_callbacks"]["remove"]
+            args = kwargs["show_favorite_callbacks"]["args"]
+            fav_button, fav_image = self.core.UIHelper.favorite_button(
+                set_callback,
+                remove_callback,
+                kwargs["show_favorite_callbacks"]["state"],
+                *args,
+            )
 
-            self.grid.attach(self.favorite_butt, 4, row, 1, 1)
+            self.grid.attach(fav_button, 4, row, 1, 1)
 
         if kwargs.get("show_slider", False):
             self.enabled_features.append("show_slider")
             self.scale = Gtk.Scale().new_with_range(Gtk.Orientation.HORIZONTAL, 0, 1, 1)
             self.scale.connect("format-value", self._format_millis)
             self.scale.connect("value-changed", self._set_vlc_position)
             self.scale.set_hexpand(True)
@@ -306,28 +277,30 @@
             self.grid.attach(self.seek_forward_button, 3, row, 1, 1)
             add_row = True
 
         if kwargs.get("show_play_pause", False):
             self.enabled_features.append("show_play_pause")
             self.play_pause_button = Gtk.Button()
             self.play_pause_button.set_image(
-                self.core.IconHelper.get_icon("media-playback-start")
+                self.core.IconHelper.get_icon("media-playback-start-symbolic")
             )
             self.play_pause_button.connect("clicked", self._play_pause)
             self.play_pause_button.set_hexpand(False)
             self.grid.attach(self.play_pause_button, 2, row, 1, 1)
             add_row = True
 
         if add_row:
             row += 1
 
         if kwargs.get("show_stop", False):
             self.enabled_features.append("show_stop")
             self.stop_button = Gtk.Button()
-            self.stop_button.add(self.core.IconHelper.get_icon("media-playback-stop"))
+            self.stop_button.add(
+                self.core.IconHelper.get_icon("media-playback-stop-symbolic")
+            )
             self.stop_button.connect("clicked", self._stop)
             self.grid.attach(self.stop_button, 2, row, 1, 1)
 
         if is_playlist:
             if kwargs.get("show_skip", False):
                 self.enabled_features.append("show_skip")
 
@@ -348,22 +321,25 @@
 
         self.autoexit = kwargs.get("autoexit", False)
 
     def clean_up(self):
         self.stop()
         if self.event_handler.source_id:
             GLib.source_remove(self.event_handler.source_id)
-        self.grid.destroy()
+        if self.grid:
+            self.grid.destroy()
 
     def stop(self):
         self.playing_active = False
         self.vlc_player.stop()
         self.vlc_player.release()
         self.vlc_instance.release()
-        self.grid.destroy()
+        if self.grid:
+            self.grid.destroy()
+            self.grid = None
 
     def _init_vlc(self, input: str):
         vlc_instance = vlc.Instance()
         vlc_player = vlc_instance.media_player_new()
         vlc_media = vlc_instance.media_new(input)
 
         self.vlc_player = vlc_player
@@ -374,33 +350,34 @@
 
         self.player_event_manager = vlc_player.event_manager()
         self.media_event_manager = vlc_media.event_manager()
 
         self.playing_active = True
         return vlc_instance, vlc_player, vlc_media
 
+    # Simple wrapper around vlc without gui
     def play_no_gui(self, input: str, on_error: callable, on_return: callable):
         self.on_error = on_error
         self.on_return = on_return
         vlc_instance, vlc_player, vlc_media = self._init_vlc(input)
         vlc_player.play()
 
+    # For playing audio with a basic gui
     def play(self, input: str, on_error, on_return, **kwargs):
-        self.localizer.install()
         self.on_error = on_error
         self.on_return = on_return
 
         vlc_instance, vlc_player, vlc_media = self._init_vlc(input)
 
         grid = Gtk.Grid()
         self.grid = grid
 
         back_arrow = Gtk.Image()
         back_arrow = self.core.IconHelper.get_icon(
-            "go-previous", size=Gtk.IconSize.MENU
+            "go-previous-symbolic", size=Gtk.IconSize.MENU
         )
 
         go_back_button = Gtk.Button()
         go_back_button.add(back_arrow)
         go_back_button.connect("clicked", self._return)
         grid.attach(go_back_button, 0, 0, 1, 1)
```

### Comparing `OpenRadio-1.0/OpenRadio/core/Core.py` & `OpenRadio-1.1.0/OpenRadio/core/Core.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 from . import (
     Settings,
-    Localizer,
     HTTPApi,
     AudioPlayer,
     IconHelper,
     ModuleHandler,
     Window,
+    UIHelper,
 )
 from gi.repository import Gtk
 
 
+# Core class containing all core functionality
 class Core:
     def __init__(self, **kwargs):
         self.Settings = Settings.Settings()  # Needed by almost all modules
-        self.IconHelper = IconHelper.IconHelper()
-        self.Localizer = Localizer.Localizer(self)
+        self.IconHelper = IconHelper.IconHelper(self)
+        self.UIHelper = UIHelper.UIHelper(self)
         self.HTTPApi = HTTPApi.HTTPApi(self)
         self.AudioPlayer = AudioPlayer.AudioPlayer(self)
         self.ModuleHandler = ModuleHandler.ModuleHandler(self)
         self.Window = Window.Window(self, **kwargs)
 
     def quit(self, exit_code):
         for module in self.ModuleHandler.get_all_modules().values():
             module.on_quit()
         self.HTTPApi.on_quit()
         Gtk.main_quit()
-        if exit_code is not int:
+        if not isinstance(exit_code, int):
             exit_code = 0
         exit(exit_code)
```

### Comparing `OpenRadio-1.0/OpenRadio/core/HTTPApi.py` & `OpenRadio-1.1.0/OpenRadio/core/HTTPApi.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from .const import *
 from .Exceptions import *
-import http.server as http
 from http import HTTPStatus
 import http.server as httpd
 
 import urllib.parse as urlparser
 import json
 
 from threading import Thread
@@ -17,56 +16,57 @@
 
 NOT_FOUND = {
     "response_code": HTTPStatus.NOT_FOUND,
     "content_type": "application/json",
     "response": {"error": "The Requested Path was not found."},
 }
 UNKNOWN_REQUEST = {
-    "response_code": HTTPStatus.NOT_FOUND,
+    "response_code": HTTPStatus.BAD_REQUEST,
     "content_type": "application/json",
     "response": {"error": "Not a valid request."},
 }
 
 
 NOT_DECODEABLE_MSG = {"error": "Response data not in str,bytes or dict format."}
 
 FACTORY_SETTINGS = {"ip": "0.0.0.0", "port": 8081}
 
 
+# Class for interacting with http.server
 class HTTPApi:
     def __init__(self, core):
         self.core = core
 
-        http_handler = Handler
-        http_handler.set_core(Handler, self.core)
+        http_handler = HTTPHandler
+        http_handler.set_core(HTTPHandler, self.core)
 
         server_stat = self._start_server(http_handler)
 
         if not server_stat:
             LOGGER.warning(
                 "Error while starting http server. Falling back to factory settings."
             )
             self.restore_server_settings()
             server_stat = self._start_server(http_handler)
 
         if not server_stat:
-            raise HTTPApiNotStarting(f"""Server not staring with factory defaults. Is the port ({self.get_config_entry("ip")}:{self.get_config_entry("port")}) unused?""")
-
-
+            raise HTTPApiNotStarting(
+                f"""Server not staring with factory defaults. Is the port ({self.get_config_entry("ip")}:{self.get_config_entry("port")}) unused?"""
+            )
 
         LOGGER.info(
             f"""Server is available at : {self.get_config_entry("ip")}:{self.get_config_entry("port")}."""
         )
         thread = Thread(target=self.server.serve_forever, name="HTTPApi")
 
         self.thread = thread
 
         thread.start()
 
-    def _start_server(self,http_handler):
+    def _start_server(self, http_handler):
         try:
             server = httpd.HTTPServer(
                 (self.get_config_entry("ip"), self.get_config_entry("port")),
                 http_handler,
             )
 
         except:
@@ -96,48 +96,50 @@
         self.core.Settings.save_config("core.httpapi", FACTORY_SETTINGS)
 
     def on_quit(self):
         self.server.shutdown()
         self.thread.join()
 
 
-class Handler(httpd.BaseHTTPRequestHandler):
-    def _answer_request(self, response):
+# This class handles the incoming http requests
+class HTTPHandler(httpd.BaseHTTPRequestHandler):
+    def _answer_request(self, response: dict):
+        # Dict format : {"response": <data to send to client>, "response_code": <Http status code>, "content_type": "Content Type of response"}
         response_data = response["response"]
         response_type = type(response_data)
 
         response_code = response["response_code"]
 
         response_content = response["content_type"]
 
-        if response_type != bytes and response_type != str and response_type != dict:
+        if not isinstance(response_type, (bytes, str, dict)):
             LOGGER.error("Unable to send data to client. Not bytes,str or dict.")
             response_data = NOT_DECODEABLE_MSG
 
             response_code = HTTPStatus.INTERNAL_SERVER_ERROR
             response_content = "application/json"
 
-        if response_type == str:
+        if isinstance(response_data, str):
             response_data = response_data.encode("utf-8")
-        elif response_type == dict:
+        elif isinstance(response_data, dict):
             try:
                 response_data = json.dumps(response_data).encode("utf-8")
             except TypeError:
                 LOGGER.error("Got unserializable dict.")
                 response_data = json.dumps(NOT_DECODEABLE_MSG).encode("utf-8")
                 response_code = HTTPStatus.INTERNAL_SERVER_ERROR
                 response_content = "application/json"
 
         self.send_response(response_code)
         self.send_header("Content-Type", response["content_type"])
         self.end_headers()
 
         self.wfile.write(response_data)
 
-    def _parse_request(self, post_data=None):
+    def _parse_request(self, post_data: bytes = None):
         decoded_url = urlparser.unquote(self.path)
         split_url = decoded_url.split("/")
 
         rootpath = split_url[1]
 
         if rootpath == "":
             self._answer_request(UNKNOWN_REQUEST)
@@ -151,14 +153,15 @@
 
         module = self.core.ModuleHandler.get_module_by_domain(http_modules[rootpath])
 
         module_sub_path = split_url
 
         module_sub_path.pop(0)
         module_sub_path.pop(0)
+
         if "" in module_sub_path:
             module_sub_path.remove("")
 
         module_response = module.on_http(
             path=module_sub_path, data=post_data, handler=self
         )
         self._answer_request(module_response)
```

### Comparing `OpenRadio-1.0/OpenRadio/core/IconHelper.py` & `OpenRadio-1.1.0/OpenRadio/core/IconHelper.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,45 +5,69 @@
 import os.path as path
 
 LOGGER = logging.getLogger(__name__)
 LOGGER.setLevel(LOG_LEVEL)
 LOGGER.addHandler(LOG_HANDLER)
 
 
+# Helper for retrieving Icons
 class IconHelper:
-    def __init__(self):
-        pass
+    def __init__(self, core):
+        self.core = core
 
-    def _get_backup_icon(self,name,size,subdir = ""):
-        icon_search_path = os.path.join(BACKUP_ICONS,subdir)
+    def _get_force_backup(self):
+        config = self.core.Settings.get_config("core")
+        return config.get("force_backup", False)
+
+    def _set_force_backup(self, state):
+        config = self.core.Settings.get_config("core")
+        config["force_backup"] = state
+        return self.core.Settings.save_config("core", config)
+
+    def _get_backup_icon(self, name, size, subdir=""):
+        icon_search_path = os.path.join(BACKUP_ICONS, subdir)
         icon = Gtk.Image()
-        if type(size) != int:
-            size = int(size)
+
+        width, height = size, size
+
+        if isinstance(size, Gtk.IconSize):
+            exists, width, height = Gtk.IconSize.lookup(size)
 
         for path in os.listdir(icon_search_path):
             file_name = os.path.splitext(path)[0]
             if file_name == name:
-                pixbuf = GdkPixbuf.Pixbuf.new_from_file_at_scale(os.path.join(icon_search_path,path),size,size,True)
+                pixbuf = GdkPixbuf.Pixbuf.new_from_file_at_scale(
+                    os.path.join(icon_search_path, path), width, height, True
+                )
                 icon.set_from_pixbuf(pixbuf)
                 break
         return icon
 
-    def _get_theme_icon(self,name,size):
+    def _get_theme_icon(self, name, size):
         default_size = Gtk.IconSize.MENU
         if type(size) == Gtk.IconSize:
             default_size = size
 
-        icon = Gtk.Image.new_from_icon_name(name,size)
+        icon = Gtk.Image.new_from_icon_name(name, size)
 
         if type(size) != Gtk.IconSize:
             icon.set_pixel_size(size)
 
         return icon
 
-    def get_icon(self,name: str, size: int | Gtk.IconSize = DEFAULT_ICON_SIZE , backup_subdir: str = "",force_backup: bool = False) -> Gtk.Image:
+    def get_icon(
+        self,
+        name: str,
+        size: int | Gtk.IconSize = DEFAULT_ICON_SIZE,
+        backup_subdir: str = "",
+        force_backup: bool = False,
+    ) -> Gtk.Image:
+        if self._get_force_backup():
+            force_backup = True
+
         icon_theme = Gtk.IconTheme.get_default()
+
         if icon_theme.has_icon(name) and not force_backup:
-            icon = self._get_theme_icon(name,size)
+            icon = self._get_theme_icon(name, size)
         else:
-            icon = self._get_backup_icon(name,size,backup_subdir)
-
+            icon = self._get_backup_icon(name, size, backup_subdir)
         return icon
```

### Comparing `OpenRadio-1.0/OpenRadio/core/ModuleHandler.py` & `OpenRadio-1.1.0/OpenRadio/core/ModuleHandler.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,19 +5,22 @@
 from gi.repository import Gtk
 
 LOGGER = logging.getLogger(__name__)
 LOGGER.setLevel(LOG_LEVEL)
 LOGGER.addHandler(LOG_HANDLER)
 
 
+# Loads, parses and sorts modules
 class ModuleHandler:
     modules = {}
 
     def __init__(self, core):
         for module_dir in os.listdir(MODULE_PATH_PREFIX):
+            self.core = core
+
             current_module = import_module("OpenRadio.modules." + module_dir)
 
             if "MODULE_CLASS_NAME" not in current_module.__dict__:
                 LOGGER.error("Module doesn't have MODULE_CLASS_NAME.")
                 Gtk.main_quit()
                 exit(1)
 
@@ -35,14 +38,15 @@
 
             if not self._validate_module(module):
                 Gtk.main_quit()
                 exit(1)
 
             self.modules[module.DOMAIN] = module
 
+    # Check for required tags and variables
     def _validate_module(self, module):
         if module.NAME == None:
             LOGGER.error(
                 f"Module {module.__module__} doesn't have the NAME variable set. Exiting."
             )
             return False
 
@@ -59,28 +63,45 @@
             LOGGER.error(
                 f"Module {module.__module__} doesn't have the ICON variable set or the icon is nonexistent. Exiting."
             )
             return False
 
         return True
 
+    # Sorts modules by module_order
+    def _sort(self, module_domains: list):
+        module_order = self.core.Settings.get_config("core").get("module_order", [])
+        sorted_list = []
+        for module_domain in module_order:
+            if module_domain in module_domains:
+                module_domains.remove(module_domain)
+                sorted_list.append(module_domain)
+        sorted_list.extend(module_domains)
+        return sorted_list
+
+    # Returns all modules
     def get_all_modules(self) -> dict:
         return self.modules
 
+    # Get module by domain
     def get_module_by_domain(self, domain: str):
         if domain not in self.modules:
             return None
         return self.modules[domain]
 
-    def get_modules_by_tags(self, tags: dict) -> dict:
+    # Get modules by tags provided as list
+    def get_modules_by_tags(self, tags: list, sort: bool = False) -> dict:
         previous_modules = self.get_all_modules().keys()
         matched = []
         for tag in tags:
             matched = []
             for module_domain in previous_modules:
                 module = self.get_module_by_domain(module_domain)
 
                 if getattr(module, tag, None):
                     matched.append(module_domain)
             previous_modules = matched
 
+        if sort:
+            sorted = self._sort(matched)
+            return sorted
         return matched
```

### Comparing `OpenRadio-1.0/OpenRadio/core/Settings.py` & `OpenRadio-1.1.0/OpenRadio/core/Settings.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import logging
 
 LOGGER = logging.getLogger(__name__)
 LOGGER.setLevel(LOG_LEVEL)
 LOGGER.addHandler(LOG_HANDLER)
 
 
+# Simple class for editing ~/.config/OpenRadio/config.toml
 class Settings:
     def __init__(self):
         self._load_config()
 
     def _get_yaml_fd(self, delete: bool = False):
         if not os.path.exists(CONFIG_DIR):
             os.makedirs(CONFIG_DIR)
@@ -30,23 +31,21 @@
 
         if self.toml == None:
             self.toml = {}
             LOGGER.debug("Empty Toml using empty dict.")
 
         config_fd.close()
 
+    # Returns config for module by domain
     def get_config(self, domain: str) -> dict:
         keys = self.toml.keys()
-        if domain not in keys:
-            return {}
-        return self.toml[domain]
+        return self.toml.get(domain, {})
 
+    # Save config for module by domain
     def save_config(self, domain: str, data: dict) -> None:
-        if type(data) is not dict and type(data) is not items.Table:
-            LOGGER.warning(
-                "Function returned config not in dict or toml format not saving."
-            )
+        if not isinstance(data, dict):
+            LOGGER.warning("Function returned config not in dict format not saving.")
 
         self.toml[domain] = data
         config_fd = self._get_yaml_fd(delete=True)
         dump(self.toml, config_fd)
         config_fd.close()
```

### Comparing `OpenRadio-1.0/OpenRadio/core/Window.py` & `OpenRadio-1.1.0/OpenRadio/core/Window.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,43 +3,51 @@
     LOG_LEVEL,
     LOG_HANDLER,
     VERSION,
     ASSETS_PATH_PREFIX,
     DEFAULT_WINDOW_SIZE,
     DEFAULT_ICON_SIZE,
 )
+from .Localizer import CoreLocalizer
 from gi.repository import Gtk, Gdk, GLib
 from os.path import join
 
 LOGGER = logging.getLogger(__name__)
 LOGGER.setLevel(LOG_LEVEL)
 LOGGER.addHandler(LOG_HANDLER)
 
+localizer = CoreLocalizer()
+translator = localizer.get_translator()
+_ = translator.gettext
 
+
+# The Main window
 class Window(Gtk.Window):
     button_map = {}
 
     FULLSCREEN = False
 
     def __init__(self, core_object, **kwargs):
         Gtk.Window.__init__(self, title="Open Radio v{}".format(VERSION))
+
         self.core = core_object
         self.FULLSCREEN = False
 
         if kwargs.get("fullscreen", False):
             GLib.timeout_add(
                 100, self._set_fullscreen
             )  # Only run after main loop started
+        else:
+            self._restore_fullscreen()
 
         self.current_module = None
 
-        core_object.Localizer.get_core_translator().install()
-
         self.set_default_size(DEFAULT_WINDOW_SIZE[0], DEFAULT_WINDOW_SIZE[1])
         self.set_icon_from_file(join(ASSETS_PATH_PREFIX, "OpenRadio.icon"))
+
         self.set_wmclass(
             "Open Radio v{}".format(VERSION), "Open Radio v{}".format(VERSION)
         )
 
         self.connect("key-press-event", self._on_key_press)
         self.connect("window-state-event", self._on_window_state_event)
 
@@ -50,15 +58,17 @@
         self.show_all()
 
     def _set_fullscreen(self):
         self.fullscreen()
         return False
 
     def _show_main_menu(self):
-        gui_modules = self.core.ModuleHandler.get_modules_by_tags(["USES_GUI"])
+        gui_modules = self.core.ModuleHandler.get_modules_by_tags(
+            ["USES_GUI", "ENABLED"], sort=True
+        )
 
         menu_container_box = Gtk.Box(orientation=Gtk.Orientation.VERTICAL)
 
         modules_flowbox = Gtk.FlowBox()
         modules_flowbox.set_valign(Gtk.Align.START)
         modules_flowbox.set_max_children_per_line(10)
         modules_flowbox.set_selection_mode(Gtk.SelectionMode.NONE)
@@ -117,14 +127,22 @@
 
     def _toggle_fullscreen(self):
         if self.FULLSCREEN:
             self.unfullscreen()
         else:
             self.fullscreen()
 
+    def _restore_fullscreen(self):
+        core_config = self.core.Settings.get_config("core")
+        fullscreen_setting = core_config.get("fullscreen", False)
+        if fullscreen_setting:
+            GLib.timeout_add(
+                100, self._set_fullscreen
+            )  # Only run after main loop started
+
     def _clear_window(self):
         self.remove(self.menu_container_box)
         self.menu_container_box.destroy()
 
     def _on_window_state_event(self, widget, event):
         self.FULLSCREEN = bool(event.new_window_state & Gdk.WindowState.FULLSCREEN)
 
@@ -133,23 +151,29 @@
             self._toggle_fullscreen()
 
     def _on_button(self, button):
         self._clear_window()
         self.current_module = self.button_map[button]
         self.current_module.on_show()
 
+    # Clears the window and calling the function with args
     def force_show(self, function: callable, *args):
         LOGGER.debug("Currently showing module : {}".format(self.current_module))
         if self.current_module:
             self.current_module.on_clear()
         else:
             self._clear_window()
         function(*args)
 
+    # Shows the module before force_show
     def show_previous_module(self):
         LOGGER.debug("Previous shown module : {}".format(self.current_module))
+        if not self.current_module:
+            self.show_menu()
+            return
         self.current_module.on_show()
 
+    # Shows the main menu if window is clear
     def show_menu(self):
         self.current_module = None
         self._show_main_menu()
         self.show_all()
```

### Comparing `OpenRadio-1.0/OpenRadio/core/const.py` & `OpenRadio-1.1.0/OpenRadio/core/const.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 LOG_FORMATTER = logging.Formatter("[%(name)s][%(levelname)s]: %(message)s")
 LOG_HANDLER = logging.StreamHandler()
 LOG_HANDLER.setLevel(LOG_LEVEL)
 LOG_HANDLER.setFormatter(LOG_FORMATTER)
 
 # App version
-VERSION = "1.0"
+VERSION = "1.1.0"
 
 # The name of the core
 CORE_NAME = "core"
 
 # Retrieve the Location of the source directory and Core
 CORE = os.path.dirname(__file__)
 MAIN = os.path.abspath(os.path.join(CORE, os.pardir))
@@ -36,16 +36,16 @@
 # Directory where the assets are stored
 ASSETS_PATH_PREFIX = os.path.join(MAIN, "assets")
 
 # Directory where the config is stored
 CONFIG_DIR = os.path.join(os.environ["HOME"], ".config", "OpenRadio")
 # Config file
 CONFIG_FILE = os.path.join(CONFIG_DIR, "config.toml")
-
+# Default size on startup
 DEFAULT_WINDOW_SIZE = (300, 300)
-
+# Icon size used for icons and media icons
 DEFAULT_ICON_SIZE = 48
 DEFAULT_MEDIA_IMAGE_SIZE = 96
-
+# Backup dir for icons
 BACKUP_ICONS = os.path.join(ASSETS_PATH_PREFIX, "icons")
-
+# The interval to seek with buttons
 VLC_SEEK_INTERVAL = 5000
```

### Comparing `OpenRadio-1.0/OpenRadio/locales/modules/builtin.about/de/LC_MESSAGES/builtin.about.mo` & `OpenRadio-1.1.0/OpenRadio/locales/src/de/modules/builtin.about/builtin.about.pot`

 * *Files 23% similar despite different names*

```diff
@@ -1,57 +1,69 @@
-00000000: de12 0495 0000 0000 0200 0000 1c00 0000  ................
-00000010: 2c00 0000 0500 0000 3c00 0000 0000 0000  ,.......<.......
-00000020: 5000 0000 f700 0000 5100 0000 1401 0000  P.......Q.......
-00000030: 4901 0000 2301 0000 5e02 0000 0100 0000  I...#...^.......
-00000040: 0000 0000 0000 0000 0200 0000 0000 0000  ................
-00000050: 0041 6e20 6f70 656e 2d73 6f75 7263 652c  .An open-source,
-00000060: 2074 6f75 6368 2d66 6f63 7573 6564 2072   touch-focused r
-00000070: 6164 696f 2061 7070 6c69 6361 7469 6f6e  adio application
-00000080: 2077 6869 6368 2069 7320 7772 6974 7465   which is writte
-00000090: 6e20 696e 2050 7974 686f 6e2e 0a54 6865  n in Python..The
-000000a0: 2047 7569 2077 6173 2062 7569 6c74 2075   Gui was built u
-000000b0: 7369 6e67 2047 746b 332e 0a41 6e64 2069  sing Gtk3..And i
-000000c0: 7420 6973 204d 6f64 756c 6172 2041 462e  t is Modular AF.
-000000d0: 0a46 6f72 206d 6f72 6520 696e 666f 2076  .For more info v
-000000e0: 6973 6974 203c 6120 6872 6566 3d22 6874  isit <a href="ht
-000000f0: 7470 733a 2f2f 6769 746c 6162 2e63 6f6d  tps://gitlab.com
-00000100: 2f31 3333 374d 6973 6f6d 2f4f 7065 6e52  /1337Misom/OpenR
-00000110: 6164 696f 223e 4769 746c 6162 3c2f 613e  adio">Gitlab</a>
-00000120: 2e0a 4f70 656e 5261 6469 6f20 436f 7079  ..OpenRadio Copy
-00000130: 7269 6768 7420 2843 2920 3230 3233 2031  right (C) 2023 1
-00000140: 3333 374d 6973 6f6d 0050 726f 6a65 6374  337Misom.Project
-00000150: 2d49 642d 5665 7273 696f 6e3a 2050 4143  -Id-Version: PAC
-00000160: 4b41 4745 2056 4552 5349 4f4e 0a50 4f2d  KAGE VERSION.PO-
-00000170: 5265 7669 7369 6f6e 2d44 6174 653a 2059  Revision-Date: Y
-00000180: 4541 522d 4d4f 2d44 4120 484f 3a4d 492b  EAR-MO-DA HO:MI+
-00000190: 5a4f 4e45 0a4c 6173 742d 5472 616e 736c  ZONE.Last-Transl
-000001a0: 6174 6f72 3a20 4655 4c4c 204e 414d 4520  ator: FULL NAME 
-000001b0: 3c45 4d41 494c 4041 4444 5245 5353 3e0a  <EMAIL@ADDRESS>.
-000001c0: 4c61 6e67 7561 6765 2d54 6561 6d3a 204c  Language-Team: L
-000001d0: 414e 4755 4147 4520 3c4c 4c40 6c69 2e6f  ANGUAGE <LL@li.o
-000001e0: 7267 3e0a 4d49 4d45 2d56 6572 7369 6f6e  rg>.MIME-Version
-000001f0: 3a20 312e 300a 436f 6e74 656e 742d 5479  : 1.0.Content-Ty
-00000200: 7065 3a20 7465 7874 2f70 6c61 696e 3b20  pe: text/plain; 
-00000210: 6368 6172 7365 743d 5554 462d 380a 436f  charset=UTF-8.Co
-00000220: 6e74 656e 742d 5472 616e 7366 6572 2d45  ntent-Transfer-E
-00000230: 6e63 6f64 696e 673a 2038 6269 740a 4765  ncoding: 8bit.Ge
-00000240: 6e65 7261 7465 642d 4279 3a20 7079 6765  nerated-By: pyge
-00000250: 7474 6578 742e 7079 2031 2e35 0a00 4569  ttext.py 1.5..Ei
-00000260: 6e20 4f70 656e 2d53 6f75 7263 6520 756e  n Open-Source un
-00000270: 6420 546f 7563 6873 6372 6565 6e20 666f  d Touchscreen fo
-00000280: 6b75 7369 6572 7465 7320 7072 6f67 7261  kusiertes progra
-00000290: 6d6d 2c20 7765 6c63 6865 7320 696e 2050  mm, welches in P
-000002a0: 7974 686f 6e20 6765 7363 6872 6965 6265  ython geschriebe
-000002b0: 6e20 7775 7264 652e 0a44 6965 2042 656e  n wurde..Die Ben
-000002c0: 7574 7a65 726f 6265 7266 6cc3 a463 6865  utzeroberfl..che
-000002d0: 2077 7572 6465 206d 6974 2047 746b 3320   wurde mit Gtk3 
-000002e0: 6765 6261 7574 2e0a 4573 2069 7374 2061  gebaut..Es ist a
-000002f0: 7563 6820 7665 7264 616d 6d74 204d 6f64  uch verdammt Mod
-00000300: 756c 6172 2e0a 46c3 bc72 206d 6568 7220  ular..F..r mehr 
-00000310: 696e 666f 7320 6765 6865 207a 7520 3c61  infos gehe zu <a
-00000320: 2068 7265 663d 2268 7474 7073 3a2f 2f67   href="https://g
-00000330: 6974 6c61 622e 636f 6d2f 3133 3337 4d69  itlab.com/1337Mi
-00000340: 736f 6d2f 4f70 656e 5261 6469 6f22 3e47  som/OpenRadio">G
-00000350: 6974 6c61 623c 2f61 3e2e 0a4f 7065 6e52  itlab</a>..OpenR
-00000360: 6164 696f 2043 6f70 7972 6967 6874 2028  adio Copyright (
-00000370: 4329 2032 3032 3320 3133 3337 4d69 736f  C) 2023 1337Miso
-00000380: 6d00                                     m.
+00000000: 2320 534f 4d45 2044 4553 4352 4950 5449  # SOME DESCRIPTI
+00000010: 5645 2054 4954 4c45 2e0a 2320 436f 7079  VE TITLE..# Copy
+00000020: 7269 6768 7420 2843 2920 5945 4152 204f  right (C) YEAR O
+00000030: 5247 414e 495a 4154 494f 4e0a 2320 4649  RGANIZATION.# FI
+00000040: 5253 5420 4155 5448 4f52 203c 454d 4149  RST AUTHOR <EMAI
+00000050: 4c40 4144 4452 4553 533e 2c20 5945 4152  L@ADDRESS>, YEAR
+00000060: 2e0a 230a 6d73 6769 6420 2222 0a6d 7367  ..#.msgid "".msg
+00000070: 7374 7220 2222 0a22 5072 6f6a 6563 742d  str ""."Project-
+00000080: 4964 2d56 6572 7369 6f6e 3a20 5041 434b  Id-Version: PACK
+00000090: 4147 4520 5645 5253 494f 4e5c 6e22 0a22  AGE VERSION\n"."
+000000a0: 504f 542d 4372 6561 7469 6f6e 2d44 6174  POT-Creation-Dat
+000000b0: 653a 2032 3032 332d 3036 2d32 3520 3136  e: 2023-06-25 16
+000000c0: 3a31 342b 3032 3030 5c6e 220a 2250 4f2d  :14+0200\n"."PO-
+000000d0: 5265 7669 7369 6f6e 2d44 6174 653a 2059  Revision-Date: Y
+000000e0: 4541 522d 4d4f 2d44 4120 484f 3a4d 492b  EAR-MO-DA HO:MI+
+000000f0: 5a4f 4e45 5c6e 220a 224c 6173 742d 5472  ZONE\n"."Last-Tr
+00000100: 616e 736c 6174 6f72 3a20 4655 4c4c 204e  anslator: FULL N
+00000110: 414d 4520 3c45 4d41 494c 4041 4444 5245  AME <EMAIL@ADDRE
+00000120: 5353 3e5c 6e22 0a22 4c61 6e67 7561 6765  SS>\n"."Language
+00000130: 2d54 6561 6d3a 204c 414e 4755 4147 4520  -Team: LANGUAGE 
+00000140: 3c4c 4c40 6c69 2e6f 7267 3e5c 6e22 0a22  <LL@li.org>\n"."
+00000150: 4d49 4d45 2d56 6572 7369 6f6e 3a20 312e  MIME-Version: 1.
+00000160: 305c 6e22 0a22 436f 6e74 656e 742d 5479  0\n"."Content-Ty
+00000170: 7065 3a20 7465 7874 2f70 6c61 696e 3b20  pe: text/plain; 
+00000180: 6368 6172 7365 743d 5554 462d 385c 6e22  charset=UTF-8\n"
+00000190: 0a22 436f 6e74 656e 742d 5472 616e 7366  ."Content-Transf
+000001a0: 6572 2d45 6e63 6f64 696e 673a 2038 6269  er-Encoding: 8bi
+000001b0: 745c 6e22 0a22 4765 6e65 7261 7465 642d  t\n"."Generated-
+000001c0: 4279 3a20 7079 6765 7474 6578 742e 7079  By: pygettext.py
+000001d0: 2031 2e35 5c6e 220a 0a0a 233a 202e 2e2f   1.5\n"...#: ../
+000001e0: 4f70 656e 5261 6469 6f5f 7465 7374 2f4f  OpenRadio_test/O
+000001f0: 7065 6e52 6164 696f 2f2f 6d6f 6475 6c65  penRadio//module
+00000200: 732f 4162 6f75 742f 5f5f 696e 6974 5f5f  s/About/__init__
+00000210: 2e70 793a 3331 0a6d 7367 6964 2022 220a  .py:31.msgid "".
+00000220: 2241 6e20 6f70 656e 2d73 6f75 7263 652c  "An open-source,
+00000230: 2074 6f75 6368 2d66 6f63 7573 6564 2072   touch-focused r
+00000240: 6164 696f 2061 7070 6c69 6361 7469 6f6e  adio application
+00000250: 2077 6869 6368 2069 7320 7772 6974 7465   which is writte
+00000260: 6e20 696e 2050 7974 686f 6e2e 5c6e 220a  n in Python.\n".
+00000270: 2254 6865 2047 7569 2077 6173 2062 7569  "The Gui was bui
+00000280: 6c74 2075 7369 6e67 2047 746b 332e 5c6e  lt using Gtk3.\n
+00000290: 220a 2241 6e64 2069 7420 6973 204d 6f64  "."And it is Mod
+000002a0: 756c 6172 2041 462e 5c6e 220a 2246 6f72  ular AF.\n"."For
+000002b0: 206d 6f72 6520 696e 666f 2076 6973 6974   more info visit
+000002c0: 203c 6120 6872 6566 3d5c 2268 7474 7073   <a href=\"https
+000002d0: 3a2f 2f67 6974 6c61 622e 636f 6d2f 3133  ://gitlab.com/13
+000002e0: 3337 4d69 736f 6d2f 4f70 656e 5261 6469  37Misom/OpenRadi
+000002f0: 6f5c 223e 4769 746c 6162 3c2f 613e 2e5c  o\">Gitlab</a>.\
+00000300: 6e22 0a22 4f70 656e 5261 6469 6f20 436f  n"."OpenRadio Co
+00000310: 7079 7269 6768 7420 2843 2920 3230 3233  pyright (C) 2023
+00000320: 2031 3333 374d 6973 6f6d 220a 6d73 6773   1337Misom".msgs
+00000330: 7472 2022 220a 2245 696e 204f 7065 6e2d  tr ""."Ein Open-
+00000340: 536f 7572 6365 2075 6e64 2054 6f75 6368  Source und Touch
+00000350: 2066 6f6b 7573 6965 7274 6573 2070 726f   fokusiertes pro
+00000360: 6772 616d 2c20 7765 6c63 6865 7320 696e  gram, welches in
+00000370: 2050 7974 686f 6e20 6765 7363 6872 6965   Python geschrie
+00000380: 6265 6e20 7775 7264 652e 5c6e 220a 2244  ben wurde.\n"."D
+00000390: 6965 2047 5549 2077 7572 6465 206d 6974  ie GUI wurde mit
+000003a0: 2047 746b 3320 6765 6261 7574 2e5c 6e22   Gtk3 gebaut.\n"
+000003b0: 0a22 4573 2069 7374 2061 7563 6820 6d6f  ."Es ist auch mo
+000003c0: 6475 6c61 722e 5c6e 220a 2246 c3bc 7220  dular.\n"."F..r 
+000003d0: 6d65 6872 2069 6e66 6f73 2062 6573 7563  mehr infos besuc
+000003e0: 6865 203c 6120 6872 6566 3d5c 2268 7474  he <a href=\"htt
+000003f0: 7073 3a2f 2f67 6974 6c61 622e 636f 6d2f  ps://gitlab.com/
+00000400: 3133 3337 4d69 736f 6d2f 4f70 656e 5261  1337Misom/OpenRa
+00000410: 6469 6f5c 223e 4769 746c 6162 3c2f 613e  dio\">Gitlab</a>
+00000420: 2e5c 6e22 0a22 4f70 656e 5261 6469 6f20  .\n"."OpenRadio 
+00000430: 436f 7079 7269 6768 7420 2843 2920 3230  Copyright (C) 20
+00000440: 3233 2031 3333 374d 6973 6f6d 220a       23 1337Misom".
```

### Comparing `OpenRadio-1.0/OpenRadio/locales/modules/builtin.about/en/LC_MESSAGES/builtin.about.mo` & `OpenRadio-1.1.0/OpenRadio/locales/modules/builtin.about/en/LC_MESSAGES/builtin.about.mo`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/locales/modules/builtin.internetradio/de/LC_MESSAGES/builtin.internetradio.mo` & `OpenRadio-1.1.0/OpenRadio/locales/modules/builtin.internetradio/de/LC_MESSAGES/builtin.internetradio.mo`

 * *Files 25% similar despite different names*

#### msgunfmt {}

```diff
@@ -9,14 +9,14 @@
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: pygettext.py 1.5\n"
 
 msgid "Favorites"
 msgstr "Favoriten"
 
 msgid "Search by language"
-msgstr "Mit Sprache Suchen"
+msgstr "Mit sprache suchen"
 
 msgid "Search by region"
-msgstr "Mit Region Suchen"
+msgstr "Mit region suchen"
 
 msgid "Search by tag"
-msgstr "Mit Tag Suchen"
+msgstr "Mit tag suchen"
```

### Comparing `OpenRadio-1.0/OpenRadio/locales/modules/builtin.internetradio/en/LC_MESSAGES/builtin.internetradio.mo` & `OpenRadio-1.1.0/OpenRadio/locales/modules/builtin.internetradio/en/LC_MESSAGES/builtin.internetradio.mo`

 * *Files identical despite different names*

### Comparing `OpenRadio-1.0/OpenRadio/locales/src/de/core/core.pot` & `OpenRadio-1.1.0/OpenRadio/locales/templates/modules/builtin.about/builtin.about.pot`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR ORGANIZATION
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"POT-Creation-Date: 2023-02-07 22:21+0100\n"
+"POT-Creation-Date: 2023-06-25 16:14+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: pygettext.py 1.5\n"
 
 
-#: ../OpenRadio/OpenRadio/core/window.py:112
-msgid "Select one of the following Modules"
-msgstr "Wähle ein Modul aus"
+#: ../OpenRadio_test/OpenRadio//modules/About/__init__.py:31
+msgid ""
+"An open-source, touch-focused radio application which is written in Python.\n"
+"The Gui was built using Gtk3.\n"
+"And it is Modular AF.\n"
+"For more info visit <a href=\"https://gitlab.com/1337Misom/OpenRadio\">Gitlab</a>.\n"
+"OpenRadio Copyright (C) 2023 1337Misom"
+msgstr ""
+
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `OpenRadio-1.0/OpenRadio/locales/src/de/modules/builtin.internetradio/builtin.internetradio.pot` & `OpenRadio-1.1.0/OpenRadio/locales/src/de/modules/builtin.internetradio/builtin.internetradio.pot`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR ORGANIZATION
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"POT-Creation-Date: 2023-05-13 18:32+0200\n"
+"POT-Creation-Date: 2023-06-25 16:16+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: pygettext.py 1.5\n"
 
 
-#: ../OpenRadio/OpenRadio/modules/InternetRadio/UI.py:429
+#: ../OpenRadio_test/OpenRadio//modules/InternetRadio/UI.py:448
 msgid "Search by region"
-msgstr "Mit Region Suchen"
+msgstr "Mit region suchen"
 
-#: ../OpenRadio/OpenRadio/modules/InternetRadio/UI.py:436
+#: ../OpenRadio_test/OpenRadio//modules/InternetRadio/UI.py:455
 msgid "Search by tag"
-msgstr "Mit Tag Suchen"
+msgstr "Mit tag suchen"
 
-#: ../OpenRadio/OpenRadio/modules/InternetRadio/UI.py:443
+#: ../OpenRadio_test/OpenRadio//modules/InternetRadio/UI.py:462
 msgid "Search by language"
-msgstr "Mit Sprache Suchen"
+msgstr "Mit sprache suchen"
 
-#: ../OpenRadio/OpenRadio/modules/InternetRadio/UI.py:450
+#: ../OpenRadio_test/OpenRadio//modules/InternetRadio/UI.py:469
 msgid "Favorites"
 msgstr "Favoriten"
```

### Comparing `OpenRadio-1.0/OpenRadio/locales/src/en/core/core.pot` & `OpenRadio-1.1.0/OpenRadio/locales/src/en/core/core.pot`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR ORGANIZATION
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"POT-Creation-Date: 2023-02-07 22:21+0100\n"
+"POT-Creation-Date: 2023-06-25 16:14+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: pygettext.py 1.5\n"
 
 
-#: ../OpenRadio/OpenRadio/core/window.py:112
+#: ../OpenRadio_test/OpenRadio/core/Window.py:108
 msgid "Select one of the following Modules"
 msgstr "Select one of the following Modules"
```

### Comparing `OpenRadio-1.0/OpenRadio/locales/src/en/modules/builtin.about/builtin.about.pot` & `OpenRadio-1.1.0/OpenRadio/locales/src/en/modules/builtin.about/builtin.about.pot`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR ORGANIZATION
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"POT-Creation-Date: 2023-02-07 22:22+0100\n"
+"POT-Creation-Date: 2023-06-25 16:14+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: pygettext.py 1.5\n"
 
 
-#: ../OpenRadio/OpenRadio//modules/About/__init__.py:28
+#: ../OpenRadio_test/OpenRadio//modules/About/__init__.py:31
 msgid ""
 "An open-source, touch-focused radio application which is written in Python.\n"
 "The Gui was built using Gtk3.\n"
 "And it is Modular AF.\n"
 "For more info visit <a href=\"https://gitlab.com/1337Misom/OpenRadio\">Gitlab</a>.\n"
 "OpenRadio Copyright (C) 2023 1337Misom"
 msgstr ""
```

### Comparing `OpenRadio-1.0/OpenRadio/locales/src/en/modules/builtin.internetradio/builtin.internetradio.pot` & `OpenRadio-1.1.0/OpenRadio/locales/src/en/modules/builtin.internetradio/builtin.internetradio.pot`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR ORGANIZATION
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"POT-Creation-Date: 2023-05-13 18:32+0200\n"
+"POT-Creation-Date: 2023-06-25 16:16+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: pygettext.py 1.5\n"
 
 
-#: ../OpenRadio/OpenRadio/modules/InternetRadio/UI.py:429
+#: ../OpenRadio_test/OpenRadio//modules/InternetRadio/UI.py:448
 msgid "Search by region"
 msgstr "Search by region"
 
-#: ../OpenRadio/OpenRadio/modules/InternetRadio/UI.py:436
+#: ../OpenRadio_test/OpenRadio//modules/InternetRadio/UI.py:455
 msgid "Search by tag"
 msgstr "Search by tag"
 
-#: ../OpenRadio/OpenRadio/modules/InternetRadio/UI.py:443
+#: ../OpenRadio_test/OpenRadio//modules/InternetRadio/UI.py:462
 msgid "Search by language"
 msgstr "Search by language"
 
-#: ../OpenRadio/OpenRadio/modules/InternetRadio/UI.py:450
+#: ../OpenRadio_test/OpenRadio//modules/InternetRadio/UI.py:469
 msgid "Favorites"
 msgstr "Favorites"
```

### Comparing `OpenRadio-1.0/OpenRadio/locales/templates/core/core.pot` & `OpenRadio-1.1.0/OpenRadio/locales/src/de/core/core.pot`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR ORGANIZATION
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"POT-Creation-Date: 2023-02-07 22:21+0100\n"
+"POT-Creation-Date: 2023-06-25 16:14+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: pygettext.py 1.5\n"
 
 
-#: ../OpenRadio/OpenRadio/core/window.py:112
+#: ../OpenRadio_test/OpenRadio/core/Window.py:108
 msgid "Select one of the following Modules"
-msgstr ""
+msgstr "Wähle ein Modul aus"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `OpenRadio-1.0/OpenRadio/locales/templates/modules/builtin.about/builtin.about.pot` & `OpenRadio-1.1.0/OpenRadio/locales/templates/core/core.pot`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,21 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR ORGANIZATION
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"POT-Creation-Date: 2023-05-13 18:31+0200\n"
+"POT-Creation-Date: 2023-06-25 16:14+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: pygettext.py 1.5\n"
 
 
-#: ../OpenRadio/OpenRadio/modules/About/__init__.py:29
-msgid ""
-"An open-source, touch-focused radio application which is written in Python.\n"
-"The Gui was built using Gtk3.\n"
-"And it is Modular AF.\n"
-"For more info visit <a href=\"https://gitlab.com/1337Misom/OpenRadio\">Gitlab</a>.\n"
-"OpenRadio Copyright (C) 2023 1337Misom"
+#: ../OpenRadio_test/OpenRadio/core/Window.py:108
+msgid "Select one of the following Modules"
 msgstr ""
```

### Comparing `OpenRadio-1.0/OpenRadio/locales/templates/modules/builtin.internetradio/builtin.internetradio.pot` & `OpenRadio-1.1.0/OpenRadio/locales/templates/modules/builtin.internetradio/builtin.internetradio.pot`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR ORGANIZATION
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"POT-Creation-Date: 2023-05-13 18:45+0200\n"
+"POT-Creation-Date: 2023-06-25 16:16+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: pygettext.py 1.5\n"
 
 
-#: ../OpenRadio/OpenRadio/modules/InternetRadio/UI.py:430
+#: ../OpenRadio_test/OpenRadio//modules/InternetRadio/UI.py:448
 msgid "Search by region"
 msgstr ""
 
-#: ../OpenRadio/OpenRadio/modules/InternetRadio/UI.py:437
+#: ../OpenRadio_test/OpenRadio//modules/InternetRadio/UI.py:455
 msgid "Search by tag"
 msgstr ""
 
-#: ../OpenRadio/OpenRadio/modules/InternetRadio/UI.py:444
+#: ../OpenRadio_test/OpenRadio//modules/InternetRadio/UI.py:462
 msgid "Search by language"
 msgstr ""
 
-#: ../OpenRadio/OpenRadio/modules/InternetRadio/UI.py:451
+#: ../OpenRadio_test/OpenRadio//modules/InternetRadio/UI.py:469
 msgid "Favorites"
 msgstr ""
```

### Comparing `OpenRadio-1.0/OpenRadio/locales/templates/modules/builtin.settings/builtin.settings.pot` & `OpenRadio-1.1.0/OpenRadio/locales/src/de/modules/builtin.settings/builtin.settings.pot`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR ORGANIZATION
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"POT-Creation-Date: 2023-05-13 18:32+0200\n"
+"POT-Creation-Date: 2023-06-25 16:16+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: pygettext.py 1.5\n"
 
 
-#: ../OpenRadio/OpenRadio/modules/Settings/__init__.py:63
+#: ../OpenRadio_test/OpenRadio//modules/Settings/__init__.py:70
 msgid "Select one of the following Modules"
-msgstr ""
-
+msgstr "Wähle ein Modul aus"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `OpenRadio-1.0/OpenRadio/modules/About/__init__.py` & `OpenRadio-1.1.0/OpenRadio/modules/About/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,46 +1,52 @@
 from gi.repository import Gtk, Gdk, GdkPixbuf
 from OpenRadio.core.ModuleClass import ModuleClass
+from OpenRadio.core.Localizer import ModuleLocalizer
 import logging
 
 MODULE_CLASS_NAME = "AboutModule"
 
+DOMAIN = "builtin.about"
 
+localizer = ModuleLocalizer(DOMAIN)
+translator = localizer.get_translator()
+_ = translator.gettext
+
+
+# Simple module to show about
 class AboutModule(ModuleClass):
     NAME = "About"
-    DOMAIN = "builtin.about"
+    DOMAIN = DOMAIN
 
     USES_GUI = True
     USES_HTTP = False
     USES_CONFIG = False
+    USES_FAVORITES = False
+
+    ENABLED = True
 
     def __init__(self):
         self.ICON = self.core.IconHelper.get_icon("dialog-information")
-        translator = self.core.Localizer.get_translator(self.DOMAIN)
-        self.translator = translator
 
     def on_clear(self):
         self.grid.destroy()
 
     def on_show(self):
-        self.translator.install()
-
         about_page = Gtk.Label()
         about_page.set_markup(
             _(
                 """An open-source, touch-focused radio application which is written in Python.\nThe Gui was built using Gtk3.\nAnd it is Modular AF.\nFor more info visit <a href="https://gitlab.com/1337Misom/OpenRadio">Gitlab</a>.\nOpenRadio Copyright (C) 2023 1337Misom"""
             )
         )
         about_page.set_justify(Gtk.Justification.CENTER)
         about_page.set_hexpand(True)
         about_page.set_vexpand(True)
 
-        back_arrow = Gtk.Image()
         back_arrow = self.core.IconHelper.get_icon(
-            "go-previous", size=Gtk.IconSize.MENU
+            "go-previous-symbolic", size=Gtk.IconSize.MENU
         )
 
         go_back_button = Gtk.Button()
         go_back_button.add(back_arrow)
         go_back_button.connect("clicked", self.return_to_main_menu)
 
         grid = Gtk.Grid()
```

### Comparing `OpenRadio-1.0/OpenRadio/modules/Clock/__init__.py` & `OpenRadio-1.1.0/OpenRadio/modules/Alarm/RingUI.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,88 +1,101 @@
-from gi.repository import Gtk, Gdk, GdkPixbuf, GLib
-import logging
-import threading
-from time import sleep
-from datetime import *
 from OpenRadio.core.ModuleClass import ModuleClass
+from gi.repository import Gtk, GLib
+import html
+from datetime import datetime
+
+size_fmt_time = """<span size="500%" >{}</span>"""
+size_fmt_name = """<span size="200%" >{}</span>"""
+size_fmt_stop = """<span size="200%" >{}</span>"""
+
+
+# Widget while Ringing
+class RingUI:
+    def __init__(self, parent):
+        self.parent = parent
+        self.core = parent.core
+        self.container = None
+        self.exit = False
+        self.ringing = False
+        self.playing_module = None
+
+    def cleanup(self):
+        self.exit = True
+        self.ringing = False
+        if self.container:
+            self.container.destroy()
+            self.container = None
+
+    def on_done(self, button, *args):
+        self.cleanup()
+        if self.playing_module:
+            self.playing_module.on_stop_favorite(*args)
+        self.core.Window.show_previous_module()
+
+    def on_error(self, *ignore):
+        self.cleanup()
+        self.core.Window.show_previous_module()
 
-MODULE_CLASS_NAME = "ClockModule"
-
-
-class ClockModule(ModuleClass):
-    # Some parts of this code originates from https://gist.github.com/olisolomons/b7b924628881a044638e68adb6982fd1. A few changes were made to improve compatibility.
-    NAME = "Clock"
-    DOMAIN = "builtin.clock"
-
-    USES_GUI = True
-    USES_HTTP = False
-    USES_CONFIG = False
-    USES_FAVORITES = False
-
-    def __init__(self):
-        self.ICON = self.core.IconHelper.get_icon("globe-symbolic")
-
-    def return_to_main_menu(self, widget, ignore=None):
-        self.on_clear()
-        self.core.Window.show_menu()
-
-    def update_time(self):
-        if self.quit:
+    def update_time(self, label):
+        if self.exit:
             return False
-        t = datetime.now()
-        self.clock.set_text(t.strftime("%H:%M:%S"))
-        return True
-
-    def on_quit(self, ignore=None):
-        self.quit = True
-
-    def on_clear(self):
-        self.quit = True
-
-        self.style_context.remove_provider_for_screen(self.screen, self.provider)
-
-        self.button.destroy()
+        current_time = datetime.now()
 
-        self.core.Window.disconnect(self.exit_signal_id)
-
-    def on_show(self):
-        self.quit = False
-
-        self.exit_signal_id = self.core.Window.connect(
-            "key-press-event", self.return_to_main_menu
-        )
-
-        self.screen = Gdk.Screen.get_default()
-        self.provider = Gtk.CssProvider()
-        self.style_context = Gtk.StyleContext()
-
-        self.style_context.add_provider_for_screen(
-            self.screen, self.provider, Gtk.STYLE_PROVIDER_PRIORITY_APPLICATION
-        )
-
-        css = b"""
-        #clock_label {
-            font-size: 500%;
-        }
-        """
-        self.provider.load_from_data(css)
-
-        self.grid = Gtk.Grid()
-
-        self.clock = Gtk.Label()
-        self.clock.set_name("clock_label")
-        self.clock.set_hexpand(True)
-        self.clock.set_vexpand(True)
-
-        self.update_time()
+        if self.parent.get_metric_time():
+            time_str = current_time.strftime("%H:%M")
+        else:
+            time_str = current_time.strftime("%I:%M")
+        label.set_markup(size_fmt_time.format(time_str))
+        label.show()
+        return True
 
-        self.grid.attach(self.clock, 0, 0, 1, 1)
+    def play_module(self, alarm_name, module: ModuleClass, *args):
+        self.exit = False
 
-        self.button = Gtk.Button()
-        self.button.add(self.grid)
-        self.button.connect("clicked", self.return_to_main_menu)
+        if self.ringing:
+            return False
 
-        self.core.Window.add(self.button)
+        self.ringing = True
 
+        name_escaped = html.escape(alarm_name)
+        grid = Gtk.Grid(orientation=Gtk.Orientation.VERTICAL)
+        time_label = Gtk.Label()
+        time_label.set_margin_top(50)
+        time_label.set_vexpand(False)
+        time_label.set_hexpand(True)
+        time_label.set_halign(Gtk.Align.CENTER)
+        time_label.set_valign(Gtk.Align.START)
+
+        name_label = Gtk.Label()
+        name_label.set_markup(size_fmt_name.format(name_escaped))
+        name_label.set_vexpand(True)
+        name_label.set_hexpand(True)
+        name_label.set_halign(Gtk.Align.CENTER)
+        name_label.set_valign(Gtk.Align.START)
+
+        stop_label = Gtk.Label()
+        stop_label.set_markup(size_fmt_stop.format("Stop"))
+
+        stop_button = Gtk.Button()
+        stop_button.connect("clicked", self.on_done, *args)
+        stop_button.add(stop_label)
+        stop_button.set_margin_bottom(50)
+        stop_button.set_margin_top(50)
+        stop_button.set_halign(Gtk.Align.CENTER)
+        stop_button.set_valign(Gtk.Align.END)
+
+        grid.attach(time_label, 1, 0, 1, 1)
+        grid.attach(name_label, 1, 1, 1, 1)
+        grid.attach(stop_button, 1, 3, 1, 1)
+        self.update_time(time_label)
+        GLib.timeout_add(1000, self.update_time, time_label)
+        self.container = grid
+
+        self.playing_module = module
+
+        error = module.on_play_favorite(self.on_done, self.on_error, *args)
+        if error:
+            self.core.Window.show_previous_module()
+            return
+        self.core.Window.add(grid)
         self.core.Window.show_all()
-
-        GLib.timeout_add(500, self.update_time)
+        return
```

### Comparing `OpenRadio-1.0/OpenRadio/modules/Exit/__init__.py` & `OpenRadio-1.1.0/OpenRadio/modules/Exit/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from OpenRadio.core.ModuleClass import ModuleClass
 from gi.repository import Gtk
 
 MODULE_CLASS_NAME = "ExitModule"
 
 
+# Module for closing OpenRadio
 class ExitModule(ModuleClass):
     NAME = "Exit"
     DOMAIN = "builtin.exit"
 
     USES_CONFIG = True
     USES_GUI = True
     USES_HTTP = False
```

### Comparing `OpenRadio-1.0/OpenRadio/modules/InternetRadio/IconThread.py` & `OpenRadio-1.1.0/OpenRadio/modules/InternetRadio/IconThread.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 from gi.repository import Gtk, GLib, GdkPixbuf
+
 import requests
+
 from urllib.parse import urlparse
+
 from OpenRadio.core.const import DEFAULT_ICON_SIZE
 
 
+# Thread to fetch favicons
 class IconThread:
     def __init__(self, logger):
         self.running = False
         self.logger = logger
 
     def _icon_fetcher(self):
         session = requests.session()
@@ -72,8 +76,8 @@
         self.fetched_icons = []
         self.running = True
         GLib.idle_add(self._icon_idle)
         self.thread = GLib.Thread("IconThread", self._icon_fetcher)
 
     def stop(self):
         self.running = False
-        #self.thread.join()
+        # self.thread.join()
```

### Comparing `OpenRadio-1.0/OpenRadio/modules/InternetRadio/UI.py` & `OpenRadio-1.1.0/OpenRadio/modules/InternetRadio/UI.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,37 @@
 from gi.repository import Gtk
-import logging
+
 from .IconThread import IconThread
+
 import requests
+
 from OpenRadio.core.const import LOG_LEVEL, LOG_HANDLER
+from OpenRadio.core.Localizer import ModuleLocalizer
+
 import logging
 
 LOGGER = logging.getLogger(__name__)
 LOGGER.setLevel(LOG_LEVEL)
 LOGGER.addHandler(LOG_HANDLER)
 LOGGER.propagate = False
 
+localizer = ModuleLocalizer("builtin.internetradio")
+translator = localizer.get_translator()
+_ = translator.gettext
+
 
+# Class implementing the UI for the InternetRadio
 class UI:
-    def __init__(self, parent, logger, browser):
+    def __init__(self, parent, logger):
         self.core = parent.core
-        self.localizer = parent.localizer
         self.parent = parent
         self.current_container = None
         self.window_history = []
         self.logger = logger
         self.icon_thread = IconThread(logger)
-        self.RadioBrowser = browser
         self.playing = False
 
     def _clean_up(self):
         LOGGER.debug("Cleaning up")
         if self.playing:
             self.core.AudioPlayer.stop()
             self.playing = False
@@ -45,15 +52,17 @@
         flowbox = Gtk.FlowBox()
         flowbox.set_valign(Gtk.Align.START)
         flowbox.set_max_children_per_line(15)
         flowbox.set_selection_mode(Gtk.SelectionMode.NONE)
 
         go_back = Gtk.Button()
         go_back.set_image(
-            self.core.IconHelper.get_icon("go-previous", size=Gtk.IconSize.MENU)
+            self.core.IconHelper.get_icon(
+                "go-previous-symbolic", size=Gtk.IconSize.MENU
+            )
         )
         go_back.connect("clicked", self._show_previous_window)
 
         flowbox.add(go_back)
         scrolled_window.add(flowbox)
 
         return flowbox, scrolled_window
@@ -125,15 +134,17 @@
         self.toggle_button_map = {}
 
         vbox = Gtk.Box(orientation=Gtk.Orientation.VERTICAL)
         control_box = Gtk.Box(orientation=Gtk.Orientation.HORIZONTAL)
 
         return_button = Gtk.Button()
         return_button.add(
-            self.core.IconHelper.get_icon("go-previous", size=Gtk.IconSize.MENU)
+            self.core.IconHelper.get_icon(
+                "go-previous-symbolic", size=Gtk.IconSize.MENU
+            )
         )
         return_button.connect("clicked", self._show_previous_window)
 
         continue_button = Gtk.Button()
         continue_button.add(
             self.core.IconHelper.get_icon("go-next", size=Gtk.IconSize.MENU)
         )
@@ -190,15 +201,15 @@
             country_callback = self._show_states
 
         self._clean_up()
         self._update_previous_window(self._show_countries, button, country_callback)
 
         flowbox, scrolled_window = self._gen_basic_ui()
         self.logger.debug("Fetching all countries")
-        all_countries = self.RadioBrowser.countries()
+        all_countries = self.parent.browser.countries()
         country_list, country_dict = self._sort_by_alpha(all_countries, "name")
 
         for country_name in country_list:
             button, image = self._gen_simple_button(
                 country_name,
                 country_dict[country_name]["iso_3166_1"].lower(),
                 country_callback,
@@ -227,29 +238,29 @@
         self.icon_thread.start(image_map)
         return flowbox, scrolled_window
 
     def _show_stations_in_state(self, button, state):
         self._clean_up()
         self._update_previous_window(self._show_stations_in_state, button, state)
 
-        all_stations = self.RadioBrowser.stations_by_state(state)
+        all_stations = self.parent.browser.stations_by_state(state)
 
         flowbox, scrolled_window = self._show_stations(all_stations)
 
         self.current_container = scrolled_window
 
         self.core.Window.add(scrolled_window)
         self.core.Window.show_all()
 
     def _show_states(self, button, country):
         self._clean_up()
         self._update_previous_window(self._show_states, button, country)
 
         flowbox, scrolled_window = self._gen_basic_ui()
-        all_states = self.RadioBrowser.states(country)
+        all_states = self.parent.browser.states(country)
 
         state_list, state_dict = self._sort_by_alpha(all_states, "name")
 
         for state_name in state_list:
             button, image = self._gen_simple_button(
                 state_name, None, self._show_stations_in_state, state_name
             )
@@ -279,15 +290,15 @@
         self.core.Window.show_all()
 
     def _show_tags_in_country(self, button, country):
         self._clean_up()
         self._update_previous_window(self._show_tags_in_country, button, country)
         self.current_tags = []
         tag_list = []
-        all_stations = self.RadioBrowser.stations_by_country(country)
+        all_stations = self.parent.browser.stations_by_country(country)
         for station in all_stations:
             if len(station["tags"]) < 1:
                 continue
             for tag in station["tags"].split(","):
                 if tag in tag_list:
                     continue
                 tag_list.append(tag)
@@ -306,27 +317,27 @@
     def _show_tags(self, button):
         self._show_countries(None, self._show_tags_in_country)
 
     def _show_stations_by_language(self, button, language):
         self._clean_up()
         self._update_previous_window(self._show_stations_by_language, button, language)
 
-        stations = self.RadioBrowser.stations_by_language(language)
+        stations = self.parent.browser.stations_by_language(language)
 
         flowbox, scrolled_window = self._show_stations(stations)
 
         self.current_container = scrolled_window
 
         self.core.Window.add(scrolled_window)
         self.core.Window.show_all()
 
     def _show_languages(self, button):
         self._clean_up()
         self._update_previous_window(self._show_languages, button)
-        all_languages = self.RadioBrowser.languages()
+        all_languages = self.parent.browser.languages()
         language_list, language_dict = self._sort_by_alpha(all_languages, "name")
 
         flowbox, scrolled_window = self._gen_basic_ui()
 
         for language in language_list:
             button, image = self._gen_simple_button(
                 language, None, self._show_stations_by_language, language
@@ -339,15 +350,15 @@
         self.core.Window.show_all()
 
     def _show_favorites(self, button):
         self._clean_up()
         self._update_previous_window(self._show_favorites, button)
         stations = []
         for station in self.parent.on_get_favorites().values():
-            stations.append(self.RadioBrowser.station_by_uuid(station)[0])
+            stations.append(self.parent.browser.station_by_uuid(station[0])[0])
 
         flowbox, scrolled_window = self._show_stations(stations)
 
         self.current_container = scrolled_window
         self.core.Window.add(scrolled_window)
         self.core.Window.show_all()
 
@@ -357,15 +368,15 @@
         return False
 
     def _player_error(self):
         self.playing = False
         self._show_previous_window()
         return False
 
-    def _play_station(self, button, station):
+    def _play_station(self, button, station, is_gui=True, on_end=None, on_error=None):
         self._clean_up()
         session = requests.session()
 
         self._update_previous_window(self._play_station, button, station)
 
         new_image = self.icon_thread._icon_from_station(station, session)
 
@@ -378,26 +389,29 @@
         player_settings["show_favorite_callbacks"] = {
             "set": self.parent.on_set_favorite,
             "remove": self.parent.on_remove_favorite,
             "state": False,
             "args": [station],
         }
 
-        for uuid in self.parent.on_get_favorites().values():
-            if str(uuid) == station["stationuuid"]:
+        for args in self.parent.on_get_favorites().values():
+            if str(args[0]) == station["stationuuid"]:
                 player_settings["show_favorite_callbacks"]["state"] = True
 
         if new_image:
             player_settings["show_cover_gtk_image"] = new_image
 
         LOGGER.debug(f"Starting Audio with {player_settings}.")
         self.playing = True
-        self.core.AudioPlayer.play(
-            station["url"], self._player_error, self._player_end, **player_settings
-        )
+        if is_gui:
+            self.core.AudioPlayer.play(
+                station["url"], self._player_error, self._player_end, **player_settings
+            )
+        else:
+            self.core.AudioPlayer.play_no_gui(station["url"], on_error, on_end)
 
     def _main_add_option(self, name, icon, callback, main_grid, pos):
         grid = Gtk.Grid()
         button = Gtk.Button()
         label = Gtk.Label(name)
 
         image = self.core.IconHelper.get_icon(icon)
@@ -421,22 +435,22 @@
 
     def show_main_menu(self, button=None):
         self._clean_up()
         self.window_history = []
 
         self._update_previous_window(self.show_main_menu, button)
 
-        self.localizer.install()
-
         grid = Gtk.Grid()
         self.current_container = grid
 
         go_back = Gtk.Button()
         go_back.set_image(
-            self.core.IconHelper.get_icon("go-previous", size=Gtk.IconSize.MENU)
+            self.core.IconHelper.get_icon(
+                "go-previous-symbolic", size=Gtk.IconSize.MENU
+            )
         )
         go_back.connect("clicked", self._return)
         go_back.set_halign(Gtk.Align.START)
 
         self._main_add_option(
             _("Search by region"),
             "map-search-outline",
```

### Comparing `OpenRadio-1.0/OpenRadio/modules/InternetRadio/__init__.py` & `OpenRadio-1.1.0/OpenRadio/modules/InternetRadio/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,73 +1,110 @@
 import pyradios
 from gi.repository import Gtk, GdkPixbuf, GLib
+
 from OpenRadio.core.ModuleClass import ModuleClass
 from OpenRadio.core.const import LOG_LEVEL, LOG_HANDLER, DEFAULT_ICON_SIZE
+from OpenRadio.core.Localizer import ModuleLocalizer
+
 from .UI import UI
-import requests
+
 from urllib.parse import urlparse
+
 import logging
 
+
+import socket
+
+DOMAIN = "builtin.internetradio"
+
 MODULE_CLASS_NAME = "InternetRadio"
 
 LOGGER = logging.getLogger(__name__)
 LOGGER.setLevel(LOG_LEVEL)
 LOGGER.addHandler(LOG_HANDLER)
 
 
+# Class implementing a simple internet radio
 class InternetRadio(ModuleClass):
     NAME = "InternetRadio"
-    DOMAIN = "builtin.internetradio"
+    DOMAIN = DOMAIN
 
     USES_GUI = True
     USES_CONFIG = False
     USES_HTTP = False
     USES_FAVORITES = True
 
+    ENABLED = True
+
     def __init__(self):
-        self.ICON = self.core.IconHelper.get_icon(
-            "applications-internet"
-        )
-        browser = pyradios.RadioBrowser()
-        self.localizer = self.core.Localizer.get_translator(self.DOMAIN)
-        self.browser = browser
-        self.UI = UI(self, LOGGER, self.browser)
+        self.ICON = self.core.IconHelper.get_icon("applications-internet")
+
+        self.browser = None
+
+        self.UI = UI(self, LOGGER)
+
+    def _return_error(self, button):
+        self.error_grid.destroy()
+        self.core.Window.show_menu()
+
+    def _create_browser(self):
+        try:
+            browser = pyradios.RadioBrowser()
+            self.browser = browser
+        except socket.gaierror:
+            self.browser = None
+
+            return False
+        return True
 
     def on_clear(self):
+        self.browser = None
         self.UI._clean_up()
 
     def on_get_favorites(self):
         config = self.core.Settings.get_config(self.DOMAIN)
         return config
 
     def on_set_favorite(self, station):
         current_favorites = self.core.Settings.get_config(self.DOMAIN)
-        current_favorites[f"""{station["name"]} ({self.NAME})"""] = station[
-            "stationuuid"
+        current_favorites[f"""{station["name"]} ({self.NAME})"""] = [
+            station["stationuuid"]
         ]
         self.core.Settings.save_config(self.DOMAIN, current_favorites)
 
     def on_remove_favorite(self, station):
         current_favorites = self.core.Settings.get_config(self.DOMAIN)
         current_favorites.pop(f"""{station["name"]} ({self.NAME})""")
         self.core.Settings.save_config(self.DOMAIN, current_favorites)
 
-    def on_favorite_info(self, station_uuid):
-        session = requests.session()
+    def on_play_favorite(self, on_end, on_error, station_uuid):
+        if not self.browser:
+            internet = self._create_browser()
+            if not internet:
+                return True
 
         station = self.browser.station_by_uuid(station_uuid)[0]
+        self.UI._play_station(
+            None, station, is_gui=False, on_end=on_end, on_error=on_error
+        )
+        return False
 
-        icon = self.UI.icon_thread._icon_from_station(station, session)
+    def on_stop_favorite(self, station_uuid):
+        self.core.AudioPlayer.stop()
 
-        favorite_info = {"icon": None, "name": station["name"], "mrl": station["url"]}
+    def on_show(self):
+        LOGGER.debug("Showing Main menu")
+        if not self.browser:
+            internet = self._create_browser()
 
-        if icon:
-            favorite_info["icon"] = icon
-        return favorite_info
+            if not internet:
+                grid = self.core.UIHelper.error_message(
+                    "No Internet connection", self._return_error
+                )
 
-    def on_play_favorite(self, station_uuid):
-        station = self.browser.station_by_uuid(station_uuid)
-        self.UI._play_station(None, station)
+                self.core.Window.add(grid)
+                self.core.Window.show_all()
+
+                self.error_grid = grid
+                return
 
-    def on_show(self):
-        LOGGER.debug("Showing Main menu")
         self.UI.show_main_menu()
```

### Comparing `OpenRadio-1.0/OpenRadio/modules/Settings/__init__.py` & `OpenRadio-1.1.0/OpenRadio/modules/Settings/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,28 @@
 from OpenRadio.core.ModuleClass import ModuleClass
 from OpenRadio.core.const import LOG_LEVEL, LOG_HANDLER
+from OpenRadio.core.Localizer import ModuleLocalizer
+
 from gi.repository import Gtk
+
 import logging
 
+DOMAIN = "builtin.settings"
+
+localizer = ModuleLocalizer(DOMAIN)
+translator = localizer.get_translator()
+_ = translator.gettext
+
 MODULE_CLASS_NAME = "SettingsModule"
 
 
+# Module handling the visualization of settings
 class SettingsModule(ModuleClass):
     NAME = "Settings"
-    DOMAIN = "builtin.settings"
+    DOMAIN = DOMAIN
 
     USES_GUI = True
     USES_HTTP = False
     USES_CONFIG = False
 
     def __init__(self):
         self.ICON = self.core.IconHelper.get_icon("emblem-system")
```

### Comparing `OpenRadio-1.0/OpenRadio.egg-info/SOURCES.txt` & `OpenRadio-1.1.0/OpenRadio.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -8,22 +8,35 @@
 OpenRadio.egg-info/PKG-INFO
 OpenRadio.egg-info/SOURCES.txt
 OpenRadio.egg-info/dependency_links.txt
 OpenRadio.egg-info/entry_points.txt
 OpenRadio.egg-info/requires.txt
 OpenRadio.egg-info/top_level.txt
 OpenRadio/assets/OpenRadio.icon
-OpenRadio/assets/bitmap.png
+OpenRadio/assets/OpenRadio.png
 OpenRadio/assets/icons/alarm-symbolic.svg
+OpenRadio/assets/icons/application-exit.png
+OpenRadio/assets/icons/applications-internet.png
+OpenRadio/assets/icons/dialog-information.png
+OpenRadio/assets/icons/emblem-system.png
 OpenRadio/assets/icons/globe-symbolic.svg
+OpenRadio/assets/icons/go-down-symbolic.svg
+OpenRadio/assets/icons/go-previous-symbolic.svg
+OpenRadio/assets/icons/go-up-symbolic.svg
+OpenRadio/assets/icons/list-add-symbolic.svg
 OpenRadio/assets/icons/map-search-outline.png
+OpenRadio/assets/icons/media-playback-pause-symbolic.svg
+OpenRadio/assets/icons/media-playback-start-symbolic.svg
+OpenRadio/assets/icons/media-playback-stop-symbolic.svg
+OpenRadio/assets/icons/network-wireless-hotspot-symbolic.svg
 OpenRadio/assets/icons/search-web.png
 OpenRadio/assets/icons/star-outline.png
 OpenRadio/assets/icons/star.png
 OpenRadio/assets/icons/tag-search-outline.png
+OpenRadio/assets/icons/user-trash-symbolic.svg
 OpenRadio/assets/icons/countries/ad.svg
 OpenRadio/assets/icons/countries/ae.svg
 OpenRadio/assets/icons/countries/af.svg
 OpenRadio/assets/icons/countries/ag.svg
 OpenRadio/assets/icons/countries/ai.svg
 OpenRadio/assets/icons/countries/al.svg
 OpenRadio/assets/icons/countries/am.svg
@@ -274,48 +287,74 @@
 OpenRadio/core/Exceptions.py
 OpenRadio/core/HTTPApi.py
 OpenRadio/core/IconHelper.py
 OpenRadio/core/Localizer.py
 OpenRadio/core/ModuleClass.py
 OpenRadio/core/ModuleHandler.py
 OpenRadio/core/Settings.py
+OpenRadio/core/UIHelper.py
 OpenRadio/core/Window.py
 OpenRadio/core/const.py
 OpenRadio/locales/core/de/LC_MESSAGES/core.mo
 OpenRadio/locales/core/en/LC_MESSAGES/core.mo
 OpenRadio/locales/modules/builtin.about/de/LC_MESSAGES/builtin.about.mo
 OpenRadio/locales/modules/builtin.about/en/LC_MESSAGES/builtin.about.mo
+OpenRadio/locales/modules/builtin.alarm/de/LC_MESSAGES/builtin.alarm.mo
+OpenRadio/locales/modules/builtin.alarm/en/LC_MESSAGES/builtin.alarm.mo
 OpenRadio/locales/modules/builtin.clock/de/LC_MESSAGES/builtin.clock.mo
+OpenRadio/locales/modules/builtin.clock/en/LC_MESSAGES/builtin.clock.mo
+OpenRadio/locales/modules/builtin.core_settings/de/LC_MESSAGES/builtin.core_settings.mo
+OpenRadio/locales/modules/builtin.core_settings/en/LC_MESSAGES/builtin.core_settings.mo
+OpenRadio/locales/modules/builtin.dab/de/LC_MESSAGES/builtin.dab.mo
+OpenRadio/locales/modules/builtin.dab/en/LC_MESSAGES/builtin.dab.mo
 OpenRadio/locales/modules/builtin.exit/de/LC_MESSAGES/builtin.exit.mo
+OpenRadio/locales/modules/builtin.exit/en/LC_MESSAGES/builtin.exit.mo
 OpenRadio/locales/modules/builtin.internetradio/de/LC_MESSAGES/builtin.internetradio.mo
 OpenRadio/locales/modules/builtin.internetradio/en/LC_MESSAGES/builtin.internetradio.mo
 OpenRadio/locales/modules/builtin.settings/de/LC_MESSAGES/builtin.settings.mo
+OpenRadio/locales/modules/builtin.settings/en/LC_MESSAGES/builtin.settings.mo
 OpenRadio/locales/src/de/core/core.pot
 OpenRadio/locales/src/de/modules/builtin.about/builtin.about.pot
+OpenRadio/locales/src/de/modules/builtin.alarm/builtin.alarm.pot
 OpenRadio/locales/src/de/modules/builtin.clock/builtin.clock.pot
-OpenRadio/locales/src/de/modules/builtin.demo/builtin.demo.pot
+OpenRadio/locales/src/de/modules/builtin.core_settings/builtin.core_settings.pot
+OpenRadio/locales/src/de/modules/builtin.dab/builtin.dab.pot
 OpenRadio/locales/src/de/modules/builtin.exit/builtin.exit.pot
 OpenRadio/locales/src/de/modules/builtin.internetradio/builtin.internetradio.pot
 OpenRadio/locales/src/de/modules/builtin.settings/builtin.settings.pot
 OpenRadio/locales/src/en/core/core.pot
 OpenRadio/locales/src/en/modules/builtin.about/builtin.about.pot
+OpenRadio/locales/src/en/modules/builtin.alarm/builtin.alarm.pot
 OpenRadio/locales/src/en/modules/builtin.clock/builtin.clock.pot
-OpenRadio/locales/src/en/modules/builtin.demo/builtin.demo.pot
+OpenRadio/locales/src/en/modules/builtin.core_settings/builtin.core_settings.pot
+OpenRadio/locales/src/en/modules/builtin.dab/builtin.dab.pot
 OpenRadio/locales/src/en/modules/builtin.exit/builtin.exit.pot
 OpenRadio/locales/src/en/modules/builtin.internetradio/builtin.internetradio.pot
 OpenRadio/locales/src/en/modules/builtin.settings/builtin.settings.pot
 OpenRadio/locales/templates/core/core.pot
 OpenRadio/locales/templates/modules/builtin.about/builtin.about.pot
+OpenRadio/locales/templates/modules/builtin.alarm/builtin.alarm.pot
 OpenRadio/locales/templates/modules/builtin.clock/builtin.clock.pot
+OpenRadio/locales/templates/modules/builtin.core_settings/builtin.core_settings.pot
+OpenRadio/locales/templates/modules/builtin.dab/builtin.dab.pot
 OpenRadio/locales/templates/modules/builtin.exit/builtin.exit.pot
 OpenRadio/locales/templates/modules/builtin.internetradio/builtin.internetradio.pot
 OpenRadio/locales/templates/modules/builtin.settings/builtin.settings.pot
 OpenRadio/modules/About/__init__.py
-OpenRadio/modules/Alarm/TimeThread.py
+OpenRadio/modules/Alarm/AlarmScheduler.py
+OpenRadio/modules/Alarm/AlarmWidget.py
+OpenRadio/modules/Alarm/RingUI.py
 OpenRadio/modules/Alarm/TimeWidget.py
+OpenRadio/modules/Alarm/UI.py
 OpenRadio/modules/Alarm/__init__.py
+OpenRadio/modules/Alarm/const.py
 OpenRadio/modules/Clock/__init__.py
+OpenRadio/modules/CoreSettings/__init__.py
+OpenRadio/modules/DAB/__init__.py
+OpenRadio/modules/DAB/const.py
+OpenRadio/modules/DAB/dab_helper.py
+OpenRadio/modules/DAB/player.py
 OpenRadio/modules/Exit/__init__.py
 OpenRadio/modules/InternetRadio/IconThread.py
 OpenRadio/modules/InternetRadio/UI.py
 OpenRadio/modules/InternetRadio/__init__.py
 OpenRadio/modules/Settings/__init__.py
```

