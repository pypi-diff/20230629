# Comparing `tmp/AshCrypt-1.2.0.tar.gz` & `tmp/AshCrypt-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AshCrypt-1.2.0.tar", last modified: Tue Jun 27 16:08:10 2023, max compression
+gzip compressed data, was "AshCrypt-1.2.1.tar", last modified: Thu Jun 29 13:13:10 2023, max compression
```

## Comparing `AshCrypt-1.2.0.tar` & `AshCrypt-1.2.1.tar`

### file list

```diff
@@ -1,33 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 16:08:10.045924 AshCrypt-1.2.0/
-drwxrwxrwx   0        0        0        0 2023-06-27 16:08:09.973736 AshCrypt-1.2.0/AshCrypt/
--rw-rw-rw-   0        0        0     5157 2023-06-17 18:15:01.000000 AshCrypt-1.2.0/AshCrypt/Ash.py
--rw-rw-rw-   0        0        0    34125 2023-06-27 15:57:29.000000 AshCrypt-1.2.0/AshCrypt/AshCryptGUI.py
--rw-rw-rw-   0        0        0     8855 2023-06-27 15:57:29.000000 AshCrypt-1.2.0/AshCrypt/AshDatabase.py
--rw-rw-rw-   0        0        0     4128 2023-06-27 15:57:29.000000 AshCrypt-1.2.0/AshCrypt/AshFileCrypt.py
--rw-rw-rw-   0        0        0     2074 2023-06-17 18:15:01.000000 AshCrypt-1.2.0/AshCrypt/AshTextCrypt.py
--rw-rw-rw-   0        0        0     6450 2023-06-27 15:57:29.000000 AshCrypt-1.2.0/AshCrypt/CliCrypt.py
--rw-rw-rw-   0        0        0    14164 2023-06-27 15:57:29.000000 AshCrypt-1.2.0/AshCrypt/README.md
--rw-rw-rw-   0        0        0       91 2023-06-17 18:15:01.000000 AshCrypt-1.2.0/AshCrypt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 16:08:10.028504 AshCrypt-1.2.0/AshCrypt/__pycache__/
--rw-rw-rw-   0        0        0     6435 2023-06-27 15:57:46.000000 AshCrypt-1.2.0/AshCrypt/__pycache__/Ash.cpython-310.pyc
--rw-rw-rw-   0        0        0    19153 2023-06-27 15:57:46.000000 AshCrypt-1.2.0/AshCrypt/__pycache__/AshCryptGUI.cpython-310.pyc
--rw-rw-rw-   0        0        0     7808 2023-06-27 15:57:46.000000 AshCrypt-1.2.0/AshCrypt/__pycache__/AshDatabase.cpython-310.pyc
--rw-rw-rw-   0        0        0     3515 2023-06-27 15:57:46.000000 AshCrypt-1.2.0/AshCrypt/__pycache__/AshFileCrypt.cpython-310.pyc
--rw-rw-rw-   0        0        0     2650 2023-06-27 15:57:46.000000 AshCrypt-1.2.0/AshCrypt/__pycache__/AshTextCrypt.cpython-310.pyc
--rw-rw-rw-   0        0        0      248 2023-06-27 15:57:46.000000 AshCrypt-1.2.0/AshCrypt/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     1294 2023-06-27 15:57:46.000000 AshCrypt-1.2.0/AshCrypt/__pycache__/qr.cpython-310.pyc
--rw-rw-rw-   0        0        0     1045 2023-06-17 18:15:01.000000 AshCrypt-1.2.0/AshCrypt/qr.py
-drwxrwxrwx   0        0        0        0 2023-06-27 16:08:10.037808 AshCrypt-1.2.0/AshCrypt/unittests/
--rw-rw-rw-   0        0        0       25 2023-06-27 15:57:29.000000 AshCrypt-1.2.0/AshCrypt/unittests/__init__.py
--rw-rw-rw-   0        0        0     3402 2023-06-27 15:57:29.000000 AshCrypt-1.2.0/AshCrypt/unittests/unittestAsh.py
-drwxrwxrwx   0        0        0        0 2023-06-27 16:08:09.998617 AshCrypt-1.2.0/AshCrypt.egg-info/
--rw-rw-rw-   0        0        0    15187 2023-06-27 16:08:09.000000 AshCrypt-1.2.0/AshCrypt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      765 2023-06-27 16:08:09.000000 AshCrypt-1.2.0/AshCrypt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 16:08:09.000000 AshCrypt-1.2.0/AshCrypt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2023-06-27 16:08:09.000000 AshCrypt-1.2.0/AshCrypt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-27 16:08:09.000000 AshCrypt-1.2.0/AshCrypt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2023-06-17 16:19:54.000000 AshCrypt-1.2.0/LICENSE
--rw-rw-rw-   0        0        0    15187 2023-06-27 16:08:10.043934 AshCrypt-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0    17100 2023-06-27 15:57:29.000000 AshCrypt-1.2.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-27 16:08:10.046925 AshCrypt-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1613 2023-06-27 16:06:57.000000 AshCrypt-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 13:13:10.691218 AshCrypt-1.2.1/
+drwxrwxrwx   0        0        0        0 2023-06-29 13:13:10.669014 AshCrypt-1.2.1/AshCrypt/
+-rw-rw-rw-   0        0        0     5157 2023-06-17 18:15:01.000000 AshCrypt-1.2.1/AshCrypt/Ash.py
+-rw-rw-rw-   0        0        0    35745 2023-06-28 15:21:31.000000 AshCrypt-1.2.1/AshCrypt/AshCryptGUI.py
+-rw-rw-rw-   0        0        0     8855 2023-06-29 12:59:01.000000 AshCrypt-1.2.1/AshCrypt/AshDatabase.py
+-rw-rw-rw-   0        0        0     4128 2023-06-27 15:57:29.000000 AshCrypt-1.2.1/AshCrypt/AshFileCrypt.py
+-rw-rw-rw-   0        0        0     2074 2023-06-17 18:15:01.000000 AshCrypt-1.2.1/AshCrypt/AshTextCrypt.py
+-rw-rw-rw-   0        0        0     6660 2023-06-29 12:50:18.000000 AshCrypt-1.2.1/AshCrypt/CliCrypt.py
+-rw-rw-rw-   0        0        0    18472 2023-06-29 13:08:37.000000 AshCrypt-1.2.1/AshCrypt/README.md
+-rw-rw-rw-   0        0        0       91 2023-06-17 18:15:01.000000 AshCrypt-1.2.1/AshCrypt/__init__.py
+-rw-rw-rw-   0        0        0     1045 2023-06-17 18:15:01.000000 AshCrypt-1.2.1/AshCrypt/qr.py
+drwxrwxrwx   0        0        0        0 2023-06-29 13:13:10.686390 AshCrypt-1.2.1/AshCrypt/unittests/
+-rw-rw-rw-   0        0        0       25 2023-06-27 15:57:29.000000 AshCrypt-1.2.1/AshCrypt/unittests/__init__.py
+-rw-rw-rw-   0        0        0     3402 2023-06-27 15:57:29.000000 AshCrypt-1.2.1/AshCrypt/unittests/unittestAsh.py
+drwxrwxrwx   0        0        0        0 2023-06-29 13:13:10.681802 AshCrypt-1.2.1/AshCrypt.egg-info/
+-rw-rw-rw-   0        0        0    19499 2023-06-29 13:13:10.000000 AshCrypt-1.2.1/AshCrypt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      440 2023-06-29 13:13:10.000000 AshCrypt-1.2.1/AshCrypt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 13:13:10.000000 AshCrypt-1.2.1/AshCrypt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2023-06-29 13:13:10.000000 AshCrypt-1.2.1/AshCrypt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-29 13:13:10.000000 AshCrypt-1.2.1/AshCrypt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2023-06-17 16:19:54.000000 AshCrypt-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0    19499 2023-06-29 13:13:10.691218 AshCrypt-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0    21651 2023-06-29 13:08:37.000000 AshCrypt-1.2.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-29 13:13:10.692231 AshCrypt-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1629 2023-06-29 13:08:37.000000 AshCrypt-1.2.1/setup.py
```

### Comparing `AshCrypt-1.2.0/AshCrypt/Ash.py` & `AshCrypt-1.2.1/AshCrypt/Ash.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.2.0/AshCrypt/AshCryptGUI.py` & `AshCrypt-1.2.1/AshCrypt/AshCryptGUI.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,365 +36,14 @@
 
 lowerFrame = tk.Frame(master=object, width=1000 ,height=260)
 lowerFrame.place(x=500,y=540)
 
 
 '''--------------------------------------FRAMING DONE--------------------------------------------------------------'''
 
