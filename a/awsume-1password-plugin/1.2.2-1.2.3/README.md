# Comparing `tmp/awsume_1password_plugin-1.2.2-py3-none-any.whl.zip` & `tmp/awsume_1password_plugin-1.2.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3976 bytes, number of entries: 7
--rw-r--r--  2.0 unx     4335 b- defN 23-Sep-27 16:15 1password.py
--rw-r--r--  2.0 unx     1069 b- defN 23-Sep-27 16:16 awsume_1password_plugin-1.2.2.dist-info/LICENSE
--rw-r--r--  2.0 unx      263 b- defN 23-Sep-27 16:16 awsume_1password_plugin-1.2.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Sep-27 16:16 awsume_1password_plugin-1.2.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       31 b- defN 23-Sep-27 16:16 awsume_1password_plugin-1.2.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       10 b- defN 23-Sep-27 16:16 awsume_1password_plugin-1.2.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      645 b- defN 23-Sep-27 16:16 awsume_1password_plugin-1.2.2.dist-info/RECORD
-7 files, 6445 bytes uncompressed, 2808 bytes compressed:  56.4%
+Zip file size: 4074 bytes, number of entries: 7
+-rw-r--r--  2.0 unx     4901 b- defN 24-Apr-13 00:38 1password.py
+-rw-r--r--  2.0 unx     1069 b- defN 24-Apr-13 00:39 awsume_1password_plugin-1.2.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx      263 b- defN 24-Apr-13 00:39 awsume_1password_plugin-1.2.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-13 00:39 awsume_1password_plugin-1.2.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       31 b- defN 24-Apr-13 00:39 awsume_1password_plugin-1.2.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       10 b- defN 24-Apr-13 00:39 awsume_1password_plugin-1.2.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      645 b- defN 24-Apr-13 00:39 awsume_1password_plugin-1.2.3.dist-info/RECORD
+7 files, 7011 bytes uncompressed, 2906 bytes compressed:  58.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: 1password.py
 Comment: 
 
-Filename: awsume_1password_plugin-1.2.2.dist-info/LICENSE
+Filename: awsume_1password_plugin-1.2.3.dist-info/LICENSE
 Comment: 
 
-Filename: awsume_1password_plugin-1.2.2.dist-info/METADATA
+Filename: awsume_1password_plugin-1.2.3.dist-info/METADATA
 Comment: 
 
-Filename: awsume_1password_plugin-1.2.2.dist-info/WHEEL
+Filename: awsume_1password_plugin-1.2.3.dist-info/WHEEL
 Comment: 
 
-Filename: awsume_1password_plugin-1.2.2.dist-info/entry_points.txt
+Filename: awsume_1password_plugin-1.2.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: awsume_1password_plugin-1.2.2.dist-info/top_level.txt
+Filename: awsume_1password_plugin-1.2.3.dist-info/top_level.txt
 Comment: 
 
-Filename: awsume_1password_plugin-1.2.2.dist-info/RECORD
+Filename: awsume_1password_plugin-1.2.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## 1password.py

