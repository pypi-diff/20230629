# Comparing `tmp/bring_order-0.3.1.tar.gz` & `tmp/bring_order-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bring_order-0.3.1.tar", max compression
+gzip compressed data, was "bring_order-0.3.2.tar", max compression
```

## Comparing `bring_order-0.3.1.tar` & `bring_order-0.3.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1067 2023-06-26 19:16:39.675135 bring_order-0.3.1/LICENSE
--rw-r--r--   0        0        0     3792 2023-06-26 19:16:39.675135 bring_order-0.3.1/README.md
--rw-r--r--   0        0        0       46 2023-06-26 19:16:39.675135 bring_order-0.3.1/bring_order/__init__.py
--rw-r--r--   0        0        0     7743 2023-06-26 19:16:39.675135 bring_order-0.3.1/bring_order/bodi.py
--rw-r--r--   0        0        0     3266 2023-06-26 19:16:39.675135 bring_order-0.3.1/bring_order/bogui.py
--rw-r--r--   0        0        0     9124 2023-06-26 19:16:39.675135 bring_order-0.3.1/bring_order/boutils.py
--rw-r--r--   0        0        0     2542 2023-06-26 19:16:39.675135 bring_order-0.3.1/bring_order/bringorder.py
--rw-r--r--   0        0        0    14310 2023-06-26 19:16:39.675135 bring_order-0.3.1/bring_order/deductive.py
--rw-r--r--   0        0        0    10071 2023-06-26 19:16:39.675135 bring_order-0.3.1/bring_order/inductive.py
--rw-r--r--   0        0        0        0 2023-06-26 19:16:39.675135 bring_order-0.3.1/bring_order/untitled
--rw-r--r--   0        0        0      568 2023-06-26 19:17:17.511103 bring_order-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     4521 1970-01-01 00:00:00.000000 bring_order-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-29 13:58:00.702863 bring_order-0.3.2/LICENSE
+-rw-r--r--   0        0        0     3792 2023-06-29 13:58:00.702863 bring_order-0.3.2/README.md
+-rw-r--r--   0        0        0       46 2023-06-29 13:58:00.702863 bring_order-0.3.2/bring_order/__init__.py
+-rw-r--r--   0        0        0     8154 2023-06-29 13:58:00.702863 bring_order-0.3.2/bring_order/bodi.py
+-rw-r--r--   0        0        0     3394 2023-06-29 13:58:00.702863 bring_order-0.3.2/bring_order/bogui.py
+-rw-r--r--   0        0        0     9124 2023-06-29 13:58:00.702863 bring_order-0.3.2/bring_order/boutils.py
+-rw-r--r--   0        0        0     2542 2023-06-29 13:58:00.702863 bring_order-0.3.2/bring_order/bringorder.py
+-rw-r--r--   0        0        0    14410 2023-06-29 13:58:00.702863 bring_order-0.3.2/bring_order/deductive.py
+-rw-r--r--   0        0        0    10184 2023-06-29 13:58:00.702863 bring_order-0.3.2/bring_order/inductive.py
+-rw-r--r--   0        0        0        0 2023-06-29 13:58:00.702863 bring_order-0.3.2/bring_order/untitled
+-rw-r--r--   0        0        0      568 2023-06-29 13:58:36.914316 bring_order-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     4521 1970-01-01 00:00:00.000000 bring_order-0.3.2/PKG-INFO
```

### Comparing `bring_order-0.3.1/LICENSE` & `bring_order-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bring_order-0.3.1/README.md` & `bring_order-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `bring_order-0.3.1/bring_order/bodi.py` & `bring_order-0.3.2/bring_order/bodi.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 '''Bring Order Data Import (and preparation). 
 Creates code cells for importing and cleaning data and markdown cell to describe the limitations
 and requirements of data. After code cells displays "ready to analyse" button. After button is 
 pressed displays text field and "ready" button. Empty text field is not accepted.'''
 from ipywidgets import widgets
 from IPython.display import display, clear_output
-from ipywidgets import GridspecLayout
 
 
 class Bodi:
     '''Creates code cells for importing data and markdown cell(s) to describe data limitations'''
     def __init__(self, boutils, bogui, start_analysis):
         """Class constructor
         """
@@ -17,15 +16,15 @@
         self.bogui = bogui
         self.cell_count = 0
         self.buttons = self.bogui.init_buttons(self.button_list)
         self.data_name = self.bogui.create_input_field()
         self.data_description = self.bogui.create_text_area()
         self.add_cells_int = self.bogui.create_int_text()
         self.import_grid = self.data_import_grid()
-        self.data_limitations = []
+        self.data_limitations = [self.bogui.create_input_field('', 'Limitation 1')]
         self.limitation_grid = None
         self.empty_limitations_error = self.bogui.create_error_message()
 
     @property
     def button_list(self):
         """Buttons for Bodi class.
 
@@ -33,15 +32,16 @@
             list of tuples in format (description: str, command: func, style: str) """
         button_list = [
             ('Save description', self.start_data_import, 'success'),
             ('Open cells', self.open_cells, 'warning'),
             ('Delete last cell', self.delete_last_cell, 'danger'),
             ('Run cells', self.run_cells, 'primary'),
             ('Add limitation', self.add_limitation, 'primary'),
-            ('Start analysis', self.start_analysis_clicked, 'success')
+            ('Start analysis', self.start_analysis_clicked, 'success'),
+            ('Remove limitation', self.remove_limitation, 'warning')
         ]
 
         return button_list
 
     def data_import_grid(self):
         """Creates widget grid"""
         cell_number_label = self.bogui.create_label(
@@ -68,53 +68,56 @@
         if self.cell_count > 1:
             self.boutils.delete_cell_above()
             self.cell_count -= 1
 
     def run_cells(self, _=None):
         """Button function that runs data import cells"""
         self.boutils.run_cells_above(self.cell_count)
-
         if self.limitation_grid:
             self.limitation_grid.close()
-
         self.display_limitations()
 
     def add_limitation(self, _=None):
         """Button function to add new limitation"""
         if self.limitation_grid:
             self.limitation_grid.close()
-
-        self.data_limitations.append(self.bogui.create_text_area('',f'Limitation {len(self.data_limitations)+1}'))
-
+        self.data_limitations.append(self.bogui.create_input_field
+                                    ('',f'Limitation {len(self.data_limitations)+1}'))
+        self.empty_limitations_error.value = ''
         self.display_limitations()
 
+    def remove_limitation(self, _=None):
+        """Button function to remove a limitation field"""
+        if len(self.data_limitations) > 1:
+            # implementation
+            self.data_limitations.pop()
+            self.limitation_grid.close()
+            self.empty_limitations_error.value = ''
+            self.display_limitations()
+
     def display_limitations(self):
         """Shows text boxes and buttons for adding limitations"""
         limitations_label = self.bogui.create_message(
                 value='Identify limitations to the data: what kind of questions cannot be answered with it?')
 
-        rows = len(self.data_limitations)
-        if rows == 0:
-            self.data_limitations.append(self.bogui.create_text_area('', 'Limitation 1'))
-            rows +=1
-
-        grid = GridspecLayout(rows, 1)
-
-        for i in range(rows):
-            for j in range(1):
-                grid[i, j] = self.data_limitations[i]
+        limitation_grid = widgets.VBox(self.data_limitations)
 
         self.limitation_grid = widgets.AppLayout(
             header=limitations_label,
-            center=grid,
-            footer=widgets.HBox([
-                self.buttons['Start analysis'],
+            center=limitation_grid,
+            footer=widgets.VBox([
                 self.empty_limitations_error,
-                self.buttons['Add limitation']
-            ])
+                widgets.HBox([
+                    self.buttons['Start analysis'],
+                    self.buttons['Add limitation'],
+                    self.buttons['Remove limitation']
+                ])
+            ]),
+            pane_heights=['30px', 1, '70px'],
+            grid_gap='12px'
         )
 
         display(self.limitation_grid)
 
     def check_limitations(self, item=''):
         """Checks that limitations have been given or commented"""
         if item == '':
@@ -125,20 +128,18 @@
         """Checks that none of the limitations is empty"""
         for limitation in self.data_limitations:
             if not self.check_limitations(limitation.value):
                 return False
         return True
 
     def format_limitations(self):
-        """Formats limitations for markdown to prevent Javascript error
-        
+        """Formats limitations for markdown to prevent Javascript error        
         Returns:
             formatted_limitations (str)
         """
-
         formatted_limitations = '## Limitations\\n'
         for item in self.data_limitations:
             limitation = '<br />'.join(item.value.split('\n'))
             limitation_text = f'- {limitation}\\n'
             formatted_limitations += limitation_text
 
         return formatted_limitations
@@ -157,15 +158,15 @@
         """Formats data description for markdown
         
         Returns:
             formatted_text (str)
         """
         title = f'# Data: {self.data_name.value}'
         description = '<br />'.join(self.data_description.value.split('\n'))
-        formatted_text = f'{title}\\n## Description\\n{description}\\n## Import and cleaning'
+        formatted_text = f'{title}\\n## Description\\n{description}'
 
         return formatted_text
 
     def start_data_import(self, _=None):
         """Creates markdown for data description and shows buttons for data import"""
         if self.data_name.value == '':
             self.bodi(error='You must name the data set')
@@ -202,14 +203,13 @@
             footer=widgets.HBox([
                 self.buttons['Save description'],
                 error_message,
             ]),
             pane_widths=[1, 5, 0],
             grid_gap='10px'
         )
-
         display(grid)
 
         if 'description' in error:
             self.data_description.focus()
         else:
             self.data_name.focus()
```

