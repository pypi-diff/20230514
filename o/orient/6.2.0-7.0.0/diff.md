# Comparing `tmp/orient-6.2.0.tar.gz` & `tmp/orient-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orient-6.2.0.tar", last modified: Sun Dec 25 21:45:56 2022, max compression
+gzip compressed data, was "orient-7.0.0.tar", last modified: Sun May 14 00:38:28 2023, max compression
```

## Comparing `orient-6.2.0.tar` & `orient-7.0.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-25 21:45:56.336961 orient-6.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2022-12-25 21:45:46.000000 orient-6.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       41 2022-12-25 21:45:46.000000 orient-6.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7718 2022-12-25 21:45:56.336961 orient-6.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6911 2022-12-25 21:45:46.000000 orient-6.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-25 21:45:56.332961 orient-6.2.0/orient/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2022-12-25 21:45:46.000000 orient-6.2.0/orient/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-25 21:45:56.336961 orient-6.2.0/orient/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-25 21:45:46.000000 orient-6.2.0/orient/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2022-12-25 21:45:46.000000 orient-6.2.0/orient/core/box.py
--rw-r--r--   0 runner    (1001) docker     (123)     8546 2022-12-25 21:45:46.000000 orient-6.2.0/orient/core/contour.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2022-12-25 21:45:46.000000 orient-6.2.0/orient/core/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     7536 2022-12-25 21:45:46.000000 orient-6.2.0/orient/core/event.py
--rw-r--r--   0 runner    (1001) docker     (123)    17874 2022-12-25 21:45:46.000000 orient-6.2.0/orient/core/events_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2022-12-25 21:45:46.000000 orient-6.2.0/orient/core/hints.py
--rw-r--r--   0 runner    (1001) docker     (123)    10366 2022-12-25 21:45:46.000000 orient-6.2.0/orient/core/multipolygon.py
--rw-r--r--   0 runner    (1001) docker     (123)     7940 2022-12-25 21:45:46.000000 orient-6.2.0/orient/core/multiregion.py
--rw-r--r--   0 runner    (1001) docker     (123)     7095 2022-12-25 21:45:46.000000 orient-6.2.0/orient/core/multisegment.py
--rw-r--r--   0 runner    (1001) docker     (123)    16526 2022-12-25 21:45:46.000000 orient-6.2.0/orient/core/polygon.py
--rw-r--r--   0 runner    (1001) docker     (123)     8979 2022-12-25 21:45:46.000000 orient-6.2.0/orient/core/processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    13460 2022-12-25 21:45:46.000000 orient-6.2.0/orient/core/region.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2022-12-25 21:45:46.000000 orient-6.2.0/orient/core/segment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3025 2022-12-25 21:45:46.000000 orient-6.2.0/orient/core/sweep_line.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2022-12-25 21:45:46.000000 orient-6.2.0/orient/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2022-12-25 21:45:46.000000 orient-6.2.0/orient/hints.py
--rw-r--r--   0 runner    (1001) docker     (123)    97040 2022-12-25 21:45:46.000000 orient-6.2.0/orient/planar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-25 21:45:56.332961 orient-6.2.0/orient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7718 2022-12-25 21:45:56.000000 orient-6.2.0/orient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      637 2022-12-25 21:45:56.000000 orient-6.2.0/orient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-25 21:45:56.000000 orient-6.2.0/orient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2022-12-25 21:45:56.000000 orient-6.2.0/orient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2022-12-25 21:45:56.000000 orient-6.2.0/orient.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2022-12-25 21:45:46.000000 orient-6.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-25 21:45:56.336961 orient-6.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2022-12-25 21:45:46.000000 orient-6.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 00:38:28.518749 orient-7.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-14 00:38:12.000000 orient-7.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-14 00:38:12.000000 orient-7.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9101 2023-05-14 00:38:28.518749 orient-7.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6911 2023-05-14 00:38:12.000000 orient-7.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 00:38:28.510749 orient-7.0.0/orient/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-14 00:38:12.000000 orient-7.0.0/orient/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 00:38:28.518749 orient-7.0.0/orient/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 00:38:12.000000 orient-7.0.0/orient/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-14 00:38:12.000000 orient-7.0.0/orient/core/box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8356 2023-05-14 00:38:12.000000 orient-7.0.0/orient/core/contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-14 00:38:12.000000 orient-7.0.0/orient/core/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-05-14 00:38:12.000000 orient-7.0.0/orient/core/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17921 2023-05-14 00:38:12.000000 orient-7.0.0/orient/core/events_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-14 00:38:12.000000 orient-7.0.0/orient/core/hints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10376 2023-05-14 00:38:12.000000 orient-7.0.0/orient/core/multipolygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7945 2023-05-14 00:38:12.000000 orient-7.0.0/orient/core/multiregion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-05-14 00:38:12.000000 orient-7.0.0/orient/core/multisegment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16612 2023-05-14 00:38:12.000000 orient-7.0.0/orient/core/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8979 2023-05-14 00:38:12.000000 orient-7.0.0/orient/core/processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13381 2023-05-14 00:38:12.000000 orient-7.0.0/orient/core/region.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-14 00:38:12.000000 orient-7.0.0/orient/core/segment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-05-14 00:38:12.000000 orient-7.0.0/orient/core/sweep_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-14 00:38:12.000000 orient-7.0.0/orient/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-14 00:38:12.000000 orient-7.0.0/orient/hints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97176 2023-05-14 00:38:12.000000 orient-7.0.0/orient/planar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 00:38:28.514749 orient-7.0.0/orient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9101 2023-05-14 00:38:28.000000 orient-7.0.0/orient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-14 00:38:28.000000 orient-7.0.0/orient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 00:38:28.000000 orient-7.0.0/orient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-14 00:38:28.000000 orient-7.0.0/orient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-14 00:38:28.000000 orient-7.0.0/orient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-14 00:38:12.000000 orient-7.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 00:38:28.518749 orient-7.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-14 00:38:12.000000 orient-7.0.0/setup.py
```

### Comparing `orient-6.2.0/LICENSE` & `orient-7.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `orient-6.2.0/PKG-INFO` & `orient-7.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: orient
-Version: 6.2.0
-Summary: Geometric queries.
-Home-page: https://github.com/lycantropos/orient/
-Download-URL: https://github.com/lycantropos/orient/archive/master.zip
-Author: Azat Ibrakov
-Author-email: azatibrakov@gmail.com
-License: MIT License
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 orient
 ======
 
 [![](https://github.com/lycantropos/orient/workflows/CI/badge.svg)](https://github.com/lycantropos/orient/actions/workflows/ci.yml "Github Actions")
 [![](https://readthedocs.org/projects/orient/badge/?version=latest)](https://orient.readthedocs.io/en/latest "Documentation")
 [![](https://codecov.io/gh/lycantropos/orient/branch/master/graph/badge.svg)](https://codecov.io/gh/lycantropos/orient "Codecov")
 [![](https://img.shields.io/github/license/lycantropos/orient.svg)](https://github.com/lycantropos/orient/blob/master/LICENSE "License")
```

