# Comparing `tmp/consolekit-1.4.1.tar.gz` & `tmp/consolekit-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "consolekit-1.4.1.tar", last modified: Thu May 19 13:45:02 2022, max compression
+gzip compressed data, was "consolekit-1.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `consolekit-1.4.1.tar` & `consolekit-1.5.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1064 2022-05-19 13:44:31.646916 consolekit-1.4.1/LICENSE
--rw-r--r--   0        0        0     5469 2022-05-19 13:44:31.646916 consolekit-1.4.1/README.rst
--rw-r--r--   0        0        0     4814 2022-05-19 13:44:31.646916 consolekit-1.4.1/consolekit/__init__.py
--rw-r--r--   0        0        0     1362 2022-05-19 13:44:31.646916 consolekit-1.4.1/consolekit/__init__.pyi
--rw-r--r--   0        0        0     1507 2022-05-19 13:44:31.646916 consolekit-1.4.1/consolekit/_types.py
--rw-r--r--   0        0        0    13480 2022-05-19 13:44:31.646916 consolekit-1.4.1/consolekit/commands.py
--rw-r--r--   0        0        0    11573 2022-05-19 13:44:31.646916 consolekit-1.4.1/consolekit/input.py
--rw-r--r--   0        0        0    15406 2022-05-19 13:44:31.646916 consolekit-1.4.1/consolekit/options.py
--rw-r--r--   0        0        0        0 2022-05-19 13:44:31.646916 consolekit-1.4.1/consolekit/py.typed
--rw-r--r--   0        0        0    16647 2022-05-19 13:44:31.646916 consolekit-1.4.1/consolekit/terminal_colours.py
--rw-r--r--   0        0        0     6068 2022-05-19 13:44:31.646916 consolekit-1.4.1/consolekit/terminal_colours.pyi
--rw-r--r--   0        0        0     8746 2022-05-19 13:44:31.646916 consolekit-1.4.1/consolekit/testing.py
--rw-r--r--   0        0        0     6824 2022-05-19 13:44:31.646916 consolekit-1.4.1/consolekit/tracebacks.py
--rw-r--r--   0        0        0    13768 2022-05-19 13:44:31.646916 consolekit-1.4.1/consolekit/utils.py
--rw-r--r--   0        0        0     5168 2022-05-19 13:44:31.650916 consolekit-1.4.1/pyproject.toml
--rw-r--r--   0        0        0     7598 1970-01-01 00:00:00.000000 consolekit-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-29 15:57:01.811913 consolekit-1.5.0/LICENSE
+-rw-r--r--   0        0        0     5471 2023-06-29 15:57:01.811913 consolekit-1.5.0/README.rst
+-rw-r--r--   0        0        0     4832 2023-06-29 15:57:01.811913 consolekit-1.5.0/consolekit/__init__.py
+-rw-r--r--   0        0        0     1488 2023-06-29 15:57:01.811913 consolekit-1.5.0/consolekit/__init__.pyi
+-rw-r--r--   0        0        0     1507 2023-06-29 15:57:01.811913 consolekit-1.5.0/consolekit/_types.py
+-rw-r--r--   0        0        0    13518 2023-06-29 15:57:01.811913 consolekit-1.5.0/consolekit/commands.py
+-rw-r--r--   0        0        0    11911 2023-06-29 15:57:01.811913 consolekit-1.5.0/consolekit/input.py
+-rw-r--r--   0        0        0    15750 2023-06-29 15:57:01.811913 consolekit-1.5.0/consolekit/options.py
+-rw-r--r--   0        0        0        0 2023-06-29 15:57:01.811913 consolekit-1.5.0/consolekit/py.typed
+-rw-r--r--   0        0        0    16739 2023-06-29 15:57:01.811913 consolekit-1.5.0/consolekit/terminal_colours.py
+-rw-r--r--   0        0        0     6084 2023-06-29 15:57:01.811913 consolekit-1.5.0/consolekit/terminal_colours.pyi
+-rw-r--r--   0        0        0     8778 2023-06-29 15:57:01.811913 consolekit-1.5.0/consolekit/testing.py
+-rw-r--r--   0        0        0     6801 2023-06-29 15:57:01.811913 consolekit-1.5.0/consolekit/tracebacks.py
+-rw-r--r--   0        0        0    13859 2023-06-29 15:57:01.811913 consolekit-1.5.0/consolekit/utils.py
+-rw-r--r--   0        0        0     5222 2023-06-29 15:57:01.815913 consolekit-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     7651 1970-01-01 00:00:00.000000 consolekit-1.5.0/PKG-INFO
```

### Comparing `consolekit-1.4.1/LICENSE` & `consolekit-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `consolekit-1.4.1/README.rst` & `consolekit-1.5.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -53,16 +53,16 @@
 	:target: https://github.com/domdfcoding/consolekit/actions?query=workflow%3A%22Flake8%22
 	:alt: Flake8 Status
 
 .. |actions_mypy| image:: https://github.com/domdfcoding/consolekit/workflows/mypy/badge.svg
 	:target: https://github.com/domdfcoding/consolekit/actions?query=workflow%3A%22mypy%22
 	:alt: mypy status
 
-.. |requires| image:: https://dependency-dash.herokuapp.com/github/domdfcoding/consolekit/badge.svg
-	:target: https://dependency-dash.herokuapp.com/github/domdfcoding/consolekit/
+.. |requires| image:: https://dependency-dash.repo-helper.uk/github/domdfcoding/consolekit/badge.svg
+	:target: https://dependency-dash.repo-helper.uk/github/domdfcoding/consolekit/
 	:alt: Requirements Status
 
 .. |coveralls| image:: https://img.shields.io/coveralls/github/domdfcoding/consolekit/master?logo=coveralls
 	:target: https://coveralls.io/github/domdfcoding/consolekit?branch=master
 	:alt: Coverage
 
 .. |codefactor| image:: https://img.shields.io/codefactor/grade/github/domdfcoding/consolekit?logo=codefactor
@@ -96,23 +96,23 @@
 .. |license| image:: https://img.shields.io/github/license/domdfcoding/consolekit
 	:target: https://github.com/domdfcoding/consolekit/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/consolekit
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/consolekit/v1.4.1
+.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/consolekit/v1.5.0
 	:target: https://github.com/domdfcoding/consolekit/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/consolekit
 	:target: https://github.com/domdfcoding/consolekit/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2022
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/consolekit
 	:target: https://pypi.org/project/consolekit/
 	:alt: PyPI - Downloads
 
 .. end shields
```

