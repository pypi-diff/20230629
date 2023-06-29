# Comparing `tmp/arguably-1.2.4.tar.gz` & `tmp/arguably-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arguably-1.2.4.tar", max compression
+gzip compressed data, was "arguably-1.2.5.tar", max compression
```

## Comparing `arguably-1.2.4.tar` & `arguably-1.2.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1538 2023-06-23 09:24:29.956304 arguably-1.2.4/LICENSE.txt
--rw-r--r--   0        0        0     2445 2023-06-23 09:24:29.956304 arguably-1.2.4/arguably/__init__.py
--rw-r--r--   0        0        0     2291 2023-06-23 09:24:29.956304 arguably-1.2.4/arguably/__main__.py
--rw-r--r--   0        0        0    14402 2023-06-23 09:24:29.960305 arguably-1.2.4/arguably/_argparse_extensions.py
--rw-r--r--   0        0        0    16936 2023-06-23 09:24:29.960305 arguably-1.2.4/arguably/_commands.py
--rw-r--r--   0        0        0    40492 2023-06-23 09:24:29.960305 arguably-1.2.4/arguably/_context.py
--rw-r--r--   0        0        0     5815 2023-06-23 09:24:29.960305 arguably-1.2.4/arguably/_modifiers.py
--rw-r--r--   0        0        0    17310 2023-06-23 09:24:29.960305 arguably-1.2.4/arguably/_util.py
--rw-r--r--   0        0        0     6839 2023-06-23 09:24:29.960305 arguably-1.2.4/arguably/arg.py
--rw-r--r--   0        0        0        0 2023-06-23 09:24:29.960305 arguably-1.2.4/arguably/py.typed
--rw-r--r--   0        0        0     7143 2023-06-23 09:24:29.960305 arguably-1.2.4/etc/pypi/PYPI_README.md
--rw-r--r--   0        0        0     1129 2023-06-23 09:24:29.960305 arguably-1.2.4/pyproject.toml
--rw-r--r--   0        0        0     7900 1970-01-01 00:00:00.000000 arguably-1.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1538 2023-06-29 11:09:55.701140 arguably-1.2.5/LICENSE.txt
+-rw-r--r--   0        0        0     2445 2023-06-29 11:09:55.701140 arguably-1.2.5/arguably/__init__.py
+-rw-r--r--   0        0        0     2291 2023-06-29 11:09:55.701140 arguably-1.2.5/arguably/__main__.py
+-rw-r--r--   0        0        0    14402 2023-06-29 11:09:55.701140 arguably-1.2.5/arguably/_argparse_extensions.py
+-rw-r--r--   0        0        0    17738 2023-06-29 11:09:55.701140 arguably-1.2.5/arguably/_commands.py
+-rw-r--r--   0        0        0    41036 2023-06-29 11:09:55.701140 arguably-1.2.5/arguably/_context.py
+-rw-r--r--   0        0        0     5815 2023-06-29 11:09:55.701140 arguably-1.2.5/arguably/_modifiers.py
+-rw-r--r--   0        0        0    18995 2023-06-29 11:09:55.701140 arguably-1.2.5/arguably/_util.py
+-rw-r--r--   0        0        0     6839 2023-06-29 11:09:55.701140 arguably-1.2.5/arguably/arg.py
+-rw-r--r--   0        0        0        0 2023-06-29 11:09:55.701140 arguably-1.2.5/arguably/py.typed
+-rw-r--r--   0        0        0     6941 2023-06-29 11:09:55.705140 arguably-1.2.5/etc/pypi/PYPI_README.md
+-rw-r--r--   0        0        0     1129 2023-06-29 11:09:55.705140 arguably-1.2.5/pyproject.toml
+-rw-r--r--   0        0        0     7698 1970-01-01 00:00:00.000000 arguably-1.2.5/PKG-INFO
```

### Comparing `arguably-1.2.4/LICENSE.txt` & `arguably-1.2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `arguably-1.2.4/arguably/__init__.py` & `arguably-1.2.5/arguably/__init__.py`

 * *Files identical despite different names*

### Comparing `arguably-1.2.4/arguably/__main__.py` & `arguably-1.2.5/arguably/__main__.py`

 * *Files identical despite different names*

### Comparing `arguably-1.2.4/arguably/_argparse_extensions.py` & `arguably-1.2.5/arguably/_argparse_extensions.py`

 * *Files identical despite different names*

### Comparing `arguably-1.2.4/arguably/_commands.py` & `arguably-1.2.5/arguably/_commands.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import asyncio
 import enum
 import inspect
 import re
 from dataclasses import dataclass, field
-from typing import Callable, Any, Union, Optional, List, Dict, Tuple, cast
+from typing import Callable, Any, Union, Optional, List, Dict, Tuple, cast, Set
 
 from docstring_parser import parse as docparse
 
 import arguably._modifiers as mods
 import arguably._util as util
 
 
@@ -88,84 +88,97 @@
             arg_value_type, modifiers = CommandArg.normalize_type(processed_name, param, hints)
             tuple_modifiers = [m for m in modifiers if isinstance(m, mods.TupleModifier)]
             expected_metavars = 1
             if len(tuple_modifiers) > 0:
                 assert len(tuple_modifiers) == 1
                 expected_metavars = len(tuple_modifiers[0].tuple_arg)
 
