# Comparing `tmp/pyvista-imgui-0.2.0.tar.gz` & `tmp/pyvista-imgui-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvista-imgui-0.2.0.tar", last modified: Fri Jun  2 19:42:38 2023, max compression
+gzip compressed data, was "pyvista-imgui-0.3.0.tar", last modified: Thu Jun 29 11:52:22 2023, max compression
```

## Comparing `pyvista-imgui-0.2.0.tar` & `pyvista-imgui-0.3.0.tar`

### file list

```diff
@@ -1,28 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:42:38.731080 pyvista-imgui-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:42:38.723080 pyvista-imgui-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:42:38.727080 pyvista-imgui-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-02 19:42:19.000000 pyvista-imgui-0.2.0/.github/workflows/python-package-build-and-publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-02 19:42:19.000000 pyvista-imgui-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-02 19:42:19.000000 pyvista-imgui-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-02 19:42:19.000000 pyvista-imgui-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-06-02 19:42:38.731080 pyvista-imgui-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-02 19:42:19.000000 pyvista-imgui-0.2.0/PyVista.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-06-02 19:42:19.000000 pyvista-imgui-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:42:38.727080 pyvista-imgui-0.2.0/example/
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-02 19:42:19.000000 pyvista-imgui-0.2.0/example/example_embedded.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-02 19:42:19.000000 pyvista-imgui-0.2.0/example/example_standalone.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-02 19:42:19.000000 pyvista-imgui-0.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:42:38.727080 pyvista-imgui-0.2.0/pyvista_imgui/
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-02 19:42:19.000000 pyvista-imgui-0.2.0/pyvista_imgui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-02 19:42:38.000000 pyvista-imgui-0.2.0/pyvista_imgui/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-06-02 19:42:19.000000 pyvista-imgui-0.2.0/pyvista_imgui/imgui_render_window.py
--rw-r--r--   0 runner    (1001) docker     (123)    10132 2023-06-02 19:42:19.000000 pyvista-imgui-0.2.0/pyvista_imgui/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     6354 2023-06-02 19:42:19.000000 pyvista-imgui-0.2.0/pyvista_imgui/texture_render_window.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:42:38.731080 pyvista-imgui-0.2.0/pyvista_imgui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-06-02 19:42:38.000000 pyvista-imgui-0.2.0/pyvista_imgui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-02 19:42:38.000000 pyvista-imgui-0.2.0/pyvista_imgui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 19:42:38.000000 pyvista-imgui-0.2.0/pyvista_imgui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-02 19:42:38.000000 pyvista-imgui-0.2.0/pyvista_imgui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-02 19:42:38.000000 pyvista-imgui-0.2.0/pyvista_imgui.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 19:42:38.731080 pyvista-imgui-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-02 19:42:19.000000 pyvista-imgui-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:52:22.679389 pyvista-imgui-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:52:22.675389 pyvista-imgui-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:52:22.675389 pyvista-imgui-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-29 11:51:58.000000 pyvista-imgui-0.3.0/.github/workflows/python-package-build-and-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-29 11:51:58.000000 pyvista-imgui-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-29 11:51:58.000000 pyvista-imgui-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-29 11:51:58.000000 pyvista-imgui-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-06-29 11:52:22.679389 pyvista-imgui-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-29 11:51:58.000000 pyvista-imgui-0.3.0/PyVista.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-06-29 11:51:58.000000 pyvista-imgui-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:52:22.675389 pyvista-imgui-0.3.0/example/
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-29 11:51:58.000000 pyvista-imgui-0.3.0/example/example_embedded.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-29 11:51:58.000000 pyvista-imgui-0.3.0/example/example_standalone.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-29 11:51:58.000000 pyvista-imgui-0.3.0/example/example_standalone_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-29 11:51:58.000000 pyvista-imgui-0.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:52:22.675389 pyvista-imgui-0.3.0/pyvista_imgui/
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-29 11:51:58.000000 pyvista-imgui-0.3.0/pyvista_imgui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9676 2023-06-29 11:51:58.000000 pyvista-imgui-0.3.0/pyvista_imgui/_backend_imgui_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-06-29 11:51:58.000000 pyvista-imgui-0.3.0/pyvista_imgui/_backend_pyimgui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-29 11:52:22.000000 pyvista-imgui-0.3.0/pyvista_imgui/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-06-29 11:51:58.000000 pyvista-imgui-0.3.0/pyvista_imgui/imgui_render_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6613 2023-06-29 11:51:58.000000 pyvista-imgui-0.3.0/pyvista_imgui/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6354 2023-06-29 11:51:58.000000 pyvista-imgui-0.3.0/pyvista_imgui/texture_render_window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:52:22.679389 pyvista-imgui-0.3.0/pyvista_imgui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-06-29 11:52:22.000000 pyvista-imgui-0.3.0/pyvista_imgui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-29 11:52:22.000000 pyvista-imgui-0.3.0/pyvista_imgui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 11:52:22.000000 pyvista-imgui-0.3.0/pyvista_imgui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-29 11:52:22.000000 pyvista-imgui-0.3.0/pyvista_imgui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-29 11:52:22.000000 pyvista-imgui-0.3.0/pyvista_imgui.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 11:52:22.679389 pyvista-imgui-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-29 11:51:58.000000 pyvista-imgui-0.3.0/setup.py
```

### Comparing `pyvista-imgui-0.2.0/.github/workflows/python-package-build-and-publish.yaml` & `pyvista-imgui-0.3.0/.github/workflows/python-package-build-and-publish.yaml`

 * *Files identical despite different names*

### Comparing `pyvista-imgui-0.2.0/.gitignore` & `pyvista-imgui-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pyvista-imgui-0.2.0/LICENSE` & `pyvista-imgui-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvista-imgui-0.2.0/PKG-INFO` & `pyvista-imgui-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvista-imgui
-Version: 0.2.0
+Version: 0.3.0
 Summary: Pyvista imgui integration
 Author-email: Felix Igelbrink <felix.igelbrink@dfki.de>
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mortacious/pyvista-imgui/issues
 Project-URL: Source Code, https://github.com/mortacious/pyvista-imgui
 Keywords: vtk,imgui,plotting
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyvista-imgui-0.2.0/README.md` & `pyvista-imgui-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pyvista-imgui-0.2.0/example/example_embedded.py` & `pyvista-imgui-0.3.0/example/example_embedded.py`

 * *Files identical despite different names*

### Comparing `pyvista-imgui-0.2.0/pyproject.toml` & `pyvista-imgui-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyvista-imgui-0.2.0/pyvista_imgui/imgui_render_window.py` & `pyvista-imgui-0.3.0/pyvista_imgui/_backend_pyimgui.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,155 +1,52 @@
-from .texture_render_window import VTKOpenGLTextureRenderWindow
-from vtkmodules.vtkRenderingUI import vtkGenericRenderWindowInteractor
+import typing as typ
+from .imgui_render_window import RendererBackend, register_backend
 from vtkmodules.vtkCommonCore import vtkCommand