### Comparing `bring_order-0.3.1/bring_order/bogui.py` & `bring_order-0.3.2/bring_order/bogui.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,24 +40,25 @@
     def create_error_message(self, value=''):
         """Creates HTML, color: red"""
         error = self.create_message(value=value,
                                     style={'font_size': '12px',
                                            'text_color': 'red'})
         return error
 
-    def create_input_field(self, default_value=''):
+    def create_input_field(self, default_value='', placeholder=''):
         """Creates input field"""
-        input_field = widgets.Text(value=default_value)
+        input_field = widgets.Text(value=default_value, placeholder=placeholder)
         return input_field
 
     def create_text_area(self, default_value='', place_holder=''):
         """Creates text box"""
-        text_area = widgets.Textarea(value=default_value,layout={'width': '70%'}, placeholder=place_holder)
+        text_area = widgets.Textarea(value=default_value,layout={'width': '70%'},
+                                     placeholder=place_holder)
         return text_area
-    
+
     def create_label(self, value):
         """Creates label"""
         label = widgets.Label(value=value,
                               layout=widgets.Layout(justify_content='flex-end'))
         return label
 
     def create_placeholder(self):
@@ -87,10 +88,12 @@
 
     def create_radiobuttons(self, options, desc=''):
         """Creates radiobuttons"""
         radiobuttons = widgets.RadioButtons(
             options=options,
             description=desc,
             disabled=False,
-            font_size ="15px")
+            font_size ="15px",
+            layout={'width': 'max-content'}
+        )
 
         return radiobuttons