+            # What kind of argument is this? Is it required-positional, optional-positional, or an option?
+            if param.kind == param.KEYWORD_ONLY:
+                input_method = InputMethod.OPTION
+            elif arg_default is util.NoDefault:
+                input_method = InputMethod.REQUIRED_POSITIONAL
+            else:
+                input_method = InputMethod.OPTIONAL_POSITIONAL
+
             # Get the description
             arg_description = ""
             if docs is not None and docs.params is not None:
                 ds_matches = [ds_p for ds_p in docs.params if ds_p.arg_name.lstrip("*") == param.name]
                 if len(ds_matches) > 1:
                     raise util.ArguablyException(
-                        f"Function parameter `{param.name}` in " f"`{processed_name}` has multiple docstring entries."
+                        f"Function argument `{param.name}` in " f"`{processed_name}` has multiple docstring entries."
                     )
                 if len(ds_matches) == 1:
                     ds_info = ds_matches[0]
                     arg_description = "" if ds_info.description is None else ds_info.description
 
             # Extract the alias
             arg_alias = None
-            if alias_match := re.match(r"^\[-([a-zA-Z0-9])(/--([a-zA-Z0-9]+))?]", arg_description):
-                arg_alias, desc_name = alias_match.group(1), alias_match.group(3)
-                arg_description = arg_description[len(alias_match.group(0)) :].lstrip(" ")
-                if desc_name is not None:
-                    cli_arg_name = desc_name
+            has_long_name = True
+            if input_method == InputMethod.OPTION:
+                arg_description, arg_alias, long_name = util.parse_short_and_long_name(
+                    cli_arg_name, arg_description, func
+                )
+                if long_name is None:
+                    has_long_name = False
+                else:
+                    cli_arg_name = long_name
+            else:
+                if arg_description.startswith("["):
+                    util.warn(
+                        f"Function argument `{param.name}` in `{processed_name}` is a positional argument, but starts "
+                        f"with a `[`, which is used to specify --option names. To make this argument an --option, make "
+                        f"it into be a keyword-only argument.",
+                        func,
+                    )
 
             # Extract the metavars
             metavars = None
             if metavar_split := re.split(r"\{((?:[a-zA-Z0-9_-]+(?:, *)*)+)}", arg_description):
                 if len(metavar_split) == 3:
                     # format would be: ['pre-metavar', 'METAVAR', 'post-metavar']
                     match_items = [i.strip() for i in metavar_split[1].split(",")]
                     if is_variadic:
                         if len(match_items) != 1:
                             raise util.ArguablyException(
-                                f"Function parameter `{param.name}` in `{processed_name}` should only have one item in "
+                                f"Function argument `{param.name}` in `{processed_name}` should only have one item in "
                                 f"its metavar descriptor, but found {len(match_items)}: {','.join(match_items)}."
                             )
                     elif len(match_items) != expected_metavars:
                         if len(match_items) == 1:
                             match_items *= expected_metavars
                         else:
                             raise util.ArguablyException(
-                                f"Function parameter `{param.name}` in `{processed_name}` takes {expected_metavars} "
+                                f"Function argument `{param.name}` in `{processed_name}` takes {expected_metavars} "
                                 f"items, but metavar descriptor has {len(match_items)}: {','.join(match_items)}."
                             )
                     metavars = [i.upper() for i in match_items]
                     arg_description = "".join(metavar_split)  # Strips { and } from metavars for description
                 if len(metavar_split) > 3:
                     raise util.ArguablyException(
-                        f"Function parameter `{param.name}` in `{processed_name}` has multiple metavar sequences - "
+                        f"Function argument `{param.name}` in `{processed_name}` has multiple metavar sequences - "
                         f"these are denoted like {{A, B, C}}. There should be only one."
                     )
 
-            # What kind of argument is this? Is it required-positional, optional-positional, or an option?
-            if param.kind == param.KEYWORD_ONLY:
-                input_method = InputMethod.OPTION
-            elif arg_default is util.NoDefault:
-                input_method = InputMethod.REQUIRED_POSITIONAL
-            else:
-                input_method = InputMethod.OPTIONAL_POSITIONAL
-
             # Check modifiers
             for modifier in modifiers:
                 modifier.check_valid(arg_value_type, param, processed_name)
 
             # Finished processing this arg
             processed_args.append(
                 CommandArg(
                     func_arg_name,
                     cli_arg_name,
                     input_method,
                     is_variadic,
                     arg_value_type,
                     arg_description,
                     arg_alias,
+                    has_long_name,
                     metavars,
                     arg_default,
                     modifiers,
                 )
             )
 
         # Return the processed command
@@ -198,27 +211,32 @@
 
     input_method: InputMethod
     is_variadic: bool
     arg_value_type: type
 
     description: str
     alias: Optional[str] = None
+    has_long_name: bool = True
     metavars: Optional[List[str]] = None
 
     default: Any = util.NoDefault
 
     modifiers: List[mods.CommandArgModifier] = field(default_factory=list)
 
+    def __post_init__(self) -> None:
+        if not self.has_long_name and self.alias is None:
+            raise ValueError("CommandArg has no short or long name")
+
     def get_options(self) -> Union[Tuple[()], Tuple[str], Tuple[str, str]]:
