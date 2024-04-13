# Comparing `tmp/inpost-0.1.5a2.tar.gz` & `tmp/inpost-0.2.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inpost-0.1.5a2.tar", max compression
+gzip compressed data, was "inpost-0.2.0a2.tar", max compression
```

## Comparing `inpost-0.1.5a2.tar` & `inpost-0.2.0a2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1307 2023-06-24 19:18:25.396890 inpost-0.1.5a2/README.md
--rw-r--r--   0        0        0       24 2023-01-11 14:04:51.297207 inpost-0.1.5a2/inpost/__init__.py
--rw-r--r--   0        0        0    59170 2023-07-23 09:01:08.211300 inpost-0.1.5a2/inpost/api.py
--rw-r--r--   0        0        0     3541 2023-06-24 17:20:24.712098 inpost-0.1.5a2/inpost/static/__init__.py
--rw-r--r--   0        0        0     2951 2023-06-24 16:59:22.179852 inpost-0.1.5a2/inpost/static/endpoints.py
--rw-r--r--   0        0        0     2715 2023-06-24 17:48:43.048073 inpost-0.1.5a2/inpost/static/exceptions.py
--rw-r--r--   0        0        0     2677 2023-06-24 21:04:10.186415 inpost-0.1.5a2/inpost/static/friends.py
--rw-r--r--   0        0        0       47 2023-01-08 12:39:56.709189 inpost-0.1.5a2/inpost/static/headers.py
--rw-r--r--   0        0        0     1559 2023-06-24 20:38:42.495391 inpost-0.1.5a2/inpost/static/notifications.py
--rw-r--r--   0        0        0    46977 2023-07-02 08:49:07.499846 inpost-0.1.5a2/inpost/static/parcels.py
--rw-r--r--   0        0        0     8116 2023-06-24 19:22:24.781835 inpost-0.1.5a2/inpost/static/statuses.py
--rw-r--r--   0        0        0     1517 2023-07-23 09:00:39.784483 inpost-0.1.5a2/pyproject.toml
--rw-r--r--   0        0        0     2225 1970-01-01 00:00:00.000000 inpost-0.1.5a2/setup.py
--rw-r--r--   0        0        0     2522 1970-01-01 00:00:00.000000 inpost-0.1.5a2/PKG-INFO
+-rw-r--r--   0        0        0    26525 2024-03-08 14:38:28.982854 inpost-0.2.0a2/LICENSE
+-rw-r--r--   0        0        0     1307 2024-03-08 14:38:28.982854 inpost-0.2.0a2/README.md
+-rw-r--r--   0        0        0       24 2024-03-08 14:38:28.996188 inpost-0.2.0a2/inpost/__init__.py
+-rw-r--r--   0        0        0    59945 2024-04-13 16:44:19.776055 inpost-0.2.0a2/inpost/api.py
+-rw-r--r--   0        0        0     3599 2024-03-08 14:38:28.996188 inpost-0.2.0a2/inpost/static/__init__.py
+-rw-r--r--   0        0        0     2963 2024-04-13 15:44:11.831868 inpost-0.2.0a2/inpost/static/endpoints.py
+-rw-r--r--   0        0        0     2715 2024-03-08 14:38:28.996188 inpost-0.2.0a2/inpost/static/exceptions.py
+-rw-r--r--   0        0        0     2677 2024-03-08 14:38:28.996188 inpost-0.2.0a2/inpost/static/friends.py
+-rw-r--r--   0        0        0      165 2024-04-13 10:05:34.738146 inpost-0.2.0a2/inpost/static/headers.py
+-rw-r--r--   0        0        0     1559 2024-03-08 14:38:28.996188 inpost-0.2.0a2/inpost/static/notifications.py
+-rw-r--r--   0        0        0    46910 2024-04-13 15:34:10.406771 inpost-0.2.0a2/inpost/static/parcels.py
+-rw-r--r--   0        0        0     8112 2024-03-08 14:38:28.996188 inpost-0.2.0a2/inpost/static/statuses.py
+-rw-r--r--   0        0        0     1525 2024-04-13 16:44:30.042695 inpost-0.2.0a2/pyproject.toml
+-rw-r--r--   0        0        0     2491 1970-01-01 00:00:00.000000 inpost-0.2.0a2/PKG-INFO
```

### Comparing `inpost-0.1.5a2/README.md` & `inpost-0.2.0a2/README.md`

 * *Files identical despite different names*

### Comparing `inpost-0.1.5a2/inpost/api.py` & `inpost-0.2.0a2/inpost/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     SmsCodeError,
     UnauthorizedError,
     UnidentifiedAPIError,
     appjson,
     blik_status_url,
     collect_url,
     compartment_open_url,