```

### Comparing `bring_order-0.3.1/bring_order/boutils.py` & `bring_order-0.3.2/bring_order/boutils.py`

 * *Files identical despite different names*

### Comparing `bring_order-0.3.1/bring_order/bringorder.py` & `bring_order-0.3.2/bring_order/bringorder.py`

 * *Files identical despite different names*

### Comparing `bring_order-0.3.1/bring_order/deductive.py` & `bring_order-0.3.2/bring_order/deductive.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,24 +13,24 @@
             start_new (function): Function to start new analysis with same data
         """
         self.cell_count = 0
         self.start_new = start_new
         self.bogui = bogui
         self.boutils = boutils
         self.buttons = self.bogui.init_buttons(self.button_list)
-        self.theory_desc = self.bogui.create_text_area()
+        self.theory_desc = self.bogui.create_text_area('','Theory')
         #List of hypotheses: 0 = hypothesis, 1 = null hypothesis
         self.hypotheses = [
             self.bogui.create_input_field(),
             self.bogui.create_input_field()
         ]
         self.add_cells_int = self.bogui.create_int_text()
         self.conclusion = None
-        self.data_limitations = ['Data limitations missing']
-        self.result_description = self.bogui.create_text_area()
+        self.data_limitations = [self.bogui.create_input_field('Data limitations missing')]
+        self.result_description = self.bogui.create_text_area('','Results')
 
     @property
     def button_list(self):
         """Buttons for deductive class.
 
         Returns:
             list of tuples in format (description: str, command: func, style: str)"""
@@ -148,24 +148,25 @@
         empty_hypo_error = empty_hypo if self.hypotheses[0].value == '' else ''
         empty_null_error = empty_null if self.hypotheses[1].value == '' else ''
 
         return (theory_error, empty_hypo_error, empty_null_error)
 
     def __create_limitation_prompt(self):
         """Creates limitation prompt grid"""
-       
+
         hypothesis_text = self.bogui.create_message(
             f'You have set hypothesis (H1): {self.hypotheses[0].value}'
         )
         null_text = self.bogui.create_message(
             f'You have set null hypothesis (H0): {self.hypotheses[1].value}'
         )
 
         limitations = "<ul>\n"
-        limitations += "\n".join(["<li>" + limitation.value + "</li>" for limitation in self.data_limitations])
+        limitations += "\n".join(["<li>" + limitation.value + "</li>"
+                                 for limitation in self.data_limitations])
         limitations += "\n</ul>"
 
         limitation_prompt_text = widgets.HTML(
             '</br>'+ '<h4> Do the hypotheses fit within the limitations of the data set? </h4>' 
              + limitations)
 
         limitation_prompt = widgets.VBox([
@@ -265,14 +266,15 @@
 
     def __create_conclusion_grid(self):
         question = self.bogui.create_message(value='What happened?')
         conclusion_label = self.bogui.create_message(value='Accepted hypothesis:')
         self.conclusion = self.bogui.create_radiobuttons(
             options=[f'H1: {self.hypotheses[0].value}',
                      f'H0: {self.hypotheses[1].value}'])
+
         notes_label = self.bogui.create_message(value='Describe your results here:')
 
         grid = widgets.AppLayout(
             header=question,
             left_sidebar=conclusion_label,
             center=self.conclusion,
             footer=widgets.VBox([
@@ -280,15 +282,15 @@
                 self.result_description,
                 widgets.HBox([
                     self.buttons['New analysis'],
                     self.buttons['Prepare new data'],
                     self.buttons['All done']
                 ])
             ]),
-            pane_widths=[1, 5, 0],
+            pane_widths=['150px', 1, 0],
             pane_heights=['20px', '40px', 1],
             grid_gap='12px'
         )
 
         return grid
 
     def run_cells(self, _=None):
@@ -308,35 +310,36 @@
         """Clear button function to clear cells above"""
         self.boutils.clear_code_cells_above(self.cell_count)
 
     def __create_cell_operations_grid(self):
         """Creates widget grid"""
         cell_number_label = self.bogui.create_label('Add code cells for your analysis:')
 
-        grid = widgets.GridspecLayout(2, 2, justify_items='center', width='70%', align_items='center')
+        grid = widgets.GridspecLayout(2, 2, justify_items='center',
+                                     width='70%', align_items='center')
         grid[1, 0] = widgets.HBox([cell_number_label, self.add_cells_int])
         grid[1, 1] = widgets.TwoByTwoLayout(
             top_left=self.buttons['Open cells'],
             bottom_left=self.buttons['Run cells'],
             top_right=self.buttons['Delete last cell'],
             bottom_right=self.buttons['Clear cells'])
 
         return grid
 
     def save_results(self):
         """Prints results as markdown and hides widgets"""
-        
+
         text = (f'## Conclusion\\n### Accepted hypothesis: {self.conclusion.value[4:]}\\n'
                 f'The hypotheses were:\\n- Hypothesis (H1): {self.hypotheses[0].value}\\n'
                 f'- Null hypothesis (H0): {self.hypotheses[1].value}\\n')
-        
+
         if self.result_description.value:
             formatted_description = '<br />'.join(self.result_description.value.split('\n'))
             text += f'### Notes\\n {formatted_description}'
-        
+
         self.boutils.create_markdown_cells_above(1, text=text)
         clear_output(wait=True)
 
     def start_new_analysis(self, _=None):
         """Button function to save results and star new analysis"""
         self.save_results()
         self.start_new()
```

### Comparing `bring_order-0.3.1/bring_order/inductive.py` & `bring_order-0.3.2/bring_order/inductive.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 class Inductive:
     """Class that guides inductive analysis"""
     def __init__(self, bogui, boutils, start_new):
         """Class constructor."""
         self.bogui = bogui
         self.utils = boutils
         self.start_new = start_new
-        self.cell_count = 0
+        self._cell_count = 0
         self.buttons = self.bogui.init_buttons(self.button_list)
-        self.add_cells_int = self.bogui.create_int_text()
-        self.notes = self.bogui.create_text_area()
+        self._add_cells_int = self.bogui.create_int_text()
+        self._notes = self.bogui.create_text_area()
         self.conclusion = None
-        self.summary = self.bogui.create_text_area()
+        self.summary = self.bogui.create_text_area('', 'Summary')
         self.empty_notes_error = self.bogui.create_error_message()
         self.observations = []
         self.new_analysis_view = widgets.HBox([
             self.buttons['New analysis'],
             self.buttons['Prepare new data'],
             self.buttons['All done']]
         )
@@ -27,79 +27,79 @@
 
     @property
     def button_list(self):
         """Buttons for Inductive class.
 
         Returns:
             list of tuples in format (description: str, command: func, style: str) """
-        button_list = [('Open cells', self.open_cells, 'warning'),
-                   ('Delete last cell', self.delete_last_cell, 'danger'),
-                   ('Clear cells', self.clear_cells, 'danger'),
-                   ('Run cells', self.run_cells, 'primary'),
-                   ('New analysis', self.start_new_analysis, 'success'),
-                   ('Ready to summarize', self.execute_ready, 'primary'),
-                   ('Submit observation', self.new_observation, 'warning'),
-                   ('Submit summary', self.submit_summary, 'success'),
-                   ('Prepare new data', self.prepare_new_data_pressed, 'success'),
-                   ('All done', self.all_done, 'success'),
-                   ('Export to pdf', self.export_to_pdf, 'success'),
-                   ('Close BringOrder', self.no_export, 'success')]
+        button_list = [('Open cells', self._open_cells, 'warning'),
+                   ('Delete last cell', self._delete_last_cell, 'danger'),
+                   ('Clear cells', self._clear_cells, 'danger'),
+                   ('Run cells', self._run_cells, 'primary'),
+                   ('New analysis', self._start_new_analysis, 'success'),
+                   ('Ready to summarize', self._execute_ready, 'primary'),
+                   ('Submit observation', self._new_observation, 'warning'),
+                   ('Submit summary', self._submit_summary, 'success'),
+                   ('Prepare new data', self._prepare_new_data_pressed, 'success'),
+                   ('All done', self._all_done, 'success'),
+                   ('Export to pdf', self._export_to_pdf, 'success'),
+                   ('Close BringOrder', self._no_export, 'success')]
 
         return button_list
 
-    def open_cells(self, _=None):
+    def _open_cells(self, _=None):
         """Open cells button function that opens the selected
         number of code cells"""
-        if self.add_cells_int.value > 0:
-            self.cell_count += self.add_cells_int.value
-            self.utils.create_code_cells_above(self.add_cells_int.value)
+        if self._add_cells_int.value > 0:
+            self._cell_count += self._add_cells_int.value
+            self.utils.create_code_cells_above(self._add_cells_int.value)
 
-    def delete_last_cell(self, _=None):
+    def _delete_last_cell(self, _=None):
         """Delete last cell-button function"""
-        if self.cell_count > 0:
+        if self._cell_count > 0:
             self.utils.delete_cell_above()
-            self.cell_count -= 1
+            self._cell_count -= 1
 
-    def clear_cells(self, _=None):
+    def _clear_cells(self, _=None):
         """Clears all code cells above."""
-        self.utils.clear_code_cells_above(self.cell_count)
+        self.utils.clear_code_cells_above(self._cell_count)
 
-    def buttons_disabled(self, disabled):
+    def _buttons_disabled(self, disabled):
         """Activates/deactivates buttons
         
         Args:
             disbled (bool): True to disable, False to activate
         """
 
         self.buttons['Open cells'].disabled = disabled
         self.buttons['Clear cells'].disabled = disabled
         self.buttons['Delete last cell'].disabled = disabled
         self.buttons['Ready to summarize'].disabled = disabled
 
-    def run_cells(self, _=None):
+    def _run_cells(self, _=None):
         """Executes cells above and displays text area for observations of analysis."""
-        if self.cell_count == 0:
+        if self._cell_count == 0:
             return
 
-        self.utils.run_cells_above(self.cell_count)
+        self.utils.run_cells_above(self._cell_count)
         if self.conclusion:
             self.conclusion.close()
 
-        self.buttons_disabled(True)
+        self._buttons_disabled(True)
 
         notes_label = self.bogui.create_label(value='Explain what you observed:')
         self.conclusion = widgets.VBox([
-            widgets.HBox([notes_label, self.notes]),
+            widgets.HBox([notes_label, self._notes]),
             self.empty_notes_error,
             self.buttons['Submit observation']
         ])
 
         display(self.conclusion)
 
-    def get_first_words(self, word_list):
+    def _get_first_words(self, word_list):
         """Takes a word list and returns a string that has the first sentence or
         the first five words and three dots if the sentence is longer.
         
         Args:
             word_list (list)
             
         Returns:
@@ -114,67 +114,68 @@
 
         first_words.strip('.').strip(',')
         if len(word_list) > 5:
             first_words += '...'
 
         return first_words
 
-    def format_observation(self):
+    def _format_observation(self):
         """Formats observation for markdown.
         
         Returns:
             formatted_obs (str)
         """
         formatted_obs = f'## Observation {len(self.observations)}: '
 
-        notes_list = self.notes.value.split('\n')
+        notes_list = self._notes.value.split('\n')
         first_line_list = notes_list[0].split(' ')
-        first_words = self.get_first_words(first_line_list)
+        first_words = self._get_first_words(first_line_list)
         formatted_obs += f'{first_words}\\n'
 
         notes = '<br />'.join(notes_list)
         formatted_obs += notes
 
         return formatted_obs
 
-    def new_observation(self, _=None):
+    def _new_observation(self, _=None):
         """Checks new observation, saves it, and resets cell count"""
-        if self.check_notes():
-            self.observations.append(self.notes.value)
-            text = self.format_observation()
+        if self._check_notes():
+            self.observations.append(self._notes.value)
+            text = self._format_observation()
             self.utils.create_markdown_cells_above(1, text=text)
-            self.buttons_disabled(False)
+            self._buttons_disabled(False)
             self.empty_notes_error.value = ''
             self.conclusion.close()
