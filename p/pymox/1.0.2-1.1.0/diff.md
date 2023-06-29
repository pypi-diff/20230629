# Comparing `tmp/pymox-1.0.2.tar.gz` & `tmp/pymox-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymox-1.0.2.tar", max compression
+gzip compressed data, was "pymox-1.1.0.tar", max compression
```

## Comparing `pymox-1.0.2.tar` & `pymox-1.1.0.tar`

### file list

```diff
@@ -1,6 +1,10 @@
--rw-r--r--   0        0        0    11875 2023-06-14 11:36:14.149469 pymox-1.0.2/README.rst
--rw-r--r--   0        0        0      991 2023-06-14 11:22:28.830014 pymox-1.0.2/mox/__init__.py
--rwxr-xr-x   0        0        0    74885 2023-06-14 11:36:37.635178 pymox-1.0.2/mox/mox.py
--rw-r--r--   0        0        0     5488 2023-06-14 11:22:28.832449 pymox-1.0.2/mox/stubout.py
--rw-r--r--   0        0        0     2271 2023-06-14 11:37:46.154860 pymox-1.0.2/pyproject.toml
--rw-r--r--   0        0        0    13811 1970-01-01 00:00:00.000000 pymox-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11796 2023-06-23 22:13:45.122864 pymox-1.1.0/README.rst
+-rw-r--r--   0        0        0     1160 2023-06-29 13:56:32.121525 pymox-1.1.0/mox/__init__.py
+-rw-r--r--   0        0        0    15666 2023-06-29 13:36:44.187644 pymox-1.1.0/mox/comparators.py
+-rw-r--r--   0        0        0     5455 2023-06-29 13:57:43.844169 pymox-1.1.0/mox/exceptions.py
+-rw-r--r--   0        0        0     5669 2023-06-29 13:54:19.660221 pymox-1.1.0/mox/groups.py
+-rwxr-xr-x   0        0        0    45161 2023-06-29 14:47:51.913389 pymox-1.1.0/mox/mox.py
+-rw-r--r--   0        0        0     5503 2023-06-29 14:38:09.743396 pymox-1.1.0/mox/stubout.py
+-rw-r--r--   0        0        0     3570 2023-06-29 14:07:50.861301 pymox-1.1.0/mox/testing.py
+-rw-r--r--   0        0        0     2689 2023-06-29 14:52:40.162187 pymox-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0    13632 1970-01-01 00:00:00.000000 pymox-1.1.0/PKG-INFO
```

### Comparing `pymox-1.0.2/README.rst` & `pymox-1.1.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -163,39 +163,39 @@
 ~~~~~~~~~~~
 
 You can use comparators when you are unsure of the arguments of a method
 call.
 
 .. code:: python
 
-       def test_quack_7(self):  
+       def test_quack_7(self):
            m = mox.Mox()
            duck = Duck()
-           
+
            m.stubout(Duck, 'quack')
-           
+
            def validate_arg(arg):
             if arg in [1, 2, 3]:
              return True
             return False
-           
+
            duck.quack(times=mox.is_a(int)).returns(['new quack'])
            duck.quack(times=mox.not_(mox.is_(4))).returns(['new quack'])
            duck.quack(times=mox.func(validate_arg)).returns(['new quack'])
            duck.quack(times=mox.or_(mox.Is(1), mox.is_(2), mox.is_(3))).returns(['new quack'])
-           
+
            duck.quack(times=mox.ignore_arg()).returns(['new quack'])
            duck.quack(times=mox.is_almost(1.00003, places=4)).returns(['new quack'])
-           
+
            m.replay_all()
            assert duck.quack(times=random.choice([1, 2, 3])) == ['new quack']
            assert duck.quack(times=random.choice([1, 2, 3])) == mox.in_('new quack')
            assert duck.quack(times=random.choice([1, 2, 3]))[0] == mox.str_contains('quack')
            assert duck.quack(times=random.choice([1, 2, 3])) == mox.same_elements_as({'new quack'})
-           
+
            assert duck.quack(times=random.choice([1, 2, 3])) == ['new quack']
            assert duck.quack(times=1) == ['new quack']
            m.verify_all()
 
 All the assertions for the test above should pass. There are other cool
 comparators, like: ``and``, ``contains_attribute_value``,
 ``contains_key_value``.
@@ -223,15 +223,15 @@
                        choices.pop()
                    self._do_quack(choices=choices)
 
            m = mox.Mox()
            duck = StopQuackingDuck()
 
            m.stubout(StopQuackingDuck, '_do_quack')
-           
+
            choices_1 = mox.value()
            choices_2 = mox.value()
            duck._do_quack(choices=mox.remember(choices_1))
            duck._do_quack(choices=mox.remember(choices_2))
            duck._do_quack(choices=mox.remember(choices_2))
            duck._do_quack(choices=mox.remember(choices_2))
```

### Comparing `pymox-1.0.2/mox/mox.py` & `pymox-1.1.0/mox/mox.py`

 * *Files 27% similar despite different names*

```diff
@@ -54,209 +54,44 @@
   my_mox.ReplayAll()
 
   # Inject mock object and run test
   controller.SetDao(mock_dao)
   controller.DeletePersonById('1')
 
   # Verify all methods were called as expected