-        if self.input_method is not InputMethod.OPTION:
-            return cast(Tuple[()], tuple())
-        elif self.alias is None:
-            return (f"--{self.cli_arg_name}",)
-        else:
-            return f"-{self.alias}", f"--{self.cli_arg_name}"
+        options = list()
+        if self.alias is not None:
+            options.append(f"-{self.alias}")
+        if self.has_long_name:
+            options.append(f"--{self.cli_arg_name}")
+        return cast(Union[Tuple[()], Tuple[str], Tuple[str, str]], tuple(options))
 
     @staticmethod
     def _normalize_type_union(
         function_name: str,
         param: inspect.Parameter,
         value_type: type,
     ) -> type:
@@ -226,15 +244,15 @@
         We break this out because Python 3.10 seems to want to wrap `Annotated[Optional[...` in another `Optional`, so
         we call this twice.
         """
         if isinstance(value_type, util.UnionType) or util.get_origin(value_type) is Union:
             filtered_types = [x for x in util.get_args(value_type) if x is not type(None)]
             if len(filtered_types) != 1:
                 raise util.ArguablyException(
-                    f"Function parameter `{param.name}` in `{function_name}` is an unsupported type. It must be either "
+                    f"Function argument `{param.name}` in `{function_name}` is an unsupported type. It must be either "
                     f"a single, non-generic type or a Union with None."
                 )
             value_type = filtered_types[0]
         return value_type
 
     @staticmethod
     def normalize_type(
@@ -268,23 +286,21 @@
         # Extra call to normalize a union here, see note in `_normalize_type_union`
         value_type = CommandArg._normalize_type_union(function_name, param, value_type)
 
         # Handle annotated types
         if util.get_origin(value_type) == util.Annotated:
             type_args = util.get_args(value_type)
             if len(type_args) == 0:
-                raise util.ArguablyException(
-                    f"Function parameter `{param.name}` is Annotated, but no type is specified"
-                )
+                raise util.ArguablyException(f"Function argument `{param.name}` is Annotated, but no type is specified")
             else:
                 value_type = type_args[0]
             for type_arg in type_args[1:]:
                 if not isinstance(type_arg, mods.CommandArgModifier):
                     raise util.ArguablyException(
-                        f"Function parameter `{param.name}` has an invalid annotation value: {type_arg}"
+                        f"Function argument `{param.name}` has an invalid annotation value: {type_arg}"
                     )
                 modifiers.append(type_arg)
 
         # Normalize Union with None
         value_type = CommandArg._normalize_type_union(function_name, param, value_type)
 
         # Validate list/tuple and error on other parameterized types
@@ -293,49 +309,49 @@
             isinstance(origin, type) and issubclass(origin, list)
         ):
             type_args = util.get_args(value_type)
             if len(type_args) == 0:
                 value_type = str
             elif len(type_args) > 1:
                 raise util.ArguablyException(
-                    f"Function parameter `{param.name}` in `{function_name}` has too many items passed to List[...]."
+                    f"Function argument `{param.name}` in `{function_name}` has too many items passed to List[...]."
                     f"There should be exactly one item between the square brackets."
                 )
             else:
                 value_type = type_args[0]
             modifiers.append(mods.ListModifier())
         elif (isinstance(value_type, type) and issubclass(value_type, tuple)) or (
             isinstance(origin, type) and issubclass(origin, tuple)
         ):
             if param.kind in [param.VAR_KEYWORD, param.VAR_POSITIONAL]:
                 raise util.ArguablyException(
-                    f"Function parameter `{param.name}` in `{function_name}` is an *args or **kwargs, which should "
+                    f"Function argument `{param.name}` in `{function_name}` is an *args or **kwargs, which should "
                     f"be annotated with what only one of its items should be."
                 )
             type_args = util.get_args(value_type)
             if len(type_args) == 0:
                 raise util.ArguablyException(
-                    f"Function parameter `{param.name}` in `{function_name}` is a tuple but doesn't specify the "
+                    f"Function argument `{param.name}` in `{function_name}` is a tuple but doesn't specify the "
                     f"type of its items, which arguably requires."
                 )
             if type_args[-1] is Ellipsis:
                 raise util.ArguablyException(
-                    f"Function parameter `{param.name}` in `{function_name}` is a variable-length tuple, which is "
+                    f"Function argument `{param.name}` in `{function_name}` is a variable-length tuple, which is "
                     f"not supported."
                 )
             value_type = type(None)
             modifiers.append(mods.TupleModifier(list(type_args)))
         elif origin is not None:
             if param.kind in [param.VAR_KEYWORD, param.VAR_POSITIONAL]:
                 raise util.ArguablyException(
-                    f"Function parameter `{param.name}` in `{function_name}` is an *args or **kwargs, which should "
+                    f"Function argument `{param.name}` in `{function_name}` is an *args or **kwargs, which should "
                     f"be annotated with what only one of its items should be."
                 )
             raise util.ArguablyException(
-                f"Function parameter `{param.name}` in `{function_name}` is a generic type "
+                f"Function argument `{param.name}` in `{function_name}` is a generic type "
                 f"(`{util.get_origin(value_type)}`), which is not supported."
             )
 
         return value_type, modifiers
 
 
 @dataclass
@@ -345,44 +361,46 @@
     function: Callable
     name: str
     args: List[CommandArg]
     description: str = ""
     alias: Optional[str] = None
     add_help: bool = True
 
-    arg_map: Dict[str, CommandArg] = field(init=False)
+    func_arg_names: Set[str] = field(default_factory=set)
+    cli_arg_map: Dict[str, CommandArg] = field(default_factory=dict)
 
     def __post_init__(self) -> None:
-        self.arg_map = dict()
+        self.cli_arg_map = dict()
         for arg in self.args:
-            assert arg.func_arg_name not in self.arg_map
-            if arg.cli_arg_name in self.arg_map:
+            assert arg.func_arg_name not in self.func_arg_names
+            self.func_arg_names.add(arg.func_arg_name)
+
+            if arg.cli_arg_name in self.cli_arg_map:
                 raise util.ArguablyException(
-                    f"Function parameter `{arg.func_arg_name}` in `{self.name}` conflicts with "
-                    f"`{self.arg_map[arg.cli_arg_name].func_arg_name}`, both names simplify to `{arg.cli_arg_name}`"
+                    f"Function argument `{arg.func_arg_name}` in `{self.name}` conflicts with "
+                    f"`{self.cli_arg_map[arg.cli_arg_name].func_arg_name}`, both have the CLI name `{arg.cli_arg_name}`"
                 )
-            self.arg_map[arg.cli_arg_name] = arg
-            self.arg_map[arg.func_arg_name] = arg
+            self.cli_arg_map[arg.cli_arg_name] = arg
 
     def call(self, parsed_args: Dict[str, Any]) -> Any:
         """Filters arguments from argparse to only include the ones used by this command, then calls it"""
 
         args = list()
         kwargs = dict()
 
-        filtered_args = {k: v for k, v in parsed_args.items() if k in self.arg_map}
+        filtered_args = {k: v for k, v in parsed_args.items() if k in self.func_arg_names}
 
         # Add to either args or kwargs
         for arg in self.args:
             if arg.input_method.is_positional and not arg.is_variadic:
-                args.append(filtered_args[arg.cli_arg_name])
+                args.append(filtered_args[arg.func_arg_name])
             elif arg.input_method.is_positional and arg.is_variadic:
-                args.extend(filtered_args[arg.cli_arg_name])
+                args.extend(filtered_args[arg.func_arg_name])
             else:
-                kwargs[arg.func_arg_name] = filtered_args[arg.cli_arg_name]
+                kwargs[arg.func_arg_name] = filtered_args[arg.func_arg_name]
 
         # Call the function
         if util.is_async_callable(self.function):
             util.log_args(
                 util.logger.debug, f"Calling {self.name} function async: ", self.function.__name__, *args, **kwargs
             )
             return asyncio.get_event_loop().run_until_complete(self.function(*args, **kwargs))
```

### Comparing `arguably-1.2.4/arguably/_context.py` & `arguably-1.2.5/arguably/_context.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     normalize_name,
     NoDefault,
     get_type_hints,
     info_for_flags,
     get_ancestors,
     get_parser_name,
     warn,
-    func_info,
+    func_or_class_info,
 )
 
 
 @dataclass
 class _ContextOptions:
     name: Optional[str]
 
@@ -242,15 +242,15 @@
                         f"implementation limitations, all enum.Flag parameters must have a default value."
                     )
 
             # Validate `bool`
             if issubclass(arg_.arg_value_type, bool):
                 if arg_.input_method is not InputMethod.OPTION or arg_.default is NoDefault:
                     raise ArguablyException(
-                        f"Function parameter `{arg_.func_arg_name}` in `{cmd.name}` is a `bool`. Boolean parameters "
+                        f"Function argument `{arg_.func_arg_name}` in `{cmd.name}` is a `bool`. Boolean parameters "
                         f"must have a default value and be an optional, not a positional, argument."
                     )
 
     def _set_up_args(self, cmd: Command) -> None:
         """Adds all arguments to the parser for a given command"""
 
         parser = self._parsers[cmd.name]
@@ -271,15 +271,15 @@
                         nargs=0,
                         help=entry.description,
                     )
                     parser.add_argument(*argspec.args, **argspec.kwargs)
                 continue
 
             # Optional kwargs for parser.add_argument
-            add_arg_kwargs: Dict[str, Any] = dict(type=arg_.arg_value_type)
+            add_arg_kwargs: Dict[str, Any] = dict(type=arg_.arg_value_type, action="store")
 
             arg_description = arg_.description
             description_extras = []
 
             # Show arg type?
             if self._options.show_types:
                 list_modifiers = [m for m in arg_.modifiers if isinstance(m, ListModifier)]
@@ -323,20 +323,20 @@
                     add_arg_kwargs.update(metavar=tuple(arg_.metavars))
 
             # Possible choices `choices`?
             if issubclass(arg_.arg_value_type, enum.Enum):
                 mapping = self.set_up_enum(arg_.arg_value_type)
                 add_arg_kwargs.update(choices=[n for n in mapping])
 
-            cli_arg_names: Tuple[str, ...] = (arg_.cli_arg_name,)
+            name_spec: Tuple[str, ...] = (arg_.func_arg_name,)
 
             # Special handling for optional arguments
             if arg_.input_method is InputMethod.OPTION:
-                cli_arg_names = arg_.get_options()
-                add_arg_kwargs.update(dest=arg_.cli_arg_name)
+                name_spec = arg_.get_options()
+                add_arg_kwargs.update(dest=arg_.func_arg_name)
 
             # `bool` should be flags
             if issubclass(arg_.arg_value_type, bool):
                 # Use `store_true` or `store_false` for bools
                 add_arg_kwargs.update(action="store_true" if arg_.default is False else "store_false")
                 if "type" in add_arg_kwargs:
                     del add_arg_kwargs["type"]
@@ -348,21 +348,31 @@
                 arg_description += f"({', '.join(description_extras)})"
             add_arg_kwargs.update(help=arg_description)
 
             # Run modifiers for this arg
             for modifier in arg_.modifiers:
                 modifier.modify_arg_dict(cmd, arg_, add_arg_kwargs)
 
+            if (
+                "choices" not in add_arg_kwargs
+                and "metavar" not in add_arg_kwargs
+                and add_arg_kwargs["action"] not in ["store_true", "store_false", "count", "help", "version"]
+            ):
+                if arg_.input_method is InputMethod.OPTION:
+                    add_arg_kwargs.update(metavar=arg_.cli_arg_name.upper())
+                else:
+                    add_arg_kwargs.update(metavar=arg_.cli_arg_name)
+
             # Add the argument to the parser
             argspec = log_args(
                 logger.debug,
                 f"Parser({repr(get_parser_name(parser.prog))}).",
                 parser.add_argument.__name__,
                 # Args for the call are below:
-                *cli_arg_names,
+                *name_spec,
                 **add_arg_kwargs,
             )
             parser.add_argument(*argspec.args, **argspec.kwargs)
 
     def _build_subparser_tree(self, command_decorator_info: CommandDecoratorInfo) -> str:
         """Builds up the subparser tree for a given `_CommandDecoratorInfo`. Inserts dummy entries to `self._parsers`
         and `self._commands` if necessary. Returns the name of the parent for this command."""
@@ -457,15 +467,15 @@
         if self._current_parser is None:
             raise ArguablyException("Unknown current parser.")
         self._current_parser.error(message)  # This will exit the script
 
     def _soft_failure(self, msg: str, function: Optional[Callable] = None) -> None:
         if self._options.strict:
             if function is not None:
-                info = func_info(function)
+                info = func_or_class_info(function)
                 if info is not None:
                     source_file, source_file_line = info
                     msg = f"({source_file}:{source_file_line}) {function.__name__}: {msg}"
             raise ArguablyException(msg)
         else:
             warn(msg, function)
 
@@ -834,38 +844,38 @@
 
         @arguably.command
         def some_function(required, not_required=2, *others: int, option: float = 3.14):
             \"\"\"
             this function is on the command line!
 
             Args:
-                required: a required parameter
-                not_required: this one isn't required, since it has a default
+                required: a required argument
+                not_required: this one isn't required, since it has a default value
                 *others: all the other positional arguments go here
-                option: [-x] an option, short name is in brackets
+                option: [-x] keyword-only args are options, short name is in brackets
             \"\"\"
 
         if __name__ == "__main__":
             arguably.run()
         ```
 
         ```console
         user@machine:~$ python3 intro.py -h
         usage: intro.py [-h] [-x OPTION] required [not-required] [others ...]
 
         this function is on the command line!
 
         positional arguments:
-          required             a required parameter (type: str)
-          not-required         this one isn't required, since it has a default (type: int, default: 2)
+          required             a required argument (type: str)
+          not-required         this one isn't required, since it has a default value (type: int, default: 2)
           others               all the other positional arguments go here (type: int)
 
         options:
           -h, --help           show this help message and exit
-          -x, --option OPTION  an option, short name is in brackets (type: float, default: 3.14)
+          -x, --option OPTION  keyword-only args are options, short name is in brackets (type: float, default: 3.14)
         ```
 
         Or, with multiple commands:
 
         ```python
         #!/usr/bin/env python3
         import arguably
```

### Comparing `arguably-1.2.4/arguably/_modifiers.py` & `arguably-1.2.5/arguably/_modifiers.py`

 * *Files identical despite different names*

### Comparing `arguably-1.2.4/arguably/_util.py` & `arguably-1.2.5/arguably/_util.py`

 * *Files 5% similar despite different names*

```diff
@@ -151,15 +151,14 @@
 
 def info_for_flags(cli_arg_name: str, flag_class: Type[enum.Flag]) -> List[EnumFlagInfo]:
     """Generates a list of `_EnumFlagInfo` corresponding to all flags in an `enum.Flag`."""
     result = list()
     docs = docparse(flag_class.__doc__ or "")
     enum_member_docs = get_enum_member_docs(flag_class)
     for item in flag_class:
-        options = [f"--{normalize_name(cast(str, item.name))}"]
         arg_description = ""
 
         # `docstring_parser` does not specially parse out attibutes declared in the docstring - we have to do that
         # ourselves here.
         found = False
         for doc_item in docs.meta:
             assert len(doc_item.args) >= 2
@@ -174,24 +173,51 @@
             break
 
         if not found and item.name in enum_member_docs:
             # noinspection PyTypeChecker
             arg_description = enum_member_docs[item.name]
 
         # Extract the alias from the docstring for the flag item
-        if alias_match := re.match(r"^\[-([a-zA-Z0-9])] ", arg_description):
-            arg_description = arg_description[len(alias_match.group(0)) :]
-            options.insert(0, f"-{alias_match.group(1)}")
+        options = list()
+        long_name: Optional[str] = normalize_name(cast(str, item.name))
+        arg_description, short_name, long_name = parse_short_and_long_name(long_name, arg_description, flag_class)
+        if short_name is not None:
+            options.append(f"-{short_name}")
+        if long_name is not None:
+            options.append(f"--{long_name}")
 
         result.append(
             EnumFlagInfo(cast(Union[Tuple[str], Tuple[str, str]], tuple(options)), cli_arg_name, item, arg_description)
         )
     return result
 
 
+def parse_short_and_long_name(
+    long_name: Optional[str], arg_description: str, func_or_class: Callable
+) -> Tuple[str, Optional[str], Optional[str]]:
+    """Extracts the short and long name for an option"""
+    short_name = None
+    if alias_match := re.match(r"^\[-([a-zA-Z0-9])(/--([a-zA-Z0-9][a-zA-Z0-9\-]*))?]", arg_description):
+        short_name, maybe_long_name = alias_match.group(1), alias_match.group(3)
+        arg_description = arg_description[len(alias_match.group(0)) :].lstrip(" ")
+        if maybe_long_name is not None:
+            long_name = maybe_long_name
+    elif alias_match := re.match(r"^\[--([a-zA-Z0-9][a-zA-Z0-9\-]*)(/-([a-zA-Z0-9]))?]", arg_description):
+        long_name, short_name = alias_match.group(1), alias_match.group(3)
+        arg_description = arg_description[len(alias_match.group(0)) :].lstrip(" ")
+    elif alias_match := re.match(r"^\[-([a-zA-Z0-9])/]", arg_description):
+        short_name = alias_match.group(1)
+        long_name = None
+        arg_description = arg_description[len(alias_match.group(0)) :].lstrip(" ")
+    elif arg_description.startswith("["):
+        # TODO: Should this be an exception?
+        warn(f"Description for {long_name} starts with `[`, but doesn't match any known option formats.", func_or_class)
+    return arg_description, short_name, long_name
+
+
 ########################################################################################################################
 # For __main__
 
 
 class RedirectedIO(StringIO):
     def __init__(self, pipe: Any) -> None:
         super().__init__()
@@ -275,34 +301,34 @@
         full_arg_string = f"{args_str}{kwargs_str}"
     else:
         full_arg_string = f"{args_str}, {kwargs_str}"
     logger_fn(f"{msg}{fn_name}({full_arg_string})")
     return ArgSpec(args, kwargs)
 
 
-def func_info(function: Callable) -> Optional[Tuple[str, int]]:
-    source_file = inspect.getsourcefile(function)
+def func_or_class_info(func_or_class: Callable) -> Optional[Tuple[str, int]]:
+    source_file = inspect.getsourcefile(func_or_class)
     if source_file is None:
         return None
 
     # Skip lines before the `def`. Should be cleaned up in the future.
-    source_lines, line_number = inspect.getsourcelines(function)
+    source_lines, line_number = inspect.getsourcelines(func_or_class)
     for line in source_lines:
-        if "def " not in line:
-            line_number += 1
-        break
+        if "def " in line or "class " in line:
+            break
+        line_number += 1
 
     return source_file, line_number
 
 
-def warn(message: str, function: Optional[Callable] = None) -> None:
+def warn(message: str, func_or_class: Optional[Callable] = None) -> None:
     """Provide a warning. We avoid using logging, since we're just a library, so we issue through `warnings`."""
 