### Comparing `orient-6.2.0/orient/core/contour.py` & `orient-7.0.0/orient/core/contour.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,36 +13,37 @@
 from . import box
 from .events_queue import (CompoundEventsQueue,
                            LinearEventsQueue)
 from .hints import SegmentEndpoints
 from .multisegment import to_segments_endpoints
 from .processing import (process_closed_linear_queue,
                          process_open_linear_queue)
-from .segment import (locate_point as locate_point_to_segment,
+from .segment import (locate_point as locate_point_in_segment,
                       relate_segment as relate_segments)
 
 
 def locate_point(contour: Contour, point: Point, context: Context) -> Location:
     return (Location.EXTERIOR
-            if all(locate_point_to_segment(segment, point, context)
+            if all(locate_point_in_segment(segment, point, context)
                    is Location.EXTERIOR
                    for segment in context.contour_segments(contour))
             else Location.BOUNDARY)
 
 
 def relate_segment(contour: Contour,
                    segment: Segment,
                    context: Context) -> Relation:
     angle_orientation = context.angle_orientation
     has_no_touch = has_no_cross = True
     last_touched_edge_index = last_touched_edge_start = None
     start, end = segment.start, segment.end
     for index, sub_segment in enumerate(context.contour_segments(contour)):
         sub_segment_start, sub_segment_end = sub_segment_endpoints = (
-            sub_segment.start, sub_segment.end)
+            sub_segment.start, sub_segment.end
+        )
         relation = relate_segments(sub_segment, segment, context)
         if relation is Relation.COMPONENT or relation is Relation.EQUAL:
             return Relation.COMPONENT
         elif relation is Relation.OVERLAP or relation is Relation.COMPOSITE:
             return Relation.OVERLAP
         elif relation is Relation.TOUCH:
             if has_no_touch:
@@ -63,21 +64,20 @@
             last_touched_edge_start = sub_segment_start
         elif has_no_cross and relation is Relation.CROSS:
             has_no_cross = False
     vertices = contour.vertices
     if (has_no_cross
             and not has_no_touch
             and last_touched_edge_index == len(vertices) - 1):
-        first_sub_segment_endpoints = (first_sub_segment_start,
-                                       first_sub_segment_end) = (vertices[-1],
-                                                                 vertices[0])
+        first_sub_segment_endpoints = (
+            first_sub_segment_start, first_sub_segment_end
+        ) = vertices[-1], vertices[0]
         if (relate_segments(context.segment_cls(first_sub_segment_start,
                                                 first_sub_segment_end),
-                            segment,
-                            context) is Relation.TOUCH
+                            segment, context) is Relation.TOUCH
                 and start not in first_sub_segment_endpoints
                 and end not in first_sub_segment_endpoints
                 and (angle_orientation(start, end, first_sub_segment_start)
                      is Orientation.COLLINEAR)
                 and point_vertex_line_divides_angle(start, vertices[-2],
                                                     first_sub_segment_start,
                                                     first_sub_segment_end,
@@ -165,18 +165,17 @@
 
 def to_edges_endpoints(contour: Contour) -> Iterable[SegmentEndpoints]:
     vertices = contour.vertices
     return ((vertices[index - 1], vertices[index])
             for index in range(len(vertices)))
 
 
-def to_oriented_edges_endpoints(contour: Contour,
-                                context: Context,
-                                clockwise: bool = False
-                                ) -> Iterable[SegmentEndpoints]:
+def to_oriented_edges_endpoints(
+        contour: Contour, context: Context, clockwise: bool = False
+) -> Iterable[SegmentEndpoints]:
     vertices = contour.vertices
     return (((vertices[index - 1], vertices[index])
              for index in range(len(vertices)))
             if (orientation(contour, context)
                 is (Orientation.CLOCKWISE
                     if clockwise
                     else Orientation.COUNTERCLOCKWISE))
```

### Comparing `orient-6.2.0/orient/core/event.py` & `orient-7.0.0/orient/core/event.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,16 +68,17 @@
 
     __slots__ = 'left', '_original_start', '_start'
 
     def __init__(self,
                  start: Point,
                  left: LeftEvent,
                  original_start: Point) -> None:
-        self.left, self._original_start, self._start = (left, original_start,
-                                                        start)
+        self.left, self._original_start, self._start = (
+            left, original_start, start
+        )
 
     __repr__ = recursive_repr()(generate_repr(__init__))
 
     @property
     def end(self) -> Point:
         return self.left.start
 
@@ -108,25 +109,25 @@
         start, end = endpoints
         if start > end:
             start, end = end, start
         result = cls(start, None, start, from_test, SegmentsRelation.DISJOINT)
         result.right = RightEvent(end, result, end)
         return result
 
-    __slots__ = ('right', 'relation', '_from_test', '_original_start',
-                 '_start')
+    __slots__ = '_from_test', '_original_start', '_start', 'relation', 'right'
 
     def __init__(self,
                  start: Point,
                  right: Optional[RightEvent],
                  original_start: Point,
                  from_test: bool,
                  relation: SegmentsRelation) -> None:
-        self.right, self._original_start, self._start = (right, original_start,
-                                                         start)
+        self.right, self._original_start, self._start = (
+            right, original_start, start
+        )
         self._from_test = from_test
         self.relation = relation
 
     __repr__ = recursive_repr()(generate_repr(__init__))
 
     @property
     def end(self) -> Point:
@@ -149,49 +150,52 @@
         return self._original_start
 
     @property
     def start(self) -> Point:
         return self._start
 
     def divide(self, break_point: Point) -> 'LinearLeftEvent':
-        tail = self.right.left = LinearLeftEvent(break_point, self.right,
-                                                 self.original_start,
-                                                 self.from_test, self.relation)
+        tail = self.right.left = LinearLeftEvent(
+                break_point, self.right, self.original_start, self.from_test,
+                self.relation
+        )
         self.right = RightEvent(break_point, self, self.original_end)
         return tail
 
 
 class CompoundLeftEvent(LeftEvent):
     @classmethod
     def from_endpoints(cls,
                        segment_endpoints: SegmentEndpoints,
                        from_test: bool) -> 'CompoundLeftEvent':
         start, end = segment_endpoints
         inside_on_left = True
         if start > end:
             start, end = end, start
             inside_on_left = False
-        result = cls(start, None, start, from_test,
-                     SegmentsRelation.DISJOINT, inside_on_left)
+        result = cls(start, None, start, from_test, SegmentsRelation.DISJOINT,
+                     inside_on_left)
         result.right = RightEvent(end, result, end)
         return result
 
-    __slots__ = ('right', 'interior_to_left', 'other_interior_to_left',
-                 'overlap_kind', 'relation', '_from_test', '_original_start',
-                 '_start')
+    __slots__ = (
+        'right', 'interior_to_left', 'other_interior_to_left', 'overlap_kind',
+        'relation', '_from_test', '_original_start', '_start'
+    )
 
     def __init__(self,
                  start: Point,
                  right: Optional[RightEvent],
                  original_start: Point,
                  from_test: bool,
                  relation: SegmentsRelation,
                  interior_to_left: bool) -> None:
-        self.right, self._original_start, self._start = (right, original_start,
-                                                         start)
+        self.right, self._original_start, self._start = (
+            right, original_start, start
+        )
         self._from_test = from_test
         self.relation = relation
         self.overlap_kind = OverlapKind.NONE
         self.interior_to_left = interior_to_left
         self.other_interior_to_left = False
 
     __repr__ = recursive_repr()(generate_repr(__init__))
@@ -250,10 +254,11 @@
     @property
     def start(self) -> Point:
         return self._start
 
     def divide(self, break_point: Point) -> 'CompoundLeftEvent':
         tail = self.right.left = CompoundLeftEvent(
                 break_point, self.right, self.original_start, self.from_test,
-                self.relation, self.interior_to_left)
+                self.relation, self.interior_to_left
+        )
         self.right = RightEvent(break_point, self, self.original_end)
         return tail
```

### Comparing `orient-6.2.0/orient/core/events_queue.py` & `orient-7.0.0/orient/core/events_queue.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,27 +128,29 @@
                 raise ValueError('Segments of the same geometry '
                                  'should not overlap.')
             starts_equal = below_event.start == event.start
             ends_equal = below_event.end == event.end
             start_min, start_max = (
                 (event, below_event)
                 if starts_equal or self.key(event) < self.key(below_event)
-                else (below_event, event))
+                else (below_event, event)
+            )
             end_min, end_max = (
                 (event.right, below_event.right)
                 if ends_equal or (self.key(event.right)
                                   < self.key(below_event.right))
-                else (below_event.right,
-                      event.right))
+                else (below_event.right, event.right)
+            )
             if starts_equal:
                 # both line segments are equal or share the left endpoint
                 below_event.overlap_kind = event.overlap_kind = (
                     OverlapKind.SAME_ORIENTATION
                     if event.interior_to_left is below_event.interior_to_left
-                    else OverlapKind.DIFFERENT_ORIENTATION)
+                    else OverlapKind.DIFFERENT_ORIENTATION
+                )
                 if not ends_equal:
                     self._divide_segment(end_max.left, end_min.start)
                 return True
             elif ends_equal:
                 # the line segments share the right endpoint
                 self._divide_segment(start_min, start_max.start)
             elif start_min is end_max.left:
@@ -213,16 +215,16 @@
                                                 sweep_line.below(event))
                     sweep_line.remove(event)
                     if above_event is not None and below_event is not None:
                         self.detect_intersection(below_event, above_event)
         self.detect_crossing_angles(same_start_events)
         yield from complete_events_relations(same_start_events)
 
-    def detect_crossing_angles(self, same_start_events: Sequence[Event]
-                               ) -> None:
+    def detect_crossing_angles(self,
+                               same_start_events: Sequence[Event]) -> None:
         if (len(same_start_events) < 4
                 or not (1 < sum(event.from_test for event in same_start_events)
                         < len(same_start_events) - 1)):
             # for crossing angles there should be at least two pairs
             # of segments from different origins
             return
         from_test_events, from_goal_events = [], []
@@ -236,15 +238,16 @@
                          key=partial(point_event_cosine,
                                      from_goal_events[0].end))
         base_end = base_event.end
         largest_angle_event = min(from_goal_events,
                                   key=partial(point_event_cosine, base_end))
         largest_angle_end = largest_angle_event.end
         base_orientation = self.context.angle_orientation(
-                start, base_end, largest_angle_end)
+                start, base_end, largest_angle_end
+        )
         if not all_equal(self._point_in_angle(test_event.end, start, base_end,
                                               largest_angle_end,
                                               base_orientation)
                          for test_event in from_test_events):
             for event in same_start_events:
                 left_event = event if event.is_left else event.left
                 left_event.relation = max(left_event.relation,
@@ -269,21 +272,22 @@
                 raise ValueError('Segments of the same geometry '
                                  'should not overlap.')
             starts_equal = below_event.start == event.start
             ends_equal = below_event.end == event.end
             start_min, start_max = (
                 (event, below_event)
                 if starts_equal or self.key(event) < self.key(below_event)
-                else (below_event, event))
+                else (below_event, event)
+            )
             end_min, end_max = (
                 (event.right, below_event.right)
                 if ends_equal or (self.key(event.right)
                                   < self.key(below_event.right))
-                else (below_event.right,
-                      event.right))
+                else (below_event.right, event.right)
+            )
             if starts_equal:
                 # both line segments are equal or share the left endpoint
                 if not ends_equal:
                     self._divide_segment(end_max.left, end_min.start)
             elif ends_equal:
                 # the line segments share the right endpoint
                 self._divide_segment(start_min, start_max.start)