-  my_mox.VerifyAll()
+  my_mox.verify_all()
 """
+from .comparators import IsA
+from .exceptions import (
+    Error,
+    ExpectedMethodCallsError,
+    ExpectedMockCreationError,
+    PrivateAttributeError,
+    SwallowedExceptionError,
+    UnexpectedMethodCallError,
+    UnexpectedMockCreationError,
+    UnknownMethodCallError,
+)
+from .groups import MethodGroup, MultipleTimesGroup, UnorderedGroup
+
 
 try:
+    # Python imports
     import abc
 except ImportError:
     abc = None  # Python 2.5 and earlier
-import difflib
+# Python imports
 import inspect
-import re
 import types
-import unittest
 from collections import deque
 from re import search as re_search
 
 from . import stubout
 
 
-class Error(AssertionError):
-    """Base exception for this module."""
-
-    pass
-
-
-class ExpectedMethodCallsError(Error):
-    """Raised when Verify() is called before all expected methods have been
-    called
-    """
-
-    def __init__(self, expected_methods):
-        """Init exception.
-
-        Args:
-          # expected_methods: A sequence of MockMethod objects that should have
-          #   been called.
-
-          expected_methods: [MockMethod]
-
-        Raises:
-          ValueError: if expected_methods contains no methods.
-        """
-
-        if not expected_methods:
-            raise ValueError("There must be at least one expected method")
-        Error.__init__(self)
-        self._expected_methods = expected_methods
-
-    def __str__(self):
-        calls = "\n".join(["%3d.  %s" % (i, m) for i, m in enumerate(self._expected_methods)])
-        return "Verify: Expected methods never called:\n%s" % (calls,)
-
-
-class UnexpectedMethodCallError(Error):
-    """Raised when an unexpected method is called.
-
-    This can occur if a method is called with incorrect parameters, or out of
-    the specified order.
-    """
-
-    def __init__(self, unexpected_method, expected):
-        """Init exception.
-
-        Args:
-          # unexpected_method: MockMethod that was called but was not at the
-          #   head of the expected_method queue.
-          # expected: MockMethod or UnorderedGroup the method should have
-          #   been in.
-          unexpected_method: MockMethod
-          expected: MockMethod or UnorderedGroup
-        """
-
-        Error.__init__(self)
-        if expected is None:
-            self._str = "Unexpected method call %s" % (unexpected_method,)
-        else:
-            differ = difflib.Differ()
-            diff = differ.compare(str(unexpected_method).splitlines(True), str(expected).splitlines(True))
-            self._str = "Unexpected method call.  unexpected:-  expected:+\n%s" % (
-                "\n".join(line.rstrip() for line in diff),
-            )
-
-    def __str__(self):
-        return self._str
-
-
-class UnknownMethodCallError(Error):
-    """Raised if an unknown method is requested of the mock object."""
-
-    def __init__(self, unknown_method_name):
-        """Init exception.
-
-        Args:
-          # unknown_method_name: Method call that is not part of the mocked
-          #   class's public interface.
-          unknown_method_name: str
-        """
-
-        Error.__init__(self)
-        self._unknown_method_name = unknown_method_name
-
-    def __str__(self):
-        return "Method called is not a member of the object: %s" % self._unknown_method_name
-
-
-class PrivateAttributeError(Error):
-    """
-    Raised if a MockObject is passed a private additional attribute name.
-    """
-
-    def __init__(self, attr):
-        Error.__init__(self)
-        self._attr = attr
-
-    def __str__(self):
-        return "Attribute '%s' is private and should not be available in a " " mock object." % self._attr
-
-
-class ExpectedMockCreationError(Error):
-    """Raised if mocks should have been created by StubOutClassWithMocks."""
-
-    def __init__(self, expected_mocks):
-        """Init exception.
-
-        Args:
-          # expected_mocks: A sequence of MockObjects that should have been
-          #   created
-
-        Raises:
-          ValueError: if expected_mocks contains no methods.
-        """
-
-        if not expected_mocks:
-            raise ValueError("There must be at least one expected method")
-        Error.__init__(self)
-        self._expected_mocks = expected_mocks
-
-    def __str__(self):
-        mocks = "\n".join(["%3d.  %s" % (i, m) for i, m in enumerate(self._expected_mocks)])
-        return "Verify: Expected mocks never created:\n%s" % (mocks,)
-
-
-class UnexpectedMockCreationError(Error):
-    """Raised if too many mocks were created by StubOutClassWithMocks."""
-
-    def __init__(self, instance, *params, **named_params):
-        """Init exception.
-
-        Args:
-          # instance: the type of obejct that was created
-          # params: parameters given during instantiation
-          # named_params: named parameters given during instantiation
-        """
-
-        Error.__init__(self)
-        self._instance = instance
-        self._params = params
-        self._named_params = named_params
-
-    def __str__(self):
-        args = ", ".join(["%s" % v for i, v in enumerate(self._params)])
-        error = "Unexpected mock creation: %s(%s" % (self._instance, args)
-
-        if self._named_params:
-            error += ", " + ", ".join(["%s=%s" % (k, v) for k, v in self._named_params.items()])
-
-        error += ")"
-        return error
-
-
-class SwallowedExceptionError(Error):
-    """Raised when Verify() is called after something already threw an
-    exception.
-
-    This means that the exception that was thrown was somehow swallowed,
-    allowing the test to continue when it should not have.
-    """
-
-    def __init__(self, previous_exceptions):
-        """Init exception.
-
-        Args:
-          # previous_exceptions: A sequence of Error objects that were raised.
-          previous_exceptions: [Error]
-        """
-
-        Error.__init__(self)
-        self._previous_exceptions = previous_exceptions
-
-    def __str__(self):
-        exceptions = "\n".join(
-            ["%3d.  %s: %s" % (i, e.__class__.__name__, e) for i, e in enumerate(self._previous_exceptions)]
-        )
-        return "Previous exceptions thrown:\n%s" % (exceptions,)
-
-
 class Mox(object):
     """Mox: a factory for creating mock objects."""
 
     # A list of types that should be stubbed out with MockObjects (as
     # opposed to MockAnythings).
     _USE_MOCK_OBJECT = [
         getattr(types, "ClassType", type),
@@ -315,27 +150,27 @@
         self._mock_objects.append(new_mock)
         return new_mock
 
     def replay_all(self):
         """Set all mock objects to replay mode."""
 
         for mock_obj in self._mock_objects:
-            mock_obj._Replay()
+            mock_obj._replay()
 
     def verify_all(self):
         """Call verify on all mock objects created."""
 
         for mock_obj in self._mock_objects:
-            mock_obj._Verify()
+            mock_obj._verify()
 
     def reset_all(self):
         """Call reset on all mock objects.  This does not unset stubs."""
 
         for mock_obj in self._mock_objects:
-            mock_obj._Reset()
+            mock_obj._reset()
 
     def stubout(self, obj, attr_name, use_mock_anything=False):
         """Replace a method, attribute, etc. with a Mock.
 
         This will replace a class or module with a MockObject, and everything
         else (method, function, etc) with a MockAnything.  This can be
         overridden to always use a MockAnything by setting use_mock_anything to
