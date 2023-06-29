# Comparing `tmp/globox-2.1.3b0.tar.gz` & `tmp/globox-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "globox-2.1.3b0.tar", max compression
+gzip compressed data, was "globox-2.2.0.tar", max compression
```

## Comparing `globox-2.1.3b0.tar` & `globox-2.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     9236 2023-05-26 20:44:52.964782 globox-2.1.3b0/README.md
--rw-r--r--   0        0        0     1042 2023-05-26 20:44:52.964782 globox-2.1.3b0/pyproject.toml
--rw-r--r--   0        0        0      273 2023-05-26 20:44:52.968782 globox-2.1.3b0/src/globox/__init__.py
--rw-r--r--   0        0        0       30 2023-05-26 20:44:52.968782 globox-2.1.3b0/src/globox/__main__.py
--rw-r--r--   0        0        0    18551 2023-05-26 20:44:52.968782 globox-2.1.3b0/src/globox/annotation.py
--rw-r--r--   0        0        0    33312 2023-05-26 20:44:52.968782 globox-2.1.3b0/src/globox/annotationset.py
--rw-r--r--   0        0        0     1015 2023-05-26 20:44:52.968782 globox-2.1.3b0/src/globox/atomic.py
--rw-r--r--   0        0        0    17250 2023-05-26 20:44:52.968782 globox-2.1.3b0/src/globox/boundingbox.py
--rw-r--r--   0        0        0    14247 2023-05-26 20:44:52.968782 globox-2.1.3b0/src/globox/cli.py
--rw-r--r--   0        0        0      539 2023-05-26 20:44:52.968782 globox-2.1.3b0/src/globox/errors.py
--rw-r--r--   0        0        0    21347 2023-05-26 20:44:52.968782 globox-2.1.3b0/src/globox/evaluation.py
--rw-r--r--   0        0        0      699 2023-05-26 20:44:52.968782 globox-2.1.3b0/src/globox/file_utils.py
--rw-r--r--   0        0        0     6983 2023-05-26 20:44:52.968782 globox-2.1.3b0/src/globox/image_utils.py
--rw-r--r--   0        0        0      880 2023-05-26 20:44:52.968782 globox-2.1.3b0/src/globox/thread_utils.py
--rw-r--r--   0        0        0      747 2023-05-26 20:44:52.968782 globox-2.1.3b0/src/globox/utils.py
--rw-r--r--   0        0        0    10289 1970-01-01 00:00:00.000000 globox-2.1.3b0/PKG-INFO
+-rw-r--r--   0        0        0     9236 2023-06-29 20:59:14.310527 globox-2.2.0/README.md
+-rw-r--r--   0        0        0     1085 2023-06-29 20:59:14.310527 globox-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0      273 2023-06-29 20:59:14.310527 globox-2.2.0/src/globox/__init__.py
+-rw-r--r--   0        0        0       30 2023-06-29 20:59:14.310527 globox-2.2.0/src/globox/__main__.py
+-rw-r--r--   0        0        0    20545 2023-06-29 20:59:14.310527 globox-2.2.0/src/globox/annotation.py
+-rw-r--r--   0        0        0    35767 2023-06-29 20:59:14.310527 globox-2.2.0/src/globox/annotationset.py
+-rw-r--r--   0        0        0     1015 2023-06-29 20:59:14.310527 globox-2.2.0/src/globox/atomic.py
+-rw-r--r--   0        0        0    20920 2023-06-29 20:59:14.310527 globox-2.2.0/src/globox/boundingbox.py
+-rw-r--r--   0        0        0    14350 2023-06-29 20:59:14.310527 globox-2.2.0/src/globox/cli.py
+-rw-r--r--   0        0        0      492 2023-06-29 20:59:14.310527 globox-2.2.0/src/globox/errors.py
+-rw-r--r--   0        0        0    23244 2023-06-29 20:59:14.310527 globox-2.2.0/src/globox/evaluation.py
+-rw-r--r--   0        0        0      720 2023-06-29 20:59:14.310527 globox-2.2.0/src/globox/file_utils.py
+-rw-r--r--   0        0        0     6983 2023-06-29 20:59:14.310527 globox-2.2.0/src/globox/image_utils.py
+-rw-r--r--   0        0        0      880 2023-06-29 20:59:14.310527 globox-2.2.0/src/globox/thread_utils.py
+-rw-r--r--   0        0        0      747 2023-06-29 20:59:14.310527 globox-2.2.0/src/globox/utils.py
+-rw-r--r--   0        0        0    10287 1970-01-01 00:00:00.000000 globox-2.2.0/PKG-INFO
```

### Comparing `globox-2.1.3b0/README.md` & `globox-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `globox-2.1.3b0/pyproject.toml` & `globox-2.2.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "globox"
-version = "2.1.3-beta"
+version = "2.2.0"
 authors = ["Louis Lac <lac.louis5@gmail.com>"]
 license = "MIT"
 packages = [{include = "globox", from = "src"}]
 readme = "README.md"
 description = "Globox is a package and command line interface to read and convert object detection databases (COCO, YOLO, PascalVOC, LabelMe, CVAT, OpenImage, ...) and evaluate them with COCO and PascalVOC."
 homepage = "https://github.com/laclouis5/globox"
 repository = "https://github.com/laclouis5/globox"
@@ -20,22 +20,25 @@
     "pascal voc",
     "average precision",
     "mean average precision",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-numpy = "^1.24.3"
+numpy = "^1.23.5"
 tqdm = "^4.65.0"
 rich = "^13.3.5"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 pycocotools = "^2.0.6"
 pillow = "^9.5.0"
 
 [tool.poetry.scripts]
 globox = "globox.cli:main"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.pytest.ini_options]
+testpaths = ["tests"]
```

### Comparing `globox-2.1.3b0/src/globox/annotation.py` & `globox-2.2.0/src/globox/annotation.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,53 +7,96 @@
 from typing import Mapping, Optional, Union
 import xml.etree.ElementTree as et
 import json
 from warnings import warn
 
 
 class Annotation:
-    """Stores bounding box annotations for one image.
+    """
+    The bounding boxes associated with a uniquely identified image.
+    """
 
-    The image should be uniquely identified by the `image_id` str. The
-    image size is necessary for some operations."""
+    __slots__ = ("_image_id", "_image_size", "boxes")
 
     def __init__(
         self,
         image_id: str,
         image_size: Optional["tuple[int, int]"] = None,
         boxes: Optional["list[BoundingBox]"] = None,
     ) -> None:
+        """
+        Create an `Annotation` for an image identified with a unique `str` tag and with
+        the provided list of bounding boxes.
+
+        The image size in pixels ((width, height) tuple) can be optionally specified and is required
+        for some export formats. This value can be queried from an image file with the
+        `get_image_size()` function if it cannot be retreived from the annotation file.
+        """
         if image_size is not None:
             img_w, img_h = image_size
