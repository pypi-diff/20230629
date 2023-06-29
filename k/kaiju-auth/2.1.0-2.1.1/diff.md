# Comparing `tmp/kaiju_auth-2.1.0-py3-none-any.whl.zip` & `tmp/kaiju_auth-2.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 16207 bytes, number of entries: 11
--rw-r--r--  2.0 unx       93 b- defN 23-Jun-27 19:26 kaiju_auth/__init__.py
--rw-r--r--  2.0 unx    39292 b- defN 23-Jun-27 19:26 kaiju_auth/services.py
--rw-r--r--  2.0 unx       55 b- defN 23-Jun-27 19:26 kaiju_auth/permissions_gui/__init__.py
--rw-r--r--  2.0 unx     3228 b- defN 23-Jun-27 19:26 kaiju_auth/permissions_gui/models.py
--rw-r--r--  2.0 unx    18327 b- defN 23-Jun-27 19:26 kaiju_auth/permissions_gui/service.py
--rw-r--r--  2.0 unx     1212 b- defN 23-Jun-27 19:26 kaiju_auth/permissions_gui/validators.py
--rw-rw-rw-  2.0 unx      610 b- defN 23-Jun-27 19:26 kaiju_auth-2.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     2987 b- defN 23-Jun-27 19:26 kaiju_auth-2.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-27 19:26 kaiju_auth-2.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jun-27 19:26 kaiju_auth-2.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      935 b- defN 23-Jun-27 19:26 kaiju_auth-2.1.0.dist-info/RECORD
-11 files, 66842 bytes uncompressed, 14611 bytes compressed:  78.1%
+Zip file size: 16219 bytes, number of entries: 11
+-rw-r--r--  2.0 unx       93 b- defN 23-Jun-29 12:35 kaiju_auth/__init__.py
+-rw-r--r--  2.0 unx    39335 b- defN 23-Jun-29 12:35 kaiju_auth/services.py
+-rw-r--r--  2.0 unx       55 b- defN 23-Jun-29 12:35 kaiju_auth/permissions_gui/__init__.py
+-rw-r--r--  2.0 unx     3228 b- defN 23-Jun-29 12:35 kaiju_auth/permissions_gui/models.py
+-rw-r--r--  2.0 unx    18327 b- defN 23-Jun-29 12:35 kaiju_auth/permissions_gui/service.py
+-rw-r--r--  2.0 unx     1212 b- defN 23-Jun-29 12:35 kaiju_auth/permissions_gui/validators.py
+-rw-rw-rw-  2.0 unx      610 b- defN 23-Jun-29 12:36 kaiju_auth-2.1.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2987 b- defN 23-Jun-29 12:36 kaiju_auth-2.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-29 12:36 kaiju_auth-2.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-29 12:36 kaiju_auth-2.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      935 b- defN 23-Jun-29 12:36 kaiju_auth-2.1.1.dist-info/RECORD
+11 files, 66885 bytes uncompressed, 14623 bytes compressed:  78.1%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: kaiju_auth/permissions_gui/service.py
 Comment: 
 
 Filename: kaiju_auth/permissions_gui/validators.py
 Comment: 
 
-Filename: kaiju_auth-2.1.0.dist-info/LICENSE
+Filename: kaiju_auth-2.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: kaiju_auth-2.1.0.dist-info/METADATA
+Filename: kaiju_auth-2.1.1.dist-info/METADATA
 Comment: 
 
-Filename: kaiju_auth-2.1.0.dist-info/WHEEL
+Filename: kaiju_auth-2.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: kaiju_auth-2.1.0.dist-info/top_level.txt
+Filename: kaiju_auth-2.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: kaiju_auth-2.1.0.dist-info/RECORD
+Filename: kaiju_auth-2.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kaiju_auth/__init__.py

```diff
@@ -1,4 +1,4 @@
 from kaiju_auth.services import *
 
-__version__ = '2.1.0'
+__version__ = '2.1.1'
 __author__ = 'antonnidhoggr@me.com'
```

## kaiju_auth/services.py

