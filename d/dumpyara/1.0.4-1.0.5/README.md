# Comparing `tmp/dumpyara-1.0.4.tar.gz` & `tmp/dumpyara-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dumpyara-1.0.4.tar", max compression
+gzip compressed data, was "dumpyara-1.0.5.tar", max compression
```

## Comparing `dumpyara-1.0.4.tar` & `dumpyara-1.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1235 2024-02-23 13:42:11.844459 dumpyara-1.0.4/README.md
--rw-r--r--   0        0        0      215 2024-02-23 13:48:05.797452 dumpyara-1.0.4/dumpyara/__init__.py
--rw-r--r--   0        0        0      166 2024-02-23 13:42:11.844459 dumpyara-1.0.4/dumpyara/__main__.py
--rw-r--r--   0        0        0     2240 2024-02-23 13:42:11.844459 dumpyara-1.0.4/dumpyara/dumpyara.py
--rw-r--r--   0        0        0      249 2024-02-23 13:42:11.844459 dumpyara-1.0.4/dumpyara/lib/liberofs/__init__.py
--rw-r--r--   0        0        0     1061 2024-02-23 13:42:11.844459 dumpyara-1.0.4/dumpyara/lib/libpayload/LICENSE
--rw-r--r--   0        0        0     4190 2024-02-23 13:42:11.844459 dumpyara-1.0.4/dumpyara/lib/libpayload/__init__.py
--rw-r--r--   0        0        0     7291 2024-02-23 13:42:11.847792 dumpyara-1.0.4/dumpyara/lib/libpayload/update_metadata_pb2.py
--rw-r--r--   0        0        0     5148 2024-02-23 13:42:11.847792 dumpyara-1.0.4/dumpyara/lib/libsdat2img/__init__.py
--rw-r--r--   0        0        0      234 2024-02-23 13:42:11.847792 dumpyara-1.0.4/dumpyara/lib/libsevenz/__init__.py
--rw-r--r--   0        0        0     1047 2024-02-23 13:42:11.847792 dumpyara-1.0.4/dumpyara/main.py
--rw-r--r--   0        0        0      112 2024-02-23 13:42:11.847792 dumpyara-1.0.4/dumpyara/steps/__init__.py
--rw-r--r--   0        0        0      656 2024-02-23 13:42:11.847792 dumpyara-1.0.4/dumpyara/steps/extract_archive.py
--rw-r--r--   0        0        0     1719 2024-02-23 13:42:11.847792 dumpyara-1.0.4/dumpyara/steps/extract_images.py
--rw-r--r--   0        0        0     1481 2024-02-23 13:42:11.847792 dumpyara-1.0.4/dumpyara/steps/prepare_images.py
--rw-r--r--   0        0        0      961 2024-02-23 13:42:11.847792 dumpyara-1.0.4/dumpyara/utils/bootimg.py
--rw-r--r--   0        0        0     1137 2024-02-23 13:42:11.847792 dumpyara-1.0.4/dumpyara/utils/files.py
--rw-r--r--   0        0        0      352 2024-02-23 13:42:11.847792 dumpyara-1.0.4/dumpyara/utils/logging.py
--rw-r--r--   0        0        0      993 2024-02-23 13:42:11.847792 dumpyara-1.0.4/dumpyara/utils/multipartitions.py
--rw-r--r--   0        0        0     4957 2024-02-23 13:42:11.847792 dumpyara-1.0.4/dumpyara/utils/partitions.py
--rw-r--r--   0        0        0     1777 2024-02-23 13:42:11.847792 dumpyara-1.0.4/dumpyara/utils/raw_image.py
--rw-r--r--   0        0        0     1100 2024-02-23 13:42:11.847792 dumpyara-1.0.4/dumpyara/utils/sparsed_images.py
--rw-r--r--   0        0        0      556 2024-02-23 13:48:00.347406 dumpyara-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     2144 1970-01-01 00:00:00.000000 dumpyara-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1304 2024-04-10 18:38:03.743982 dumpyara-1.0.5/README.md
+-rw-r--r--   0        0        0      215 2024-04-13 19:54:43.719360 dumpyara-1.0.5/dumpyara/__init__.py
+-rw-r--r--   0        0        0      166 2022-02-24 11:26:29.453827 dumpyara-1.0.5/dumpyara/__main__.py
+-rw-r--r--   0        0        0     2273 2024-04-10 10:30:16.574915 dumpyara-1.0.5/dumpyara/dumpyara.py
+-rw-r--r--   0        0        0      249 2024-02-22 14:20:03.637781 dumpyara-1.0.5/dumpyara/lib/liberofs/__init__.py
+-rw-r--r--   0        0        0     1061 2022-04-13 02:01:29.000000 dumpyara-1.0.5/dumpyara/lib/libpayload/LICENSE
+-rw-r--r--   0        0        0     4190 2022-04-13 13:16:39.682675 dumpyara-1.0.5/dumpyara/lib/libpayload/__init__.py
+-rw-r--r--   0        0        0     7291 2022-06-29 23:18:10.039907 dumpyara-1.0.5/dumpyara/lib/libpayload/update_metadata_pb2.py
+-rw-r--r--   0        0        0     5148 2022-02-25 10:28:46.742568 dumpyara-1.0.5/dumpyara/lib/libsdat2img/__init__.py
+-rw-r--r--   0        0        0      336 2024-04-10 10:30:16.614915 dumpyara-1.0.5/dumpyara/lib/libsevenzip/__init__.py
+-rw-r--r--   0        0        0     1131 2024-04-13 19:58:24.279471 dumpyara-1.0.5/dumpyara/main.py
+-rw-r--r--   0        0        0      112 2023-03-13 23:23:23.165706 dumpyara-1.0.5/dumpyara/steps/__init__.py
+-rw-r--r--   0        0        0     1831 2024-04-10 16:48:32.161503 dumpyara-1.0.5/dumpyara/steps/extract_archive.py
+-rw-r--r--   0        0        0     1725 2024-04-10 10:30:16.614915 dumpyara-1.0.5/dumpyara/steps/extract_images.py
+-rw-r--r--   0        0        0     1622 2024-04-10 16:50:48.741049 dumpyara-1.0.5/dumpyara/steps/prepare_images.py
+-rw-r--r--   0        0        0      961 2024-02-22 14:38:13.604100 dumpyara-1.0.5/dumpyara/utils/bootimg.py
+-rw-r--r--   0        0        0     1137 2023-03-13 23:30:07.843483 dumpyara-1.0.5/dumpyara/utils/files.py
+-rw-r--r--   0        0        0     1107 2024-04-10 18:32:49.324963 dumpyara-1.0.5/dumpyara/utils/multipartitions.py
+-rw-r--r--   0        0        0     4957 2024-04-10 18:29:47.692186 dumpyara-1.0.5/dumpyara/utils/partitions.py
+-rw-r--r--   0        0        0     2257 2024-04-10 18:35:00.421223 dumpyara-1.0.5/dumpyara/utils/raw_image.py
+-rw-r--r--   0        0        0      696 2024-04-10 15:32:58.328024 dumpyara-1.0.5/dumpyara/utils/shutil.py
+-rw-r--r--   0        0        0     1100 2023-03-13 23:55:49.868282 dumpyara-1.0.5/dumpyara/utils/sparsed_images.py
+-rw-r--r--   0        0        0      597 2024-04-13 19:54:40.169358 dumpyara-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2289 1970-01-01 00:00:00.000000 dumpyara-1.0.5/PKG-INFO
```

### Comparing `dumpyara-1.0.4/README.md` & `dumpyara-1.0.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -17,22 +17,25 @@
 python3 -m dumpyara <path to OTA file>
 ```
 
 ## Supported formats
 
 ### Step 1 - Archives
 -   All the ones supported by shutil's extract_archive
+-   Samsung's `.tar.md5` archives
+-   Nested archives
 
 ### Step 2 - What's inside the archive
 -   A-only OTAs (Brotli and/or sdat compressed)
 -   A/B OTAs
 -   Dynamic partitions (super.img)
 -   payload.bin
 -   Raw images (e.g. Xiaomi fastboot packages)
 -   Sparse images
+-   LZ4 images
 
 ### Step 3 - Partition images
 -   Android boot images
 -   7z supported archives/images
 -   EROFS images using erofs-utils
 
 ## Credits
```