-import enum
-
-BACKEND_IMGUI_BUNDLE = 0
-BACKEND_PYIMGUI = 1
-
+from vtkmodules.vtkRenderingCore import vtkRenderWindow, vtkRenderWindowInteractor
+import typing as typ
 try:
-    from imgui_bundle import imgui
-    _imgui_backend = BACKEND_IMGUI_BUNDLE
+    import imgui
 except ImportError:
-    # fall back to the pyimgui package
-    try:
-        import imgui
-        _imgui_backend = BACKEND_PYIMGUI
-    except ImportError:
-        raise ImportError("Could not find a supported imgui package.")
-
-
-import typing as typ
+    imgui = None
 
-__all__ = ['VTKImguiRenderWindowInteractor', 'BACKEND_IMGUI_BUNDLE', 'BACKEND_PYIMGUI']
+__all__ = ['RendererBackendPyImgui']
 
-
-class VTKImguiRenderWindowInteractor(object):
-    """
-    A RenderWindowInteractor to integrate VTK's rendering within an existing imgui ui.
-    It uses the VTKOpenGLTextureRenderWindow to render VTK's output into an openGl-texture,
-    which is displayed as an image within imgui.
-
-    All interaction events are passed to the underlying interactor to be handled, so all
-    mouse interactions are the same as in regular VTK.
-
-    Parameters
-    ----------
-    border, optional
-        display a border around the created imgui widget, by default False
-    """
+@register_backend("pyimgui")
+class RendererBackendPyImgui(RendererBackend):
     def __init__(self, 
-                 border: bool = False) -> None:
-        self.imgui_backed = _imgui_backend
-        self.border = border
-        self.renwin = VTKOpenGLTextureRenderWindow(viewport_size=(0, 0))
-
-        self.interactor = vtkGenericRenderWindowInteractor()
-        # do not render unless explicitly requested, as imgui has control over the event loop
-        self.interactor.EnableRenderOff()
-        self.renwin.SetInteractor(self.interactor)
-    
-    def __getattr__(self, attr):
-        """
-        Makes the object behave like a vtkRenderWindowInteractor
-        """
-        if attr == '__vtk__':
-            return lambda t=self.interactor: t
-        elif hasattr(self.interactor, attr):
-            return getattr(self.interactor, attr)
-        else:
-            raise AttributeError(self.__class__.__name__ +
-                  " has no attribute named " + attr)
-        
-    def _render_imgui_bundle(self, size: typ.Optional[tuple[int, int]] = None):
-        if size is None:
-            # get the maximum available size
-            size = imgui.get_content_region_avail()
-            size = (size.x, size.y)
+                 interactor: vtkRenderWindowInteractor, 
+                 render_window: vtkRenderWindow,
+                 border = False) -> None:
+        if not imgui:
+            raise ModuleNotFoundError(f"{self.__class__.__name__} requires the 'pyimgui' package.")
+        super().__init__(interactor, render_window, border=border)
 
