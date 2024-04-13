# Comparing `tmp/PyCatFile-0.7.6.tar.gz` & `tmp/PyCatFile-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyCatFile-0.7.6.tar", last modified: Thu Apr 11 01:29:34 2024, max compression
+gzip compressed data, was "PyCatFile-0.7.8.tar", last modified: Sat Apr 13 01:28:31 2024, max compression
```

## Comparing `PyCatFile-0.7.6.tar` & `PyCatFile-0.7.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:29:34.890832 PyCatFile-0.7.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-11 01:29:24.000000 PyCatFile-0.7.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-11 01:29:34.890832 PyCatFile-0.7.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:29:34.890832 PyCatFile-0.7.6/PyCatFile.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-11 01:29:34.000000 PyCatFile-0.7.6/PyCatFile.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-11 01:29:34.000000 PyCatFile-0.7.6/PyCatFile.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 01:29:34.000000 PyCatFile-0.7.6/PyCatFile.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-11 01:29:34.000000 PyCatFile-0.7.6/PyCatFile.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 01:29:34.000000 PyCatFile-0.7.6/PyCatFile.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-11 01:29:24.000000 PyCatFile-0.7.6/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     7356 2024-04-11 01:29:24.000000 PyCatFile-0.7.6/catfile.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4969 2024-04-11 01:29:24.000000 PyCatFile-0.7.6/neocatfile.py
--rwxr-xr-x   0 runner    (1001) docker     (127)   332511 2024-04-11 01:29:24.000000 PyCatFile-0.7.6/pycatfile.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-11 01:29:34.890832 PyCatFile-0.7.6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     5451 2024-04-11 01:29:24.000000 PyCatFile-0.7.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:28:31.939092 PyCatFile-0.7.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-13 01:28:23.000000 PyCatFile-0.7.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-13 01:28:31.939092 PyCatFile-0.7.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:28:31.939092 PyCatFile-0.7.8/PyCatFile.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-13 01:28:31.000000 PyCatFile-0.7.8/PyCatFile.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-13 01:28:31.000000 PyCatFile-0.7.8/PyCatFile.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 01:28:31.000000 PyCatFile-0.7.8/PyCatFile.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-13 01:28:31.000000 PyCatFile-0.7.8/PyCatFile.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 01:28:31.000000 PyCatFile-0.7.8/PyCatFile.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-13 01:28:23.000000 PyCatFile-0.7.8/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7310 2024-04-13 01:28:23.000000 PyCatFile-0.7.8/catfile.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4969 2024-04-13 01:28:23.000000 PyCatFile-0.7.8/neocatfile.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)   322887 2024-04-13 01:28:23.000000 PyCatFile-0.7.8/pycatfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-13 01:28:31.939092 PyCatFile-0.7.8/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5451 2024-04-13 01:28:23.000000 PyCatFile-0.7.8/setup.py
```

### Comparing `PyCatFile-0.7.6/LICENSE` & `PyCatFile-0.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `PyCatFile-0.7.6/PKG-INFO` & `PyCatFile-0.7.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyCatFile
-Version: 0.7.6
+Version: 0.7.8
 Summary: A tar like file format name catfile after unix cat command (concatenate files) .
 Home-page: https://github.com/GameMaker2k/PyCatFile
 Download-URL: https://github.com/GameMaker2k/PyCatFile/archive/master.tar.gz
 Author: Kazuki Przyborowski
 Author-email: kazuki.przyborowski@gmail.com
 Maintainer: Kazuki Przyborowski
 Maintainer-email: kazuki.przyborowski@gmail.com
```

### Comparing `PyCatFile-0.7.6/PyCatFile.egg-info/PKG-INFO` & `PyCatFile-0.7.8/PyCatFile.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyCatFile
-Version: 0.7.6
+Version: 0.7.8
 Summary: A tar like file format name catfile after unix cat command (concatenate files) .
 Home-page: https://github.com/GameMaker2k/PyCatFile
 Download-URL: https://github.com/GameMaker2k/PyCatFile/archive/master.tar.gz
 Author: Kazuki Przyborowski
 Author-email: kazuki.przyborowski@gmail.com
 Maintainer: Kazuki Przyborowski
 Maintainer-email: kazuki.przyborowski@gmail.com
```

### Comparing `PyCatFile-0.7.6/catfile.py` & `PyCatFile-0.7.8/catfile.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2018-2024 Cool Dude 2k - http://idb.berlios.de/
     Copyright 2018-2024 Game Maker 2k - http://intdb.sourceforge.net/
     Copyright 2018-2024 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: catfile.py - Last Update: 4/10/2024 Ver. 0.7.6 RC 1 - Author: cooldude2k $
+    $FileInfo: catfile.py - Last Update: 4/12/2024 Ver. 0.7.8 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import argparse, pycatfile, binascii;
 
 rarfile_support = pycatfile.rarfile_support;
 