-
-'''-------------------------------TEXT DECRYPTION/ENCRYPTION STARTED---------------------------------------------------'''
-
-
-
-
-def encryption():
-    m = inputfield1_1.get()
-    if AF.CryptFile.keyverify(mainkeyvar.get()) == 1 and keySelectionFlag.get() == 1:
-        if len(m) > 200 :
-            outputvar1.set('Too Long')
-        else :
-            if inputfield1_1.get():
-                progressbar.start()
-                a = AT.Crypt(m, mainkeyvar.get())
-                b =  a.encrypt()[1]
-                outputvar1.set(b.__str__())
-                if var1.get() == 1:
-                    qr.tqr(b)
-
-
-def decryption():
-    n =inputfield2_1.get()
-    if AF.CryptFile.keyverify(mainkeyvar.get()) == 1 and keySelectionFlag.get() == 1:
-        if inputfield2_1.get():
-            progressbar2.start()
-            a = AT.Crypt(n, mainkeyvar.get())
-            b = a.decrypt()[1]
-            outputvar2.set(b.__str__())
-            if var2.get() == 1:
-                if not len(b) > 200:
-                    qr.tqr(b)
-
-def func1():
-    if var1.get() == 1 :
-        label1.config(text='QR ON')
-    else:
-        label1.config(text='QR OFF')
-
-def func2():
-    if var2.get() == 1 :
-        label2.config(text='QR ON')
-    else:
-        label2.config(text='QR OFF')
-
-
-button1 = tk.Button(master=textFrame1 ,text='ENCRYPT', command=encryption, bootstyle='light outline').place(relx=0.42, rely=0.73)
-button2 = tk.Button(master=textFrame2 , text='DECRYPT', command=decryption,bootstyle='light outline').place(relx=0.42,rely=0.8)
-
-inputfield1_1 = tk.StringVar()
-textfield1_1 = tk.Entry(master=textFrame1 ,
-                        width=20,
-                        font='Calibre 11 bold',
-                        textvariable=inputfield1_1).place(relx=0.29 , rely=0.30)
-
-inputfield2_1 = tk.StringVar(value='')
-textfield2_1 = tk.Entry(master=textFrame2 ,
-                        font='Calibre 11 bold',
-                        width=20,
-                        textvariable=inputfield2_1).place(relx=0.290 ,rely=0.38)
-
-namelabel1 = tk.Label(master=textFrame1 ,
-                      text='TEXT ENCRYPTION',
-                      font='Calibre 20 bold' ,
-                      )
-namelabel1.place(relx=0.190 ,rely=0.10)
-namelabel2 = tk.Label(master=textFrame2 ,
-                      text='TEXT DECRYPTION' ,
-                      font='Calibre 20 bold'  ,
-                      ).place(relx=0.190 ,rely=0.200)
-
-outputvar1 = tk.StringVar(value='')
-outputlabel1 =  tk.Entry(master= textFrame1,
-                         textvariable=outputvar1,
-                         font='terminal 11 bold').place(relx= 0.02,
-                                                       rely= 0.48 ,
-                                                       width= 480,
-                                                       height= 50)
-outputvar2 = tk.StringVar(value='')
-outputlabel2 = tk.Entry(master=textFrame2 ,
-                        textvariable= outputvar2 ,
-                        font='terminal 11 bold').place(relx= 0.02,
-                                                       rely= 0.55,
-                                                       width= 480,
-                                                       height= 50)
-
-
-
-label1 = tk.Label(master=textFrame1,text='QR',font=('terminal',17))
-label1.place(relx=0.2,rely=0.75)
-var1 = tk.IntVar()
-mytoolbutt3 = tk.Checkbutton(bootstyle='success , round-toggle',
-                        master=textFrame1,
-                        variable=var1,
-                        offvalue=0,
-                        command=func1)
-
-mytoolbutt3.place(relx=0.1,rely=0.77)
-
-
-
-
-label2 = tk.Label(master=textFrame2,text='QR',font=('terminal',17))
-label2.place(relx=0.2,rely=0.82)
-var2 = tk.IntVar()
-mytoolbutt6 = tk.Checkbutton(bootstyle='success , round-toggle',
-                        master=textFrame2,
-                        variable=var2,
-                        offvalue=0,
-                        command=func2)
-
-mytoolbutt6.place(relx=0.1,rely=0.84)
-
-
-progressbar = tk.Progressbar(master=textFrame1,mode='indeterminate',style='secondary',length=100,)
-progressbar.place(relx=0.05,rely=0.34)
-
-progressbar2 = tk.Progressbar(master=textFrame2,mode='indeterminate',style='secondary',length=100,)
-progressbar2.place(relx=0.05,rely=0.42)
-
-'''-------------------------------TEXT DECRYPTION/ENCRYPTION ENDED---------------------------------------------------'''
-
-
-
-
-
-
-
-
-
-'''-------------------------------FILE ENCRYPTION/DECRYPTION STARTED--------------------------------------------'''
-
-
-filepathlabel = tk.Label(master=frameFile1 ,
-                      text='FILE PATH',
-                      font='Calibre 20 bold' ,
-                      )
-filepathlabel.place(relx=0.335,rely=0.10)
-
-
-resultvarfile = tk.StringVar(value='                  ..RESULT..')
-resultLabelfile =  tk.Label(master= frameFile1,
-                         textvariable=resultvarfile,
-                         font='terminal 13 bold').place(
-                                                       rely= 0.55 ,
-                                                       )
-
-
-def encFile():
-    global fileaccessSemo ,add_enc_to_db ,main_db_conn,mainkey
-    if 1 :
-        if keySelectionFlag.get() != 0:
-            filename = filenameStringVar.get().strip()
-            key = mainkey
-            target = AF.CryptFile(filename, key)
-            a = target.encrypt()
-            if a == 1:
-                filename = filename + '.crypt'
-                filenameStringVar.set(filename)
-                resultvarfile.set('    Encrypted Successfully / added .crypt')
-                if encfiletoolbuttvar.get() == 1:
-                    with open(filename,'rb') as f:
-                        file_content = f.read()
-                    main_db_conn.insert(filename,file_content, outputKeyref.get().strip())
-            if a == 2:
-                resultvarfile.set('                 File is Empty')
-            if a == 3:
-                resultvarfile.set("               File Doesn't Exist")
-            if a == 0:
-                resultvarfile.set("                  Can't Encrypt")
-            if  a == 4:
-                resultvarfile.set('                     ERROR')
-            if a == 5 :
-                resultvarfile.set('          ERROR : Key is Not 512-bit')
-            if a == 6:
-                resultvarfile.set('       ERROR : File is already encrypted')
-            elif a == 7:
-                resultvarfile.set(' ERROR : Given a directory instead of a file')
-
-def decfile():
-    global fileaccessSemo,add_dec_to_db,main_db_conn,mainkey
-    if 1:
-        if keySelectionFlag.get() != 0:
-            filename =filenameStringVar.get().strip()
-            key = mainkey
-            target = AF.CryptFile(filename, key)
-            a = target.decrypt()
-            if a == 1:
-                filename = os.path.splitext(filename)[0]
-                filenameStringVar.set(filename)
-                resultvarfile.set('   Decrypted Successfully + removed .crypt')
-                if decfiletoolbuttvar.get() == 1:
-                    with open(filename,'rb') as f:
-                        file_content = f.read()
-                    main_db_conn.insert(filename,file_content, outputKeyref.get().strip())
-            if a == 2:
-                resultvarfile.set('                 File is Empty')
-            if a == 3:
-                resultvarfile.set("               File Doesn't Exist")
-            if a == 0:
-                resultvarfile.set("                 Can't Decrypt")
-            if  a == 4:
-                resultvarfile.set('                     ERROR')
-            elif a == 5 :
-                resultvarfile.set('          ERROR : Key is Not 512-bit')
-            if a == 6:
-                resultvarfile.set('       ERROR : File is already decrypted')
-            elif a == 7:
-                resultvarfile.set(' ERROR : Given a directory instead of a file')
-
-
-
-
-
-
-encryptionfilebutton = tk.Button(master=frameFile1 ,text='ENCRYPT FILE', command=encFile, bootstyle='warning outline').place(relx=0.25, rely=0.73)
-decryptionfilebutton = tk.Button(master=frameFile1 , text='DECRYPT FILE', command=decfile,bootstyle='warning outline').place(relx=0.55,rely=0.73)
-
-filenameStringVar = tk.StringVar(value='')
-
-filenametext = tk.Entry(master=frameFile1 ,
-                        width=31,
-                        font='Calibre 15 bold',
-                        textvariable=filenameStringVar).place(relx=0.05, rely=0.30)
-
-
-
-addtodbLabel = tk.Label(master=frameFile1,text='ADD TO DATABASE',font=('Calibre',11),bootstyle='warning')
-addtodbLabel.place(relx=0.35,rely=0.908)
-
-add_enc_to_db = 0
-def encToggleButtFunc():
-    global add_enc_to_db
-    if encfiletoolbuttvar == 1:
-        add_enc_to_db = 1
-    else:
-        add_enc_to_db = 0
-
-add_dec_to_db = 0
-def decToggleButtFunc():
-    global add_dec_to_db
-    if decfiletoolbuttvar == 1:
-        add_dec_to_db = 1
-    else:
-        add_dec_to_db = 0
-
-encfiletoolbuttvar = tk.IntVar()
-encfiletoolbutt = tk.Checkbutton(bootstyle='warning , round-toggle',
-                        master=frameFile1,
-                        variable=encfiletoolbuttvar,
-                        offvalue=0,
-                        onvalue=1,
-                        command=encToggleButtFunc)
-encfiletoolbutt.state(['disabled'])
-encfiletoolbutt.place(relx=0.25,rely=0.92)
-
-
-decfiletoolbuttvar = tk.IntVar()
-decfiletoolbutt = tk.Checkbutton(bootstyle='warning , round-toggle',
-                        master=frameFile1,
-                        variable=decfiletoolbuttvar,
-                        offvalue=0,
-                        command=decToggleButtFunc)
-decfiletoolbutt.state(['disabled'])
-decfiletoolbutt.place(relx=0.717,rely=0.92)
-
-
-
-
-keySelectionFlag = tk.IntVar(value=0)
-def mainKeyWrapper():
-    global success_keysdb_connection_blocker,mainkey
-    if AF.CryptFile.keyverify(mainkeyvar.get().strip()) == 1 :
-        mainkey = mainkeyvar.get().strip()
-        keyrefGen()
-        keyselectionvar.set('       SELECTED')
-        keySelectionFlag.set(1)
-        if success_keysdb_connection_blocker and os.path.isfile(filenameStringVar.get().strip()):
-            keys_db_conn.insert(filenameStringVar.get().strip(),mainkey,outputKeyref.get())
-        if success_keysdb_connection_blocker and not os.path.isfile(filenameStringVar.get().strip()):
-            keys_db_conn.insert('STANDALONE',mainkey,outputKeyref.get())
-
-    else :
-        keySelectionFlag.set(0)
-        keyselectionvar.set('     NOT SELECTED')
-
-
-
-mainkeyLabel = tk.Label(master=frameFile2 ,
-                      text='MAIN KEY' ,
-                      font='Calibre 20 bold',
-                      bootstyle='info',
-                      ).place(relx=0.3 ,rely=0.075)
-
-
-mainkeyvar = tk.StringVar()
-mainkeyEntry = tk.Entry(master=frameFile2 ,
-                        font='Calibre 14 bold',
-                        textvariable=mainkeyvar,
-                        width=29
-                        ).place(relx=0.09 ,rely=0.29)
-
-
-def keyrefGen():
-    ref = '#'
-    for _ in range(6):
-        character = secrets.choice(string.ascii_letters + string.digits + '$' + '?' + '&' + '@' + '!' + '-' + '+')
-        ref += character
-    outputKeyref.set(ref)
-
-
-
-outputKeyref = tk.StringVar(value='#XXXXXX')
-keyrefLabel = tk.Label(master=frameFile2,textvariable=outputKeyref,bootstyle='secondary',font=('terminal',12))
-keyrefLabel.place(relx=0.712,rely=0.12)
-
-keySelectButton = tk.Button(master=frameFile2 ,text='SELECT KEY', command=mainKeyWrapper, bootstyle='info outline').place(relx=0.6725, rely=0.5)
-
-
-keyselectionvar = tk.StringVar(value='   KEY NOT SELECTED')
-keyselectionLabel = tk.Label(master=frameFile2 ,
-                        textvariable= keyselectionvar ,
-                        bootstyle='info',
-                        font='terminal 11 bold').place(relx= 0.15 ,
-                                        rely= 0.465,
-                                        height= 50)
-
-
-
-def genMainKey():
-    keyGenVar.set(AF.CryptFile.genkey())
-
-
-keyGenVar = tk.StringVar(value='')
-keyGenEntry = tk.Entry(master=frameFile2 ,
-                        font='terminal 15 bold',
-                        textvariable=keyGenVar,
-                        width=14,
-                        show='').place(relx=0.1 ,rely=0.69)
-
-keyButton = tk.Button(master=frameFile2 ,
-                      text='GENERATE',
-                      command=genMainKey,
-                      bootstyle='success outline').place(relx=0.671, rely=0.7)
-
-
-'''-------------------------------FILE ENCRYPTION/DECRYPTION ENDED--------------------------------------------'''
-
-
-
-
 '''--------------------------------------DATA BASE FRAME STARTED------------------------------------------------'''
 
 
 databaseFrame = tk.Frame(master=object,height=800, width=500)
 databaseFrame.place(rely=0, relx=0)
 
 console_label = tk.Label(master=databaseFrame, text='DATABASE OUTPUT CONSOLE', font='Terminal 15 bold')
@@ -457,23 +106,28 @@
                             f.write(eJSON)
                         db_display_text.insert(tk.END, f"Successful fetch !\n\nCheck the 'output.json' file in the"
                                                        f"chosen path :\n\n'{usable_real_path}'")
                     if int(idd) == last_id:
                         db_display_text.delete('1.0', tk.END)
                         db_display_text.insert(tk.END, 'Chosen last ID\n\n')
                         to_json_path = os.path.join(usable_real_path,'output.json')
-                        with open(to_json_path, 'w') as f:
-                            eBuffer = {}
-                            for e in conn.content_by_id(int(idd)):
-                                eBuffer['ID_' + e[0].__str__()] = [{'Filename': e[1]}, {'Content': e[2].__str__()},
-                                                                   {'KeyRef': e[3]}]
-                            eJSON = json.dumps(eBuffer, indent=2)
-                            f.write(eJSON)
-                        db_display_text.insert(tk.END, f"Successful fetch !\n\nCheck the 'output.json' file in the"
-                                                       f"the chosen path :\n\n'{usable_real_path}'")
+                        try:
+                            with open(to_json_path, 'w') as f:
+                                eBuffer = {}
+                                for e in conn.content_by_id(int(idd)):
+                                    eBuffer['ID_' + e[0].__str__()] = [{'Filename': e[1]}, {'Content': e[2].__str__()},
+                                                                       {'KeyRef': e[3]}]
+                                eJSON = json.dumps(eBuffer, indent=2)
+                                f.write(eJSON)
+                            db_display_text.insert(tk.END, f"Successful fetch !\n\nCheck the 'output.json' file in the"
+                                                           f"the chosen path :\n\n'{usable_real_path}'")
+                        except:
+                            db_display_text.delete('1.0', tk.END)
+                            db_display_text.insert(tk.END,"ERROR \n\nCheck the validity of 'output.json' file"
+                                                          "\n\nCheck if the database is faulty\n")
                     elif int(idd) > last_id:
                         db_display_text.delete('1.0', tk.END)
                         db_display_text.insert(tk.END, 'Given ID is greater than the highest available ID')
             else:
                 db_display_text.delete('1.0', tk.END)
                 db_display_text.insert(tk.END, 'ID must be strictly greater than 0')
         except:
@@ -622,75 +276,83 @@
         usable_real_path,db_path_blocker,\
         success_maindb_connection_blocker,\
         main_db_conn,\
         maindbname
 
     dbname = main_db_name_var.get().strip()
     if re.match(r'((^[\w(-.)?]+\.db$)|(^[\w?(-.)]\.db$))', dbname):
