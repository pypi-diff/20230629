# Comparing `tmp/tdwnsv3-1.9.2.tar.gz` & `tmp/tdwnsv3-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tdwnsv3-1.9.2.tar", last modified: Tue Jun 27 12:15:56 2023, max compression
+gzip compressed data, was "tdwnsv3-1.9.3.tar", last modified: Thu Jun 29 09:21:11 2023, max compression
```

## Comparing `tdwnsv3-1.9.2.tar` & `tdwnsv3-1.9.3.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-27 12:15:56.127000 tdwnsv3-1.9.2/
--rw-rw----   0 root         (0) everybody  (9997)     1070 2023-02-20 13:15:55.000000 tdwnsv3-1.9.2/LICENSE
--rw-rw----   0 root         (0) everybody  (9997)     8283 2023-06-27 12:15:56.039000 tdwnsv3-1.9.2/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)     7309 2023-06-27 12:14:03.000000 tdwnsv3-1.9.2/README.md
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-06-27 12:15:56.127000 tdwnsv3-1.9.2/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)     1364 2023-06-27 12:11:46.000000 tdwnsv3-1.9.2/setup.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-27 12:15:55.711000 tdwnsv3-1.9.2/tdwnsv3/
--rw-rw----   0 root         (0) everybody  (9997)     1317 2023-06-27 12:11:26.000000 tdwnsv3-1.9.2/tdwnsv3/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)       34 2023-04-18 16:36:08.000000 tdwnsv3-1.9.2/tdwnsv3/__main__.py
--rw-rw----   0 root         (0) everybody  (9997)     2273 2023-02-20 13:15:56.000000 tdwnsv3-1.9.2/tdwnsv3/ciphersuite.py
--rw-rw----   0 root         (0) everybody  (9997)    14899 2023-02-20 13:15:56.000000 tdwnsv3-1.9.2/tdwnsv3/fav.py
--rw-rw----   0 root         (0) everybody  (9997)     9381 2023-06-26 20:14:20.000000 tdwnsv3-1.9.2/tdwnsv3/html_prettier.py
--rw-rw----   0 root         (0) everybody  (9997)     2079 2023-02-21 12:22:35.000000 tdwnsv3-1.9.2/tdwnsv3/javascript.py
--rw-rw----   0 root         (0) everybody  (9997)     2962 2023-02-20 13:15:56.000000 tdwnsv3-1.9.2/tdwnsv3/sec_server.py
--rw-rw----   0 root         (0) everybody  (9997)    13343 2023-06-27 07:33:54.000000 tdwnsv3-1.9.2/tdwnsv3/style.py
--rw-rw----   0 root         (0) everybody  (9997)    20403 2023-06-27 07:38:01.000000 tdwnsv3-1.9.2/tdwnsv3/tdwnsv3.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-27 12:15:56.019000 tdwnsv3-1.9.2/tdwnsv3.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)     8283 2023-06-27 12:15:54.000000 tdwnsv3-1.9.2/tdwnsv3.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      397 2023-06-27 12:15:54.000000 tdwnsv3-1.9.2/tdwnsv3.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-06-27 12:15:54.000000 tdwnsv3-1.9.2/tdwnsv3.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)       49 2023-06-27 12:15:54.000000 tdwnsv3-1.9.2/tdwnsv3.egg-info/entry_points.txt
--rw-rw----   0 root         (0) everybody  (9997)       49 2023-06-27 12:15:54.000000 tdwnsv3-1.9.2/tdwnsv3.egg-info/requires.txt
--rw-rw----   0 root         (0) everybody  (9997)        8 2023-06-27 12:15:54.000000 tdwnsv3-1.9.2/tdwnsv3.egg-info/top_level.txt
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-29 09:21:11.922436 tdwnsv3-1.9.3/
+-rw-rw----   0 root         (0) everybody  (9997)     1070 2023-02-20 13:15:55.000000 tdwnsv3-1.9.3/LICENSE
+-rw-rw----   0 root         (0) everybody  (9997)     8321 2023-06-29 09:21:11.818436 tdwnsv3-1.9.3/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)     7346 2023-06-29 09:20:59.000000 tdwnsv3-1.9.3/README.md
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-06-29 09:21:11.922436 tdwnsv3-1.9.3/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)     1394 2023-06-29 08:38:05.000000 tdwnsv3-1.9.3/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-29 09:21:11.502436 tdwnsv3-1.9.3/tdwnsv3/
+-rw-rw----   0 root         (0) everybody  (9997)     1317 2023-06-29 09:19:30.000000 tdwnsv3-1.9.3/tdwnsv3/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)       34 2023-04-18 16:36:08.000000 tdwnsv3-1.9.3/tdwnsv3/__main__.py
+-rw-rw----   0 root         (0) everybody  (9997)      714 2023-06-29 09:15:24.000000 tdwnsv3-1.9.3/tdwnsv3/admin.py
+-rw-rw----   0 root         (0) everybody  (9997)     2273 2023-02-20 13:15:56.000000 tdwnsv3-1.9.3/tdwnsv3/ciphersuite.py
+-rw-rw----   0 root         (0) everybody  (9997)    14899 2023-02-20 13:15:56.000000 tdwnsv3-1.9.3/tdwnsv3/fav.py
+-rw-rw----   0 root         (0) everybody  (9997)     9490 2023-06-29 09:06:30.000000 tdwnsv3-1.9.3/tdwnsv3/html_prettier.py
+-rw-rw----   0 root         (0) everybody  (9997)     2079 2023-02-21 12:22:35.000000 tdwnsv3-1.9.3/tdwnsv3/javascript.py
+-rw-rw----   0 root         (0) everybody  (9997)     2962 2023-02-20 13:15:56.000000 tdwnsv3-1.9.3/tdwnsv3/sec_server.py
+-rw-rw----   0 root         (0) everybody  (9997)    13459 2023-06-29 09:14:09.000000 tdwnsv3-1.9.3/tdwnsv3/style.py
+-rw-rw----   0 root         (0) everybody  (9997)    21036 2023-06-29 09:15:27.000000 tdwnsv3-1.9.3/tdwnsv3/tdwnsv3.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-29 09:21:11.794436 tdwnsv3-1.9.3/tdwnsv3.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)     8321 2023-06-29 09:21:10.000000 tdwnsv3-1.9.3/tdwnsv3.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      414 2023-06-29 09:21:10.000000 tdwnsv3-1.9.3/tdwnsv3.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-06-29 09:21:10.000000 tdwnsv3-1.9.3/tdwnsv3.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)       49 2023-06-29 09:21:10.000000 tdwnsv3-1.9.3/tdwnsv3.egg-info/entry_points.txt
+-rw-rw----   0 root         (0) everybody  (9997)       68 2023-06-29 09:21:10.000000 tdwnsv3-1.9.3/tdwnsv3.egg-info/requires.txt
+-rw-rw----   0 root         (0) everybody  (9997)        8 2023-06-29 09:21:10.000000 tdwnsv3-1.9.3/tdwnsv3.egg-info/top_level.txt
```

### Comparing `tdwnsv3-1.9.2/LICENSE` & `tdwnsv3-1.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tdwnsv3-1.9.2/PKG-INFO` & `tdwnsv3-1.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdwnsv3
-Version: 1.9.2
+Version: 1.9.3
 Summary: Simple local-files server with security on top!
 Home-page: https://github.com/Simatwa/tdwnsv3
 Author: Smartwa Caleb
 Author-email: smartwacaleb@gmail.com
 Maintainer: Smartwa Caleb
 Maintainer-email: smartwacaleb@gmail.com
 License: MIT