```diff
@@ -43,15 +43,15 @@
 
     id: str
     enabled: bool
     tag: str
     description: str
 
 
-class PermissionService(SQLService, ContextableService, PublicInterface):
+class PermissionService(SQLService[str, Permission], ContextableService, PublicInterface):
     """Service which stores user permission keys and information about them."""
 
     class _TaggedPermissions(TypedDict):
         tag: Optional[str]
         permissions: List[dict]
 
     table = sa.Table(
@@ -114,15 +114,15 @@
     """User group object."""
 
     id: str
     tag: str
     description: str
 
 
-class GroupService(SQLService, ContextableService, PublicInterface):
+class GroupService(SQLService[str, Group], ContextableService, PublicInterface):
     """User groups and their permissions."""
 
     class _GroupPermissions(TypedDict):
         id: str
         permissions: FrozenSet[str]
 
     table = sa.Table(
@@ -181,15 +181,15 @@
             'permissions.update': self.modify_permissions,
         }
 
     async def init(self):
         self._permission_service = self.discover_service(self._permission_service, cls=self.permission_service_class)
         self.permissions_table = self._permission_service.table
 
-    async def get_permissions(self, id) -> Union[frozenset, List[_GroupPermissions]]:
+    async def get_permissions(self, id: Union[str, Collection[str]]) -> Union[frozenset, List[_GroupPermissions]]:
         """Return group(s) permissions. Non-active permission keys will be ignored.
 
         :param id: group identifier
         :returns: a set of permissions
         """
         if isinstance(id, Collection) and not type(id) is str:
             if not id:
@@ -232,15 +232,15 @@
                 )
             )
             rows = await self._db.fetch(sql)
             result = frozenset(row['permission_id'] for row in rows)
 
         return result
 
-    async def set_permissions(self, id, permissions: list) -> frozenset:
+    async def set_permissions(self, id: str, permissions: Collection[str]) -> frozenset:
         """Set permissions in the group.
 
         All non-mentioned permissions will be removed.
 
         :param id: group identifier
         :param permissions: a list of permissions
         :returns: a new set of available permissions
@@ -265,15 +265,15 @@
                 [{'group_id': id, 'permission_id': key} for key in _to_add]
             )
             tasks.append(self._db.execute(sql))
 
         await asyncio.gather(*tasks)
         return frozenset(permissions)
 
-    async def modify_permissions(self, id, permissions: Dict[str, bool]) -> frozenset:
+    async def modify_permissions(self, id: str, permissions: Dict[str, bool]) -> frozenset:
         """Modify permissions in a group.
 
         .. code-block:: python
 
             await groups.modify_permissions('users', {'do.this': True, 'do.that': False})
 
         :param id: group identifier
@@ -335,15 +335,15 @@
     salt: bytes
     is_active: bool
     is_blocked: bool
     settings: dict
     created: datetime
 
 
-class UserService(SQLService, ContextableService, PublicInterface, UserInterface):
+class UserService(SQLService[uuid.UUID, User], ContextableService, PublicInterface, UserInterface):
     """Information about users and user groups."""
 
     class ErrorCode:
         """User service error codes."""
 
         RPC_PERMISSION_DENIED = 'auth.rpc.permission_denied'
 
@@ -512,28 +512,28 @@
     async def get_default_nonlogin_permissions(self) -> frozenset:
         """Return a set of guest user permissions."""
         if self._default_nonlogin_group:
             return await self._group_service.get_permissions(self._default_nonlogin_group)
         else:
             return frozenset()
 
-    async def get_user_groups(self, id) -> _UserGroups:
+    async def get_user_groups(self, id: uuid.UUID) -> _UserGroups:
         """Return a list of groups of a user."""
         sql = (
             self.user_groups_table.select()
             .with_only_columns(*[self.user_groups_table.c.group_id])
             .where(self.user_groups_table.c.user_id == id)
         )
         rows = await self._db.fetch(sql)
         _groups = list(row['group_id'] for row in rows)
         if not _groups and self._default_group:
             _groups = [self._default_group]
         return {'id': id, 'groups': _groups}
 
-    async def set_user_groups(self, id, groups: list):
+    async def set_user_groups(self, id: uuid.UUID, groups: Collection[str]):
         """Set groups for a user. All non-mentioned groups will be removed."""
         _groups = set(groups)
         _existing_groups = await self.get_user_groups(id)
         _existing_groups = set(_existing_groups['groups'])
         _to_delete = _existing_groups.difference(_groups)
         _to_add = _groups.difference(_existing_groups)
         tasks = []
@@ -546,15 +546,15 @@
 
         if _to_add:
             sql = self.user_groups_table.insert().values([{'user_id': id, 'group_id': key} for key in _to_add])
             tasks.append(self._db.execute(sql))
 
         await asyncio.gather(*tasks)
 
-    async def modify_user_groups(self, id, groups: Dict[str, bool]) -> _UserGroups:
+    async def modify_user_groups(self, id: uuid.UUID, groups: Dict[str, bool]) -> _UserGroups:
         """Modify user groups."""
         if not groups:
             return await self.get_user_groups(id)
 
         keys = list(groups.keys())
         sql = (
             self.user_groups_table.select()
@@ -585,27 +585,27 @@
                 sa.and_(self.user_groups_table.c.user_id == id, self.user_groups_table.c.group_id.in_(to_remove))
             )
             tasks.append(self._db.execute(sql))
 
         await asyncio.gather(*tasks)
         return await self.get_user_groups(id)
 
-    async def get_user_permissions(self, id) -> _UserPermissions:
+    async def get_user_permissions(self, id: uuid.UUID) -> _UserPermissions:
         """Get user permissions."""
         _groups = await self.get_user_groups(id)
         if _groups:
             _permissions = await self._group_service.get_permissions(_groups['groups'])
             _permissions = set().union(*(_group['permissions'] for _group in _permissions))
             _permissions = frozenset(_permissions)
         else:
             _permissions = frozenset()
 
         return {'id': id, 'permissions': _permissions}
 
-    async def register(self, username: str, email: str, password: str, columns='*', settings: dict = None):
+    async def register(self, username: str, email: str, password: str, settings: dict = None) -> User:
         """Add a new user. Used by administrators or user managers."""
         self.validate_username(username)
         self.validate_email(email)
         password = self.validate_password(password)
 
         sql = self.table.select().where(sa.or_(self.table.c.username == username, self.table.c.email == email))
 
@@ -622,29 +622,29 @@
         settings['username'] = username
         settings['email'] = email
         settings['password'] = password
         settings['salt'] = salt
         settings['id'] = uuid.uuid4()
         sql = self.table.insert().values(settings)
         await self._db.execute(sql)
-        return await self._get_user_and_permissions(settings['id'], columns)
+        return await self._get_user_and_permissions(settings['id'])
 
     async def update_profile(self, id: uuid.UUID, settings: dict):
         data = await self.get(id, columns=['settings'])
         meta = data['settings']
         for key, value in settings.items():
             if value is None:
                 if key in meta:
                     del meta[key]
             else:
                 meta[key] = value
         await self.update(id, {'settings': meta})
         return {'id': id, 'settings': meta}
 
-    async def auth(self, username: str, password: str, columns='*'):
+    async def auth(self, username: str, password: str) -> Optional[User]:
         """Get user authorization."""
         sql = (
             self.table.select()
             .with_only_columns(*[self.table.c.id, self.table.c.password, self.table.c.salt])
             .where(
                 sa.and_(
                     self.table.c.username == username,
@@ -659,15 +659,15 @@
             return
             # raise NotAuthorized('User authentication failed.', code=self.ErrorCode.USER_AUTH_FAILED)
 
         if not self._check_password(username, password, user['salt'], user['password']):
             return
             # raise NotAuthorized('User authentication failed.', code=self.ErrorCode.USER_AUTH_FAILED)
 
-        return await self._get_user_and_permissions(user['id'], columns)
+        return await self._get_user_and_permissions(user['id'])
 
     async def change_password(self, username: str, password: str, new_password: str):
 
         if password == new_password:
             raise ValidationError(
                 'Old password matches the new one.', code=self.ErrorCode.USER_IDENTICAL_PASSWORDS_SUPPLIED
             )
@@ -735,19 +735,16 @@
 
     def _get_timeout(self):
         return random.random() * self.bad_password_timeout_jitter + self.bad_password_timeout
 
     def process_update_data(self, password=None, salt=None, created=None, id=None, **data):
         return data
 
-    async def _get_user_and_permissions(self, id, columns='*'):
-        if columns:
-            user = await self.get(id, columns=columns)
-        else:
-            user = {'id': id}
+    async def _get_user_and_permissions(self, id) -> dict:
+        user = await self.get(id)
         _permissions = await self.get_user_permissions(id)
         return {**user, 'permissions': _permissions['permissions']}
 
 
 class JWTClientService(TokenClientService):
     """JWT client which renews tokens automatically."""
```