-        maindbname = dbname
-        main_db_name_blocker = 1
-        main_db_name_result_var.set('SET')
-        if db_path_blocker == 1:
-            fullpath = usable_real_path
-            conn_path_db = os.path.join(usable_real_path, maindbname)
-            if os.path.isfile(fullpath + f'\\{maindbname}') or os.path.isfile(fullpath + f'/{maindbname}')  :
-                db_already_exists_blocker = 1
-                main_db_conn = AD.Database(conn_path_db)
-                main_db_conn.addtable()
-                main_db_name_result_var.set('CONNECTED')
-                db_display_text.delete('1.0', tk.END)
-                db_display_text.insert(tk.END, f'Connected to {maindbname}..\n\n')
-                success_maindb_connection_blocker = 1
-                encfiletoolbutt.state(['!disabled'])
-                decfiletoolbutt.state(['!disabled'])
+        try:
+            maindbname = dbname
+            main_db_name_blocker = 1
+            main_db_name_result_var.set('SET')
+            if db_path_blocker == 1:
+                fullpath = usable_real_path
+                conn_path_db = os.path.join(usable_real_path, maindbname)
+                if os.path.isfile(fullpath + f'\\{maindbname}') or os.path.isfile(fullpath + f'/{maindbname}')  :
+                    db_already_exists_blocker = 1
+                    main_db_conn = AD.Database(conn_path_db)
+                    main_db_conn.addtable()
+                    main_db_name_result_var.set('CONNECTED')
+                    db_display_text.delete('1.0', tk.END)
+                    db_display_text.insert(tk.END, f'Connected to {maindbname}..\n\n')
+                    success_maindb_connection_blocker = 1
+                    encfiletoolbutt.state(['!disabled'])
+                    decfiletoolbutt.state(['!disabled'])
+                else:
+                    db_already_exists_blocker = 0
+                    main_db_conn = AD.Database(conn_path_db)
+                    main_db_conn.addtable()
+                    db_display_text.delete('1.0', tk.END)
+                    db_display_text.insert(tk.END, f"Created and Connected to '{maindbname}'.. in the directory '{fullpath}'\n\n")
+                    success_maindb_connection_blocker = 1
+                    encfiletoolbutt.state(['!disabled'])
+                    decfiletoolbutt.state(['!disabled'])
+
             else:
-                db_already_exists_blocker = 0
-                main_db_conn = AD.Database(conn_path_db)
-                main_db_conn.addtable()
                 db_display_text.delete('1.0', tk.END)
-                db_display_text.insert(tk.END, f"Created and Connected to '{maindbname}'.. in the directory '{fullpath}'\n\n")
-                success_maindb_connection_blocker = 1
-                encfiletoolbutt.state(['!disabled'])
-                decfiletoolbutt.state(['!disabled'])
-
-        else:
+                db_display_text.insert(tk.END, f"PATH : '{db_path_var.get().strip()}' is not a valid path\n\n")
+        except:
             db_display_text.delete('1.0', tk.END)
-            db_display_text.insert(tk.END, f"PATH : '{db_path_var.get().strip()}' is not a valid path\n\n")
+            db_display_text.insert(tk.END, f"The database might be distorted")
     else:
         main_db_name_result_var.set('NOT SET')
         main_db_name_blocker = 0
 
 
 def keyDBsetup():
     global usable_real_path,\
         success_keysdb_connection_blocker,\
         keys_db_conn
     print(usable_real_path)
     if db_path_blocker == 1 and main_db_name_blocker == 1:
-        dbname = main_db_name_var.get().strip()
-        keysDB = dbname[:-3] + 'Keys.db'
-        dbnameKeysWindows = '\\' + keysDB
-        dbnameKeysUnix = '/' + keysDB
-        conn_path_keys = os.path.join(usable_real_path, keysDB)
-        if db_already_exists_blocker == 1 :
-            if os.path.isfile(usable_real_path + dbnameKeysWindows) or os.path.isfile(usable_real_path + dbnameKeysUnix):
-                keys_db_conn = AD.Database(conn_path_keys)
-                keys_db_conn.addtable()
-                db_display_text.insert(tk.END, f"Connected to '{keysDB}' ..\n\n")
-                success_keysdb_connection_blocker = 1
+        try:
+            dbname = main_db_name_var.get().strip()
+            keysDB = dbname[:-3] + 'Keys.db'
+            dbnameKeysWindows = '\\' + keysDB
+            dbnameKeysUnix = '/' + keysDB
+            conn_path_keys = os.path.join(usable_real_path, keysDB)
+            if db_already_exists_blocker == 1 :
+                if os.path.isfile(usable_real_path + dbnameKeysWindows) or os.path.isfile(usable_real_path + dbnameKeysUnix):
+                    keys_db_conn = AD.Database(conn_path_keys)
+                    keys_db_conn.addtable()
+                    db_display_text.insert(tk.END, f"Connected to '{keysDB}' ..\n\n")
+                    success_keysdb_connection_blocker = 1
+                else:
+                    keys_db_conn = AD.Database(conn_path_keys)
+                    keys_db_conn.addtable()
+                    db_display_text.insert(tk.END, f"'{keysDB}' NOT FOUND ! ==> Created and Connected to '{keysDB}' ..\n\n")
+                    success_keysdb_connection_blocker = 1
             else:
                 keys_db_conn = AD.Database(conn_path_keys)
                 keys_db_conn.addtable()
-                db_display_text.insert(tk.END, f"'{keysDB}' NOT FOUND ! ==> Created and Connected to '{keysDB}' ..\n\n")
+                db_display_text.insert(tk.END, f"Created and Connected to '{keysDB}' ..\n\n")
                 success_keysdb_connection_blocker = 1
-        else:
-            keys_db_conn = AD.Database(conn_path_keys)
-            keys_db_conn.addtable()
-            db_display_text.insert(tk.END, f"Created and Connected to '{keysDB}' ..\n\n")
-            success_keysdb_connection_blocker = 1
+        except:
+            db_display_text.delete('1.0', tk.END)
+            db_display_text.insert(tk.END, f"The database might be distorted\n")
 
 
 success_maindb_connection_blocker = 0
 success_keysdb_connection_blocker = 0
 db_enable_blocker = 0
 def path_name_wrapper():
     set_db_path()
@@ -846,14 +508,380 @@
 
 swich_db_toggle.place(relx=0.47,rely=0.413)
 
 
 '''----------------------------------------LOWER FRAME ENDED----------------------------------'''
 
 