@@ -357,20 +192,20 @@
         if (
             attr_type in self._USE_MOCK_OBJECT
             or
             # isinstance(attr_type, tuple(self._USE_MOCK_OBJECT)) or
             isinstance(attr_to_replace, object)
             or inspect.isclass(attr_to_replace)
         ) and not use_mock_anything:
-            stub = self.CreateMock(attr_to_replace)
+            stub = self.create_mock(attr_to_replace)
         else:
-            stub = self.CreateMockAnything(description="Stub for %s" % attr_to_replace)
+            stub = self.create_mock_anything(description="Stub for %s" % attr_to_replace)
             stub.__name__ = attr_name
 
-        self.stubs.Set(obj, attr_name, stub)
+        self.stubs.set(obj, attr_name, stub)
 
     def stubout_class(self, obj, attr_name):
         """Replace a class with a "mock factory" that will create mock objects.
 
         This is useful if the code-under-test directly instantiates
         dependencies.  Previously some boilerplate was necessary to
         create a mock that would act as a factory.  Using
@@ -389,39 +224,39 @@
                                           use_mock_anything=True)
         foo_factory(1, 2).AndReturn(mock1)
         foo_factory(9, 10).AndReturn(mock2)
         mox.ReplayAll()
 
         my_import.FooClass(1, 2)   # Returns mock1 again.
         my_import.FooClass(9, 10)  # Returns mock2 again.
-        mox.VerifyAll()
+        mox.verify_all()
 
         # Example using StubOutClassWithMocks:
 
         mox.StubOutClassWithMocks(my_import, 'FooClass')
         mock1 = my_import.FooClass(1, 2)   # Returns a new mock of FooClass
         mock2 = my_import.FooClass(9, 10)  # Returns another mock instance
         mox.ReplayAll()
 
         my_import.FooClass(1, 2)   # Returns mock1 again.
         my_import.FooClass(9, 10)  # Returns mock2 again.
-        mox.VerifyAll()
+        mox.verify_all()
         """
         attr_to_replace = getattr(obj, attr_name)
         attr_type = type(attr_to_replace)
 
         if attr_type == MockAnything or attr_type == MockObject:
             raise TypeError("Cannot mock a MockAnything! Did you remember to call unset_stubs in your previous test?")
 
         if not inspect.isclass(attr_to_replace):
             raise TypeError("Given attr is not a Class. Use stubout.")
 
         factory = _MockObjectFactory(attr_to_replace, self)
         self._mock_objects.append(factory)
-        self.stubs.Set(obj, attr_name, factory)
+        self.stubs.set(obj, attr_name, factory)
 
     def unset_stubs(self):
         """Restore stubs to their original state."""
 
         self.stubs.unset_all()
 
     CreateMock = create_mock
@@ -602,15 +437,15 @@
         if self._expected_calls_queue:
             # The last MultipleTimesGroup is not popped from the queue.
             is_multiple_times_group = isinstance(self._expected_calls_queue[0], MultipleTimesGroup)
 
             if (
                 len(self._expected_calls_queue) == 1
                 and is_multiple_times_group
-                and self._expected_calls_queue[0].IsSatisfied()
+                and self._expected_calls_queue[0].is_satisfied()
             ):
                 pass
             else:
                 raise ExpectedMethodCallsError(self._expected_calls_queue)
 
     def _reset(self):
         """Reset the state of this mock to record mode with an empty queue."""
@@ -968,15 +803,15 @@
 
             mock_method(*params, **named_params)
 
             return self._instance_queue.pop()
         else:
             mock_method(*params, **named_params)
 
-            instance = self._mox.CreateMock(self._class_to_mock)
+            instance = self._mox.create_mock(self._class_to_mock)
             self._instance_queue.appendleft(instance)
             return instance
 
     def _verify(self):
         """Verify that all mocks have been created."""
         if self._instance_queue:
             raise ExpectedMockCreationError(self._instance_queue)
@@ -1216,19 +1051,19 @@
         """
 
         self._params = params
         self._named_params = named_params
 
         if not self._replay_mode:
             if self._checker is not None:
-                self._checker.Check(params, named_params)
+                self._checker.check(params, named_params)
             self._call_queue.append(self)
             return self
 
-        expected_method = self._VerifyMethodCall()
+        expected_method = self._verify_method_call()
 
         if expected_method._side_effects:
             result = expected_method._side_effects(*params, **named_params)
             if expected_method._return_value is None:
                 expected_method._return_value = result
 
         if expected_method._exception:
@@ -1270,20 +1105,20 @@
         Returns:
           The expected mock method.
 
         Raises:
           UnexpectedMethodCall if the method called was not expected.
         """
 
-        expected = self._PopNextMethod()
+        expected = self._pop_next_method()
 
         # Loop here, because we might have a MethodGroup followed by another
         # group.
         while isinstance(expected, MethodGroup):
-            expected, method = expected.MethodCalled(self)
+            expected, method = expected.method_called(self)
             if method is not None:
                 return method
 
         # This is a mock method, so just check equality.
         if expected != self:
             exception = UnexpectedMethodCallError(self, expected)
             self._exception_list.append(exception)