@@ -39,35 +39,35 @@
 __version_date_info__ = pycatfile.__version_date_info__;
 __version_date__ = pycatfile.__version_date__;
 __version_date_plusrc__ = pycatfile.__version_date_plusrc__;
 __version__ = pycatfile.__version__;
 
 argparser = argparse.ArgumentParser(description="Manipulate concatenated files.", conflict_handler="resolve", add_help=True);
 argparser.add_argument("-V", "--version", action="version", version=__program_name__ + " " + __version__);
-argparser.add_argument("-i", "-f", "--input", help="Specify the file(s) to concatenate or the concatenated file to extract.", required=True);
-argparser.add_argument("-d", "-v", "--verbose", action="store_true", help="Enable verbose mode to display various debugging information.");
+argparser.add_argument("-i", "--input", help="Specify the file(s) to concatenate or the concatenated file to extract.", required=True);
+argparser.add_argument("-d", "--verbose", action="store_true", help="Enable verbose mode to display various debugging information.");
 argparser.add_argument("-c", "--create", action="store_true", help="Perform concatenation operation only.");
-argparser.add_argument("-I", "-validate", "--validate", action="store_true", help="Validate CatFile checksums");
-argparser.add_argument("-C", "-checksum", "--checksum", default="crc32", help="Specify the type of checksum to use. Default is crc32.");
-argparser.add_argument("-S", "-skipchecksum", "--skipchecksum", action="store_true", help="Skip checksum check of files.");
-argparser.add_argument("-e", "-x", "--extract", action="store_true", help="Perform extraction operation only.");
-argparser.add_argument("-F", "-format", "--format", default=__file_format_list__[0], help="Specify the format to use");
-argparser.add_argument("-D", "-delimiter", "--delimiter", default=__file_format_list__[5], help="Specify the format to use");
-argparser.add_argument("-m", "-formatver", "--formatver", default=__file_format_list__[6], help="Specify the format version");
-argparser.add_argument("-l", "-t", "--list", action="store_true", help="List files included in the concatenated file.");
-argparser.add_argument("-p", "-preserve", "--preserve", action="store_false", help="Preserve permissions and time of files");
-argparser.add_argument("-R", "-repack", "--repack", action="store_true", help="Re-concatenate files, fixing checksum errors if any.");
-argparser.add_argument("-o", "--output", default=None, help="Specify the name for the extracted concatenated files or the output concatenated file.");
-argparser.add_argument("-P", "-compression", "--compression", default="auto", help="Specify the compression method to use for concatenation.");
-argparser.add_argument("-L", "-level", "--level", default=None, help="Specify the compression level for concatenation.");
-argparser.add_argument("-t", "-tar", "--converttar", action="store_true", help="Convert a tar file to a catfile.");
-argparser.add_argument("-z", "-zip", "--convertzip", action="store_true", help="Convert a zip file to a catfile.");
-argparser.add_argument("-r", "-rar", "--convertrar", action="store_true", help="Convert a rar file to a catfile.");
+argparser.add_argument("-v", "--validate", action="store_true", help="Validate CatFile checksums.");
+argparser.add_argument("-C", "--checksum", default="crc32", help="Specify the type of checksum to use. The default is crc32.");
+argparser.add_argument("-s", "--skipchecksum", action="store_true", help="Skip the checksum check of files.");
+argparser.add_argument("-e", "--extract", action="store_true", help="Perform extraction operation only.");
+argparser.add_argument("-F", "--format", default=__file_format_list__[0], help="Specify the format to use.");
+argparser.add_argument("-D", "--delimiter", default=__file_format_list__[5], help="Specify the delimiter to use.");
+argparser.add_argument("-m", "--formatver", default=__file_format_list__[6], help="Specify the format version.");
+argparser.add_argument("-l", "--list", action="store_true", help="List files included in the concatenated file.");
+argparser.add_argument("-p", "--preserve", action="store_false", help="Preserve permissions and timestamps of files.");
+argparser.add_argument("-R", "--repack", action="store_true", help="Re-concatenate files, fixing checksum errors, if any.");
+argparser.add_argument("-o", "--output", default=None, help="Specify the name for the extracted or output concatenated files.");
+argparser.add_argument("-P", "--compression", default="auto", help="Specify the compression method to use for concatenation.");
+argparser.add_argument("-L", "--level", default=None, help="Specify the compression level for concatenation.");
+argparser.add_argument("-t", "--converttar", action="store_true", help="Convert a tar file to a CatFile.");
+argparser.add_argument("-z", "--convertzip", action="store_true", help="Convert a zip file to a CatFile.");
+argparser.add_argument("-r", "--convertrar", action="store_true", help="Convert a rar file to a CatFile.");
 argparser.add_argument("-T", "--text", action="store_true", help="Read file locations from a text file.");
-getargs = argparser.parse_args();
+getargs = argparser.parse_args()
 
 fname = getargs.format;
 fnamelower = fname.lower();
 fnamemagic = fname;
 fnamelen = len(fname);
 fnamehex = binascii.hexlify(fname.encode("UTF-8")).decode("UTF-8");
 fnamever = getargs.formatver;