### Comparing `dumpyara-1.0.4/dumpyara/dumpyara.py` & `dumpyara-1.0.5/dumpyara/dumpyara.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,17 @@
 	# Temporary directories
 	extracted_archive_path = output_path / "temp_extracted_archive"
 	raw_images_path = output_path / "temp_raw_images"
 
 	# First, check the necessary tools are installed
 	for tool, package in REQUIRED_TOOLS.items():
 		if not which(tool):
-			raise RuntimeError(f"Please install {package} from your distro's repositories")
+			raise RuntimeError(
+				f"You are missing {tool}, please install {package} from your distro's repositories"
+			)
 
 	try:
 		# Make output and temporary directories
 		output_path.mkdir(exist_ok=True)
 		extracted_archive_path.mkdir()
 		raw_images_path.mkdir()
```

### Comparing `dumpyara-1.0.4/dumpyara/lib/libpayload/LICENSE` & `dumpyara-1.0.5/dumpyara/lib/libpayload/LICENSE`

 * *Files identical despite different names*

### Comparing `dumpyara-1.0.4/dumpyara/lib/libpayload/__init__.py` & `dumpyara-1.0.5/dumpyara/lib/libpayload/__init__.py`

 * *Files identical despite different names*

### Comparing `dumpyara-1.0.4/dumpyara/lib/libpayload/update_metadata_pb2.py` & `dumpyara-1.0.5/dumpyara/lib/libpayload/update_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `dumpyara-1.0.4/dumpyara/lib/libsdat2img/__init__.py` & `dumpyara-1.0.5/dumpyara/lib/libsdat2img/__init__.py`

 * *Files identical despite different names*

