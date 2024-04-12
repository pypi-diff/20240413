# Comparing `tmp/TMC_2209_Raspberry_Pi-0.4.3.tar.gz` & `tmp/tmc_2209_raspberry_pi-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TMC_2209_Raspberry_Pi-0.4.3.tar", last modified: Mon Apr  8 18:32:13 2024, max compression
+gzip compressed data, was "tmc_2209_raspberry_pi-0.4.4.tar", last modified: Fri Apr 12 22:42:02 2024, max compression
```

## Comparing `TMC_2209_Raspberry_Pi-0.4.3.tar` & `tmc_2209_raspberry_pi-0.4.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:32:13.027114 TMC_2209_Raspberry_Pi-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)    35305 2024-04-08 18:32:03.000000 TMC_2209_Raspberry_Pi-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10210 2024-04-08 18:32:13.027114 TMC_2209_Raspberry_Pi-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9331 2024-04-08 18:32:03.000000 TMC_2209_Raspberry_Pi-0.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-08 18:32:03.000000 TMC_2209_Raspberry_Pi-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-08 18:32:13.027114 TMC_2209_Raspberry_Pi-0.4.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:32:13.019114 TMC_2209_Raspberry_Pi-0.4.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:32:13.023114 TMC_2209_Raspberry_Pi-0.4.3/src/TMC_2209/
--rw-r--r--   0 runner    (1001) docker     (127)    19108 2024-04-08 18:32:03.000000 TMC_2209_Raspberry_Pi-0.4.3/src/TMC_2209/TMC_2209_StepperDriver.py
--rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-04-08 18:32:03.000000 TMC_2209_Raspberry_Pi-0.4.3/src/TMC_2209/_TMC_2209_GPIO_board.py
--rw-r--r--   0 runner    (1001) docker     (127)    22221 2024-04-08 18:32:03.000000 TMC_2209_Raspberry_Pi-0.4.3/src/TMC_2209/_TMC_2209_comm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-08 18:32:03.000000 TMC_2209_Raspberry_Pi-0.4.3/src/TMC_2209/_TMC_2209_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-04-08 18:32:03.000000 TMC_2209_Raspberry_Pi-0.4.3/src/TMC_2209/_TMC_2209_math.py
--rw-r--r--   0 runner    (1001) docker     (127)    12473 2024-04-08 18:32:03.000000 TMC_2209_Raspberry_Pi-0.4.3/src/TMC_2209/_TMC_2209_move.py
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-08 18:32:03.000000 TMC_2209_Raspberry_Pi-0.4.3/src/TMC_2209/_TMC_2209_reg.py
--rw-r--r--   0 runner    (1001) docker     (127)     6423 2024-04-08 18:32:03.000000 TMC_2209_Raspberry_Pi-0.4.3/src/TMC_2209/_TMC_2209_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10019 2024-04-08 18:32:03.000000 TMC_2209_Raspberry_Pi-0.4.3/src/TMC_2209/_TMC_2209_uart.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-08 18:32:03.000000 TMC_2209_Raspberry_Pi-0.4.3/src/TMC_2209/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:32:13.027114 TMC_2209_Raspberry_Pi-0.4.3/src/TMC_2209_Raspberry_Pi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10210 2024-04-08 18:32:13.000000 TMC_2209_Raspberry_Pi-0.4.3/src/TMC_2209_Raspberry_Pi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-08 18:32:13.000000 TMC_2209_Raspberry_Pi-0.4.3/src/TMC_2209_Raspberry_Pi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 18:32:13.000000 TMC_2209_Raspberry_Pi-0.4.3/src/TMC_2209_Raspberry_Pi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-08 18:32:13.000000 TMC_2209_Raspberry_Pi-0.4.3/src/TMC_2209_Raspberry_Pi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-08 18:32:13.000000 TMC_2209_Raspberry_Pi-0.4.3/src/TMC_2209_Raspberry_Pi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:32:13.023114 TMC_2209_Raspberry_Pi-0.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-08 18:32:03.000000 TMC_2209_Raspberry_Pi-0.4.3/tests/test_TMC_2209_math.py
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-08 18:32:03.000000 TMC_2209_Raspberry_Pi-0.4.3/tests/test_TMC_2209_move.py
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-08 18:32:03.000000 TMC_2209_Raspberry_Pi-0.4.3/tests/test_TMC_2209_uart.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:42:02.625630 tmc_2209_raspberry_pi-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    35305 2024-04-12 22:41:58.000000 tmc_2209_raspberry_pi-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10210 2024-04-12 22:42:02.625630 tmc_2209_raspberry_pi-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9331 2024-04-12 22:41:58.000000 tmc_2209_raspberry_pi-0.4.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-12 22:41:58.000000 tmc_2209_raspberry_pi-0.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-12 22:42:02.625630 tmc_2209_raspberry_pi-0.4.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:42:02.621630 tmc_2209_raspberry_pi-0.4.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:42:02.625630 tmc_2209_raspberry_pi-0.4.4/src/TMC_2209/
+-rw-r--r--   0 runner    (1001) docker     (127)    19464 2024-04-12 22:41:58.000000 tmc_2209_raspberry_pi-0.4.4/src/TMC_2209/TMC_2209_StepperDriver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-04-12 22:41:58.000000 tmc_2209_raspberry_pi-0.4.4/src/TMC_2209/_TMC_2209_GPIO_board.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23126 2024-04-12 22:41:58.000000 tmc_2209_raspberry_pi-0.4.4/src/TMC_2209/_TMC_2209_comm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5418 2024-04-12 22:41:58.000000 tmc_2209_raspberry_pi-0.4.4/src/TMC_2209/_TMC_2209_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-04-12 22:41:58.000000 tmc_2209_raspberry_pi-0.4.4/src/TMC_2209/_TMC_2209_math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12473 2024-04-12 22:41:58.000000 tmc_2209_raspberry_pi-0.4.4/src/TMC_2209/_TMC_2209_move.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-12 22:41:58.000000 tmc_2209_raspberry_pi-0.4.4/src/TMC_2209/_TMC_2209_reg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6457 2024-04-12 22:41:58.000000 tmc_2209_raspberry_pi-0.4.4/src/TMC_2209/_TMC_2209_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10465 2024-04-12 22:41:58.000000 tmc_2209_raspberry_pi-0.4.4/src/TMC_2209/_TMC_2209_uart.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-12 22:41:58.000000 tmc_2209_raspberry_pi-0.4.4/src/TMC_2209/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:42:02.625630 tmc_2209_raspberry_pi-0.4.4/src/TMC_2209_Raspberry_Pi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10210 2024-04-12 22:42:02.000000 tmc_2209_raspberry_pi-0.4.4/src/TMC_2209_Raspberry_Pi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-12 22:42:02.000000 tmc_2209_raspberry_pi-0.4.4/src/TMC_2209_Raspberry_Pi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 22:42:02.000000 tmc_2209_raspberry_pi-0.4.4/src/TMC_2209_Raspberry_Pi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-12 22:42:02.000000 tmc_2209_raspberry_pi-0.4.4/src/TMC_2209_Raspberry_Pi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 22:42:02.000000 tmc_2209_raspberry_pi-0.4.4/src/TMC_2209_Raspberry_Pi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:42:02.625630 tmc_2209_raspberry_pi-0.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-12 22:41:58.000000 tmc_2209_raspberry_pi-0.4.4/tests/test_TMC_2209_math.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-12 22:41:58.000000 tmc_2209_raspberry_pi-0.4.4/tests/test_TMC_2209_move.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-12 22:41:58.000000 tmc_2209_raspberry_pi-0.4.4/tests/test_TMC_2209_uart.py
```

### Comparing `TMC_2209_Raspberry_Pi-0.4.3/LICENSE` & `tmc_2209_raspberry_pi-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `TMC_2209_Raspberry_Pi-0.4.3/PKG-INFO` & `tmc_2209_raspberry_pi-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TMC_2209_Raspberry_Pi
-Version: 0.4.3
+Version: 0.4.4
 Summary: this is a Python libary to drive a stepper motor with a Trinamic TMC2209 stepper driver and a Raspberry Pi
 Home-page: https://github.com/Chr157i4n/TMC2209_Raspberry_Pi
 Author: Christian Köhlke
 Author-email: christian@koehlke.de
 Project-URL: Bug Tracker, https://github.com/Chr157i4n/TMC2209_Raspberry_Pi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `TMC_2209_Raspberry_Pi-0.4.3/README.md` & `tmc_2209_raspberry_pi-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `TMC_2209_Raspberry_Pi-0.4.3/setup.cfg` & `tmc_2209_raspberry_pi-0.4.4/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = TMC_2209_Raspberry_Pi
-version = 0.4.3
+version = 0.4.4
 author = Christian Köhlke
 author_email = christian@koehlke.de
 description = this is a Python libary to drive a stepper motor with a Trinamic TMC2209 stepper driver and a Raspberry Pi
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Chr157i4n/TMC2209_Raspberry_Pi
 project_urls =
```