```diff
@@ -1,20 +1,18 @@
 import argparse
-import colorama
-import traceback
 import sys
+import traceback
+from subprocess import PIPE, Popen
 
-from subprocess import Popen, PIPE
-
+import colorama
 from awsume.awsumepy import hookimpl, safe_print
-from awsume.awsumepy.lib import profile as profile_lib
 from awsume.awsumepy.lib import cache as cache_lib
+from awsume.awsumepy.lib import profile as profile_lib
 from awsume.awsumepy.lib.logger import logger
 
-
 # Truncate proxied subprocess output to avoid stack trace spam
 MAX_OUTPUT_LINES = 2
 
 
 # Map an MFA serial to a 1Password vault item
 def find_item(config, mfa_serial):
     config = config.get('1password')
@@ -31,16 +29,15 @@
     if not item:
         logger.debug('No vault item specified for this mfa_serial')
     return item
 
 
 # Find the MFA serial for a given AWS profile.
 def get_mfa_serial(profiles, target_name):
-    mfa_serial = profile_lib.get_mfa_serial(
-        profiles, target_name)
+    mfa_serial = profile_lib.get_mfa_serial(profiles, target_name)
     if not mfa_serial:
         logger.debug('No MFA required')
     return mfa_serial
 
 
 # Make a 1Password error message more succinct before safe_printing it.
 # Return None if it's not worth printing (e.g. an expected error).
@@ -52,64 +49,87 @@
     else:
         return msg
 
 
 # Call 1Password to get an OTP for a given vault item.
 def get_otp(title):
     try:
-        op = Popen(['op', 'item', 'get', '--otp', title],
-                   stdout=PIPE, stderr=PIPE)
+        op = Popen(['op', 'item', 'get', '--otp', title], stdout=PIPE, stderr=PIPE)
         linecount = 0
         while True:
             msg = op.stderr.readline().decode()
             if msg == '' and op.poll() is not None:
                 break
             elif msg != '' and linecount < MAX_OUTPUT_LINES:
                 msg = beautify(msg)
                 if msg:
-                    safe_print('1Password: ' + msg,
-                               colorama.Fore.CYAN)
+                    safe_print('1Password: ' + msg, colorama.Fore.CYAN)
                     linecount += 1
             else:
                 logger.debug(msg.strip('\n'))
         if op.returncode != 0:
             return None
         return op.stdout.readline().decode().strip('\n')
     except FileNotFoundError:
         logger.error('Failed: missing `op` command')
         return None
 
 
 # Print sad message to console with instructions for filing a bug report.
 # Log stack trace to stderr in lieu of safe_print.
 def handle_crash():
-    safe_print('Error invoking 1Password plugin; please file a bug report:\n  %s' %
-               ('https://github.com/xeger/awsume-1password-plugin/issues/new/choose'), colorama.Fore.RED)
+    safe_print(
+        'Error invoking 1Password plugin; please file a bug report:\n  %s'
+        % ('https://github.com/xeger/awsume-1password-plugin/issues/new/choose'),
+        colorama.Fore.RED,
+    )
     traceback.print_exc(file=sys.stderr)
 
 
 @hookimpl
 def pre_get_credentials(config: dict, arguments: argparse.Namespace, profiles: dict):
     try:
-        target_profile_name = profile_lib.get_profile_name(config, profiles, arguments.target_profile_name)
+        target_profile_name = profile_lib.get_profile_name(
+            config, profiles, arguments.target_profile_name
+        )
         if not profiles.get(target_profile_name):
             logger.debug('No profile %s found, skip plugin flow' % target_profile_name)
             return None
         if target_profile_name != None:
-            role_chain = profile_lib.get_role_chain(config, arguments, profiles, target_profile_name)
-            first_profile_name = role_chain[0]
+            if target_profile_name == "default":
+                first_profile_name = "default"
+            else:
+                role_chain = profile_lib.get_role_chain(
+                    config, arguments, profiles, target_profile_name
+                )
+                first_profile_name = role_chain[0]
             first_profile = profiles.get(first_profile_name)
             source_credentials = profile_lib.profile_to_credentials(first_profile)
-            cache_file_name = 'aws-credentials-' + source_credentials.get('AccessKeyId')
+            source_access_key_id = source_credentials.get('AccessKeyId')
+            if source_access_key_id == None:
+                logger.debug(
+                    'No access key for profile %, skip plugin flow'
+                    % target_profile_name
+                )
+                return None
+            cache_file_name = 'aws-credentials-' + source_access_key_id
             cache_session = cache_lib.read_aws_cache(cache_file_name)
-            valid_cache_session = cache_session and cache_lib.valid_cache_session(cache_session)
+            valid_cache_session = cache_session and cache_lib.valid_cache_session(
+                cache_session
+            )
 
             mfa_serial = profile_lib.get_mfa_serial(profiles, first_profile_name)
-            if mfa_serial and (not valid_cache_session or arguments.force_refresh) and not arguments.mfa_token:
+            if (
+                mfa_serial
+                and (not valid_cache_session or arguments.force_refresh)
+                and not arguments.mfa_token
+            ):
                 item = find_item(config, mfa_serial)
                 if item:
                     arguments.mfa_token = get_otp(item)
                     if arguments.mfa_token:
-                        safe_print('Obtained MFA token from 1Password item: %s' %
-                                   (item), colorama.Fore.CYAN)
+                        safe_print(
+                            'Obtained MFA token from 1Password item: %s' % (item),
+                            colorama.Fore.CYAN,
+                        )
     except Exception:
         handle_crash()
```

## Comparing `awsume_1password_plugin-1.2.2.dist-info/LICENSE` & `awsume_1password_plugin-1.2.3.dist-info/LICENSE`

 * *Files identical despite different names*