@@ -299,17 +303,19 @@
     def _point_in_angle(self,
                         point: Point,
                         vertex: Point,
                         first_ray_point: Point,
                         second_ray_point: Point,
                         angle_orientation: Orientation) -> bool:
         first_half_orientation = self.context.angle_orientation(
-                vertex, first_ray_point, point)
+                vertex, first_ray_point, point
+        )
         second_half_orientation = self.context.angle_orientation(
-                second_ray_point, vertex, point)
+                second_ray_point, vertex, point
+        )
         return (second_half_orientation is angle_orientation
                 if first_half_orientation is Orientation.COLLINEAR
                 else (first_half_orientation is angle_orientation
                       if second_half_orientation is Orientation.COLLINEAR
                       else (first_half_orientation is second_half_orientation
                             is (angle_orientation
                                 # if angle is degenerate
@@ -358,28 +364,30 @@
                     else (other_end_orientation
                           # the lowest segment is processed first
                           is (Orientation.COUNTERCLOCKWISE
                               if event.is_left
                               else Orientation.CLOCKWISE)))
 
 
-def complete_events_relations(same_start_events: Sequence[Event]
-                              ) -> Iterable[Event]:
+def complete_events_relations(
+        same_start_events: Sequence[Event]
+) -> Iterable[Event]:
     for offset, first in enumerate(same_start_events,
                                    start=1):
         first_left = first if first.is_left else first.left
         for second_index in range(offset, len(same_start_events)):
             second = same_start_events[second_index]
             second_left = second if second.is_left else second.left
             if second_left.from_test is first_left.from_test:
                 continue
             elif (first_left.start == second_left.start
                   and first_left.end == second_left.end):
                 first_left.relation = second_left.relation = (
-                    SegmentsRelation.OVERLAP)
+                    SegmentsRelation.OVERLAP
+                )
             else:
                 relation = (SegmentsRelation.TOUCH
                             if (first.start == first.original_start
                                 or second.start == second.original_start)
                             else SegmentsRelation.CROSS)
                 first_left.relation = max(first_left.relation, relation)
                 second_left.relation = max(second_left.relation, relation)
```

### Comparing `orient-6.2.0/orient/core/multipolygon.py` & `orient-7.0.0/orient/core/multipolygon.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,16 @@
 
 
 def relate_region(multipolygon: Multipolygon,
                   region: Region,
                   context: Context) -> Relation:
     region_bounding_box = context.contour_box(region)
     all_disjoint, none_disjoint, multipolygon_max_x, events_queue = (
-        True, True, None, None)
+        True, True, None, None
+    )
     for polygon in multipolygon.polygons:
         polygon_bounding_box = context.polygon_box(polygon)
         if box.disjoint_with(region_bounding_box, polygon_bounding_box):
             if none_disjoint:
                 none_disjoint = False
         else:
             if all_disjoint:
@@ -160,15 +161,16 @@
 
 
 def relate_polygon(multipolygon: Multipolygon,
                    polygon: Polygon,
                    context: Context) -> Relation:
     polygon_bounding_box = context.polygon_box(polygon)
     all_disjoint, none_disjoint, multipolygon_max_x, events_queue = (
-        True, True, None, None)
+        True, True, None, None
+    )
     for sub_polygon in multipolygon.polygons:
         sub_polygon_bounding_box = context.polygon_box(sub_polygon)
         if box.disjoint_with(sub_polygon_bounding_box, polygon_bounding_box):
             if none_disjoint:
                 none_disjoint = False
         else:
             if all_disjoint:
```

### Comparing `orient-6.2.0/orient/core/multiregion.py` & `orient-7.0.0/orient/core/multiregion.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,15 +116,16 @@
 
 
 def _relate_region(goal_regions: Iterable[Region],
                    region: Region,
                    region_bounding_box: Box,
                    context: Context) -> Relation:
     all_disjoint, none_disjoint, goal_regions_max_x, events_queue = (
-        True, True, None, None)
+        True, True, None, None
+    )
     for goal_region in goal_regions:
         goal_region_bounding_box = context.contour_box(goal_region)
         if box.disjoint_with(region_bounding_box, goal_region_bounding_box):
             if none_disjoint:
                 none_disjoint = False
         else:
             if all_disjoint:
```

### Comparing `orient-6.2.0/orient/core/multisegment.py` & `orient-7.0.0/orient/core/multisegment.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,41 +56,46 @@
                 components.append(to_sorted_pair(sub_segment_endpoints))
         elif relation is Relation.OVERLAP:
             if is_segment_superset:
                 is_segment_superset = False
             if has_no_overlap:
                 has_no_overlap = False
             start, end = segment_endpoints = _subtract_segments_overlap(
-                    segment_endpoints, sub_segment_endpoints)
+                    segment_endpoints, sub_segment_endpoints
+            )
         else:
             if is_segment_superset:
                 is_segment_superset = False
             if has_no_overlap:
                 if relation is Relation.TOUCH:
                     if has_no_touch:
                         has_no_touch = False
                     if has_no_cross:
                         intersection = context.segments_intersection(
-                                sub_segment, segment)
+                                sub_segment, segment
+                        )
                         if intersection != start and intersection != end:
                             sub_start, sub_end = sub_segment_endpoints
                             non_touched_endpoint = (sub_start
                                                     if intersection == sub_end
                                                     else sub_end)
                             try:
                                 previous_orientation = (
-                                    middle_touching_orientations[intersection])
+                                    middle_touching_orientations[intersection]
+                                )
                             except KeyError:
                                 middle_touching_orientations[intersection] = (
                                     context.angle_orientation(
-                                            start, end, non_touched_endpoint))
+                                            start, end, non_touched_endpoint
+                                    )
+                                )
                             else:
-                                if (context.angle_orientation(
-                                        start, end, non_touched_endpoint)
-                                        is not previous_orientation):
+                                if context.angle_orientation(
+                                        start, end, non_touched_endpoint
+                                ) is not previous_orientation:
                                     has_no_cross = False
                 elif has_no_cross and relation is Relation.CROSS:
                     has_no_cross = False
     if has_no_overlap:
         return (Relation.DISJOINT
                 if has_no_touch and has_no_cross
                 else (Relation.TOUCH
```

### Comparing `orient-6.2.0/orient/core/polygon.py` & `orient-7.0.0/orient/core/polygon.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,16 @@
     relation_without_holes = relate_contour_to_region(polygon.border, contour,
                                                       contour_bounding_box,
                                                       context)
     holes = polygon.holes
     if holes and (relation_without_holes is Relation.ENCLOSED
                   or relation_without_holes is Relation.WITHIN):
         relation_with_holes = relate_contour_to_multiregion(
-                holes, contour, contour_bounding_box, context)
+                holes, contour, contour_bounding_box, context
+        )
         if relation_with_holes is Relation.DISJOINT:
             return relation_without_holes
         elif relation_with_holes is Relation.TOUCH:
             return Relation.ENCLOSED
         elif (relation_with_holes is Relation.CROSS
               or relation_with_holes is Relation.COMPONENT):
             return relation_with_holes
@@ -180,15 +181,16 @@
     if subsets_regions_indices:
         is_subset_of_border = len(subsets_regions_indices) == len(multiregion)
         relation_with_holes = relate_multiregions(
                 holes,
                 multiregion
                 if is_subset_of_border
                 else [multiregion[index] for index in subsets_regions_indices],
-                context)
+                context
+        )
         if relation_with_holes is Relation.DISJOINT:
             return ((Relation.WITHIN
                      if none_touch
                      else Relation.ENCLOSED)
                     if is_subset_of_border
                     else Relation.OVERLAP)
         elif relation_with_holes is Relation.TOUCH:
@@ -277,17 +279,19 @@
                 holes_relation = (
                     relate_multiregions(
                             test_holes,
                             goal_holes
                             if len(subsets_holes_indices) == len(goal_holes)
                             else [goal_holes[index]
                                   for index in subsets_holes_indices],
-                            context)
+                            context
+                    )
                     if test_holes
-                    else Relation.DISJOINT)
+                    else Relation.DISJOINT
+                )
                 if holes_relation is Relation.EQUAL:
                     return (Relation.ENCLOSED
                             if borders_relation is Relation.WITHIN
                             else borders_relation)
                 elif (holes_relation is Relation.COMPONENT
                       or holes_relation is Relation.ENCLOSED):
                     return Relation.ENCLOSED
@@ -327,17 +331,19 @@
             holes_relation = (
                 relate_multiregions(
                         goal_holes,
                         test_holes
                         if len(subsets_holes_indices) == len(test_holes)
                         else [test_holes[index]
                               for index in subsets_holes_indices],
-                        context)
+                        context
+                )
                 if goal_holes
-                else Relation.DISJOINT)
+                else Relation.DISJOINT
+            )
             if holes_relation is Relation.EQUAL:
                 return (Relation.ENCLOSES
                         if borders_relation is Relation.COVER
                         else borders_relation)
             elif (holes_relation is Relation.COMPONENT
                   or holes_relation is Relation.ENCLOSED):
                 return Relation.ENCLOSES
```

### Comparing `orient-6.2.0/orient/core/processing.py` & `orient-7.0.0/orient/core/processing.py`

 * *Files identical despite different names*

### Comparing `orient-6.2.0/orient/core/region.py` & `orient-7.0.0/orient/core/region.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,20 +8,21 @@
 from ground.hints import (Box,
                           Contour,
                           Multisegment,
                           Point,
                           Segment)
 
 from . import box
-from .contour import (equal as contours_equal,
-                      orientation as contour_orientation,
-                      point_vertex_line_divides_angle,
-                      to_edges_endpoints as contour_to_edges_endpoints,
-                      to_oriented_edges_endpoints
-                      as contour_to_oriented_segments)
+from .contour import (
+    equal as contours_equal,
+    orientation as contour_orientation,
+    point_vertex_line_divides_angle,
+    to_edges_endpoints as contour_to_edges_endpoints,
+    to_oriented_edges_endpoints as contour_to_oriented_segments
+)
 from .events_queue import CompoundEventsQueue
 from .hints import Region
 from .multisegment import to_segments_endpoints
 from .processing import (process_compound_queue,
                          process_linear_compound_queue)
 from .segment import (locate_point as locate_point_in_segment,
                       relate_segment as relate_segments)
@@ -87,15 +88,16 @@
             last_touched_edge_index = index
             last_touched_edge_start = edge_start
         elif relation_with_edge is Relation.CROSS:
             return Relation.CROSS
     vertices = contour.vertices
     if not has_no_touch and last_touched_edge_index == len(vertices) - 1:
         first_edge_endpoints = first_edge_start, first_edge_end = (
-            vertices[-1], vertices[0])
+            vertices[-1], vertices[0]
+        )
         if (relate_segments(context.segment_cls(first_edge_start,
                                                 first_edge_end), segment,
                             context) is Relation.TOUCH
                 and start not in first_edge_endpoints
                 and end not in first_edge_endpoints
                 and (context.angle_orientation(start, end, first_edge_start)
                      is Orientation.COLLINEAR)
```

### Comparing `orient-6.2.0/orient/core/segment.py` & `orient-7.0.0/orient/core/segment.py`

 * *Files identical despite different names*

### Comparing `orient-6.2.0/orient/core/sweep_line.py` & `orient-7.0.0/orient/core/sweep_line.py`

 * *Files identical despite different names*

### Comparing `orient-6.2.0/orient/planar.py` & `orient-7.0.0/orient/planar.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,29 +51,30 @@
     True
     >>> point_in_segment(Point(3, 0), segment) is Location.EXTERIOR
     True
     >>> point_in_segment(Point(0, 1), segment) is Location.EXTERIOR
     True
     """
     return _segment.locate_point(
-            segment, point, _get_context() if context is None else context)
+            segment, point, _get_context() if context is None else context
+    )
 
 
 def segment_in_segment(left: _Segment, right: _Segment,
                        *,
                        context: _Optional[_Context] = None) -> _Relation:
     """
     Finds relation between segments.
 
     Time complexity:
         ``O(1)``
     Memory complexity:
         ``O(1)``
 
-    :param left: point to check for.
+    :param left: segment to check for.
     :param right: segment to check in.
     :param context: geometric context.
     :returns: relation between segments.
 
     >>> from ground.base import Relation, get_context
     >>> context = get_context()
     >>> Point = context.point_cls
@@ -98,15 +99,16 @@
     ...  is Relation.TOUCH)
     True
     >>> (segment_in_segment(Segment(Point(3, 0), Point(4, 0)), segment)
     ...  is Relation.DISJOINT)
     True
     """
     return _segment.relate_segment(
-            right, left, _get_context() if context is None else context)
+            right, left, _get_context() if context is None else context
+    )
 
 
 def point_in_multisegment(point: _Point,
                           multisegment: _Multisegment,
                           *,
                           context: _Optional[_Context] = None) -> _Location:
     """