-        self.renwin.render(size)
-
-        # adjust the size of this interactor as well
-        self.interactor.SetSize(int(size[0]), int(size[1]))
-        # render the texture with the vtk output into an image
-        imgui.push_style_var(imgui.StyleVar_.window_padding, (0, 0))
-        # make the image unscrollable to ensure correct mouse behavior
-        no_scroll_flags = imgui.WindowFlags_.no_scrollbar | imgui.WindowFlags_.no_scroll_with_mouse
-        imgui.begin_child("##Viewport", size, self.border, no_scroll_flags)
-        imgui.image(self.renwin.texture_id, 
-                    imgui.get_content_region_avail(), 
-                    (0, 1), (1, 0))
-        # process the events of this widget
-        self.process_events()
-        imgui.end_child()
-        imgui.pop_style_var()
-
-    def _render_pyimgui(self, size: typ.Optional[tuple[int, int]] = None):
+    def render(self, size: tuple[int, int] | None = None):
         if size is None:
             # get the maximum available size
             size = imgui.get_content_region_available()
             size = (size.x, size.y)
 
-        self.renwin.render(size)
+        self.render_window.render(size)
 
         # adjust the size of this interactor as well
         self.interactor.SetSize(int(size[0]), int(size[1]))
         imgui.push_style_var(imgui.STYLE_WINDOW_PADDING, (0, 0))
         no_scroll_flags = imgui.WINDOW_NO_SCROLLBAR | imgui.WINDOW_NO_SCROLL_WITH_MOUSE
         imgui.begin_child("##Viewport", size[0], size[1], self.border, no_scroll_flags)
         image_size = imgui.get_content_region_available()