@@ -108,11 +108,14 @@
  elif rarfile_support and getargs.convertrar:
   pycatfile.RarFileListFiles(getargs.input, getargs.verbose, False);
  else:
   pycatfile.ArchiveFileListFiles(getargs.input, 0, 0, getargs.skipchecksum, fnamelist, getargs.verbose, False);
 
 elif should_validate:
  fvalid = pycatfile.ArchiveFileValidate(getargs.input, fnamelist, getargs.verbose, False);
+ if(not getargs.verbose):
+  import sys, logging;
+  logging.basicConfig(format="%(message)s", stream=sys.stdout, level=logging.DEBUG);
  if(fvalid):
   pycatfile.VerbosePrintOut("File is valid: \n" + str(getargs.input));
  else:
   pycatfile.VerbosePrintOut("File is invalid: \n" + str(getargs.input));
```

### Comparing `PyCatFile-0.7.6/neocatfile.py` & `PyCatFile-0.7.8/neocatfile.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2018-2024 Cool Dude 2k - http://idb.berlios.de/
     Copyright 2018-2024 Game Maker 2k - http://intdb.sourceforge.net/
     Copyright 2018-2024 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: neocatfile.py - Last Update: 4/10/2024 Ver. 0.7.6 RC 1 - Author: cooldude2k $
+    $FileInfo: neocatfile.py - Last Update: 4/12/2024 Ver. 0.7.8 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals
 import argparse
 import pycatfile
 
 # Compatibility layer for Python 2 and 3 input
```

### Comparing `PyCatFile-0.7.6/pycatfile.py` & `PyCatFile-0.7.8/pycatfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2018-2024 Cool Dude 2k - http://idb.berlios.de/
     Copyright 2018-2024 Game Maker 2k - http://intdb.sourceforge.net/
     Copyright 2018-2024 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: pycatfile.py - Last Update: 4/10/2024 Ver. 0.7.6 RC 1 - Author: cooldude2k $
+    $FileInfo: pycatfile.py - Last Update: 4/12/2024 Ver. 0.7.8 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import io, os, re, sys, time, stat, zlib, base64, shutil, socket, hashlib, datetime, logging, binascii, tempfile, zipfile, platform;
 from ftplib import FTP, FTP_TLS;
 if(sys.version[0]=="2"):
  from urlparse import urlparse, urlunparse;
@@ -160,19 +160,19 @@
 __file_format_ver__ = "001";
 __use_new_style__ = True;
 __use_advanced_list__ = True;
 __use_alt_inode__ = False;
 __file_format_list__ = [__file_format_name__, __file_format_magic__, __file_format_lower__, __file_format_len__, __file_format_hex__, __file_format_delimiter__, __file_format_ver__, __use_new_style__, __use_advanced_list__, __use_alt_inode__];
 __project__ = __program_name__;
 __project_url__ = "https://github.com/GameMaker2k/PyCatFile";
-__version_info__ = (0, 7, 6, "RC 1", 1);
-__version_date_info__ = (2024, 4, 10, "RC 1", 1);
+__version_info__ = (0, 7, 8, "RC 1", 1);
+__version_date_info__ = (2024, 4, 12, "RC 1", 1);
 __version_date__ = str(__version_date_info__[0]) + "." + str(__version_date_info__[1]).zfill(2) + "." + str(__version_date_info__[2]).zfill(2);
 __revision__ = __version_info__[3];
-__revision_id__ = "$Id: 9f413e59b208687ef02639cef9ddfc34278a2f0e $";
+__revision_id__ = "$Id: 08fb47c714ff74769abf5a6def7842a572a87a9a $";
 if(__version_info__[4] is not None):
  __version_date_plusrc__ = __version_date__ + "-" + str(__version_date_info__[4]);
 if(__version_info__[4] is None):
  __version_date_plusrc__ = __version_date__;
 if(__version_info__[3] is not None):
  __version__ = str(__version_info__[0]) + "." + str(__version_info__[1]) + "." + str(__version_info__[2]) + " " + str(__version_info__[3]);
 if(__version_info__[3] is None):
@@ -2745,15 +2745,15 @@
    ffullmode = member.mode;
    ftype = 12;
   else:
    ffullmode = member.mode;
    ftype = 0;
   flinkname = "";
   fcurfid = format(int(curfid), 'x').lower();
-  fcurinode = format(int(0), 'x').lower();
+  fcurinode = format(int(curfid), 'x').lower();
   curfid = curfid + 1;
   if(ftype==2):
    flinkname = member.linkname;
   fdev_minor = format(int(member.devminor), 'x').lower();
   fdev_major = format(int(member.devmajor), 'x').lower();
   frdev_minor = format(int(member.devminor), 'x').lower();
   frdev_major = format(int(member.devmajor), 'x').lower();
@@ -3014,15 +3014,15 @@
   ftype = 0;
   if(not member.is_dir()):
    ftype = 0;
   elif(member.is_dir()):
    ftype = 5;
   flinkname = "";
   fcurfid = format(int(curfid), 'x').lower();
