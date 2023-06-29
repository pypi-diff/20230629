# Comparing `tmp/error-alerts-5.1.tar.gz` & `tmp/error-alerts-5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "error-alerts-5.1.tar", last modified: Tue Jun 27 12:24:15 2023, max compression
+gzip compressed data, was "error-alerts-5.2.tar", last modified: Thu Jun 29 13:22:43 2023, max compression
```

## Comparing `error-alerts-5.1.tar` & `error-alerts-5.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 12:24:15.910360 error-alerts-5.1/
--rw-rw-rw-   0        0        0       35 2022-03-16 16:39:52.000000 error-alerts-5.1/.gitignore
--rw-rw-rw-   0        0        0     1301 2023-06-27 12:24:15.910360 error-alerts-5.1/PKG-INFO
--rw-rw-rw-   0        0        0      994 2023-06-27 12:00:22.000000 error-alerts-5.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-27 12:24:15.904364 error-alerts-5.1/error_alerts/
--rw-rw-rw-   0        0        0     3307 2023-06-27 12:24:07.000000 error-alerts-5.1/error_alerts/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 12:24:15.909361 error-alerts-5.1/error_alerts.egg-info/
--rw-rw-rw-   0        0        0     1301 2023-06-27 12:24:15.000000 error-alerts-5.1/error_alerts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-06-27 12:24:15.000000 error-alerts-5.1/error_alerts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 12:24:15.000000 error-alerts-5.1/error_alerts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-06-27 12:24:15.000000 error-alerts-5.1/error_alerts.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-27 12:24:15.000000 error-alerts-5.1/error_alerts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-27 12:24:15.911360 error-alerts-5.1/setup.cfg
--rw-rw-rw-   0        0        0      462 2023-06-27 12:24:11.000000 error-alerts-5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 13:22:43.223208 error-alerts-5.2/
+-rw-rw-rw-   0        0        0       35 2022-03-16 16:39:52.000000 error-alerts-5.2/.gitignore
+-rw-rw-rw-   0        0        0     1301 2023-06-29 13:22:43.223208 error-alerts-5.2/PKG-INFO
+-rw-rw-rw-   0        0        0      994 2023-06-27 12:00:22.000000 error-alerts-5.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 13:22:43.218211 error-alerts-5.2/error_alerts/
+-rw-rw-rw-   0        0        0     4273 2023-06-29 13:22:32.000000 error-alerts-5.2/error_alerts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 13:22:43.222208 error-alerts-5.2/error_alerts.egg-info/
+-rw-rw-rw-   0        0        0     1301 2023-06-29 13:22:42.000000 error-alerts-5.2/error_alerts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-06-29 13:22:43.000000 error-alerts-5.2/error_alerts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 13:22:42.000000 error-alerts-5.2/error_alerts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-06-29 13:22:42.000000 error-alerts-5.2/error_alerts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-29 13:22:42.000000 error-alerts-5.2/error_alerts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-29 13:22:43.224207 error-alerts-5.2/setup.cfg
+-rw-rw-rw-   0        0        0      462 2023-06-29 13:22:36.000000 error-alerts-5.2/setup.py
```

### Comparing `error-alerts-5.1/PKG-INFO` & `error-alerts-5.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: error-alerts
-Version: 5.1
+Version: 5.2
 Summary: Error alerts via Telegram
 Home-page: https://github.com/xjxckk/error-alerts/
 Download-URL: https://github.com/xjxckk/error-alerts/archive/refs/tags/v2.tar.gz
 Description-Content-Type: text/markdown
 
 ### error-alerts
 Python error alerts via Telegram
```

### Comparing `error-alerts-5.1/README.md` & `error-alerts-5.2/README.md`

 * *Files identical despite different names*

### Comparing `error-alerts-5.1/error_alerts/__init__.py` & `error-alerts-5.2/error_alerts/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,20 +4,22 @@
 DEFAULT_IGNORED_ERRORS = [
     'The service is currently unavailable', # Google sheets API down
     'Could not authenticate you', # Twitter app suspended
     ]
 
 class alerts(Bot):
     def __init__(self, token=None, channel=None, logger=None, full_error=True, raise_error=False, resend_repeat_errors=True):