+    compartment_reopen_url,
     compartment_status_url,
     confirm_sms_code_url,
     create_blik_url,
     create_url,
     friendship_url,
     logout_url,
     multi_url,
@@ -53,63 +54,85 @@
     shared_url,
     status_sent_url,
     terminate_collect_session_url,
     tracked_url,
     validate_friendship_url,
     validate_sent_url,
 )
+from inpost.static.headers import useragent
 
 
 class Inpost:
     """Python representation of an Inpost app. Essentially implements methods to manage all incoming parcels"""
 
-    def __init__(self, phone_number):
+    def __init__(self,
+                 prefix: str,
+                 phone_number: str,
+                 sms_code=None,
+                 auth_token=None,
+                 refr_token=None,
+                 ):
         """Constructor method
 
         :param phone_number: phone number
         :type phone_number: str
         :raises PhoneNumberError: Wrong phone number format or is not digit
         """
 
         if isinstance(phone_number, int):
             phone_number = str(phone_number)
 
-        if not (len(phone_number) == 9 and phone_number.isdigit()):
-            raise PhoneNumberError(f"Wrong phone number format: {phone_number} (should be 9 digits)")
-
-        self.phone_number: str = phone_number
-        self.sms_code: str | None = None
-        self.auth_token: str | None = None
-        self.refr_token: str | None = None
+        if (not (len(phone_number) == 9 and phone_number.isdigit())
+                or not (prefix.startswith('+') and prefix[1:].isdigit() and 2 <= len(prefix) <= 3)):
+            raise PhoneNumberError(f"Wrong phone number format: {phone_number} "
+                                   f"(should be +xxx123123123 or +xx123123123)")
+        self.prefix: str = prefix
+        self.phone_number: str = phone_number[-9:]
+        self.sms_code: str | None = sms_code
+        self.auth_token: str | None = auth_token
+        self.refr_token: str | None = refr_token
         self.sess: ClientSession = ClientSession()
         self._log = logging.getLogger(f"{self.__class__.__name__}.{phone_number}")
 
         self._log.setLevel(level=logging.DEBUG)
         self._log.info(f"initialized inpost object with phone number {phone_number}")
 
+    @property
+    def combined_phone_number(self) -> str:
+        return self.prefix + self.phone_number
+
+    @property
+    def login_auth_data(self) -> dict:
+        return {
+            "phoneNumber": {
+                "prefix": self.prefix,
+                "value": self.phone_number
+            }
+        }
+
     def __repr__(self):
         return f"{self.__class__.__name__}(phone_number={self.phone_number})"
 
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
         return self.disconnect()
 
     async def request(
-        self,
-        method: str,
-        action: str,
-        url: StrOrURL,
-        auth: bool = True,
-        headers: dict | None = None,
-        params: dict | None = None,
-        data: dict | None = None,
-        autorefresh: bool = True,
-        **kwargs,
+            self,
+            method: str,
+            action: str,
+            url: StrOrURL,
+            auth: bool = True,
+            headers: dict | None = None,
+            params: dict | None = None,
+            data: dict | None = None,
+            autorefresh: bool = True,
+            **kwargs,
     ) -> ClientResponse:
         """Validates sent data and fetches required compartment properties for opening
 
         :param method: HTTP method of request
         :type method: str
         :param action: action type (e.g. "get parcels" or "send sms code") for logging purposes
         :type action: str
@@ -137,14 +160,17 @@
         if auth and headers:
             if "Authorization" in headers:
                 raise ValueError("Both auth==True and Authorization in additional headers")
 
         headers_ = {} if headers is None else headers
 
         if auth:
+            if self.auth_token is None:
+                raise UnauthorizedError("Missing authorization token")
+
             headers_.update({"Authorization": self.auth_token})
 
         resp = await self.sess.request(method, url, headers=headers_, params=params, json=data, **kwargs)
 
         if autorefresh and resp.status == 401:
             await self.refresh_token()
             headers_.update({"Authorization": self.auth_token})
@@ -161,33 +187,14 @@
                 self._log.error(f"could not perform {action}, not found")
                 raise NotFoundError(reason=resp)
             case _:
                 self._log.error(f"could not perform {action}, unhandled status")
 
         raise UnidentifiedAPIError(reason=resp)
 
-    @classmethod
-    def from_dict(cls, data: dict) -> "Inpost":
-        """`Classmethod` to initialize :class:`Inpost` object with dict.
-        Should be used when retrieving configuration from database.
-
-        :param data: User's Inpost data (e.g. phone_number, sms_code, auth_token, refr_token)
-        :type data: dict
-        :return: Inpost object from provided dict
-        :rtype: Inpost
-        """
-
-        inp = cls(phone_number=data["phone_number"])
-        inp.sms_code = data["sms_code"]
-        inp.auth_token = data["auth_token"]
-        inp.refr_token = data["refr_token"]
-
-        inp._log.info("initialized by from_dict")
-        return inp
-
     async def send_sms_code(self) -> bool:
         """Sends sms code to `Inpost.phone_number`
 
         :return: True if sms code is sent else False
         :rtype: bool
         :raises PhoneNumberError: Missing phone number
         """
@@ -198,16 +205,16 @@
         self._log.info("sending sms code")
 
         resp = await self.request(
             method="post",
             action="send sms code",
             url=send_sms_code_url,
             auth=False,
-            headers=None,
-            data={"phoneNumber": f"{self.phone_number}"},
+            headers=useragent | appjson,
+            data=self.login_auth_data,
             autorefresh=False,
         )
 
         return resp.status == 200
 
     async def confirm_sms_code(self, sms_code: str | int) -> bool:
         """Confirms sms code sent to `Inpost.phone_number` and fetches tokens
