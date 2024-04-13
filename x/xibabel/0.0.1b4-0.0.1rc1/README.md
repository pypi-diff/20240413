# Comparing `tmp/xibabel-0.0.1b4.tar.gz` & `tmp/xibabel-0.0.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xibabel-0.0.1b4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "xibabel-0.0.1rc1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `xibabel-0.0.1b4.tar` & `xibabel-0.0.1rc1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     3421 2024-04-07 16:56:14.320676 xibabel-0.0.1b4/README.md
--rw-r--r--   0        0        0     1406 2024-04-07 16:25:21.695205 xibabel-0.0.1b4/pyproject.toml
--rw-r--r--   0        0        0      200 2024-04-07 16:56:41.024072 xibabel-0.0.1b4/src/xibabel/__init__.py
--rw-r--r--   0        0        0      571 2024-04-07 15:22:16.624201 xibabel-0.0.1b4/src/xibabel/bench/bench_nib_xib_load.py
--rw-r--r--   0        0        0    26467 2024-04-07 15:22:16.624535 xibabel-0.0.1b4/src/xibabel/loaders.py
--rw-r--r--   0        0        0       20 2024-04-07 15:22:16.624850 xibabel-0.0.1b4/src/xibabel/testing/.gitignore
--rw-r--r--   0        0        0     2584 2024-04-07 15:22:16.625223 xibabel-0.0.1b4/src/xibabel/testing/__init__.py
--rw-r--r--   0        0        0      627 2024-04-07 15:22:16.625441 xibabel-0.0.1b4/src/xibabel/testing/__main__.py
--rw-r--r--   0        0        0     5225 2024-04-07 15:22:16.625822 xibabel-0.0.1b4/src/xibabel/testing/fetcher.py
--rw-r--r--   0        0        0      463 2024-04-07 15:22:16.626137 xibabel-0.0.1b4/src/xibabel/testing/test_files.yml
--rw-r--r--   0        0        0      396 2024-04-07 15:22:16.626362 xibabel-0.0.1b4/src/xibabel/testing/test_sets.yml
--rw-r--r--   0        0        0        0 2024-04-07 15:22:16.626413 xibabel-0.0.1b4/src/xibabel/tests/__init__.py
--rw-r--r--   0        0        0     2512 2024-04-07 15:22:16.626863 xibabel-0.0.1b4/src/xibabel/tests/conftest.py
--rw-r--r--   0        0        0      332 2024-04-07 15:22:16.627123 xibabel-0.0.1b4/src/xibabel/tests/markers.py
--rw-r--r--   0        0        0     1306 2024-04-07 15:22:16.627411 xibabel-0.0.1b4/src/xibabel/tests/run_server.py
--rw-r--r--   0        0        0    20900 2024-04-07 15:22:16.627824 xibabel-0.0.1b4/src/xibabel/tests/test_loaders.py
--rw-r--r--   0        0        0     1205 2024-04-07 15:22:16.628147 xibabel-0.0.1b4/src/xibabel/tests/test_merge.py
--rw-r--r--   0        0        0     2855 2024-04-07 15:22:16.628417 xibabel-0.0.1b4/src/xibabel/tests/test_scripting.py
--rw-r--r--   0        0        0     2264 2024-04-07 15:22:16.628815 xibabel-0.0.1b4/src/xibabel/tests/test_testing.py
--rw-r--r--   0        0        0      794 2024-04-07 15:22:16.629096 xibabel-0.0.1b4/src/xibabel/xutils.py
--rw-r--r--   0        0        0     5292 1970-01-01 00:00:00.000000 xibabel-0.0.1b4/PKG-INFO
+-rw-r--r--   0        0        0     3426 2024-04-07 17:42:35.750454 xibabel-0.0.1rc1/README.md
+-rw-r--r--   0        0        0     1406 2024-04-07 16:25:21.695205 xibabel-0.0.1rc1/pyproject.toml
+-rw-r--r--   0        0        0      213 2024-04-13 18:48:43.861862 xibabel-0.0.1rc1/src/xibabel/__init__.py
+-rw-r--r--   0        0        0      571 2024-04-07 15:22:16.624201 xibabel-0.0.1rc1/src/xibabel/bench/bench_nib_xib_load.py
+-rw-r--r--   0        0        0    31370 2024-04-13 18:48:14.108529 xibabel-0.0.1rc1/src/xibabel/loaders.py
+-rw-r--r--   0        0        0       20 2024-04-07 15:22:16.624850 xibabel-0.0.1rc1/src/xibabel/testing/.gitignore
+-rw-r--r--   0        0        0     2584 2024-04-07 15:22:16.625223 xibabel-0.0.1rc1/src/xibabel/testing/__init__.py
+-rw-r--r--   0        0        0      627 2024-04-07 15:22:16.625441 xibabel-0.0.1rc1/src/xibabel/testing/__main__.py
+-rw-r--r--   0        0        0     5225 2024-04-07 15:22:16.625822 xibabel-0.0.1rc1/src/xibabel/testing/fetcher.py
+-rw-r--r--   0        0        0      463 2024-04-07 15:22:16.626137 xibabel-0.0.1rc1/src/xibabel/testing/test_files.yml
+-rw-r--r--   0        0        0      396 2024-04-07 15:22:16.626362 xibabel-0.0.1rc1/src/xibabel/testing/test_sets.yml
+-rw-r--r--   0        0        0        0 2024-04-07 15:22:16.626413 xibabel-0.0.1rc1/src/xibabel/tests/__init__.py
+-rw-r--r--   0        0        0     2512 2024-04-07 15:22:16.626863 xibabel-0.0.1rc1/src/xibabel/tests/conftest.py
+-rw-r--r--   0        0        0      332 2024-04-07 15:22:16.627123 xibabel-0.0.1rc1/src/xibabel/tests/markers.py
+-rw-r--r--   0        0        0     1306 2024-04-07 15:22:16.627411 xibabel-0.0.1rc1/src/xibabel/tests/run_server.py
+-rw-r--r--   0        0        0    30927 2024-04-13 18:48:14.109065 xibabel-0.0.1rc1/src/xibabel/tests/test_loaders.py
+-rw-r--r--   0        0        0     1205 2024-04-07 15:22:16.628147 xibabel-0.0.1rc1/src/xibabel/tests/test_merge.py
+-rw-r--r--   0        0        0     2855 2024-04-07 15:22:16.628417 xibabel-0.0.1rc1/src/xibabel/tests/test_scripting.py
+-rw-r--r--   0        0        0     2264 2024-04-07 15:22:16.628815 xibabel-0.0.1rc1/src/xibabel/tests/test_testing.py
+-rw-r--r--   0        0        0      794 2024-04-07 15:22:16.629096 xibabel-0.0.1rc1/src/xibabel/xutils.py
+-rw-r--r--   0        0        0     5298 1970-01-01 00:00:00.000000 xibabel-0.0.1rc1/PKG-INFO
```

### Comparing `xibabel-0.0.1b4/README.md` & `xibabel-0.0.1rc1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -54,28 +54,28 @@
   the point at which you need the data in memory.
 - Xarrays and Dask allow new storage formats, including storage as
   [Zarr](https://zarr.readthedocs.io) and
   HDF5 / [netCDF](https://en.wikipedia.org/wiki/NetCDF).
 - You can optimize the on-disk format for memory and CPU by adjusting
   _chunking_. We are working on performance metrics for different processing
   steps.
-- Xibabel uses [fsspec](https://filesystem-spec.readthedocs.io) for reading
+- Xibabel uses [`fsspec`](https://filesystem-spec.readthedocs.io) for reading
   NIfTI and other files, allowing you to use many filesystems as the source for
-  your data, including HTTP, Amazon, Google Cloud and others. See the FSSpec
+  your data, including HTTP, Amazon, Google Cloud and others. See the `fsspec`
   documentation for details, and the code above for an example using HTTP as
   a backing store.
 
 ## Status
 
 Xibabel is in development mode at the moment. We are still experimenting with
 the API. We'd love to hear from you if you are interested to help. Please do
 not rely on any particular features in this alpha version, including
 compatibility of file formats; prefer to save outputs as BIDS / NIfTI format,
 for which we do guarantee input compatibility (e.g. `xib.save(ximg,
-'out.nii.gz'`).
+'out.nii.gz')`).
 
 ## Install
 
 From Pip — the current pre-release:
 
 ```bash
 pip install --pre xarray
```

### Comparing `xibabel-0.0.1b4/pyproject.toml` & `xibabel-0.0.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xibabel-0.0.1b4/src/xibabel/bench/bench_nib_xib_load.py` & `xibabel-0.0.1rc1/src/xibabel/bench/bench_nib_xib_load.py`

 * *Files identical despite different names*

### Comparing `xibabel-0.0.1b4/src/xibabel/loaders.py` & `xibabel-0.0.1rc1/src/xibabel/loaders.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 from nibabel.fileholders import FileHolder
 from nibabel.affines import from_matvec, apply_affine
 
 import fsspec
 import xarray as xr
 import dask.array as da
 
+from .xutils import merge
+
 
 logger = logging.getLogger(__name__)
 
 
 def max_available_div(div=10):
     """ Set default chunk as fraction of maximum aailable memory
     """
@@ -34,14 +36,17 @@
 MAXCHUNK_STRATEGY = max_available_div
 
 
 class FDataObj:
     """ Wrapper for dataobj that returns floating point values from indexing.
     """
 
+    # Signal that this is a proxy (for a proxy).
+    is_proxy = True
+
     def __init__(self, dataobj, dtype=np.float64):
         dtype = np.dtype(dtype)
         if not issubclass(dtype.type, np.inexact):
             raise ValueError(f'{dtype} should be floating point type')
         self._dataobj = dataobj
         self.dtype = dtype
         self.shape = dataobj.shape
@@ -63,58 +68,98 @@
 
         Returns
         -------
         chunk_sizes : list
             Chunk sizes for Dask array creation, being number of elements in
             one chunk over all axes of array in ``self.dataobj``.
         """
-        sizes = [None] * self.ndim
-        if maxchunk is None:
-            maxchunk = MAXCHUNK_STRATEGY()
-        chunk_size = np.prod(self.shape) * self.dtype.itemsize
-        if chunk_size <= maxchunk:
-            return sizes
-        axis_nos = range(self.ndim)
-        if self.order == 'F':  # Assume C order by default.
-            axis_nos = axis_nos[::-1]
-        for axis_no in axis_nos:
-            chunk_size //= self.shape[axis_no]
-            n_chunks = maxchunk // chunk_size
-            if n_chunks:
-                sizes[axis_no] = int(n_chunks)
-                return sizes
-            sizes[axis_no] = 1
+        return default_chunks(self, maxchunk)
+
+    def reshape(self, shape):
+        """ Return object reshaped to `shape`
+
+        Notes
+        -----
+        There is no requirement that the contained ``dataobj`` has a
+        ``reshape`` method; if not, calling this method will raise an
+        ``AttributeError``.
+        """
+        return self.__class__(self._dataobj.reshape(shape), self.dtype)
+
+
+def default_chunks(arr, order=None, maxchunk=None):
+    """ Calculate chunk sizes for array-like `arr` from shape and `order`.
+
+    Parameters
+    ----------
+    arr : array-like
+        Object with attributes `.shape` and `.dtype`.  It can also have
+        attribute `order`, and / or `.flags.f_contiguous`, used only if `order`
+        below is None.
+    order : {None, "F", "C"}
+        Memory ordering of array.
+    maxchunk : None or int, optional
+        The largest allowable chunk sizes in bytes.
+
+    Returns
+    -------
+    chunk_sizes : list
+        Chunk sizes for Dask array creation, being number of elements in
+        one chunk over all axes of array in ``self.dataobj``.
+    """
+    if order is None:  # FDataObj, dataobj
+        order = getattr(arr, 'order', None)  # FDataObj, dataobj
+    if order is None:  # ndarray
+        order = getattr(getattr(arr, 'flags', None), 'f_contiguous', 'C')
+    ndim = len(arr.shape)
+    sizes = [None] * ndim
+    if maxchunk is None:
+        maxchunk = MAXCHUNK_STRATEGY()
+    chunk_size = np.prod(arr.shape) * arr.dtype.itemsize
+    if chunk_size <= maxchunk:
         return sizes
+    axis_nos = range(ndim)
+    if order == 'F':
+        axis_nos = axis_nos[::-1]
+    for axis_no in axis_nos:
+        chunk_size //= arr.shape[axis_no]
+        n_chunks = maxchunk // chunk_size
+        if n_chunks:
+            sizes[axis_no] = int(n_chunks)
+            return sizes
+        sizes[axis_no] = 1
+    return sizes
 
 
-dimno2name= {
+_DIMNO2NAME = {
     None: None,
     0: 'i',
     1: 'j',
     2: 'k'}
 
-dimname2no = {v: k for k, v in dimno2name.items()}
+
+_DIMNAME2NO = {v: k for k, v in _DIMNO2NAME.items()}
 
 
-time_unit_scaler = {
+_TIME_UNIT_SCALER = {
     'sec': 1,
     'msec': 1 / 1000,
     'usec': 1 / 1_000_000}
 
 
-class NiHeader2Meta:
+class NiHeader2Attrs:
 
     def __init__(self, header):
         self.header = nib.Nifti1Header.from_header(header)
 
     def get_dim_labels(self):
         freq_dim, phase_dim, slice_dim = self.header.get_dim_info()
-        return {'xib-FrequencyEncodingDirection': dimno2name[freq_dim],
-                'PhaseEncodingDirection': dimno2name[phase_dim],
-                'SliceEncodingDirection': dimno2name[slice_dim]}
+        return {'xib-FrequencyEncodingDirection': _DIMNO2NAME[freq_dim],
+                'PhaseEncodingDirection': _DIMNO2NAME[phase_dim],
+                'SliceEncodingDirection': _DIMNO2NAME[slice_dim]}
 
     def get_slice_timing(self):
         hdr = self.header
         freq_dim, phase_dim, slice_dim = hdr.get_dim_info()
         if not slice_dim:
             return None
         duration = hdr.get_slice_duration()
@@ -134,98 +179,96 @@
         zooms = hdr.get_zooms()
         if len(zooms) < 4:
             return None
         time_zoom = zooms[3]
         space_units, time_units = hdr.get_xyzt_units()
         if time_units == 'unknown':
             return None
-        return time_unit_scaler[time_units] * time_zoom
+        return _TIME_UNIT_SCALER[time_units] * time_zoom
 
     def get_affines(self):
         """ Collect valid affines
         """
         hdr = self.header
         affines = {}
         for affine_type in 'qform', 'sform':
             code = hdr.get_value_label(affine_type + '_code')
             if code != 'unknown':
                 affine = getattr(hdr, 'get_' + affine_type)()
                 affines[code] = affine.tolist()
         return affines
 
-    def to_meta(self):
-        meta = self.get_dim_labels()
-        meta['SliceTiming'] = self.get_slice_timing()
-        meta['RepetitionTime'] = self.get_repetition_time()
-        meta['xib-affines'] = self.get_affines()
-        return {k: v for k, v in meta.items() if v is not None}
+    def to_attrs(self):
+        attrs = self.get_dim_labels()
+        attrs['SliceTiming'] = self.get_slice_timing()
+        attrs['RepetitionTime'] = self.get_repetition_time()
+        attrs['xib-affines'] = self.get_affines()
+        return {k: v for k, v in attrs.items() if v is not None}
 
 
-class Meta2NiHeader:
+class Attrs2NiHeader:
     """ Class writes BIDS attribute dictionary into NIfTI header.
     """
 
-    def __init__(self, header=None, meta=None):
+    def __init__(self, header=None, attrs=None):
         self.header = nib.Nifti1Header.from_header(header)
-        self.meta = {} if meta is None else meta.copy()
+        self.attrs = {} if attrs is None else attrs.copy()
 
     def set_dim_labels(self):
         # Assume canonical axis order.
-        d = self.meta
+        d = self.attrs
         self.header.set_dim_info(
-            freq=dimname2no.get(d.get('xib-FrequencyEncodingDirection')),
-            phase=dimname2no.get(d.get('PhaseEncodingDirection')),
-            slice=dimname2no.get(d.get('SliceEncodingDirection')))
+            freq=_DIMNAME2NO.get(d.get('xib-FrequencyEncodingDirection')),
+            phase=_DIMNAME2NO.get(d.get('PhaseEncodingDirection')),
+            slice=_DIMNAME2NO.get(d.get('SliceEncodingDirection')))
 
     def set_slice_timing(self):
-        slice_times = self.meta.get('SliceTiming')
+        slice_times = self.attrs.get('SliceTiming')
         if slice_times is None:
             return
         try:
             return self.header.set_slice_times(slice_times)
         except HeaderDataError:
             pass
 
     def set_repetition_time(self):
         hdr = self.header
         zooms = np.array(hdr.get_zooms())
         # Assume header record of image already has correct shape.
         if len(zooms) < 4:
             return
-        TR = self.meta.get('RepetitionTime')
+        TR = self.attrs.get('RepetitionTime')
         TR, units = (0, None) if TR is None else (TR, 'sec')
         zooms[3] = TR
         hdr.set_xyzt_units(t=units)
         hdr.set_zooms(zooms)
 
     def set_affines(self):
         """ Set valid affines to header.
         """
         hdr = self.header
-        affines = self.meta.get('xib-affines', {})
-        for code in ('aligned', 'scanner'):
-            if code in affines:
-                hdr.set_qform(affines[code], code)
-                break
-        for code in ('mni', 'talairach', 'template'):
+        affines = self.attrs.get('xib-affines', {})
+        methods = [hdr.set_sform, hdr.set_qform]
+        for code in ('mni', 'talairach', 'template', 'aligned', 'scanner'):
             if code in affines:
-                hdr.set_sform(affines[code], code)
-                break
+                methods.pop()(affines[code], code)
+                if not methods:
+                    break
 
     def updated_header(self):
         self.set_dim_labels()
         self.set_slice_timing()
         self.set_affines()
         self.set_repetition_time()
         return self.header
 
 
-def hdr2meta(header):
+def hdr2attrs(header):
     # We could try extracting more information from other file types, but
-    return NiHeader2Meta(header).to_meta()
+    return NiHeader2Attrs(header).to_attrs()
 
 
 def load_zarr(url_or_path, **kwargs):
     r""" Load image from Zarr/Xibabel-format data at `url_or_path`
 
     Parameters
     ----------
@@ -288,15 +331,16 @@
 
 
 class NPEncoder(json.JSONEncoder):
 
     def default(self, obj):
         if hasattr(obj, 'tolist'):
             return obj.tolist()
-        return super().default(self, obj)
+        # No supported serialization, pass to default encoder to raise.
+        return super().default(obj)
 
 
 _jdumps = partial(json.dumps, cls=NPEncoder)
 
 
 def _attrs2json_attrs(attrs):
     """ Write JSON formed for encoding nested structures to netCDF
@@ -495,19 +539,21 @@
         url_json = replace_suffix(url_uncomp, (), '.json')
         if fs.exists(url_json):
             sidecar_file = fs.open(url_json)
         elif require_json:
             raise XibFileError(
                 f'BIDS loading {url_or_path} but no corresponding '
                 f'{url_json} file, and `require_json` is True')
-    img, meta = _nibabel2img_meta(img_file)
+    nib_img, attrs = _nibabel2img_attrs(img_file)
     if sidecar_file:
         with sidecar_file as fobj:
-            meta.update(json.load(fobj))
-    return _img_meta2ximg(img, meta, url_or_path)
+            attrs.update(json.load(fobj))
+    return _img_attrs2ximg(
+        nib_img,
+        **{'attrs': attrs, 'name': _url2name(url_or_path)})
 
 
 def load_nibabel(url_or_path, **kwargs):
     r""" Load image from Nibabel-format data at `url_or_path`
 
     `url_or_path` may point directly to ``.json`` file, or to Nibabel format
     file, for expect a ``.json`` file to be present, in which case we will load
@@ -527,74 +573,144 @@
     ------
     XibFileError
         If there is no file corresponding to `url_or_path`.
     """
     return load_bids(url_or_path, require_json=False, **kwargs)
 
 
+def from_array(arr, *, fa_kwargs=None, **kwargs):
+    r""" Create image from array-like `arr`
+
+    Assume array dimensions correspond to NIfTI labels.
+
+    Parameters
+    ----------
+    arr : array-like
+    chunks : 'auto' or int or tuple
+        See documentation for ``dask.array.from_array``
+    fa_kwargs : None or mapping, optional, keyword only
+        Keyword arguments that we pass through the ``dask.array.from_array``
+        function.
+    \*\*kwargs : mapping, keyword arguments
+        Keyword arguments to pass to ``DataArray`` constructor.  A common
+        example is ``dims`` (None or sequence of dimension names).  If None,
+        use NIfTI convention for coordinate names.  If sequence, it must match
+        the number of dimensions of `arr`.
+
+    Returns
+    -------
+    ximg : Xibabel image
+    """
+    arr_like = FDataObj(arr) if nib.is_proxy(arr) else arr
+    ximg = _arr_attrs2ximg(arr_like, fa_kwargs=fa_kwargs, **kwargs)
+    if 'dims' not in kwargs:  # Use NIfTI conventions
+        ximg = _squeeze_time(ximg)
+    return ximg
+
+
 def _comp_exts():
     return tuple(f'.{ext}' for ext in fsspec.utils.compressions)
 
 
 def _path2class(filename):
     compression_exts = _comp_exts()
     for klass in nib.all_image_classes:
+        if len(klass.files_types) > 1:
+            continue
         base, ext, gzext, ftype = parse_filename(filename,
                                                  klass.files_types,
                                                  compression_exts)
         if ftype == 'image':
             return klass
     raise XibFileError(f'No single-file Nibabel class for {filename}')
 
 
 class FSFileHolder(FileHolder):
 
     def __del__(self):
         self.fileobj.close()
 
 
-_NI_SPACE_DIMS = ('i', 'j', 'k')
-_NI_TIME_DIM = 'time'
+_NI_DIM_NAMES = ('i', 'j', 'k', 'time', 'p', 'q', 'r')
+_NI_SPACE_DIMS = _NI_DIM_NAMES[:3]
+_NI_TIME_DIM = _NI_DIM_NAMES[3]
 
 
-def _nibabel2img_meta(img_file):
+def _nibabel2img_attrs(img_file):
     # Identify relevant files from img_file
     # Make file_map with opened files.
     if 'local' in img_file.fs.protocol:
         img = nib.load(img_file.path)
     else:  # Not local - use stream interface.
-        img_klass = _path2class(img_file.full_name)
+        img_klass = _path2class(img_file.path)
         # We are passing out opened fsspec files.
-        fh = FileHolder(img_file.full_name, img_file.open())
+        fh = FileHolder(img_file.path, img_file.open())
         img = img_klass.from_file_map({'image': fh})
-    return img, hdr2meta(img.header)
+    return img, hdr2attrs(img.header)
 
 
-def _img_meta2ximg(img, meta, url_or_path):
-    dataobj = FDataObj(img.dataobj)
-    coords = {}
-    dims = _NI_SPACE_DIMS
+def _img_attrs2ximg(obj, *, fa_kwargs=None, **kwargs):
+    arr_like = FDataObj(obj.dataobj)
+    fa_kwargs = {} if fa_kwargs is None else {}
+    if not fa_kwargs.get('fancy'):  # Assume no fancy indexing by default.
+        fa_kwargs['fancy'] = False
+    if not fa_kwargs.get('chunks'):
+        fa_kwargs['chunks'] = arr_like.chunk_sizes()
+    ximg = _arr_attrs2ximg(arr_like,
+                           fa_kwargs=fa_kwargs,
+                           **kwargs)
+    return _squeeze_time(ximg) if hasattr(obj, 'get_sform') else ximg
+
+
+def _squeeze_time(ximg):
+    # https://nifti.nimh.nih.gov/nifti-1/documentation/nifti1fields/nifti1fields_pages/dim.html
+    # > If dim[4]=1 or dim[0] < 4, there is no time axis.
+    if 'time' in ximg.dims and len(ximg['time']) == 1:
+        ximg = ximg.sel(time=0)
+    return ximg
+
+
+def _arr_attrs2ximg(arr, *, fa_kwargs=None, **kwargs):
+    fa_kwargs = {} if fa_kwargs is None else fa_kwargs
+    if not fa_kwargs.get('chunks'):
+        fa_kwargs['chunks'] = default_chunks(arr)
+    shape = arr.shape
+    if not kwargs.get('dims'):
+        kwargs['dims'] = list(_NI_DIM_NAMES)[:len(shape)]
+    kwargs['coords'] = _filled_coords(kwargs.get('coords', {}),
+                                      kwargs['dims'],
+                                      shape,
+                                      kwargs.get('attrs', {}))
+    return xr.DataArray(da.from_array(arr, **fa_kwargs), **kwargs)
+
+
+def _filled_coords(coords, dims, shape, attrs):
+    # Fill space coordinate axes
+    out_coords = coords.copy()
     for ax_no, ax_name in enumerate(dims):
-        coords[ax_name] = xr.DataArray(
-            np.arange(img.shape[ax_no]),
+        if ax_name not in _NI_SPACE_DIMS or ax_name in out_coords:
+            continue
+        out_coords[ax_name] = xr.DataArray(
+            np.arange(shape[ax_no]),
             dims=[ax_name])
-    if dataobj.ndim > 3 and (TR := meta.get("RepetitionTime")):
-        dims += (_NI_TIME_DIM,)
-        time_coords = np.arange(0, (img.shape[-1]) * TR, TR)
-        coords[_NI_TIME_DIM] = xr.DataArray(
-            time_coords,
-            dims=[_NI_TIME_DIM],
-            attrs={"units": "s"})
-    return xr.DataArray(
-        da.from_array(dataobj, chunks=dataobj.chunk_sizes()),
-        dims=dims,
-        coords=coords,
-        name=_url2name(url_or_path),
-        # NB: zarr can't serialize numpy arrays as attrs
-        attrs=meta)
+    if _NI_TIME_DIM not in dims:
+        return out_coords
+    # Consider special cases for: hz, ppm, rad
+    # https://nifti.nimh.nih.gov/nifti-1/documentation/nifti1fields/nifti1fields_pages/xyzt_units.html
+    # Maybe set attrs['xib-time-unts'] from header, and use here.
+    TR = attrs.get("RepetitionTime")
+    if not TR:
+        return out_coords
+    # Add time axis coordinates.
+    n_time = shape[dims.index(_NI_TIME_DIM)]
+    out_coords[_NI_TIME_DIM] = xr.DataArray(
+        np.arange(0, n_time) * TR,
+        dims=[_NI_TIME_DIM],
+        attrs={"units": "s"})
+    return out_coords
 
 
 def _url2name(url_or_path):
     name = drop_suffix(url_or_path, _comp_exts())
     return Path(name).stem
 
 
@@ -676,25 +792,24 @@
         img_uop = replace_suffix(url_or_path, '.json', '.nii.gz')
     else:
         img_uop = url_or_path
         json_uop = replace_suffix(
             drop_suffix(url_or_path, _comp_exts()),
             (),
             '.json')
-    sidecar_file, img_file = fsspec.open_files((json_uop, img_uop),
-                                               mode='wt',
-                                               compression='infer',
-                                               **kwargs)
+    img_file = fsspec.open(img_uop, compression='infer', **kwargs)
+    sidecar_kwargs = merge(kwargs, {'mode': 'wt'})
+    sidecar_file = img_file.fs.open(json_uop, **sidecar_kwargs)
     with sidecar_file as f:
         f.write(_jdumps(attrs))
     if 'local' in img_file.fs.protocol:
         nib.save(nib_img, img_file.path)
         return
     # Not local - use stream interface.
-    img_klass = _path2class(img_uop.full_name)
+    img_klass = _path2class(img_uop.path)
     # We are passing out opened fsspec files.
     with img_uop as fh:
         img_klass.to_file_map({'image': fh})
 
 
 class Processors:
 
@@ -776,15 +891,15 @@
     ximg = ximg.transpose(*order).expand_dims(dims, axes)
     # Adjust affines to current state of ximg.
     back = ximg.xi.with_updated_affines()
     # Build preliminary header.
     hdr = nib.Nifti1Header()
     hdr.set_data_shape(back.shape)
     # Build header from attributes.
-    hdr = Meta2NiHeader(hdr, back.attrs).updated_header()
+    hdr = Attrs2NiHeader(hdr, back.attrs).updated_header()
     return nib.Nifti1Image(back, None, hdr), back.attrs
 
 
 @xr.register_dataarray_accessor("xi")
 class XiAccessor:
 
     def __init__(self, xarray_obj):
@@ -803,14 +918,37 @@
         -----
         Returned `affines` are copies; if you modify the arrays in `affines`,
         this will not affect the original image.
         """
         aff_d = self._obj.attrs.get('xib-affines', {})
         return {space: np.array(aff) for space, aff in aff_d.items()}
 
+    def set_affines(self, affines):
+        """ Set spatial affines to attributes of image
+
+        Affines overwrite existing affines.  If the affine does not exist, we
+        append to the affines dictionary.
+
+        Parameters
+        ----------
+        affines : dict
+            Dictionary where key, value pairs are affine space name and 4x4
+            affine array, respectively.
+
+        Notes
+        -----
+        Set `affines` are copies; if you modify the arrays in `affines`,
+        this will not affect the image affines.  The set affines overwrite
+        correspnding existing affines.
+        """
+        aff_d = self._obj.attrs.get('xib-affines', {})
+        for space, aff in affines.items():
+            aff_d[space] = np.array(aff)
+        self._obj.attrs['xib-affines'] = aff_d
+
     def with_updated_affines(self):
         """ Return image with affines, coordinates updated to match state.
 
         Return image `adj_img` where the affines and coordinates correctly
         reflect any detected slicing of the original image.
 
         Returns
@@ -842,15 +980,15 @@
         for i, name in enumerate(_NI_SPACE_DIMS):
             vox_indices = np.ravel(coords.get(name, 0))
             vox_origin[i] = vox_indices[0]
             if len(vox_indices) > 1:
                 vd = np.diff(vox_indices)
                 if any(vd[1:] != vd[0]):
                     raise XibFormatError(
-                        'Cannot handle irregular voxel spacing for {name}')
+                        f'Cannot handle irregular voxel spacing for "{name}"')
                 vox_scalings[i] = vd[0]
         return from_matvec(affine[:3, :3] * vox_scalings,
                            apply_affine(affine, vox_origin))
 
     def _with_reset_coordinates(self):
         ximg = self._obj
         coords = {}
```

### Comparing `xibabel-0.0.1b4/src/xibabel/testing/__init__.py` & `xibabel-0.0.1rc1/src/xibabel/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `xibabel-0.0.1b4/src/xibabel/testing/__main__.py` & `xibabel-0.0.1rc1/src/xibabel/testing/__main__.py`

 * *Files identical despite different names*

### Comparing `xibabel-0.0.1b4/src/xibabel/testing/fetcher.py` & `xibabel-0.0.1rc1/src/xibabel/testing/fetcher.py`

 * *Files identical despite different names*

### Comparing `xibabel-0.0.1b4/src/xibabel/tests/conftest.py` & `xibabel-0.0.1rc1/src/xibabel/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `xibabel-0.0.1b4/src/xibabel/tests/run_server.py` & `xibabel-0.0.1rc1/src/xibabel/tests/run_server.py`

 * *Files identical despite different names*

### Comparing `xibabel-0.0.1b4/src/xibabel/tests/test_merge.py` & `xibabel-0.0.1rc1/src/xibabel/tests/test_merge.py`

 * *Files identical despite different names*

### Comparing `xibabel-0.0.1b4/src/xibabel/tests/test_scripting.py` & `xibabel-0.0.1rc1/src/xibabel/tests/test_scripting.py`

 * *Files identical despite different names*

### Comparing `xibabel-0.0.1b4/src/xibabel/tests/test_testing.py` & `xibabel-0.0.1rc1/src/xibabel/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `xibabel-0.0.1b4/src/xibabel/xutils.py` & `xibabel-0.0.1rc1/src/xibabel/xutils.py`

 * *Files identical despite different names*

### Comparing `xibabel-0.0.1b4/PKG-INFO` & `xibabel-0.0.1rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xibabel
-Version: 0.0.1b4
+Version: 0.0.1rc1
 Summary: Xibabel neuroimaging interface
 Author-email: Matthew Brett <matthew.brett@gmail.com>, Paul Ivanov <pi@berkeley.edu>, "Christopher J. Markiewicz" <markiewicz@stanford.edu>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 3 - Alpha
 Requires-Dist: xarray
@@ -99,28 +99,28 @@
   the point at which you need the data in memory.
 - Xarrays and Dask allow new storage formats, including storage as
   [Zarr](https://zarr.readthedocs.io) and
   HDF5 / [netCDF](https://en.wikipedia.org/wiki/NetCDF).
 - You can optimize the on-disk format for memory and CPU by adjusting
   _chunking_. We are working on performance metrics for different processing
   steps.
-- Xibabel uses [fsspec](https://filesystem-spec.readthedocs.io) for reading
+- Xibabel uses [`fsspec`](https://filesystem-spec.readthedocs.io) for reading
   NIfTI and other files, allowing you to use many filesystems as the source for
-  your data, including HTTP, Amazon, Google Cloud and others. See the FSSpec
+  your data, including HTTP, Amazon, Google Cloud and others. See the `fsspec`
   documentation for details, and the code above for an example using HTTP as
   a backing store.
 
 ## Status
 
 Xibabel is in development mode at the moment. We are still experimenting with
 the API. We'd love to hear from you if you are interested to help. Please do
 not rely on any particular features in this alpha version, including
 compatibility of file formats; prefer to save outputs as BIDS / NIfTI format,
 for which we do guarantee input compatibility (e.g. `xib.save(ximg,
-'out.nii.gz'`).
+'out.nii.gz')`).
 
 ## Install
 
 From Pip — the current pre-release:
 
 ```bash
 pip install --pre xarray
```