### Comparing `TMC_2209_Raspberry_Pi-0.4.3/src/TMC_2209/TMC_2209_StepperDriver.py` & `tmc_2209_raspberry_pi-0.4.4/src/TMC_2209/TMC_2209_StepperDriver.py`

 * *Files 8% similar despite different names*

```diff
@@ -96,29 +96,35 @@
     _movement_thread = None
 
     _deinit_finished = False
 
 
 
     def __init__(self, pin_en, pin_step=-1, pin_dir=-1, baudrate=115200, serialport="/dev/serial0",
-                 driver_address=0, gpio_mode=GPIO.BCM, loglevel=None, skip_uart_init=False):
+                 driver_address=0, gpio_mode=GPIO.BCM, loglevel=None, logprefix=None,
+                 log_handlers=None, skip_uart_init=False):
         """constructor
 
         Args:
             pin_en (int): EN pin number
             pin_step (int, optional): STEP pin number. Defaults to -1.
             pin_dir (int, optional): DIR pin number. Defaults to -1.
             baudrate (int, optional): baudrate. Defaults to 115200.
             serialport (str, optional): serialport path. Defaults to "/dev/serial0".
             driver_address (int, optional): driver adress [0-3]. Defaults to 0.
             gpio_mode (enum, optional): gpio mode. Defaults to GPIO.BCM.
             loglevel (enum, optional): loglevel. Defaults to None.
+            logprefix (str, optional): log prefix. Defaults to None (standard TMC prefix).
+            log_handlers (list, optional): list of logging handlers.
+                Defaults to None (log to console).
             skip_uart_init (bool, optional): skip UART init. Defaults to False.
         """
-        self.tmc_logger = TMC_logger(loglevel, f"TMC2209 {driver_address}")
+        if logprefix is None:
+            logprefix = f"TMC2209 {driver_address}"
+        self.tmc_logger = TMC_logger(loglevel, logprefix, log_handlers)
         self.tmc_uart = tmc_uart(self.tmc_logger, serialport, baudrate, driver_address)
 
 
         self.tmc_logger.log("Init", Loglevel.INFO)
         GPIO.setwarnings(False)
         GPIO.setmode(gpio_mode)
 
@@ -153,15 +159,15 @@
     def __del__(self):
         """destructor"""
         if self._deinit_finished is False:
             self.tmc_logger.log("Deinit", Loglevel.INFO)
 
             self.set_motor_enabled(False)
 
-            self.tmc_logger.log("GPIO cleanup")
+            self.tmc_logger.log("GPIO cleanup", Loglevel.INFO)
             if self._pin_step != -1:
                 GPIO.cleanup(self._pin_step)
             if self._pin_dir != -1:
                 GPIO.cleanup(self._pin_dir)
             if self._pin_en != -1:
                 GPIO.cleanup(self._pin_en)
             if self._pin_stallguard != -1:
```