@@ -226,22 +233,21 @@
         if isinstance(sms_code, int):
             sms_code = str(sms_code)
 
         if len(sms_code) != 6 or not sms_code.isdigit():
             raise SmsCodeError(reason=f"Wrong sms code format: {sms_code} (should be 6 digits)")
 
         self._log.info("confirming sms code")
-
         resp = await self.request(
             method="post",
             action="confirm sms code",
             url=confirm_sms_code_url,
             auth=False,
             headers=appjson,
-            data={"phoneNumber": self.phone_number, "smsCode": sms_code, "phoneOS": "Android"},
+            data={"smsCode": sms_code, "devicePlatform": "Android"} | self.login_auth_data,
             autorefresh=False,
         )
 
         if resp.status == 200:
             auth_token_data = await resp.json()
             self.sms_code = sms_code
             self.refr_token = auth_token_data["refreshToken"]
@@ -339,15 +345,15 @@
             self._log.debug("disconnected")
             return True
 
         self._log.error("could not disconnect")
         return False
 
     async def get_parcel(
-        self, shipment_number: int | str, parcel_type: ParcelType = ParcelType.TRACKED, parse=False
+            self, shipment_number: int | str, parcel_type: ParcelType = ParcelType.TRACKED, parse=False
     ) -> dict | Parcel | SentParcel | ReturnParcel:
         """Fetches single parcel from provided shipment number
 
         :param shipment_number: Parcel's shipment number
         :type shipment_number: int | str
         :param parcel_type: Parcel type (e.g. received, sent, returned)
         :type parcel_type: ParcelType
@@ -381,15 +387,15 @@
             case _:
                 self._log.error(f"unexpected parcel type {parcel_type}")
                 raise ParcelTypeError(reason=f"Unexpected parcel type: {parcel_type}")
 
         resp = await self.request(
             method="get",
             action=f"parcel with shipment number {shipment_number}",
-            url=f"{url}{shipment_number}",
+            url=f"{url}/{shipment_number}",
             auth=True,
             headers=None,
             data=None,
             autorefresh=True,
         )
 
         if resp.status == 200:
@@ -404,20 +410,20 @@
                 case _:
                     self._log.error(f"wrong parcel type {parcel_type}")
                     raise ParcelTypeError(reason=f"Unknown parcel type: {parcel_type}")
 
         raise UnidentifiedAPIError(reason=resp)
 
     async def get_parcels(
-        self,
-        parcel_type: ParcelType = ParcelType.TRACKED,
-        status: ParcelStatus | List[ParcelStatus] | None = None,
-        pickup_point: str | List[str] | None = None,
-        shipment_type: ParcelShipmentType | List[ParcelShipmentType] | None = None,
-        parse: bool = False,
+            self,
+            parcel_type: ParcelType = ParcelType.TRACKED,
+            status: ParcelStatus | List[ParcelStatus] | None = None,
+            pickup_point: str | List[str] | None = None,
+            shipment_type: ParcelShipmentType | List[ParcelShipmentType] | None = None,
+            parse: bool = False,
     ) -> List[dict] | List[Parcel]:
         """Fetches all available parcels for set `Inpost.phone_number` and optionally filters them
 
         :param parcel_type: Parcel type (e.g. received, sent, returned)
         :type parcel_type: ParcelType
         :param status: status that each fetched parcels has to be in
         :type status: ParcelStatus | list[ParcelStatus] | None
