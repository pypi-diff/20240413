# Comparing `tmp/pydantic_settings_vault-2.0.0.tar.gz` & `tmp/pydantic_settings_vault-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_settings_vault-2.0.0.tar", max compression
+gzip compressed data, was "pydantic_settings_vault-2.1.0.tar", max compression
```

## Comparing `pydantic_settings_vault-2.0.0.tar` & `pydantic_settings_vault-2.1.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1070 2023-11-19 14:25:24.921538 pydantic_settings_vault-2.0.0/LICENSE
--rw-r--r--   0        0        0    27276 2023-11-19 14:25:24.921538 pydantic_settings_vault-2.0.0/README.md
--rw-r--r--   0        0        0     1585 2023-11-19 14:25:24.921538 pydantic_settings_vault-2.0.0/pyproject.toml
--rw-r--r--   0        0        0      150 2023-11-19 14:25:24.921538 pydantic_settings_vault-2.0.0/src/pydantic_vault/__init__.py
--rw-r--r--   0        0        0      536 2023-11-19 14:25:24.921538 pydantic_settings_vault-2.0.0/src/pydantic_vault/entities.py
--rw-r--r--   0        0        0        0 2023-11-19 14:25:24.921538 pydantic_settings_vault-2.0.0/src/pydantic_vault/py.typed
--rw-r--r--   0        0        0    14406 2023-11-19 14:25:24.921538 pydantic_settings_vault-2.0.0/src/pydantic_vault/vault_settings.py
--rw-r--r--   0        0        0    28978 1970-01-01 00:00:00.000000 pydantic_settings_vault-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-13 11:07:58.525452 pydantic_settings_vault-2.1.0/LICENSE
+-rw-r--r--   0        0        0    31857 2024-04-13 11:07:58.525452 pydantic_settings_vault-2.1.0/README.md
+-rw-r--r--   0        0        0     1591 2024-04-13 11:07:58.525452 pydantic_settings_vault-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0      150 2024-04-13 11:07:58.525452 pydantic_settings_vault-2.1.0/src/pydantic_vault/__init__.py
+-rw-r--r--   0        0        0      615 2024-04-13 11:07:58.525452 pydantic_settings_vault-2.1.0/src/pydantic_vault/entities.py
+-rw-r--r--   0        0        0        0 2024-04-13 11:07:58.525452 pydantic_settings_vault-2.1.0/src/pydantic_vault/py.typed
+-rw-r--r--   0        0        0    17288 2024-04-13 11:07:58.525452 pydantic_settings_vault-2.1.0/src/pydantic_vault/vault_settings.py
+-rw-r--r--   0        0        0    33559 1970-01-01 00:00:00.000000 pydantic_settings_vault-2.1.0/PKG-INFO
```

### Comparing `pydantic_settings_vault-2.0.0/LICENSE` & `pydantic_settings_vault-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_settings_vault-2.0.0/README.md` & `pydantic_settings_vault-2.1.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -19,25 +19,28 @@
 - [Documentation](#documentation)
   * [`Field` additional parameters](#field-additional-parameters)
   * [Configuration](#configuration)
   * [Authentication](#authentication)
     + [Approle](#approle)
     + [Kubernetes](#kubernetes)
     + [Vault token](#vault-token)
+    + [JWT/OIDC](#jwtoidc)
   * [Order of priority](#order-of-priority)
 - [Logging](#logging)
 - [Examples](#examples)
   * [Retrieve a secret from a KV v2 secret engine](#retrieve-a-secret-from-a-kv-v2-secret-engine)
   * [Retrieve a whole secret at once](#retrieve-a-whole-secret-at-once)
   * [Retrieve a secret from a KV v1 secret engine](#retrieve-a-secret-from-a-kv-v1-secret-engine)
   * [Retrieve a secret from a database secret engine](#retrieve-a-secret-from-a-database-secret-engine)
   * [Use a dynamic path to retrieve secrets](#use-a-dynamic-path-to-retrieve-secrets)
 - [Known limitations](#known-limitations)
 - [Inspirations](#inspirations)
 - [License](#license)
+- [Development](#development)
+  * [Debugging with a real Vault server](#debugging-with-a-real-vault-server)
 
 <!-- tocstop -->
 
 ## Installation
 
 ```shell
 pip install pydantic-settings-vault
@@ -48,15 +51,15 @@
 ```
 
 ## Getting started
 
 With `pydantic_settings.BaseSettings` class, you can easily "create a clearly-defined, type-hinted
 application configuration class" that gets its configuration from environment variables. It will work the same when 
 developing locally (where you probably login with the Vault CLI and your own user account) and when deploying in 
-production (using a Vault Approle or Kubernetes authentication for example).
+production (using a Vault Approle, Kubernetes or JWT/OIDC authentication for example).
 
 You can create a normal `BaseSettings` class, and define the `settings_customise_sources()` method to load secrets from your Vault instance using the `VaultSettingsSource` class:
 
 ```python
 import os
 
 from pydantic import Field, SecretStr
@@ -64,20 +67,26 @@
 from pydantic_vault import VaultSettingsSource
 
 
 class Settings(BaseSettings):
     # The `vault_secret_path` is the full path (with mount point included) to the secret
     # The `vault_secret_key` is the specific key to extract from a secret
     username: str = Field(
-        ..., vault_secret_path="secret/data/path/to/secret", vault_secret_key="my_user"
+        ...,
+        json_schema_extra={
+            "vault_secret_path": "secret/data/path/to/secret",
+            "vault_secret_key": "my_user",
+        },
     )
     password: SecretStr = Field(
         ...,
-        vault_secret_path="secret/data/path/to/secret",
-        vault_secret_key="my_password",
+        json_schema_extra={
+            "vault_secret_path": "secret/data/path/to/secret",
+            "vault_secret_key": "my_password",
+        },
     )
 
     model_config = {
         "vault_url": "https://vault.tld",
         "vault_token": os.environ["VAULT_TOKEN"],
         "vault_namespace": "your/namespace",  # Optional, pydantic-settings-vault supports Vault namespaces (for Vault Enterprise)
     }
@@ -130,40 +139,46 @@
 | `vault_secret_path`         | **Yes**  | The path to your secret in Vault<br>This needs to be the *full path* to the secret, including its mount point (see [examples](#examples) below) |
 | `vault_secret_key`          | No       | The key to use in the secret<br>If it is not specified the whole secret content will be loaded as a dict (see [examples](#examples) below)      |
 
 For example, if you create a secret `database/prod` with a key `password` and a value of `a secret password` in a KV v2 secret engine mounted at the default `secret/` location, you would access it with
 
 ```python
 password: SecretStr = Field(
-    ..., vault_secret_path="secret/data/database/prod", vault_secret_key="password"
+    ...,
+    json_schema_extra={
+        "vault_secret_path": "secret/data/database/prod",
+        "vault_secret_key": "password",
+    },
 )
 ```
 
 ### Configuration
 
 You can configure the behaviour of pydantic-settings-vault in your `Settings.model_config` dict, or using environment variables:
 
-| Settings name                  | Type                  | Required | Environment variable     | Description                                                                                                                      |
-|--------------------------------|-----------------------|----------|--------------------------|----------------------------------------------------------------------------------------------------------------------------------|
-| `settings_customise_sources()` |                       | **Yes**  | N/A                      | You need to implement this function to use Vault as a settings source, and choose the priority order you want                    |
-| `vault_url`                    | `str`                 | **Yes**  | `VAULT_ADDR`             | Your Vault URL                                                                                                                   |
-| `vault_namespace`              | `str \| None`         | No       | `VAULT_NAMESPACE`        | Your Vault namespace (if you use one, requires Vault Enterprise)                                                                 |
-| `vault_auth_mount_point`       | `str \| None`         | No       | `VAULT_AUTH_MOUNT_POINT` | The mount point of the authentication method, if different from its default mount point                                          |
-| `vault_certificate_verify`     | `str \| bool \| None` | No       | `VAULT_CA_BUNDLE`        | The path to a CA bundle validating your Vault certificate, or `False` to disable verification (see [hvac docs][hvac-private-ca]) |
+| Settings name                   | Type                  | Required | Environment variable     | Description                                                                                                                                            |
+|---------------------------------|-----------------------|----------|--------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------|
+| `settings_customise_sources()`  |                       | **Yes**  | N/A                      | You need to implement this function to use Vault as a settings source, and choose the priority order you want                                          |
+| `vault_url`                     | `str`                 | **Yes**  | `VAULT_ADDR`             | Your Vault URL                                                                                                                                         |
+| `vault_namespace`               | `str \| None`         | No       | `VAULT_NAMESPACE`        | Your Vault namespace (if you use one, requires Vault Enterprise)                                                                                       |
+| `vault_auth_path`               | `str \| None`         | No       | `VAULT_AUTH_PATH`        | The path of the authentication method, such as /auth/{path}/login, if different from its default, is only supported by the JWT authentication method.  |
+| `vault_auth_mount_point`        | `str \| None`         | No       | `VAULT_AUTH_MOUNT_POINT` | The mount point of the authentication method, if different from its default mount point                                                                |
+| `vault_certificate_verify`      | `str \| bool \| None` | No       | `VAULT_CA_BUNDLE`        | The path to a CA bundle validating your Vault certificate, or `False` to disable verification (see [hvac docs][hvac-private-ca])                       |
 
 Environment variables override what has been defined in the `Config` class.
 
 You can also configure everything available in the original Pydantic `BaseSettings` class.
 
 ### Authentication
 
 pydantic-settings-vault supports the following authentication method (in descending order of priority):
   - [direct token authentication][vault-auth-token]
   - [kubernetes][vault-auth-kubernetes]
   - [approle][vault-auth-approle]
+  - [jwt/oidc][vault-auth-jwt-oidc]
 
 pydantic-settings-vault tries to be transparent and help you work, both during local development and in production. It will try to
 find the required information for the first authentication method, if it can't it goes on to the next method, until it
 has exhausted all authentication methods. In this case it gives up and logs the failure.
 
 You only need to know this order of priority if you specify the authentication parameters for multiple methods.
 
@@ -184,18 +199,26 @@
 from pydantic import Field, SecretStr
 from pydantic_settings import BaseSettings, PydanticBaseSettingsSource
 from pydantic_vault import VaultSettingsSource
 
 
 class Settings(BaseSettings):
     username: str = Field(
-        ..., vault_secret_path="path/to/secret", vault_secret_key="my_user"
+        ...,
+        json_schema_extra={
+            "vault_secret_path": "path/to/secret",
+            "vault_secret_key": "my_user",
+        },
     )
     password: SecretStr = Field(
-        ..., vault_secret_path="path/to/secret", vault_secret_key="my_password"
+        ...,
+        json_schema_extra={
+            "vault_secret_path": "path/to/secret",
+            "vault_secret_key": "my_password",
+        },
     )
 
     model_config = {
         "vault_url": "https://vault.tld",
         "vault_role_id": "my-role-id",
         "vault_secret_id": SecretStr("my-secret-id"),
     }
@@ -233,18 +256,26 @@
 from pydantic import Field, SecretStr
 from pydantic_settings import BaseSettings, PydanticBaseSettingsSource
 from pydantic_vault import VaultSettingsSource
 
 
 class Settings(BaseSettings):
     username: str = Field(
-        ..., vault_secret_path="path/to/secret", vault_secret_key="my_user"
+        ...,
+        json_schema_extra={
+            "vault_secret_path": "path/to/secret",
+            "vault_secret_key": "my_user",
+        },
     )
     password: SecretStr = Field(
-        ..., vault_secret_path="path/to/secret", vault_secret_key="my_password"
+        ...,
+        json_schema_extra={
+            "vault_secret_path": "path/to/secret",
+            "vault_secret_key": "my_password",
+        },
     )
 
     model_config = {
         "vault_url": "https://vault.tld",
         "vault_kubernetes_role": "my-role",
     }
 
@@ -280,18 +311,26 @@
 from pydantic import Field, SecretStr
 from pydantic_settings import BaseSettings, PydanticBaseSettingsSource
 from pydantic_vault import VaultSettingsSource
 
 
 class Settings(BaseSettings):
     username: str = Field(
-        ..., vault_secret_path="path/to/secret", vault_secret_key="my_user"
+        ...,
+        json_schema_extra={
+            "vault_secret_path": "path/to/secret",
+            "vault_secret_key": "my_user",
+        },
     )
     password: SecretStr = Field(
-        ..., vault_secret_path="path/to/secret", vault_secret_key="my_password"
+        ...,
+        json_schema_extra={
+            "vault_secret_path": "path/to/secret",
+            "vault_secret_key": "my_password",
+        },
     )
 
     model_config = {
         "vault_url": "https://vault.tld",
         "vault_token": SecretStr("my-secret-token"),
     }
 
@@ -309,14 +348,75 @@
             env_settings,
             dotenv_settings,
             VaultSettingsSource(settings_cls),
             file_secret_settings,
         )
 ```
 
+#### JWT/OIDC
+
+To authenticate using the [JWT/OIDC method][vault-auth-jwt-oidc], you need to pass 
+a token role and a token itself to your Settings class.
+
+pydantic-settings-vault reads this information from the following sources (in descending order of priority):
+
+- the `VAULT_JWT_ROLE` and `VAULT_JWT_TOKEN` environment variables
+- the `vault_jwt_role` and `vault_jwt_token` configuration fields in your 
+  `Settings.model_config` class (`vault_jwt_token` can be a `str` or a `SecretStr`)
+
+You can also mix and match, for example, write the role in your `Settings.model_config` 
+class and retrieve the token from the environment at runtime.
+
+Example:
+```python
+from pydantic import Field, SecretStr
+from pydantic_settings import BaseSettings, PydanticBaseSettingsSource
+from pydantic_vault import VaultSettingsSource
+
+
+class Settings(BaseSettings):
+    username: str = Field(
+        ...,
+        json_schema_extra={
+            "vault_secret_path": "path/to/secret",
+            "vault_secret_key": "my_user",
+        },
+    )
+    password: SecretStr = Field(
+        ...,
+        json_schema_extra={
+            "vault_secret_path": "path/to/secret",
+            "vault_secret_key": "my_password",
+        },
+    )
+
+    model_config = {
+        "vault_url": "https://vault.tld",
+        "vault_jwt_role": "my-role",
+        "vault_jwt_token": SecretStr("my-token"),
+    }
+
+    @classmethod
+    def settings_customise_sources(
+        cls,
+        settings_cls: type[BaseSettings],
+        init_settings: PydanticBaseSettingsSource,
+        env_settings: PydanticBaseSettingsSource,
+        dotenv_settings: PydanticBaseSettingsSource,
+        file_secret_settings: PydanticBaseSettingsSource,
+    ) -> tuple[PydanticBaseSettingsSource, ...]:
+        return (
+            init_settings,
+            env_settings,
+            dotenv_settings,
+            VaultSettingsSource(settings_cls),
+            file_secret_settings,
+        )
+```
+
 ### Order of priority
 
 You can customize settings sources and choose the order of priority you want.
 
 Here are some examples:
 ```python
 from pydantic_settings import BaseSettings, PydanticBaseSettingsSource
@@ -401,15 +501,19 @@
 from pydantic_vault import VaultSettingsSource
 
 
 class Settings(BaseSettings):
     ###############################################
     # THIS PART CHANGES IN THE DIFFERENT EXAMPLES #
     username: str = Field(
-        ..., vault_secret_path="secret/data/path/to/secret", vault_secret_key="my_user"
+        ...,
+        json_schema_extra={
+            "vault_secret_path": "secret/data/path/to/secret",
+            "vault_secret_key": "my_user",
+        },
     )
     ###############################################
 
     model_config = {"vault_url": "https://vault.tld"}
 
     @classmethod
     def settings_customise_sources(
@@ -444,20 +548,26 @@
 class Settings(BaseSettings):
     # The `vault_secret_path` is the full path (with mount point included) to the secret.
     # For a KV v2 secret engine, there is always a `data/` sub-path between the mount point and
     # the secret actual path, eg. if your mount point is `secret/` (the default) and your secret
     # path is `my-api/prod`, the full path to use is `secret/data/my-api/prod`.
     # The `vault_secret_key` is the specific key to extract from a secret.
     username: str = Field(
-        ..., vault_secret_path="secret/data/my-api/prod", vault_secret_key="root_user"
+        ...,
+        json_schema_extra={
+            "vault_secret_path": "secret/data/my-api/prod",
+            "vault_secret_key": "root_user",
+        },
     )
     password: SecretStr = Field(
         ...,
-        vault_secret_path="secret/data/my-api/prod",
-        vault_secret_key="root_password",
+        json_schema_extra={
+            "vault_secret_path": "secret/data/my-api/prod",
+            "vault_secret_key": "root_password",
+        },
     )
 
 
 settings = Settings()
 
 settings.username  # "root"
 settings.password.get_secret_value()  # "a_v3ry_s3cur3_p4ssw0rd"
@@ -480,15 +590,17 @@
 ```python
 class Settings(BaseSettings):
     # The `vault_secret_path` is the full path (with mount point included) to the secret.
     # For a KV v2 secret engine, there is always a `data/` sub-path between the mount point and
     # the secret actual path, eg. if your mount point is `secret/` (the default) and your secret
     # path is `my-api/prod`, the full path to use is `secret/data/my-api/prod`.
     # We don't pass a `vault_secret_key` here so that pydantic-settings-vault fetches all fields at once.
-    credentials: dict = Field(..., vault_secret_path="secret/data/my-api/prod")
+    credentials: dict = Field(
+        ..., json_schema_extra={"vault_secret_path": "secret/data/my-api/prod"}
+    )
 
 
 settings = Settings()
 settings.credentials  # { "root_user": "root", "root_password": "a_v3ry_s3cur3_p4ssw0rd" }
 ```
 
 You can also use a Pydantic `BaseModel` class to parse and validate the incoming secret:
@@ -500,15 +612,17 @@
 
 class Settings(BaseSettings):
     # The `vault_secret_path` is the full path (with mount point included) to the secret.
     # For a KV v2 secret engine, there is always a `data/` sub-path between the mount point and
     # the secret actual path, eg. if your mount point is `secret/` (the default) and your secret
     # path is `my-api/prod`, the full path to use is `secret/data/my-api/prod`.
     # We don't pass a `vault_secret_key` here so that pydantic-settings-vault fetches all fields at once.
-    credentials: Credentials = Field(..., vault_secret_path="secret/data/my-api/prod")
+    credentials: Credentials = Field(
+        ..., json_schema_extra={"vault_secret_path": "secret/data/my-api/prod"}
+    )
 
 
 settings = Settings()
 settings.credentials.root_user  # "root"
 settings.credentials.root_password.get_secret_value()  # "a_v3ry_s3cur3_p4ssw0rd"
 ```
 
@@ -527,18 +641,26 @@
 class Settings(BaseSettings):
     # The `vault_secret_path` is the full path (with mount point included) to the secret.
     # For a KV v1 secret engine, the secret path is directly appended to the mount point,
     # eg. if your mount point is `kv/` (the default) and your secret path is `my-api/prod`,
     # the full path to use is `kv/my-api/prod` (unlike with KV v2 secret engines).
     # The `vault_secret_key` is the specific key to extract from a secret.
     username: str = Field(
-        ..., vault_secret_path="kv/my-api/prod", vault_secret_key="root_user"
+        ...,
+        json_schema_extra={
+            "vault_secret_path": "kv/my-api/prod",
+            "vault_secret_key": "root_user",
+        },
     )
     password: SecretStr = Field(
-        ..., vault_secret_path="kv/my-api/prod", vault_secret_key="root_password"
+        ...,
+        json_schema_extra={
+            "vault_secret_path": "kv/my-api/prod",
+            "vault_secret_key": "root_password",
+        },
     )
 
 
 settings = Settings()
 
 settings.username  # "root"
 settings.password.get_secret_value()  # "a_v3ry_s3cur3_p4ssw0rd"
@@ -564,16 +686,20 @@
 class Settings(BaseSettings):
     # The `vault_secret_path` is the full path (with mount point included) to the secret.
     # For a database secret engine, the secret path is `<mount point>/creds/<role name>`.
     # For example if your mount point is `database/` (the default) and your role name is
     # `my-db-prod`, the full path to use is `database/creds/my-db-prod`. You will receive
     # `username` and `password` fields in response.
     # You must *not* pass a `vault_secret_key` so that pydantic-settings-vault fetches both fields at once.
-    db_creds: DbCredentials = Field(..., vault_secret_path="database/creds/my-db-prod")
-    db_creds_in_dict: dict = Field(..., vault_secret_path="database/creds/my-db-prod")
+    db_creds: DbCredentials = Field(
+        ..., json_schema_extra={"vault_secret_path": "database/creds/my-db-prod"}
+    )
+    db_creds_in_dict: dict = Field(
+        ..., json_schema_extra={"vault_secret_path": "database/creds/my-db-prod"}
+    )
 
 
 settings = Settings()
 
 settings.db_creds.username  # "generated-username-1"
 settings.db_creds.password.get_secret_value()  # "generated-password-for-username-1"
 settings.db_creds_in_dict["username"]  # "generated-username-2"
@@ -592,18 +718,26 @@
 # default it falls back to "dev"
 ENV = os.getenv("ENV", "dev")
 
 
 class Settings(BaseSettings):
     # This will load different secrets depending on the value of the ENV environment variable
     username: str = Field(
-        ..., vault_secret_path=f"kv/my-api/{ENV}", vault_secret_key="root_user"
+        ...,
+        json_schema_extra={
+            "vault_secret_path": f"kv/my-api/{ENV}",
+            "vault_secret_key": "root_user",
+        },
     )
     password: SecretStr = Field(
-        ..., vault_secret_path=f"kv/my-api/{ENV}", vault_secret_key="root_password"
+        ...,
+        json_schema_extra={
+            "vault_secret_path": f"kv/my-api/{ENV}",
+            "vault_secret_key": "root_password",
+        },
     )
 
 
 settings = Settings()
 
 settings.username  # "root"
 settings.password.get_secret_value()  # "a_v3ry_s3cur3_p4ssw0rd"
@@ -620,15 +754,17 @@
   user            root
   password        a_v3ry_s3cur3_p4ssw0rd
   data            a very important piece of data
   ```
   and the settings class
   ```python
   class Settings(BaseSettings):
-      my_secret: dict = Field(..., vault_secret_path="kv/my-secret")
+      my_secret: dict = Field(
+          ..., json_schema_extra={"vault_secret_path": "kv/my-secret"}
+      )
   ```
   pydantic-settings-vault will try to load only the `data` value (`a very important piece of data`) in
   `my_secret`, which will fail validation from Pydantic because it is not a dict.
 
   **Workaround:** Rename the `data` key in your secret 😅
 
   **Workaround:** Migrate to KV v2
@@ -638,18 +774,40 @@
 - [Ansible `hashi_vault` lookup plugin][ansible hashi_vault] for the API and some code
 - [Hashicorp's Vault GitHub Action][vault-action] for the API
 
 ## License
 
 pydantic-settings-vault is available under the [MIT license](./LICENSE).
 
+## Development
+
+### Debugging with a real Vault server
+
+You can use a real Vault server to debug this project. To make this process
+easier, this project includes a `docker-compose.yml` file that can run a 
+ready-to-use Vault server.
+
+To run the server and set it up, run the following commands:
+
+```shell
+docker-compose up
+make setup-vault
+```
+
+After that, you will have a Vault server running at `http://localhost:8200`, where you can authorize in two ways:
+
+- using the root token (which is `token`)
+- using the JWT method (role=jwt_role, token=[link](./configs/vault/jwt_token.txt))
+- using the AppRole method (the values of role_id and secret_id can be found in the logs of the `make setup-vault` command).
+
 [ansible hashi_vault]: https://docs.ansible.com/ansible/latest/collections/community/hashi_vault/hashi_vault_lookup.html
 [hvac-private-ca]: https://hvac.readthedocs.io/en/stable/advanced_usage.html#making-use-of-private-ca
 [pydantic]: https://docs.pydantic.dev/latest/
 [pydantic-basesettings]: https://docs.pydantic.dev/latest/usage/pydantic_settings/
 [pydantic-basesettings-customsource]: https://docs.pydantic.dev/latest/usage/pydantic_settings/#adding-sources
 [vault]: https://www.vaultproject.io/
 [vault-action]: https://github.com/hashicorp/vault-action
 [vault-auth-approle]: https://www.vaultproject.io/docs/auth/approle
 [vault-auth-kubernetes]: https://www.vaultproject.io/docs/auth/kubernetes
 [vault-auth-token]: https://www.vaultproject.io/docs/auth/token
+[vault-auth-jwt-oidc]: https://developer.hashicorp.com/vault/docs/auth/jwt
 [vault-kv-v2]: https://www.vaultproject.io/docs/secrets/kv/kv-v2/
```

### Comparing `pydantic_settings_vault-2.0.0/pyproject.toml` & `pydantic_settings_vault-2.1.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-settings-vault"
-version = "2.0.0"
+version = "2.1.0"
 description = "A simple extension to pydantic-settings that can retrieve secrets from Hashicorp Vault"
 authors = [
   "Aleksey Petrunnik <petrunnik.a@gmail.com>",
   "Thomas Gaudin <thomas.gaudin@centraliens-lille.org>",
 ]
 license = "MIT"
 readme = "README.md"
@@ -33,19 +33,19 @@
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pydantic = ">=2.1.1, <3"
 pydantic-settings = ">=2.0.2, <3"
 hvac = ">=0.10.6"
 
-[tool.poetry.dev-dependencies]
-mypy = "^1.5.1"
+[tool.poetry.group.dev.dependencies]
+mypy = "^1.9.0"
 pytest = "^7.4.0"
-pytest-mock = "^3.11.1"
-pytest-cov = "^4.1.0"
+pytest-mock = "^3.14.0"
+pytest-cov = "^5.0.0"
 pyfakefs = "^5.2.3"
 pre-commit = "^2.21.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pydantic_settings_vault-2.0.0/src/pydantic_vault/entities.py` & `pydantic_settings_vault-2.1.0/src/pydantic_vault/entities.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,17 +13,23 @@
 class HvacReadSecretParameters(TypedDict, total=False):
     path: str
     mount_point: str
 
 
 class AuthMethodParameters(TypedDict, total=False):
     mount_point: str
+    path: str
 
 
 class Approle(NamedTuple):
     role_id: str
     secret_id: SecretStr
 
 
 class Kubernetes(NamedTuple):
     role: str
     jwt_token: SecretStr
+
+
+class VaultJwt(NamedTuple):
+    role: str
+    token: SecretStr
```

### Comparing `pydantic_settings_vault-2.0.0/src/pydantic_vault/vault_settings.py` & `pydantic_settings_vault-2.1.0/src/pydantic_vault/vault_settings.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from pydantic_settings.sources import SettingsError, _annotation_is_complex
 
 from pydantic_vault.entities import (
     Approle,
     AuthMethodParameters,
     HvacClientParameters,
     Kubernetes,
+    VaultJwt,
 )
 
 logger = logging.getLogger("pydantic-vault")
 logger.addHandler(logging.NullHandler())
 
 
 class PydanticVaultException(BaseException):
@@ -87,15 +88,17 @@
 
     # Certificate verification
     if settings.model_config.get("vault_certificate_verify") is not None:
         _vault_certificate_verify: Union[bool, str] = cast(
             Union[bool, str], settings.model_config.get("vault_certificate_verify")
         )
         hvac_parameters.update({"verify": _vault_certificate_verify})
-        logger.debug(f"Found Vault CA bundle '{_vault_certificate_verify}' in Config")
+        logger.debug(
+            f"Found Vault CA bundle '{_vault_certificate_verify}' in model_config"
+        )
     if "VAULT_CA_BUNDLE" in os.environ:
         _vault_certificate_verify = os.environ["VAULT_CA_BUNDLE"]
         try:
             hvac_parameters.update(
                 {"verify": TypeAdapter(bool).validate_python(_vault_certificate_verify)}
             )
         except ValidationError:
@@ -114,14 +117,24 @@
         )
     if "VAULT_AUTH_MOUNT_POINT" in os.environ:
         _vault_auth_mount_point = os.environ["VAULT_AUTH_MOUNT_POINT"]
         _vault_auth_method_parameters["mount_point"] = _vault_auth_mount_point
         logger.debug(
             f"Found Vault Auth mount point '{_vault_auth_mount_point}' in environment variables"
         )
+    if settings.model_config.get("vault_auth_path") is not None:
+        _vault_auth_path: str = settings.model_config["vault_auth_path"]  # type: ignore
+        _vault_auth_method_parameters["path"] = _vault_auth_path
+        logger.debug(f"Found Vault Auth path '{_vault_auth_path}' in model_config")
+    if "VAULT_AUTH_PATH" in os.environ:
+        _vault_auth_path = os.environ["VAULT_AUTH_PATH"]
+        _vault_auth_method_parameters["path"] = _vault_auth_path
+        logger.debug(
+            f"Found Vault Auth path '{_vault_auth_path}' in environment variables"
+        )
 
     _vault_token = _extract_vault_token(settings)
     if _vault_token is not None:
         hvac_parameters.update({"token": _vault_token.get_secret_value()})
         hvac_client = HvacClient(_vault_url, **hvac_parameters)
         logger.info(
             _format_vault_client_auth_log(_vault_url, "Vault Token", _vault_namespace)
@@ -131,15 +144,15 @@
     hvac_client = HvacClient(_vault_url, **hvac_parameters)
 
     _vault_kubernetes = _extract_kubernetes(settings)
     if _vault_kubernetes is not None:
         hvac_client.auth.kubernetes.login(
             _vault_kubernetes.role,
             _vault_kubernetes.jwt_token.get_secret_value(),
-            **_vault_auth_method_parameters,
+            mount_point=_vault_auth_method_parameters.get("mount_point", "kubernetes"),
         )
         logger.info(
             _format_vault_client_auth_log(
                 _vault_url,
                 "Kubernetes",
                 _vault_namespace,
                 {"kubernetes_role": _vault_kubernetes.role},
@@ -148,26 +161,43 @@
         return hvac_client
 
     _vault_approle = _extract_approle(settings)
     if _vault_approle is not None:
         hvac_client.auth.approle.login(
             role_id=_vault_approle.role_id,
             secret_id=_vault_approle.secret_id.get_secret_value(),
-            **_vault_auth_method_parameters,
+            mount_point=_vault_auth_method_parameters.get("mount_point", "approle"),
         )
         logger.info(
             _format_vault_client_auth_log(
                 _vault_url,
                 "Approle",
                 _vault_namespace,
                 {"role_id": _vault_approle.role_id},
             )
         )
         return hvac_client
 
+    _vault_jwt = _extract_jwt_token(settings)
+    if _vault_jwt is not None:
+        hvac_client.auth.jwt.jwt_login(
+            _vault_jwt.role,
+            _vault_jwt.token.get_secret_value(),
+            path=_vault_auth_method_parameters.get("path"),
+        )
+        logger.info(
+            _format_vault_client_auth_log(
+                _vault_url,
+                "JWT",
+                _vault_namespace,
+                {"role": _vault_jwt.role},
+            )
+        )
+        return hvac_client
+
     # We couldn't find suitable information to authenticate against Vault
     return None
 
 
 def _extract_approle(settings: Type[BaseSettings]) -> Optional[Approle]:
     """Extract Approle information from environment or from BaseSettings.model_config"""
     _vault_role_id: Optional[str] = None
@@ -246,14 +276,49 @@
 
         if kubernetes_role is not None:
             return Kubernetes(role=kubernetes_role, jwt_token=_kubernetes_jwt)
 
     return None
 
 
+def _extract_jwt_token(settings: Type[BaseSettings]) -> Optional[VaultJwt]:
+    """
+    Extract jwt auth params from environment or from BaseSettings.model_config
+    """
+    vault_jwt: Optional[VaultJwt] = None
+    _vault_jwt_role: Optional[str] = None
+    _vault_jwt_token: Optional[SecretStr] = None
+
+    # Load from BaseSettings.model_config
+    if settings.model_config.get("vault_jwt_role") is not None:
+        _vault_jwt_role = settings.model_config["vault_jwt_role"]  # type: ignore[typeddict-item]
+        logger.debug(f"Found Vault JWT Role '{_vault_jwt_role}' in model_config")
+    if settings.model_config.get("vault_jwt_token") is not None:
+        if isinstance(settings.model_config["vault_jwt_token"], SecretStr):  # type: ignore[typeddict-item]
+            _vault_jwt_token = settings.model_config["vault_jwt_token"]  # type: ignore[typeddict-item]
+        else:
+            _vault_jwt_token = SecretStr(settings.model_config["vault_jwt_token"])  # type: ignore[typeddict-item]
+        logger.debug("Found Vault JWT Token in model_config")
+
+    # Load (and eventually override) from environment
+    if "VAULT_JWT_ROLE" in os.environ:
+        _vault_jwt_role = os.environ["VAULT_JWT_ROLE"]
+        logger.debug(
+            f"Found Vault JWT Role '{_vault_jwt_role}' in environment variables"
+        )
+    if "VAULT_JWT_TOKEN" in os.environ:
+        _vault_jwt_token = SecretStr(os.environ["VAULT_JWT_TOKEN"])
+        logger.debug("Found Vault JWT Token in environment variables")
+
+    if _vault_jwt_role is not None and _vault_jwt_token is not None:
+        vault_jwt = VaultJwt(role=_vault_jwt_role, token=_vault_jwt_token)
+
+    return vault_jwt
+
+
 class VaultSettingsSource(PydanticBaseSettingsSource):
     def __init__(self, settings_cls: Type[BaseSettings]) -> None:
         super().__init__(settings_cls)
 
     def get_field_value(
         self, field: FieldInfo, field_name: str
     ) -> Tuple[Any, str, bool]:
```

### Comparing `pydantic_settings_vault-2.0.0/PKG-INFO` & `pydantic_settings_vault-2.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-settings-vault
-Version: 2.0.0
+Version: 2.1.0
 Summary: A simple extension to pydantic-settings that can retrieve secrets from Hashicorp Vault
 Home-page: https://github.com/aleksey925/pydantic-settings-vault/
 License: MIT
 Keywords: hashicorp,vault,hvac,pydantic
 Author: Aleksey Petrunnik
 Author-email: petrunnik.a@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -55,25 +55,28 @@
 - [Documentation](#documentation)
   * [`Field` additional parameters](#field-additional-parameters)
   * [Configuration](#configuration)
   * [Authentication](#authentication)
     + [Approle](#approle)
     + [Kubernetes](#kubernetes)
     + [Vault token](#vault-token)
+    + [JWT/OIDC](#jwtoidc)
   * [Order of priority](#order-of-priority)
 - [Logging](#logging)
 - [Examples](#examples)
   * [Retrieve a secret from a KV v2 secret engine](#retrieve-a-secret-from-a-kv-v2-secret-engine)
   * [Retrieve a whole secret at once](#retrieve-a-whole-secret-at-once)
   * [Retrieve a secret from a KV v1 secret engine](#retrieve-a-secret-from-a-kv-v1-secret-engine)
   * [Retrieve a secret from a database secret engine](#retrieve-a-secret-from-a-database-secret-engine)
   * [Use a dynamic path to retrieve secrets](#use-a-dynamic-path-to-retrieve-secrets)
 - [Known limitations](#known-limitations)
 - [Inspirations](#inspirations)
 - [License](#license)
+- [Development](#development)
+  * [Debugging with a real Vault server](#debugging-with-a-real-vault-server)
 
 <!-- tocstop -->
 
 ## Installation
 
 ```shell
 pip install pydantic-settings-vault
@@ -84,15 +87,15 @@
 ```
 
 ## Getting started
 
 With `pydantic_settings.BaseSettings` class, you can easily "create a clearly-defined, type-hinted
 application configuration class" that gets its configuration from environment variables. It will work the same when 
 developing locally (where you probably login with the Vault CLI and your own user account) and when deploying in 
-production (using a Vault Approle or Kubernetes authentication for example).
+production (using a Vault Approle, Kubernetes or JWT/OIDC authentication for example).
 
 You can create a normal `BaseSettings` class, and define the `settings_customise_sources()` method to load secrets from your Vault instance using the `VaultSettingsSource` class:
 
 ```python
 import os
 
 from pydantic import Field, SecretStr
@@ -100,20 +103,26 @@
 from pydantic_vault import VaultSettingsSource
 
 
 class Settings(BaseSettings):
     # The `vault_secret_path` is the full path (with mount point included) to the secret
     # The `vault_secret_key` is the specific key to extract from a secret
     username: str = Field(
-        ..., vault_secret_path="secret/data/path/to/secret", vault_secret_key="my_user"
+        ...,
+        json_schema_extra={
+            "vault_secret_path": "secret/data/path/to/secret",
+            "vault_secret_key": "my_user",
+        },
     )
     password: SecretStr = Field(
         ...,
-        vault_secret_path="secret/data/path/to/secret",
-        vault_secret_key="my_password",
+        json_schema_extra={
+            "vault_secret_path": "secret/data/path/to/secret",
+            "vault_secret_key": "my_password",
+        },
     )
 
     model_config = {
         "vault_url": "https://vault.tld",
         "vault_token": os.environ["VAULT_TOKEN"],
         "vault_namespace": "your/namespace",  # Optional, pydantic-settings-vault supports Vault namespaces (for Vault Enterprise)
     }
@@ -166,40 +175,46 @@
 | `vault_secret_path`         | **Yes**  | The path to your secret in Vault<br>This needs to be the *full path* to the secret, including its mount point (see [examples](#examples) below) |
 | `vault_secret_key`          | No       | The key to use in the secret<br>If it is not specified the whole secret content will be loaded as a dict (see [examples](#examples) below)      |
 
 For example, if you create a secret `database/prod` with a key `password` and a value of `a secret password` in a KV v2 secret engine mounted at the default `secret/` location, you would access it with
 
 ```python
 password: SecretStr = Field(
-    ..., vault_secret_path="secret/data/database/prod", vault_secret_key="password"
+    ...,
+    json_schema_extra={
+        "vault_secret_path": "secret/data/database/prod",
+        "vault_secret_key": "password",
+    },
 )
 ```
 
 ### Configuration
 
 You can configure the behaviour of pydantic-settings-vault in your `Settings.model_config` dict, or using environment variables:
 
-| Settings name                  | Type                  | Required | Environment variable     | Description                                                                                                                      |
-|--------------------------------|-----------------------|----------|--------------------------|----------------------------------------------------------------------------------------------------------------------------------|
-| `settings_customise_sources()` |                       | **Yes**  | N/A                      | You need to implement this function to use Vault as a settings source, and choose the priority order you want                    |
-| `vault_url`                    | `str`                 | **Yes**  | `VAULT_ADDR`             | Your Vault URL                                                                                                                   |
-| `vault_namespace`              | `str \| None`         | No       | `VAULT_NAMESPACE`        | Your Vault namespace (if you use one, requires Vault Enterprise)                                                                 |
-| `vault_auth_mount_point`       | `str \| None`         | No       | `VAULT_AUTH_MOUNT_POINT` | The mount point of the authentication method, if different from its default mount point                                          |
-| `vault_certificate_verify`     | `str \| bool \| None` | No       | `VAULT_CA_BUNDLE`        | The path to a CA bundle validating your Vault certificate, or `False` to disable verification (see [hvac docs][hvac-private-ca]) |
+| Settings name                   | Type                  | Required | Environment variable     | Description                                                                                                                                            |
+|---------------------------------|-----------------------|----------|--------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------|
+| `settings_customise_sources()`  |                       | **Yes**  | N/A                      | You need to implement this function to use Vault as a settings source, and choose the priority order you want                                          |
+| `vault_url`                     | `str`                 | **Yes**  | `VAULT_ADDR`             | Your Vault URL                                                                                                                                         |
+| `vault_namespace`               | `str \| None`         | No       | `VAULT_NAMESPACE`        | Your Vault namespace (if you use one, requires Vault Enterprise)                                                                                       |
+| `vault_auth_path`               | `str \| None`         | No       | `VAULT_AUTH_PATH`        | The path of the authentication method, such as /auth/{path}/login, if different from its default, is only supported by the JWT authentication method.  |
+| `vault_auth_mount_point`        | `str \| None`         | No       | `VAULT_AUTH_MOUNT_POINT` | The mount point of the authentication method, if different from its default mount point                                                                |
+| `vault_certificate_verify`      | `str \| bool \| None` | No       | `VAULT_CA_BUNDLE`        | The path to a CA bundle validating your Vault certificate, or `False` to disable verification (see [hvac docs][hvac-private-ca])                       |
 
 Environment variables override what has been defined in the `Config` class.
 
 You can also configure everything available in the original Pydantic `BaseSettings` class.
 
 ### Authentication
 
 pydantic-settings-vault supports the following authentication method (in descending order of priority):
   - [direct token authentication][vault-auth-token]
   - [kubernetes][vault-auth-kubernetes]
   - [approle][vault-auth-approle]
+  - [jwt/oidc][vault-auth-jwt-oidc]
 
 pydantic-settings-vault tries to be transparent and help you work, both during local development and in production. It will try to
 find the required information for the first authentication method, if it can't it goes on to the next method, until it
 has exhausted all authentication methods. In this case it gives up and logs the failure.
 
 You only need to know this order of priority if you specify the authentication parameters for multiple methods.
 
@@ -220,18 +235,26 @@
 from pydantic import Field, SecretStr
 from pydantic_settings import BaseSettings, PydanticBaseSettingsSource
 from pydantic_vault import VaultSettingsSource
 
 
 class Settings(BaseSettings):
     username: str = Field(
-        ..., vault_secret_path="path/to/secret", vault_secret_key="my_user"
+        ...,
+        json_schema_extra={
+            "vault_secret_path": "path/to/secret",
+            "vault_secret_key": "my_user",
+        },
     )
     password: SecretStr = Field(
-        ..., vault_secret_path="path/to/secret", vault_secret_key="my_password"
+        ...,
+        json_schema_extra={
+            "vault_secret_path": "path/to/secret",
+            "vault_secret_key": "my_password",
+        },
     )
 
     model_config = {
         "vault_url": "https://vault.tld",
         "vault_role_id": "my-role-id",
         "vault_secret_id": SecretStr("my-secret-id"),
     }
@@ -269,18 +292,26 @@
 from pydantic import Field, SecretStr
 from pydantic_settings import BaseSettings, PydanticBaseSettingsSource
 from pydantic_vault import VaultSettingsSource
 
 
 class Settings(BaseSettings):
     username: str = Field(
-        ..., vault_secret_path="path/to/secret", vault_secret_key="my_user"
+        ...,
+        json_schema_extra={
+            "vault_secret_path": "path/to/secret",
+            "vault_secret_key": "my_user",
+        },
     )
     password: SecretStr = Field(
-        ..., vault_secret_path="path/to/secret", vault_secret_key="my_password"
+        ...,
+        json_schema_extra={
+            "vault_secret_path": "path/to/secret",
+            "vault_secret_key": "my_password",
+        },
     )
 
     model_config = {
         "vault_url": "https://vault.tld",
         "vault_kubernetes_role": "my-role",
     }
 
@@ -316,18 +347,26 @@
 from pydantic import Field, SecretStr
 from pydantic_settings import BaseSettings, PydanticBaseSettingsSource
 from pydantic_vault import VaultSettingsSource
 
 
 class Settings(BaseSettings):
     username: str = Field(
-        ..., vault_secret_path="path/to/secret", vault_secret_key="my_user"
+        ...,
+        json_schema_extra={
+            "vault_secret_path": "path/to/secret",
+            "vault_secret_key": "my_user",
+        },
     )
     password: SecretStr = Field(
-        ..., vault_secret_path="path/to/secret", vault_secret_key="my_password"
+        ...,
+        json_schema_extra={
+            "vault_secret_path": "path/to/secret",
+            "vault_secret_key": "my_password",
+        },
     )
 
     model_config = {
         "vault_url": "https://vault.tld",
         "vault_token": SecretStr("my-secret-token"),
     }
 
@@ -345,14 +384,75 @@
             env_settings,
             dotenv_settings,
             VaultSettingsSource(settings_cls),
             file_secret_settings,
         )
 ```
 
+#### JWT/OIDC
+
+To authenticate using the [JWT/OIDC method][vault-auth-jwt-oidc], you need to pass 
+a token role and a token itself to your Settings class.
+
+pydantic-settings-vault reads this information from the following sources (in descending order of priority):
+
+- the `VAULT_JWT_ROLE` and `VAULT_JWT_TOKEN` environment variables
+- the `vault_jwt_role` and `vault_jwt_token` configuration fields in your 
+  `Settings.model_config` class (`vault_jwt_token` can be a `str` or a `SecretStr`)
+
+You can also mix and match, for example, write the role in your `Settings.model_config` 
+class and retrieve the token from the environment at runtime.
+
+Example:
+```python
+from pydantic import Field, SecretStr
+from pydantic_settings import BaseSettings, PydanticBaseSettingsSource
+from pydantic_vault import VaultSettingsSource
+
+
+class Settings(BaseSettings):
+    username: str = Field(
+        ...,
+        json_schema_extra={
+            "vault_secret_path": "path/to/secret",
+            "vault_secret_key": "my_user",
+        },
+    )
+    password: SecretStr = Field(
+        ...,
+        json_schema_extra={
+            "vault_secret_path": "path/to/secret",
+            "vault_secret_key": "my_password",
+        },
+    )
+
+    model_config = {
+        "vault_url": "https://vault.tld",
+        "vault_jwt_role": "my-role",
+        "vault_jwt_token": SecretStr("my-token"),
+    }
+
+    @classmethod
+    def settings_customise_sources(
+        cls,
+        settings_cls: type[BaseSettings],
+        init_settings: PydanticBaseSettingsSource,
+        env_settings: PydanticBaseSettingsSource,
+        dotenv_settings: PydanticBaseSettingsSource,
+        file_secret_settings: PydanticBaseSettingsSource,
+    ) -> tuple[PydanticBaseSettingsSource, ...]:
+        return (
+            init_settings,
+            env_settings,
+            dotenv_settings,
+            VaultSettingsSource(settings_cls),
+            file_secret_settings,
+        )
+```
+
 ### Order of priority
 
 You can customize settings sources and choose the order of priority you want.
 
 Here are some examples:
 ```python
 from pydantic_settings import BaseSettings, PydanticBaseSettingsSource
@@ -437,15 +537,19 @@
 from pydantic_vault import VaultSettingsSource
 
 
 class Settings(BaseSettings):
     ###############################################
     # THIS PART CHANGES IN THE DIFFERENT EXAMPLES #
     username: str = Field(
-        ..., vault_secret_path="secret/data/path/to/secret", vault_secret_key="my_user"
+        ...,
+        json_schema_extra={
+            "vault_secret_path": "secret/data/path/to/secret",
+            "vault_secret_key": "my_user",
+        },
     )
     ###############################################
 
     model_config = {"vault_url": "https://vault.tld"}
 
     @classmethod
     def settings_customise_sources(
@@ -480,20 +584,26 @@
 class Settings(BaseSettings):
     # The `vault_secret_path` is the full path (with mount point included) to the secret.
     # For a KV v2 secret engine, there is always a `data/` sub-path between the mount point and
     # the secret actual path, eg. if your mount point is `secret/` (the default) and your secret
     # path is `my-api/prod`, the full path to use is `secret/data/my-api/prod`.
     # The `vault_secret_key` is the specific key to extract from a secret.
     username: str = Field(
-        ..., vault_secret_path="secret/data/my-api/prod", vault_secret_key="root_user"
+        ...,
+        json_schema_extra={
+            "vault_secret_path": "secret/data/my-api/prod",
+            "vault_secret_key": "root_user",
+        },
     )
     password: SecretStr = Field(
         ...,
-        vault_secret_path="secret/data/my-api/prod",
-        vault_secret_key="root_password",
+        json_schema_extra={
+            "vault_secret_path": "secret/data/my-api/prod",
+            "vault_secret_key": "root_password",
+        },
     )
 
 
 settings = Settings()
 
 settings.username  # "root"
 settings.password.get_secret_value()  # "a_v3ry_s3cur3_p4ssw0rd"
@@ -516,15 +626,17 @@
 ```python
 class Settings(BaseSettings):
     # The `vault_secret_path` is the full path (with mount point included) to the secret.
     # For a KV v2 secret engine, there is always a `data/` sub-path between the mount point and
     # the secret actual path, eg. if your mount point is `secret/` (the default) and your secret
     # path is `my-api/prod`, the full path to use is `secret/data/my-api/prod`.
     # We don't pass a `vault_secret_key` here so that pydantic-settings-vault fetches all fields at once.
-    credentials: dict = Field(..., vault_secret_path="secret/data/my-api/prod")
+    credentials: dict = Field(
+        ..., json_schema_extra={"vault_secret_path": "secret/data/my-api/prod"}
+    )
 
 
 settings = Settings()
 settings.credentials  # { "root_user": "root", "root_password": "a_v3ry_s3cur3_p4ssw0rd" }
 ```
 
 You can also use a Pydantic `BaseModel` class to parse and validate the incoming secret:
@@ -536,15 +648,17 @@
 
 class Settings(BaseSettings):
     # The `vault_secret_path` is the full path (with mount point included) to the secret.
     # For a KV v2 secret engine, there is always a `data/` sub-path between the mount point and
     # the secret actual path, eg. if your mount point is `secret/` (the default) and your secret
     # path is `my-api/prod`, the full path to use is `secret/data/my-api/prod`.
     # We don't pass a `vault_secret_key` here so that pydantic-settings-vault fetches all fields at once.
-    credentials: Credentials = Field(..., vault_secret_path="secret/data/my-api/prod")
+    credentials: Credentials = Field(
+        ..., json_schema_extra={"vault_secret_path": "secret/data/my-api/prod"}
+    )
 
 
 settings = Settings()
 settings.credentials.root_user  # "root"
 settings.credentials.root_password.get_secret_value()  # "a_v3ry_s3cur3_p4ssw0rd"
 ```
 
@@ -563,18 +677,26 @@
 class Settings(BaseSettings):
     # The `vault_secret_path` is the full path (with mount point included) to the secret.
     # For a KV v1 secret engine, the secret path is directly appended to the mount point,
     # eg. if your mount point is `kv/` (the default) and your secret path is `my-api/prod`,
     # the full path to use is `kv/my-api/prod` (unlike with KV v2 secret engines).
     # The `vault_secret_key` is the specific key to extract from a secret.
     username: str = Field(
-        ..., vault_secret_path="kv/my-api/prod", vault_secret_key="root_user"
+        ...,
+        json_schema_extra={
+            "vault_secret_path": "kv/my-api/prod",
+            "vault_secret_key": "root_user",
+        },
     )
     password: SecretStr = Field(
-        ..., vault_secret_path="kv/my-api/prod", vault_secret_key="root_password"
+        ...,
+        json_schema_extra={
+            "vault_secret_path": "kv/my-api/prod",
+            "vault_secret_key": "root_password",
+        },
     )
 
 
 settings = Settings()
 
 settings.username  # "root"
 settings.password.get_secret_value()  # "a_v3ry_s3cur3_p4ssw0rd"
@@ -600,16 +722,20 @@
 class Settings(BaseSettings):
     # The `vault_secret_path` is the full path (with mount point included) to the secret.
     # For a database secret engine, the secret path is `<mount point>/creds/<role name>`.
     # For example if your mount point is `database/` (the default) and your role name is
     # `my-db-prod`, the full path to use is `database/creds/my-db-prod`. You will receive
     # `username` and `password` fields in response.
     # You must *not* pass a `vault_secret_key` so that pydantic-settings-vault fetches both fields at once.
-    db_creds: DbCredentials = Field(..., vault_secret_path="database/creds/my-db-prod")
-    db_creds_in_dict: dict = Field(..., vault_secret_path="database/creds/my-db-prod")
+    db_creds: DbCredentials = Field(
+        ..., json_schema_extra={"vault_secret_path": "database/creds/my-db-prod"}
+    )
+    db_creds_in_dict: dict = Field(
+        ..., json_schema_extra={"vault_secret_path": "database/creds/my-db-prod"}
+    )
 
 
 settings = Settings()
 
 settings.db_creds.username  # "generated-username-1"
 settings.db_creds.password.get_secret_value()  # "generated-password-for-username-1"
 settings.db_creds_in_dict["username"]  # "generated-username-2"
@@ -628,18 +754,26 @@
 # default it falls back to "dev"
 ENV = os.getenv("ENV", "dev")
 
 
 class Settings(BaseSettings):
     # This will load different secrets depending on the value of the ENV environment variable
     username: str = Field(
-        ..., vault_secret_path=f"kv/my-api/{ENV}", vault_secret_key="root_user"
+        ...,
+        json_schema_extra={
+            "vault_secret_path": f"kv/my-api/{ENV}",
+            "vault_secret_key": "root_user",
+        },
     )
     password: SecretStr = Field(
-        ..., vault_secret_path=f"kv/my-api/{ENV}", vault_secret_key="root_password"
+        ...,
+        json_schema_extra={
+            "vault_secret_path": f"kv/my-api/{ENV}",
+            "vault_secret_key": "root_password",
+        },
     )
 
 
 settings = Settings()
 
 settings.username  # "root"
 settings.password.get_secret_value()  # "a_v3ry_s3cur3_p4ssw0rd"
@@ -656,15 +790,17 @@
   user            root
   password        a_v3ry_s3cur3_p4ssw0rd
   data            a very important piece of data
   ```
   and the settings class
   ```python
   class Settings(BaseSettings):
-      my_secret: dict = Field(..., vault_secret_path="kv/my-secret")
+      my_secret: dict = Field(
+          ..., json_schema_extra={"vault_secret_path": "kv/my-secret"}
+      )
   ```
   pydantic-settings-vault will try to load only the `data` value (`a very important piece of data`) in
   `my_secret`, which will fail validation from Pydantic because it is not a dict.
 
   **Workaround:** Rename the `data` key in your secret 😅
 
   **Workaround:** Migrate to KV v2
@@ -674,19 +810,41 @@
 - [Ansible `hashi_vault` lookup plugin][ansible hashi_vault] for the API and some code
 - [Hashicorp's Vault GitHub Action][vault-action] for the API
 
 ## License
 
 pydantic-settings-vault is available under the [MIT license](./LICENSE).
 
+## Development
+
+### Debugging with a real Vault server
+
+You can use a real Vault server to debug this project. To make this process
+easier, this project includes a `docker-compose.yml` file that can run a 
+ready-to-use Vault server.
+
+To run the server and set it up, run the following commands:
+
+```shell
+docker-compose up
+make setup-vault
+```
+
+After that, you will have a Vault server running at `http://localhost:8200`, where you can authorize in two ways:
+
+- using the root token (which is `token`)
+- using the JWT method (role=jwt_role, token=[link](./configs/vault/jwt_token.txt))
+- using the AppRole method (the values of role_id and secret_id can be found in the logs of the `make setup-vault` command).
+
 [ansible hashi_vault]: https://docs.ansible.com/ansible/latest/collections/community/hashi_vault/hashi_vault_lookup.html
 [hvac-private-ca]: https://hvac.readthedocs.io/en/stable/advanced_usage.html#making-use-of-private-ca
 [pydantic]: https://docs.pydantic.dev/latest/
 [pydantic-basesettings]: https://docs.pydantic.dev/latest/usage/pydantic_settings/
 [pydantic-basesettings-customsource]: https://docs.pydantic.dev/latest/usage/pydantic_settings/#adding-sources
 [vault]: https://www.vaultproject.io/
 [vault-action]: https://github.com/hashicorp/vault-action
 [vault-auth-approle]: https://www.vaultproject.io/docs/auth/approle
 [vault-auth-kubernetes]: https://www.vaultproject.io/docs/auth/kubernetes
 [vault-auth-token]: https://www.vaultproject.io/docs/auth/token
+[vault-auth-jwt-oidc]: https://developer.hashicorp.com/vault/docs/auth/jwt
 [vault-kv-v2]: https://www.vaultproject.io/docs/secrets/kv/kv-v2/
```