### Comparing `consolekit-1.4.1/consolekit/__init__.py` & `consolekit-1.5.0/consolekit/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,49 +34,53 @@
 #  MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
 #  IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
 #  DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
 #  OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
 #  OR OTHER DEALINGS IN THE SOFTWARE.
 #
 
+# pylint: disable=redefined-builtin
+
 # stdlib
 import sys
 from typing import Any, Callable, Dict, Optional, Type, TypeVar, cast
 
 # 3rd party
 import click
 
 # this package
-from consolekit import commands, input, terminal_colours, tracebacks, utils  # pylint: disable=redefined-builtin
+from consolekit import commands, input, terminal_colours, tracebacks, utils  # noqa: F401
 from consolekit.commands import SuggestionGroup
 from consolekit.options import _Option
 
+# pylint: enable=redefined-builtin
+
 __author__: str = "Dominic Davis-Foster"
 __copyright__: str = "2020 Dominic Davis-Foster"
 __license__: str = "MIT License"
-__version__: str = "1.4.1"
+__version__: str = "1.5.0"
 __email__: str = "dominic@davis-foster.co.uk"
 
 if not bool(getattr(sys, "ps1", sys.flags.interactive)):  # pragma: no cover
 	try:
 		# stdlib
 		import readline
 		readline.set_history_length(0)
 		readline.set_auto_history(False)
 	except (ImportError, AttributeError):
 		# Attribute error on PyPy, ImportError on Windows etc.
 		pass
 
-__all__ = [
+__all__ = (
 		"CONTEXT_SETTINGS",
 		"click_command",
 		"click_group",
 		"option",
 		"SuggestionGroup",
-		]
+		)
 
 _C = TypeVar("_C", bound=click.Command)
 _G = TypeVar("_G", bound=click.Group)
 
 CONTEXT_SETTINGS: Dict[str, Any] = dict(help_option_names=["-h", "--help"], max_content_width=120)
 
 
@@ -117,18 +121,18 @@
 
 	:rtype:
 
 	.. latex:clearpage::
 	"""
 
 	if cls is None:
-		cls = SuggestionGroup  # type: ignore
+		cls = SuggestionGroup
 
 	attrs.setdefault("context_settings", CONTEXT_SETTINGS)
-	return click_command(name, cls=cls, **attrs)  # type: ignore
+	return click_command(name, cls=cls, **attrs)
 
 
 def option(
 		*param_decls: str,
 		**attrs: Any,
 		) -> Callable[[_C], _C]:
 	r"""
```

### Comparing `consolekit-1.4.1/consolekit/__init__.pyi` & `consolekit-1.5.0/consolekit/__init__.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,23 @@
+# pylint: disable=redefined-builtin
+
 # stdlib
 from typing import Any, Callable, Dict, List, Optional, Type, TypeVar, overload
 
 # 3rd party
 import click
 
 # this package
-from consolekit import commands as commands
-from consolekit import input as input  # noqa: A001  # pylint: disable=redefined-builtin
-from consolekit import terminal_colours as terminal_colours
-from consolekit import tracebacks as tracebacks
-from consolekit import utils as utils
-from consolekit.commands import SuggestionGroup as SuggestionGroup
-from consolekit.options import _Option
+from consolekit import commands as commands  # noqa: F401
+from consolekit import input as input  # noqa: A001,F401  # pylint: disable=redefined-builtin
+from consolekit import terminal_colours as terminal_colours  # noqa: F401
+from consolekit import tracebacks as tracebacks  # noqa: F401
+from consolekit import utils as utils  # noqa: F401
+from consolekit.commands import SuggestionGroup as SuggestionGroup  # noqa: F401
+from consolekit.options import _Option  # noqa: F401
 
 __author__: str
 __copyright__: str
 __license__: str
 __version__: str
 __email__: str
 __all__: List[str]