-        if token:
+        if token and channel:
             bot = super()
             bot.__init__(token=token)
-            self.message = bot.send_message
             self.telegram_bot = bot
 
+            chat = self.get_chat(channel)
+            # print(chat.title)
+
         self.channel = channel
         if logger:
             self.log, self.current_time = logger.log, logger.current_time
         else:
             self.log = None
         self.full_error = full_error
         self.raise_error = raise_error
@@ -38,45 +40,68 @@
         if error != self.last_error or self.resend_repeat_errors:
 
             if channel:
                 if all(ignored_error not in error for ignored_error in DEFAULT_IGNORED_ERRORS):
                     self.last_error = error
 
                     try:
-                        self.message(channel, message[:4096])
+                        self.telegram_bot.send_message(channel, message[:4096])
                     except Exception as telegram_error:
                         self.printer('Error sending alert message to Telegram:', telegram_error, level='error')
 
         if self.raise_error:
             raise Exception('Raiser') from exception
 
-    def send_message(self, *messages, print_message=True, current_time=True, channel=None, buttons_dict={}):
+    def send_message(self, *messages, print_message=True, current_time=True, channel=None, buttons={}):
+        'buttons should be a list or dict, 64 character limit'
         if not channel:
             channel = self.channel
         final_message = ''
         for message in messages:
             final_message += message
             final_message += ' '
         if print_message:
             self.printer(final_message, current_time=current_time)
         if channel:
-            buttons_markup = self.convert_dict_to_buttons(buttons_dict)
+            buttons_markup = self.convert_to_buttons(buttons)
             try:
-                message = self.message(channel, final_message[:4096], reply_markup=buttons_markup)
+                message = self.telegram_bot.send_message(channel, final_message[:4096], reply_markup=buttons_markup)
                 return message
             except Exception as telegram_error:
                 self.printer('Error sending message to Telegram:', telegram_error, level='error')
+                self.printer('buttons_markup:')
+                self.printer(buttons_markup)
+                raise Exception('Raiser') from telegram_error
         return None
+    
+    def send_photo(self, photo, *messages, channel=None):
+        if not channel:
+            channel = self.channel
+        caption = ''
+        for message in messages:
+            caption += message
+            caption += ' '
+        try:
+            self.telegram_bot.send_photo(channel, photo, caption)
+        except Exception as telegram_error:
+            self.printer('Error sending photo to Telegram:', telegram_error, level='error')
+
+    def convert_to_buttons(self, buttons):
+        buttons_list = []
+        if type(buttons) == list:
+            for item in buttons:
+                button = [InlineKeyboardButton(text=item, callback_data=item)]
+                buttons_list.append(button)
+
+        elif type(buttons) == dict:
+            for key in buttons:
+                button = [InlineKeyboardButton(text=key, callback_data=buttons[key])]
+                buttons_list.append(button)
 
-    def convert_dict_to_buttons(self, buttons_dict):
-        buttons = []
-        for key in buttons_dict:
-            button = [InlineKeyboardButton(text=key, callback_data=buttons_dict[key])]
-            buttons.append(button)
-        buttons_markup = InlineKeyboardMarkup(buttons)
+        buttons_markup = InlineKeyboardMarkup(buttons_list)
         return buttons_markup
     
     def printer(self, *items, level='info', current_time=True):
         if self.log:
             if current_time:
                 self.current_time(*items, level=level)
             else:
```

### Comparing `error-alerts-5.1/error_alerts.egg-info/PKG-INFO` & `error-alerts-5.2/error_alerts.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: error-alerts
-Version: 5.1
+Version: 5.2
 Summary: Error alerts via Telegram
 Home-page: https://github.com/xjxckk/error-alerts/
 Download-URL: https://github.com/xjxckk/error-alerts/archive/refs/tags/v2.tar.gz
 Description-Content-Type: text/markdown
 
 ### error-alerts
 Python error alerts via Telegram
```