### Comparing `dumpyara-1.0.4/dumpyara/main.py` & `dumpyara-1.0.5/dumpyara/main.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 #
 # SPDX-License-Identifier: GPL-3.0
 #
 
 from argparse import ArgumentParser
 from dumpyara import __version__ as version, current_path
 from dumpyara.dumpyara import dumpyara
-from dumpyara.utils.logging import setup_logging
+from dumpyara.utils.shutil import setup_shutil_formats
 from pathlib import Path
 from sebaubuntu_libs.liblocale import setup_locale
+from sebaubuntu_libs.liblogging import setup_logging
 
 def main():
 	print(f"Dumpyara\n"
 	      f"Version {version}\n")
 
 	parser = ArgumentParser(prog='python3 -m dumpyara')
 
@@ -29,14 +30,16 @@
 
 	args = parser.parse_args()
 
 	setup_locale()
 
 	setup_logging(args.debug)
 
+	setup_shutil_formats()
+
 	output = current_path / args.file.stem
 	if args.output:
 		output = args.output
 
 	output_path = dumpyara(args.file, output, args.debug)
 
 	print(f"\nDone! You can find the dump in {str(output_path)}")
```

### Comparing `dumpyara-1.0.4/dumpyara/steps/extract_images.py` & `dumpyara-1.0.5/dumpyara/steps/extract_images.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from pathlib import Path
 from dumpyara.lib.liberofs import erofs
 from sebaubuntu_libs.libexception import format_exception
 from sebaubuntu_libs.liblogging import LOGD, LOGE, LOGI
 from shutil import copyfile
 from subprocess import CalledProcessError
 
-from dumpyara.lib.libsevenz import sevenz
+from dumpyara.lib.libsevenzip import sevenzip
 from dumpyara.utils.bootimg import extract_bootimg
 from dumpyara.utils.partitions import (
 	BOOTIMAGE, FILESYSTEM, RAW,
     PARTITIONS,
 	get_partition_names,
 )
 
@@ -46,14 +46,14 @@
 				LOGE(f"{format_exception(e)}")
 		elif partition_type == FILESYSTEM:
 			try:
 				erofs(f'--extract="{output_path / partition}" {image_path}')
 			except CalledProcessError as e:
 				LOGD(f"Failed to extract {image_path.name} with erofs, trying 7z")
 				try:
-					sevenz(f'x {image_path} -y -o"{output_path / partition}"/')
+					sevenzip(f'x {image_path} -y -o"{output_path / partition}"/')
 				except CalledProcessError as e:
 					LOGE(f"Error extracting {image_path.name}")
 					LOGE(f"{e.output.decode('UTF-8', errors='ignore')}")
 
 		if partition_type in (RAW, BOOTIMAGE):
 			copyfile(image_path, output_path / f"{partition}.img", follow_symlinks=True)
```

### Comparing `dumpyara-1.0.4/dumpyara/steps/prepare_images.py` & `dumpyara-1.0.5/dumpyara/steps/prepare_images.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,48 +5,55 @@
 #
 """
 Step 2.
 
 This step will convert the archive files to raw images ready to be extracted.
 """
 