## Comparing `kaiju_auth-2.1.0.dist-info/LICENSE` & `kaiju_auth-2.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `kaiju_auth-2.1.0.dist-info/METADATA` & `kaiju_auth-2.1.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaiju-auth
-Version: 2.1.0
+Version: 2.1.1
 Summary: Authentication services.
 Home-page: https://gitlab.com/kaiju-python/kaiju-auth
 Author: antonnidhoggr@me.com
 Author-email: antonnidhoggr@me.com
 License: Apache Software License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
```

## Comparing `kaiju_auth-2.1.0.dist-info/RECORD` & `kaiju_auth-2.1.1.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-kaiju_auth/__init__.py,sha256=0CItXnOnes0agKFUQmTYbi9belogs4uDGRma8z17i0g,93
-kaiju_auth/services.py,sha256=sQLRSZuY2_LlAClAuELsijJ5HE8YaWvnWZi5NUWYsXs,39292
+kaiju_auth/__init__.py,sha256=A_fVZ_iy87sOrFtMADVKbgmqvQDiWAE5mPgi1UdmPgQ,93
+kaiju_auth/services.py,sha256=E66pMoXqjTwisstt2qG67AgsKCZ6uNTAuHNjV-iVY98,39335
 kaiju_auth/permissions_gui/__init__.py,sha256=8Bxbwkjqk5QjDlZyXQ7R8dWLajhggp8of-yeZPz_pN0,55
 kaiju_auth/permissions_gui/models.py,sha256=JJFA7O1W-TaiJjVG1XgRKlhm92c0RRi4KJzFqKCXcWQ,3228
 kaiju_auth/permissions_gui/service.py,sha256=-zq5O6XhkF5wV7cRHHZBvpbdNZwOGyrzdkzlxWk2GOY,18327
 kaiju_auth/permissions_gui/validators.py,sha256=sytK30UHT8fg_SI5DaQRlsp1dEuyAholiOgF7fICp1I,1212