@@ -1359,20 +1194,20 @@
           group_name: the name of the group.
           group_class: the class used to create instance of this new group
         """
         group = self.get_possible_group()
 
         # If this is a group, and it is the correct group, add the method.
         if isinstance(group, group_class) and group.group_name() == group_name:
-            group.AddMethod(self)
+            group.add_method(self)
             return self
 
         # Create a new group and add the method.
         new_group = group_class(group_name, self._exception_list)
-        new_group.AddMethod(self)
+        new_group.add_method(self)
         self._call_queue.append(new_group)
         return self
 
     def any_order(self, group_name="default"):
         """Move this method into a group of unordered calls.
 
         A group of unordered calls must be defined together, and must be
@@ -1443,945 +1278,7 @@
     GetPossibleGroup = get_possible_group
     _CheckAndCreateNewGroup = _check_and_create_new_group
     InAnyOrder = any_order
     MultipleTimes = multiple_times
     AndReturn = returns
     AndRaise = raises
     WithSideEffects = with_side_effects
-
-
-class Comparator:
-    """Base class for all Mox comparators.
-
-    A Comparator can be used as a parameter to a mocked method when the exact
-    value is not known.  For example, the code you are testing might build up a
-    long SQL string that is passed to your mock DAO. You're only interested
-    that the IN clause contains the proper primary keys, so you can set your
-    mock up as follows:
-
-    mock_dao.RunQuery(StrContains('IN (1, 2, 4, 5)')).AndReturn(mock_result)
-
-    Now whatever query is passed in must contain the string 'IN (1, 2, 4, 5)'.
-
-    A Comparator may replace one or more parameters, for example:
-    # return at most 10 rows
-    mock_dao.RunQuery(StrContains('SELECT'), 10)
-
-    or
-
-    # Return some non-deterministic number of rows
-    mock_dao.RunQuery(StrContains('SELECT'), IsA(int))
-    """
-
-    def equals(self, rhs):
-        """Special equals method that all comparators must implement.
-
-        Args:
-          rhs: any python object
-        """
-
-        raise NotImplementedError
-
-    def __eq__(self, rhs):
-        return self.equals(rhs)
-
-    def __ne__(self, rhs):
-        return not self.equals(rhs)
-
-
-class Is(Comparator):
-    """Comparison class used to check identity, instead of equality."""
-
-    def __init__(self, obj):
-        self._obj = obj
-
-    def equals(self, rhs):
-        return rhs is self._obj
-
-    def __repr__(self):
-        return "<is %r (%s)>" % (self._obj, id(self._obj))
-
-
-is_ = Is
-
-
-class IsA(Comparator):
-    """This class wraps a basic Python type or class.  It is used to verify
-    that a parameter is of the given type or class.
-
-    Example:
-    mock_dao.Connect(IsA(DbConnectInfo))
-    """
-
-    def __init__(self, class_name):
-        """Initialize IsA
-
-        Args:
-          class_name: basic python type or a class
-        """
-
-        self._class_name = class_name
-
-    def equals(self, rhs):
-        """Check to see if the RHS is an instance of class_name.
-
-        Args:
-          # rhs: the right hand side of the test
-          rhs: object
-
-        Returns:
-          bool
-        """
-
-        try:
-            return isinstance(rhs, self._class_name)
-        except TypeError:
-            # Check raw types if there was a type error.  This is helpful for
-            # things like cStringIO.StringIO.
-            return isinstance(rhs, type(self._class_name))
-
-    def _is_subclass(self, clazz):
-        """Check to see if the IsA comparators class is a subclass of clazz.
-
-        Args:
-          # clazz: a class object
-
-        Returns:
-          bool
-        """
-
-        try:
-            return issubclass(self._class_name, clazz)
-        except TypeError:
-            # Check raw types if there was a type error.  This is helpful for
-            # things like cStringIO.StringIO.
-            return isinstance(clazz, type(self._class_name))
-
-    def __repr__(self):
-        return "mox.IsA(%s) " % str(self._class_name)
-
-    _IsSubClass = _is_subclass
-
-
-is_a = IsA
-
-
-class IsAlmost(Comparator):
-    """Comparison class used to check whether a parameter is nearly equal
-    to a given value.  Generally useful for floating point numbers.
-
-    Example mock_dao.SetTimeout((IsAlmost(3.9)))
-    """
-
-    def __init__(self, float_value, places=7):
-        """Initialize IsAlmost.
-
-        Args:
-          float_value: The value for making the comparison.
-          places: The number of decimal places to round to.
-        """
-
-        self._float_value = float_value
-        self._places = places
-
-    def equals(self, rhs):
-        """Check to see if RHS is almost equal to float_value
-
-        Args:
-          rhs: the value to compare to float_value
-
-        Returns:
-          bool
-        """
-
-        try:
-            return round(rhs - self._float_value, self._places) == 0
-        except Exception:
-            # This is probably because either float_value or rhs is not a
-            # number.
-            return False
-
-    def __repr__(self):
-        return str(self._float_value)
-
-
-is_almost = IsAlmost
-
-
-class StrContains(Comparator):
-    """Comparison class used to check whether a substring exists in a
-    string parameter.  This can be useful in mocking a database with SQL
-    passed in as a string parameter, for example.
-
-    Example:
-    mock_dao.RunQuery(StrContains('IN (1, 2, 4, 5)')).AndReturn(mock_result)
-    """
-
-    def __init__(self, search_string):
-        """Initialize.
-
-        Args:
-          # search_string: the string you are searching for
-          search_string: str
-        """
-
-        self._search_string = search_string
-
-    def equals(self, rhs):
-        """Check to see if the search_string is contained in the rhs string.
-
-        Args:
-          # rhs: the right hand side of the test
-          rhs: object
-
-        Returns:
-          bool
-        """
-
-        try:
-            return rhs.find(self._search_string) > -1
-        except Exception:
-            return False
-
-    def __repr__(self):
-        return "<str containing '%s'>" % self._search_string
-
-
-str_contains = StrContains
-
-
-class Regex(Comparator):
-    """Checks if a string matches a regular expression.
-
-    This uses a given regular expression to determine equality.
-    """
-
-    def __init__(self, pattern, flags=0):
-        """Initialize.
-
-        Args:
-          # pattern is the regular expression to search for
-          pattern: str
-          # flags passed to re.compile function as the second argument
-          flags: int
-        """
-
-        self.regex = re.compile(pattern, flags=flags)
-
-    def equals(self, rhs):
-        """Check to see if rhs matches regular expression pattern.
-
-        Returns:
-          bool
-        """
-
-        try:
-            return self.regex.search(rhs) is not None
-        except Exception:
-            return False
-
-    def __repr__(self):
-        pattern = self.regex.pattern
-        if isinstance(pattern, bytes):
-            pattern = pattern.decode()
-        s = "<regular expression '{}'".format(pattern)
-        if self.regex.flags:
-            s += ", flags=%d" % self.regex.flags
-        s += ">"
-        return s
-
-
-regex = Regex
-
-
-class In(Comparator):
-    """Checks whether an item (or key) is in a list (or dict) parameter.
-
-    Example:
-    mock_dao.GetUsersInfo(In('expectedUserName')).AndReturn(mock_result)
-    """
-
-    def __init__(self, key):
-        """Initialize.
-
-        Args:
-          # key is anything that could be in a list or a key in a dict
-        """
-
-        self._key = key
-
-    def equals(self, rhs):
-        """Check to see whether key is in rhs.
-
-        Args:
-          rhs: dict
-
-        Returns:
-          bool
-        """
-
-        try:
-            return self._key in rhs
-        except Exception:
-            return False
-
-    def __repr__(self):
-        return "<sequence or map containing '%s'>" % str(self._key)
-
-
-in_ = In
-
-
-class Not(Comparator):
-    """Checks whether a predicates is False.
-
-    Example:
-      mock_dao.UpdateUsers(Not(ContainsKeyValue('stevepm', stevepm_user_info)))
-    """
-
-    def __init__(self, predicate):
-        """Initialize.
-
-        Args:
-          # predicate: a Comparator instance.
-        """
-
-        if not isinstance(predicate, Comparator):
-            raise Error("predicate %r must be a" " Comparator." % predicate)
-        self._predicate = predicate
-
-    def equals(self, rhs):
-        """Check to see whether the predicate is False.
-
-        Args:
-          rhs: A value that will be given in argument of the predicate.
-
-        Returns:
-          bool
-        """
-
-        try:
-            return not self._predicate.equals(rhs)
-        except Exception:
-            return False
-
-    def __repr__(self):
-        return "<not '%s'>" % self._predicate
-
-
-not_ = Not
-
-
-class ContainsKeyValue(Comparator):
-    """Checks whether a key/value pair is in a dict parameter.
-
-    Example:
-    mock_dao.UpdateUsers(ContainsKeyValue('stevepm', stevepm_user_info))
-    """
-
-    def __init__(self, key, value):
-        """Initialize.
-
-        Args:
-          # key: a key in a dict
-          # value: the corresponding value
-        """
-
-        self._key = key
-        self._value = value
-
-    def equals(self, rhs):
-        """Check whether the given key/value pair is in the rhs dict.
-
-        Returns:
-          bool
-        """
-
-        try:
-            return rhs[self._key] == self._value
-        except Exception:
-            return False
-
-    def __repr__(self):
-        return "<map containing the entry '%s: %s'>" % (
-            str(self._key),
-            str(self._value),
-        )
-
-
-contains_key_value = ContainsKeyValue
-
-
-class ContainsAttributeValue(Comparator):
-    """Checks whether a passed parameter contains attributes with a given
-    value.
-
-    Example:
-    mock_dao.UpdateSomething(ContainsAttribute('stevepm', stevepm_user_info))
-    """
-
-    def __init__(self, key, value):
-        """Initialize.
-
-        Args:
-          # key: an attribute name of an object
-          # value: the corresponding value
-        """
-
-        self._key = key
-        self._value = value
-
-    def equals(self, rhs):
-        """Check whether the given attribute has a matching value in the rhs
-        object.
-
-        Returns:
-          bool
-        """
-
-        try:
-            return getattr(rhs, self._key) == self._value
-        except Exception:
-            return False
-
-
-contains_attribute_value = ContainsAttributeValue
-
-
-class SameElementsAs(Comparator):
-    """Checks whether sequences contain the same elements (ignoring order).
-
-    Example:
-    mock_dao.ProcessUsers(SameElementsAs('stevepm', 'salomaki'))
-    """
-
-    def __init__(self, expected_seq):
-        """Initialize.
-
-        Args:
-          expected_seq: a sequence
-        """
-        # Store in case expected_seq is an iterator.
-        self._expected_list = list(expected_seq)
-
-    def equals(self, actual_seq):
-        """Check to see whether actual_seq has same elements as expected_seq.
-
-        Args:
-          actual_seq: sequence
-
-        Returns:
-          bool
-        """
-        try:
-            # Store in case actual_seq is an iterator.  We potentially iterate
-            # twice: once to make the dict, once in the list fallback.
-            actual_list = list(actual_seq)
-        except TypeError:
-            # actual_seq cannot be read as a sequence.
-            #
-            # This happens because Mox uses __eq__ both to check object
-            # equality (in MethodSignatureChecker) and to invoke Comparators.
-            return False
-
-        try:
-            expected = dict([(element, None) for element in self._expected_list])
-            actual = dict([(element, None) for element in actual_list])
-        except TypeError:
-            # Fall back to slower list-compare if any of the objects are
-            # unhashable.
-            expected = self._expected_list
-            actual = actual_list
-            for element in actual:
-                if element not in expected:
-                    return False
-            for element in expected:
-                if element not in actual:
-                    return False
-            return True
-        else:
-            return set(actual_list) == set(self._expected_list)
-
-    def __repr__(self):
-        return "<sequence with same elements as '%s'>" % self._expected_list
-
-
-same_elements_as = SameElementsAs
-
-
-class And(Comparator):
-    """Evaluates one or more Comparators on RHS and returns an AND of the
-    results.
-    """
-
-    def __init__(self, *args):
-        """Initialize.
-
-        Args:
-          *args: One or more Comparator
-        """
-
-        self._comparators = args
-
-    def equals(self, rhs):
-        """Checks whether all Comparators are equal to rhs.
-
-        Args:
-          # rhs: can be anything
-
-        Returns:
-          bool
-        """
-
-        for comparator in self._comparators:
-            if not comparator.equals(rhs):
-                return False
-
-        return True
-
-    def __repr__(self):
-        return "<AND %s>" % str(self._comparators)
-
-
-and_ = And
-
-
-class Or(Comparator):
-    """Evaluates one or more Comparators on RHS and returns an OR of the
-    results.
-    """
-
-    def __init__(self, *args):
-        """Initialize.
-
-        Args:
-          *args: One or more Mox comparators
-        """
-
-        self._comparators = args
-
-    def equals(self, rhs):
-        """Checks whether any Comparator is equal to rhs.
-
-        Args:
-          # rhs: can be anything
-
-        Returns:
-          bool
-        """
-
-        for comparator in self._comparators:
-            if comparator.equals(rhs):
-                return True
-
-        return False
-
-    def __repr__(self):
-        return "<OR %s>" % str(self._comparators)
-
-
-or_ = Or
-
-
-class Func(Comparator):
-    """Call a function that should verify the parameter passed in is correct.
-
-    You may need the ability to perform more advanced operations on the
-    parameter in order to validate it.  You can use this to have a callable
-    validate any parameter. The callable should return either True or False.
-
-
-    Example:
-
-    def myParamValidator(param):
-      # Advanced logic here
-      return True
-
-    mock_dao.DoSomething(Func(myParamValidator), true)
-    """
-
-    def __init__(self, func):
-        """Initialize.
-
-        Args:
-          func: callable that takes one parameter and returns a bool
-        """
-
-        self._func = func
-
-    def equals(self, rhs):
-        """Test whether rhs passes the function test.
-
-        rhs is passed into func.
-
-        Args:
-          rhs: any python object
-
-        Returns:
-          the result of func(rhs)
-        """
-
-        return self._func(rhs)
-
-    def __repr__(self):
-        return str(self._func)
-
-
-func = Func
-
-
-class IgnoreArg(Comparator):
-    """Ignore an argument.
-
-    This can be used when we don't care about an argument of a method call.
-
-    Example:
-    # Check if CastMagic is called with 3 as first arg and 'disappear' as
-    third. mymock.CastMagic(3, IgnoreArg(), 'disappear')
-    """
-
-    def equals(self, unused_rhs):
-        """Ignores arguments and returns True.
-
-        Args:
-          unused_rhs: any python object
-
-        Returns:
-          always returns True
-        """
-
-        return True
-
-    def __repr__(self):
-        return "<IgnoreArg>"
-
-
-ignore_arg = IgnoreArg
-
-
-class Value(Comparator):
-    """Compares argument against a remembered value.
-
-    To be used in conjunction with Remember comparator.  See Remember()
-    for example.
-    """
-
-    def __init__(self):
-        self._value = None
-        self._has_value = False
-
-    def store_value(self, rhs):
-        self._value = rhs
-        self._has_value = True
-
-    def equals(self, rhs):
-        if not self._has_value:
-            return False
-        else:
-            return rhs == self._value
-
-    def __repr__(self):
-        if self._has_value:
-            return "<Value %r>" % self._value
-        else:
-            return "<Value>"
-
-
-value = Value
-
-
-class Remember(Comparator):
-    """Remembers the argument to a value store.
-
-    To be used in conjunction with Value comparator.
-
-    Example:
-    # Remember the argument for one method call.
-    users_list = Value()
-    mock_dao.ProcessUsers(Remember(users_list))
-
-    # Check argument against remembered value.
-    mock_dao.ReportUsers(users_list)
-    """
-
-    def __init__(self, value_store):
-        if not isinstance(value_store, Value):
-            raise TypeError("value_store is not an instance of the Value class")
-        self._value_store = value_store
-
-    def equals(self, rhs):
-        self._value_store.store_value(rhs)
-        return True
-
-    def __repr__(self):
-        return "<Remember %d>" % id(self._value_store)
-
-
-remember = Remember
-
-
-class MethodGroup(object):
-    """Base class containing common behaviour for MethodGroups."""
-
-    def __init__(self, group_name, exception_list):
-        """Construct a new method group.
-
-        Args:
-          # group_name: the name of the method group
-          # exception_list: list of exceptions; any exceptions thrown by this
-          #     instance are appended to this list.
-          group_name: str
-          exception_list: list
-        """
-        self._group_name = group_name
-        self._exception_list = exception_list
-
-    def group_name(self):
-        return self._group_name
-
-    def __str__(self):
-        return '<%s "%s">' % (self.__class__.__name__, self._group_name)
-
-    def add_method(self, mock_method):
-        raise NotImplementedError
-
-    def method_called(self, mock_method):
-        raise NotImplementedError
-
-    def is_satisfied(self):
-        raise NotImplementedError
-
-    AddMethod = add_method
-    MethodCalled = method_called
-    IsSatisfied = is_satisfied
-
-
-class UnorderedGroup(MethodGroup):
-    """UnorderedGroup holds a set of method calls that may occur in any order.
-
-    This construct is helpful for non-deterministic events, such as iterating
-    over the keys of a dict.
-    """
-
-    def __init__(self, group_name, exception_list):
-        super(UnorderedGroup, self).__init__(group_name, exception_list)
-        self._methods = []
-
-    def __str__(self):
-        return '%s "%s" pending calls:\n%s' % (
-            self.__class__.__name__,
-            self._group_name,
-            "\n".join(str(method) for method in self._methods),
-        )
-
-    def add_method(self, mock_method):
-        """Add a method to this group.
-
-        Args:
-          mock_method: A mock method to be added to this group.
-        """
-
-        self._methods.append(mock_method)
-
-    def method_called(self, mock_method):
-        """Remove a method call from the group.
-
-        If the method is not in the set, an UnexpectedMethodCallError will be
-        raised.
-
-        Args:
-          mock_method: a mock method that should be equal to a method in the
-          group.
-
-        Returns:
-          The mock method from the group
-
-        Raises:
-          UnexpectedMethodCallError if the mock_method was not in the group.
-        """
-
-        # Check to see if this method exists, and if so, remove it from the set
-        # and return it.
-        for method in self._methods:
-            if method == mock_method:
-                # Remove the called mock_method instead of the method in the
-                # group. The called method will match any comparators when
-                # equality is checked during removal. The method in the group
-                # could pass a comparator to another comparator during the
-                # equality check.
-                self._methods.remove(mock_method)
-
-                # If this group is not empty, put it back at the head of the
-                # queue.
-                if not self.IsSatisfied():
-                    mock_method._call_queue.appendleft(self)
-
-                return self, method
-
-        exception = UnexpectedMethodCallError(mock_method, self)
-        self._exception_list.append(exception)
-        raise exception
-
-    def is_satisfied(self):
-        """Return True if there are not any methods in this group."""
-
-        return len(self._methods) == 0
-
-    AddMethod = add_method
-    MethodCalled = method_called
-    IsSatisfied = is_satisfied
-
-
-class MultipleTimesGroup(MethodGroup):
-    """MultipleTimesGroup holds methods that may be called any number of times.
-
-    Note: Each method must be called at least once.
-
-    This is helpful, if you don't know or care how many times a method is
-    called.
-    """
-
-    def __init__(self, group_name, exception_list):
-        super(MultipleTimesGroup, self).__init__(group_name, exception_list)
-        self._methods = set()
-        self._methods_left = set()
-
-    def add_method(self, mock_method):
-        """Add a method to this group.
-
-        Args:
-          mock_method: A mock method to be added to this group.
-        """
-
-        self._methods.add(mock_method)
-        self._methods_left.add(mock_method)
-
-    def method_called(self, mock_method):
-        """Remove a method call from the group.
-
-        If the method is not in the set, an UnexpectedMethodCallError will be
-        raised.
-
-        Args:
-          mock_method: a mock method that should be equal to a method in the
-            group.
-
-        Returns:
-          The mock method from the group
-
-        Raises:
-          UnexpectedMethodCallError if the mock_method was not in the group.
-        """
-
-        # Check to see if this method exists, and if so add it to the set of
-        # called methods.
-        for method in self._methods:
-            if method == mock_method:
-                self._methods_left.discard(method)
-                # Always put this group back on top of the queue, because we
-                # don't know when we are done.
-                mock_method._call_queue.appendleft(self)
-                return self, method
-
-        if self.IsSatisfied():
-            next_method = mock_method._PopNextMethod()
-            return next_method, None
-        else:
-            exception = UnexpectedMethodCallError(mock_method, self)
-            self._exception_list.append(exception)
-            raise exception
-
-    def is_satisfied(self):
-        """Return True if all methods in this group are called at least once."""
-        return len(self._methods_left) == 0
-
-    AddMethod = add_method
-    MethodCalled = method_called
-    IsSatisfied = is_satisfied
-
-
-class MoxMetaTestBase(type):
-    """Metaclass to add mox cleanup and verification to every test.
-    As the mox unit testing class is being constructed (MoxTestBase or a
-    subclass), this metaclass will modify all test functions to call the
-    CleanUpMox method of the test class after they finish. This means that
-    unstubbing and verifying will happen for every test with no additional
-    code, and any failures will result in test failures as opposed to errors.
-    """
-
-    def __init__(cls, name, bases, d):
-        super().__init__(name, bases, d)
-        # type.__init__(cls, name, bases, d)
-
-        # also get all the attributes from the base classes to account
-        # for a case when test class is not the immediate child of MoxTestBase
-        for base in bases:
-            for attr_name in dir(base):
-                if attr_name not in d:
-                    try:  # pragma: nocover
-                        d[attr_name] = getattr(base, attr_name)
-                    except AttributeError:
-                        continue
-
-        for func_name, func in d.items():
-            if func_name.startswith("test") and callable(func):
-                setattr(cls, func_name, MoxMetaTestBase.clean_up_test(cls, func))
-
-    @staticmethod
-    def clean_up_test(cls, func):
-        """Adds Mox cleanup code to any MoxTestBase method.
-        Always unsets stubs after a test. Will verify all mocks for tests that
-        otherwise pass.
-        Args:
-          cls: MoxTestBase or subclass; the class whose test method we are
-            altering.
-          func: method; the method of the MoxTestBase test class we wish to
-            alter.
-        Returns:
-          The modified method.
-        """
-
-        def new_method(self, *args, **kwargs):
-            mox_obj = getattr(self, "mox", None)
-            stubout_obj = getattr(self, "stubs", None)
-            cleanup_mox = False
-            cleanup_stubout = False
-            if mox_obj and isinstance(mox_obj, Mox):
-                cleanup_mox = True
-            if stubout_obj and isinstance(stubout_obj, stubout.StubOutForTesting):
-                cleanup_stubout = True
-            try:
-                func(self, *args, **kwargs)
-            finally:
-                if cleanup_mox:
-                    mox_obj.UnsetStubs()
-                if cleanup_stubout:
-                    stubout_obj.UnsetAll()
-                    stubout_obj.SmartUnsetAll()
-            if cleanup_mox:
-                mox_obj.VerifyAll()
-
-        new_method.__name__ = func.__name__
-        new_method.__doc__ = func.__doc__
-        new_method.__module__ = func.__module__
-        return new_method
-
-    CleanUpTest = clean_up_test
-
-
-_MoxTestBase = MoxMetaTestBase("_MoxTestBase", (unittest.TestCase,), {})
-
-
-class MoxTestBase(_MoxTestBase):
-    # class MoxTestBase(unittest.TestCase, metaclass=MoxMetaTestBase):
-    """Convenience test class to make stubbing easier.
-    Sets up a "mox" attribute which is an instance of Mox (any mox tests will
-    want this), and a "stubs" attribute that is an instance of
-    StubOutForTesting (needed at times). Also automatically unsets any stubs
-    and verifies that all mock methods have been called at the end of each
-    test, eliminating boilerplate code.
-    """
-
-    def setUp(self):
-        super(MoxTestBase, self).setUp()
-        self.mox = Mox()
-        self.stubs = stubout.StubOutForTesting()
```

### Comparing `pymox-1.0.2/mox/stubout.py` & `pymox-1.1.0/mox/stubout.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+# Python imports
 import inspect
 
 
 class StubOutForTesting:
     """Sample Usage:
     You want os.path.exists() to always return true during testing.
 
@@ -146,8 +147,8 @@
 
     SmartSet = smart_set
     SmartUnsetAll = smart_unset_all
     Set = set
     UnsetAll = unset_all
 
 
-stubout = StubOutForTesting()
+stubout = StubOutForTesting
```

### Comparing `pymox-1.0.2/pyproject.toml` & `pymox-1.1.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -6,29 +6,27 @@
 name = "pymox"
 dynamic = ["version"]
 
 [tool.poetry]
 name = "pymox"
 description = "Mock object framework"
 packages = [{include = "mox"}]
-version = "1.0.2"
+version = "1.1.0"
 authors = ["Ivan Neto <ivan.cr.neto@gmail.com>"]
 license = "Apache License, Version 2.0"
 homepage = "http://pymox.rtfd.io"
 repository = "https://github.com/ivancrneto/pymox"
 classifiers = [
     "Environment :: Console",
     "Development Status :: 5 - Production/Stable",
     "Framework :: Pytest",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
-    "Programming Language :: Python :: 3.3",
-    "Programming Language :: Python :: 3.4",
     "Programming Language :: Python :: 3.5",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
@@ -73,7 +71,37 @@
     ".coveragerc",
     "--cov=mox",
     "--cov-branch",
     "--cov-report",
     "term-missing",
     "test/mox_test.py"
 ]
+
+
+[tool.black]
+line-length = 120
+target-version = [ "py35" ]
+
+
+[tool.isort]
+atomic = true
+case_sensitive = true
+filter_files = true
+import_heading_firstparty = "Internal imports"
+import_heading_stdlib = "Python imports"
+import_heading_thirdparty = "Pip imports"
+known_startup = [
+  "startup",
+]
+line_length = 120
+lines_after_imports = 2
+profile = "black"
+py_version = "auto"
+remove_redundant_aliases = true
+sections = [
+  "FUTURE",
+  "STARTUP",
+  "STDLIB",
+  "THIRDPARTY",
+  "FIRSTPARTY",
+  "LOCALFOLDER",
+]
```

### Comparing `pymox-1.0.2/PKG-INFO` & `pymox-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymox
-Version: 1.0.2
+Version: 1.1.0
 Summary: Mock object framework
 Home-page: http://pymox.rtfd.io
 License: Apache License, Version 2.0
 Keywords: mox,mock,test,mocking,unittest,pymox
 Author: Ivan Neto
 Author-email: ivan.cr.neto@gmail.com
 Requires-Python: >=3.3,<4
@@ -23,16 +23,14 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
@@ -207,39 +205,39 @@
 ~~~~~~~~~~~
 
 You can use comparators when you are unsure of the arguments of a method
 call.
 
 .. code:: python
 
-       def test_quack_7(self):  
+       def test_quack_7(self):
            m = mox.Mox()
            duck = Duck()
-           
+
            m.stubout(Duck, 'quack')
-           
+
            def validate_arg(arg):
             if arg in [1, 2, 3]:
              return True
             return False
-           
+
            duck.quack(times=mox.is_a(int)).returns(['new quack'])
            duck.quack(times=mox.not_(mox.is_(4))).returns(['new quack'])
            duck.quack(times=mox.func(validate_arg)).returns(['new quack'])
            duck.quack(times=mox.or_(mox.Is(1), mox.is_(2), mox.is_(3))).returns(['new quack'])
-           
+
            duck.quack(times=mox.ignore_arg()).returns(['new quack'])
            duck.quack(times=mox.is_almost(1.00003, places=4)).returns(['new quack'])
-           
+
            m.replay_all()
            assert duck.quack(times=random.choice([1, 2, 3])) == ['new quack']
            assert duck.quack(times=random.choice([1, 2, 3])) == mox.in_('new quack')
            assert duck.quack(times=random.choice([1, 2, 3]))[0] == mox.str_contains('quack')
            assert duck.quack(times=random.choice([1, 2, 3])) == mox.same_elements_as({'new quack'})
-           
+
            assert duck.quack(times=random.choice([1, 2, 3])) == ['new quack']
            assert duck.quack(times=1) == ['new quack']
            m.verify_all()
 
 All the assertions for the test above should pass. There are other cool
 comparators, like: ``and``, ``contains_attribute_value``,
 ``contains_key_value``.
@@ -267,15 +265,15 @@
                        choices.pop()
                    self._do_quack(choices=choices)
 
            m = mox.Mox()
            duck = StopQuackingDuck()
 
            m.stubout(StopQuackingDuck, '_do_quack')
-           
+
            choices_1 = mox.value()
            choices_2 = mox.value()
            duck._do_quack(choices=mox.remember(choices_1))
            duck._do_quack(choices=mox.remember(choices_2))
            duck._do_quack(choices=mox.remember(choices_2))
            duck._do_quack(choices=mox.remember(choices_2))
```

