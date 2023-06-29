# Comparing `tmp/advancedfernetdataencryption-1.0.1.tar.gz` & `tmp/advancedfernetdataencryption-1.1.tar.gz`

## Comparing `advancedfernetdataencryption-1.0.1.tar` & `advancedfernetdataencryption-1.1.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rwxr-xr-x   0        0        0      694 2020-02-02 00:00:00.000000 advancedfernetdataencryption-1.0.1/.pypirc
--rwxr-xr-x   0        0        0     4604 2020-02-02 00:00:00.000000 advancedfernetdataencryption-1.0.1/AdvancedFernetDataEncryption.py
--rwxr-xr-x   0        0        0      390 2020-02-02 00:00:00.000000 advancedfernetdataencryption-1.0.1/__init__.py
--rwxr-xr-x   0        0        0      117 2020-02-02 00:00:00.000000 advancedfernetdataencryption-1.0.1/requirements.txt
--rwxr-xr-x   0        0        0     1058 2020-02-02 00:00:00.000000 advancedfernetdataencryption-1.0.1/test/test_encryption.py
--rwxr-xr-x   0        0        0     1069 2020-02-02 00:00:00.000000 advancedfernetdataencryption-1.0.1/LICENSE
--rwxr-xr-x   0        0        0     1390 2020-02-02 00:00:00.000000 advancedfernetdataencryption-1.0.1/README.md
--rwxr-xr-x   0        0        0      805 2020-02-02 00:00:00.000000 advancedfernetdataencryption-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 advancedfernetdataencryption-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     4726 2020-02-02 00:00:00.000000 advancedfernetdataencryption-1.1/AdvancedFernetDataEncryption.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 advancedfernetdataencryption-1.1/__init__.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 advancedfernetdataencryption-1.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 advancedfernetdataencryption-1.1/test/test_encryption.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 advancedfernetdataencryption-1.1/LICENSE
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 advancedfernetdataencryption-1.1/README.md
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 advancedfernetdataencryption-1.1/pyproject.toml
+-rw-r--r--   0        0        0     2456 2020-02-02 00:00:00.000000 advancedfernetdataencryption-1.1/PKG-INFO
```

### Comparing `advancedfernetdataencryption-1.0.1/AdvancedFernetDataEncryption.py` & `advancedfernetdataencryption-1.1/AdvancedFernetDataEncryption.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-from operator import indexOf
-import cryptography
-from cryptography.fernet import Fernet
-from datetime import datetime
-import string, random
-
-def passwordToken():
-    #---- Generates a random token that is stored that will be used to encrypt user data ----
-    passwordToken = ''.join(random.choice(string.ascii_lowercase + string.digits + string.ascii_uppercase + string.punctuation) for _ in range(random.randint(100,120)))
-    RandomTextPoint = random.randrange(len(passwordToken))
-    RandomInputToken, RandomInputKey = encryption(''.join(random.choice(string.ascii_lowercase + string.digits + string.ascii_uppercase + string.punctuation) for _ in range(random.randint(100,120))))
-    randominputprivateKey =  RandomInputKey.decode("UTF-8") + RandomInputToken.decode("UTF-8")  
-    text = passwordToken[:RandomTextPoint] + randominputprivateKey + passwordToken[RandomTextPoint:]
-    privateToken, privateKey = encryption(text)
-    return privateKey.decode("UTF-8") + ":" + privateToken.decode("UTF-8")   
-
-def generateSessionToken(username):
-    #---- Generates a random 128 character long SessionToken 
-    sessionToken = ''.join(random.choice(string.ascii_lowercase + string.digits + string.ascii_uppercase) for _ in range(random.randint(100,120)))
-    return encryption(username + ":" + sessionToken)
-
-def dataEncrpytion(text):
-    #---- Generate a random 128 character password with password to show on the servers and files to save ----
-    RandomText = ''.join(random.choice(text + string.ascii_lowercase + string.digits + string.ascii_uppercase + string.punctuation) for _ in range(random.randint(100,120)))
-    #---- Creates a random number within the bounds of the length of passwords (basically shoves text in a random location) ----
-    TextPoint = random.randrange(len(text))
-    RandomTextPoint = random.randrange(len(RandomText))
-    RandomToken = passwordToken()
-    #---- Combine all the random points and text together to store this password ----
-    text = text[:TextPoint] + RandomText[:RandomTextPoint] + RandomToken + RandomText[RandomTextPoint:] + text[TextPoint:]
-    TextToken, TextKey = encryption(text)
-    timestamp = datetime.utcfromtimestamp(Fernet(str.encode(RandomToken.split(":")[0])).extract_timestamp(str.encode(RandomToken.split(":")[1]))).strftime(''.join(random.choice('%d%H%d%M%d%S') for _ in range(20,30)))
-    RandomTextToken, RandomTextKey = encryption(RandomText)
-    return TextKey.decode("utf-8") +":" + timestamp[0:random.randint(1, len(timestamp))] +"=" + TextToken.decode("utf-8") + ":" + timestamp[0:random.randint(1, len(timestamp))] +"=" + RandomTextToken.decode("UTF-8") + ":" + timestamp[0:random.randint(1, len(timestamp))] + "=" + RandomTextKey.decode("UTF-8") +":" + timestamp[0:random.randint(1, len(timestamp))]  + "=" + RandomToken
-
-def encryption(text):
-    #---- Changes string to byte format ----
-    bytetext = str.encode(text)
-    #--- Generates a special key ----
-    key = Fernet.generate_key()
-    encryption_type = Fernet(key)
-    #---- Makes Token string an encrypted fernet with the generated key for the byte string ----
-    token = encryption_type.encrypt(bytetext)
-    #---- Returns encrypted text text format ----
-    return token, key
-
-def dataDecryption(EncryptedText):
-    ShortenedText = EncryptedText.split(":")[len(EncryptedText.split(":"))-2]
-    RandomKey = ShortenedText[ShortenedText.index("=")+1:len(ShortenedText)]
-    RandomToken = EncryptedText.split(":")[len(EncryptedText.split(":"))-1]
-    timestamp = datetime.utcfromtimestamp(Fernet(str.encode(RandomKey)).extract_timestamp(str.encode(RandomToken))).strftime('%d%H:%d%M:%d%S')
-    Textkey = EncryptedText.split(":")[0]
-    textToken = CleanToken(EncryptedText.split(":")[1], timestamp)
-    RandomtextToken = CleanToken(EncryptedText.split(":")[2], timestamp)
-    RandomtextKey = CleanToken(EncryptedText.split(":")[3], timestamp)
-    return str(decryption(str.encode(textToken), str.encode(Textkey))).replace(RandomKey +":" + RandomToken, "").replace(str(decryption(str.encode(RandomtextToken), str.encode(RandomtextKey))), "")
-
-def CleanToken(TokenString, timestamp):
-    for x in timestamp +"%:dHMS":
-        if x+"=" in TokenString:
-            cleanToken = TokenString[TokenString.index(x+"=") +2: len(TokenString)]
-            if TokenString.index(x+"=") < 30:
-                break
-    return cleanToken
-
-def decryption(token, key):
-    #---- Will decrypt the encrypted text with a token and key ----
-    encryption_type = Fernet(key)
-    return encryption_type.decrypt(token).decode()
+from operator import indexOf
+import cryptography
+from cryptography.fernet import Fernet
+from datetime import datetime
+import string, random
+
+def passwordToken(MinLength=100, MaxLength=120):
+    #---- Generates a random token that is stored that will be used to encrypt user data ----
+    passwordToken = ''.join(random.choice(string.ascii_lowercase + string.digits + string.ascii_uppercase + string.punctuation) for _ in range(random.randint(MinLength,MaxLength)))
+    RandomTextPoint = random.randrange(len(passwordToken))
+    RandomInputToken, RandomInputKey = encryption(''.join(random.choice(string.ascii_lowercase + string.digits + string.ascii_uppercase + string.punctuation) for _ in range(random.randint(100,120))))
+    randominputprivateKey =  RandomInputKey.decode("UTF-8") + RandomInputToken.decode("UTF-8")  
+    text = passwordToken[:RandomTextPoint] + randominputprivateKey + passwordToken[RandomTextPoint:]
+    privateToken, privateKey = encryption(text)
+    return privateKey.decode("UTF-8") + ":" + privateToken.decode("UTF-8")   
+
+def generateSessionToken(username, MinLength=100, MaxLength=120):
+    #---- Generates a random 128 character long SessionToken 
+    sessionToken = ''.join(random.choice(string.ascii_lowercase + string.digits + string.ascii_uppercase) for _ in range(random.randint(MinLength,MaxLength)))
+    return encryption(username + ":" + sessionToken)
+
+def dataEncrpytion(text, MinLength=100, MaxLength=120):
+    #---- Generate a random 128 character password with password to show on the servers and files to save ----
+    RandomText = ''.join(random.choice(text + string.ascii_lowercase + string.digits + string.ascii_uppercase + string.punctuation) for _ in range(random.randint(MinLength,MaxLength)))
+    #---- Creates a random number within the bounds of the length of passwords (basically shoves text in a random location) ----
+    TextPoint = random.randrange(len(text))
+    RandomTextPoint = random.randrange(len(RandomText))
+    RandomToken = passwordToken(MinLength, MaxLength)
+    #---- Combine all the random points and text together to store this password ----
+    text = text[:TextPoint] + RandomText[:RandomTextPoint] + RandomToken + RandomText[RandomTextPoint:] + text[TextPoint:]
+    TextToken, TextKey = encryption(text)
+    timestamp = datetime.utcfromtimestamp(Fernet(str.encode(RandomToken.split(":")[0])).extract_timestamp(str.encode(RandomToken.split(":")[1]))).strftime(''.join(random.choice(['%d','%H','%d','%M','%d','%S']) for _ in range(int(MinLength/4),int(MaxLength/2))))
+    RandomTextToken, RandomTextKey = encryption(RandomText)
+    return TextKey.decode("utf-8") +":" + timestamp[0:random.randint(1, len(timestamp))] +"/" + TextToken.decode("utf-8") + ":" + timestamp[0:random.randint(1, len(timestamp))] +"/" + RandomTextToken.decode("UTF-8") + ":" + timestamp[0:random.randint(1, len(timestamp))] + "/" + RandomTextKey.decode("UTF-8") +":" + timestamp[0:random.randint(1, len(timestamp))]  + "/" + RandomToken
+
+def encryption(text):
+    #---- Changes string to byte format ----
+    bytetext = str.encode(text)
+    #--- Generates a special key ----
+    key = Fernet.generate_key()
+    encryption_type = Fernet(key)
+    #---- Makes Token string an encrypted fernet with the generated key for the byte string ----
+    token = encryption_type.encrypt(bytetext)
+    #---- Returns encrypted text text format ----
+    return token, key
+
+def dataDecryption(EncryptedText):
+    ShortenedText = EncryptedText.split(":")[len(EncryptedText.split(":"))-2]
+    RandomKey = ShortenedText[ShortenedText.index("/")+1:len(ShortenedText)]
+    RandomToken = EncryptedText.split(":")[len(EncryptedText.split(":"))-1]
+    timestamp = datetime.utcfromtimestamp(Fernet(str.encode(RandomKey)).extract_timestamp(str.encode(RandomToken))).strftime('%d%H:%d%M:%d%S')
+    Textkey = EncryptedText.split(":")[0]
+    textToken = CleanToken(EncryptedText.split(":")[1], timestamp)
+    RandomtextToken = CleanToken(EncryptedText.split(":")[2], timestamp)
+    RandomtextKey = CleanToken(EncryptedText.split(":")[3], timestamp)
+    return str(decryption(str.encode(textToken), str.encode(Textkey))).replace(RandomKey +":" + RandomToken, "").replace(str(decryption(str.encode(RandomtextToken), str.encode(RandomtextKey))), "")
+
+def CleanToken(TokenString, timestamp):
+    for x in timestamp +"%:dHMS":
+        if x+"/" in TokenString:
+            cleanToken = TokenString[TokenString.index(x+"/") +2: len(TokenString)]
+            if TokenString.index(x+"/") < 30:
+                break
+    return cleanToken
+
+def decryption(token, key):
+    #---- Will decrypt the encrypted text with a token and key ----
+    encryption_type = Fernet(key)
+    return encryption_type.decrypt(token).decode()
```

### Comparing `advancedfernetdataencryption-1.0.1/LICENSE` & `advancedfernetdataencryption-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `advancedfernetdataencryption-1.0.1/README.md` & `advancedfernetdataencryption-1.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,27 @@
-# **AdvancedFernetDataEncryption**
-
-An encryption that uses the Fernet symetric key generator and random values to create a secure token and key that can be stored and still be unreadable to any user. 
-
-## **Methods Supported**
-- generateSessionToken(<AnyString>): Generates a random 120 length string and encrypts with fernet symetric algorithm. Used for Web Sessions `return Token, Key`
-- dataEncryption(<PlainTxt>): Generates a random 120 length string and shoves it randomly in the PlainTxt and shoves the token randomly in the 120 length string generated. Then all of this information is encrypted with the fernet algorithm. `return <string>`
-- dataDecrpytion(<EncyptedTxt>): Decodes the giant encrypted text generated and creates a plain text version `return <String>`
-- decryption(<EncryptedTxt>): Decodes the basic encrypted text generated and creates a plain text version `return <String>` Recommended to use only this method for the generated session token
-
-## **Basic Usage Example**
-```python
-from Encryption.AdvancedFernetDataEncryption import *
-
-text = "Hello I would like to be encrypted
-encryptedText = dataEncryption(text)
-unencryptedText = dataDecrpytion(encryptedText)
-```
-
-When run these following lines the text will be encrypted and would be unecryptable without the usage of the Token generated, which is randomly generated for each encrypted text.
+# **AdvancedFernetDataEncryption**
+
+An encryption that uses the Fernet symetric key generator and random values to create a secure token and key that can be stored and still be unreadable to any user. 
+
+## **Methods Supported**
+- generateSessionToken(<AnyString>): Generates a random 120 length string and encrypts with fernet symetric algorithm. Used for Web Sessions `return Token, Key`
+- dataEncryption(<PlainTxt>): Generates a random 120 length string and shoves it randomly in the PlainTxt and shoves the token randomly in the 120 length string generated. Then all of this information is encrypted with the fernet algorithm. `return <string>`
+- dataDecrpytion(<EncyptedTxt>): Decodes the giant encrypted text generated and creates a plain text version `return <String>`
+- decryption(<EncryptedTxt>): Decodes the basic encrypted text generated and creates a plain text version `return <String>` Recommended to use only this method for the generated session token
+  
+## **Package Installation**
+  pip install AdvancedFernetDataEncryption
+More Info can be found on pypi.org [here](https://pypi.org/project/AdvancedFernetDataEncryption/)
+
+## **Basic Usage Example**
+```python
+from Encryption.AdvancedFernetDataEncryption import *
+
+text = "Hello I would like to be encrypted
+encryptedText = dataEncryption(text, MinLength=20, MaxLength=100)
+unencryptedText = dataDecrpytion(encryptedText)
+```
+
+When run these following lines the text will be encrypted and would be unecryptable without the usage of the Token generated, which is randomly generated for each encrypted text.
+
+## **Example of Encryption Result**
+<img width="848" alt="image" src="https://user-images.githubusercontent.com/34069094/199623092-733cfb1f-a78d-43d5-add9-47c879c6e06a.png">
```