+
+
+
+
+'''-------------------------------TEXT DECRYPTION/ENCRYPTION STARTED---------------------------------------------------'''
+
+
+
+
+def encryption():
+    m = inputfield1_1.get()
+    if AF.CryptFile.keyverify(mainkeyvar.get()) == 1 and keySelectionFlag.get() == 1:
+        if len(m) > 200 :
+            outputvar1.set('Too Long')
+        else :
+            if inputfield1_1.get():
+                progressbar.start()
+                a = AT.Crypt(m, mainkeyvar.get())
+                b =  a.encrypt()[1]
+                outputvar1.set(b.__str__())
+                if var1.get() == 1:
+                    qr.tqr(b)
+
+
+def decryption():
+    n =inputfield2_1.get()
+    if AF.CryptFile.keyverify(mainkeyvar.get()) == 1 and keySelectionFlag.get() == 1:
+        if inputfield2_1.get():
+            progressbar2.start()
+            a = AT.Crypt(n, mainkeyvar.get())
+            b = a.decrypt()[1]
+            outputvar2.set(b.__str__())
+            if var2.get() == 1:
+                if not len(b) > 200:
+                    qr.tqr(b)
+
+def func1():
+    if var1.get() == 1 :
+        label1.config(text='QR ON')
+    else:
+        label1.config(text='QR OFF')
+
+def func2():
+    if var2.get() == 1 :
+        label2.config(text='QR ON')
+    else:
+        label2.config(text='QR OFF')
+
+
+button1 = tk.Button(master=textFrame1 ,text='ENCRYPT', command=encryption, bootstyle='light outline').place(relx=0.42, rely=0.73)
+button2 = tk.Button(master=textFrame2 , text='DECRYPT', command=decryption,bootstyle='light outline').place(relx=0.42,rely=0.8)
+
+inputfield1_1 = tk.StringVar()
+textfield1_1 = tk.Entry(master=textFrame1 ,
+                        width=20,
+                        font='Calibre 11 bold',
+                        textvariable=inputfield1_1).place(relx=0.29 , rely=0.30)
+
+inputfield2_1 = tk.StringVar(value='')
+textfield2_1 = tk.Entry(master=textFrame2 ,
+                        font='Calibre 11 bold',
+                        width=20,
+                        textvariable=inputfield2_1).place(relx=0.290 ,rely=0.38)
+
+namelabel1 = tk.Label(master=textFrame1 ,
+                      text='TEXT ENCRYPTION',
+                      font='Calibre 20 bold' ,
+                      )
+namelabel1.place(relx=0.190 ,rely=0.10)
+namelabel2 = tk.Label(master=textFrame2 ,
+                      text='TEXT DECRYPTION' ,
+                      font='Calibre 20 bold'  ,
+                      ).place(relx=0.190 ,rely=0.200)
+
+outputvar1 = tk.StringVar(value='')
+outputlabel1 =  tk.Entry(master= textFrame1,
+                         textvariable=outputvar1,
+                         font='terminal 11 bold').place(relx= 0.02,
+                                                       rely= 0.48 ,
+                                                       width= 480,
+                                                       height= 50)
+outputvar2 = tk.StringVar(value='')
+outputlabel2 = tk.Entry(master=textFrame2 ,
+                        textvariable= outputvar2 ,
+                        font='terminal 11 bold').place(relx= 0.02,
+                                                       rely= 0.55,
+                                                       width= 480,
+                                                       height= 50)
+
+
+
+label1 = tk.Label(master=textFrame1,text='QR',font=('terminal',17))
+label1.place(relx=0.2,rely=0.75)
+var1 = tk.IntVar()
+mytoolbutt3 = tk.Checkbutton(bootstyle='success , round-toggle',
+                        master=textFrame1,
+                        variable=var1,
+                        offvalue=0,
+                        command=func1)
+
+mytoolbutt3.place(relx=0.1,rely=0.77)
+
+
+
+
+label2 = tk.Label(master=textFrame2,text='QR',font=('terminal',17))
+label2.place(relx=0.2,rely=0.82)
+var2 = tk.IntVar()
+mytoolbutt6 = tk.Checkbutton(bootstyle='success , round-toggle',
+                        master=textFrame2,
+                        variable=var2,
+                        offvalue=0,
+                        command=func2)
+
+mytoolbutt6.place(relx=0.1,rely=0.84)
+
+
+progressbar = tk.Progressbar(master=textFrame1,mode='indeterminate',style='secondary',length=100,)
+progressbar.place(relx=0.05,rely=0.34)
+
+progressbar2 = tk.Progressbar(master=textFrame2,mode='indeterminate',style='secondary',length=100,)
+progressbar2.place(relx=0.05,rely=0.42)
+
+'''-------------------------------TEXT DECRYPTION/ENCRYPTION ENDED---------------------------------------------------'''
+
+
+
+
+
+
+
+
+
+'''-------------------------------FILE ENCRYPTION/DECRYPTION STARTED--------------------------------------------'''
+
+
+filepathlabel = tk.Label(master=frameFile1 ,
+                      text='FILE PATH',
+                      font='Calibre 20 bold' ,
+                      )
+filepathlabel.place(relx=0.335,rely=0.10)
+
+
+resultvarfile = tk.StringVar(value='                  ..RESULT..')
+resultLabelfile =  tk.Label(master= frameFile1,
+                         textvariable=resultvarfile,
+                         font='terminal 13 bold').place(
+                                                       rely= 0.55 ,
+                                                       )
+
+
+def encFile():
+    global fileaccessSemo ,add_enc_to_db ,main_db_conn,mainkey
+    if 1 :
+        if keySelectionFlag.get() != 0:
+            filename = filenameStringVar.get().strip()
+            key = mainkey
+            target = AF.CryptFile(filename, key)
+            a = target.encrypt()
+            if a == 1:
+                filename = filename + '.crypt'
+                filenameStringVar.set(filename)
+                resultvarfile.set('    Encrypted Successfully / added .crypt')
+                if encfiletoolbuttvar.get() == 1:
+                    with open(filename,'rb') as f:
+                        file_content = f.read()
+                    try:
+                        main_db_conn.insert(filename,file_content, outputKeyref.get().strip())
+                    except:
+                        db_display_text.delete('1.0', tk.END)
+                        db_display_text.insert(tk.END, f"ERROR \n\nDatabase might be distorted\n")
+            if a == 2:
+                resultvarfile.set('                 File is Empty')
+            if a == 3:
+                resultvarfile.set("               File Doesn't Exist")
+            if a == 0:
+                resultvarfile.set("                  Can't Encrypt")
+            if  a == 4:
+                resultvarfile.set('                     ERROR')
+            if a == 5 :
+                resultvarfile.set('          ERROR : Key is Not 512-bit')
+            if a == 6:
+                resultvarfile.set('       ERROR : File is already encrypted')
+            elif a == 7:
+                resultvarfile.set(' ERROR : Given a directory instead of a file')
+
+def decfile():
+    global fileaccessSemo,add_dec_to_db,main_db_conn,mainkey
+    if 1:
+        if keySelectionFlag.get() != 0:
+            filename =filenameStringVar.get().strip()
+            key = mainkey
+            target = AF.CryptFile(filename, key)
+            a = target.decrypt()
+            if a == 1:
+                filename = os.path.splitext(filename)[0]
+                filenameStringVar.set(filename)
+                resultvarfile.set('   Decrypted Successfully + removed .crypt')
+                if decfiletoolbuttvar.get() == 1:
+                    with open(filename,'rb') as f:
+                        file_content = f.read()
+                    try:
+                        main_db_conn.insert(filename,file_content, outputKeyref.get().strip())
+                    except:
+                        db_display_text.delete('1.0', tk.END)
+                        db_display_text.insert(tk.END, f"ERROR \n\nDatabase might be distorted\n")
+            if a == 2:
+                resultvarfile.set('                 File is Empty')
+            if a == 3:
+                resultvarfile.set("               File Doesn't Exist")
+            if a == 0:
+                resultvarfile.set("                 Can't Decrypt")
+            if  a == 4:
+                resultvarfile.set('                     ERROR')
+            elif a == 5 :
+                resultvarfile.set('          ERROR : Key is Not 512-bit')
+            if a == 6:
+                resultvarfile.set('       ERROR : File is already decrypted')
+            elif a == 7:
+                resultvarfile.set(' ERROR : Given a directory instead of a file')
+
+
+
+
+
+
+encryptionfilebutton = tk.Button(master=frameFile1 ,text='ENCRYPT FILE', command=encFile, bootstyle='warning outline').place(relx=0.25, rely=0.73)
+decryptionfilebutton = tk.Button(master=frameFile1 , text='DECRYPT FILE', command=decfile,bootstyle='warning outline').place(relx=0.55,rely=0.73)
+
+filenameStringVar = tk.StringVar(value='')
+
+filenametext = tk.Entry(master=frameFile1 ,
+                        width=31,
+                        font='Calibre 15 bold',
+                        textvariable=filenameStringVar).place(relx=0.05, rely=0.30)
+
+
+
+addtodbLabel = tk.Label(master=frameFile1,text='ADD TO DATABASE',font=('Calibre',11),bootstyle='warning')
+addtodbLabel.place(relx=0.35,rely=0.908)
+
+add_enc_to_db = 0
+def encToggleButtFunc():
+    global add_enc_to_db
+    if encfiletoolbuttvar == 1:
+        add_enc_to_db = 1
+    else:
+        add_enc_to_db = 0
+
+add_dec_to_db = 0
+def decToggleButtFunc():
+    global add_dec_to_db
+    if decfiletoolbuttvar == 1:
+        add_dec_to_db = 1
+    else:
+        add_dec_to_db = 0
+
+encfiletoolbuttvar = tk.IntVar()
+encfiletoolbutt = tk.Checkbutton(bootstyle='warning , round-toggle',
+                        master=frameFile1,
+                        variable=encfiletoolbuttvar,
+                        offvalue=0,
+                        onvalue=1,
+                        command=encToggleButtFunc)
+encfiletoolbutt.state(['disabled'])
+encfiletoolbutt.place(relx=0.25,rely=0.92)
+
+
+decfiletoolbuttvar = tk.IntVar()
+decfiletoolbutt = tk.Checkbutton(bootstyle='warning , round-toggle',
+                        master=frameFile1,
+                        variable=decfiletoolbuttvar,
+                        offvalue=0,
+                        command=decToggleButtFunc)
+decfiletoolbutt.state(['disabled'])
+decfiletoolbutt.place(relx=0.717,rely=0.92)
+
+
+
+
+keySelectionFlag = tk.IntVar(value=0)
+def mainKeyWrapper():
+    global success_keysdb_connection_blocker,mainkey
+    if AF.CryptFile.keyverify(mainkeyvar.get().strip()) == 1 :
+        mainkey = mainkeyvar.get().strip()
+        keyrefGen()
+        keyselectionvar.set('       SELECTED')
+        keySelectionFlag.set(1)
+        try:
+            if success_keysdb_connection_blocker and os.path.isfile(filenameStringVar.get().strip()):
+                keys_db_conn.insert(filenameStringVar.get().strip(),mainkey,outputKeyref.get())
+            if success_keysdb_connection_blocker and not os.path.isfile(filenameStringVar.get().strip()):
+                keys_db_conn.insert('STANDALONE',mainkey,outputKeyref.get())
+        except:
+            db_display_text.delete('1.0', tk.END)
+            db_display_text.insert(tk.END, f"Faulty Database\n")
+    else :
+        keySelectionFlag.set(0)
+        keyselectionvar.set('     NOT SELECTED')
+
+
+mainkeyLabel = tk.Label(master=frameFile2 ,
+                      text='MAIN KEY' ,
+                      font='Calibre 20 bold',
+                      bootstyle='info',
+                      ).place(relx=0.3 ,rely=0.075)
+
+
+mainkeyvar = tk.StringVar()
+mainkeyEntry = tk.Entry(master=frameFile2 ,
+                        font='Calibre 14 bold',
+                        textvariable=mainkeyvar,
+                        width=29
+                        ).place(relx=0.09 ,rely=0.29)
+
+
+def keyrefGen():
+    ref = '#'
+    for _ in range(6):
+        character = secrets.choice(string.ascii_letters + string.digits + '$' + '?' + '&' + '@' + '!' + '-' + '+')
+        ref += character
+    outputKeyref.set(ref)
+
+
+
+outputKeyref = tk.StringVar(value='#XXXXXX')
+keyrefLabel = tk.Label(master=frameFile2,textvariable=outputKeyref,bootstyle='secondary',font=('terminal',12))
+keyrefLabel.place(relx=0.712,rely=0.12)
+
+keySelectButton = tk.Button(master=frameFile2 ,text='SELECT KEY', command=mainKeyWrapper, bootstyle='info outline').place(relx=0.6725, rely=0.5)
+
+
+keyselectionvar = tk.StringVar(value='   KEY NOT SELECTED')
+keyselectionLabel = tk.Label(master=frameFile2 ,
+                        textvariable= keyselectionvar ,
+                        bootstyle='info',
+                        font='terminal 11 bold').place(relx= 0.15 ,
+                                        rely= 0.465,
+                                        height= 50)
+
+
+
+def genMainKey():
+    keyGenVar.set(AF.CryptFile.genkey())
+
+
+keyGenVar = tk.StringVar(value='')
+keyGenEntry = tk.Entry(master=frameFile2 ,
+                        font='terminal 15 bold',
+                        textvariable=keyGenVar,
+                        width=14,
+                        show='').place(relx=0.1 ,rely=0.69)
+
+keyButton = tk.Button(master=frameFile2 ,
+                      text='GENERATE',
+                      command=genMainKey,
+                      bootstyle='success outline').place(relx=0.671, rely=0.7)
+
+
+'''-------------------------------FILE ENCRYPTION/DECRYPTION ENDED--------------------------------------------'''
+
+
+
+
+
+
 '''---------------------------------------STAMP STARTED -------------------------------------------------------'''
 
 
 latest_ID_key_label = tk.Label(master=lowerFrame,text='GitHub.com/AshGw/AES-256', font='Calibre 6')
 latest_ID_key_label.place(relx=0.84,rely=0.92)
 
 '''---------------------------------------STAMP ENDED-------------------------------------------------------'''
@@ -863,17 +891,24 @@
 
 
 def rm_json():
     global usable_real_path
     file = os.path.join(usable_real_path,'output.json')
     if os.path.exists(file):
         os.remove(file)
-    else:
-        pass
-atexit.register(rm_json)
+
+def rm_qr():
+    if os.path.exists('qrv10.png'):
+        os.remove('qrv10.png')
+
+def rm_all():
+    rm_qr()
+    rm_json()
+
+atexit.register(rm_all)
 
 
 
 if __name__ == '__main__':
     object.mainloop()
```

### Comparing `AshCrypt-1.2.0/AshCrypt/AshDatabase.py` & `AshCrypt-1.2.1/AshCrypt/AshDatabase.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.2.0/AshCrypt/AshFileCrypt.py` & `AshCrypt-1.2.1/AshCrypt/AshFileCrypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.2.0/AshCrypt/AshTextCrypt.py` & `AshCrypt-1.2.1/AshCrypt/AshTextCrypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.2.0/AshCrypt/CliCrypt.py` & `AshCrypt-1.2.1/AshCrypt/CliCrypt.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from AshCrypt import AshFileCrypt as AF
 from AshCrypt import AshTextCrypt as A
+import os.path
 import sys
 
 
 print('Welcome to the CLI')
 
 commands = 'Commands : \n\tq: to quit the program \n\tc : view commands\n\te: for encryption\n\td : for decryption\n' \
            '\tef : to encrypt a file\n\tdf : to decrypt a file\n'
@@ -147,15 +148,16 @@
         inputWrap(pre)
         if pre == '' :
             print("You can use the commands AFTER entering the file name.. ")
             filename = input('Enter full file name to be Decrypted : ')
             target = AF.CryptFile(filename, key)
             a = target.decrypt()
             if a == 1:
-                print('File successfully decrypted ')
+                print('File successfully decrypted + removed .crypt extension')
+                print(f'File is now named {os.path.splitext(filename)[0]}')
             if a == 2:
                 print('Cannot decrypt the file  when it is already empty')
             if a == 3:
                 print(f'The file named : "{filename}" does not exists , try specifying the whole sys path')
             if a == 0:
                 print('Error in the decryption process. Check if the the file is distorted or it might just be '
                       'decrypted already')
@@ -179,15 +181,16 @@
         inputWrap(pre)
         if pre == '' :
             print("You can use the commands AFTER entering the file name.. ")
             filename = input('Enter full file name to be Encrypted : ')
             target = AF.CryptFile(filename, key)
             a = target.encrypt()
             if a == 1:
-                print('File successfully encrypted ')
+                print('File successfully encrypted + added .crypt extension')
+                print(f"File is now named : '{filename}.crypt' ")
             if a == 2:
                 print('Cannot encrypt the file  when it is already empty')
             if a == 3:
                 print(f'The file named : "{filename}" does not exists , try specifying the whole sys path')
             if a == 0:
                 print('Error in the encryption process. Check if the the file is distorted')
             elif a == 4 :