@@ -19,15 +19,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">tdwnsv3</h1>
 
 <p align="center"><a href="https://github.com/Simatwa/tdwnsv3"><img src="https://img.shields.io/static/v1?label=Github&message=Passing&logo=github&color=green" alt="Github"/></a>
 
-<a href="https://pypi.org/project/tdwnsv3"><img src="https://img.shields.io/static/v1?label=Pypi&message=v1.9.2&color=yellow&logo=pypi" alt="pypi"/></a>
+<a href="https://pypi.org/project/tdwnsv3"><img src="https://img.shields.io/static/v1?label=Pypi&message=v1.9.3&color=yellow&logo=pypi" alt="pypi"/></a>
 
 <a href="#"><img src="https://img.shields.io/static/v1?label=Coverage&message=80%&color=lime&logo=Coverage" alt="Coverage"/></a>
 
 <a href="https://wakatime.com/badge/github/Simatwa/svinf3"><img src="https://wakatime.com/badge/github/Simatwa/svinf3.svg" alt="wakatime"/></a>
 
 <a href="https://pepy.tech/project/tdwnsv3"><img src="https://static.pepy.tech/badge/tdwnsv3" alt="Downloads"/></a>
 
@@ -73,14 +73,16 @@
 
 - Compatible with multiple devices and browsers
 
 - Fully customizable web interface - css
 
 - Upload and download files
 
+- Delete multiple files with a click
+
 
 
 ## Installation 
 
 
 
 - Choose your suit from the following ways:
```

### Comparing `tdwnsv3-1.9.2/README.md` & `tdwnsv3-1.9.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <h1 align="center">tdwnsv3</h1>
 <p align="center"><a href="https://github.com/Simatwa/tdwnsv3"><img src="https://img.shields.io/static/v1?label=Github&message=Passing&logo=github&color=green" alt="Github"/></a>