-import fnmatch
 from pathlib import Path
 from sebaubuntu_libs.liblogging import LOGI
 
 from dumpyara.utils.files import get_recursive_files_list
 from dumpyara.utils.multipartitions import MULTIPARTITIONS
 from dumpyara.utils.partitions import (
-    correct_ab_filenames,
+	correct_ab_filenames,
 	fix_aliases,
 	prepare_raw_images,
 )
 from dumpyara.utils.sparsed_images import prepare_sparsed_images
 
 def prepare_images(extracted_archive_path: Path, raw_images_path: Path):
 	"""
 	Convert the archive files to raw images ready to be extracted.
 	"""
-    # Check for sparsed images
+
+	# Check for sparsed images
 	prepare_sparsed_images(extracted_archive_path)
 
+	# Check for partitions
+	prepare_raw_images(extracted_archive_path, raw_images_path)
+
 	# Check for multipartitions
-	extracted_archive_tempdir_files_list = list(get_recursive_files_list(extracted_archive_path, True, True))
+	extracted_archive_tempdir_files_list = list(get_recursive_files_list(extracted_archive_path, True))
 	for pattern, func in MULTIPARTITIONS.items():
-		match = fnmatch.filter(extracted_archive_tempdir_files_list, pattern)
-		if not match:
-			LOGI(f"Pattern {pattern} not found")
+		matches = [
+			file for file in extracted_archive_tempdir_files_list
+			if pattern.match(str(file))
+		]
+
+		if not matches:
+			LOGI(f"Pattern {pattern.pattern} not found")
 			continue
 
-		for file in match:
+		for file in matches:
 			multipart_image = extracted_archive_path / file
 			LOGI(f"Found multipartition image: {multipart_image.name}")
 			func(multipart_image, raw_images_path)
 
-	# Check for partitions
+	# Check for partitions again, in case of multipartitions
 	prepare_raw_images(extracted_archive_path, raw_images_path)
 
 	# Fix slotted filenames if needed
 	correct_ab_filenames(raw_images_path)
 
 	# Fix aliases
 	fix_aliases(raw_images_path)
```

### Comparing `dumpyara-1.0.4/dumpyara/utils/bootimg.py` & `dumpyara-1.0.5/dumpyara/utils/bootimg.py`

 * *Files identical despite different names*

### Comparing `dumpyara-1.0.4/dumpyara/utils/files.py` & `dumpyara-1.0.5/dumpyara/utils/files.py`

 * *Files identical despite different names*

### Comparing `dumpyara-1.0.4/dumpyara/utils/multipartitions.py` & `dumpyara-1.0.5/dumpyara/utils/multipartitions.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 #
 # SPDX-License-Identifier: GPL-3.0
 #
 
 from typing import Callable, Dict
 from liblp.partition_tools.lpunpack import lpunpack
 from pathlib import Path
+from re import Pattern, compile
 from sebaubuntu_libs.liblogging import LOGI
 from shutil import move
 from subprocess import STDOUT, check_output
 
 from dumpyara.lib.libpayload import extract_android_ota_payload
 
 def extract_payload(image: Path, output_dir: Path):
@@ -27,11 +28,14 @@
 		move(unsparsed_super, image)
 
 	if unsparsed_super.is_file():
 		unsparsed_super.unlink()
 
 	lpunpack(image, output_dir)
 