```

### Comparing `AshCrypt-1.2.0/AshCrypt/README.md` & `AshCrypt-1.2.1/AshCrypt/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Cryptography Library : AES-256
+# Cryptography App &  Library : AES-256
 ##  Objective ## 
 #### Enhanced Security, Simplicity & Ease of use For Everyone And Anyone Willing To Use AES 256 With No Unnecessary Complications.
 ## Overview ## 
 **Visit The [GitHub](https://github.com/AshGw/AES-256/tree/main) Repository**
 <br>The library incorporates a base cryptography mdoule called **Ash** 
 
 <br>A simple, secure, and developer-oriented module for
@@ -10,38 +10,40 @@
 interface, seamless integration with precompiled 
 functions, and robust security measures to safeguard
 sensitive data,  providing a hassle-free experience when dealing with cryptographic libraries.
 <br>View **Features** Header for more details.
 
 
 
-The library uses that same module to ensure secure data encryption and decryption for Files and Texts while keeping it very easy and simple to use .
-view the headers for **AshFileCrypt**  and **AshTextCrypt** learn more.
 
-It also includes a simple graphical user interface (GUI) for easy interaction with the **AshTextCrypt** module.
-<br>If you're trying to either encrypt or decrypt some messages on the go ( 200 characters max ) you can use this GUI.
-<br>It also has a qr module associated with it to display the message.
-<br>check **GUI**  for more info.
+The project mainly includes a fully fledged application that integrates all the modules in the library merging them into a unified and powerful software solution for developers and for people with no programming knowledge whatsoever
+<br>check `GUI` header for more info.
+
+
+### For Developers ###
+The project uses `Ash` module to ensure secure data encryption and decryption for Files and Texts while keeping it very easy and simple to use .
+view the headers for `AshFileCrypt` and `AshTextCrypt` to learn more.
 
-While The **GUI** is limited to 200 characters of text, if you want to be free over how much data or type of data you want to include, then u can use `CliCrypt.py` which is an innovative command line interface (CLI) designed to provide encryption and decryption capabilities for both text and file data with no constraints
 
 It also incorporates a database module that serve the same purpose which is allowing for the management and storage of classified content in a secure, 
 safe and simple manner, you can use whichever you see fit.
 
+<br>The module has a simple straight forward approach for dealing with sqlite3 databases, even if youre not familiar with Python itself you can still use this module to run SQL queries and built in functions to perform various operations on a given database.<br>
+Check `AshDatabase` header to learn more.
+
 **After the library is installed**
 <br>to run the GUI 
 ```shell
 python -m AshCrypt.AshCryptGUI
 ```
 To run the CLI
 ```shell
 python -m AshCrypt.CliCrypt
 ```
 
-<br>The module has a simple straight forward apporach for dealing with sqlite3 databases, even if youre not familiar with Python itself you can still use this module to run SQL queries and built in functions to perform various operations on a given database.<br>Check **AshDatabase** header to learn more.
 
 ## Ash Module ##
 The `Ash.py` module is a comprehensive collection of carefully designed functions and code modules that facilitate optimal performance and reliability in data encryption and decryption operations  while ensuring the utmost security and 
 confidentiality.
 
 <br>It uses primitives from the `cryptography` library with added security features while keeping it simple and highly flexible to provide a head-ache free solution for developers. 
 
@@ -114,14 +116,57 @@
 ### Regarding KDFs
 Note that bcrypt is intentionally slow and computationally expensive, enhancing protection against brute-force attacks. The number of iterations, including salt and pepper, increases derivation time to strike a balance between security and performance. Use a suitable value based on your machine's capabilities and desired security level.
 
 <br>Im using 50 just to demonstrate the process and make it quick.
 <br>The bare minimum is 50, the max is 100 000, choose somewhere in between.
 <br>In my use case 50 takes around 0.5 secs while using the maximun number of iterations takes around 11 minutes to derive the keys and finish the cryptographic operations at hand.
 
+
+
+## AshCryptGUI ##
+The GUI as mentioned above is a fully fledged application , you can use it to encrypt files , texts , keep track of files by storing them on demand to a main database , also on demand it can keep track of the keys used for cryptographic operations.
+### Usage ###
+1) Set the main key up. If you don't have one , press on the button `generate` to generate a secure safe key ready for use. 
+2) Now you're able to encrypt files or text (text is limited to 200 characters max)
+####  Text : 
+- You can insert some text in the entry right below the `TEXT ENCRYPTION` label.<br>The given text will be encrypted and you can choose if you want to have that text displayed as a qr code, a qr image will pop on the screen and you'll be able to scan it using your phone.
+- Insert some encrypted text below the `TEXT DECRYPTION` label.<br>The Given text will be decrypted and you'd have the option to display the "plaintext" as a qr code to be scanned by other devices.
+#### Files
+- Under the `FILE PATH` label enter the file name (if it's in the current working directory) or submit the whole file path , the file can be of any type, click on `ENCRYPT FILE` Button to encrypt the given file , if the encryption turned out to be successful , you'll see a success message along with a `added .crypt extention to the file` message if the encryption wasn't successful you'll see an error message specifying the problem.<br>Note that you cannot re-encrypt a file that  has `.crypt` as extention.
+- The file name should be changed by now to `filename + '.crypt'` , if the file has .crypt extention you can go ahead and decrypt it , if the same key is used for both enc/dec operations then the result should be `success` + `removed .crypt extention` from the file.
+#### Database
+- Now you have some encrypted/decrypted files but you want to keep them stored somewhere safe, this is where the main database comes in , where you need to store your files + their content + reference to the key used for their encryption/decryption. you can specify your database by 
+1) Specify the actual path where you want your database to be 
+2) Give it a name, it must be a valid file name that ends with `.db` .<br>
+If the database doesn't exist then a database with the name you've given will be created and automatically connected to.<br>If the given database already exists then it will automatically be connected.
+3) Did I mention the keys database ? well if you give a database it will also create a keys database with the same name as the database you chose plus `Keys` added to its name. This database holds the actual keys and the reference to these keys.
+<br>The only common piece of data that the two separate databases have in common are the key reference values.  
+
+**Note** : If your main database gets compromised , then the attacker wouldnt have anything useful , they can never know the actual key from the reference key so no problem with that if it only contains encrypted content BUT NEVER EVER GET YOUR KEYS DATABASE COMPROMISED ! 
+<br>If anyone gets hold of your main database they would only see some encrypted content and some key refrence that is actually 100% independent of the actual key used for encryption so they have nothing , but if they get hold of the keys database they can look for matching refs and use the matching key to decrypt that binary encrypted data to its actual format.
+That's why I made two different databases not two tables within a single database. 
+<br> So you keep your keys database safe and secure.
+
+
+**Info** Both databases have the same table called `Classified` that has 4 columns <br>`ID` which is auto generated & incremented for each piece of data that gets inserted<br>
+`Name` that holds the filename in both databases , although in the keys database if you haven't specified any file to operate on and keep selecting keys the keys name will be `STANDALONE` 
+<br>`Contnet` in the main db that holds the entire content of the given file, in keys db that holds the actual 512 bit long encryption key.
+<br>`Key` in  both db's that holds the `KeyRef` or key reference value
+#### Usage 
+The buttons are self-explanatory so do what you see fit. the result of any task related to the databases is displayed in `DATABASE OUTPUT CONSOLE` although you can run a query anytime by writing a query and using `query` button , the result will be displayed to an `output.json` file that auto-deletes when you exit the app.
+<br>Just click buttons and check the result in the output console, it will guide you the process.
+
+<br>To run the GUI anywhere
+```shell
+python -m AshCrypt.AshCryptGUI
+```
+
+
+
+
 ## AshFileCrypt ## 
 If you want to encrypt a file :
 1) Follow the steps above to set the key up.
 2) Create an instance of the class CryptFiles and pass 2 arguments, the first one being the target file and the second argument being the key :
 ```python
 instance1 = CryptFile('target.txt', key)
 ```
@@ -141,16 +186,23 @@
 target = CryptFile('/User/Desktop/MyProjects/SomeOtherfolder/myfile.txt',key)
 ```
 3) Apply either the encryption or decryption functions to that instance :
 ```python
 instance1 = CryptFile('qrv10.png',key)
 instance1.encrypt()
 ```
-you can apply `print()` on `instance1.encrypt()`to check the result, if it is `1` then everything went ok , if it's `3` then the file doesn't even exists otherwise some other Error has occurred (usually the file is distorted).
-
+you can apply `print()` on `instance1.encrypt()`to check the result :
+<br> 1 : File successfully encrypted/decrypted + added/removed .crypt extension 
+<br> 2 : File is empty
+<br> 3 : File doesn't exist
+<br> 4 : Unknown Error usually a system related one 
+<br> 5 : Key is denied for cryptographic use
+<br> 6 : File is already encrypted/decrypted
+<br> 7 : File is not a file it's a directory
+<br> 0 : Error in enc/dec probable file distortion or tampering or wrong key
 ```python
 instance1.encrypt()
 ```
 ```python
 instance1.decrypt()
 ```
 **Note** : 
@@ -178,20 +230,14 @@
 in `AshFileCryt` & `AshTextCrypt` it's simpler if you attempt to decrypt an non-encrypted message then you'll get the same message back along with an integer in this case `0` for failure.
 <br>`1`'s for success.
 <br>Non `1`'s for failure (`2`/`0.0`/`0`) each indicate different Errors. 
 
 Error handling here has no Exceptions raised just `1`'s, `0`'s & `2`'s for feedback, just to make it simple and Non-Technical.
 
 
-## AshCryptGUI ##
-This is a fully fledged application that integrates all the modules in the library merging them into a unified and powerful software solution. run this command and see for yourself !
-
-```shell
-python -m AshCrypt.AshCryptGUI
-```
 ### QR ## 
 The `qr.py` module is used to display a qr code of the encrypted/decrypted messages to be quickly scanned and transmitted , you can use qr versions from `1` to `40` , although I recommend using `40` since it can take the maximum number of characters for small files , and `10` if you're working with the GUI which is intended for text/short messages,
 
 ## AshDatabase ##
 To support efficient content management, I have integrated this database module to enable the storage and retrieval of encrypted content in a safe and secure manner using an sqlite3 database
 
 Ensuring that the encrypted data remains organized and readily accessible to anyone with the right key. Any content going in must be encrypted with a key that you must keep off grid.
@@ -243,28 +289,28 @@
 
 6) Check the module itself so you can run through all the available methods.
 <br>The methods available perform the usual operations like insertion, deletion , updating the database and more..
 
 
 7) to run more complex queries I've dedicated a query function that takes in *queries and returns the result fetched 
 ```python
-query1 = 'SELECT COUNT(*) AS cc ,content FROM Classified WHERE key = "#5482A" ORDER BY cc DESC '
-print(connect.query(query1))
+query = 'SELECT COUNT(*) AS cc ,content FROM Classified WHERE key = "#5482A" ORDER BY cc DESC '
+print(connect.query(query))
 ```
 The result fetched should look like this : 
  ```python
-[{'query1': [(3, 'some encrypted content of bytes or strings')]}]
+[{'query 0': ['SUCCESS', [(1, 'some encrypted content of bytes or strings')]]}]
 ```
-If some error has occured while doing a query like : 
+If some error has occurred while doing a query like : 
 ```python
-query1 = 'SELECT COUNT(*) AS cc ,content FROM DoesntExist WHERE key = "#5482A" ORDER BY cc DESC '
+query = 'SELECT COUNT(*) AS cc ,content FROM DoesntExist WHERE key = "#5482A" ORDER BY cc DESC '
 ```
-The result fetched should look similair to this : 
+The result fetched should look similar to this : 
 ```python
-[{'query1': (0, OperationalError('no such table: DoesntExist'))}]
+[{'query 0': ('FAILURE', 'no such table: DoesntExist')}]
 ```
 Thats it so simple !
 
 ## License ##
 This project is licensed under the [MIT LICENSE](https://github.com/AshGw/AES-256/blob/main/LICENSE).
 ## Acknowledgments ##
 This cryptographic scheme is inspired by secure cryptographic practices and various open-source implementations.
```