-  fcurinode = format(int(0), 'x').lower();
+  fcurinode = format(int(curfid), 'x').lower();
   curfid = curfid + 1;
   fdev_minor = format(int(0), 'x').lower();
   fdev_major = format(int(0), 'x').lower();
   frdev_minor = format(int(0), 'x').lower();
   frdev_major = format(int(0), 'x').lower();
   if(ftype==5):
    fsize = format(int("0"), 'x').lower();
@@ -3341,15 +3341,15 @@
     ftype = 2;
    elif(member.is_dir()):
     ftype = 5;
    flinkname = "";
    if(ftype==2):
     flinkname = rarfp.read(member.filename).decode("UTF-8");
    fcurfid = format(int(curfid), 'x').lower();
-   fcurinode = format(int(0), 'x').lower();
+   fcurinode = format(int(curfid), 'x').lower();
    curfid = curfid + 1;
    fdev_minor = format(int(0), 'x').lower();
    fdev_major = format(int(0), 'x').lower();
    frdev_minor = format(int(0), 'x').lower();
    frdev_major = format(int(0), 'x').lower();
    if(ftype==5):
     fsize = format(int("0"), 'x').lower();
@@ -3721,59 +3721,27 @@
    prefccs = preheaderdata[extrastart + 2].lower();
    hc = 0;
    hcmax = len(preheaderdata) - 2;
    hout = "";
    while(hc<hcmax):
     hout = hout + AppendNullByte(preheaderdata[hc], formatspecs[5]);
     hc = hc + 1;
-   if(prefchecksumtype=="none" or prefchecksumtype==""):
-    prenewfcs = 0;
-   elif(prefchecksumtype=="crc16" or prefchecksumtype=="crc16_ansi" or prefchecksumtype=="crc16_ibm"):
-    prenewfcs = format(crc16(hout.encode('UTF-8')) & 0xffff, '04x').lower();
-   elif(prefchecksumtype=="adler32"):
-    prenewfcs = format(zlib.adler32(hout.encode('UTF-8')) & 0xffffffff, '08x').lower();
-   elif(prefchecksumtype=="crc32"):
-    prenewfcs = format(crc32(hout.encode('UTF-8')) & 0xffffffff, '08x').lower();
-   elif(prefchecksumtype=="crc64_ecma"):
-    prenewfcs = format(crc64_ecma(hout.encode('UTF-8')) & 0xffffffffffffffff, '016x').lower();
-   elif(prefchecksumtype=="crc64" or prefchecksumtype=="crc64_iso"):
-    prenewfcs = format(crc64_iso(hout.encode('UTF-8')) & 0xffffffffffffffff, '016x').lower();
-   elif(CheckSumSupportAlt(prefchecksumtype, hashlib_guaranteed)):
-    checksumoutstr = hashlib.new(prefchecksumtype);
-    checksumoutstr.update(hout.encode('UTF-8'));
-    prenewfcs = checksumoutstr.hexdigest().lower();
+   prenewfcs = GetFileChecksum(hout, preheaderdata[-3].lower(), True, formatspecs);
    if(prefcs!=prenewfcs and not skipchecksum):
     VerbosePrintOut("File Header Checksum Error with file " + prefname + " at offset " + str(prefhstart));
     return False;
     valid_archive = False;
     invalid_archive = True;
    prefhend = catfp.tell() - 1;
    prefcontentstart = catfp.tell();
    prefcontents = "";
    pyhascontents = False;
    if(prefsize>0):
     prefcontents = catfp.read(prefsize);
-    if(prefchecksumtype=="none" or prefchecksumtype==""):
-     prenewfccs = 0;
-    elif(prefchecksumtype=="crc16" or prefchecksumtype=="crc16_ansi" or prefchecksumtype=="crc16_ibm"):
-     prenewfccs = format(crc16(prefcontents) & 0xffff, '04x').lower();
-    elif(prefchecksumtype=="crc16_ccitt"):
-     prenewfcs = format(crc16_ccitt(prefcontents) & 0xffff, '04x').lower();
-    elif(prefchecksumtype=="adler32"):
-     prenewfccs = format(zlib.adler32(prefcontents) & 0xffffffff, '08x').lower();
-    elif(prefchecksumtype=="crc32"):
-     prenewfccs = format(crc32(prefcontents) & 0xffffffff, '08x').lower();
-    elif(prefchecksumtype=="crc64_ecma"):
-     prenewfcs = format(crc64_ecma(prefcontents) & 0xffffffffffffffff, '016x').lower();
-    elif(prefchecksumtype=="crc64" or prefchecksumtype=="crc64_iso"):
-     prenewfcs = format(crc64_iso(prefcontents) & 0xffffffffffffffff, '016x').lower();
-    elif(CheckSumSupportAlt(prefchecksumtype, hashlib_guaranteed)):
-     checksumoutstr = hashlib.new(prefchecksumtype);
-     checksumoutstr.update(prefcontents);
-     prenewfccs = checksumoutstr.hexdigest().lower();
+    prenewfccs = GetFileChecksum(prefcontents, preheaderdata[-3].lower(), False, formatspecs);
     pyhascontents = True;
     if(prefccs!=prenewfccs and not skipchecksum):
      VerbosePrintOut("File Content Checksum Error with file " + prefname + " at offset " + str(prefcontentstart));
      return False;
    catfp.seek(1, 1);
    il = il + 1;
  catfp.seek(seekstart, 0);