-MULTIPARTITIONS: Dict[str, Callable[[Path, Path], None]] = {
-	"*payload.bin*": extract_payload,
-	"*super*": extract_super,
+MULTIPARTITIONS: Dict[Pattern[str], Callable[[Path, Path], None]] = {
+	compile(key): value
+	for key, value in {
+		"payload.bin": extract_payload,
+		"super(?!.*(_empty)).*\\.img": extract_super,
+	}.items()
 }
```

### Comparing `dumpyara-1.0.4/dumpyara/utils/partitions.py` & `dumpyara-1.0.5/dumpyara/utils/partitions.py`

 * *Files identical despite different names*

### Comparing `dumpyara-1.0.4/dumpyara/utils/raw_image.py` & `dumpyara-1.0.5/dumpyara/utils/raw_image.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,62 +2,75 @@
 # Copyright (C) 2022 Dumpyara Project
 #
 # SPDX-License-Identifier: GPL-3.0
 #
 
 import brotli
 from dumpyara.lib.libsdat2img import main as sdat2img
+import io
+from lz4.frame import LZ4FrameFile
 from pathlib import Path
-from sebaubuntu_libs.liblogging import LOGI
+from sebaubuntu_libs.liblogging import LOGD, LOGI
 from shutil import copyfile, move
 from subprocess import STDOUT, check_output
 
 def get_raw_image(partition: str, files_path: Path, output_image_path: Path):
 	"""
 	Convert a partition image to a raw image.
 
 	This function handles brotli compression, sdat and sparse images.
 	"""
 	brotli_image = files_path / f"{partition}.new.dat.br"
 	dat_image = files_path / f"{partition}.new.dat"
 	transfer_list = files_path / f"{partition}.transfer.list"
+	lz4_image = files_path / f"{partition}.img.lz4"
 	raw_image = files_path / f"{partition}.img"
 	unsparsed_image = files_path / f"{partition}.unsparsed.img"
 	possible_image_names = [
 		f"{partition}",
 		f"{partition}.bin",
 		f"{partition}.ext4",
 		f"{partition}.image",
 		f"{partition}.img",
+		f"{partition}.img.ext4",
 		f"{partition}.mbn",
 		f"{partition}.raw",
 		f"{partition}.raw.img",
 	]
 
 	if brotli_image.is_file():
-		LOGI(f"Decompressing {brotli_image.name}")
+		LOGI(f"Decompressing {brotli_image.name} as brotli image")
 		dat_image.write_bytes(brotli.decompress(brotli_image.read_bytes()))
 
 	if dat_image.is_file() and transfer_list.is_file():
 		LOGI(f"Converting {dat_image.name} to {raw_image.name}")
 		sdat2img(transfer_list, dat_image, raw_image)
 
+	if lz4_image.is_file():
+		LOGI(f"Decompressing {lz4_image.name} as LZ4 image")
+		with LZ4FrameFile(lz4_image, mode="rb") as lz4_image:
+			with io.open(raw_image, "wb") as raw_image:
+				raw_image.write(lz4_image.read())
+
 	for image_name in possible_image_names:
 		image_path = files_path / image_name
 		if not image_path.is_file():
 			continue
 
 		try:
 			check_output(["simg2img", image_path, unsparsed_image], stderr=STDOUT) # TODO: Rewrite libsparse...
 		except Exception:
+			LOGD(f"Failed to unsparse {image_path.name}, should be a raw image")
 			pass
 		else:
 			move(unsparsed_image, image_path)
 
 		if unsparsed_image.is_file():
 			unsparsed_image.unlink()
 
 		LOGI(f"Copying {image_path.name}")
 		copyfile(image_path, output_image_path, follow_symlinks=True)
 		return True
 
+	LOGD(f"Partition {partition} not found")
+
 	return False
```

### Comparing `dumpyara-1.0.4/dumpyara/utils/sparsed_images.py` & `dumpyara-1.0.5/dumpyara/utils/sparsed_images.py`

 * *Files identical despite different names*

### Comparing `dumpyara-1.0.4/PKG-INFO` & `dumpyara-1.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dumpyara
-Version: 1.0.4
+Version: 1.0.5
 Summary: Android firmware extractor
 Home-page: https://github.com/sebaubuntu-python/dumpyara
 License: GPL-3.0
 Author: Sebastiano Barezzi
 Author-email: seba@sebaubuntu.dev
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -12,15 +12,17 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: Brotli (>=1.0.9,<2.0.0)
 Requires-Dist: liblp (>=1.0.2,<2.0.0)
-Requires-Dist: protobuf (>=4.22.1,<5.0.0)
+Requires-Dist: lz4 (>=4.3.3,<5.0.0)
+Requires-Dist: protobuf (>=4.22.1,<6.0.0)
+Requires-Dist: py7zr (>=0.21.0,<0.22.0)
 Requires-Dist: sebaubuntu-libs (>=1.4.2,<2.0.0)
 Project-URL: Repository, https://github.com/sebaubuntu-python/dumpyara
 Description-Content-Type: text/markdown
 
 # dumpyara
 
 [![PyPI version](https://img.shields.io/pypi/v/dumpyara)](https://pypi.org/project/dumpyara/)
@@ -40,22 +42,25 @@
 python3 -m dumpyara <path to OTA file>
 ```
 
 ## Supported formats
 
 ### Step 1 - Archives
 -   All the ones supported by shutil's extract_archive
+-   Samsung's `.tar.md5` archives
+-   Nested archives
 
 ### Step 2 - What's inside the archive
 -   A-only OTAs (Brotli and/or sdat compressed)
 -   A/B OTAs
 -   Dynamic partitions (super.img)
 -   payload.bin
 -   Raw images (e.g. Xiaomi fastboot packages)
 -   Sparse images
+-   LZ4 images
 
 ### Step 3 - Partition images
 -   Android boot images
 -   7z supported archives/images
 -   EROFS images using erofs-utils
 
 ## Credits
```