-kaiju_auth-2.1.0.dist-info/LICENSE,sha256=XIlN2qA8UqpBDA-PteoYP4hTU0qBW0G9PRB__khO2zc,610
-kaiju_auth-2.1.0.dist-info/METADATA,sha256=RRLlbYhJK-pFos9dh2a4lFG6KHs3Z16m15BweZBpHQQ,2987
-kaiju_auth-2.1.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-kaiju_auth-2.1.0.dist-info/top_level.txt,sha256=5F9g7EZLuzcI4ioeLmgI2Pp_r2yuzykkUc5L7lcUl2I,11
-kaiju_auth-2.1.0.dist-info/RECORD,,
+kaiju_auth-2.1.1.dist-info/LICENSE,sha256=XIlN2qA8UqpBDA-PteoYP4hTU0qBW0G9PRB__khO2zc,610
+kaiju_auth-2.1.1.dist-info/METADATA,sha256=iBCvrS6jJPzOpxsfvB3aRchZbA7P1qrQPkQSea3Xz5M,2987
+kaiju_auth-2.1.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+kaiju_auth-2.1.1.dist-info/top_level.txt,sha256=5F9g7EZLuzcI4ioeLmgI2Pp_r2yuzykkUc5L7lcUl2I,11
+kaiju_auth-2.1.1.dist-info/RECORD,,
```