-<a href="https://pypi.org/project/tdwnsv3"><img src="https://img.shields.io/static/v1?label=Pypi&message=v1.9.2&color=yellow&logo=pypi" alt="pypi"/></a>
+<a href="https://pypi.org/project/tdwnsv3"><img src="https://img.shields.io/static/v1?label=Pypi&message=v1.9.3&color=yellow&logo=pypi" alt="pypi"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Coverage&message=80%&color=lime&logo=Coverage" alt="Coverage"/></a>
 <a href="https://wakatime.com/badge/github/Simatwa/svinf3"><img src="https://wakatime.com/badge/github/Simatwa/svinf3.svg" alt="wakatime"/></a>
 <a href="https://pepy.tech/project/tdwnsv3"><img src="https://static.pepy.tech/badge/tdwnsv3" alt="Downloads"/></a>
 <a href="#"><img src="https://visitor-badge.glitch.me/badge?page_id=Simatwa.tdwnsv3&left_color=red&right_color=lime&left_text=Counts" alt="Visitors"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Code Style&message=Black&color=black&logo=Black" alt="Code-style"/></a>
 </p>
 
@@ -23,14 +23,15 @@
 - Simple commandline interface
 - Web interface with multiple themes
 - Serve as static files server - index.html
 - Highly immune against variety of attacks
 - Compatible with multiple devices and browsers
 - Fully customizable web interface - css
 - Upload and download files
+- Delete multiple files with a click
 
 ## Installation 
 
 - Choose your suit from the following ways:
 
 1. From pip
```

### Comparing `tdwnsv3-1.9.2/setup.py` & `tdwnsv3-1.9.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 __info__ = "Simple local-files server with security on top!"
-__version__ = "1.9.2"
+__version__ = "1.9.3"
 __author__ = "Smartwa Caleb"
 __email__ = "smartwacaleb@gmail.com"
 __repo__ = "https://github.com/Simatwa/tdwnsv3"
 
 
 def get_file(nm: str) -> list:
     with open(nm, encoding="utf-8") as fp:
@@ -20,14 +20,15 @@
     project_urls={"Bug Report": f"{__repo__}/issues/new"},
     license="MIT",
     author=__author__,
     install_requires=[
         "Flask>=2.2.2",
         "cryptography>=39.0.0",
         "appdirs>=1.4.4",
+        "Flask-Admin==1.6.1",
     ],
     author_email=__email__,
     maintainer=__author__,
     maintainer_email=__email__,
     description=__info__,
     long_description="\n".join(get_file("README.md")),
     long_description_content_type="text/markdown",
```

### Comparing `tdwnsv3-1.9.2/tdwnsv3/__init__.py` & `tdwnsv3-1.9.3/tdwnsv3/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 __info__ = "Simple local-files server with security on top!"
-__version__ = "1.9.2"
+__version__ = "1.9.3"
 __author__ = "Smartwa Caleb"
 __email__ = "smartwacaleb@gmail.com"
 __repo__ = "https://github.com/Simatwa/tdwnsv3"
 
 __all__ = [
     "tdwnsv3",
     "app",
```

### Comparing `tdwnsv3-1.9.2/tdwnsv3/ciphersuite.py` & `tdwnsv3-1.9.3/tdwnsv3/ciphersuite.py`

 * *Files identical despite different names*

### Comparing `tdwnsv3-1.9.2/tdwnsv3/fav.py` & `tdwnsv3-1.9.3/tdwnsv3/fav.py`

 * *Files identical despite different names*

### Comparing `tdwnsv3-1.9.2/tdwnsv3/html_prettier.py` & `tdwnsv3-1.9.3/tdwnsv3/html_prettier.py`

 * *Files 2% similar despite different names*

```diff
@@ -220,14 +220,15 @@
         <input type='hidden' name='{config['folder_name']}' value='{path}/'>
         <input type='submit' value='Upload'/>
         </form>"""
         if args.upload
         else ""
     )
     r.append(
-        """<hr><div class="container"><footer>
+        f"""<hr><div class="container"><footer>
+        { '<a class="admin_login" href="/admin/fileadmin">Manage Files</a><br><br>' if args.admin else ''} 
 		 <a class='but' href='#' target='self' onclick='refresh()'>Refresh Page</a>
         <p style="color:red;font-size:160%;font-family:cursive;">Regards <a href='https://github.com/Simatwa' target='_blank'>Smartwa</a></p></footer></div>
        """
     )
     r.append("</body></html>")
     return "".join(r)
```

### Comparing `tdwnsv3-1.9.2/tdwnsv3/javascript.py` & `tdwnsv3-1.9.3/tdwnsv3/javascript.py`

 * *Files identical despite different names*

### Comparing `tdwnsv3-1.9.2/tdwnsv3/sec_server.py` & `tdwnsv3-1.9.3/tdwnsv3/sec_server.py`

 * *Files identical despite different names*

### Comparing `tdwnsv3-1.9.2/tdwnsv3/style.py` & `tdwnsv3-1.9.3/tdwnsv3/style.py`

 * *Files 1% similar despite different names*

```diff
@@ -626,14 +626,22 @@
 marquee{
     margin:5px;
     font-family:'Helvetica Neue',Helvetica,Arial,sans-serif;
     font-size:14px;
     color:#222;
 }
 