@@ -453,15 +459,15 @@
                 self._log.debug(f"getting parcel type {parcel_type}")
                 url = returns_url
             case _:
                 self._log.error(f"wrong parcel type {parcel_type}")
                 raise ParcelTypeError(reason=f"Unknown parcel type: {parcel_type}")
 
         async with await self.request(
-            method="get", action="get parcels", url=url, auth=True, headers=None, data=None, autorefresh=True
+                method="get", action="get parcels", url=url, auth=True, headers=None, data=None, autorefresh=True
         ) as resp:
             if resp.status != 200:
                 self._log.debug(f"Could not get parcels due to HTTP error {resp.status}")
                 raise UnidentifiedAPIError(reason=resp)
 
             self._log.debug(f"received {parcel_type} parcels")
             _parcels = (await resp.json())["parcels"]
@@ -506,15 +512,15 @@
         if not self.auth_token:
             self._log.error("authorization token missing")
             raise NotAuthenticatedError(reason="Not logged in")
 
         resp = await self.request(
             method="get",
             action=f"parcel with multi-compartment uuid {multi_uuid}",
-            url=f"{multi_url}{multi_uuid}",
+            url=f"{multi_url}/{multi_uuid}",
             auth=True,
             headers=None,
             data=None,
             autorefresh=True,
         )
 
         if resp.status == 200:
@@ -524,15 +530,16 @@
                 if not parse
                 else [Parcel(data, logger=self._log) for data in (await resp.json())["parcels"]]
             )
 
         raise UnidentifiedAPIError(reason=resp)
 
     async def collect_compartment_properties(
-        self, shipment_number: str | int | None = None, parcel_obj: Parcel | None = None, location: dict | None = None
+            self, shipment_number: str | int | None = None, parcel_obj: Parcel | None = None,
+            location: dict | None = None
     ) -> Parcel:
         """Validates sent data and fetches required compartment properties for opening
 
         :param shipment_number: Parcel's shipment number
         :type shipment_number: int | str | None
         :param parcel_obj: :class:`Parcel` object to obtain data from
         :type parcel_obj: Parcel | None
@@ -572,15 +579,20 @@
         resp = await self.request(
             method="post",
             action="collect compartment properties",
             url=collect_url,
             auth=True,
             headers=None,
             data={
-                "parcel": parcel_obj_.compartment_open_data,
+                "parcel": parcel_obj_.compartment_open_data | {
+                    "receiverPhoneNumber": {
+                        "prefix": self.prefix,
+                        "value": self.phone_number
+                    },
+                },
                 "geoPoint": location if location is not None else parcel_obj_.mocked_location,
             },
             autorefresh=True,
         )
 
         if resp.status == 200:
             self._log.debug(f"collected compartment properties for {parcel_obj_.shipment_number}")
@@ -622,15 +634,15 @@
             self._log.debug(f"opened compartment for {parcel_obj.shipment_number}")
             parcel_obj.compartment_location = await resp.json()
             return parcel_obj
 
         raise UnidentifiedAPIError(reason=resp)
 
     async def check_compartment_status(
-        self, parcel_obj: Parcel, expected_status: CompartmentExpectedStatus = CompartmentExpectedStatus.OPENED
+            self, parcel_obj: Parcel, expected_status: CompartmentExpectedStatus = CompartmentExpectedStatus.OPENED
     ) -> bool:
         """Checks and compare compartment status (e.g. opened, closed) with expected status
 
         :param parcel_obj: Parcel object
         :type parcel_obj: Parcel
         :param expected_status: Compartment expected status
         :type expected_status: CompartmentExpectedStatus
@@ -660,15 +672,16 @@
             },
             autorefresh=True,
         )
 
         if resp.status == 200:
             self._log.debug(f"checked compartment status for {parcel_obj.shipment_number}")
             parcel_obj.compartment_status = (await resp.json())["status"]
-            return CompartmentExpectedStatus[(await resp.json())["status"]] == expected_status
+            # return CompartmentExpectedStatus[(await resp.json())["status"]] == expected_status
+            return True
 
         raise UnidentifiedAPIError(reason=resp)
 
     async def terminate_collect_session(self, parcel_obj: Parcel) -> bool:
         """Terminates user session in inpost api service
 
         :param parcel_obj: Parcel object
@@ -699,15 +712,15 @@
         if resp.status == 200:
             self._log.debug(f"terminated collect session for {parcel_obj.shipment_number}")
             return True
 
         raise UnidentifiedAPIError(reason=resp)
 
     async def collect(
-        self, shipment_number: str | None = None, parcel_obj: Parcel | None = None, location: dict | None = None
+            self, shipment_number: str | None = None, parcel_obj: Parcel | None = None, location: dict | None = None
     ) -> Parcel | None:
         """Simplified method to open compartment
 
         :param shipment_number: Parcel's shipment number
         :type shipment_number: int | str | None
         :param parcel_obj: :class:`Parcel` object to obtain data from
         :type parcel_obj: Parcel | None