@@ -3976,59 +3944,27 @@
    prefccs = preheaderdata[extrastart + 2].lower();
    hc = 0;
    hcmax = len(preheaderdata) - 2;
    hout = "";
    while(hc<hcmax):
     hout = hout + AppendNullByte(preheaderdata[hc], formatspecs[5]);
     hc = hc + 1;
-   if(prefchecksumtype=="none" or prefchecksumtype==""):
-    prenewfcs = 0;
-   elif(prefchecksumtype=="crc16" or prefchecksumtype=="crc16_ansi" or prefchecksumtype=="crc16_ibm"):
-    prenewfcs = format(crc16(hout.encode('UTF-8')) & 0xffff, '04x').lower();
-   elif(prefchecksumtype=="adler32"):
-    prenewfcs = format(zlib.adler32(hout.encode('UTF-8')) & 0xffffffff, '08x').lower();
-   elif(prefchecksumtype=="crc32"):
-    prenewfcs = format(crc32(hout.encode('UTF-8')) & 0xffffffff, '08x').lower();
-   elif(prefchecksumtype=="crc64_ecma"):
-    prenewfcs = format(crc64_ecma(hout.encode('UTF-8')) & 0xffffffffffffffff, '016x').lower();
-   elif(prefchecksumtype=="crc64" or prefchecksumtype=="crc64_iso"):
-    prenewfcs = format(crc64_iso(hout.encode('UTF-8')) & 0xffffffffffffffff, '016x').lower();
-   elif(CheckSumSupportAlt(prefchecksumtype, hashlib_guaranteed)):
-    checksumoutstr = hashlib.new(prefchecksumtype);
-    checksumoutstr.update(hout.encode('UTF-8'));
-    prenewfcs = checksumoutstr.hexdigest().lower();
+   prenewfcs = GetFileChecksum(hout, preheaderdata[-3].lower(), True, formatspecs);
    if(prefcs!=prenewfcs and not skipchecksum):
     VerbosePrintOut("File Header Checksum Error with file " + prefname + " at offset " + str(prefhstart));
     return False;
     valid_archive = False;
     invalid_archive = True;
    prefhend = catfp.tell() - 1;
    prefcontentstart = catfp.tell();
    prefcontents = "";
    pyhascontents = False;
    if(prefsize>0):
     prefcontents = catfp.read(prefsize);
-    if(prefchecksumtype=="none" or prefchecksumtype==""):
-     prenewfccs = 0;
-    elif(prefchecksumtype=="crc16" or prefchecksumtype=="crc16_ansi" or prefchecksumtype=="crc16_ibm"):
-     prenewfccs = format(crc16(prefcontents) & 0xffff, '04x').lower();
-    elif(prefchecksumtype=="crc16_ccitt"):
-     prenewfcs = format(crc16_ccitt(prefcontents) & 0xffff, '04x').lower();
-    elif(prefchecksumtype=="adler32"):
-     prenewfccs = format(zlib.adler32(prefcontents) & 0xffffffff, '08x').lower();
-    elif(prefchecksumtype=="crc32"):
-     prenewfccs = format(crc32(prefcontents) & 0xffffffff, '08x').lower();
-    elif(prefchecksumtype=="crc64_ecma"):
-     prenewfcs = format(crc64_ecma(prefcontents) & 0xffffffffffffffff, '016x').lower();
-    elif(prefchecksumtype=="crc64" or prefchecksumtype=="crc64_iso"):
-     prenewfcs = format(crc64_iso(prefcontents) & 0xffffffffffffffff, '016x').lower();
-    elif(CheckSumSupportAlt(prefchecksumtype, hashlib_guaranteed)):
-     checksumoutstr = hashlib.new(prefchecksumtype);
-     checksumoutstr.update(prefcontents);
-     prenewfccs = checksumoutstr.hexdigest().lower();
+    prenewfccs = GetFileChecksum(prefcontents, preheaderdata[-3].lower(), False, formatspecs);
     pyhascontents = True;
     if(prefccs!=prenewfccs and not skipchecksum):
      VerbosePrintOut("File Content Checksum Error with file " + prefname + " at offset " + str(prefcontentstart));
      return False;
    catfp.seek(1, 1);
    il = il + 1;
    filefound = False;
@@ -4251,30 +4187,15 @@
   catfccs = catheaderdata[extrastart + 2].lower();
   hc = 0;
   hcmax = len(catheaderdata) - 2;
   hout = "";
   while(hc<hcmax):
    hout = hout + AppendNullByte(catheaderdata[hc], formatspecs[5]);
    hc = hc + 1;