-            assert img_w > 0 and img_h > 0
-            assert int(img_w) == img_w and int(img_h) == img_h
+            assert (
+                img_w > 0 and img_h > 0
+            ), f"Image size '({img_h}, {img_w})' should be positive."
+            assert (
+                int(img_w) == img_w and int(img_h) == img_h
+            ), f"Image size '({img_h}, {img_w})' components should be integers."
 
-        self.image_id = image_id
-        self.image_size = image_size
+        self._image_id = image_id
+        self._image_size = image_size
         self.boxes = boxes or []
 
     @property
+    def image_id(self) -> str:
+        """The unique identifier of the image for this annotation."""
+        return self._image_id
+
+    @property
+    def image_size(self) -> "Optional[tuple[int, int]]":
+        """The image size in pixels ((width, height) tuple) if present."""
+        return self._image_size
+
+    @image_size.setter
+    def image_size(self, image_size: "Optional[tuple[int, int]]"):
+        if image_size is not None:
+            img_w, img_h = image_size
+            assert (
+                img_w > 0 and img_h > 0
+            ), f"Image size '({img_h}, {img_w})' should be positive."
+            assert (
+                int(img_w) == img_w and int(img_h) == img_h
+            ), f"Image size '({img_h}, {img_w})' components should be integers."
+        self._image_size = image_size
+
+    @property
     def image_width(self) -> Optional[int]:
+        """The image width in pixels."""
         return self.image_size[0] if self.image_size is not None else None
 
     @property
     def image_height(self) -> Optional[int]:
+        """The image height in pixels."""
         return self.image_size[1] if self.image_size is not None else None
 
     def add(self, box: BoundingBox):
+        """Add a bounding box to the image annotation."""
         self.boxes.append(box)
 
     def map_labels(self, mapping: Mapping[str, str]) -> "Annotation":
-        """Change all the bounding box annotation labels according to
-        the provided mapping (act as a translation)."""
+        """
+        Update all the bounding box labels according to the provided dictionary which maps former
+        names to new names. If a label name is not present in the dictionary keys, then it won't
+        be updated.
+        """
         for box in self.boxes:
-            box.label = mapping[box.label]
+            if box.label in mapping.keys():
+                box.label = mapping[box.label]
         return self
 
     def _labels(self) -> "set[str]":
+        """The set of the different label names present in the annotation."""
         return {b.label for b in self.boxes}
 
     @staticmethod
     def from_txt(
         file_path: PathLike,
         *,
         image_id: Optional[str] = None,
@@ -63,15 +106,17 @@
         image_size: Optional["tuple[int, int]"] = None,
         separator: str = " ",
         conf_last: bool = False,
     ) -> "Annotation":
         path = Path(file_path).expanduser().resolve()
 
         if image_id is None:
-            assert image_extension.startswith(".")
+            assert image_extension.startswith(
+                "."
+            ), f"Image extension '{image_extension}' should start with a dot."
             image_id = path.with_suffix(image_extension).name
 
         try:
             lines = path.read_text().splitlines()
         except OSError:
             raise FileParsingError(path, reason="cannot read file")
 
@@ -332,15 +377,16 @@
         image_size: Optional["tuple[int, int]"] = None,
         conf_last: bool = False,
     ) -> str:
         image_size = image_size or self.image_size
 
         if image_size is None:
             raise ValueError(
-                "Either `image_size` shoud be provided as argument or stored in the Annotation object for conversion to YOLO format."
+                "Either `image_size` shoud be provided as argument or stored in the Annotation "
+                "object for conversion to YOLO format."
             )
 
         return "\n".join(
             box.to_yolo(
                 image_size=image_size, label_to_id=label_to_id, conf_last=conf_last
             )
             for box in self.boxes
@@ -570,22 +616,25 @@
         *,
         image_folder: PathLike,
         label_key: str = "label_id",
         confidence_key: str = "confidence",
     ) -> dict:
         path = Path(image_folder).expanduser().resolve()
 
-        assert path.is_dir()
+        assert path.is_dir(), f"Filepath '{path}' is not a folder or does not exist."
 
         image_id = self.image_id
         image_path = path / image_id
         file_size = image_path.stat().st_size
 
         regions = [
             box.to_via_json(label_key=label_key, confidence_key=confidence_key)
             for box in self.boxes
         ]
 
         return {"filename": image_id, "size": file_size, "regions": regions}
 
     def __repr__(self) -> str:
-        return f"Annotation(image_id: {self.image_id}, image_size: {self.image_size}, boxes: {self.boxes})"
+        return (
+            f"Annotation(image_id: {self.image_id}, image_size: {self.image_size}, "
+            "boxes: {self.boxes})"
+        )
```

### Comparing `globox-2.1.3b0/src/globox/annotationset.py` & `globox-2.2.0/src/globox/annotationset.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,27 +25,35 @@
 from tqdm import tqdm
 from warnings import warn
 
 T = TypeVar("T")
 
 
 class AnnotationSet:
-    """Represents a set of annotations.
-
-    This class efficiently stores annotations for several images (a validation
-    database for instance) with a fast lookup by `image_id`. It behaves like a
-    set or dictionary and has similar methods (contains, update, iterator, +
-    operator)."""
+    """
+    A set of annotations of multiple and distinct images, most commonly refered to a 'dataset'.
+    """
 
     def __init__(
         self,
         annotations: Optional[Iterable[Annotation]] = None,
         *,
         override=False,
     ):
+        """
+        Create an `AnnotationSet` from multiple image annotations. Each annotation should be unique,
+        i.e. multiple annotations for a single image (as idendified by its `image_id`) is not
+        allowed.
+
+        Parameters:
+
+        * `annotation`: an iterable of image annotations.
+        * `override`: if `True`, image annotations not unique are allowed and only the last one in
+        the iterator will be kept, else an error is thrown.
+        """
         # TODO: Add optional addition of labels found during
         # parsing, for instance COCO names and YOLO `.names`.
         # Could also add a (lazy) computed accessor that
         # runs through all boxes to get labels.
 
         self._annotations: Dict[str, Annotation] = {}
 
@@ -53,89 +61,113 @@
             for annotation in annotations:
                 self.add(annotation, override=override)
 
         self._id_to_label: Optional["dict[Any, str]"] = None
         self._id_to_imageid: Optional["dict[Any, str]"] = None
 
     def __getitem__(self, image_id: str) -> Annotation:
+        """
+        Get the image annotation with the corresponding `image_id`. Will raise an exception
+        if the image ID is not present in the dataset.
+        """
         return self._annotations[image_id]
 
     def get(self, image_id: str) -> Optional[Annotation]:
+        """
+        Get the image annotation with the corresponding `image_id`, if present in the dataset
+        (else `None` is returned).
+        """
         return self._annotations.get(image_id)
 
     def __len__(self) -> int:
+        """The number of annotations in the dataset."""
         return len(self._annotations)
 
     def __iter__(self):
         yield from self._annotations.values()
 
     def items(self):