-    if function is not None:
-        info = func_info(function)
+    if func_or_class is not None:
+        info = func_or_class_info(func_or_class)
         if info is not None:
             source_file, source_file_line = info
             warnings.warn_explicit(
                 message,
                 ArguablyWarning,
                 source_file,
                 source_file_line,
@@ -458,40 +484,43 @@
                   ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
           File ".../arguably/arguably/_context.py", line 284, in _process_decorator_info
             return Command(
                    ^^^^^^^^
           File "<string>", line 9, in __init__
           File ".../arguably/arguably/_commands.py", line 214, in __post_init__
             raise util.ArguablyException(
-        arguably._util.ArguablyException: Function parameter `_collision` in `example` conflicts with `collision_`, both
+        arguably._util.ArguablyException: Function argument `_collision` in `example` conflicts with `collision_`, both
         names simplify to `collision`
         ```
     """
 
 
 class ArguablyWarning(UserWarning):
     """
-    Emitted when a decorated function is incorrectly set up in some way, but arguably can continue. Will *not* be raised
-    when a user provides incorrect input to the CLI.
+    If strict checks are disabled through `arguably.run(strict=False)` this is emitted when a decorated function is
+    incorrectly set up in some way, but arguably can continue. Will *not* be raised when a user provides incorrect input
+    to the CLI.
+
+    When `arguably` is directly invoked through `python3 -m arguably ...`, `strict=False` is always set.
 
     Note that this is a warning - it is used with `warnings.warn`.
 
     Examples:
         ```python
         def example_failed(collision_, _collision):
             print("You should never see this")
 
         def example_ok():
             print("All good")
         ```
 
         ```console
-        user@machine:~$ python3 -m arguably-warn.py -h
+        user@machine:~$ python3 -m arguably arguably-warn.py -h
         .../arguably/etc/scripts/api-examples/arguably-warn.py:1: ArguablyWarning: Unable to add function
-        example_failed: Function parameter `_collision` in `example-failed` conflicts with `collision_`, both names
+        example_failed: Function argument `_collision` in `example-failed` conflicts with `collision_`, both names
         simplify to `collision`
           def example_failed(collision_, _collision):
         usage: arguably-warn [-h] command ...
 
         positional arguments:
           command
             example-ok
```

### Comparing `arguably-1.2.4/arguably/arg.py` & `arguably-1.2.5/arguably/arg.py`

 * *Files identical despite different names*

### Comparing `arguably-1.2.4/etc/pypi/PYPI_README.md` & `arguably-1.2.5/etc/pypi/PYPI_README.md`

 * *Files 9% similar despite different names*

```diff
@@ -12,16 +12,16 @@
     <a href="https://github.com/treykeown/arguably/actions/workflows/python-package.yml"><img src="https://github.com/treykeown/arguably/actions/workflows/python-package.yml/badge.svg" alt="Test status"></a>
     <a href="https://treykeown.github.io/arguably/coverage/"><img src="https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/treykeown/f493b14288af4e8358ea8578c393213a/raw/arguably-coverage-badge.json" alt="Code coverage"></a>
     <a href="https://pypi.org/project/arguably/"><img src="https://shields.io/pypi/pyversions/arguably" alt="Supported Python versions"></a>
     <a href="https://pypi.org/project/arguably/"><img src="https://shields.io/pypi/v/arguably" alt="PyPI version"></a>
 </p>
 <hr>
 
-`arguably` turns functions into command line interfaces (CLIs). `arguably` has a tiny API and is extremely easy to
-integrate. You can also use it directly through `python3 -m arguably your_script.py`, more on that
+`arguably` turns functions and docstrings into command line interfaces (CLIs). `arguably` has a tiny API and is
+extremely easy to integrate. You can also use it directly through `python3 -m arguably your_script.py`, more on that
 [here](#no-integration-required).
 
 To use `arguably` in a script, decorate any functions that should appear on the command line with `@arguably.command`,
 then call `arguably.run()`. If multiple functions are decorated, they'll all appear as subcommands. You can even have
 *multiple levels* of subcommands: `def s3__ls()` becomes `s3 ls`.
 
 <div align="right"><sub>
@@ -34,50 +34,55 @@
 
 @arguably.command
 def some_function(required, not_required=2, *others: int, option: float = 3.14):
     """
     this function is on the command line!
 
     Args:
-        required: a required parameter
-        not_required: this one isn't required, since it has a default
+        required: a required argument
+        not_required: this one isn't required, since it has a default value
         *others: all the other positional arguments go here
-        option: [-x] an option, short name is in brackets
+        option: [-x] keyword-only args are options, short name is in brackets
     """
+    print(f"{required=}, {not_required=}, {others=}, {option=}")
 
 if __name__ == "__main__":
     arguably.run()
 ```
 
 <p align="center"><b><em>becomes</em></b></p>
 
 ```console
 user@machine:~$ ./intro.py -h
 usage: intro.py [-h] [-x OPTION] required [not-required] [others ...]
 
 this function is on the command line!
 
 positional arguments:
-  required             a required parameter (type: str)
-  not-required         this one isn't required, since it has a default (type: int, default: 2)
+  required             a required argument (type: str)
+  not-required         this one isn't required, since it has a default value (type: int, default: 2)
   others               all the other positional arguments go here (type: int)
 
 options:
   -h, --help           show this help message and exit
-  -x, --option OPTION  an option, short name is in brackets (type: float, default: 3.14)
+  -x, --option OPTION  keyword-only args are options, short name is in brackets (type: float, default: 3.14)
 ```
 
-`arguably` looks at any decorated functions and maps their arguments from Python to the CLI:
+Arguments to the CLI look just like calling the Python function.
 
-| This Python ...                                | ... becomes this on the CLI.                   |
-|------------------------------------------------|------------------------------------------------|
-| positional args, no default `required`         | positional CLI args, required `required`       |
-| positional args, with default `not_required=2` | positional CLI args, optional `[not-required]` |
-| positional args, variadic `*others`            | any extra positional CLI args `[others ...]`   |
-| keyword-only arguments `option`                | command-line options `[-x OPTION]`             |
+```pycon
+>>> from intro import some_function
+>>> some_function("asdf", 0, 7, 8, 9, option=2.71)
+required='asdf', not_required=0, others=(7, 8, 9), option=2.71
+```
+
+```console
+user@machine:~$ ./intro.py asdf 0 7 8 9 --option 2.71
+required='asdf', not_required=0, others=(7, 8, 9), option=2.71
+```
 
 `arguably` uses your docstrings to automatically generate help messages. It supports all major formats for docstrings:
 reStructuredText, Google, Numpydoc, and Epydoc.
 
 Type annotations are optional, but `arguably` can use them to automatically convert arguments. It has smart handling for
 mapping built-in types to the command line, including `tuple`, `list`, `enum.Enum`, and `enum.Flag`.
```

### Comparing `arguably-1.2.4/pyproject.toml` & `arguably-1.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "arguably"
-version = "1.2.4"
+version = "1.2.5"
 description = "The best Python CLI library, arguably."
 authors = ["treykeown <2755914+treykeown@users.noreply.github.com>"]
 readme = "etc/pypi/PYPI_README.md"
 homepage = "https://treykeown.github.io/arguably/"
 repository = "https://github.com/treykeown/arguably"
 
 [tool.poetry.dependencies]
```

### Comparing `arguably-1.2.4/PKG-INFO` & `arguably-1.2.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arguably
-Version: 1.2.4
+Version: 1.2.5
 Summary: The best Python CLI library, arguably.
 Home-page: https://treykeown.github.io/arguably/
 Author: treykeown
 Author-email: 2755914+treykeown@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -30,16 +30,16 @@
     <a href="https://github.com/treykeown/arguably/actions/workflows/python-package.yml"><img src="https://github.com/treykeown/arguably/actions/workflows/python-package.yml/badge.svg" alt="Test status"></a>
     <a href="https://treykeown.github.io/arguably/coverage/"><img src="https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/treykeown/f493b14288af4e8358ea8578c393213a/raw/arguably-coverage-badge.json" alt="Code coverage"></a>
     <a href="https://pypi.org/project/arguably/"><img src="https://shields.io/pypi/pyversions/arguably" alt="Supported Python versions"></a>
     <a href="https://pypi.org/project/arguably/"><img src="https://shields.io/pypi/v/arguably" alt="PyPI version"></a>
 </p>
 <hr>
 
-`arguably` turns functions into command line interfaces (CLIs). `arguably` has a tiny API and is extremely easy to
-integrate. You can also use it directly through `python3 -m arguably your_script.py`, more on that
+`arguably` turns functions and docstrings into command line interfaces (CLIs). `arguably` has a tiny API and is
+extremely easy to integrate. You can also use it directly through `python3 -m arguably your_script.py`, more on that
 [here](#no-integration-required).
 
 To use `arguably` in a script, decorate any functions that should appear on the command line with `@arguably.command`,
 then call `arguably.run()`. If multiple functions are decorated, they'll all appear as subcommands. You can even have
 *multiple levels* of subcommands: `def s3__ls()` becomes `s3 ls`.
 
 <div align="right"><sub>
@@ -52,50 +52,55 @@
 
 @arguably.command
 def some_function(required, not_required=2, *others: int, option: float = 3.14):
     """
     this function is on the command line!
 
     Args:
-        required: a required parameter
-        not_required: this one isn't required, since it has a default
+        required: a required argument
+        not_required: this one isn't required, since it has a default value
         *others: all the other positional arguments go here
-        option: [-x] an option, short name is in brackets
+        option: [-x] keyword-only args are options, short name is in brackets
     """
+    print(f"{required=}, {not_required=}, {others=}, {option=}")
 
 if __name__ == "__main__":
     arguably.run()
 ```
 
 <p align="center"><b><em>becomes</em></b></p>
 
 ```console
 user@machine:~$ ./intro.py -h
 usage: intro.py [-h] [-x OPTION] required [not-required] [others ...]
 
 this function is on the command line!
 
 positional arguments:
-  required             a required parameter (type: str)
-  not-required         this one isn't required, since it has a default (type: int, default: 2)
+  required             a required argument (type: str)
+  not-required         this one isn't required, since it has a default value (type: int, default: 2)
   others               all the other positional arguments go here (type: int)
 
 options:
   -h, --help           show this help message and exit
-  -x, --option OPTION  an option, short name is in brackets (type: float, default: 3.14)
+  -x, --option OPTION  keyword-only args are options, short name is in brackets (type: float, default: 3.14)
 ```
 
-`arguably` looks at any decorated functions and maps their arguments from Python to the CLI:
+Arguments to the CLI look just like calling the Python function.
 
-| This Python ...                                | ... becomes this on the CLI.                   |
-|------------------------------------------------|------------------------------------------------|
-| positional args, no default `required`         | positional CLI args, required `required`       |
-| positional args, with default `not_required=2` | positional CLI args, optional `[not-required]` |
-| positional args, variadic `*others`            | any extra positional CLI args `[others ...]`   |
-| keyword-only arguments `option`                | command-line options `[-x OPTION]`             |
+```pycon
+>>> from intro import some_function
+>>> some_function("asdf", 0, 7, 8, 9, option=2.71)
+required='asdf', not_required=0, others=(7, 8, 9), option=2.71
+```
+
+```console
+user@machine:~$ ./intro.py asdf 0 7 8 9 --option 2.71
+required='asdf', not_required=0, others=(7, 8, 9), option=2.71
+```
 
 `arguably` uses your docstrings to automatically generate help messages. It supports all major formats for docstrings:
 reStructuredText, Google, Numpydoc, and Epydoc.
 
 Type annotations are optional, but `arguably` can use them to automatically convert arguments. It has smart handling for
 mapping built-in types to the command line, including `tuple`, `list`, `enum.Enum`, and `enum.Flag`.
```