-  if(catfchecksumtype=="none" or catfchecksumtype==""):
-   catnewfcs = 0;
-  elif(catfchecksumtype=="crc16" or catfchecksumtype=="crc16_ansi" or catfchecksumtype=="crc16_ibm"):
-   catnewfcs = format(crc16(hout.encode('UTF-8')) & 0xffff, '04x').lower();
-  elif(catfchecksumtype=="adler32"):
-   catnewfcs = format(zlib.adler32(hout.encode('UTF-8')) & 0xffffffff, '08x').lower();
-  elif(catfchecksumtype=="crc32"):
-   catnewfcs = format(crc32(hout.encode('UTF-8')) & 0xffffffff, '08x').lower();
-  elif(catfchecksumtype=="crc64_ecma"):
-   catnewfcs = format(crc64_ecma(hout.encode('UTF-8')) & 0xffffffffffffffff, '016x').lower();
-  elif(catfchecksumtype=="crc64" or catfchecksumtype=="crc64_iso"):
-   catnewfcs = format(crc64_iso(hout.encode('UTF-8')) & 0xffffffffffffffff, '016x').lower();
-  elif(CheckSumSupportAlt(catfchecksumtype, hashlib_guaranteed)):
-   checksumoutstr = hashlib.new(catfchecksumtype);
-   checksumoutstr.update(hout.encode('UTF-8'));
-   catnewfcs = checksumoutstr.hexdigest().lower();
+  catnewfcs = GetFileChecksum(hout, catheaderdata[-3].lower(), True, formatspecs);
   if(verbose):
    VerbosePrintOut(catfname);
    VerbosePrintOut("Record Number " + str(il) + "; File ID " + str(fid) + "; iNode Number " + str(finode));
   if(catfcs==catnewfcs):
    if(verbose):
     VerbosePrintOut("File Header Checksum Passed at offset " + str(catfhstart));
   else:
@@ -4284,32 +4205,15 @@
    invalid_archive = True;
   catfhend = catfp.tell() - 1;
   catfcontentstart = catfp.tell();
   catfcontents = "";
   pyhascontents = False;
   if(catfsize>0):
    catfcontents = catfp.read(catfsize);
-   if(catfchecksumtype=="none" or catfchecksumtype==""):
-    catnewfccs = 0;
-   elif(catfchecksumtype=="crc16" or catfchecksumtype=="crc16_ansi" or catfchecksumtype=="crc16_ibm"):
-    catnewfccs = format(crc16(catfcontents) & 0xffff, '04x').lower();
-   elif(catfchecksumtype=="crc16_ccitt"):
-    catnewfcs = format(crc16_ccitt(catfcontents) & 0xffff, '04x').lower();
-   elif(catfchecksumtype=="adler32"):
-    catnewfccs = format(zlib.adler32(catfcontents) & 0xffffffff, '08x').lower();
-   elif(catfchecksumtype=="crc32"):
-    catnewfccs = format(crc32(catfcontents) & 0xffffffff, '08x').lower();
-   elif(catfchecksumtype=="crc64_ecma"):
-    catnewfcs = format(crc64_ecma(catfcontents) & 0xffffffffffffffff, '016x').lower();
-   elif(catfchecksumtype=="crc64" or catfchecksumtype=="crc64_iso"):
-    catnewfcs = format(crc64_iso(catfcontents) & 0xffffffffffffffff, '016x').lower();
-   elif(CheckSumSupportAlt(catfchecksumtype, hashlib_guaranteed)):
-    checksumoutstr = hashlib.new(catfchecksumtype);
-    checksumoutstr.update(catfcontents);
-    catnewfccs = checksumoutstr.hexdigest().lower();
+   catnewfccs = GetFileChecksum(catfcontents, catheaderdata[-3].lower(), False, formatspecs);
    pyhascontents = True;
    if(catfccs==catnewfccs):
     if(verbose):
      VerbosePrintOut("File Content Checksum Passed at offset " + str(catfcontentstart));
    else:
     if(verbose):
      VerbosePrintOut("File Content Checksum Failed at offset " + str(catfcontentstart));
@@ -4492,59 +4396,27 @@
    prefccs = preheaderdata[extrastart + 2].lower();
    hc = 0;
    hcmax = len(preheaderdata) - 2;
    hout = "";
    while(hc<hcmax):
     hout = hout + AppendNullByte(preheaderdata[hc], formatspecs[5]);
     hc = hc + 1;