```

### Comparing `consolekit-1.4.1/consolekit/_types.py` & `consolekit-1.5.0/consolekit/_types.py`

 * *Files identical despite different names*

### Comparing `consolekit-1.4.1/consolekit/commands.py` & `consolekit-1.5.0/consolekit/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,30 +64,30 @@
 # 3rd party
 import click
 from click.core import iter_params_for_processing
 from click.parser import split_opt
 from click.utils import make_str
 from domdf_python_tools.stringlist import DelimitedList
 from domdf_python_tools.words import Plural
-from mistletoe import block_token  # type: ignore
+from mistletoe import block_token  # type: ignore[import]
 
 # this package
 from consolekit.terminal_colours import ColourTrilean, resolve_color_default, strip_ansi
 from consolekit.utils import TerminalRenderer
 
-__all__ = [
+__all__ = (
 		"MarkdownHelpCommand",
 		"MarkdownHelpGroup",
 		"MarkdownHelpMixin",
 		"RawHelpCommand",
 		"RawHelpGroup",
 		"RawHelpMixin",
 		"SuggestionGroup",
 		"ContextInheritingGroup",
-		]
+		)
 
 _argument = Plural("argument", "arguments")
 
 
 class RawHelpMixin:
 	"""
 	Mixin class for :class:`click.Command` and :class:`click.Group` which leaves the help text unformatted.
@@ -97,15 +97,15 @@
 	.. tip:: This can be combined with groups such as :class:`~.SuggestionGroup`.
 
 	.. versionadded:: 0.8.0
 	"""
 
 	help: Optional[str]  # noqa: A003  # pylint: disable=redefined-builtin
 
-	def format_help_text(self, ctx: click.Context, formatter: click.formatting.HelpFormatter):
+	def format_help_text(self, ctx: click.Context, formatter: click.formatting.HelpFormatter) -> None:
 		"""
 		Writes the help text to the formatter if it exists.
 
 		:param ctx:
 		:param formatter:
 		"""
 
@@ -177,15 +177,15 @@
 			Creates the underlying option parser for this command.
 
 			:param ctx:
 			"""
 
 			raise NotImplementedError
 
-	def format_help_text(self, ctx: click.Context, formatter: click.formatting.HelpFormatter):
+	def format_help_text(self, ctx: click.Context, formatter: click.formatting.HelpFormatter) -> None:
 		"""
 		Writes the help text to the formatter if it exists.
 
 		:param ctx:
 		:param formatter:
 		"""
 
@@ -407,8 +407,8 @@
 			if closest:
 				message.append(f"The most similar command is {closest[0]!r}.")
 			ctx.fail('\n'.join(message))
 
 		# TODO: cmd here is Optional[click.Command], typeshed says it should be just click.Command
 		#  I think typeshed is wrong.
 		#  https://github.com/python/typeshed/blob/484c014665cdf071b292dd9630f207c03e111895/third_party/2and3/click/core.pyi#L171
-		return cmd_name, cmd, args[1:]  # type: ignore
+		return cmd_name, cmd, args[1:]  # type: ignore[return-value]
```

### Comparing `consolekit-1.4.1/consolekit/input.py` & `consolekit-1.5.0/consolekit/input.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,36 +64,35 @@
 # 3rd party
 import click
 from click.termui import _build_prompt, hidden_prompt_func
 from click.types import Path, convert_type
 
 # this package
 from consolekit._types import _ConvertibleType
-from consolekit.utils import hidden_cursor, hide_cursor, show_cursor  # noqa
 
-__all__ = [
+__all__ = (
 		"prompt",
 		"confirm",
 		"stderr_input",
 		"choice",
-		]
+		)
 
 if not bool(getattr(sys, "ps1", sys.flags.interactive)):  # pragma: no cover
 
 	try:
 		# stdlib
 		import readline
 		readline.set_history_length(0)
 		readline.set_auto_history(False)
 	except (ImportError, AttributeError):
 		# Attribute error on PyPy, ImportError on Windows etc.
 		pass
 
 
-def prompt(
+def prompt(  # noqa: MAN002
 		text: str,
 		default: Optional[str] = None,
 		hide_input: bool = False,
 		confirmation_prompt: Union[bool, str] = False,
 		type: Optional[_ConvertibleType] = None,  # noqa: A002  # pylint: disable=redefined-builtin
 		value_proc: Optional[Callable[[Optional[str]], Any]] = None,
 		prompt_suffix: str = ": ",
@@ -124,65 +123,73 @@
 		For example, if the choice is either ``day`` or ``week``,
 		``show_choices`` is :py:obj:`True` and ``text`` is ``'Group by'`` then the
 		prompt will be ``'Group by (day, week): '``.
 	"""
 
 	result = None  # noqa
 
-	def prompt_func(text):
+	def prompt_func(text: Any) -> Any:
 		try:
 			return _prompt(text, err=err, hide_input=hide_input)
 		except (KeyboardInterrupt, EOFError):
 			if hide_input:
 				click.echo(None, err=err)
 			raise click.Abort()
 
 	if value_proc is None:
 		value_proc = convert_type(type, default)
 