### Comparing `AshCrypt-1.2.0/AshCrypt/qr.py` & `AshCrypt-1.2.1/AshCrypt/qr.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.2.0/AshCrypt/unittests/unittestAsh.py` & `AshCrypt-1.2.1/AshCrypt/unittests/unittestAsh.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.2.0/AshCrypt.egg-info/PKG-INFO` & `AshCrypt-1.2.1/AshCrypt.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: AshCrypt
-Version: 1.2.0
-Summary: Comprehensive AES-256 Cryptography library equipped with a file handling module along with a text module w/ a user-friendly GUI and a database module to store encrypted content.
+Version: 1.2.1
+Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
-Keywords: Cryptography,AES-256
+Keywords: Cryptography application,cryptography libraryAES-256
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Cryptography Library : AES-256
+# Cryptography App &  Library : AES-256
 ##  Objective ## 
 #### Enhanced Security, Simplicity & Ease of use For Everyone And Anyone Willing To Use AES 256 With No Unnecessary Complications.
 ## Overview ## 
 **Visit The [GitHub](https://github.com/AshGw/AES-256/tree/main) Repository**
 <br>The library incorporates a base cryptography mdoule called **Ash** 
 
 <br>A simple, secure, and developer-oriented module for
@@ -33,38 +33,40 @@
 interface, seamless integration with precompiled 
 functions, and robust security measures to safeguard
 sensitive data,  providing a hassle-free experience when dealing with cryptographic libraries.
 <br>View **Features** Header for more details.
 
 
 
-The library uses that same module to ensure secure data encryption and decryption for Files and Texts while keeping it very easy and simple to use .
-view the headers for **AshFileCrypt**  and **AshTextCrypt** learn more.
 
-It also includes a simple graphical user interface (GUI) for easy interaction with the **AshTextCrypt** module.
-<br>If you're trying to either encrypt or decrypt some messages on the go ( 200 characters max ) you can use this GUI.
-<br>It also has a qr module associated with it to display the message.
-<br>check **GUI**  for more info.
+The project mainly includes a fully fledged application that integrates all the modules in the library merging them into a unified and powerful software solution for developers and for people with no programming knowledge whatsoever
+<br>check `GUI` header for more info.
+
+
+### For Developers ###
+The project uses `Ash` module to ensure secure data encryption and decryption for Files and Texts while keeping it very easy and simple to use .
+view the headers for `AshFileCrypt` and `AshTextCrypt` to learn more.
 
-While The **GUI** is limited to 200 characters of text, if you want to be free over how much data or type of data you want to include, then u can use `CliCrypt.py` which is an innovative command line interface (CLI) designed to provide encryption and decryption capabilities for both text and file data with no constraints
 
 It also incorporates a database module that serve the same purpose which is allowing for the management and storage of classified content in a secure, 
 safe and simple manner, you can use whichever you see fit.
 
+<br>The module has a simple straight forward approach for dealing with sqlite3 databases, even if youre not familiar with Python itself you can still use this module to run SQL queries and built in functions to perform various operations on a given database.<br>
+Check `AshDatabase` header to learn more.
+
 **After the library is installed**
 <br>to run the GUI 
 ```shell
 python -m AshCrypt.AshCryptGUI
 ```
 To run the CLI
 ```shell
 python -m AshCrypt.CliCrypt
 ```
 
-<br>The module has a simple straight forward apporach for dealing with sqlite3 databases, even if youre not familiar with Python itself you can still use this module to run SQL queries and built in functions to perform various operations on a given database.<br>Check **AshDatabase** header to learn more.
 
 ## Ash Module ##
 The `Ash.py` module is a comprehensive collection of carefully designed functions and code modules that facilitate optimal performance and reliability in data encryption and decryption operations  while ensuring the utmost security and 
 confidentiality.
 
 <br>It uses primitives from the `cryptography` library with added security features while keeping it simple and highly flexible to provide a head-ache free solution for developers. 
 
@@ -137,14 +139,57 @@
 ### Regarding KDFs
 Note that bcrypt is intentionally slow and computationally expensive, enhancing protection against brute-force attacks. The number of iterations, including salt and pepper, increases derivation time to strike a balance between security and performance. Use a suitable value based on your machine's capabilities and desired security level.
 
 <br>Im using 50 just to demonstrate the process and make it quick.
 <br>The bare minimum is 50, the max is 100 000, choose somewhere in between.
 <br>In my use case 50 takes around 0.5 secs while using the maximun number of iterations takes around 11 minutes to derive the keys and finish the cryptographic operations at hand.
 
+
+
+## AshCryptGUI ##
+The GUI as mentioned above is a fully fledged application , you can use it to encrypt files , texts , keep track of files by storing them on demand to a main database , also on demand it can keep track of the keys used for cryptographic operations.
+### Usage ###
+1) Set the main key up. If you don't have one , press on the button `generate` to generate a secure safe key ready for use. 
+2) Now you're able to encrypt files or text (text is limited to 200 characters max)
+####  Text : 
+- You can insert some text in the entry right below the `TEXT ENCRYPTION` label.<br>The given text will be encrypted and you can choose if you want to have that text displayed as a qr code, a qr image will pop on the screen and you'll be able to scan it using your phone.
+- Insert some encrypted text below the `TEXT DECRYPTION` label.<br>The Given text will be decrypted and you'd have the option to display the "plaintext" as a qr code to be scanned by other devices.
+#### Files
+- Under the `FILE PATH` label enter the file name (if it's in the current working directory) or submit the whole file path , the file can be of any type, click on `ENCRYPT FILE` Button to encrypt the given file , if the encryption turned out to be successful , you'll see a success message along with a `added .crypt extention to the file` message if the encryption wasn't successful you'll see an error message specifying the problem.<br>Note that you cannot re-encrypt a file that  has `.crypt` as extention.
+- The file name should be changed by now to `filename + '.crypt'` , if the file has .crypt extention you can go ahead and decrypt it , if the same key is used for both enc/dec operations then the result should be `success` + `removed .crypt extention` from the file.
+#### Database
+- Now you have some encrypted/decrypted files but you want to keep them stored somewhere safe, this is where the main database comes in , where you need to store your files + their content + reference to the key used for their encryption/decryption. you can specify your database by 
+1) Specify the actual path where you want your database to be 
+2) Give it a name, it must be a valid file name that ends with `.db` .<br>
+If the database doesn't exist then a database with the name you've given will be created and automatically connected to.<br>If the given database already exists then it will automatically be connected.
+3) Did I mention the keys database ? well if you give a database it will also create a keys database with the same name as the database you chose plus `Keys` added to its name. This database holds the actual keys and the reference to these keys.
+<br>The only common piece of data that the two separate databases have in common are the key reference values.  
+
+**Note** : If your main database gets compromised , then the attacker wouldnt have anything useful , they can never know the actual key from the reference key so no problem with that if it only contains encrypted content BUT NEVER EVER GET YOUR KEYS DATABASE COMPROMISED ! 
+<br>If anyone gets hold of your main database they would only see some encrypted content and some key refrence that is actually 100% independent of the actual key used for encryption so they have nothing , but if they get hold of the keys database they can look for matching refs and use the matching key to decrypt that binary encrypted data to its actual format.
+That's why I made two different databases not two tables within a single database. 
+<br> So you keep your keys database safe and secure.
+
+
+**Info** Both databases have the same table called `Classified` that has 4 columns <br>`ID` which is auto generated & incremented for each piece of data that gets inserted<br>
+`Name` that holds the filename in both databases , although in the keys database if you haven't specified any file to operate on and keep selecting keys the keys name will be `STANDALONE` 
+<br>`Contnet` in the main db that holds the entire content of the given file, in keys db that holds the actual 512 bit long encryption key.
+<br>`Key` in  both db's that holds the `KeyRef` or key reference value
+#### Usage 
+The buttons are self-explanatory so do what you see fit. the result of any task related to the databases is displayed in `DATABASE OUTPUT CONSOLE` although you can run a query anytime by writing a query and using `query` button , the result will be displayed to an `output.json` file that auto-deletes when you exit the app.
+<br>Just click buttons and check the result in the output console, it will guide you the process.
+
+<br>To run the GUI anywhere
+```shell
+python -m AshCrypt.AshCryptGUI
+```
+
+
+
+
 ## AshFileCrypt ## 
 If you want to encrypt a file :
 1) Follow the steps above to set the key up.
 2) Create an instance of the class CryptFiles and pass 2 arguments, the first one being the target file and the second argument being the key :
 ```python
 instance1 = CryptFile('target.txt', key)
 ```
@@ -164,16 +209,23 @@
 target = CryptFile('/User/Desktop/MyProjects/SomeOtherfolder/myfile.txt',key)
 ```
 3) Apply either the encryption or decryption functions to that instance :
 ```python
 instance1 = CryptFile('qrv10.png',key)
 instance1.encrypt()
 ```
-you can apply `print()` on `instance1.encrypt()`to check the result, if it is `1` then everything went ok , if it's `3` then the file doesn't even exists otherwise some other Error has occurred (usually the file is distorted).
-
+you can apply `print()` on `instance1.encrypt()`to check the result :
+<br> 1 : File successfully encrypted/decrypted + added/removed .crypt extension 
+<br> 2 : File is empty
+<br> 3 : File doesn't exist
+<br> 4 : Unknown Error usually a system related one 
+<br> 5 : Key is denied for cryptographic use
+<br> 6 : File is already encrypted/decrypted
+<br> 7 : File is not a file it's a directory
+<br> 0 : Error in enc/dec probable file distortion or tampering or wrong key
 ```python
 instance1.encrypt()
 ```
 ```python
 instance1.decrypt()
 ```
 **Note** : 
@@ -201,20 +253,14 @@
 in `AshFileCryt` & `AshTextCrypt` it's simpler if you attempt to decrypt an non-encrypted message then you'll get the same message back along with an integer in this case `0` for failure.
 <br>`1`'s for success.
 <br>Non `1`'s for failure (`2`/`0.0`/`0`) each indicate different Errors. 
 
 Error handling here has no Exceptions raised just `1`'s, `0`'s & `2`'s for feedback, just to make it simple and Non-Technical.
 
 
-## AshCryptGUI ##
-This is a fully fledged application that integrates all the modules in the library merging them into a unified and powerful software solution. run this command and see for yourself !
-
-```shell
-python -m AshCrypt.AshCryptGUI
-```
 ### QR ## 
 The `qr.py` module is used to display a qr code of the encrypted/decrypted messages to be quickly scanned and transmitted , you can use qr versions from `1` to `40` , although I recommend using `40` since it can take the maximum number of characters for small files , and `10` if you're working with the GUI which is intended for text/short messages,
 
 ## AshDatabase ##
 To support efficient content management, I have integrated this database module to enable the storage and retrieval of encrypted content in a safe and secure manner using an sqlite3 database
 
 Ensuring that the encrypted data remains organized and readily accessible to anyone with the right key. Any content going in must be encrypted with a key that you must keep off grid.
@@ -266,28 +312,28 @@
 
 6) Check the module itself so you can run through all the available methods.
 <br>The methods available perform the usual operations like insertion, deletion , updating the database and more..
 
 
 7) to run more complex queries I've dedicated a query function that takes in *queries and returns the result fetched 
 ```python
-query1 = 'SELECT COUNT(*) AS cc ,content FROM Classified WHERE key = "#5482A" ORDER BY cc DESC '
-print(connect.query(query1))
+query = 'SELECT COUNT(*) AS cc ,content FROM Classified WHERE key = "#5482A" ORDER BY cc DESC '
+print(connect.query(query))
 ```
 The result fetched should look like this : 
  ```python
-[{'query1': [(3, 'some encrypted content of bytes or strings')]}]
+[{'query 0': ['SUCCESS', [(1, 'some encrypted content of bytes or strings')]]}]
 ```
-If some error has occured while doing a query like : 
+If some error has occurred while doing a query like : 
 ```python
-query1 = 'SELECT COUNT(*) AS cc ,content FROM DoesntExist WHERE key = "#5482A" ORDER BY cc DESC '
+query = 'SELECT COUNT(*) AS cc ,content FROM DoesntExist WHERE key = "#5482A" ORDER BY cc DESC '
 ```
-The result fetched should look similair to this : 
+The result fetched should look similar to this : 
 ```python
-[{'query1': (0, OperationalError('no such table: DoesntExist'))}]
+[{'query 0': ('FAILURE', 'no such table: DoesntExist')}]
 ```
 Thats it so simple !
 
 ## License ##
 This project is licensed under the [MIT LICENSE](https://github.com/AshGw/AES-256/blob/main/LICENSE).
 ## Acknowledgments ##
 This cryptographic scheme is inspired by secure cryptographic practices and various open-source implementations.
```