-   if(prefchecksumtype=="none" or prefchecksumtype==""):
-    prenewfcs = 0;
-   elif(prefchecksumtype=="crc16" or prefchecksumtype=="crc16_ansi" or prefchecksumtype=="crc16_ibm"):
-    prenewfcs = format(crc16(hout.encode('UTF-8')) & 0xffff, '04x').lower();
-   elif(prefchecksumtype=="adler32"):
-    prenewfcs = format(zlib.adler32(hout.encode('UTF-8')) & 0xffffffff, '08x').lower();
-   elif(prefchecksumtype=="crc32"):
-    prenewfcs = format(crc32(hout.encode('UTF-8')) & 0xffffffff, '08x').lower();
-   elif(prefchecksumtype=="crc64_ecma"):
-    prenewfcs = format(crc64_ecma(hout.encode('UTF-8')) & 0xffffffffffffffff, '016x').lower();
-   elif(prefchecksumtype=="crc64" or prefchecksumtype=="crc64_iso"):
-    prenewfcs = format(crc64_iso(hout.encode('UTF-8')) & 0xffffffffffffffff, '016x').lower();
-   elif(CheckSumSupportAlt(prefchecksumtype, hashlib_guaranteed)):
-    checksumoutstr = hashlib.new(prefchecksumtype);
-    checksumoutstr.update(hout.encode('UTF-8'));
-    prenewfcs = checksumoutstr.hexdigest().lower();
+   prenewfcs = GetFileChecksum(hout, preheaderdata[-3].lower(), True, formatspecs);
    if(prefcs!=prenewfcs and not skipchecksum):
     VerbosePrintOut("File Header Checksum Error with file " + prefname + " at offset " + str(prefhstart));
     return False;
     valid_archive = False;
     invalid_archive = True;
    prefhend = catfp.tell() - 1;
    prefcontentstart = catfp.tell();
    prefcontents = "";
    pyhascontents = False;
    if(prefsize>0):
     prefcontents = catfp.read(prefsize);
-    if(prefchecksumtype=="none" or prefchecksumtype==""):
-     prenewfccs = 0;
-    elif(prefchecksumtype=="crc16" or prefchecksumtype=="crc16_ansi" or prefchecksumtype=="crc16_ibm"):
-     prenewfccs = format(crc16(prefcontents) & 0xffff, '04x').lower();
-    elif(prefchecksumtype=="crc16_ccitt"):
-     prenewfcs = format(crc16_ccitt(prefcontents) & 0xffff, '04x').lower();
-    elif(prefchecksumtype=="adler32"):
-     prenewfccs = format(zlib.adler32(prefcontents) & 0xffffffff, '08x').lower();
-    elif(prefchecksumtype=="crc32"):
-     prenewfccs = format(crc32(prefcontents) & 0xffffffff, '08x').lower();
-    elif(prefchecksumtype=="crc64_ecma"):
-     prenewfcs = format(crc64_ecma(prefcontents) & 0xffffffffffffffff, '016x').lower();
-    elif(prefchecksumtype=="crc64" or prefchecksumtype=="crc64_iso"):
-     prenewfcs = format(crc64_iso(prefcontents) & 0xffffffffffffffff, '016x').lower();
-    elif(CheckSumSupportAlt(prefchecksumtype, hashlib_guaranteed)):
-     checksumoutstr = hashlib.new(prefchecksumtype);
-     checksumoutstr.update(prefcontents);
-     prenewfccs = checksumoutstr.hexdigest().lower();
+    prenewfccs = GetFileChecksum(prefcontents, preheaderdata[-3].lower(), False, formatspecs);
     pyhascontents = True;
     if(prefccs!=prenewfccs and not skipchecksum):
      VerbosePrintOut("File Content Checksum Error with file " + prefname + " at offset " + str(prefcontentstart));
      return False;
    catfp.seek(1, 1);
    il = il + 1;
  fileidnum = seekstart;
@@ -4600,57 +4472,25 @@
   catfccs = catheaderdata[extrastart + 2].lower();
   hc = 0;
   hcmax = len(catheaderdata) - 2;
   hout = "";
   while(hc<hcmax):
    hout = hout + AppendNullByte(catheaderdata[hc], formatspecs[5]);
    hc = hc + 1;
-  if(catfchecksumtype=="none" or catfchecksumtype==""):
-   catnewfcs = 0;
-  elif(catfchecksumtype=="crc16" or catfchecksumtype=="crc16_ansi" or catfchecksumtype=="crc16_ibm"):
-   catnewfcs = format(crc16(hout.encode('UTF-8')) & 0xffff, '04x').lower();
-  elif(catfchecksumtype=="adler32"):
-   catnewfcs = format(zlib.adler32(hout.encode('UTF-8')) & 0xffffffff, '08x').lower();
-  elif(catfchecksumtype=="crc32"):
-   catnewfcs = format(crc32(hout.encode('UTF-8')) & 0xffffffff, '08x').lower();
-  elif(catfchecksumtype=="crc64_ecma"):
-   catnewfcs = format(crc64_ecma(hout.encode('UTF-8')) & 0xffffffffffffffff, '016x').lower();
-  elif(catfchecksumtype=="crc64" or catfchecksumtype=="crc64_iso"):
-   catnewfcs = format(crc64_iso(hout.encode('UTF-8')) & 0xffffffffffffffff, '016x').lower();
-  elif(CheckSumSupportAlt(catfchecksumtype, hashlib_guaranteed)):
-   checksumoutstr = hashlib.new(catfchecksumtype);
-   checksumoutstr.update(hout.encode('UTF-8'));
-   catnewfcs = checksumoutstr.hexdigest().lower();
+  catnewfcs = GetFileChecksum(hout, catheaderdata[-3].lower(), True, formatspecs);
   if(catfcs!=catnewfcs and not skipchecksum):
    VerbosePrintOut("File Header Checksum Error with file " + catfname + " at offset " + str(catfhstart));
    return False;
   catfhend = catfp.tell() - 1;
   catfcontentstart = catfp.tell();
   catfcontents = "";
   pyhascontents = False;
   if(catfsize>0 and not listonly):
    catfcontents = catfp.read(catfsize);
