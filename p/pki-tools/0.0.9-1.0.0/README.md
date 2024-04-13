# Comparing `tmp/pki_tools-0.0.9.tar.gz` & `tmp/pki_tools-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pki_tools-0.0.9.tar", max compression
+gzip compressed data, was "pki_tools-1.0.0.tar", max compression
```

## Comparing `pki_tools-0.0.9.tar` & `pki_tools-1.0.0.tar`

### file list

```diff
@@ -1,9 +1,24 @@
--rw-r--r--   0        0        0     1096 2023-09-17 22:27:01.209783 pki_tools-0.0.9/LICENSE
--rw-r--r--   0        0        0     1276 2023-09-17 22:27:01.209783 pki_tools-0.0.9/README.md
--rw-r--r--   0        0        0     4845 2023-09-17 22:27:01.229783 pki_tools-0.0.9/pki_tools/__init__.py
--rw-r--r--   0        0        0     2688 2023-09-17 22:27:01.229783 pki_tools-0.0.9/pki_tools/crl.py
--rw-r--r--   0        0        0      283 2023-09-17 22:27:01.229783 pki_tools-0.0.9/pki_tools/exceptions.py
--rw-r--r--   0        0        0     3753 2023-09-17 22:27:01.229783 pki_tools-0.0.9/pki_tools/ocsp.py
--rw-r--r--   0        0        0     4960 2023-09-17 22:27:01.229783 pki_tools-0.0.9/pki_tools/types.py
--rw-r--r--   0        0        0     1525 2023-09-17 22:27:11.289866 pki_tools-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     2377 1970-01-01 00:00:00.000000 pki_tools-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1096 2024-04-13 12:56:09.562684 pki_tools-1.0.0/LICENSE
+-rw-r--r--   0        0        0     1967 2024-04-13 12:56:09.562684 pki_tools-1.0.0/README.md
+-rw-r--r--   0        0        0     1321 2024-04-13 12:56:09.570684 pki_tools-1.0.0/pki_tools/__init__.py
+-rw-r--r--   0        0        0     1798 2024-04-13 12:56:09.570684 pki_tools-1.0.0/pki_tools/crl.py
+-rw-r--r--   0        0        0     1397 2024-04-13 12:56:09.570684 pki_tools-1.0.0/pki_tools/exceptions.py
+-rw-r--r--   0        0        0       70 2024-04-13 12:56:09.570684 pki_tools-1.0.0/pki_tools/funcs/__init__.py
+-rw-r--r--   0        0        0     5448 2024-04-13 12:56:09.570684 pki_tools-1.0.0/pki_tools/funcs/check_revocation.py
+-rw-r--r--   0        0        0     5227 2024-04-13 12:56:09.570684 pki_tools-1.0.0/pki_tools/ocsp.py
+-rw-r--r--   0        0        0     1637 2024-04-13 12:56:09.570684 pki_tools-1.0.0/pki_tools/types/__init__.py
+-rw-r--r--   0        0        0    14191 2024-04-13 12:56:09.570684 pki_tools-1.0.0/pki_tools/types/certificate.py
+-rw-r--r--   0        0        0     4652 2024-04-13 12:56:09.570684 pki_tools-1.0.0/pki_tools/types/certificates.py
+-rw-r--r--   0        0        0     3158 2024-04-13 12:56:09.574684 pki_tools-1.0.0/pki_tools/types/chain.py
+-rw-r--r--   0        0        0     7794 2024-04-13 12:56:09.574684 pki_tools-1.0.0/pki_tools/types/crl.py
+-rw-r--r--   0        0        0     7023 2024-04-13 12:56:09.574684 pki_tools-1.0.0/pki_tools/types/crypto_parser.py
+-rw-r--r--   0        0        0     6351 2024-04-13 12:56:09.574684 pki_tools-1.0.0/pki_tools/types/csr.py
+-rw-r--r--   0        0        0      462 2024-04-13 12:56:09.574684 pki_tools-1.0.0/pki_tools/types/enums.py
+-rw-r--r--   0        0        0    50236 2024-04-13 12:56:09.574684 pki_tools-1.0.0/pki_tools/types/extensions.py
+-rw-r--r--   0        0        0    26475 2024-04-13 12:56:09.574684 pki_tools-1.0.0/pki_tools/types/key_pair.py
+-rw-r--r--   0        0        0     4292 2024-04-13 12:56:09.574684 pki_tools-1.0.0/pki_tools/types/name.py
+-rw-r--r--   0        0        0    12326 2024-04-13 12:56:09.574684 pki_tools-1.0.0/pki_tools/types/ocsp.py
+-rw-r--r--   0        0        0     9779 2024-04-13 12:56:09.574684 pki_tools-1.0.0/pki_tools/types/signature_algorithm.py
+-rw-r--r--   0        0        0     1940 2024-04-13 12:56:09.574684 pki_tools-1.0.0/pki_tools/types/utils.py
+-rw-r--r--   0        0        0     1800 2024-04-13 12:56:18.318687 pki_tools-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3195 1970-01-01 00:00:00.000000 pki_tools-1.0.0/PKG-INFO
```

### Comparing `pki_tools-0.0.9/LICENSE` & `pki_tools-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pki_tools-0.0.9/pki_tools/types.py` & `pki_tools-1.0.0/pki_tools/types/name.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,88 +1,44 @@
-import re
-from typing import List
+from collections import defaultdict
+from typing import List, Type
 
 from cryptography import x509
 from cryptography.hazmat._oid import NameOID