### Comparing `AshCrypt-1.2.0/LICENSE` & `AshCrypt-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.2.0/PKG-INFO` & `AshCrypt-1.2.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: AshCrypt
-Version: 1.2.0
-Summary: Comprehensive AES-256 Cryptography library equipped with a file handling module along with a text module w/ a user-friendly GUI and a database module to store encrypted content.
+Version: 1.2.1
+Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
-Keywords: Cryptography,AES-256
+Keywords: Cryptography application,cryptography libraryAES-256
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Cryptography Library : AES-256
+# Cryptography App &  Library : AES-256
 ##  Objective ## 
 #### Enhanced Security, Simplicity & Ease of use For Everyone And Anyone Willing To Use AES 256 With No Unnecessary Complications.
 ## Overview ## 
 **Visit The [GitHub](https://github.com/AshGw/AES-256/tree/main) Repository**
 <br>The library incorporates a base cryptography mdoule called **Ash** 
 
 <br>A simple, secure, and developer-oriented module for
@@ -33,38 +33,40 @@
 interface, seamless integration with precompiled 
 functions, and robust security measures to safeguard
 sensitive data,  providing a hassle-free experience when dealing with cryptographic libraries.
 <br>View **Features** Header for more details.
 
 
 
-The library uses that same module to ensure secure data encryption and decryption for Files and Texts while keeping it very easy and simple to use .
-view the headers for **AshFileCrypt**  and **AshTextCrypt** learn more.
 
-It also includes a simple graphical user interface (GUI) for easy interaction with the **AshTextCrypt** module.
-<br>If you're trying to either encrypt or decrypt some messages on the go ( 200 characters max ) you can use this GUI.
-<br>It also has a qr module associated with it to display the message.
-<br>check **GUI**  for more info.
+The project mainly includes a fully fledged application that integrates all the modules in the library merging them into a unified and powerful software solution for developers and for people with no programming knowledge whatsoever
+<br>check `GUI` header for more info.
+
+
+### For Developers ###
+The project uses `Ash` module to ensure secure data encryption and decryption for Files and Texts while keeping it very easy and simple to use .
+view the headers for `AshFileCrypt` and `AshTextCrypt` to learn more.
 
-While The **GUI** is limited to 200 characters of text, if you want to be free over how much data or type of data you want to include, then u can use `CliCrypt.py` which is an innovative command line interface (CLI) designed to provide encryption and decryption capabilities for both text and file data with no constraints
 
 It also incorporates a database module that serve the same purpose which is allowing for the management and storage of classified content in a secure, 
 safe and simple manner, you can use whichever you see fit.
 
+<br>The module has a simple straight forward approach for dealing with sqlite3 databases, even if youre not familiar with Python itself you can still use this module to run SQL queries and built in functions to perform various operations on a given database.<br>
+Check `AshDatabase` header to learn more.
+
 **After the library is installed**
 <br>to run the GUI 
 ```shell
 python -m AshCrypt.AshCryptGUI
 ```
 To run the CLI
 ```shell
 python -m AshCrypt.CliCrypt
 ```
 
-<br>The module has a simple straight forward apporach for dealing with sqlite3 databases, even if youre not familiar with Python itself you can still use this module to run SQL queries and built in functions to perform various operations on a given database.<br>Check **AshDatabase** header to learn more.
 
 ## Ash Module ##
 The `Ash.py` module is a comprehensive collection of carefully designed functions and code modules that facilitate optimal performance and reliability in data encryption and decryption operations  while ensuring the utmost security and 
 confidentiality.
 
 <br>It uses primitives from the `cryptography` library with added security features while keeping it simple and highly flexible to provide a head-ache free solution for developers. 
 
@@ -137,14 +139,57 @@
 ### Regarding KDFs
 Note that bcrypt is intentionally slow and computationally expensive, enhancing protection against brute-force attacks. The number of iterations, including salt and pepper, increases derivation time to strike a balance between security and performance. Use a suitable value based on your machine's capabilities and desired security level.
 
 <br>Im using 50 just to demonstrate the process and make it quick.
 <br>The bare minimum is 50, the max is 100 000, choose somewhere in between.
 <br>In my use case 50 takes around 0.5 secs while using the maximun number of iterations takes around 11 minutes to derive the keys and finish the cryptographic operations at hand.
 
+
+
+## AshCryptGUI ##
+The GUI as mentioned above is a fully fledged application , you can use it to encrypt files , texts , keep track of files by storing them on demand to a main database , also on demand it can keep track of the keys used for cryptographic operations.
+### Usage ###
+1) Set the main key up. If you don't have one , press on the button `generate` to generate a secure safe key ready for use. 
+2) Now you're able to encrypt files or text (text is limited to 200 characters max)
+####  Text : 
+- You can insert some text in the entry right below the `TEXT ENCRYPTION` label.<br>The given text will be encrypted and you can choose if you want to have that text displayed as a qr code, a qr image will pop on the screen and you'll be able to scan it using your phone.
+- Insert some encrypted text below the `TEXT DECRYPTION` label.<br>The Given text will be decrypted and you'd have the option to display the "plaintext" as a qr code to be scanned by other devices.
+#### Files
+- Under the `FILE PATH` label enter the file name (if it's in the current working directory) or submit the whole file path , the file can be of any type, click on `ENCRYPT FILE` Button to encrypt the given file , if the encryption turned out to be successful , you'll see a success message along with a `added .crypt extention to the file` message if the encryption wasn't successful you'll see an error message specifying the problem.<br>Note that you cannot re-encrypt a file that  has `.crypt` as extention.
+- The file name should be changed by now to `filename + '.crypt'` , if the file has .crypt extention you can go ahead and decrypt it , if the same key is used for both enc/dec operations then the result should be `success` + `removed .crypt extention` from the file.
+#### Database
+- Now you have some encrypted/decrypted files but you want to keep them stored somewhere safe, this is where the main database comes in , where you need to store your files + their content + reference to the key used for their encryption/decryption. you can specify your database by 
+1) Specify the actual path where you want your database to be 
+2) Give it a name, it must be a valid file name that ends with `.db` .<br>
+If the database doesn't exist then a database with the name you've given will be created and automatically connected to.<br>If the given database already exists then it will automatically be connected.
+3) Did I mention the keys database ? well if you give a database it will also create a keys database with the same name as the database you chose plus `Keys` added to its name. This database holds the actual keys and the reference to these keys.
+<br>The only common piece of data that the two separate databases have in common are the key reference values.  
+
+**Note** : If your main database gets compromised , then the attacker wouldnt have anything useful , they can never know the actual key from the reference key so no problem with that if it only contains encrypted content BUT NEVER EVER GET YOUR KEYS DATABASE COMPROMISED ! 
+<br>If anyone gets hold of your main database they would only see some encrypted content and some key refrence that is actually 100% independent of the actual key used for encryption so they have nothing , but if they get hold of the keys database they can look for matching refs and use the matching key to decrypt that binary encrypted data to its actual format.
+That's why I made two different databases not two tables within a single database. 
+<br> So you keep your keys database safe and secure.
+
+
+**Info** Both databases have the same table called `Classified` that has 4 columns <br>`ID` which is auto generated & incremented for each piece of data that gets inserted<br>
+`Name` that holds the filename in both databases , although in the keys database if you haven't specified any file to operate on and keep selecting keys the keys name will be `STANDALONE` 
+<br>`Contnet` in the main db that holds the entire content of the given file, in keys db that holds the actual 512 bit long encryption key.
+<br>`Key` in  both db's that holds the `KeyRef` or key reference value
+#### Usage 
+The buttons are self-explanatory so do what you see fit. the result of any task related to the databases is displayed in `DATABASE OUTPUT CONSOLE` although you can run a query anytime by writing a query and using `query` button , the result will be displayed to an `output.json` file that auto-deletes when you exit the app.
+<br>Just click buttons and check the result in the output console, it will guide you the process.
+
+<br>To run the GUI anywhere
+```shell
+python -m AshCrypt.AshCryptGUI
+```
+
+
+
+
 ## AshFileCrypt ## 
 If you want to encrypt a file :
 1) Follow the steps above to set the key up.
 2) Create an instance of the class CryptFiles and pass 2 arguments, the first one being the target file and the second argument being the key :
 ```python
 instance1 = CryptFile('target.txt', key)
 ```
@@ -164,16 +209,23 @@
 target = CryptFile('/User/Desktop/MyProjects/SomeOtherfolder/myfile.txt',key)
 ```
 3) Apply either the encryption or decryption functions to that instance :
 ```python
 instance1 = CryptFile('qrv10.png',key)
 instance1.encrypt()
 ```
-you can apply `print()` on `instance1.encrypt()`to check the result, if it is `1` then everything went ok , if it's `3` then the file doesn't even exists otherwise some other Error has occurred (usually the file is distorted).
-
+you can apply `print()` on `instance1.encrypt()`to check the result :
+<br> 1 : File successfully encrypted/decrypted + added/removed .crypt extension 
+<br> 2 : File is empty
+<br> 3 : File doesn't exist
+<br> 4 : Unknown Error usually a system related one 
+<br> 5 : Key is denied for cryptographic use
+<br> 6 : File is already encrypted/decrypted
+<br> 7 : File is not a file it's a directory
+<br> 0 : Error in enc/dec probable file distortion or tampering or wrong key
 ```python
 instance1.encrypt()
 ```
 ```python
 instance1.decrypt()
 ```
 **Note** : 
@@ -201,20 +253,14 @@
 in `AshFileCryt` & `AshTextCrypt` it's simpler if you attempt to decrypt an non-encrypted message then you'll get the same message back along with an integer in this case `0` for failure.
 <br>`1`'s for success.
 <br>Non `1`'s for failure (`2`/`0.0`/`0`) each indicate different Errors. 
 
 Error handling here has no Exceptions raised just `1`'s, `0`'s & `2`'s for feedback, just to make it simple and Non-Technical.
 
 
-## AshCryptGUI ##
-This is a fully fledged application that integrates all the modules in the library merging them into a unified and powerful software solution. run this command and see for yourself !
-
-```shell
-python -m AshCrypt.AshCryptGUI
-```
 ### QR ## 
 The `qr.py` module is used to display a qr code of the encrypted/decrypted messages to be quickly scanned and transmitted , you can use qr versions from `1` to `40` , although I recommend using `40` since it can take the maximum number of characters for small files , and `10` if you're working with the GUI which is intended for text/short messages,
 
 ## AshDatabase ##
 To support efficient content management, I have integrated this database module to enable the storage and retrieval of encrypted content in a safe and secure manner using an sqlite3 database
 
 Ensuring that the encrypted data remains organized and readily accessible to anyone with the right key. Any content going in must be encrypted with a key that you must keep off grid.
@@ -266,28 +312,28 @@
 
 6) Check the module itself so you can run through all the available methods.
 <br>The methods available perform the usual operations like insertion, deletion , updating the database and more..
 
 
 7) to run more complex queries I've dedicated a query function that takes in *queries and returns the result fetched 
 ```python
-query1 = 'SELECT COUNT(*) AS cc ,content FROM Classified WHERE key = "#5482A" ORDER BY cc DESC '
-print(connect.query(query1))
+query = 'SELECT COUNT(*) AS cc ,content FROM Classified WHERE key = "#5482A" ORDER BY cc DESC '
+print(connect.query(query))
 ```
 The result fetched should look like this : 
  ```python
-[{'query1': [(3, 'some encrypted content of bytes or strings')]}]
+[{'query 0': ['SUCCESS', [(1, 'some encrypted content of bytes or strings')]]}]
 ```
-If some error has occured while doing a query like : 
+If some error has occurred while doing a query like : 
 ```python
-query1 = 'SELECT COUNT(*) AS cc ,content FROM DoesntExist WHERE key = "#5482A" ORDER BY cc DESC '
+query = 'SELECT COUNT(*) AS cc ,content FROM DoesntExist WHERE key = "#5482A" ORDER BY cc DESC '
 ```
-The result fetched should look similair to this : 
+The result fetched should look similar to this : 
 ```python
-[{'query1': (0, OperationalError('no such table: DoesntExist'))}]
+[{'query 0': ('FAILURE', 'no such table: DoesntExist')}]
 ```
 Thats it so simple !
 
 ## License ##
 This project is licensed under the [MIT LICENSE](https://github.com/AshGw/AES-256/blob/main/LICENSE).
 ## Acknowledgments ##
 This cryptographic scheme is inspired by secure cryptographic practices and various open-source implementations.
```

### Comparing `AshCrypt-1.2.0/README.md` & `AshCrypt-1.2.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,54 +1,42 @@
-# Cryptography w/ AES-256
+# Cryptography App & Library w/ AES-256
 ##  Objective ## 
 #### Enhanced Security, Simplicity & Ease of use For Everyone And Anyone Willing To Use AES 256.
 ## Reason Behind It
 In a world where control, surveillance, and privacy violations are increasingly prevalent, the protection of individual freedom becomes crucial. 
 
 As a firm believer in **Freedom** , I have developed a set of tools in Python that leverages the AES-256 algorithm to make it easier for undividuals to safeguard their data without blindly relying on third parties to do it tor them  . 
 
 My aim here is to make these tools accessible and user-friendly, even for individuals with limited programming knowledge. By providing these resources, I hope to contribute to the preservation of privacy and enable individuals to take control of their own data security, so feel free to explore these tools.
 ## Overview ## 