### Comparing `TMC_2209_Raspberry_Pi-0.4.3/src/TMC_2209/_TMC_2209_GPIO_board.py` & `tmc_2209_raspberry_pi-0.4.4/src/TMC_2209/_TMC_2209_GPIO_board.py`

 * *Files identical despite different names*

### Comparing `TMC_2209_Raspberry_Pi-0.4.3/src/TMC_2209/_TMC_2209_comm.py` & `tmc_2209_raspberry_pi-0.4.4/src/TMC_2209/_TMC_2209_comm.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,61 +14,61 @@
 
 def read_drv_status(self):
     """read the register Adress "DRV_STATUS" and prints all current setting
 
     Returns:
         int: 32bit DRV_STATUS Register
     """
-    self.tmc_logger.log("---")
-    self.tmc_logger.log("DRIVER STATUS:")
+    self.tmc_logger.log("---", Loglevel.INFO)
+    self.tmc_logger.log("DRIVER STATUS:", Loglevel.INFO)
     drvstatus =self.tmc_uart.read_int(tmc_reg.DRVSTATUS)
     self.tmc_logger.log(bin(drvstatus), Loglevel.INFO)
     if drvstatus & tmc_reg.stst:
-        self.tmc_logger.log("Info: motor is standing still")
+        self.tmc_logger.log("Motor is standing still", Loglevel.INFO)
     else:
-        self.tmc_logger.log("Info: motor is running")
+        self.tmc_logger.log("Motor is running", Loglevel.INFO)
 
     if drvstatus & tmc_reg.stealth:
-        self.tmc_logger.log("Info: motor is running on StealthChop")
+        self.tmc_logger.log("Motor is running on StealthChop", Loglevel.INFO)
     else:
-        self.tmc_logger.log("Info: motor is running on SpreadCycle")
+        self.tmc_logger.log("Motor is running on SpreadCycle", Loglevel.INFO)
 
     cs_actual = drvstatus & tmc_reg.cs_actual
     cs_actual = cs_actual >> 16
-    self.tmc_logger.log(f"CS actual: {cs_actual}")
+    self.tmc_logger.log(f"CS actual: {cs_actual}", Loglevel.INFO)
 
     if drvstatus & tmc_reg.olb:
-        self.tmc_logger.log("Warning: Open load detected on phase B")
+        self.tmc_logger.log("Open load detected on phase B", Loglevel.WARNING)
 
     if drvstatus & tmc_reg.ola:
-        self.tmc_logger.log("Warning: Open load detected on phase A")
+        self.tmc_logger.log("Open load detected on phase A", Loglevel.WARNING)
 
     if drvstatus & tmc_reg.s2vsb:
-        self.tmc_logger.log("""Error: Short on low-side MOSFET detected on phase B.
-                    The driver becomes disabled""")
+        self.tmc_logger.log("""Short on low-side MOSFET detected on phase B.
+                    The driver becomes disabled""", Loglevel.ERROR)
 
     if drvstatus & tmc_reg.s2vsa:
-        self.tmc_logger.log("""Error: Short on low-side MOSFET detected on phase A.
-                    The driver becomes disabled""")
+        self.tmc_logger.log("""Short on low-side MOSFET detected on phase A.
+                    The driver becomes disabled""", Loglevel.ERROR)
 
     if drvstatus & tmc_reg.s2gb:
-        self.tmc_logger.log("""Error: Short to GND detected on phase B.
-                            The driver becomes disabled.""")
+        self.tmc_logger.log("""Short to GND detected on phase B.
+                            The driver becomes disabled.""", Loglevel.ERROR)
 
     if drvstatus & tmc_reg.s2ga:
-        self.tmc_logger.log("""Error: Short to GND detected on phase A.
-                            The driver becomes disabled.""")
+        self.tmc_logger.log("""Short to GND detected on phase A.
+                            The driver becomes disabled.""", Loglevel.ERROR)
 
     if drvstatus & tmc_reg.ot:
-        self.tmc_logger.log("Error: Driver Overheating!")
+        self.tmc_logger.log("Driver Overheating!", Loglevel.ERROR)
 
     if drvstatus & tmc_reg.otpw:
-        self.tmc_logger.log("Warning: Driver Overheating Prewarning!")
+        self.tmc_logger.log("Driver Overheating Prewarning!", Loglevel.WARNING)
 
-    self.tmc_logger.log("---")
+    self.tmc_logger.log("---", Loglevel.INFO)
     return drvstatus
 
 
 
 def read_gconf(self):
     """read the register Adress "GCONF" and prints all current setting
 
@@ -77,69 +77,72 @@
     """
     self.tmc_logger.log("---")
     self.tmc_logger.log("GENERAL CONFIG")
     gconf = self.tmc_uart.read_int(tmc_reg.GCONF)
     self.tmc_logger.log(bin(gconf), Loglevel.INFO)
 
     if gconf & tmc_reg.i_scale_analog:
-        self.tmc_logger.log("Driver is using voltage supplied to VREF as current reference")
+        self.tmc_logger.log("Driver is using voltage supplied to VREF as current reference",
+                            Loglevel.INFO)
     else:
-        self.tmc_logger.log("Driver is using internal reference derived from 5VOUT")
+        self.tmc_logger.log("Driver is using internal reference derived from 5VOUT", Loglevel.INFO)
     if gconf & tmc_reg.internal_rsense:
         self.tmc_logger.log("""Internal sense resistors.
-                            Use current supplied into VREF as reference.""")
-        self.tmc_logger.log("VREF pin internally is driven to GND in this mode.")
-        self.tmc_logger.log("This will most likely destroy your driver!!!")
+                            Use current supplied into VREF as reference.""", Loglevel.WARNING)
+        self.tmc_logger.log("VREF pin internally is driven to GND in this mode.", Loglevel.WARNING)
+        self.tmc_logger.log("This will most likely destroy your driver!!!", Loglevel.WARNING)
         raise SystemExit
-    self.tmc_logger.log("Operation with external sense resistors")
+    self.tmc_logger.log("Operation with external sense resistors", Loglevel.INFO)
     if gconf & tmc_reg.en_spreadcycle:
-        self.tmc_logger.log("SpreadCycle mode enabled")
+        self.tmc_logger.log("SpreadCycle mode enabled", Loglevel.INFO)
     else:
-        self.tmc_logger.log("StealthChop PWM mode enabled")
+        self.tmc_logger.log("StealthChop PWM mode enabled", Loglevel.INFO)
     if gconf & tmc_reg.shaft:
-        self.tmc_logger.log("Inverse motor direction")
+        self.tmc_logger.log("Inverse motor direction", Loglevel.INFO)
     else:
-        self.tmc_logger.log("normal motor direction")
+        self.tmc_logger.log("Normal motor direction", Loglevel.INFO)
     if gconf & tmc_reg.index_otpw:
-        self.tmc_logger.log("INDEX pin outputs overtemperature prewarning flag")
+        self.tmc_logger.log("INDEX pin outputs overtemperature prewarning flag", Loglevel.INFO)
     else:
-        self.tmc_logger.log("INDEX shows the first microstep position of sequencer")
+        self.tmc_logger.log("INDEX shows the first microstep position of sequencer", Loglevel.INFO)
     if gconf & tmc_reg.index_step:
-        self.tmc_logger.log("INDEX output shows step pulses from internal pulse generator")
+        self.tmc_logger.log("INDEX output shows step pulses from internal pulse generator",
+                            Loglevel.INFO)
     else:
-        self.tmc_logger.log("INDEX output as selected by index_otpw")
+        self.tmc_logger.log("INDEX output as selected by index_otpw", Loglevel.INFO)
     if gconf & tmc_reg.mstep_reg_select:
-        self.tmc_logger.log("Microstep resolution selected by MSTEP register")
+        self.tmc_logger.log("Microstep resolution selected by MSTEP register", Loglevel.INFO)
     else:
-        self.tmc_logger.log("Microstep resolution selected by pins MS1, MS2")
+        self.tmc_logger.log("Microstep resolution selected by pins MS1, MS2", Loglevel.INFO)
 
-    self.tmc_logger.log("---")
+    self.tmc_logger.log("---", Loglevel.INFO)
     return gconf
 
 
 
 def read_gstat(self):
     """read the register Adress "GSTAT" and prints all current setting
 
     Returns:
         int: 3bit GSTAT Register
     """
-    self.tmc_logger.log("---")
-    self.tmc_logger.log("GSTAT")
+    self.tmc_logger.log("---", Loglevel.INFO)
+    self.tmc_logger.log("GSTAT", Loglevel.INFO)
     gstat = self.tmc_uart.read_int(tmc_reg.GSTAT)
     self.tmc_logger.log(bin(gstat), Loglevel.INFO)
     if gstat & tmc_reg.reset:
-        self.tmc_logger.log("The Driver has been reset since the last read access to GSTAT")
+        self.tmc_logger.log("The Driver has been reset since the last read access to GSTAT",
+                            Loglevel.WARNING)
     if gstat & tmc_reg.drv_err:
         self.tmc_logger.log("""The driver has been shut down due to overtemperature or
-                    short circuit detection since the last read access""")
+                    short circuit detection since the last read access""", Loglevel.ERROR)
     if gstat & tmc_reg.uv_cp:
         self.tmc_logger.log("""Undervoltage on the charge pump.
-                            The driver is disabled in this case""")
-    self.tmc_logger.log("---")
+                            The driver is disabled in this case""", Loglevel.ERROR)
+    self.tmc_logger.log("---", Loglevel.INFO)
     return gstat
 
 
 
 def clear_gstat(self):
     """clears the "GSTAT" register"""
     self.tmc_logger.log("clearing GSTAT", Loglevel.INFO)
@@ -154,65 +157,66 @@
 
 def read_ioin(self):
     """read the register Adress "IOIN" and prints all current setting
 
     Returns:
         int: 10+8bit IOIN Register
     """
-    self.tmc_logger.log("---")
-    self.tmc_logger.log("INPUTS")
+    self.tmc_logger.log("---", Loglevel.INFO)
+    self.tmc_logger.log("INPUTS", Loglevel.INFO)
     ioin = self.tmc_uart.read_int(tmc_reg.IOIN)
     self.tmc_logger.log(bin(ioin), Loglevel.INFO)
     if ioin & tmc_reg.io_spread:
-        self.tmc_logger.log("spread is high")
+        self.tmc_logger.log("spread is high", Loglevel.INFO)
     else:
-        self.tmc_logger.log("spread is low")
+        self.tmc_logger.log("spread is low", Loglevel.INFO)
 
     if ioin & tmc_reg.io_dir:
-        self.tmc_logger.log("dir is high")
+        self.tmc_logger.log("dir is high", Loglevel.INFO)
     else:
-        self.tmc_logger.log("dir is low")
+        self.tmc_logger.log("dir is low", Loglevel.INFO)
 
     if ioin & tmc_reg.io_step:
-        self.tmc_logger.log("step is high")
+        self.tmc_logger.log("step is high", Loglevel.INFO)
     else:
-        self.tmc_logger.log("step is low")
+        self.tmc_logger.log("step is low", Loglevel.INFO)
 
     if ioin & tmc_reg.io_enn:
-        self.tmc_logger.log("en is high")
+        self.tmc_logger.log("en is high", Loglevel.INFO)
     else:
-        self.tmc_logger.log("en is low")
+        self.tmc_logger.log("en is low", Loglevel.INFO)
 
-    self.tmc_logger.log("---")
+    self.tmc_logger.log("---", Loglevel.INFO)
     return ioin
 
 
 
 def read_chopconf(self):
     """read the register Adress "CHOPCONF" and prints all current setting
 
     Returns:
         int: 3bit CHOPCONF Register
     """
-    self.tmc_logger.log("---")
-    self.tmc_logger.log("CHOPPER CONTROL")
+    self.tmc_logger.log("---", Loglevel.INFO)
+    self.tmc_logger.log("CHOPPER CONTROL", Loglevel.INFO)
     chopconf = self.tmc_uart.read_int(tmc_reg.CHOPCONF)
     self.tmc_logger.log(bin(chopconf), Loglevel.INFO)
 
-    self.tmc_logger.log(f"native {self.get_microstepping_resolution()} microstep setting")
+    self.tmc_logger.log(f"native {self.get_microstepping_resolution()} microstep setting",
+                        Loglevel.INFO)
 
     if chopconf & tmc_reg.intpol:
-        self.tmc_logger.log("interpolation to 256 µsteps")
+        self.tmc_logger.log("interpolation to 256 µsteps", Loglevel.INFO)
 
     if chopconf & tmc_reg.vsense:
-        self.tmc_logger.log("1: High sensitivity, low sense resistor voltage")
+        self.tmc_logger.log("1: High sensitivity, low sense resistor voltage", Loglevel.INFO)
     else:
-        self.tmc_logger.log("0: Low sensitivity, high sense resistor voltage")
+        self.tmc_logger.log("0: Low sensitivity, high sense resistor voltage", Loglevel.INFO)
 
-    self.tmc_logger.log("---")
+    self.tmc_logger.log("---", Loglevel.INFO)
     return chopconf
 
 
 
 def get_direction_reg(self):
     """returns the motor shaft direction: False = CCW; True = CW