-	prompt = _build_prompt(text, prompt_suffix, show_default, default, show_choices, type)  # type: ignore
+	prompt = _build_prompt(
+			text,
+			prompt_suffix,
+			show_default,
+			default,
+			show_choices,
+			type,  # type: ignore[arg-type]
+			)
+
+	has_default = default is not None
 
 	while True:
 		while True:
 			value = prompt_func(prompt)
 
 			if value:
 				break
-			elif default is not None:
-				if isinstance(value_proc, Path):
+			elif has_default:
+				if isinstance(value_proc, Path):  # pylint: disable=loop-invariant-statement
 					# validate Path default value (exists, dir_okay etc.)
 					value = default
 					break
 				return default
 
-		try:
+		try:  # pylint: disable=loop-try-except-usage
 			result = value_proc(value)
 		except click.UsageError as e:
-			click.echo(f"Error: {e.message}", err=err)
+			click.echo(f"Error: {e.message}", err=err)  # pylint: disable=loop-invariant-statement
 			continue
 
 		if not confirmation_prompt:
 			return result
 
-		if confirmation_prompt:
-			if confirmation_prompt is True:
-				confirmation_prompt = "Repeat for confirmation: "
+		if confirmation_prompt is True:
+			confirmation_prompt = "Repeat for confirmation: "
 
 		while True:
 			value2 = prompt_func(confirmation_prompt)
 			if value2:
 				break
 
-		if value == value2:
+		if value == value2:  # pylint: disable=loop-invariant-statement
 			return result
 
 		click.echo("Error: the two entered values do not match", err=err)
 
 
