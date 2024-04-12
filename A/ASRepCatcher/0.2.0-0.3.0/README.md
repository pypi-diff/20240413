# Comparing `tmp/ASRepCatcher-0.2.0.tar.gz` & `tmp/ASRepCatcher-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ASRepCatcher-0.2.0.tar", last modified: Thu Mar 28 21:04:17 2024, max compression
+gzip compressed data, was "ASRepCatcher-0.3.0.tar", last modified: Fri Apr 12 22:32:13 2024, max compression
```

## Comparing `ASRepCatcher-0.2.0.tar` & `ASRepCatcher-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 youkessou  (1000) youkessou  (1000)        0 2024-03-28 21:04:17.431969 ASRepCatcher-0.2.0/
-drwxr-xr-x   0 youkessou  (1000) youkessou  (1000)        0 2024-03-28 21:04:17.431969 ASRepCatcher-0.2.0/ASRepCatcher/
--rw-r--r--   0 youkessou  (1000) youkessou  (1000)    25910 2024-03-28 20:51:54.000000 ASRepCatcher-0.2.0/ASRepCatcher/ASRepCatcher.py
--rw-r--r--   0 youkessou  (1000) youkessou  (1000)        0 2024-03-28 00:47:42.000000 ASRepCatcher-0.2.0/ASRepCatcher/__init__.py
-drwxr-xr-x   0 youkessou  (1000) youkessou  (1000)        0 2024-03-28 21:04:17.431969 ASRepCatcher-0.2.0/ASRepCatcher.egg-info/
--rw-r--r--   0 youkessou  (1000) youkessou  (1000)      351 2024-03-28 21:04:17.000000 ASRepCatcher-0.2.0/ASRepCatcher.egg-info/PKG-INFO
--rw-r--r--   0 youkessou  (1000) youkessou  (1000)      298 2024-03-28 21:04:17.000000 ASRepCatcher-0.2.0/ASRepCatcher.egg-info/SOURCES.txt
--rw-r--r--   0 youkessou  (1000) youkessou  (1000)        1 2024-03-28 21:04:17.000000 ASRepCatcher-0.2.0/ASRepCatcher.egg-info/dependency_links.txt
--rw-r--r--   0 youkessou  (1000) youkessou  (1000)       64 2024-03-28 21:04:17.000000 ASRepCatcher-0.2.0/ASRepCatcher.egg-info/entry_points.txt
--rw-r--r--   0 youkessou  (1000) youkessou  (1000)       31 2024-03-28 21:04:17.000000 ASRepCatcher-0.2.0/ASRepCatcher.egg-info/requires.txt
--rw-r--r--   0 youkessou  (1000) youkessou  (1000)       13 2024-03-28 21:04:17.000000 ASRepCatcher-0.2.0/ASRepCatcher.egg-info/top_level.txt
--rw-r--r--   0 youkessou  (1000) youkessou  (1000)    35149 2024-03-26 23:13:36.000000 ASRepCatcher-0.2.0/LICENSE
--rw-r--r--   0 youkessou  (1000) youkessou  (1000)      351 2024-03-28 21:04:17.431969 ASRepCatcher-0.2.0/PKG-INFO
--rw-r--r--   0 youkessou  (1000) youkessou  (1000)     4880 2024-03-28 20:59:43.000000 ASRepCatcher-0.2.0/README.md
--rw-r--r--   0 youkessou  (1000) youkessou  (1000)       38 2024-03-28 21:04:17.431969 ASRepCatcher-0.2.0/setup.cfg
--rw-r--r--   0 youkessou  (1000) youkessou  (1000)      520 2024-03-28 21:04:07.000000 ASRepCatcher-0.2.0/setup.py
+drwxr-xr-x   0 youkessou  (1000) youkessou  (1000)        0 2024-04-12 22:32:13.419994 ASRepCatcher-0.3.0/
+drwxr-xr-x   0 youkessou  (1000) youkessou  (1000)        0 2024-04-12 22:32:13.419994 ASRepCatcher-0.3.0/ASRepCatcher/
+-rw-r--r--   0 youkessou  (1000) youkessou  (1000)    26022 2024-04-12 22:28:48.000000 ASRepCatcher-0.3.0/ASRepCatcher/ASRepCatcher.py
+-rw-r--r--   0 youkessou  (1000) youkessou  (1000)        0 2024-03-28 00:47:42.000000 ASRepCatcher-0.3.0/ASRepCatcher/__init__.py
+drwxr-xr-x   0 youkessou  (1000) youkessou  (1000)        0 2024-04-12 22:32:13.419994 ASRepCatcher-0.3.0/ASRepCatcher.egg-info/
+-rw-r--r--   0 youkessou  (1000) youkessou  (1000)      374 2024-04-12 22:32:13.000000 ASRepCatcher-0.3.0/ASRepCatcher.egg-info/PKG-INFO
+-rw-r--r--   0 youkessou  (1000) youkessou  (1000)      298 2024-04-12 22:32:13.000000 ASRepCatcher-0.3.0/ASRepCatcher.egg-info/SOURCES.txt
+-rw-r--r--   0 youkessou  (1000) youkessou  (1000)        1 2024-04-12 22:32:13.000000 ASRepCatcher-0.3.0/ASRepCatcher.egg-info/dependency_links.txt
+-rw-r--r--   0 youkessou  (1000) youkessou  (1000)       64 2024-04-12 22:32:13.000000 ASRepCatcher-0.3.0/ASRepCatcher.egg-info/entry_points.txt
+-rw-r--r--   0 youkessou  (1000) youkessou  (1000)       31 2024-04-12 22:32:13.000000 ASRepCatcher-0.3.0/ASRepCatcher.egg-info/requires.txt
+-rw-r--r--   0 youkessou  (1000) youkessou  (1000)       13 2024-04-12 22:32:13.000000 ASRepCatcher-0.3.0/ASRepCatcher.egg-info/top_level.txt
+-rw-r--r--   0 youkessou  (1000) youkessou  (1000)    35149 2024-03-26 23:13:36.000000 ASRepCatcher-0.3.0/LICENSE
+-rw-r--r--   0 youkessou  (1000) youkessou  (1000)      374 2024-04-12 22:32:13.419994 ASRepCatcher-0.3.0/PKG-INFO
+-rw-r--r--   0 youkessou  (1000) youkessou  (1000)     5024 2024-04-12 22:30:42.000000 ASRepCatcher-0.3.0/README.md
+-rw-r--r--   0 youkessou  (1000) youkessou  (1000)       38 2024-04-12 22:32:13.419994 ASRepCatcher-0.3.0/setup.cfg
+-rw-r--r--   0 youkessou  (1000) youkessou  (1000)      551 2024-04-12 22:29:03.000000 ASRepCatcher-0.3.0/setup.py
```

### Comparing `ASRepCatcher-0.2.0/ASRepCatcher/ASRepCatcher.py` & `ASRepCatcher-0.3.0/ASRepCatcher/ASRepCatcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,23 +30,25 @@
     /  \  | (___ | |__) |___ _ __ | |     __ _| |_ ___| |__   ___ _ __ 
    / /\ \  \___ \|  _  // _ \ '_ \| |    / _` | __/ __| '_ \ / _ \ '__|
   / ____ \ ____) | | \ \  __/ |_) | |___| (_| | || (__| | | |  __/ |   
  /_/    \_\_____/|_|  \_\___| .__/ \_____\__,_|\__\___|_| |_|\___|_|   
                             | |                                        
                             |_|                                     
 Author : Yassine OUKESSOU
-Version : 0.2.0
+Version : 0.3.0
                             """)
 
-def is_dc_up(dc, iface):
-    ans = sr1( IP(dst=dc)/TCP(dport=88,flags="S"), iface=iface, verbose=False, timeout=1)
-    if ans is not None and ans[TCP].flags == 'SA' :
+def is_dc_up(dc):
+    sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+    sock.settimeout(1)
+    result = sock.connect_ex((dc,88))
+    sock.close()
+    if result == 0:
         return True
-    else :
-        return False
+    return False
 
 def is_valid_ip_list(iplist):
     if not re.match(r'^(((25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\.){3}(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?),)*((25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\.){3}(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)$', iplist) :
         return False
     return True
 
 def is_valid_ipwithmask(ip_with_mask):
@@ -188,15 +190,15 @@
 netmask = netifaces.ifaddresses(str(iface))[netifaces.AF_INET][0]['netmask']
 subnet = ipaddress.IPv4Network(f'{iface_ip}/{netmask}', strict=False)
 
 if parameters.gw is not None and ipaddress.ip_address(parameters.gw) not in ipaddress.ip_network(subnet) :
     logging.error(f'[!] Gateway not in {iface} subnet. Quitting...')
     sys.exit(1)
 
-if parameters.dc is not None and not is_dc_up(dc, iface):
+if parameters.dc is not None and not is_dc_up(dc):
     logging.error('[!] DC did not respond to TCP/88 ping probe. Quitting...')
     sys.exit(1)
 
 
 if parameters.dc is not None and ipaddress.ip_address(dc) in ipaddress.ip_network(subnet) :
     if parameters.gw is None :
         if mode == 'relay' :
@@ -382,14 +384,15 @@
         if username in UsernamesCaptured :
             UsernamesCaptured[username].append(etype)
         else :
             UsernamesCaptured[username] = [etype]
     print_asrep_hash(username,domain,etype,cipher)
     if mode == 'listen' and stop_spoofing and not disable_spoofing :
         Targets.remove(packet[IP].dst)
+        InitialTargets.remove(packet[IP].dst)
         restore(gw,packet[IP].dst)
         logging.info(f'[+] Restored arp cache of {packet[IP].dst}')
 
 
 
 def has_net_admin_cap():
     return "cap_net_admin" in os.popen("/sbin/capsh --decode=$(cat /proc/self/status | grep CapBnd | awk '{print $2}')").read().strip().split('=')[1].split(',')
@@ -552,14 +555,15 @@
     
     response = await relay_without_modification_to_dc(data)
     krb_response = KerberosTCPHeader(response)
     if krb_response.haslayer(KRB_AS_REP):
         handle_as_rep(krb_response)
         if stop_spoofing and not disable_spoofing :
             if client_ip in Targets : Targets.remove(client_ip)
+            if client_ip in InitialTargets : InitialTargets.remove(client_ip)
             restore(client_ip, gw)
             logging.info(f'[+] Restored arp cache of {client_ip}')
         return response
     return response
```

### Comparing `ASRepCatcher-0.2.0/LICENSE` & `ASRepCatcher-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ASRepCatcher-0.2.0/README.md` & `ASRepCatcher-0.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 
 During an Active Directory black box pentest, if multicast DNS protocols are disabled and/or all protocols (SMB, LDAP, etc.) are signed and no exposed service is vulnerable, you quickly run out of options to get a domain user.
 
 
 ASRepCatcher uses ARP spoofing to catch AS-REP messages returned by the Domain Controller to the clients and prints out the hash to crack.
 
+**This technique does not rely on Kerberos pre-authentication being disabled. It works for all users on the VLAN.**
 
 ## Two modes
 
 
 ### Relay
 
 **This is the preferred way.**<br>
@@ -46,28 +47,28 @@
 ```
 OR
 ```bash
 git clone https://github.com/Yaxxine7/ASRepCatcher
 cd ASRepCatcher
 python3 setup.py install
 ```
-
+Requires at least Python 3.7
 ## Usage
 
 ```
             _____ _____             _____      _       _               
      /\    / ____|  __ \           / ____|    | |     | |              
     /  \  | (___ | |__) |___ _ __ | |     __ _| |_ ___| |__   ___ _ __ 
    / /\ \  \___ \|  _  // _ \ '_ \| |    / _` | __/ __| '_ \ / _ \ '__|
   / ____ \ ____) | | \ \  __/ |_) | |___| (_| | || (__| | | |  __/ |   
  /_/    \_\_____/|_|  \_\___| .__/ \_____\__,_|\__\___|_| |_|\___|_|   
                             | |                                        
                             |_|                                     
 Author : Yassine OUKESSOU
-Version : 0.2.0
+Version : 0.3.0
                             
 usage: ASRepCatcher [-h] [-outfile OUTFILE] [-format {hashcat,john}] [-debug] [-t Client workstations] [-tf targets file] [-gw Gateway IP] [-dc DC IP] [-iface interface]
                     [--stop-spoofing] [--disable-spoofing]
                     {relay,listen}
 
 Catches Kerberos AS-REP packets and outputs it to a crackable format
```

### Comparing `ASRepCatcher-0.2.0/setup.py` & `ASRepCatcher-0.3.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from setuptools import setup
 
 setup(name='ASRepCatcher',
-      version='0.2.0',
+      version='0.3.0',
       description='Make everyone in your VLAN ASREProastable',
       license='GPLv3',
       author='Yassine OUKESSOU',
       author_email='yassine.oukess@gmail.com',
       url='https://github.com/Yaxxine7/ASRepCatcher',
       packages=['ASRepCatcher'],
       install_requires=["scapy", "asn1", "termcolor", "netifaces"],
+      python_requires='>=3.7',
       entry_points = {
           'console_scripts': ['ASRepCatcher=ASRepCatcher.ASRepCatcher:main']
           }
      )
```