+        """A view on the image annotation items (key-value pairs)."""
         return self._annotations.items()
 
     def __contains__(self, annotation: Annotation) -> bool:
+        """Return `True` if a given annotation is present in the dataset, else `False`."""
         return annotation.image_id in self._annotations.keys()
 
     def add(self, annotation: Annotation, *, override=False):
-        """Add an annotation to the set. The annotation 'image_id'
-        should not already be present in the set.
+        """
+        Add an annotation to the dataset.
 
         Parameters:
-        - annotation: the annotation to add.
-        - override: set to true to override any annotation with the same
-        'image_id' already present in the set with the annotation."""
+
+        * `annotation`: the annotation to add.
+        * `override`: set to `True` if the annotation may already be in the dataset and the former
+        it should be replaced by the new one. If `False` and the annotation is already in the
+        dataset, an error is thrown.
+        """
 
         if not override:
-            assert (
-                annotation.image_id not in self.image_ids
-            ), f"The annotation with id '{annotation.image_id}' is already present in the set (set `override` to True to remove this assertion)."
+            assert annotation.image_id not in self.image_ids, (
+                f"The annotation with id '{annotation.image_id}' is already present in the set "
+                "(set `override` to True to remove this assertion)."
+            )
         self._annotations[annotation.image_id] = annotation
 
     def update(self, other: "AnnotationSet", *, override=False) -> "AnnotationSet":
-        """Add annotations from another set to this set.
+        """
+        Add annotations from another datasetset to this one.
 
         Parameters:
-        - other: the set of annotations to add.
-        - override: set to true to override any annotation with the same
-        'image_id' already present in the set.
 
-        Returns:
-        - the input set."""
+        * `other`: the annotations to add.
+        * `override`: if `True`, image annotations in `other` that aren't unique are allowed and
+        only the last one in the iterator will be kept, else an error is thrown.
+        """
 
         if not override:
-            assert self.image_ids.isdisjoint(
-                other.image_ids
-            ), "some image ids are already in the set (set 'override' to True to remove this assertion)."
+            assert self.image_ids.isdisjoint(other.image_ids), (
+                "some image ids are already in the set (set 'override' to True to remove "
+                "this assertion)."
+            )
         self._annotations.update(other._annotations)
         return self
 
     def __ior__(self, other: "AnnotationSet") -> "AnnotationSet":
         return self.update(other)
 
     def __or__(self, other: "AnnotationSet") -> "AnnotationSet":
         return AnnotationSet().update(self).update(other)
 
     def map_labels(self, mapping: Mapping[str, str]) -> "AnnotationSet":
+        """
+        Update all the bounding box labels according to the provided dictionary which maps former
+        names to new names. If a label name is not present in the dictionary keys, then it won't
+        be updated.
+        """
         for annotation in self:
             annotation.map_labels(mapping)
         return self
 
     @property
     def image_ids(self):
+        "A view on the set of image IDs of this dataset."
         return self._annotations.keys()
 
     @property
     def all_boxes(self) -> Iterator[BoundingBox]:
-        """An iterator of all the bounding boxes."""
+        """An iterator of all the bounding boxes of the dataset."""
         for annotation in self:
             yield from annotation.boxes
 
     def nb_boxes(self) -> int:
+        """The number of bounding boxes in the dataset."""
         return sum(len(ann.boxes) for ann in self)
 
     def _labels(self) -> "set[str]":
+        """The set of the different label names present in the dataset."""
         return {b.label for b in self.all_boxes}
 
     @staticmethod
     def from_iter(
         parser: Callable[[T], Annotation],
         iterable: Iterable[T],
         *,
@@ -151,15 +183,17 @@
         extension: str,
         parser: Callable[[Path], Annotation],
         recursive=False,
         verbose: bool = False,
     ) -> "AnnotationSet":
         folder = Path(folder).expanduser().resolve()
 
-        assert folder.is_dir()
+        assert (
+            folder.is_dir()
+        ), f"Filepath '{folder}' is not a folder or does not exist."
 
         files = list(glob(folder, extension, recursive=recursive))
         return AnnotationSet.from_iter(parser, files, verbose=verbose)
 
     @staticmethod
     def from_txt(
         folder: PathLike,
@@ -169,44 +203,55 @@
         relative=False,
         file_extension: str = ".txt",
         image_extension: str = ".jpg",
         separator: str = " ",
         conf_last: bool = False,
         verbose: bool = False,
     ) -> "AnnotationSet":
-        """This method won't try to retreive the image sizes by default. Specify `image_folder` if you need them. `image_folder` is required when `relative` is True."""
+        """
+        This method won't try to retreive the image sizes by default. Specify `image_folder` if
+        you need them. `image_folder` is required when `relative` is True.
+        """
         # TODO: Add error handling
 
         folder = Path(folder).expanduser().resolve()
 
-        assert folder.is_dir()
-        assert image_extension.startswith(".")
+        assert (
+            folder.is_dir()
+        ), f"Filepath '{folder}' is not a folder or does not exist."
+        assert image_extension.startswith(
+            "."
+        ), f"Image extension '{image_extension}' should start with a dot."
 
         if relative:
-            assert (
-                image_folder is not None
-            ), "When `relative` is set to True, `image_folder` must be provided to read image sizes."
+            assert image_folder is not None, (
+                "When `relative` is set to True, `image_folder` must be provided) to read "
+                "image sizes."
+            )
 
         if image_folder is not None:
             image_folder = Path(image_folder).expanduser().resolve()
-            assert image_folder.is_dir()
+            assert (
+                image_folder.is_dir()
+            ), f"Filepath '{image_folder}' is not a folder or does not exist."
 
         def _get_annotation(file: Path) -> Annotation:
             image_id = file.with_suffix(image_extension).name
 
             if image_folder is not None:
                 image_path = image_folder / image_id  # type: ignore
                 assert (
                     image_path.is_file()
                 ), f"File {image_path} does not exists, unable to read the image size."
                 try:
                     image_size = get_image_size(image_path)
                 except UnknownImageFormat:
                     raise ParsingError(
-                        f"Unable to read image size of file {image_path}. The file may be corrupted or the file format not supported."
+                        f"Unable to read image size of file {image_path}. The file may be "
+                        "corrupted or the file format not supported."
                     )
             else:
                 image_size = None
 
             return Annotation.from_txt(
                 file_path=file,
                 image_id=image_id,
@@ -443,17 +488,19 @@
         assert (
             file_path.is_file() and file_path.suffix == ".json"
         ), f"COCO annotation file {file_path} must be a json file."
 
         id_to_label = self._id_to_label
         id_to_imageid = self._id_to_imageid
 
-        assert (
-            id_to_label is not None and id_to_imageid is not None
-        ), "The AnnotationSet instance should have been created with `AnnotationSet.from_coco()` or should have `self.id_to_label` and `self.id_to_image_id` populated. If not the case use the static method `AnnotationSet.from_coco_results()` instead."
+        assert id_to_label is not None and id_to_imageid is not None, (
+            "The AnnotationSet instance should have been created with `AnnotationSet.from_coco()` "
+            "or should have `self.id_to_label` and `self.id_to_image_id` populated. If not the "
+            "case use the static method `AnnotationSet.from_coco_results()` instead."
+        )
 
         id_to_annotation = {}
 
         with file_path.open() as f:
             annotations = json.load(f)
 
         # TODO: Factorize this with `Self.from_coco()`?
@@ -638,15 +685,15 @@
         verbose: bool = False,
     ):
         save_dir = Path(save_dir).expanduser().resolve()
         save_dir.mkdir(exist_ok=True)
 
         def _save(annotation: Annotation):
             path = save_dir / Path(annotation.image_id).with_suffix(".txt")