@@ -784,35 +797,35 @@
         if not self.auth_token:
             self._log.debug("authorization token missing")
             raise NotAuthenticatedError(reason="Not logged in")
 
         resp = await self.request(
             method="post",
             action=f"reopen compartment for {parcel_obj.shipment_number}",
-            url=compartment_open_url,
+            url=compartment_reopen_url,
             auth=True,
             headers=None,
             data={"sessionUuid": parcel_obj.compartment_properties.session_uuid},
             autorefresh=True,
         )
 
         if resp.status == 200:
-            self._log.debug(f"opened compartment for {parcel_obj.shipment_number}")
+            self._log.debug(f"reopened compartment for {parcel_obj.shipment_number}")
             return True
 
         raise UnidentifiedAPIError(reason=resp)
 
     async def get_parcel_points(
-        self,
-        query: str | None = None,
-        latitude: float | None = None,
-        longitude: float | None = None,
-        per_page: int = 1000,
-        operation: ParcelPointOperations = ParcelPointOperations.CREATE,
-        parse: bool = True,
+            self,
+            query: str | None = None,
+            latitude: float | None = None,
+            longitude: float | None = None,
+            per_page: int = 1000,
+            operation: ParcelPointOperations = ParcelPointOperations.CREATE,
+            parse: bool = True,
     ) -> dict | List[Point]:
         """Fetches parcel points for inpost services
 
         :param query: parcel point search query (e.g. GXO05M)
         :type query: str | None
         :param latitude: latitude of place we are looking for nearby parcel points
         :type latitude: float | None
@@ -898,21 +911,21 @@
         if resp.status == 200 and not (await resp.json())["active"]:
             self._log.debug("user has no active blik sessions")
             return True
 
         return False
 
     async def create_parcel(
-        self,
-        delivery_type: DeliveryType,
-        parcel_size: ParcelLockerSize | ParcelCarrierSize,
-        price: float | str,
-        sender: Sender,
-        receiver: Receiver,
-        delivery_point: Point,
+            self,
+            delivery_type: DeliveryType,
+            parcel_size: ParcelLockerSize | ParcelCarrierSize,
+            price: float | str,
+            sender: Sender,
+            receiver: Receiver,
+            delivery_point: Point,
     ) -> dict | None:
         """Fetches parcel points for inpost services
 
         :param delivery_type: a way parcel will be delivered
         :type delivery_type: DeliveryType
         :param parcel_size: size of parcel
         :type parcel_size: ParcelLockerSize | ParcelCarrierSize
@@ -955,15 +968,15 @@
 
         if resp.status == 200:
             return await resp.json()
 
         raise UnidentifiedAPIError(reason=resp)
 
     async def create_blik_session(
-        self, amount: float | str, shipment_number: str, currency: str = "PLN"
+            self, amount: float | str, shipment_number: str, currency: str = "PLN"
     ) -> None | dict:
         """Creates blik session for sending parcel
 
         :param amount: amount of money that has to be paid
         :type amount: float | str
         :param shipment_number: shipment number of parcel that is being sent
         :type shipment_number: str
@@ -1000,19 +1013,19 @@
         if resp.status == 200:
             self._log.debug(f"created blik session for {shipment_number}")
             return await resp.json()
 
         raise UnidentifiedAPIError(reason=resp)
 
     async def validate_send(
-        self,
-        drop_off_point: str,
-        shipment_number: str | None = None,
-        parcel_obj: SentParcel | None = None,
-        location: dict | None = None,
+            self,
+            drop_off_point: str,
+            shipment_number: str | None = None,
+            parcel_obj: SentParcel | None = None,
+            location: dict | None = None,
     ) -> SentParcel:
         """Validates sending parcel
 
         :param drop_off_point: parcel machine codename where you want to drop-opp parcel
         :type drop_off_point: str
         :param shipment_number: sent parcel shipment number
         :type shipment_number: str | None
@@ -1128,29 +1141,29 @@
         if not self.auth_token:
             self._log.debug("authorization token missing")
             raise NotAuthenticatedError(reason="Not logged in")
 
         resp = await self.request(
             method="post",
             action=f"reopen compartment for {parcel_obj.shipment_number}",
-            url=compartment_open_url,
+            url=compartment_reopen_url,
             auth=True,
             headers=None,
             data={"sessionUuid": parcel_obj.compartment_properties.session_uuid},
             autorefresh=True,
         )
 
         if resp.status == 200:
-            self._log.debug(f"opened send compartment for {parcel_obj.shipment_number}")
+            self._log.debug(f"reopened send compartment for {parcel_obj.shipment_number}")
             return True
 
         return False
 
     async def check_send_compartment_status(
-        self, parcel_obj: SentParcel, expected_status: CompartmentExpectedStatus = CompartmentExpectedStatus.OPENED
+            self, parcel_obj: SentParcel, expected_status: CompartmentExpectedStatus = CompartmentExpectedStatus.OPENED
     ) -> bool:
         """Checks and compare compartment status (e.g. opened, closed) with expected status
 
         :param parcel_obj: Parcel object
         :type parcel_obj: SentParcel
         :param expected_status: Compartment expected status
         :type expected_status: CompartmentExpectedStatus
@@ -1511,15 +1524,22 @@
         resp = await self.request(
             method="post",
             action=f"share parcel: {shipment_number}",
             url=shared_url,
             auth=True,
             headers=None,
             data={
-                "parcels": [{"shipmentNumber": shipment_number, "friendUuids": [uuid]}],
+                "parcels": [
+                    {
+                        "shipmentNumber": shipment_number,
+                        "friendUuids": [
+                            uuid
+                        ]
+                    }
+                ],
             },
             autorefresh=True,
         )
 
         if resp.status == 200:
             self._log.debug("updated user friend")
             return True
```

### Comparing `inpost-0.1.5a2/inpost/static/__init__.py` & `inpost-0.2.0a2/inpost/static/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from .endpoints import (
     accept_friendship_url,
     blik_status_url,
     collect_url,
     compartment_open_url,
+    compartment_reopen_url,
     compartment_status_url,
     confirm_sent_url,
     confirm_sms_code_url,
     create_blik_url,
     create_url,
     friendship_url,
     login_url,
@@ -86,14 +87,15 @@
 )
 
 __all__ = [
     "accept_friendship_url",
     "blik_status_url",
     "collect_url",
     "compartment_open_url",
+    "compartment_reopen_url",
     "compartment_status_url",
     "confirm_sent_url",
     "confirm_sms_code_url",
     "create_url",
     "create_blik_url",
     "friendship_url",
     "login_url",
```

### Comparing `inpost-0.1.5a2/inpost/static/endpoints.py` & `inpost-0.2.0a2/inpost/static/endpoints.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # AUTH #
 login_url: str = "https://api-inmobile-pl.easypack24.net/v1/authenticate"
-send_sms_code_url: str = "https://api-inmobile-pl.easypack24.net/v1/sendSMSCode/"  # get
-confirm_sms_code_url: str = "https://api-inmobile-pl.easypack24.net/v1/confirmSMSCode"  # post
+send_sms_code_url: str = "https://api-inmobile-pl.easypack24.net/v1/account"  # post
+confirm_sms_code_url: str = "https://api-inmobile-pl.easypack24.net/v1/account/verification"  # post
 logout_url: str = "https://api-inmobile-pl.easypack24.net/v1/logout"  # post
 refresh_token_url: str = "https://api-inmobile-pl.easypack24.net/v1/authenticate"  # post
 
 # INCOMING PARCELS #
-tracked_url: str = "https://api-inmobile-pl.easypack24.net/v3/parcels/tracked/"  # get
-multi_url: str = "https://api-inmobile-pl.easypack24.net/v3/parcels/multi/"  # get
-collect_url: str = "https://api-inmobile-pl.easypack24.net/v1/collect/validate"  # post
-reopen_url: str = "https://api-inmobile-pl.easypack24.net/v1/collect/compartment/reopen"  # post
+tracked_url: str = "https://api-inmobile-pl.easypack24.net/v4/parcels/tracked"  # get
+multi_url: str = "https://api-inmobile-pl.easypack24.net/v4/parcels/multi"  # get
+collect_url: str = "https://api-inmobile-pl.easypack24.net/v2/collect/validate"  # post
+compartment_reopen_url: str = "https://api-inmobile-pl.easypack24.net/v1/collect/compartment/reopen"  # post
 compartment_open_url: str = "https://api-inmobile-pl.easypack24.net/v1/collect/compartment/open"  # post
 compartment_status_url: str = "https://api-inmobile-pl.easypack24.net/v1/collect/compartment/status"  # post
 terminate_collect_session_url: str = "https://api-inmobile-pl.easypack24.net/v1/collect/terminate"  # post
-shared_url: str = "https://api-inmobile-pl.easypack24.net/v1/parcels/shared"  # post
+shared_url: str = "https://api-inmobile-pl.easypack24.net/v4/parcels/shared"  # post
 
 # CREATING PARCEL #
 create_url: str = "https://api-inmobile-pl.easypack24.net/v1/parcels"
 points_url: str = "https://api-inmobile-pl.easypack24.net/v3/points"
 blik_status_url: str = "https://api-inmobile-pl.easypack24.net/v1/payments/blik/alias/status"
 create_blik_url: str = "https://api-inmobile-pl.easypack24.net/v1/payments/transactions/create/blik"
```

### Comparing `inpost-0.1.5a2/inpost/static/exceptions.py` & `inpost-0.2.0a2/inpost/static/exceptions.py`

 * *Files identical despite different names*

### Comparing `inpost-0.1.5a2/inpost/static/friends.py` & `inpost-0.2.0a2/inpost/static/friends.py`

 * *Files identical despite different names*

### Comparing `inpost-0.1.5a2/inpost/static/notifications.py` & `inpost-0.2.0a2/inpost/static/notifications.py`

 * *Files identical despite different names*

### Comparing `inpost-0.1.5a2/inpost/static/parcels.py` & `inpost-0.2.0a2/inpost/static/parcels.py`

 * *Files 0% similar despite different names*

```diff
@@ -278,15 +278,14 @@
             return None
 
         if self.shipment_type == ParcelShipmentType.parcel:
             self._log.debug("got compartment open data")
             return {
                 "shipmentNumber": self.shipment_number,
                 "openCode": self._open_code,
-                "receiverPhoneNumber": self.receiver.phone_number,
             }
 
         self._log.warning(f"wrong ParcelShipmentType: {repr(self.shipment_type)}")
         return None
 
     @property
     def mocked_location(self) -> dict | None:
```

### Comparing `inpost-0.1.5a2/inpost/static/statuses.py` & `inpost-0.2.0a2/inpost/static/statuses.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from enum import Enum, EnumMeta
 
 
 class Meta(EnumMeta):  # temporary handler for unexpected keys in enums
-    def __getitem__(self, item):
+    def __getitem__(cls, item):
         try:
             return super().__getitem__(item) if item is not None else None
         except KeyError:
-            return self.UNKNOWN
+            return cls.UNKNOWN
 
-    def __getattribute__(self, item):
+    def __getattribute__(cls, item):
         try:
             return super().__getattribute__(item) if item is not None else None
         except KeyError:
-            return self.UNKNOWN
+            return cls.UNKNOWN
 
     # def get_all(cls):
     #     return [getattr(cls, name) for name in cls.__members__]
     #
     # def get_without(cls, without: "ParcelBase" | List["ParcelBase"]):
     #     if isinstance(without, ParcelBase):
     #         without = [without]
```

### Comparing `inpost-0.1.5a2/pyproject.toml` & `inpost-0.2.0a2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [tool.poetry]
 name = "inpost"
-version = "0.1.5a2"
+version = "0.2.0a2"
 description = "Asynchronous InPost package allowing you to manage existing incoming parcels without mobile app"
 authors = ["loboda4450 <loboda4450@gmail.com>", "MrKazik99 <mrkazik99@gmail.com>"]
 maintainers = ["loboda4450 <loboda4450@gmail.com>"]
 documentation = 'https://inpost-python.readthedocs.io/en/latest/index.html'
+license = 'LGPL-2.1-only'
 repository = "https://github.com/IFOSSA/inpost-python"
 readme = "README.md"
 packages = [
         {include = 'inpost'},
         {include = 'inpost/static'}
     ]
 classifiers = [
@@ -18,24 +19,23 @@
         "Intended Audience :: Developers",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: POSIX :: Linux",
         "Development Status :: 3 - Alpha"
     ]
 
 [tool.poetry.dev-dependencies]
-pre-commit = "^3.3.3"
-pytest = "^7.4.0"
+pre-commit = "^3.7.0"
+pytest = "^8.1.1"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-aiohttp = "^3.8.1"
+aiohttp = "^3.9.4"
 arrow = "^1.2.3"
 qrcode = "^7.3.1"
 Pillow = "^9.4.0"
-pytest = "^7.4.0"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
```

### Comparing `inpost-0.1.5a2/setup.py` & `inpost-0.2.0a2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,81 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: inpost
+Version: 0.2.0a2
+Summary: Asynchronous InPost package allowing you to manage existing incoming parcels without mobile app
+Home-page: https://github.com/IFOSSA/inpost-python
+License: LGPL-2.1-only
+Author: loboda4450
+Author-email: loboda4450@gmail.com
+Maintainer: loboda4450
+Maintainer-email: loboda4450@gmail.com
+Requires-Python: >=3.10,<4.0
+Classifier: Development Status :: 3 - Alpha
+Classifier: Framework :: aiohttp
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: Pillow (>=9.4.0,<10.0.0)
+Requires-Dist: aiohttp (>=3.9.4,<4.0.0)
+Requires-Dist: arrow (>=1.2.3,<2.0.0)
+Requires-Dist: qrcode (>=7.3.1,<8.0.0)
+Project-URL: Documentation, https://inpost-python.readthedocs.io/en/latest/index.html
+Project-URL: Repository, https://github.com/IFOSSA/inpost-python
+Description-Content-Type: text/markdown
 
-packages = \
-['inpost', 'inpost.static', 'static']
+[![CodeFactor](https://www.codefactor.io/repository/github/ifossa/inpost-python/badge)](https://www.codefactor.io/repository/github/ifossa/inpost-python)
+![Code Quality](https://github.com/ifossa/inpost-python/actions/workflows/lint.yml/badge.svg?barnch=main)
+![Todos](https://github.com/ifossa/inpost-python/actions/workflows/todos.yml/badge.svg?barnch=main)
 
-package_data = \
-{'': ['*']}
+# Inpost Python
 
-install_requires = \
-['Pillow>=9.4.0,<10.0.0',
- 'aiohttp>=3.8.1,<4.0.0',
- 'arrow>=1.2.3,<2.0.0',
- 'pytest>=7.4.0,<8.0.0',
- 'qrcode>=7.3.1,<8.0.0']
-
-setup_kwargs = {
-    'name': 'inpost',
-    'version': '0.1.5a2',
-    'description': 'Asynchronous InPost package allowing you to manage existing incoming parcels without mobile app',
-    'long_description': "[![CodeFactor](https://www.codefactor.io/repository/github/ifossa/inpost-python/badge)](https://www.codefactor.io/repository/github/ifossa/inpost-python)\n![Code Quality](https://github.com/ifossa/inpost-python/actions/workflows/lint.yml/badge.svg?barnch=main)\n![Todos](https://github.com/ifossa/inpost-python/actions/workflows/todos.yml/badge.svg?barnch=main)\n\n# Inpost Python\n\nFully async Inpost library using Python 3.10.\n\n\n## Documentation\n\n[Readthedocs.io](https://inpost-python.readthedocs.io/en/latest/)\n\n\n## Usage/Examples\n\n\n```python\nfrom inpost.api import Inpost\n\ninp = Inpost('555333444')\nawait inp.send_sms_code():\n...\nif await inp.confirm_sms_code(123321):\n   print('Congratulations, you initialized successfully!')\n```\n\n## Before you contribute\n\n![Contributors](https://contrib.rocks/image?repo=ifossa/inpost-python)\n\nInstall linters and checkers, unlinted pull requests will not be approved\n```commandline\npoetry run pre-commit install\n```\n\n## Authors\n\n- [@loboda4450](https://www.github.com/loboda4450)\n- [@mrkazik99](https://www.github.com/mrkazik99)\n\n\n## Used By\n\nThis project is used by the following repos:\n\n[Inpost Telegram Bot](https://github.com/loboda4450/inpost-telegram-bot)\n\n\n\n## 😂 Here is a random joke that'll make you laugh!\n![Jokes Card](https://readme-jokes.vercel.app/api)",
-    'author': 'loboda4450',
-    'author_email': 'loboda4450@gmail.com',
-    'maintainer': 'loboda4450',
-    'maintainer_email': 'loboda4450@gmail.com',
-    'url': 'https://github.com/IFOSSA/inpost-python',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.10,<4.0',
-}
+Fully async Inpost library using Python 3.10.
 
 
-setup(**setup_kwargs)
+## Documentation
+
+[Readthedocs.io](https://inpost-python.readthedocs.io/en/latest/)
+
+
+## Usage/Examples
+
+
+```python
+from inpost.api import Inpost
+
+inp = Inpost('555333444')
+await inp.send_sms_code():
+...
+if await inp.confirm_sms_code(123321):
+   print('Congratulations, you initialized successfully!')
+```
+
+## Before you contribute
+
+![Contributors](https://contrib.rocks/image?repo=ifossa/inpost-python)
+
+Install linters and checkers, unlinted pull requests will not be approved
+```commandline
+poetry run pre-commit install
+```
+
+## Authors
+
+- [@loboda4450](https://www.github.com/loboda4450)
+- [@mrkazik99](https://www.github.com/mrkazik99)
+
+
+## Used By
+
+This project is used by the following repos:
+
+[Inpost Telegram Bot](https://github.com/loboda4450/inpost-telegram-bot)
+
+
+
+## 😂 Here is a random joke that'll make you laugh!
+![Jokes Card](https://readme-jokes.vercel.app/api)
```