-            self.notes.value = ''
-            self.cell_count = 0
+            self._notes.value = ''
+            self._cell_count = 0
 
         else:
             self.empty_notes_error.value = 'Observation field can not be empty'
 
-    def start_new_analysis(self, _=None):
+    def _start_new_analysis(self, _=None):
         """Starts new bringorder object with old data"""
         clear_output(wait=True)
         self.start_new()
 
-    def prepare_new_data_pressed(self, _=None):
+    def _prepare_new_data_pressed(self, _=None):
         '''Starts new analysis with importing new data'''
         self.utils.execute_cell_from_current(0, 'BringOrder()')
 
-    def execute_ready(self, _=None):
-        """Executes code cells after Get summary button is clicked."""
+    def _execute_ready(self, _=None):
+        """Executes code cells after Ready to summarize button is clicked."""
         clear_output(wait=True)
-        self.display_summary()
+        self._display_summary()
 
-    def display_summary(self, error=''):
+    def _display_summary(self, error=''):
         """Prints all observations and asks for summary"""
         clear_output(wait=True)
 
         observations = "<ul>\n"
-        observations += "\n".join(["<li>" + observation + "</li>" for observation in self.observations])
+        observations += "\n".join(["<li>" + observation + "</li>"
+                                 for observation in self.observations])
         observations += "\n</ul>"
 
         observation_list = widgets.HTML(
             '</br>'+'<h4>All your observations from the data:</h4>'+observations)
 
         # observation_string = '\n'.join((f"Observation {i+1}: {observation}\n") for i, observation
         #          in enumerate(self.observations))