```

### Comparing `TMC_2209_Raspberry_Pi-0.4.3/src/TMC_2209/_TMC_2209_math.py` & `tmc_2209_raspberry_pi-0.4.4/src/TMC_2209/_TMC_2209_math.py`

 * *Files identical despite different names*

### Comparing `TMC_2209_Raspberry_Pi-0.4.3/src/TMC_2209/_TMC_2209_move.py` & `tmc_2209_raspberry_pi-0.4.4/src/TMC_2209/_TMC_2209_move.py`

 * *Files identical despite different names*

### Comparing `TMC_2209_Raspberry_Pi-0.4.3/src/TMC_2209/_TMC_2209_reg.py` & `tmc_2209_raspberry_pi-0.4.4/src/TMC_2209/_TMC_2209_reg.py`

 * *Files identical despite different names*

### Comparing `TMC_2209_Raspberry_Pi-0.4.3/src/TMC_2209/_TMC_2209_test.py` & `tmc_2209_raspberry_pi-0.4.4/src/TMC_2209/_TMC_2209_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -112,42 +112,42 @@
     self.tmc_logger.log(str(rtn.hex()), Loglevel.DEBUG)
 
     self.tmc_logger.log("just the first 4 bits:", Loglevel.DEBUG)
     self.tmc_logger.log(str(snd[0:4].hex()), Loglevel.DEBUG)
     self.tmc_logger.log(str(rtn[0:4].hex()), Loglevel.DEBUG)
 
     if len(rtn)==12:
-        self.tmc_logger.log("""the Raspberry Pi received the sended
-                            bits and the answer from the TMC""",Loglevel.INFO)
+        self.tmc_logger.log("""the Raspberry Pi received the sent
+                            bits and the answer from the TMC""", Loglevel.DEBUG)
     elif len(rtn)==4:
-        self.tmc_logger.log("the Raspberry Pi received only the sended bits",
-                            Loglevel.INFO)
+        self.tmc_logger.log("the Raspberry Pi received only the sent bits",
+                            Loglevel.ERROR)
         status = False
     elif len(rtn)==0:
         self.tmc_logger.log("the Raspberry Pi did not receive anything",
-                            Loglevel.INFO)
+                            Loglevel.ERROR)
         status = False
     else:
         self.tmc_logger.log(f"the Raspberry Pi received an unexpected amount of bits: {len(rtn)}",
-                            Loglevel.INFO)
+                            Loglevel.ERROR)
         status = False
 
     if snd[0:4] == rtn[0:4]:
         self.tmc_logger.log("""the Raspberry Pi received exactly the bits it has send.
-                    the first 4 bits are the same""", Loglevel.INFO)
+                    the first 4 bits are the same""", Loglevel.DEBUG)
     else:
         self.tmc_logger.log("""the Raspberry Pi did not received the bits it has send.
-                    the first 4 bits are different""", Loglevel.INFO)
+                    the first 4 bits are different""", Loglevel.DEBUG)
         status = False
 
     self.tmc_logger.log("---")
     if status:
-        self.tmc_logger.log("UART connection: OK")
+        self.tmc_logger.log("UART connection: OK", Loglevel.INFO)
     else:
-        self.tmc_logger.log("UART connection: not OK")
+        self.tmc_logger.log("UART connection: not OK", Loglevel.ERROR)
 
     self.tmc_logger.log("---")
     return True
 
 
 
 def test_stallguard_threshold(self, steps):
```

### Comparing `TMC_2209_Raspberry_Pi-0.4.3/src/TMC_2209/_TMC_2209_uart.py` & `tmc_2209_raspberry_pi-0.4.4/src/TMC_2209/_TMC_2209_uart.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 """
 
 import time
 import struct
 import serial
 
 from . import _TMC_2209_reg as reg
+from ._TMC_2209_logger import Loglevel
 
 
 class TMC_UART:
     """TMC_UART
 
     this class is used to communicate with the TMC via UART
     it can be used to change the settings of the TMC.
@@ -113,15 +114,15 @@
 
         self.r_frame[1] = self.mtr_id
         self.r_frame[2] = register
         self.r_frame[3] = self.compute_crc8_atm(self.r_frame[:-1])
 
         rtn = self.ser.write(self.r_frame)
         if rtn != len(self.r_frame):
-            self.tmc_logger.log("Err in write")
+            self.tmc_logger.log("Err in write", Loglevel.ERROR)
             return False
 
         # adjust per baud and hardware. Sequential reads without some delay fail.
         time.sleep(self.communication_pause)
 
         rtn = self.ser.read(12)
         #self.tmc_logger.log(f"received {len(rtn)} bytes; {len(rtn*8)} bits")
@@ -145,24 +146,25 @@
             tries -= 1
             rtn = self.read_reg(register)
             rtn_data = rtn[7:11]
             not_zero_count = len([elem for elem in rtn if elem != 0])
 
             if(len(rtn)<12 or not_zero_count == 0):
                 self.tmc_logger.log(f"""UART Communication Error:
-                                    {len(rtn_data)} data bytes | {len(rtn)} total bytes""")
+                                    {len(rtn_data)} data bytes |
+                                    {len(rtn)} total bytes""", Loglevel.ERROR)
             elif rtn[11] != self.compute_crc8_atm(rtn[4:11]):
-                self.tmc_logger.log("UART Communication Error: CRC MISMATCH")
+                self.tmc_logger.log("UART Communication Error: CRC MISMATCH", Loglevel.ERROR)
             else:
                 break
 
             if tries<=0:
-                self.tmc_logger.log("after 10 tries not valid answer")
-                self.tmc_logger.log(f"snd:\t{bytes(self.r_frame)}")
-                self.tmc_logger.log(f"rtn:\t{rtn}")
+                self.tmc_logger.log("after 10 tries not valid answer", Loglevel.ERROR)
+                self.tmc_logger.log(f"snd:\t{bytes(self.r_frame)}", Loglevel.DEBUG)
+                self.tmc_logger.log(f"rtn:\t{rtn}", Loglevel.DEBUG)
                 self.handle_error()
                 return -1
 
         val = struct.unpack(">i",rtn_data)[0]
         return val
 
 
@@ -190,15 +192,15 @@
         self.w_frame[6] = 0xFF & val
 
         self.w_frame[7] = self.compute_crc8_atm(self.w_frame[:-1])
 
 
         rtn = self.ser.write(self.w_frame)
         if rtn != len(self.w_frame):
-            self.tmc_logger.log("Err in write")
+            self.tmc_logger.log("Err in write", Loglevel.ERROR)
             return False
 
         time.sleep(self.communication_pause)
 
         return True
 
 
@@ -219,20 +221,20 @@
             ifcnt1 = -1
 
         while True:
             self.write_reg(register, val)
             tries -= 1
             ifcnt2 = self.read_int(reg.IFCNT)
             if ifcnt1 >= ifcnt2:
-                self.tmc_logger.log("writing not successful!")
-                self.tmc_logger.log("ifcnt:",ifcnt1,ifcnt2)
+                self.tmc_logger.log("writing not successful!", Loglevel.ERROR)
+                self.tmc_logger.log("ifcnt:",ifcnt1,ifcnt2, Loglevel.DEBUG)
             else:
                 return True
             if tries<=0:
-                self.tmc_logger.log("after 10 tries no valid write access")
+                self.tmc_logger.log("after 10 tries no valid write access", Loglevel.ERROR)
                 self.handle_error()
                 return -1
 
 
 
     def flush_serial_buffer(self):
         """this function clear the communication buffers of the Raspberry Pi"""
@@ -267,29 +269,30 @@
 
     def handle_error(self):
         """error handling"""
         if self.error_handler_running:
             return
         self.error_handler_running = True
         gstat = self.read_int(reg.GSTAT)
-        self.tmc_logger.log("GSTAT Error check:")
+        self.tmc_logger.log("GSTAT Error check:", Loglevel.DEBUG)
         if gstat == -1:
-            self.tmc_logger.log("No answer from Driver")
+            self.tmc_logger.log("No answer from Driver", Loglevel.DEBUG)
         elif gstat == 0:
-            self.tmc_logger.log("Everything looks fine in GSTAT")
+            self.tmc_logger.log("Everything looks fine in GSTAT", Loglevel.DEBUG)
         else:
             if gstat & reg.reset:
-                self.tmc_logger.log("The Driver has been reset since the last read access to GSTAT")
+                self.tmc_logger.log("The Driver has been reset since the last read access to GSTAT",
+                                    Loglevel.DEBUG)
             if gstat & reg.drv_err:
                 self.tmc_logger.log("""The driver has been shut down due to overtemperature or short