-            annotation.save_yolo(path, label_to_id=label_to_id, conf_last=conf_last)
+            annotation._save_yolo(path, label_to_id=label_to_id, conf_last=conf_last)
 
         self.save_from_it(_save, verbose=verbose)
 
     def save_yolo(
         self,
         save_dir: PathLike,
         *,
@@ -736,15 +783,20 @@
             imageid_to_id = {v: k for k, v in self._id_to_imageid.items()}
         elif auto_ids:
             label_to_id = {l: i for i, l in enumerate(sorted(self._labels()))}
             imageid_to_id = {im: i for i, im in enumerate(sorted(self.image_ids))}
         else:
             # TODO: Convert to ConversionError.
             raise ValueError(
-                "For COCO, mappings from labels and image ids to integer ids are required. They can be provided either by argument or automatically by the `AnnotationSet` instance if it was created with `AnnotationSet.from_coco()` or `AnnotationSet.from_coco_results()`. You can also set `auto_ids` to True to automatically create image and label ids (warning: this could cause unexpected compatibility issues with other COCO datasets)."
+                "For COCO, mappings from labels and image ids to integer ids are required. "
+                "They can be provided either by argument or automatically by the `AnnotationSet` "
+                "instance if it was created with `AnnotationSet.from_coco()` or "
+                "`AnnotationSet.from_coco_results()`. You can also set `auto_ids` to True to "
+                "automatically create image and label ids (warning: this could cause unexpected "
+                "compatibility issues with other COCO datasets)."
             )
 
         annotations = []
         ann_id_count = 0
         for annotation in tqdm(self, desc="Saving", disable=not verbose):
             for box in annotation.boxes:
                 box_annotation = {
@@ -792,15 +844,15 @@
         verbose: bool = False,
     ):
         path = Path(path).expanduser().resolve()
 
         if path.suffix == "":
             path = path.with_suffix(".json")
 
-        assert path.suffix == ".json"
+        assert path.suffix == ".json", f"Path '{path}' suffix should be '.json'."
 
         content = self.to_coco(
             label_to_id=label_to_id,
             imageid_to_id=imageid_to_id,
             auto_ids=auto_ids,
             verbose=verbose,
         )
@@ -810,15 +862,15 @@
 
     def save_openimage(self, path: PathLike, *, verbose: bool = False):
         path = Path(path).expanduser().resolve()
 
         if path.suffix == "":
             path = path.with_suffix(".csv")
 
-        assert path.suffix == ".csv"
+        assert path.suffix == ".csv", f"Path '{path}' suffix should be '.csv'."
 
         fields = (
             "ImageID",
             "Source",
             "LabelName",
             "Confidence",
             "XMin",
@@ -838,23 +890,29 @@
 
             for annotation in tqdm(self, desc="Saving", disable=not verbose):
                 image_id = annotation.image_id
                 image_size = annotation.image_size
 
                 if image_size is None:
                     raise ValueError(
-                        "The image size should be present in the annotation for `save_openimage`. One should parse the annotations specifying the image folder or populate the `image_size` attribute."
+                        "The image size should be present in the annotation for `save_openimage`. "
+                        "One should parse the annotations specifying the image folder or populate "
+                        "the `image_size` attribute."
                     )
 
                 for box in annotation.boxes:
                     label = box.label
 
                     if "," in label:
                         raise ValueError(
-                            f"The box label '{label}' contains the character ',' which is the same as the separtor character used for BoundingBox representation in OpenImage format (CSV). This will corrupt the saved annotation file and likely make it unreadable. Use another character in the label name, e.g. use and underscore instead of a comma."
+                            f"The box label '{label}' contains the character ',' which is the same "
+                            "as the separtor character used for BoundingBox representation in "
+                            "OpenImage format (CSV). This will corrupt the saved annotation file "
+                            "and likely make it unreadable. Use another character in the label "
+                            "name, e.g. use and underscore instead of a comma."
                         )
 
                     xmin, ymin, xmax, ymax = BoundingBox.abs_to_rel(
                         coords=box.ltrb, size=image_size
                     )
 
                     row = {
@@ -883,15 +941,15 @@
 
     def save_cvat(self, path: PathLike, *, verbose: bool = False):
         path = Path(path).expanduser().resolve()
 
         if path.suffix == "":
             path = path.with_suffix(".xml")
 
-        assert path.suffix == ".xml"
+        assert path.suffix == ".xml", f"Path '{path}' suffix should be '.xml'."
 
         content = self.to_cvat(verbose=verbose)
         content = et.tostring(content, encoding="unicode")
 
         with open_atomic(path, "w") as f:
             f.write(content)
 
@@ -927,15 +985,15 @@
         verbose: bool = False,
     ):
         path = Path(path).expanduser().resolve()
 
         if path.suffix == "":
             path = path.with_suffix(".json")
 
-        assert path.suffix == ".json"
+        assert path.suffix == ".json", f"Path '{path}' suffix should be '.json'."
 
         output = self.to_via_json(
             image_folder=image_folder,
             label_key=label_key,
             confidence_key=confidence_key,
             verbose=verbose,
         )
@@ -962,14 +1020,18 @@
         path = Path(path).expanduser().resolve()
 
         with path.open() as f:
             reader = csv.DictReader(f, fieldnames=("LabelName", "DisplayName"))
             return {l["LabelName"]: l["DisplayName"] for l in reader}
 
     def show_stats(self, *, verbose: bool = False):
+        """
+        Print in the console a synthetic view of the dataset annotations (distribution of
+        bounding boxes and images by label).
+        """
         from rich.table import Table
         from rich import print as rprint
 
         box_by_label = defaultdict(int)
         im_by_label = defaultdict(int)
 
         for annotation in tqdm(self, desc="Stats", disable=not verbose):
```

### Comparing `globox-2.1.3b0/src/globox/atomic.py` & `globox-2.2.0/src/globox/atomic.py`

 * *Files identical despite different names*

### Comparing `globox-2.1.3b0/src/globox/boundingbox.py` & `globox-2.2.0/src/globox/boundingbox.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,71 +2,95 @@
 
 from enum import Enum, auto
 from typing import Mapping, Union, Tuple, Optional, Any
 import xml.etree.ElementTree as et
 
 
 Coordinates = Tuple[float, float, float, float]
+"""
+The four raw coordinates of a `BoundingBox` with no assigned format. The coordinates at indices
+0 and 2 must be on the X-axis (horizontal) and the ones at indices 1 and 3 must be on 
+the Y-axis (vertical).
+"""
 
 
 class BoxFormat(Enum):
     """
-    The bounding box coordinate system.
+    The coordinate format of a `BoundingBox`, i.e. the order and defining coordinates.
 
-    LTRB: xmin, ymin, xmax, ymax
-    LTWH: xmin, ymin, width, height
-    XYWH: xmid, ymid, width, height
+    It can be one of:
+
+    * `BoxFormat.LTRB`: [xmin, ymin, xmax, ymax],
+    * `BoxFormat.LTWH`: [xmin, ymin, width, height],
+    * `BoxFormat.XYWH`: [xmid, ymid, width, height].
+
+    See the `BoundingBox` documentation for more detail on the coordinate format.
     """
 
     LTRB = auto()
+    """[xmin, ymin, xmax, ymax]"""
+
     LTWH = auto()
+    """[xmin, ymin, width, height]"""
+
     XYWH = auto()
+    """[xmid, ymid, width, height]"""
 
     @classmethod
     def from_string(cls, string: str) -> "BoxFormat":
+        """
+        Create a `BoxFormat` from a raw string.
+
+        The raw string can be either "ltrb", "ltwh" or "xywh".
+        """
         if string == "ltrb":
             return BoxFormat.LTRB
         elif string == "ltwh":
             return BoxFormat.LTWH
         elif string == "xywh":
             return BoxFormat.XYWH
         else:
             raise ValueError(f"Invalid BoxFormat string '{string}'")
 
 
 class BoundingBox:
-    """Represents a bounding box with a label and an optional confidence score.
+    """
+    A rectangular bounding box with a label and an optional confidence score. Coordinates are
+    absolute (i.e. in pixels) and stored internally in `BoxFormat.LTRB` format.
 
-    The bounding box coordinates are specified by the top-left corner (xmin, ymin)
-    and the bottom-right corner (xmax, ymax). Coordinates are absolute (i.e. in pixels).
+    Spatial layout:
 
     ```
         xmin   xmid   xmax
     ymin ╆╍╍╍╍╍╍┿╍╍╍╍╍╍┪
          ╏      ┆      ╏
     ymid ╂┄┄┄┄┄┄┼┄┄┄┄┄┄┨
          ╏      ┆      ╏
     ymax ┺╍╍╍╍╍╍┴╍╍╍╍╍╍┛
     ```
-
-    Use the '.create(...)' classmethod to create a BoundingBox using a different coordinate
-    system."""
+    """
 
     __slots__ = ("label", "_xmin", "_ymin", "_xmax", "_ymax", "_confidence")
 
     def __init__(
         self,
         *,
         label: str,
         xmin: float,
         ymin: float,
         xmax: float,
         ymax: float,
         confidence: Optional[float] = None,
     ) -> None:
+        """
+        Create a `BoundingBox` from the top-left and bottom-right corner coordinates.
+
+        Use `BoundingBox.create()` to instantiate a `BoundingBox` from other
+        coordinate formats.
+        """
         assert xmin <= xmax, "`xmax` must be greater than `xmin`."
         assert ymin <= ymax, "`ymax` must be greater than `ymin`."
 
         if confidence is not None:
             assert (
                 0.0 <= confidence <= 1.0
             ), f"Confidence ({confidence}) should be in [0, 1]."
@@ -76,73 +100,88 @@
         self._ymin = ymin
         self._xmax = xmax
         self._ymax = ymax
         self._confidence = confidence
 
     @property
     def confidence(self) -> Optional[float]:
+        """
+        The bounding box optional confidence score. If present, it is a `float`
+        between 0 and 1.
+        """
         return self._confidence
 
     @confidence.setter
     def confidence(self, confidence: Optional[float]):
         if confidence is not None:
             assert (
                 0.0 <= confidence <= 1.0
             ), f"Confidence ({confidence}) should be in [0, 1]."
         self._confidence = confidence
 
     @property
     def xmin(self) -> float:
+        """The `x` value in pixels of the bounding box top-left corner (horizontal axis)."""
         return self._xmin
 
     @property
     def ymin(self) -> float:
+        """The `y` value in pixels of the bounding box top-left corner (vertical axis)."""
         return self._ymin
 
     @property
     def xmax(self) -> float:
+        """The `x` value in pixels of the bounding box bottom-right corner (horizontal axis)."""
         return self._xmax
 
     @property
     def ymax(self) -> float:
+        """The `y` value in pixels of the bounding box top-left corner (vertical axis)."""
         return self._ymax
 
     @property
     def xmid(self) -> float:
+        """The `x` value in pixels of the bounding box center point (horizontal axis)."""
         return (self._xmin + self._xmax) / 2.0
 
     @property
     def ymid(self) -> float:
+        """The `y` value in pixels of the bounding box center point (vertical axis)."""
         return (self._ymin + self._ymax) / 2.0
 
     @property
     def width(self) -> float:
+        """The bounding box width in pixels."""
         return self._xmax - self._xmin
 
     @property
     def height(self) -> float:
+        """The bounding box height in pixels."""
         return self._ymax - self._ymin
 
     @property
     def area(self) -> float:
+        """The area of the bounding box in pixels."""
         return self.width * self.height
 
-    def area_in(self, range_: "tuple[float, float]") -> bool:
+    def _area_in(self, range_: "tuple[float, float]") -> bool:
+        """Returns `True` if the bounding box area is in a given range."""
         lower_bound, upper_bound = range_
         return lower_bound <= self.area <= upper_bound
 
     @property
     def pascal_area(self) -> int:
+        """The bounding box PascalVOC area in pixels."""
         width = int(self._xmax) - int(self._xmin) + 1
         height = int(self._ymax) - int(self._ymin) + 1
 
         return width * height
 
     def iou(self, other: "BoundingBox") -> float:
-        """Intersection over Union computed with float coordinates."""
+        """The Intersection over Union (IoU) between two bounding boxes."""
         xmin = max(self._xmin, other._xmin)
         ymin = max(self._ymin, other._ymin)
         xmax = min(self._xmax, other._xmax)
         ymax = min(self._ymax, other._ymax)
 
         if xmax < xmin or ymax < ymin:
             return 0.0
@@ -152,15 +191,15 @@
 
         if union == 0.0:
             return 1.0
 
         return intersection / union
 
     def pascal_iou(self, other: "BoundingBox") -> float:
-        """Intersection over Union computed with integer coordinates."""
+        """The Pascal VOC Intersection over Union (IoU) between two bounding boxes."""
         xmin = max(int(self._xmin), int(other._xmin))
         ymin = max(int(self._ymin), int(other._ymin))
         xmax = min(int(self._xmax), int(other._xmax))
         ymax = min(int(self._ymax), int(other._ymax))
 
         if xmax < xmin or ymax < ymin:
             return 0.0
@@ -171,66 +210,103 @@
         if union == 0:
             return 1.0
 
         return intersection / union
 
     @property
     def is_detection(self) -> bool:
+        """Return `True` if the bounding box confidence score is not `None`."""
         return self._confidence is not None
 
     @property
     def is_ground_truth(self) -> bool:
+        """Return `True` if the bounding box confidence score is `None`."""
         return self._confidence is None
 
     @staticmethod
     def rel_to_abs(coords: Coordinates, size: "tuple[int, int]") -> Coordinates:
+        """
+        Convert coordinates from relative (between 0 and 1) to absolute (pixels) form.
+
+        The coordinates at indices 0 and 2 must be on the X-axis (horizontal) and the ones
+        at indices 1 and 3 must be on the Y-axis (vertical).
+
+        The image size should be a `(width, height)` tuple expressed in pixels.
+        """
         a, b, c, d = coords
         w, h = size
         return a * w, b * h, c * w, d * h
 
     @staticmethod
     def abs_to_rel(coords: Coordinates, size: "tuple[int, int]") -> Coordinates:
+        """
+        Convert coordinates from absolute (pixels) to relative (between 0 and 1) form.
+
+        The coordinates at indices 0 and 2 must be on the X-axis (horizontal) and the ones
+        at indices 1 and 3 must be on the Y-axis (vertical).
+
+        The image size should be a `(width, height)` tuple expressed in pixels.
+        """
         a, b, c, d = coords
         w, h = size
         return a / w, b / h, c / w, d / h
 
     @staticmethod
     def ltwh_to_ltrb(coords: Coordinates) -> Coordinates:
+        """
+        Convert coordinates from `BoxFormat.LTWH` to `BoxFormat.LTRB` format.
+
+        The coordinates can be either in relative (between 0 and 1) or absolute (pixels) form.
+        """
         xmin, ymin, width, height = coords
         return xmin, ymin, xmin + width, ymin + height
 
     @staticmethod
     def xywh_to_ltrb(coords: Coordinates) -> Coordinates:
+        """
+        Convert coordinates from `BoxFormat.XYWH` to `BoxFormat.LTRB` format.
+
+        The coordinates can be either in relative (between 0 and 1)  or absolute (pixels) form.
+        """
         xmid, ymid, width, height = coords
         w_h, h_h = width / 2, height / 2
         return xmid - w_h, ymid - h_h, xmid + w_h, ymid + h_h
 
     @property
     def ltrb(self) -> Coordinates:
+        """The bounding box coordinates in `BoxFormat.LTRB` format and absolute form (pixels)."""
         return self._xmin, self._ymin, self._xmax, self._ymax
 
     @property
     def ltwh(self) -> Coordinates:
+        """The bounding box coordinates in `BoxFormat.LTWH` format and absolute form (pixels)."""
         return self._xmin, self._ymin, self.width, self.height
 
     @property
     def xywh(self) -> Coordinates:
+        """The bounding box coordinates in `BoxFormat.XYWH` format and absolute form (pixels)."""
         return self.xmid, self.ymid, self.width, self.height
 
     @classmethod
     def create(
         cls,
         *,
         label: str,
         coords: Coordinates,
         confidence: Optional[float] = None,
         box_format=BoxFormat.LTRB,
         relative=False,
         image_size: Optional["tuple[int, int]"] = None,
     ) -> "BoundingBox":
+        """
+        Create a `BoundingBox` from different coordinate formats.
+
+        The image size should be provided if the coordinates are given in the relative form
+        (values between 0 and 1).
+        """
         if relative:
             assert (
                 image_size is not None
             ), "For relative coordinates `image_size` should be provided."
             coords = cls.rel_to_abs(coords, image_size)
 
         if box_format is BoxFormat.LTWH:
@@ -327,15 +403,14 @@
         *,
         image_size: "tuple[int, int]",
     ) -> "BoundingBox":
         return BoundingBox.from_yolo_v5(string, image_size=image_size)
 
     @staticmethod
     def from_xml(node: et.Element) -> "BoundingBox":
-
         label = node.findtext("name")
         box_node = node.find("bndbox")
 
         if label is None or box_node is None:
             raise ValueError("Syntax error in imagenet annotation format")
 
         l, t, r, b = (
@@ -433,17 +508,21 @@
             coords = BoundingBox.abs_to_rel(coords, image_size)
 
         label = self.label
         if label_to_id is not None:
             label = label_to_id[label]
 
         if isinstance(label, str):
-            assert (
-                separator not in label
-            ), f"The box label '{label}' contains the character '{separator}' which is the same as the separtor character used for BoundingBox representation in TXT/YOLO format. This will corrupt the saved annotation file and likely make it unreadable. Use another character in the label name or `label_to_id` mapping, e.g. use and underscore instead of a whitespace."
+            assert separator not in label, (
+                f"The box label '{label}' contains the character '{separator}' which is the same "
+                "as the separtor character used for BoundingBox representation in TXT/YOLO format. "
+                "This will corrupt the saved annotation file and likely make it unreadable. "
+                "Use another character in the label name or `label_to_id` mapping, e.g. use and "
+                "underscore instead of a whitespace."
+            )
 
         if self.is_ground_truth:
             line = (label, *coords)
         elif conf_last:
             line = (label, *coords, self._confidence)
         else:
             line = (label, self._confidence, *coords)
@@ -525,15 +604,15 @@
                 "ybr": f"{ybr}",
             },
         )
 
     def to_via_json(
         self, *, label_key: str = "label_id", confidence_key: str = "confidence"
     ) -> dict:
-        assert label_key != confidence_key
+        assert label_key != confidence_key, f"Label key '{label_key}' and confidence key '{confidence_key}' should be different."
 
         shape_attributes = {
             "name": "rect",
             "x": self.xmin,
             "y": self.ymin,
             "width": self.width,
             "height": self.height,
@@ -559,8 +638,11 @@
             and self.ymin == other.ymin
             and self.xmax == other.xmax
             and self.ymax == other.ymax
             and self.confidence == other.confidence
         )
 
     def __repr__(self) -> str:
-        return f"BoundingBox(label: {self.label}, xmin: {self._xmin}, ymin: {self._ymin}, xmax: {self._xmax}, ymax: {self._ymax}, confidence: {self._confidence})"
+        return (
+            f"BoundingBox(label: {self.label}, xmin: {self._xmin}, ymin: {self._ymin}, "
+            "xmax: {self._xmax}, ymax: {self._ymax}, confidence: {self._confidence})"
+        )
```

### Comparing `globox-2.1.3b0/src/globox/cli.py` & `globox-2.2.0/src/globox/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -363,15 +363,17 @@
         if verbose:
             print(f"Evaluation saved to '{args.save_csv_path}'.", file=sys.stderr)
 
 
 def main():
     args = parse_args()
 
-    assert args.threads is None or args.threads > 0
+    assert (
+        args.threads is None or args.threads > 0
+    ), f"The number of threads '{args.threads}' should either be None or be greater than 0."
 
     mode = args.mode
     if mode == "convert":
         annotations = parse_annotations(args)
         save_annotations(args, annotations)
     elif mode == "summary":
         annotations = parse_annotations(args)