@@ -139,16 +141,16 @@
     True
     >>> point_in_multisegment(Point(3, 0), multisegment) is Location.BOUNDARY
     True
     >>> point_in_multisegment(Point(4, 0), multisegment) is Location.BOUNDARY
     True
     """
     return _multisegment.locate_point(
-            multisegment, point,
-            _get_context() if context is None else context)
+            multisegment, point, _get_context() if context is None else context
+    )
 
 
 def segment_in_multisegment(segment: _Segment,
                             multisegment: _Multisegment,
                             *,
                             context: _Optional[_Context] = None) -> _Relation:
     """
@@ -193,15 +195,16 @@
     True
     >>> segment_in_multisegment(Segment(Point(4, 4), Point(5, 5)),
     ...                         multisegment) is Relation.DISJOINT
     True
     """
     return _multisegment.relate_segment(
             multisegment, segment,
-            _get_context() if context is None else context)
+            _get_context() if context is None else context
+    )
 
 
 def multisegment_in_multisegment(left: _Multisegment,
                                  right: _Multisegment,
                                  *,
                                  context: _Optional[_Context] = None
                                  ) -> _Relation:
@@ -266,15 +269,16 @@
     >>> (multisegment_in_multisegment(Multisegment(square_edges),
     ...                               Multisegment(square_edges
     ...                                            + inner_square_edges))
     ...  is Relation.COMPONENT)
     True
     """
     return _multisegment.relate_multisegment(
-            right, left, _get_context() if context is None else context)
+            right, left, _get_context() if context is None else context
+    )
 
 
 def point_in_contour(point: _Point, contour: _Contour,
                      *,
                      context: _Optional[_Context] = None) -> _Location:
     """
     Finds location of point in contour.
@@ -300,15 +304,16 @@
     True
     >>> point_in_contour(Point(2, 2), square) is Location.BOUNDARY
     True
     >>> point_in_contour(Point(3, 3), square) is Location.EXTERIOR
     True
     """
     return _contour.locate_point(
-            contour, point, _get_context() if context is None else context)
+            contour, point, _get_context() if context is None else context
+    )
 
 
 def segment_in_contour(segment: _Segment, contour: _Contour,
                        *,
                        context: _Optional[_Context] = None) -> _Relation:
     """
     Finds relation between segment and contour.
@@ -351,15 +356,16 @@
     ...  is Relation.DISJOINT)
     True
     >>> (segment_in_contour(Segment(Point(2, 2), Point(4, 4)), square)
     ...  is Relation.CROSS)
     True
     """
     return _contour.relate_segment(
-            contour, segment, _get_context() if context is None else context)
+            contour, segment, _get_context() if context is None else context
+    )
 
 
 def multisegment_in_contour(multisegment: _Multisegment,
                             contour: _Contour,
                             *,
                             context: _Optional[_Context] = None) -> _Relation:
     """
@@ -420,15 +426,16 @@
     True
     >>> (multisegment_in_contour(Multisegment(square_edges[1:]), square)
     ...  is Relation.COMPONENT)
     True
     """
     return _contour.relate_multisegment(
             contour, multisegment,
-            _get_context() if context is None else context)
+            _get_context() if context is None else context
+    )
 
 
 def contour_in_contour(left: _Contour, right: _Contour,
                        *,
                        context: _Optional[_Context] = None) -> _Relation:
     """
     Finds relation between contours.
@@ -457,15 +464,16 @@
     True
     >>> contour_in_contour(square, triangle) is Relation.OVERLAP
     True
     >>> contour_in_contour(square, square) is Relation.EQUAL
     True
     """
     return _contour.relate_contour(
-            right, left, _get_context() if context is None else context)
+            right, left, _get_context() if context is None else context
+    )
 
 
 def point_in_region(point: _Point, region: _Region,
                     *,
                     context: _Optional[_Context] = None) -> _Location:
     """
     Finds location of point in region.
@@ -546,15 +554,16 @@
     ...  is Relation.WITHIN)
     True
     >>> (segment_in_region(Segment(Point(2, 2), Point(4, 4)), square)
     ...  is Relation.CROSS)
     True
     """
     return _region.relate_segment(
-            region, segment, _get_context() if context is None else context)
+            region, segment, _get_context() if context is None else context
+    )
 
 
 def multisegment_in_region(multisegment: _Multisegment,
                            region: _Region,
                            *,
                            context: _Optional[_Context] = None) -> _Relation:
     """
@@ -613,15 +622,16 @@
     True
     >>> (multisegment_in_region(Multisegment(inner_square_edges), square)
     ...  is Relation.WITHIN)
     True
     """
     return _region.relate_multisegment(
             region, multisegment,
-            _get_context() if context is None else context)
+            _get_context() if context is None else context
+    )
 
 
 def contour_in_region(contour: _Contour, region: _Region,
                       *,
                       context: _Optional[_Context] = None) -> _Relation:
     """
     Finds relation between contour and region.
@@ -656,15 +666,16 @@
     True
     >>> contour_in_region(triangle, square) is Relation.ENCLOSED
     True
     >>> contour_in_region(inner_square, square) is Relation.WITHIN
     True
     """
     return _region.relate_contour(
-            region, contour, _get_context() if context is None else context)
+            region, contour, _get_context() if context is None else context
+    )
 
 
 def region_in_region(left: _Region, right: _Region,
                      *,
                      context: _Optional[_Context] = None) -> _Relation:
     """
     Finds relation between regions.
@@ -706,15 +717,16 @@
     True
     >>> region_in_region(triangle, square) is Relation.ENCLOSED
     True
     >>> region_in_region(inner_square, square) is Relation.WITHIN
     True
     """
     return _region.relate_region(
-            right, left, _get_context() if context is None else context)
+            right, left, _get_context() if context is None else context
+    )
 
 
 def point_in_multiregion(point: _Point,
                          multiregion: _Multiregion,
                          *,
                          context: _Optional[_Context] = None) -> _Location:
     """
@@ -746,15 +758,16 @@
     True
     >>> point_in_multiregion(Point(2, 2), [triangle]) is Location.EXTERIOR
     True
     >>> point_in_multiregion(Point(2, 2), [square]) is Location.BOUNDARY
     True
     """
     return _multiregion.locate_point(
-            multiregion, point, _get_context() if context is None else context)
+            multiregion, point, _get_context() if context is None else context
+    )
 
 
 def segment_in_multiregion(segment: _Segment,
                            multiregion: _Multiregion,
                            *,
                            context: _Optional[_Context] = None) -> _Relation:
     """
@@ -805,15 +818,16 @@
     True
     >>> (segment_in_multiregion(Segment(Point(2, 2), Point(4, 4)), [square])
     ...  is Relation.CROSS)
     True
     """
     return _multiregion.relate_segment(
             multiregion, segment,
-            _get_context() if context is None else context)
+            _get_context() if context is None else context
+    )
 
 
 def multisegment_in_multiregion(multisegment: _Multisegment,
                                 multiregion: _Multiregion,
                                 *,
                                 context: _Optional[_Context] = None
                                 ) -> _Relation:
@@ -879,15 +893,16 @@
     >>> (multisegment_in_multiregion(Multisegment(first_inner_square_edges),
     ...                              [first_square, second_square])
     ...  is Relation.WITHIN)
     True
     """
     return _multiregion.relate_multisegment(
             multiregion, multisegment,
-            _get_context() if context is None else context)
+            _get_context() if context is None else context
+    )
 
 
 def contour_in_multiregion(contour: _Contour,
                            multiregion: _Multiregion,
                            *,
                            context: _Optional[_Context] = None) -> _Relation:
     """
@@ -940,15 +955,16 @@
     >>> (contour_in_multiregion(first_inner_square,
     ...                         [first_square, third_square])
     ...  is Relation.WITHIN)
     True
     """
     return _multiregion.relate_contour(
             multiregion, contour,
-            _get_context() if context is None else context)
+            _get_context() if context is None else context
+    )
 
 
 def region_in_multiregion(region: _Region,
                           multiregion: _Multiregion,
                           *,
                           context: _Optional[_Context] = None) -> _Relation:
     """
@@ -1007,16 +1023,16 @@
     True
     >>> (region_in_multiregion(first_inner_square,
     ...                        [first_square, third_square])
     ...  is Relation.WITHIN)
     True
     """
     return _multiregion.relate_region(
-            multiregion, region,
-            _get_context() if context is None else context)
+            multiregion, region, _get_context() if context is None else context
+    )
 
 
 def multiregion_in_multiregion(left: _Multiregion,
                                right: _Multiregion,
                                *,
                                context: _Optional[_Context] = None
                                ) -> _Relation:
@@ -1094,15 +1110,16 @@
     True
     >>> (multiregion_in_multiregion([first_inner_square, third_inner_square],
     ...                             [first_square, third_square])
     ...  is Relation.WITHIN)
     True
     """
     return _multiregion.relate_multiregion(
-            right, left, _get_context() if context is None else context)
+            right, left, _get_context() if context is None else context
+    )
 
 
 def point_in_polygon(point: _Point, polygon: _Polygon,
                      *,
                      context: _Optional[_Context] = None) -> _Location:
     """
     Finds location of point in polygon.
@@ -1145,15 +1162,16 @@
     ...  is Location.INTERIOR)
     True
     >>> (point_in_polygon(Point(2, 2), Polygon(outer_square, [inner_square]))
     ...  is Location.EXTERIOR)
     True
     """
     return _polygon.locate_point(
-            polygon, point, _get_context() if context is None else context)
+            polygon, point, _get_context() if context is None else context
+    )
 
 
 def segment_in_polygon(segment: _Segment, polygon: _Polygon,
                        *,
                        context: _Optional[_Context] = None) -> _Relation:
     """
     Finds relation between segment and polygon.
@@ -1207,15 +1225,16 @@
     True
     >>> (segment_in_polygon(Segment(Point(0, 0), Point(4, 4)),
     ...                     Polygon(outer_square, [inner_square]))
     ...  is Relation.CROSS)
     True
     """
     return _polygon.relate_segment(
-            polygon, segment, _get_context() if context is None else context)
+            polygon, segment, _get_context() if context is None else context
+    )
 
 
 def multisegment_in_polygon(multisegment: _Multisegment,
                             polygon: _Polygon,
                             *,
                             context: _Optional[_Context] = None) -> _Relation:
     """
@@ -1282,15 +1301,16 @@
     >>> (multisegment_in_polygon(Multisegment(inner_square_edges),
     ...                          Polygon(square, []))
     ...  is Relation.WITHIN)
     True
     """
     return _polygon.relate_multisegment(
             polygon, multisegment,
-            _get_context() if context is None else context)
+            _get_context() if context is None else context
+    )
 
 
 def contour_in_polygon(contour: _Contour, polygon: _Polygon,
                        *,
                        context: _Optional[_Context] = None) -> _Relation:
     """
     Finds relation between contour and polygon.
@@ -1331,15 +1351,16 @@
     >>> contour_in_polygon(triangle, Polygon(square, [])) is Relation.ENCLOSED
     True
     >>> (contour_in_polygon(inner_square, Polygon(square, []))
     ...  is Relation.WITHIN)
     True
     """
     return _polygon.relate_contour(
-            polygon, contour, _get_context() if context is None else context)
+            polygon, contour, _get_context() if context is None else context
+    )
 
 
 def region_in_polygon(region: _Region, polygon: _Polygon,
                       *,
                       context: _Optional[_Context] = None) -> _Relation:
     """
     Finds relation between region and polygon.
@@ -1386,15 +1407,16 @@
     True
     >>> region_in_polygon(triangle, Polygon(square, [])) is Relation.ENCLOSED
     True
     >>> region_in_polygon(inner_square, Polygon(square, [])) is Relation.WITHIN
     True
     """
     return _polygon.relate_region(
-            polygon, region, _get_context() if context is None else context)
+            polygon, region, _get_context() if context is None else context
+    )
 
 
 def multiregion_in_polygon(multiregion: _Multiregion,
                            polygon: _Polygon,
                            *,
                            context: _Optional[_Context] = None) -> _Relation:
     """
@@ -1463,15 +1485,16 @@
     >>> (multiregion_in_polygon([first_inner_square, second_inner_square],
     ...                         Polygon(outer_square, []))
     ...  is Relation.WITHIN)
     True
     """
     return _polygon.relate_multiregion(
             polygon, multiregion,
-            _get_context() if context is None else context)
+            _get_context() if context is None else context
+    )
 
 
 def polygon_in_polygon(left: _Polygon, right: _Polygon,
                        *,
                        context: _Optional[_Context] = None) -> _Relation:
     """
     Finds relation between polygons.
@@ -1565,15 +1588,16 @@
     ...                     Polygon(outer_square, []))
     ...  is polygon_in_polygon(Polygon(inner_square, [innermore_square]),
     ...                        Polygon(outer_square, [innermost_square]))
     ...  is Relation.WITHIN)
     True
     """
     return _polygon.relate_polygon(
-            right, left, _get_context() if context is None else context)
+            right, left, _get_context() if context is None else context
+    )
 
 
 def point_in_multipolygon(point: _Point,
                           multipolygon: _Multipolygon,
                           *,
                           context: _Optional[_Context] = None) -> _Relation:
     """
@@ -1614,16 +1638,16 @@
     >>> (point_in_multipolygon(Point(2, 2),
     ...                        Multipolygon([Polygon(first_square, []),
     ...                                      Polygon(second_square, [])]))
     ...  is Location.INTERIOR)
     True
     """
     return _multipolygon.locate_point(
-            multipolygon, point,
-            _get_context() if context is None else context)
+            multipolygon, point, _get_context() if context is None else context
+    )
 
 
 def segment_in_multipolygon(segment: _Segment,
                             multipolygon: _Multipolygon,
                             *,
                             context: _Optional[_Context] = None) -> _Relation:
     """
@@ -1683,15 +1707,16 @@
     ...                          Multipolygon([Polygon(first_square, []),
     ...                                        Polygon(second_square, [])]))
     ...  is Relation.WITHIN)
     True
     """
     return _multipolygon.relate_segment(
             multipolygon, segment,
-            _get_context() if context is None else context)
+            _get_context() if context is None else context
+    )
 
 
 def multisegment_in_multipolygon(multisegment: _Multisegment,
                                  multipolygon: _Multipolygon,
                                  *,
                                  context: _Optional[_Context] = None
                                  ) -> _Relation:
@@ -1771,15 +1796,16 @@
     ...      Multipolygon([Polygon(first_square, []),
     ...                    Polygon(second_square, [])]))
     ...  is Relation.WITHIN)
     True
     """
     return _multipolygon.relate_multisegment(
             multipolygon, multisegment,
-            _get_context() if context is None else context)
+            _get_context() if context is None else context
+    )
 
 
 def contour_in_multipolygon(contour: _Contour,
                             multipolygon: _Multipolygon,
                             *,
                             context: _Optional[_Context] = None) -> _Relation:
     """
@@ -1847,15 +1873,16 @@
     ...      first_inner_square, Multipolygon([Polygon(first_square, []),
     ...                                        Polygon(third_square, [])]))
     ...  is Relation.WITHIN)
     True
     """
     return _multipolygon.relate_contour(
             multipolygon, contour,
-            _get_context() if context is None else context)
+            _get_context() if context is None else context
+    )
 
 
 def region_in_multipolygon(region: _Region,
                            multipolygon: _Multipolygon,
                            *,
                            context: _Optional[_Context] = None) -> _Relation:
     """
@@ -1930,15 +1957,16 @@
     ...      first_inner_square, Multipolygon([Polygon(first_square, []),
     ...                                        Polygon(third_square, [])]))
     ...  is Relation.WITHIN)
     True
     """
     return _multipolygon.relate_region(
             multipolygon, region,
-            _get_context() if context is None else context)
+            _get_context() if context is None else context
+    )
 
 
 def multiregion_in_multipolygon(multiregion: _Multiregion,
                                 multipolygon: _Multipolygon,
                                 *,
                                 context: _Optional[_Context] = None
                                 ) -> _Relation:
@@ -2057,15 +2085,16 @@
     ...      Multipolygon([Polygon(first_square, []),
     ...                    Polygon(third_square, [])]))
     ...  is Relation.WITHIN)
     True
     """
     return _multipolygon.relate_multiregion(
             multipolygon, multiregion,
-            _get_context() if context is None else context)
+            _get_context() if context is None else context
+    )
 
 
 def polygon_in_multipolygon(polygon: _Polygon,
                             multipolygon: _Multipolygon,
                             *,
                             context: _Optional[_Context] = None) -> _Relation:
     """
@@ -2204,15 +2233,16 @@
     ...                 Multipolygon([Polygon(outer_square,
     ...                                       [innermost_square])]))
     ...  is Relation.WITHIN)
     True
     """
     return _multipolygon.relate_polygon(
             multipolygon, polygon,
-            _get_context() if context is None else context)
+            _get_context() if context is None else context
+    )
 
 
 def multipolygon_in_multipolygon(left: _Multipolygon,
                                  right: _Multipolygon,
                                  *,
                                  context: _Optional[_Context] = None
                                  ) -> _Relation:
@@ -2337,8 +2367,9 @@
     ...                    Polygon(third_inner_square, [])]),
     ...      Multipolygon([Polygon(first_square, []),
     ...                    Polygon(third_square, [])]))
     ...  is Relation.WITHIN)
     True
     """
     return _multipolygon.relate_multipolygon(
-            right, left, _get_context() if context is None else context)
+            right, left, _get_context() if context is None else context
+    )
```

### Comparing `orient-6.2.0/orient.egg-info/PKG-INFO` & `orient-7.0.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,49 @@
 Metadata-Version: 2.1
 Name: orient
-Version: 6.2.0
+Version: 7.0.0
 Summary: Geometric queries.
 Home-page: https://github.com/lycantropos/orient/
 Download-URL: https://github.com/lycantropos/orient/archive/master.zip
-Author: Azat Ibrakov
-Author-email: azatibrakov@gmail.com
+Author-email: Azat Ibrakov <azatibrakov@gmail.com>
 License: MIT License
+        
+        Copyright (c) 2020 Azat Ibrakov
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: tests
 License-File: LICENSE
 
 orient
 ======
 
 [![](https://github.com/lycantropos/orient/workflows/CI/badge.svg)](https://github.com/lycantropos/orient/actions/workflows/ci.yml "Github Actions")
 [![](https://readthedocs.org/projects/orient/badge/?version=latest)](https://orient.readthedocs.io/en/latest "Documentation")
```

### Comparing `orient-6.2.0/orient.egg-info/SOURCES.txt` & `orient-7.0.0/orient.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
-requirements.txt
+pyproject.toml
 setup.py
 orient/__init__.py
 orient/hints.py
 orient/planar.py
 orient.egg-info/PKG-INFO
 orient.egg-info/SOURCES.txt
 orient.egg-info/dependency_links.txt
```

