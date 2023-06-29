# Comparing `tmp/Lopster-0.1.2.tar.gz` & `tmp/Lopster-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Lopster-0.1.2.tar", last modified: Sat Jun 10 08:06:15 2023, max compression
+gzip compressed data, was "Lopster-0.1.3.tar", last modified: Wed Jun 28 15:24:59 2023, max compression
```

## Comparing `Lopster-0.1.2.tar` & `Lopster-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 08:06:15.086931 Lopster-0.1.2/
-drwxrwxrwx   0        0        0        0 2023-06-10 08:06:15.055672 Lopster-0.1.2/Lopster/
--rw-rw-rw-   0        0        0    10302 2023-06-10 08:04:38.000000 Lopster-0.1.2/Lopster/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-10 08:06:15.086931 Lopster-0.1.2/Lopster.egg-info/
--rw-rw-rw-   0        0        0      235 2023-06-10 08:06:14.000000 Lopster-0.1.2/Lopster.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-06-10 08:06:14.000000 Lopster-0.1.2/Lopster.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 08:06:14.000000 Lopster-0.1.2/Lopster.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-10 08:06:14.000000 Lopster-0.1.2/Lopster.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-10 08:06:14.000000 Lopster-0.1.2/Lopster.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      235 2023-06-10 08:06:15.086931 Lopster-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-10 08:06:15.086931 Lopster-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      383 2023-06-10 08:02:52.000000 Lopster-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-28 15:24:59.925627 Lopster-0.1.3/
+drwxrwxrwx   0        0        0        0 2023-06-28 15:24:59.894376 Lopster-0.1.3/Lopster/
+-rw-rw-rw-   0        0        0     8283 2023-06-28 15:24:15.000000 Lopster-0.1.3/Lopster/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-28 15:24:59.925627 Lopster-0.1.3/Lopster.egg-info/
+-rw-rw-rw-   0        0        0      235 2023-06-28 15:24:59.000000 Lopster-0.1.3/Lopster.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2023-06-28 15:24:59.000000 Lopster-0.1.3/Lopster.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-28 15:24:59.000000 Lopster-0.1.3/Lopster.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-28 15:24:59.000000 Lopster-0.1.3/Lopster.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-28 15:24:59.000000 Lopster-0.1.3/Lopster.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      235 2023-06-28 15:24:59.925627 Lopster-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-28 15:24:59.925627 Lopster-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      383 2023-06-28 15:24:34.000000 Lopster-0.1.3/setup.py
```

### Comparing `Lopster-0.1.2/Lopster/__init__.py` & `Lopster-0.1.3/Lopster/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
 class FakeEnemy:
     typ = "Enemy"
     x = 0
     y = 0
     h = 0
     w = 0
-    def update(): return print()
+    def update(self): return print()
 
     def __init__(self, _x, _y, _h, _w, _update):
         self.x = _x
         self.y = _y
         self.h = _h
         self.w = _w
         self.update = _update
@@ -197,19 +197,19 @@
     h = 0
     w = 0
 
     def __init__(self, height, width):
         self._h = height
         self._w = width
 
-    def Distance(x, y, x1, y1):
-        distance = math.sqrt((x1 - x) ** 2 + (y1 - y) ** 2)
+    def Distance(self, obj, obj1):
+        distance = math.sqrt((obj1.x - obj.x) ** 2 + (obj1.y - obj.y) ** 2)
         return distance
 
-    def Side(x, y, x1, y1):
+    def Side(self, x, y, x1, y1):
         if x1 > x:
             return "right"
         elif x1 < x:
             return "left"
         elif y1 > y:
             return "bottom"
         elif y1 < y:
@@ -243,71 +243,14 @@
         for card in map:
             if not type(card) == "tuple":
                 drawMap[card](self.window, "NoN")
             else:
                 for subCard in card:
                     drawMap[subCard](self.window, card)
 
-
-# class Bank:
-#     def __init__(self, src):
-#         self.src = src
-#
-#     def cash(self):
-#         text = []
-#         for obj in Enemy._object:
-#             text.append(obj.cash())
-#
-#         with open(self.src, "w") as file:
-#             file.write("\n".join(text))
-#
-#     def casher(self):
-#         with open(self.src, "r") as file:
-#             texts = file.read().split(";")
-#
-#             i = 0
-#             while i < len(texts):
-#                 text = texts[i].split("\n")
-#
-#                 variables = {}
-#                 functions = {}
-#
-#                 for line in text:
-#                     line = line.strip()
-#                     if not line:
-#                         continue
-#
-#                     if line.startswith("["):
-#                         class_name = line[1:-1]
-#                         instance_name = text[text.index(line) + 1].strip()
-#                         variables[instance_name] = {}
-#
-#                     elif line.startswith("dec"):
-#                         parts = line.split(" ")
-#                         function_name = parts[1]
-#                         function_body = " ".join(parts[2:])
-#
-#                         functions[function_name] = eval(function_body, variables)
-#
-#                     elif line.startswith("init"):
-#                         parts = line.split(" ")
-#                         instance_name = parts[1]
-#                         arguments = parts[2:]
-#
-#                         instance_variables = variables[instance_name]
-#                         for i, argument in enumerate(arguments):
-#                             if argument.startswith("@"):
-#                                 variable_name = argument[1:]
-#                                 argument_value = variables[variable_name]
-#                             else:
-#                                 argument_value = eval(argument, variables)
-#                             instance_variables[f"arg{i+1}"] = argument_value
-#
-#                 i += 1
-
 class RunLopster:
     _fps = 16
 
     def __init__(self, window_size, title, icon, update, fps):
         self._window_size = window_size
         self._title = title
         self._update = update
@@ -322,15 +265,16 @@
         icon = self._icon
 
         pygame.init()
         window = pygame.display.set_mode(window_size)
 
         pygame.display.set_caption(title)
 
-        pygame.display.set_icon(pygame.image.load(icon))
+        if(icon!=None):
+            pygame.display.set_icon(pygame.image.load(icon))
 
         is_run = True
 
         while is_run:
             update(window)
 
             pygame.time.delay(1000 // fps)
@@ -344,8 +288,8 @@
                     obj.update(window, obj)
 
             pygame.display.update()
 
         pygame.quit()
 
 
-__all__ = ['Enemy', 'FakeEnemy', 'Player', 'MathMap', 'Map', 'RunLopster', 'Sprite']
+__all__ = ['Enemy', 'FakeEnemy', 'Player', 'MathMap', 'Map', 'RunLopster']
```