```

### Comparing `globox-2.1.3b0/src/globox/evaluation.py` & `globox-2.2.0/src/globox/evaluation.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,16 +30,18 @@
         npos: int = 0,
     ) -> None:
         self._tps = tps or []
         self._scores = scores or []
         self._npos = npos
         self._cache: dict[str, Any] = {}
 
-        assert self._npos >= 0
-        assert len(self._tps) == len(self._scores)
+        assert self._npos >= 0, f"'npos' ({npos}) should be greater than or equal to 0."
+        assert len(self._tps) == len(
+            self._scores
+        ), f"The number of 'tps' ({len(self._tps)}) should be equal to the number of 'scores' ({len(self._scores)})."
 
     def __iadd__(self, other: "PartialEvaluationItem") -> "PartialEvaluationItem":
         self._tps += other._tps
         self._scores += other._scores
         self._npos += other._npos
         self.clear_cache()
         return self
@@ -159,15 +161,16 @@
         return self._ap
 
     def ar(self) -> float:
         return self._ar
 
 
 class MultiThresholdEvaluation(Dict[str, Dict[str, float]]):
-    """Evaluation of COCO metrics for multiple labels and multiple
+    """
+    Evaluation of COCO metrics for multiple labels and multiple
     IoU thresholds.
     """
 
     def __init__(self, evaluations: "list[Evaluation]") -> None:
         result: "defaultdict[str, list[EvaluationItem]]" = defaultdict(list)
 
         for evaluation in evaluations:
@@ -188,33 +191,45 @@
         return mean(ev["ap"] for ev in self.values() if not isnan(ev["ap"]))
 
     def ar(self) -> float:
         return mean(ev["ar"] for ev in self.values() if not isnan(ev["ar"]))
 
 
 class COCOEvaluator:
-    """Class for evaluating standard COCO metrics efficently.
+    """
+    COCO metrics evaluator.
+
+    Once instantiated, the standard COCO metrics can be queried using the dedicated methods:
+
+    * `COCOEvaluator.ap()`,
+    * `COCOEvaluator.ap_50()`,
+    * `COCOEvaluator.ar_medium()`,
+    * etc.
 
-    This class use an internal cache to store evaluation results,
-    hence, repeated calls to '.evaluate(...)', '.ap50()' and other
-    such methods are fast.
-
-    There are lots of asserts in the evaluation hot path to ensure
-    a valid evaluation, speed gains can be otained by disabling them
-    (python3 --OO ...).
+    Custom evaluations can be performed with `COCOEvaluator.evaluate()` and the standard
+    COCO metrics can be printed to the console with `COCOEvaluator.show_summary()`.
     """
 
     AP_THRESHOLDS = np.linspace(0.5, 0.95, 10)