@@ -187,87 +188,87 @@
             observation_list,
             widgets.HBox([summary_label, self.summary]),
             error_message,
             self.buttons['Submit summary']
         ])
         display(grid)
 
-    def format_summary(self):
+    def _format_summary(self):
         """Formats summary for markdown
         
         Returns:
             formatted_summary (str)
         """
         formatted_summary = '## Summary: '
 
         summary_list = self.summary.value.split('\n')
         first_line_list = summary_list[0].split(' ')
-        first_words = self.get_first_words(first_line_list)
+        first_words = self._get_first_words(first_line_list)
         formatted_summary += f'{first_words}\\n'
 
         summary = '<br />'.join(summary_list)
         formatted_summary += summary
 
         return formatted_summary
 
-    def submit_summary(self, _=None):
+    def _submit_summary(self, _=None):
         """Button function to submit summary"""
         if self.summary.value == '':
-            self.display_summary(error='You must write some kind of summary')
+            self._display_summary(error='You must write some kind of summary')
             return
 
-        text = self.format_summary()
+        text = self._format_summary()
         self.utils.create_markdown_cells_above(1, text=text)
         clear_output(wait=False)
         self.new_analysis()
 
-    def check_notes(self):
+    def _check_notes(self):
         """Checks that text field was filled"""