+.admin_login{
+   margin-down:1px;
+   border-radius:4px;
+   background-color:lime;
+   color:gray;
+   padding:6px;
+}
+
 footer{
   /*  position: fixed; */
     bottom: 0;
     width: 100%;
     background-color: #f2f2f2;
     padding: 10px;
     color: #666;
```

### Comparing `tdwnsv3-1.9.2/tdwnsv3/tdwnsv3.py` & `tdwnsv3-1.9.3/tdwnsv3/tdwnsv3.py`

 * *Files 3% similar despite different names*

```diff
@@ -129,14 +129,29 @@
         "--upload-limit-person",
         help="Maximum files to be uploaded per IP",
         type=int,
         default=10,
         metavar="upload_limit",
     )
     parser.add_argument(
+        "--swatch",
+        help="Flask-Admin display swatch (Theme) name listed at http://bootswatch.com/3/",
+        default="cerulean",
+    )
+    parser.add_argument(
+        "--template",
+        help="Flask-Admin template to be used - %(default)s",
+        default="bootstrap3",
+    )
+    parser.add_argument(
+        "--admin",
+        help="Enable admin view for managing entries - %(default)s",
+        action="store_true",
+    )
+    parser.add_argument(
         "--upload-multiple",
         help="Allow users to upload more than one file at a time.",
         action="store_true",
     )
     parser.add_argument(
         "--disable-aggressive",
         dest="aggressive",
@@ -293,14 +308,15 @@
 app = Flask(
     __name__,
     template_folder=dir,
 )
 
 
 def config_app():
+    app.config["SECRET_KEY"] = new_cookie(14)
     if args.upload_path:
         if os.path.isdir(args.upload_path):
             pth = args.upload_path
             if not pth.startswith("/"):
                 pth = os.path.join(os.getcwd(), pth)
         else:
             pth = os.path.join(os.getcwd(), args.upload_path)
@@ -650,14 +666,19 @@
         ),
         response_data["code"],
     )
 
 
 def main():
     log.debug("Server configured ready to start!")
+    if args.admin:
+        from .admin import AdminEndpoint
+
+        global app
+        app = AdminEndpoint(dir, args, app)
     try:
         if args.host:
             app.run(host="0.0.0.0", port=args.port, debug=args.debug, threaded=True)
         else:
             app.run(port=args.port, debug=args.debug)
     except Exception as e:
         log.exception(e)
```

### Comparing `tdwnsv3-1.9.2/tdwnsv3.egg-info/PKG-INFO` & `tdwnsv3-1.9.3/tdwnsv3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdwnsv3
-Version: 1.9.2
+Version: 1.9.3
 Summary: Simple local-files server with security on top!
 Home-page: https://github.com/Simatwa/tdwnsv3
 Author: Smartwa Caleb
 Author-email: smartwacaleb@gmail.com
 Maintainer: Smartwa Caleb
 Maintainer-email: smartwacaleb@gmail.com
 License: MIT
@@ -19,15 +19,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">tdwnsv3</h1>
 
 <p align="center"><a href="https://github.com/Simatwa/tdwnsv3"><img src="https://img.shields.io/static/v1?label=Github&message=Passing&logo=github&color=green" alt="Github"/></a>
 
-<a href="https://pypi.org/project/tdwnsv3"><img src="https://img.shields.io/static/v1?label=Pypi&message=v1.9.2&color=yellow&logo=pypi" alt="pypi"/></a>
+<a href="https://pypi.org/project/tdwnsv3"><img src="https://img.shields.io/static/v1?label=Pypi&message=v1.9.3&color=yellow&logo=pypi" alt="pypi"/></a>
 
 <a href="#"><img src="https://img.shields.io/static/v1?label=Coverage&message=80%&color=lime&logo=Coverage" alt="Coverage"/></a>
 
 <a href="https://wakatime.com/badge/github/Simatwa/svinf3"><img src="https://wakatime.com/badge/github/Simatwa/svinf3.svg" alt="wakatime"/></a>
 
 <a href="https://pepy.tech/project/tdwnsv3"><img src="https://static.pepy.tech/badge/tdwnsv3" alt="Downloads"/></a>
 
@@ -73,14 +73,16 @@
 
 - Compatible with multiple devices and browsers
 
 - Fully customizable web interface - css
 
 - Upload and download files
 
+- Delete multiple files with a click
+
 
 
 ## Installation 
 
 
 
 - Choose your suit from the following ways:
```