-        imgui.image(self.renwin.texture_id, 
+        imgui.image(self.render_window.texture_id, 
                     image_size.x, image_size.y,
                     (0, 1), (1, 0))
         # process the events of this widget
         self.process_events()
         imgui.end_child()
         imgui.pop_style_var()
 
-
-    def render(self, size: typ.Optional[tuple[int, int]] = None) -> None:
-        """
-        Renders the contents of the internal render window into an existing imgui ui 
-        with the specified size. This method should be called when building 
-        and updating the ui.
-
-        Parameters
-        ----------
-        size, optional
-            the size of the result in the ui in pixels, 
-            if None (default) the maximum available size is used.
-        """
-        if self.imgui_backed == BACKEND_IMGUI_BUNDLE:
-            self._render_imgui_bundle(size)
-        else:
-            self._render_pyimgui(size)
-
-    def _process_events_imgui_bundle(self, io):
-        if imgui.is_window_hovered():
-            if io.mouse_clicked[imgui.MouseButton_.left]:
-                self.interactor.InvokeEvent(vtkCommand.LeftButtonPressEvent)
-            elif io.mouse_clicked[imgui.MouseButton_.right]:
-                self.interactor.InvokeEvent(vtkCommand.RightButtonPressEvent)
-            elif io.mouse_clicked[imgui.MouseButton_.middle]:
-                self.interactor.InvokeEvent(vtkCommand.MiddleButtonPressEvent)
-            elif io.mouse_wheel > 0:
-                self.interactor.InvokeEvent(vtkCommand.MouseWheelForwardEvent)
-            elif io.mouse_wheel < 0:
-                self.interactor.InvokeEvent(vtkCommand.MouseWheelBackwardEvent)
-
-        if io.mouse_released[imgui.MouseButton_.left]:
-            self.interactor.InvokeEvent(vtkCommand.LeftButtonReleaseEvent)
-        elif io.mouse_released[imgui.MouseButton_.right]:
-            self.interactor.InvokeEvent(vtkCommand.RightButtonReleaseEvent)
-        elif io.mouse_released[imgui.MouseButton_.middle]:
-            self.interactor.InvokeEvent(vtkCommand.MiddleButtonReleaseEvent)
-        
-        self.interactor.InvokeEvent(vtkCommand.MouseMoveEvent)
-
-    def _process_events_pyimgui(self, io) -> None:
+    def _process_mouse_events(self, io):
         if imgui.is_window_hovered():
             if imgui.is_mouse_clicked(imgui.MOUSE_BUTTON_LEFT):
                 self.interactor.InvokeEvent(vtkCommand.LeftButtonPressEvent)
             elif imgui.is_mouse_clicked(imgui.MOUSE_BUTTON_RIGHT):
                 self.interactor.InvokeEvent(vtkCommand.RightButtonPressEvent)
             elif imgui.is_mouse_clicked(imgui.MOUSE_BUTTON_MIDDLE):
                 self.interactor.InvokeEvent(vtkCommand.MiddleButtonPressEvent)
@@ -163,15 +60,15 @@
         elif imgui.is_mouse_released(imgui.MOUSE_BUTTON_RIGHT):
             self.interactor.InvokeEvent(vtkCommand.RightButtonReleaseEvent)
         elif imgui.is_mouse_released(imgui.MOUSE_BUTTON_MIDDLE):
             self.interactor.InvokeEvent(vtkCommand.MiddleButtonReleaseEvent)
         
         self.interactor.InvokeEvent(vtkCommand.MouseMoveEvent)
 
-    def process_events(self) -> None:
+    def process_events(self):
         """
         Handle events by passing them to the underlying vtk interactor. This method is called automatically
         on rendering.
         """
         # do nothing as long as the mouse pointer is not within the current window or it is not focussed
         if not imgui.is_window_focused() and not imgui.is_window_hovered():
             return
@@ -180,15 +77,85 @@
         viewport_pos = imgui.get_cursor_start_pos()
 
         xpos = int(io.mouse_pos.x - viewport_pos.x)
         ypos = int(io.mouse_pos.y - viewport_pos.y)
 
         ctrl = io.key_ctrl
         shift = io.key_shift
-        #dclick = io.mouse_double_clicked[0] or io.mouse_double_clicked[1] or io.mouse_double_clicked[2]
         
-        self.interactor.SetEventInformationFlipY(xpos, ypos, ctrl, shift, chr(0), 0, None)
+        repeat = 0
+        #if io.mouse_double_clicked[0] or io.mouse_double_clicked[1] or io.mouse_double_clicked[2]:
+        #    repeat = 1
+
+        if xpos < 0 or ypos < 0:
+            return 
+        
+        self.interactor.SetEventInformationFlipY(xpos, ypos, ctrl, shift, chr(0), repeat, None)
+
+        self._process_mouse_events(io)
+        # no keyboard events yet
+        #self._process_keyboard_events(xpos, ypos, ctrl, shift)
+
+    def show(self,
+             title: typ.Optional[str] = None, 
+             window_size: tuple[int, int] = (1400, 1080)):
+        """
+        Show method for the pyimgui package
 
-        if self.imgui_backed == BACKEND_IMGUI_BUNDLE:
-            self._process_events_imgui_bundle(io)
-        else:
-            self._process_events_pyimgui(io)
+        Parameters
+        ----------
+        title, optional
+            The title of the window, if None, a default title is used.
+        window_size, optional
+            The size of the displayed window, by default (1400, 1080)
+        """
+        import glfw
+        import OpenGL.GL as GL
+        import imgui
+        from imgui.integrations.glfw import GlfwRenderer
+
+        if not glfw.init():
+            raise ValueError("Could not initialize OpenGL context")
+
+        # Create a window and its OpenGL context
+        window = glfw.create_window(int(window_size[0]), int(window_size[1]), title or "ImguiPlotter", None, None)
+        glfw.make_context_current(window)
+
+        if not window:
+            glfw.terminate()
+            raise ValueError("Could not initialize Window")
+        
+        background_color = (0.0, 0.0, 0.0, 1.0)
+        GL.glClearColor(*background_color)
+        imgui.create_context()
+
+        impl = GlfwRenderer(window)
+
+        while not glfw.window_should_close(window):
+            glfw.poll_events()
+            impl.process_inputs()
+            imgui.new_frame()
+            vec = imgui.get_main_viewport().pos
+            imgui.set_next_window_position(vec.x, vec.y, imgui.ONCE)
+            size = imgui.get_main_viewport().size
+            imgui.set_next_window_size(size.x, size.y)
+            imgui.set_next_window_bg_alpha(1.0)
+            window_flags = imgui.WINDOW_NO_BRING_TO_FRONT_ON_FOCUS | \
+                           imgui.WINDOW_NO_TITLE_BAR | \
+                           imgui.WINDOW_NO_DECORATION | \
+                           imgui.WINDOW_NO_RESIZE | \
+                           imgui.WINDOW_NO_MOVE
+                                 
+            imgui.begin("Vtk Viewer", flags=window_flags)
+            self.render()
+            imgui.end()
+
+            imgui.render()
+
+            GL.glClearColor(*background_color)
+            GL.glClear(GL.GL_COLOR_BUFFER_BIT)
+            impl.render(imgui.get_draw_data())
+            glfw.swap_buffers(window)
+
+        impl.shutdown()
+        glfw.terminate()
+
```

### Comparing `pyvista-imgui-0.2.0/pyvista_imgui/texture_render_window.py` & `pyvista-imgui-0.3.0/pyvista_imgui/texture_render_window.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,15 +116,15 @@
         Parameters
         ----------
         new_size
             the new size of the viewport
         """
         # skip if nothing has changed
         if ((self.viewport_size[0] == new_size[0] and self.viewport_size[1] == new_size[1]) or 
-            new_size[0] <= 0 or new_size[0] <= 0) and not self._first_render:
+            new_size[0] <= 0 or new_size[1] <= 0) and not self._first_render:
             return
 
         self.viewport_size = new_size
         # init the internal render window to use the current (texture) context
         self.render_window.InitializeFromCurrentContext() #IMPORTANT: initialize the current opengl context before messing with the textures!
         self.render_window.SetSize(int(self.viewport_size[0]), int(self.viewport_size[1]))
         # create a texture object to render into
```

### Comparing `pyvista-imgui-0.2.0/pyvista_imgui.egg-info/PKG-INFO` & `pyvista-imgui-0.3.0/pyvista_imgui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvista-imgui
-Version: 0.2.0
+Version: 0.3.0
 Summary: Pyvista imgui integration
 Author-email: Felix Igelbrink <felix.igelbrink@dfki.de>
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mortacious/pyvista-imgui/issues
 Project-URL: Source Code, https://github.com/mortacious/pyvista-imgui
 Keywords: vtk,imgui,plotting
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyvista-imgui-0.2.0/pyvista_imgui.egg-info/SOURCES.txt` & `pyvista-imgui-0.3.0/pyvista_imgui.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,18 @@
 PyVista.ini
 README.md
 pyproject.toml
 setup.py
 .github/workflows/python-package-build-and-publish.yaml
 example/example_embedded.py
 example/example_standalone.py
+example/example_standalone_thread.py
 pyvista_imgui/__init__.py
+pyvista_imgui/_backend_imgui_bundle.py
+pyvista_imgui/_backend_pyimgui.py
 pyvista_imgui/_version.py
 pyvista_imgui/imgui_render_window.py
 pyvista_imgui/plotting.py
 pyvista_imgui/texture_render_window.py
 pyvista_imgui.egg-info/PKG-INFO
 pyvista_imgui.egg-info/SOURCES.txt
 pyvista_imgui.egg-info/dependency_links.txt
```