-                      circuit detection since the last read access""")
+                      circuit detection since the last read access""", Loglevel.DEBUG)
             if gstat & reg.uv_cp:
                 self.tmc_logger.log("""Undervoltage on the charge pump.
-                      The driver is disabled in this case""")
-        self.tmc_logger.log("EXITING!")
+                      The driver is disabled in this case""", Loglevel.DEBUG)
+        self.tmc_logger.log("EXITING!", Loglevel.INFO)
         raise SystemExit
 
 
 
     def test_uart(self, register):
         """test UART connection
 
@@ -302,22 +305,22 @@
 
         self.r_frame[1] = self.mtr_id
         self.r_frame[2] = register
         self.r_frame[3] = self.compute_crc8_atm(self.r_frame[:-1])
 
         rtn = self.ser.write(self.r_frame)
         if rtn != len(self.r_frame):
-            self.tmc_logger.log("Err in write")
+            self.tmc_logger.log("Err in write", Loglevel.ERROR)
             return False
 
         # adjust per baud and hardware. Sequential reads without some delay fail.
         time.sleep(self.communication_pause)
 
         rtn = self.ser.read(12)
-        self.tmc_logger.log(f"received {len(rtn)} bytes; {len(rtn)*8} bits")
-        self.tmc_logger.log(f"hex: {rtn.hex()}")
+        self.tmc_logger.log(f"received {len(rtn)} bytes; {len(rtn)*8} bits", Loglevel.DEBUG)
+        self.tmc_logger.log(f"hex: {rtn.hex()}", Loglevel.DEBUG)
         rtn_bin = format(int(rtn.hex(),16), f"0>{len(rtn)*8}b")
-        self.tmc_logger.log(f"bin: {rtn_bin}")
+        self.tmc_logger.log(f"bin: {rtn_bin}", Loglevel.DEBUG)
 
         time.sleep(self.communication_pause)
 
         return bytes(self.r_frame), rtn
```

### Comparing `TMC_2209_Raspberry_Pi-0.4.3/src/TMC_2209_Raspberry_Pi.egg-info/PKG-INFO` & `tmc_2209_raspberry_pi-0.4.4/src/TMC_2209_Raspberry_Pi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TMC_2209_Raspberry_Pi
-Version: 0.4.3
+Version: 0.4.4
 Summary: this is a Python libary to drive a stepper motor with a Trinamic TMC2209 stepper driver and a Raspberry Pi
 Home-page: https://github.com/Chr157i4n/TMC2209_Raspberry_Pi
 Author: Christian Köhlke
 Author-email: christian@koehlke.de
 Project-URL: Bug Tracker, https://github.com/Chr157i4n/TMC2209_Raspberry_Pi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `TMC_2209_Raspberry_Pi-0.4.3/src/TMC_2209_Raspberry_Pi.egg-info/SOURCES.txt` & `tmc_2209_raspberry_pi-0.4.4/src/TMC_2209_Raspberry_Pi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TMC_2209_Raspberry_Pi-0.4.3/tests/test_TMC_2209_math.py` & `tmc_2209_raspberry_pi-0.4.4/tests/test_TMC_2209_math.py`

 * *Files identical despite different names*

### Comparing `TMC_2209_Raspberry_Pi-0.4.3/tests/test_TMC_2209_move.py` & `tmc_2209_raspberry_pi-0.4.4/tests/test_TMC_2209_move.py`

 * *Files identical despite different names*

### Comparing `TMC_2209_Raspberry_Pi-0.4.3/tests/test_TMC_2209_uart.py` & `tmc_2209_raspberry_pi-0.4.4/tests/test_TMC_2209_uart.py`

 * *Files identical despite different names*