-from pydantic import constr, BaseModel, Field, ConfigDict
+from cryptography.hazmat.bindings._rust import ObjectIdentifier
 
+from pydantic import Field, ConfigDict
 
-class PemCert(str):
-    """
-    PemCert is a string containing the PEM formatted certificate
-
-    Example:
-    ::
-        PemCert(
-            \"\"\"
-            -----BEGIN CERTIFICATE-----
-            MIICUTCCAfugAwIBAgIBADANBgkqhkiG9w0BAQQFADBXMQswCQYDVQQGEwJDTjEL
-            MAkGA1UECBMCUE4xCzAJBgNVBAcTAkNOMQswCQYDVQQKEwJPTjELMAkGA1UECxMC
-            VU4xFDASBgNVBAMTC0hlcm9uZyBZYW5nMB4XDTA1MDcxNTIxMTk0N1oXDTA1MDgx
-            NDIxMTk0N1owVzELMAkGA1UEBhMCQ04xCzAJBgNVBAgTAlBOMQswCQYDVQQHEwJD
-            TjELMAkGA1UEChMCT04xCzAJBgNVBAsTAlVOMRQwEgYDVQQDEwtIZXJvbmcgWWFu
-            ZzBcMA0GCSqGSIb3DQEBAQUAA0sAMEgCQQCp5hnG7ogBhtlynpOS21cBewKE/B7j
-            V14qeyslnr26xZUsSVko36ZnhiaO/zbMOoRcKK9vEcgMtcLFuQTWDl3RAgMBAAGj
-            gbEwga4wHQYDVR0OBBYEFFXI70krXeQDxZgbaCQoR4jUDncEMH8GA1UdIwR4MHaA
-            FFXI70krXeQDxZgbaCQoR4jUDncEoVukWTBXMQswCQYDVQQGEwJDTjELMAkGA1UE
-            CBMCUE4xCzAJBgNVBAcTAkNOMQswCQYDVQQKEwJPTjELMAkGA1UECxMCVU4xFDAS
-            BgNVBAMTC0hlcm9uZyBZYW5nggEAMAwGA1UdEwQFMAMBAf8wDQYJKoZIhvcNAQEE
-            BQADQQA/ugzBrjjK9jcWnDVfGHlk3icNRq0oV7Ri32z/+HQX67aRfgZu7KWdI+Ju
-            Wm7DCfrPNGVwFWUQOmsPue9rZBgO
-            -----END CERTIFICATE-----
-            \"\"\"
-        )
-    """
-
-
-PEM_REGEX = re.compile(r"-+BEGIN CERTIFICATE-+[\w+/\s=]*-+END CERTIFICATE-+")
-
-
-class OcspIssuerUri(BaseModel):
-    """
-    Describes the OCSP Issuer (usually a CA) URI where the public certificate
-    can be downloaded
-
-    Examples::
-        OcspIssuerUri(uri="https://my.ca.link.com/ca.pem")
-    Attributes:
-        uri -- The URI for the public issuer certificate
-        cache_time_seconds -- Specifies how long the public cert should be
-        cached, default is 1 month.
-    """
-
-    uri: constr(pattern=r"https*://.*")
-    cache_time_seconds: int = 60 * 60 * 24 * 30
+from pki_tools.types.crypto_parser import CryptoParser
 
 
-class Subject(BaseModel):
+class Name(CryptoParser):
     """
-    Subject type describes certificate subject or issuer.
+    Name type describes e.g. certificate subject or issuer.
     The attributes are following the
     [RFC5280#Section-4.1.2.4](https://datatracker.ietf.org/doc/html/rfc5280#section-4.1.2.4)
 
     Note that every attribute is a list of string in order to support
     multivalued RDNs.
 
     Attributes:
-        c -- Country Name (2.5.4.6)
-        o -- Organization Name (2.5.4.10)
-        ou -- Organizational Unit Name (2.5.4.11)
-        dnq -- Distinguished Name Qualifier (2.5.4.46)
-        s -- State Or Province Name (2.5.4.8)
-        cn -- Common Name (2.5.4.3)
-        serial -- Serial Number (2.5.4.5)
-        ln -- Locality Name (2.5.4.7)
-        t -- Title (2.5.4.12)
-        sn -- Surname (2.5.4.4)
-        gn -- Given Name (2.5.4.42)
-        i -- Initials (2.5.4.43)
-        p -- Pseudonym (2.5.4.65)
-        gq -- Generation Qualifier (2.5.4.44)
-        dc -- Domain Component (0.9.2342.19200300.100.1.25)
+        c: Country Name (2.5.4.6)
+        o:  Organization Name (2.5.4.10)
+        ou:  Organizational Unit Name (2.5.4.11)
+        dnq:  Distinguished Name Qualifier (2.5.4.46)
+        s:  State Or Province Name (2.5.4.8)
+        cn:  Common Name (2.5.4.3)
+        serial:  Serial Number (2.5.4.5)
+        ln:  Locality Name (2.5.4.7)
+        t:  Title (2.5.4.12)
+        sn:  Surname (2.5.4.4)
+        gn:  Given Name (2.5.4.42)
+        i:  Initials (2.5.4.43)
+        p:  Pseudonym (2.5.4.65)
+        gq:  Generation Qualifier (2.5.4.44)
+        dc:  Domain Component (0.9.2342.19200300.100.1.25)
     """
 
     model_config = ConfigDict(populate_by_name=True)
 
     c: List[str] = Field(alias=NameOID.COUNTRY_NAME.dotted_string, default=[])
     o: List[str] = Field(
         alias=NameOID.ORGANIZATION_NAME.dotted_string, default=[]
@@ -112,32 +68,56 @@
     gq: List[str] = Field(
         alias=NameOID.GENERATION_QUALIFIER.dotted_string, default=[]
     )
     dc: List[str] = Field(
         alias=NameOID.DOMAIN_COMPONENT.dotted_string, default=[]
     )
 
-    def to_crypto_name(self) -> x509.Name:
-        name_list = []
-        for attr_name in vars(self):
-            vals = getattr(self, attr_name)
-            if not vals:
-                continue
-
-            oid = Subject.model_fields[attr_name].alias
-            for val in vals:
-                name_list.append(
-                    x509.NameAttribute(x509.ObjectIdentifier(oid), val)
-                )
-
-        return x509.Name(name_list)
+    @classmethod
+    def from_cryptography(cls: Type["Name"], name: x509.Name) -> "Name":
+        """
+        Create a Name instance from a cryptography Name object.
+
+        Args:
+            name: The cryptography Name object.
+
+        Returns:
+            The Name instance.
+        """
+        subject = defaultdict(set)
+        for attribute in name:
+            for att in name.get_attributes_for_oid(attribute.oid):
+                subject[att.oid.dotted_string].add(att.value)
+        subject = dict(subject)
+        subject["_x509_obj"] = name
+        return cls(**subject)
+
+    def _to_cryptography(self) -> x509.Name:
+        name_attributes = []
+        for name, field in self.model_fields.items():
+            object_identifier = ObjectIdentifier(field.alias)
+            field_vals = getattr(self, name)
+            for val in field_vals:
+                name_attr = x509.NameAttribute(object_identifier, val)
+                name_attributes.append(name_attr)
+        return x509.Name(name_attributes)
+
+    def _string_dict(self):
+        ret = defaultdict(list)
+        for a in set(self.model_dump()):
+            for val in getattr(self, a):
+                ret[a.upper()].append(val)
+        return ret
 
-
-def _is_pem_str(check):
-    return _check_str(PEM_REGEX, check)
-
-
-def _check_str(pattern, check):
-    if not isinstance(check, str):
-        return False
-
-    return re.match(pattern, check)
+    def __str__(self):
+        name_list = []
+        for k in sorted(self._string_dict()):
+            v = self._string_dict()[k]
+            name_list.append(f"{k}: {','.join(v)}")
+        return ", ".join(name_list)
+
+    def __eq__(self, other):
+        for key in self.model_dump():
+            val_list = getattr(self, key)
+            if set(val_list) != set(getattr(other, key)):
+                return False
+        return True
```

### Comparing `pki_tools-0.0.9/pyproject.toml` & `pki_tools-1.0.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pki-tools"
-version = "0.0.9"
+version = "1.0.0"
 description = "PKI tools for e.g. checking certificate CRL/OCSP revocation"
 authors = ["Michal Sadowski <misad90@gmail.com>"]
 license = "MIT"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3",
@@ -16,51 +16,56 @@
 repository = "https://github.com/fulder/pki-tools"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/fulder/pki-tools/issues"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-cryptography = ">=39.0.1,<42.0.0"
-requests = "^2.28.2"
+cryptography = ">=39.0.1,<43.0.0"
 loguru = "^0.7.2"
-pydantic = "^2.3.0"
+pydantic = "^2.7.0"
+httpx = "^0.27.0"
+pyyaml = "^6.0.1"
+pytz = "^2024.1"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
-pytest = "^7.2.1"
-pytest-mock = "^3.10.0"
-pytest-cov = "^4.0.0"
+pytest = "^8.1.1"
+pytest-mock = "^3.14.0"
+pytest-xdist = "^3.5.0"
+pytest-cov = "^5.0.0"
+smokeshow = "^0.4.0"
 
 [tool.poetry.group.lint]
 optional = true
 
 [tool.poetry.group.lint.dependencies]
-black = "^23.1.0"
-ruff = "^0.0.289"
-
+ruff = ">=0.0.289,<0.3.8"
 
 [tool.poetry.group.dev.dependencies]
-mkdocs-material = "^9.3.1"
-handsdown = "^2.0.1"
+mkdocstrings = {extras = ["python"], version = "^0.24.3"}
+pymdown-extensions = "^10.7.1"
+
+[tool.poetry.group.apitest.dependencies]
+httpx = "^0.27.0"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
-[tool.isort]
-profile = "black"
-
-[tool.black]
-line_length = 79
-
 [tool.pytest.ini_options]
-addopts = "--cov=pki_tools --cov-report term-missing --cov-report=html -v"
+addopts = "--cov=pki_tools --cov-report term-missing --cov-report=html -v -n auto"
+
+[tool.ruff]
+line-length = 79
 
 [tool.ruff.per-file-ignores]
-"__init__.py" = ["F401"]
+"./pki_tools/__init__.py" = ["F401"]
+"./pki_tools/types/__init__.py" = ["F401"]
+"./pki_tools/funcs/__init__.py" = ["F401"]
+"./docs/examples/src/*" = ["E402"]
```