### Comparing `advancedfernetdataencryption-1.0.1/PKG-INFO` & `advancedfernetdataencryption-1.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AdvancedFernetDataEncryption
-Version: 1.0.1
+Version: 1.1
 Summary: An encryption that uses the Fernet assymetric key generator and random values to create a secure token and key that can be stored and still be unreadable to any user.
 Project-URL: Homepage, https://github.com/garfield8123/AdvancedFernetDataEncryption
 Project-URL: Bug Tracker, https://github.com/garfield8123/AdvancedFernetDataEncryption/issues
 Author-email: garfield8123 <garfield8123@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,18 +17,25 @@
 An encryption that uses the Fernet symetric key generator and random values to create a secure token and key that can be stored and still be unreadable to any user. 
 
 ## **Methods Supported**
 - generateSessionToken(<AnyString>): Generates a random 120 length string and encrypts with fernet symetric algorithm. Used for Web Sessions `return Token, Key`
 - dataEncryption(<PlainTxt>): Generates a random 120 length string and shoves it randomly in the PlainTxt and shoves the token randomly in the 120 length string generated. Then all of this information is encrypted with the fernet algorithm. `return <string>`
 - dataDecrpytion(<EncyptedTxt>): Decodes the giant encrypted text generated and creates a plain text version `return <String>`
 - decryption(<EncryptedTxt>): Decodes the basic encrypted text generated and creates a plain text version `return <String>` Recommended to use only this method for the generated session token
+  
+## **Package Installation**
+  pip install AdvancedFernetDataEncryption
+More Info can be found on pypi.org [here](https://pypi.org/project/AdvancedFernetDataEncryption/)
 
 ## **Basic Usage Example**
 ```python
 from Encryption.AdvancedFernetDataEncryption import *
 
 text = "Hello I would like to be encrypted
-encryptedText = dataEncryption(text)
+encryptedText = dataEncryption(text, MinLength=20, MaxLength=100)
 unencryptedText = dataDecrpytion(encryptedText)
 ```
 
-When run these following lines the text will be encrypted and would be unecryptable without the usage of the Token generated, which is randomly generated for each encrypted text.
+When run these following lines the text will be encrypted and would be unecryptable without the usage of the Token generated, which is randomly generated for each encrypted text.
+
+## **Example of Encryption Result**
+<img width="848" alt="image" src="https://user-images.githubusercontent.com/34069094/199623092-733cfb1f-a78d-43d5-add9-47c879c6e06a.png">
```