-   if(catfchecksumtype=="none" or catfchecksumtype==""):
-    catnewfccs = 0;
-   elif(catfchecksumtype=="crc16" or catfchecksumtype=="crc16_ansi" or catfchecksumtype=="crc16_ibm"):
-    catnewfccs = format(crc16(catfcontents) & 0xffff, '04x').lower();
-   elif(catfchecksumtype=="crc16_ccitt"):
-    catnewfcs = format(crc16_ccitt(catfcontents) & 0xffff, '04x').lower();
-   elif(catfchecksumtype=="adler32"):
-    catnewfccs = format(zlib.adler32(catfcontents) & 0xffffffff, '08x').lower();
-   elif(catfchecksumtype=="crc32"):
-    catnewfccs = format(crc32(catfcontents) & 0xffffffff, '08x').lower();
-   elif(catfchecksumtype=="crc64_ecma"):
-    catnewfcs = format(crc64_ecma(catfcontents) & 0xffffffffffffffff, '016x').lower();
-   elif(catfchecksumtype=="crc64" or catfchecksumtype=="crc64_iso"):
-    catnewfcs = format(crc64_iso(catfcontents) & 0xffffffffffffffff, '016x').lower();
-   elif(CheckSumSupportAlt(catfchecksumtype, hashlib_guaranteed)):
-    checksumoutstr = hashlib.new(catfchecksumtype);
-    checksumoutstr.update(catfcontents);
-    catnewfccs = checksumoutstr.hexdigest().lower();
+   catnewfccs = GetFileChecksum(catfcontents, catheaderdata[-3].lower(), False, formatspecs);
    pyhascontents = True;
    if(catfccs!=catnewfccs and skipchecksum):
     VerbosePrintOut("File Content Checksum Error with file " + catfname + " at offset " + str(catfcontentstart));
     return False;
   if(catfsize>0 and listonly):
    catfp.seek(catfsize, 1);
    pyhascontents = False;
@@ -5109,15 +4949,15 @@
    ftype = 12;
   else:
    ffullmode = member.mode;
    ftype = 0;
   flinkname = "";
   fbasedir = os.path.dirname(fname);
   fcurfid = curfid;
-  fcurinode = 0;
+  fcurinode = curfid;
   finode = fcurinode;
   curfid = curfid + 1;
   if(ftype==2):
    flinkname = member.linkname;
   fdev_minor = member.devminor;
   fdev_major = member.devmajor;
   frdev_minor = member.devminor;
@@ -5328,15 +5168,15 @@
   if(not member.is_dir()):
    ftype = 0;
   elif(member.is_dir()):
    ftype = 5;
   flinkname = "";
   fbasedir = os.path.dirname(fname);
   fcurfid = curfid;
-  fcurinode = 0;
+  fcurinode = curfid;
   finode = fcurinode;
   curfid = curfid + 1;
   fdev_minor = 0;
   fdev_major = 0;
   frdev_minor = 0;
   frdev_major = 0;
   if(ftype==5):
@@ -5603,15 +5443,15 @@
    elif(member.is_dir()):
     ftype = 5;
    flinkname = "";
    if(ftype==2):
     flinkname = rarfp.read(member.filename).decode("UTF-8");
    fbasedir = os.path.dirname(fname);
    fcurfid = curfid;
-   fcurinode = 0;
+   fcurinode = curfid;
    finode = fcurinode;
    curfid = curfid + 1;
    fdev_minor = 0;
    fdev_major = 0;
    frdev_minor = 0;
    frdev_major = 0;
    if(ftype==5):
@@ -6832,14 +6672,16 @@
  try:
   if(hasattr(infile, "read") or hasattr(infile, "write")):
    tarfp = tarfile.open(fileobj=infile, mode="r");
   else:
    tarfp = tarfile.open(infile, "r");
  except FileNotFoundError:
   return False;
+ lcfi = 0
+ returnval = {};
  for member in sorted(tarfp.getmembers(), key=lambda x: x.name):
   returnval.update({lcfi: member.name});
   fpremode = member.mode;
   ffullmode = member.mode;
   flinkcount = 0;
   ftype = 0;
   if(member.isreg()):
```

### Comparing `PyCatFile-0.7.6/setup.py` & `PyCatFile-0.7.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2016-2024 Cool Dude 2k - http://idb.berlios.de/
     Copyright 2016-2024 Game Maker 2k - http://intdb.sourceforge.net/
     Copyright 2016-2024 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: setup.py - Last Update: 4/10/2024 Ver. 0.7.6 RC 1 - Author: cooldude2k $
+    $FileInfo: setup.py - Last Update: 4/12/2024 Ver. 0.7.8 RC 1 - Author: cooldude2k $
 '''
 
 import os, re, sys, pkg_resources;
 from setuptools import setup;
 
 verinfofilename = os.path.realpath("."+os.path.sep+os.path.sep+"pycatfile.py");
 verinfofile = open(verinfofilename, "r");
```