-The project incorporates a library I made called **[AshCrypt](https://github.com/AshGw/AES-256/tree/main/src)** : 
+The project incorporates a library I made called **[AshCrypt](https://github.com/AshGw/AES-256/AshCrypt)** : 
 
 <br>A simple, secure, and developer-oriented library for
 encryption and decryption with AES-256 (CBC) . 
 <br>The core of the library is the module `Ash`
 It offers an intuitive interface, seamless integration with precompiled 
 functions, and robust security measures to safeguard
 sensitive data,  providing a hassle-free experience when dealing with cryptographic libraries.
 <br>View [Features](https://github.com/AshGw/AES-256#features) Header for more details.
 
 
 
-The project uses that same module to ensure secure data encryption and decryption for Files and Texts while keeping it very easy and simple to use .
-view the headers for [AshFileCrypt](https://github.com/AshGw/AES-256/src#ashfilecrypt) and [AshTextCrypt](https://github.com/AshGw/AES-256/src#ashtextcrypt) to learn more.
+The project mainly includes a fully fledged application that integrates all the modules in the library merging them into a unified and powerful software solution for developers and for people with no programming knowledge whatsoever
+<br>check [GUI](https://github.com/AshGw/AES-256#AshCryptGUI) header for more info.
 
-It also includes a simple graphical user interface (GUI) for easy interaction with the AshTextCrypt module.
-<br>If you're trying to either encrypt or decrypt some messages on the go ( 200 characters max ) you can use this GUI.
-<br>It also has a qr module associated with it to display the message.
-<br>check [GUI](https://github.com/AshGw/AES-256/src#ashcryptgui) header for more info.
 
+### For Developers ###
+The project uses `Ash` module to ensure secure data encryption and decryption for Files and Texts while keeping it very easy and simple to use .
+view the headers for [AshFileCrypt](https://github.com/AshGw/AES-256#ashfilecrypt) and [AshTextCrypt](https://github.com/AshGw/AES-256#ashtextcrypt) to learn more.
 
-While The **GUI** is limited to 200 characters of text, if you want to be free over how much data or type of data you want to include, then u can use `CliCrypt.py` which is an innovative command line interface (CLI) designed to provide encryption and decryption capabilities for both text and file data with no constraints.
-
-**After the library is installed** 
-<br>To run the GUI 
-```shell
-python -m AshCrypt.AshCryptGUI
-```
-To run the CLI 
-```shell
-python -m AshCrypt.CliCrypt
-```
 
 It also incorporates a database module that serve the same purpose which is allowing for the management and storage of classified content in a secure, 
 safe and simple manner, you can use whichever you see fit.
 
-<br>The module has a simple straight forward apporach for dealing with sqlite3 databases, even if youre not familiar with Python itself you can still use this module to run SQL queries and built in functions to perform various operations on a given database.<br>Check [AshDatabase](https://github.com/AshGw/CryptographyAES-256#ashdatabase) header to learn more.
+<br>The module has a simple straight forward approach for dealing with sqlite3 databases, even if you're not familiar with Python itself you can still use this module to run SQL queries and built in functions to perform various operations on a given database.<br>Check [AshDatabase](https://github.com/AshGw#AshDatabase) header to learn more.
 
 ## Installation ##
 You can simply use **pip**
 <br>First upgrade the package installer 
 ```bash
 pip install --upgrade pip 
 ```
@@ -98,22 +86,37 @@
 3) If you're running `python 3.6` or older then you might need to install `dataclasses`
 ```
 pip install dataclasses
 ```
 <br>Now if none of this works you might just use the docker image for this purpose, so check this [directory](docker-build)
 </details>
 
+**After the library is installed** 
+<br>To run the GUI 
+```shell
+python -m AshCrypt.AshCryptGUI
+```
+
+**NOTE**:
+You  can use `CliCrypt.py` which is an innovative command line interface (CLI) designed to provide encryption and decryption capabilities for both text and file data with no constraints intended for use within systems where you can't use GUI's.
+
+
+To run the CLI 
+```shell
+python -m AshCrypt.CliCrypt
+```
+
 ## Ash Module ##
 The `Ash.py` Module is a comprehensive collection of carefully designed functions and code modules that facilitate optimal performance and reliability in data encryption and decryption operations  while ensuring the utmost security and 
 confidentiality.
 
 <br>It uses primitives from the `cryptography.py` library with added security features while keeping it simple and highly flexible to provide a head-ache free solution for developers. 
 
 <br>You can check [Features](https://github.com/AshGw/AES-256#features) tag below to learn more about the security features.
-<br>You can check the [unittesting file](unittestsAC/unittestAsh.py) to verify how it works.
+<br>You can check the [unittesting file](AshCryt/unittests/unittestAsh.py) to verify how it works.
 
 ### Usage ##
 1) Generate a key if you don't have one already
 ```python
 mainkey = Enc.genMainkey()
 ```
 2) Before encrypting or decrypting anything, first set the arguments you want to pass, you can have an encrypted message or a  decrypted message , and a mainkey to use.
@@ -178,14 +181,56 @@
 ### Regarding KDFs
 Note that bcrypt is intentionally slow and computationally expensive, enhancing protection against brute-force attacks. The number of iterations, including salt and pepper, increases derivation time to strike a balance between security and performance. Use a suitable value based on your machine's capabilities and desired security level.
 
 <br>Im using 50 just to demonstrate the process and make it quick.
 <br>The bare minimum is 50, the max is 100 000, choose somewhere in between.
 <br>In my use case 50 takes around 0.5 secs while using the maximun number of iterations takes around 11 minutes to derive the keys and finish the cryptographic operations at hand.
 
+## AshCryptGUI ##
+![alt text](important/GUI.png)
+The GUI as mentioned above is a fully fledged application , you can use it to encrypt files , texts , keep track of files by storing them on demand to a main database , also on demand it can keep track of the keys used for cryptographic operations.
+### Usage ###
+1) Set the main key up. If you don't have one , press on the button `generate` to generate a secure safe key ready for use. 
+2) Now you're able to encrypt files or text (text is limited to 200 characters max)
+####  Text : 
+- You can insert some text in the entry right below the `TEXT ENCRYPTION` label.<br>The given text will be encrypted and you can choose if you want to have that text displayed as a qr code, a qr image will pop on the screen and you'll be able to scan it using your phone.
+- Insert some encrypted text below the `TEXT DECRYPTION` label.<br>The Given text will be decrypted and you'd have the option to display the "plaintext" as a qr code to be scanned by other devices.
+#### Files
+- Under the `FILE PATH` label enter the file name (if it's in the current working directory) or submit the whole file path , the file can be of any type, click on `ENCRYPT FILE` Button to encrypt the given file , if the encryption turned out to be successful , you'll see a success message along with a `added .crypt extention to the file` message if the encryption wasn't successful you'll see an error message specifying the problem.<br>Note that you cannot re-encrypt a file that  has `.crypt` as extention.
+- The file name should be changed by now to `filename + '.crypt'` , if the file has .crypt extention you can go ahead and decrypt it , if the same key is used for both enc/dec operations then the result should be `success` + `removed .crypt extention` from the file.
+#### Database
+- Now you have some encrypted/decrypted files but you want to keep them stored somewhere safe, this is where the main database comes in , where you need to store your files + their content + reference to the key used for their encryption/decryption. you can specify your database by 
+1) Specify the actual path where you want your database to be 
+2) Give it a name, it must be a valid file name that ends with `.db` .<br>
+If the database doesn't exist then a database with the name you've given will be created and automatically connected to.<br>If the given database already exists then it will automatically be connected.
+3) Did I mention the keys database ? well if you give a database it will also create a keys database with the same name as the database you chose plus `Keys` added to its name. This database holds the actual keys and the reference to these keys.
+<br>The only common piece of data that the two separate databases have in common are the key reference values.  
+
+**Note** : If your main database gets compromised , then the attacker wouldnt have anything useful , they can never know the actual key from the reference key so no problem with that if it only contains encrypted content BUT NEVER EVER GET YOUR KEYS DATABASE COMPROMISED ! 
+<br>If anyone gets hold of your main database they would only see some encrypted content and some key refrence that is actually 100% independent of the actual key used for encryption so they have nothing , but if they get hold of the keys database they can look for matching refs and use the matching key to decrypt that binary encrypted data to its actual format.
+That's why I made two different databases not two tables within a single database. 
+<br> So you keep your keys database safe and secure.
+
+
+**Info** Both databases have the same table called `Classified` that has 4 columns <br>`ID` which is auto generated & incremented for each piece of data that gets inserted<br>
+`Name` that holds the filename in both databases , although in the keys database if you haven't specified any file to operate on and keep selecting keys the keys name will be `STANDALONE` 
+<br>`Contnet` in the main db that holds the entire content of the given file, in keys db that holds the actual 512 bit long encryption key.
+<br>`Key` in  both db's that holds the `KeyRef` or key reference value
+#### Usage 
+The buttons are self-explanatory so do what you see fit. the result of any task related to the databases is displayed in `DATABASE OUTPUT CONSOLE` although you can run a query anytime by writing a query and using `query` button , the result will be displayed to an `output.json` file that auto-deletes when you exit the app.
+<br>Just click buttons and check the result in the output console, it will guide you the process.
+
+<br>To run the GUI anywhere
+```shell
+python -m AshCrypt.AshCryptGUI
+```
+
+
+
+
 ## AshFileCrypt ## 
 If you want to encrypt a file :
 1) Follow the steps above to set the key up.
 2) Create an instance of the class CryptFiles and pass 2 arguments, the first one being the target file and the second argument being the key :
 ```python
 instance1 = CryptFile('target.txt', key)
 ```
@@ -205,16 +250,23 @@
 target = CryptFile('/User/Desktop/MyProjects/SomeOtherfolder/myfile.txt',key)
 ```
 3) Apply either the encryption or decryption functions to that instance :
 ```python
 instance1 = CryptFile('qrv10.png',key)
 instance1.encrypt()
 ```
-you can apply `print()` on `instance1.encrypt()`to check the result, if it is `1` then everything went ok , if it's `3` then the file doesn't even exists otherwise some other Error has occurred (usually the file is distorted).
-
+you can apply `print()` on `instance1.encrypt()`to check the result :
+<br> 1 : File successfully encrypted/decrypted + added/removed .crypt extension 
+<br> 2 : File is empty
+<br> 3 : File doesn't exist
+<br> 4 : Unknown Error usually a system related one 
+<br> 5 : Key is denied for cryptographic use
+<br> 6 : File is already encrypted/decrypted
+<br> 7 : File is not a file it's a directory
+<br> 0 : Error in enc/dec probable file distortion or tampering or wrong key
 ```python
 instance1.encrypt()
 ```
 ```python
 instance1.decrypt()
 ```
 **Note** : 
@@ -242,22 +294,14 @@
 in `AshFileCryt` & `AshTextCrypt` it's simpler if you attempt to decrypt an non-encrypted message then you'll get the same message back along with an integer in this case `0` for failure.
 <br>`1`'s for success.
 <br>Non `1`'s for failure (`2`/`0.0`/`0`) each indicate different Errors. 
 
 Error handling here has no Exceptions raised just `1`'s, `0`'s & `2`'s for feedback, just to make it simple and Non-Technical.
 
 
-## AshCryptGUI ##
-This is a fully fledged application that integrates all the modules in the library merging them into a unified and powerful software solution
-![alt text](important/GUI.png)
-
-<br>To run the GUI anywhere
-```shell
-python -m AshCrypt.AshCryptGUI
-```
 ### QR ## 
 The `qr.py` module is used to display a qr code of the encrypted/decrypted messages to be quickly scanned and transmitted , you can use qr versions from `1` to `40` , although I recommend using `40` since it can take the maximum number of characters for small files , and `10` if you're working with the GUI which is intended for text/short messages,
 
 ## AshDatabase ##
 To support efficient content management, I have integrated this database module to enable the storage and retrieval of encrypted content in a safe and secure manner using an sqlite3 database
 
 Ensuring that the encrypted data remains organized and readily accessible to anyone with the right key. Any content going in must be encrypted with a key that you must keep off grid.
@@ -309,28 +353,28 @@
 
 6) Check the module itself so you can run through all the available methods.
 <br>The methods available perform the usual operations like insertion, deletion , updating the database and more..
 
 
 7) to run more complex queries I've dedicated a query function that takes in *queries and returns the result fetched 
 ```python
-query1 = 'SELECT COUNT(*) AS cc ,content FROM Classified WHERE key = "#5482A" ORDER BY cc DESC '
-print(connect.query(query1))
+query = 'SELECT COUNT(*) AS cc ,content FROM Classified WHERE key = "#5482A" ORDER BY cc DESC '
+print(connect.query(query))
 ```
 The result fetched should look like this : 
  ```python
-[{'query1': [(3, 'some encrypted content of bytes or strings')]}]
+[{'query 0': ['SUCCESS', [(1, 'some encrypted content of bytes or strings')]]}]
 ```
-If some error has occured while doing a query like : 
+If some error has occurred while doing a query like : 
 ```python
-query1 = 'SELECT COUNT(*) AS cc ,content FROM DoesntExist WHERE key = "#5482A" ORDER BY cc DESC '
+query = 'SELECT COUNT(*) AS cc ,content FROM DoesntExist WHERE key = "#5482A" ORDER BY cc DESC '
 ```
-The result fetched should look similair to this : 
+The result fetched should look similar to this : 
 ```python
-[{'query1': (0, OperationalError('no such table: DoesntExist'))}]
+[{'query 0': ('FAILURE', 'no such table: DoesntExist')}]
 ```
 Thats it so simple !
 
 ## License ##
 This project is licensed under the [MIT LICENSE](https://github.com/AshGw/AES-256/blob/main/LICENSE).
 ## Acknowledgments ##
 This cryptographic scheme is inspired by secure cryptographic practices and various open-source implementations.
```

### Comparing `AshCrypt-1.2.0/setup.py` & `AshCrypt-1.2.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup , find_packages
 
 with open('AshCrypt/README.md','r') as f:
     readme = f.read()
 
 setup(
     name='AshCrypt',
-    version='1.2.0',
+    version='1.2.1',
     author='Ashref Gwader',
     author_email='AshrefGw@proton.me',
     python_requires='>=3.7',
-    description="Comprehensive AES-256 Cryptography library equipped with a file handling module along with"
-                " a text module w/ a user-friendly GUI and a database module to store encrypted content.",
+    description="Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with"
+                " a database module to store encrypted content.",
     long_description_content_type='text/markdown',
     long_description=readme,
     url='https://github.com/AshGw/AES-256.git',
     packages=find_packages(exclude=['important', 'docker-build']),
     package_data={
         'AshCrypt': ['**'],
     },
@@ -37,11 +37,12 @@
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
     ],
     keywords=[
-        'Cryptography',
+        'Cryptography application',
+        'cryptography library'
         'AES-256',
     ],
 )
```