+    """The ten COCO AP thresholds: [0.5, 0.55, 0.6, 0.65, 0.7, 0.75, 0.8, 0.85, 0.9, 0.95]."""
 
     SMALL_RANGE = (0.0, 32.0**2)
+    """The COCO 'small range' (0, 1024) of bounding box areas (in pixels)."""
+
     MEDIUM_RANGE = (32.0**2, 96.0**2)
+    """The COCO 'medium range' (1024, 9216) of bounding box areas (in pixels)."""
+
     LARGE_RANGE = (96.0**2, float("inf"))
+    """The COCO 'large range' (9216, inf) of bounding box areas (in pixels)."""
+
     ALL_RANGE = (0.0, float("inf"))
+    """The range (0, inf) of any bounding box areas possible (in pixels)."""
 
     RECALL_STEPS = np.linspace(0.0, 1.0, 101)
+    """The 101 COCO recall steps used to compute the AP score."""
 
     CSV_HEADERS = (
         "label",
         "AP 50:95",
         "AP 50",
         "AP 75",
         "AP S",
@@ -231,14 +246,26 @@
     def __init__(
         self,
         *,
         ground_truths: AnnotationSet,
         predictions: AnnotationSet,
         labels: Optional[Iterable[str]] = None,
     ) -> None:
+        """
+        Intantiate a `COCOEvaluator` with the to-be-evaluated dataset and the ground truth
+        reference one.
+
+        All the bounding box annotations from the prediction dataset must have a confidence score
+        and all the ones from the ground truth one must not.
+
+        If labels are provided, only those will be evaluated, else every label will.
+
+        The evaluated datasets must not be modified during the lifetime of the `COCOEvaluator` or
+        the results will be wrong.
+        """
         self._predictions = predictions
         self._ground_truths = ground_truths
 
         if labels is None:
             self.labels = []
         else:
             self.labels = list(labels)
@@ -248,30 +275,25 @@
     def evaluate(
         self,
         *,
         iou_threshold: float,
         max_detections: int = 100,
         size_range: Optional["tuple[float, float]"] = None,
     ) -> Evaluation:
-        """COCO evaluation with custom parameters. The result
-        is cached so that repeated call as fast.
+        """
+        Evaluate COCO metrics for custom parameters.
 
         Parameters:
-        - iou_threshold: the bounding box iou threshold to
-        consider a ground-truth to detection association valid.
-        - max_detections: the maximum number of detections taken
-        into account (sorted by descreasing confidence). Defaults
-        to 100.
-        - size_range: the range of size (bounding box area) to
-        consider. Defaults to all sizes.
 
-        Returns:
-        - An evaluation holding the metrics.
+        * `iou_threshold`: the bounding box iou threshold to consider a ground-truth to
+        detection association valid.
+        * `max_detections`: the maximum number of detections taken into account (sorted by
+        descreasing confidence).
+        * `size_range`: the range of size (bounding box area) to consider.
         """
-
         return self._cached_evaluate(
             iou_threshold=iou_threshold,
             max_detections=max_detections,
             size_range=size_range,
         )
 
     def __evaluate(
@@ -418,15 +440,17 @@
         prediction: Annotation,
         ground_truth: Annotation,
         iou_threshold: float,
         max_detections: int,
         size_range: "tuple[float, float]",
         labels: Optional[Iterable[str]] = None,
     ) -> PartialEvaluation:
-        assert prediction.image_id == ground_truth.image_id
+        assert (
+            prediction.image_id == ground_truth.image_id
+        ), f"The prediction image id '{prediction.image_id}' should be the same as the ground truth image id '{ground_truth.image_id}'."
 
         preds = grouping(prediction.boxes, lambda box: box.label)
         refs = grouping(ground_truth.boxes, lambda box: box.label)
         labels = labels or set(preds.keys()).union(refs.keys())
         evaluation = PartialEvaluation()
 
         for label in labels:
@@ -444,26 +468,34 @@
         cls,
         predictions: "list[BoundingBox]",
         ground_truths: "list[BoundingBox]",
         iou_threshold: float,
         max_detections: int,
         size_range: "tuple[float, float]",
     ) -> PartialEvaluationItem:
-        assert all(p.is_detection for p in predictions)
-        assert all(g.is_ground_truth for g in ground_truths)
-        assert all_equal(p.label for p in predictions)
-        assert all_equal(g.label for g in ground_truths)
+        assert all(
+            p.is_detection for p in predictions
+        ), f"Prediction annotations should not contain ground truth annotations."
+        assert all(
+            g.is_ground_truth for g in ground_truths
+        ), f"Ground truth annotations should not contain prediction annotations."
+        assert all_equal(
+            p.label for p in predictions
+        ), f"The prediction boxes should have the same label."
+        assert all_equal(
+            g.label for g in ground_truths
+        ), f"The ground truth boxes should have the same label."
 
         cls._assert_params(iou_threshold, max_detections, size_range)
 
         dets = sorted(predictions, key=lambda box: box._confidence, reverse=True)  # type: ignore
         dets = dets[:max_detections]
 
-        gts = sorted(ground_truths, key=lambda box: not box.area_in(size_range))
-        gt_ignore = [not g.area_in(size_range) for g in gts]  # Redundant `area_in`
+        gts = sorted(ground_truths, key=lambda box: not box._area_in(size_range))
+        gt_ignore = [not g._area_in(size_range) for g in gts]  # Redundant `area_in`
 
         gt_matches = {}
         dt_matches = {}
 
         for idx_dt, det in enumerate(dets):
             best_iou = 0.0
             idx_best = -1
@@ -485,33 +517,39 @@
                 continue
 
             dt_matches[idx_dt] = idx_best
             gt_matches[idx_best] = idx_dt
 
         # This is overly complicated
         dt_ignore = [
-            gt_ignore[dt_matches[i]] if i in dt_matches else not d.area_in(size_range)
+            gt_ignore[dt_matches[i]] if i in dt_matches else not d._area_in(size_range)
             for i, d in enumerate(dets)
         ]
 
         scores = [d._confidence for i, d in enumerate(dets) if not dt_ignore[i]]
         matches = [i in dt_matches for i in range(len(dets)) if not dt_ignore[i]]
         npos = sum(1 for i in range(len(gts)) if not gt_ignore[i])
 
         return PartialEvaluationItem(matches, scores, npos)
 
     @staticmethod
     def _assert_params(
         iou_threshold: float, max_detections: int, size_range: "tuple[float, float]"
     ):
-        assert 0.0 <= iou_threshold <= 1.0
-        assert max_detections >= 0
+        assert (
+            0.0 <= iou_threshold <= 1.0
+        ), f"the IoU threshold ({iou_threshold}) should be between 0 and 1."
+        assert (
+            max_detections >= 0
+        ), f"The maximum number of detections ({max_detections}) should be positive."
 
         low, high = size_range
-        assert low >= 0.0 and high >= low
+        assert (
+            low >= 0.0 and high >= low
+        ), f"The size range '({low}, {high})' should be positive and non-empty, i.e. 0 < size_range[0] <= size_range[1]."
 
     def clear_cache(self):
         self._cached_evaluate.cache_clear()
 
     def _evaluate_all(self, *, verbose: bool = False):
         params = chain(
             product(
@@ -657,16 +695,18 @@
 
                 writer.writerow(row)
 
     @classmethod
     def _compute_ap(
         cls, scores: "list[float]", matched: "list[bool]", NP: int
     ) -> float:
-        """This curve tracing method has some quirks that do not appear when only unique confidence thresholds
-        are used (i.e. Scikit-learn's implementation), however, in order to be consistent, the COCO's method is reproduced.
+        """
+        This curve tracing method has some quirks that do not appear when only unique confidence
+        thresholds are used (i.e. Scikit-learn's implementation), however, in order to be
+        consistent, the COCO's method is reproduced.
 
         Copyrights: https://github.com/rafaelpadilla/review_object_detection_metrics
         """
         if NP == 0:
             return float("nan")
 
         # sort in descending score order
```

### Comparing `globox-2.1.3b0/src/globox/file_utils.py` & `globox-2.2.0/src/globox/file_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,14 @@
     if isinstance(extensions, str):
         extensions = {extensions}
     else:
         extensions = set(extensions)
 
     assert all(
         e.startswith(".") for e in extensions
-    ), "Parameter `extension` should start with a dot."
+    ), f"Parameter `extensions' ({extensions}) should all start with a dot."
 
     path = Path(folder).expanduser().resolve()
 
     files = path.glob("**/*") if recursive else path.glob("*")
 
     return (f for f in files if f.suffix in extensions and not f.name.startswith("."))
```

### Comparing `globox-2.1.3b0/src/globox/image_utils.py` & `globox-2.2.0/src/globox/image_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,21 +15,24 @@
     :Licence:     MIT
 
 Source: https://github.com/scardine/image_size
 """
 
 
 def get_image_size(file_path: PathLike) -> "tuple[int, int]":
-    """Compute the size of an image without loading into
-    memory, which could result in faster speed.
+    """
+    Compute the size of an image without loading into memory, which could result in faster speed.
+
+    Parameters:
+
+    * `file_path`: path to an image file.
 
-    Args:
-        - file_path (str): path to an image file
     Returns:
-        - The image size (width, height)
+
+    * The image size (width, height).
     """
     file_path = Path(file_path).expanduser().resolve()
 
     size = path.getsize(file_path)
 
     # be explicit with open arguments - we need binary mode
     with file_path.open("rb") as input:
```

### Comparing `globox-2.1.3b0/src/globox/thread_utils.py` & `globox-2.2.0/src/globox/thread_utils.py`

 * *Files identical despite different names*

### Comparing `globox-2.1.3b0/src/globox/utils.py` & `globox-2.2.0/src/globox/utils.py`

 * *Files identical despite different names*

### Comparing `globox-2.1.3b0/PKG-INFO` & `globox-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: globox
-Version: 2.1.3b0
+Version: 2.2.0
 Summary: Globox is a package and command line interface to read and convert object detection databases (COCO, YOLO, PascalVOC, LabelMe, CVAT, OpenImage, ...) and evaluate them with COCO and PascalVOC.
 Home-page: https://github.com/laclouis5/globox
 License: MIT
 Keywords: annotation,metrics,object detection,bounding boxes,yolo,openimages,cvat,coco,pascal voc,average precision,mean average precision
 Author: Louis Lac
 Author-email: lac.louis5@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: numpy (>=1.24.3,<2.0.0)
+Requires-Dist: numpy (>=1.23.5,<2.0.0)
 Requires-Dist: rich (>=13.3.5,<14.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Project-URL: Repository, https://github.com/laclouis5/globox
 Description-Content-Type: text/markdown
 
 # Globox — Object Detection Toolbox
```