-def confirm(
+def confirm(  # noqa: MAN002
 		text: str,
 		default: bool = False,
 		abort: bool = False,
 		prompt_suffix: str = ": ",
 		show_default: bool = True,
 		err: bool = False,
 		):
@@ -201,15 +208,15 @@
 	:param show_default: Shows or hides the default value in the prompt.
 	:param err: If :py:obj:`True` the file defaults to ``stderr`` instead of ``stdout``, the same as with echo.
 	"""
 
 	prompt = _build_prompt(text, prompt_suffix, show_default, "Y/n" if default else "y/N")
 
 	while True:
-		try:
+		try:  # pylint: disable=loop-try-except-usage
 			value = _prompt(prompt, err=err, hide_input=False).lower().strip()
 		except (KeyboardInterrupt, EOFError):
 			raise click.Abort()
 
 		if value in ('y', "yes"):
 			rv = True
 		elif value in ('n', "no"):
@@ -253,29 +260,29 @@
 		flush = file.flush
 	except AttributeError:
 		pass
 	else:
 		flush()
 
 	try:
-		file.softspace = 0  # type: ignore
+		file.softspace = 0  # type: ignore[attr-defined]
 	except (AttributeError, TypeError):
 		pass
 
 	line = stdin.readline()
 
 	if not line:  # inputting an empty line gives line == '\n'
 		raise EOFError
 	elif line[-1] == '\n':
 		return line[:-1]
 
 	return line
 
 
-def _prompt(text, err: bool, hide_input: bool):
+def _prompt(text: Any, err: bool, hide_input: bool):  # noqa: MAN002
 	if sys.platform != "linux":
 		# Write the prompt separately so that we get nice
 		# coloring through colorama on Windows
 		click.echo(text, nl=False, err=err)
 		text = ''
 
 	if hide_input:
@@ -364,15 +371,17 @@
 				text=text,
 				default=default,
 				type=type_,
 				prompt_suffix=prompt_suffix,
 				show_default=False,
 				err=err,
 				)
+		# pylint: disable=loop-invariant-statement
 		if isinstance(options, Mapping):
 			selection = selection.strip().upper()
 			if selection not in options:
-				click.echo(f"Please enter a valid option.")
+				click.echo("Please enter a valid option.")
 			else:
 				return selection
 		else:
 			return selection - start_index
+		# pylint: enable=loop-invariant-statement
```

### Comparing `consolekit-1.4.1/consolekit/options.py` & `consolekit-1.5.0/consolekit/options.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,28 +66,28 @@
 import click
 from click.decorators import _param_memo
 
 # this package
 import consolekit.input
 from consolekit._types import Callback, _ConvertibleType
 
-__all__ = [
+__all__ = (
 		"verbose_option",
 		"version_option",
 		"colour_option",
 		"force_option",
 		"no_pager_option",
 		"MultiValueOption",
 		"flag_option",
 		"auto_default_option",
 		"auto_default_argument",
 		"DescribedArgument",
 		"_A",
 		"_C",
-		]
+		)
 
 _A = TypeVar("_A", bound=click.Argument)
 _C = TypeVar("_C", bound=click.Command)
 
 
 class VerboseVersionCountType(click.IntRange):
 	"""
@@ -96,15 +96,15 @@
 	.. versionadded:: 0.8.1
 	"""
 
 	def __init__(self):
 		super().__init__(min=0)
 
 	@staticmethod
-	def _describe_range():  # pragma: no cover
+	def _describe_range() -> str:  # pragma: no cover
 		"""
 		Describe the range for use in help text.
 		"""
 
 		return ''
 
 
@@ -163,15 +163,15 @@
 			is_eager=True,
 			help="Show the version and exit.",
 			type=VerboseVersionCountType(),
 			callback=cast(Callback, callback),
 			)
 
 
-def colour_option(help_text="Whether to use coloured output.") -> Callable[[_C], _C]:
+def colour_option(help_text: str = "Whether to use coloured output.") -> Callable[[_C], _C]:
 	"""
 	Adds an option (via the parameter ``colour``: :class:`bool`) to enable verbose output.
 
 	.. versionadded:: 0.4.0
 
 	:param help_text: The help text for the option.
 	"""
@@ -193,15 +193,15 @@
 
 	:param help_text: The help text for the option.
 	"""
 
 	return flag_option("-f", "--force", help=help_text)
 
 
-def no_pager_option(help_text="Disable the output pager.") -> Callable[[_C], _C]:
+def no_pager_option(help_text: str = "Disable the output pager.") -> Callable[[_C], _C]:
 	"""
 	Decorator to add the ``--no-pager`` option to a click command.
 
 	The value is exposed via the parameter ``no_pager``: :class:`bool`.
 
 	.. versionadded:: 0.5.0
 
@@ -258,15 +258,15 @@
 		_get_default_from_callback_and_set(f, option)
 
 		return f
 
 	return decorator
 
 
-def _get_default_from_callback_and_set(command: click.Command, param: click.Parameter):
+def _get_default_from_callback_and_set(command: click.Command, param: click.Parameter) -> None:
 	if command.callback is not None:
 		# The callback *can* be None, for a no-op
 
 		if param.name is None:  # pragma: no cover
 			raise ValueError("The parameter name cannot be None")
 
 		signature: inspect.Signature = inspect.signature(command.callback)
@@ -373,47 +373,52 @@
 				metavar=metavar,
 				expose_value=expose_value,
 				is_eager=is_eager,
 				)
 		self._previous_parser_process: Optional[Callable] = None
 		self._eat_all_parser: Optional[click.parser.Option] = None
 
-	def add_to_parser(self, parser: click.OptionParser, ctx: click.Context):
+	def add_to_parser(self, parser: click.OptionParser, ctx: click.Context) -> Any:
 		"""
 		Add the :class:`~.MultiValueOption` to the given parser.
 
 		:param parser:
 		:param ctx:
 		"""
 
-		def parser_process(value, state):
+		def parser_process(value, state) -> None:  # noqa: MAN001
 			# method to hook to the parser.process
 			done = False
 			value = [value]
 			# grab everything up to the next option
+
+			assert self._eat_all_parser is not None  # skipcq
 			while state.rargs and not done:
-				for prefix in self._eat_all_parser.prefixes:  # type: ignore
+				for prefix in self._eat_all_parser.prefixes:
 					if state.rargs[0].startswith(prefix):
 						done = True
 				if not done:
-					value.append(state.rargs.pop(0))
+					value.append(state.rargs.pop(0))  # pylint: disable=loop-invariant-statement
 
 			value = tuple(value)
 
 			# call the actual process
-			self._previous_parser_process(value, state)  # type: ignore
+			assert self._previous_parser_process is not None  # skipcq
+			self._previous_parser_process(value, state)
 
 		retval = super().add_to_parser(parser, ctx)
 
 		for name in self.opts:
+			# pylint: disable=loop-invariant-statement
 			our_parser: Optional[click.parser.Option] = parser._long_opt.get(name) or parser._short_opt.get(name)
-			if our_parser:
+			if our_parser is not None:
+				# pylint: enable=loop-invariant-statement
 				self._eat_all_parser = our_parser
 				self._previous_parser_process = our_parser.process
-				our_parser.process = parser_process  # type: ignore
+				our_parser.process = parser_process  # type: ignore[assignment]
 				break
 
 		return retval
 
 	def process_value(self, ctx: click.Context, value: Any) -> Optional[Tuple]:
 		"""
 		Given a value and context, converts the value as necessary.
@@ -429,24 +434,24 @@
 
 		# assert isinstance(value, tuple), type(value)
 
 		if value is not None:
 			if isinstance(value, Iterable) and not isinstance(value, str):
 				return tuple(self.type_cast_value(ctx, v) for v in value)
 			elif value in ("()", str(self.default)) or not value:
-				return self.default  # type: ignore
+				return self.default  # type: ignore[return-value]
 			else:
 				return self.type_cast_value(ctx, value)
 		else:
 			return None
 
 
 class _Option(click.Option):
 
-	def prompt_for_value(self, ctx: click.Context):
+	def prompt_for_value(self, ctx: click.Context):  # noqa: MAN002
 		"""
 		This is an alternative flow that can be activated in the full value processing if a value does not exist.
 
 		It will prompt the user until a valid value exists and then returns the processed value as result.
 		"""
 
 		# Calculate the default before prompting anything to be stable.
@@ -454,15 +459,15 @@
 
 		prompt_string = cast(str, self.prompt)
 
 		# If this is a prompt for a flag we need to handle this differently.
 		if self.is_bool_flag:
 			return consolekit.input.confirm(
 					prompt_string,
-					default,  # type: ignore
+					default,  # type: ignore[arg-type]
 					)
 
 		return consolekit.input.prompt(
 				prompt_string,
 				default=default,
 				type=self.type,
 				hide_input=self.hide_input,
```

### Comparing `consolekit-1.4.1/consolekit/terminal_colours.py` & `consolekit-1.5.0/consolekit/terminal_colours.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 from functools import partial
 from typing import Deque, Iterable, List, Optional, Pattern, Type, TypeVar, Union
 
 # 3rd party
 import click
 from typing_extensions import Final
 
-__all__ = [
+__all__ = (
 		"AnsiFore",
 		"AnsiBack",
 		"AnsiStyle",
 		"AnsiCursor",
 		"Fore",
 		"Back",
 		"Style",
@@ -93,19 +93,19 @@
 		"code_to_chars",
 		"resolve_color_default",
 		"set_title",
 		"strip_ansi",
 		"CSI",
 		"OSC",
 		"BEL",
-		]
+		)
 
 try:
 	# 3rd party
-	import colorama  # type: ignore
+	import colorama  # type: ignore[import]
 	colorama.init()
 
 except ImportError:
 	pass
 
 _C = TypeVar("_C", bound="Colour")
 _AC = TypeVar("_AC", bound="AnsiCodes")
@@ -220,15 +220,15 @@
 	__slots__ = ("style", "reset", "stack")
 
 	style: str
 	reset: str
 	stack: Union[Deque[str], List[str]]
 
 	def __new__(cls, style: str, stack: Union[Deque[str], List[str]], reset: str) -> "Colour":  # noqa: D102
-		self = super().__new__(cls, style)  # type: ignore
+		self = super().__new__(cls, style)  # type: ignore[import]
 		self.style = style
 		self.stack = stack
 		self.reset = reset
 
 		return self
 
 	def __enter__(self) -> None:
@@ -236,15 +236,15 @@
 		self.stack.append(self.style)
 
 	def __exit__(self, exc_type, exc_val, exc_tb) -> None:
 		if self.style == self.stack[-1]:
 			self.stack.pop()
 			print(self.stack[-1], end='')
 
-	def __call__(self, text) -> str:
+	def __call__(self, text) -> str:  # noqa: MAN001
 		"""
 		Returns the given text in this colour.
 		"""
 
 		return f"{self}{text}{self.reset}"
 
 	@classmethod
@@ -396,19 +396,19 @@
 
 	.. note:: Not all terminals support 24-bit colours.
 	"""
 
 	# 3rd party
 	from domdf_python_tools.iterative import chunks
 
-	def print_heading(text: str, block_size: int = 3, n_blocks: int = 36):
+	def print_heading(text: str, block_size: int = 3, n_blocks: int = 36) -> None:
 		click.echo()
 		click.echo(str(text).center(((block_size + 1) * n_blocks) - 1, '-'))
 
-	def print_line(values: Iterable[int], block_size: int = 3):
+	def print_line(values: Iterable[int], block_size: int = 3) -> None:
 		values = list(values)
 		mid = len(values) // 2
 
 		colour: Optional[bool] = resolve_color_default()
 		echo = partial(click.echo, nl=False, color=colour)
 
 		for code in values[:mid]:
@@ -426,15 +426,15 @@
 			block_size=8,
 			n_blocks=16
 			)
 
 	print_line(range(16), block_size=8)
 
 	print_heading("216 Colours")
-	for row in chunks(range(16, 232), 36):
+	for row in chunks(range(16, 232), 36):  # pylint: disable=loop-invariant-statement
 		print_line(row)
 
 	print_heading("Greyscale Colours", block_size=5, n_blocks=24)
 	print_line(range(232, 256), block_size=5)
 
 	click.echo('\n')
```

### Comparing `consolekit-1.4.1/consolekit/terminal_colours.pyi` & `consolekit-1.5.0/consolekit/terminal_colours.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 	style: str
 	reset: str
 	stack: Union[Deque[str], List[str]]
 
 	def __new__(cls, style: str, stack: Union[Deque[str], List[str]], reset: str) -> "Colour": ...
 	def __enter__(self) -> None: ...
 	def __exit__(self, exc_type, exc_val, exc_tb) -> None: ...
-	def __call__(self, text) -> str: ...
+	def __call__(self, text) -> str: ...  # noqa: MAN001
 
 	@classmethod
 	def from_code(cls: Type[_C], code: Union[str, int], background: bool = ...) -> _C: ...
 
 	@classmethod
 	def from_256_code(cls: Type[_C], code: Union[str, int], background: bool = ...) -> _C: ...
```

### Comparing `consolekit-1.4.1/consolekit/testing.py` & `consolekit-1.5.0/consolekit/testing.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 # 3rd party
 import click.testing
 import pytest  # nodep
 from coincidence.regressions import check_file_regression  # nodep
 from pytest_regressions.file_regression import FileRegressionFixture  # nodep
 from typing_extensions import Literal
 
-__all__ = ["CliRunner", "Result", "cli_runner"]
+__all__ = ("CliRunner", "Result", "cli_runner")
 
 _click_major = int(click.__version__.split('.')[0])
 
 
 class Result(click.testing.Result):
 	"""
 	Holds the captured result of an invoked CLI script.
@@ -110,15 +110,15 @@
 					stderr_bytes=stderr_bytes,
 					exit_code=exit_code,
 					exception=exception,
 					exc_info=exc_info,
 					return_value=None,
 					)
 		else:
-			super().__init__(  # type: ignore
+			super().__init__(  # type: ignore[call-arg]
 				runner=runner,
 				stdout_bytes=stdout_bytes,
 				stderr_bytes=stderr_bytes,
 				exit_code=exit_code,
 				exception=exception,
 				exc_info=exc_info,
 				)
@@ -144,15 +144,15 @@
 		"""
 		The standard error as a string.
 		"""
 
 		return super().stderr
 
 	@classmethod
-	def _from_click_result(cls, result: click.testing.Result):
+	def _from_click_result(cls, result: click.testing.Result) -> "Result":
 		return cls(
 				runner=result.runner,
 				stdout_bytes=result.stdout_bytes,
 				stderr_bytes=result.stderr_bytes,
 				exit_code=result.exit_code,
 				exception=result.exception,
 				exc_info=result.exc_info,
@@ -204,15 +204,15 @@
 			env: Optional[Mapping[str, str]] = None,
 			*,
 			echo_stdin: bool = False,
 			mix_stderr: bool = True,
 			) -> None:
 		super().__init__(charset, env, echo_stdin, mix_stderr)
 
-	def invoke(  # type: ignore  # noqa: D101
+	def invoke(  # type: ignore[override]  # noqa: D101
 		self,
 		cli: click.BaseCommand,
 		args: Optional[Union[str, Iterable[str]]] = None,
 		input: Optional[Union[bytes, str, IO]] = None,  # noqa: A002  # pylint: disable=redefined-builtin
 		env: Optional[Mapping[str, str]] = None,
 		*,
 		catch_exceptions: bool = False,
```

### Comparing `consolekit-1.4.1/consolekit/tracebacks.py` & `consolekit-1.5.0/consolekit/tracebacks.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 import click
 from domdf_python_tools.compat import nullcontext
 
 if sys.version_info >= (3, 7) or TYPE_CHECKING:
 	# stdlib
 	from typing import NoReturn
 
-__all__ = ["TracebackHandler", "handle_tracebacks", "traceback_handler", "traceback_option"]
+__all__ = ("TracebackHandler", "handle_tracebacks", "traceback_handler", "traceback_option")
 
 _C = TypeVar("_C", bound=click.Command)
 
 
 class TracebackHandler:
 	"""
 	Context manager to abort execution with a short error message
@@ -135,42 +135,39 @@
 	def handle(self, e: BaseException) -> bool:
 		"""
 		Handle the given exception.
 
 		:param e:
 		"""
 
-		# this package
-		from consolekit.utils import abort
-
 		exception_name = e.__class__.__name__
 
 		if hasattr(self, f"handle_{exception_name}"):
 			return getattr(self, f"handle_{exception_name}")(e)
 
 		for base in e.__class__.__mro__:
 			if hasattr(self, f"handle_{base.__name__}"):
 				return getattr(self, f"handle_{base.__name__}")(e)
 
 		self.abort(f"An error occurred: {e}")
 
 	@contextlib.contextmanager
-	def __call__(self):
+	def __call__(self):  # noqa: MAN002
 		"""
 		Use the :class:`~.TracebackHandler` with a :keyword:`with` block, and handle any exceptions raised within.
 		"""
 
 		try:
 			yield
 		except BaseException as e:
 			self.handle(e)
 
 
 @contextlib.contextmanager
-def traceback_handler():
+def traceback_handler():  # noqa: MAN002
 	"""
 	Context manager to abort execution with a short error message on the following exception types:
 
 	* :exc:`FileNotFoundError`
 	* :exc:`FileExistsError`
 
 	Other custom exception classes inheriting from :exc:`Exception` are also handled,
```

### Comparing `consolekit-1.4.1/consolekit/utils.py` & `consolekit-1.5.0/consolekit/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,51 +47,51 @@
 from typing import IO, Any, Iterable, Iterator, List, Optional, Sequence, Union
 
 # 3rd party
 import click
 import deprecation_alias
 from domdf_python_tools.stringlist import StringList
 from domdf_python_tools.words import SANS_SERIF_ITALIC_LETTERS
-from mistletoe import block_token, span_token  # type: ignore
-from mistletoe.base_renderer import BaseRenderer  # type: ignore
+from mistletoe import block_token, span_token  # type: ignore[import]
+from mistletoe.base_renderer import BaseRenderer  # type: ignore[import]
 from typing_extensions import TypeGuard
 
 # this package
 from consolekit import terminal_colours, tracebacks
 from consolekit.terminal_colours import ColourTrilean, resolve_color_default
 
-__all__ = [
+__all__ = (
 		"get_env_vars",
 		"is_command",
 		"import_commands",
 		"abort",
 		"overtype",
 		"coloured_diff",
 		"solidus_spinner",
 		"braille_spinner",
 		"snake_spinner",
 		"hide_cursor",
 		"show_cursor",
 		"TerminalRenderer",
 		"hidden_cursor",
 		"long_echo",
-		]
+		)
 
 _deprecator = deprecation_alias.deprecated(
 		deprecated_in="1.0.0",
 		removed_in="2.0.0",
-		current_version="1.4.1",
+		current_version="1.5.0",
 		details="Import from consolekit.tracebacks instead."
 		)
 
 handle_tracebacks = _deprecator(tracebacks.handle_tracebacks)
 traceback_handler = _deprecator(tracebacks.traceback_handler)
 
 
-def get_env_vars(ctx, args, incomplete):  # noqa: D103
+def get_env_vars(ctx, args, incomplete) -> List[str]:  # noqa: D103,MAN001
 	return [k for k in os.environ.keys() if incomplete in k]
 
 
 def is_command(obj: Any) -> TypeGuard[click.Command]:
 	"""
 	Return whether ``obj`` is a click command.
 
@@ -328,18 +328,18 @@
 		hide_cursor()
 		yield
 	finally:
 		show_cursor()
 
 
 @lru_cache(1)
-def _pycharm_terminal():
+def _pycharm_terminal() -> bool:
 	try:
 		# 3rd party
-		import psutil  # type: ignore  # nodep
+		import psutil  # type: ignore[import]  # nodep
 
 		parent_process = psutil.Process(os.getppid())
 		grandparent_process = psutil.Process(parent_process.ppid())
 		great_grandparent_process = psutil.Process(grandparent_process.ppid())
 		great_grandparent_name = great_grandparent_process.name()
 
 		#: TODO: pycharm on Windows and macOS
@@ -448,24 +448,24 @@
 			self._ol_number += 1
 			return f" {self._ol_number}. {self.render_inner(token).lstrip()}"
 
 		else:
 			return f" * {self.render_inner(token).lstrip()}"
 
 	@staticmethod
-	def render_line_break(token):
+	def render_line_break(token) -> str:  # noqa: MAN001
 		"""
 		Render a line break in a multiline paragraph.
 
 		:param token:
 		"""
 
 		return ' '
 
-	def render(self, token) -> str:
+	def render(self, token) -> str:  # noqa: MAN001
 		"""
 		Render the given token for display in a terminal.
 
 		:param token:
 		"""
 
 		return super().render(token).replace("\n\n\n", "\n\n")
```

### Comparing `consolekit-1.4.1/pyproject.toml` & `consolekit-1.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "flit-core<4,>=3.2",]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "consolekit"
-version = "1.4.1"
+version = "1.5.0"
 description = "Additional utilities for click."
 readme = "README.rst"
 requires-python = ">=3.6.1"
 keywords = [ "click", "terminal",]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
@@ -18,14 +18,15 @@
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Typing :: Typed",
 ]
 dependencies = [
     "click>=7.1.2",
@@ -149,15 +150,15 @@
 base-classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Typing :: Typed",
 ]
-python-versions = [ "3.6", "3.7", "3.8", "3.9", "3.10",]
+python-versions = [ "3.6", "3.7", "3.8", "3.9", "3.10", "3.11",]
 python-implementations = [ "CPython", "PyPy",]
 platforms = [ "Windows", "macOS", "Linux",]
 license-key = "MIT"
 
 [tool.mypy]
 python_version = "3.6"
 namespace_packages = true
```

### Comparing `consolekit-1.4.1/PKG-INFO` & `consolekit-1.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: consolekit
-Version: 1.4.1
+Version: 1.5.0
 Summary: Additional utilities for click.
 Keywords: click,terminal
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 Requires-Python: >=3.6.1
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Dist: click>=7.1.2
 Requires-Dist: colorama>=0.4.3; python_version < "3.10" and platform_system == "Windows"
 Requires-Dist: deprecation-alias>=0.1.1
@@ -99,16 +100,16 @@
 	:target: https://github.com/domdfcoding/consolekit/actions?query=workflow%3A%22Flake8%22
 	:alt: Flake8 Status
 
 .. |actions_mypy| image:: https://github.com/domdfcoding/consolekit/workflows/mypy/badge.svg
 	:target: https://github.com/domdfcoding/consolekit/actions?query=workflow%3A%22mypy%22
 	:alt: mypy status
 
-.. |requires| image:: https://dependency-dash.herokuapp.com/github/domdfcoding/consolekit/badge.svg
-	:target: https://dependency-dash.herokuapp.com/github/domdfcoding/consolekit/
+.. |requires| image:: https://dependency-dash.repo-helper.uk/github/domdfcoding/consolekit/badge.svg
+	:target: https://dependency-dash.repo-helper.uk/github/domdfcoding/consolekit/
 	:alt: Requirements Status
 
 .. |coveralls| image:: https://img.shields.io/coveralls/github/domdfcoding/consolekit/master?logo=coveralls
 	:target: https://coveralls.io/github/domdfcoding/consolekit?branch=master
 	:alt: Coverage
 
 .. |codefactor| image:: https://img.shields.io/codefactor/grade/github/domdfcoding/consolekit?logo=codefactor
@@ -142,23 +143,23 @@
 .. |license| image:: https://img.shields.io/github/license/domdfcoding/consolekit
 	:target: https://github.com/domdfcoding/consolekit/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/consolekit
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/consolekit/v1.4.1
+.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/consolekit/v1.5.0
 	:target: https://github.com/domdfcoding/consolekit/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/consolekit
 	:target: https://github.com/domdfcoding/consolekit/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2022
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/consolekit
 	:target: https://pypi.org/project/consolekit/
 	:alt: PyPI - Downloads
 
 .. end shields
```