-        if self.notes.value == '':
+        if self._notes.value == '':
             return False
         return True
 
-    def create_cell_operations(self):
+    def _create_cell_operations(self):
         """Displays buttons for operations in inductive analysis"""
         self.buttons['Ready to summarize'].disabled = True
         cell_number_label = self.bogui.create_label('Add code cells for your analysis:')
 
         cell_buttons = widgets.TwoByTwoLayout(
             top_left=self.buttons['Open cells'],
             bottom_left=self.buttons['Run cells'],
             top_right=self.buttons['Delete last cell'],
             bottom_right=self.buttons['Clear cells']
         )
 
         grid = widgets.GridspecLayout(2, 3, height='auto', width='100%')
-        grid[0, 0] = widgets.HBox([cell_number_label, self.add_cells_int])
+        grid[0, 0] = widgets.HBox([cell_number_label, self._add_cells_int])
         grid[:, 1] = cell_buttons
         grid[1, 2] = self.buttons['Ready to summarize']
 
         return grid
 
     def start_inductive_analysis(self):
         """Starts inductive analysis"""
         self.utils.create_markdown_cells_above(1, '# Inductive analysis')
-        display(self.create_cell_operations())
+        display(self._create_cell_operations())
 
-    def all_done(self, _=None):
+    def _all_done(self, _=None):
         """Button function to display the export/close phase."""
         #self.boutils.delete_cell_from_current(1)
         self.new_analysis_view.close()
         display(self.export_view)
 
-    def export_to_pdf(self, _=None):
+    def _export_to_pdf(self, _=None):
         """Button function to export the notebook to pdf."""
         #os.system('jupyter nbconvert Untitled.ipynb --to pdf')
         self.export_view.close()
         display(Javascript('print()'))
         self.utils.delete_cell_from_current(0)
 
-    def no_export(self, _=None):
+    def _no_export(self, _=None):
         """Button function to close widgets without exporting."""
         self.utils.delete_cell_from_current(0)
 
     def new_analysis(self):
         """Display buttons to start a new analysis or prepare new data for analysis"""
         display(self.new_analysis_view)
```

### Comparing `bring_order-0.3.1/pyproject.toml` & `bring_order-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bring-order"
-version = "v0.3.1"
+version = "v0.3.2"
 description = ""
 authors = ["BringOrder team"]
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `bring_order-0.3.1/PKG-INFO` & `bring_order-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bring-order
-Version: 0.3.1
+Version: 0.3.2
 Summary: 
 Author: BringOrder team
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

