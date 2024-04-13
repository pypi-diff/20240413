# Comparing `tmp/novelai_python-0.4.7.tar.gz` & `tmp/novelai_python-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "novelai_python-0.4.7.tar", last modified: Mon Apr  8 16:26:06 2024, max compression
+gzip compressed data, was "novelai_python-0.4.8.tar", last modified: Sat Apr 13 16:05:37 2024, max compression
```

## Comparing `novelai_python-0.4.7.tar` & `novelai_python-0.4.8.tar`

### file list

```diff
@@ -1,77 +1,77 @@
--rwxr-xr-x   0        0        0    11357 2024-04-08 16:25:50.010580 novelai_python-0.4.7/LICENSE
--rwxr-xr-x   0        0        0      522 2024-04-08 16:25:50.010580 novelai_python-0.4.7/NOTICE.MD
--rwxr-xr-x   0        0        0     3405 2024-04-08 16:25:50.010580 novelai_python-0.4.7/README.md
--rw-r--r--   0        0        0     1201 2024-04-08 16:26:06.682767 novelai_python-0.4.7/pyproject.toml
--rwxr-xr-x   0        0        0     1239 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/__init__.py
--rwxr-xr-x   0        0        0     1761 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/_exceptions.py
--rwxr-xr-x   0        0        0      410 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/_response/__init__.py
--rwxr-xr-x   0        0        0      127 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/_response/ai/__init__.py
--rw-r--r--   0        0        0      659 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/_response/ai/generate.py
--rwxr-xr-x   0        0        0      828 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/_response/ai/generate_image.py
--rw-r--r--   0        0        0      724 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/_response/ai/generate_stream.py
--rw-r--r--   0        0        0      185 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/_response/ai/generate_voice.py
--rwxr-xr-x   0        0        0      397 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/_response/ai/upscale.py
--rwxr-xr-x   0        0        0      195 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/_response/schema.py
--rwxr-xr-x   0        0        0      128 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/_response/user/__init__.py
--rwxr-xr-x   0        0        0      721 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/_response/user/information.py
--rwxr-xr-x   0        0        0      204 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/_response/user/login.py
--rwxr-xr-x   0        0        0     2359 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/_response/user/subscription.py
--rwxr-xr-x   0        0        0     1548 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/credential/ApiToken.py
--rwxr-xr-x   0        0        0     1628 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/credential/JwtToken.py
--rwxr-xr-x   0        0        0     1701 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/credential/UserAuth.py
--rwxr-xr-x   0        0        0      424 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/credential/__init__.py
--rwxr-xr-x   0        0        0      462 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/credential/_base.py
--rwxr-xr-x   0        0        0      743 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/sdk/__init__.py
--rwxr-xr-x   0        0        0     1082 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/sdk/ai/LICENSE
--rwxr-xr-x   0        0        0      130 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/sdk/ai/__init__.py
--rw-r--r--   0        0        0     9436 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/sdk/ai/generate/__init__.py
--rw-r--r--   0        0        0     1249 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/sdk/ai/generate/_const.py
--rw-r--r--   0        0        0     1819 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/sdk/ai/generate/_enum.py
--rw-r--r--   0        0        0     6467 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/sdk/ai/generate/_preset.py
--rwxr-xr-x   0        0        0    34778 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/sdk/ai/generate_image/__init__.py
--rw-r--r--   0        0        0    52850 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/sdk/ai/generate_image/_const.py
--rwxr-xr-x   0        0        0     3578 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/sdk/ai/generate_image/_enum.py
--rwxr-xr-x   0        0        0     5306 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/sdk/ai/generate_image/suggest_tags.py
--rw-r--r--   0        0        0     7170 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/sdk/ai/generate_stream.py
--rw-r--r--   0        0        0     7379 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/sdk/ai/generate_voice/__init__.py
--rw-r--r--   0        0        0     2008 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/sdk/ai/generate_voice/_enum.py
--rwxr-xr-x   0        0        0     8223 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/sdk/ai/upscale.py
--rwxr-xr-x   0        0        0      945 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/sdk/schema.py
--rwxr-xr-x   0        0        0      130 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/sdk/user/__init__.py
--rwxr-xr-x   0        0        0     4772 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/sdk/user/information.py
--rwxr-xr-x   0        0        0     5285 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/sdk/user/login.py
--rwxr-xr-x   0        0        0     5045 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/sdk/user/subscription.py
--rwxr-xr-x   0        0        0     7524 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/server.py
--rw-r--r--   0        0        0      534 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/tokenizer/NOTICE.MD
--rw-r--r--   0        0        0     8173 2024-04-08 16:25:50.030580 novelai_python-0.4.7/src/novelai_python/tokenizer/__init__.py
--rw-r--r--   0        0        0  1356917 2024-04-08 16:25:50.034581 novelai_python-0.4.7/src/novelai_python/tokenizer/bpe_simple_vocab_16e6.txt.gz
--rw-r--r--   0        0        0  1494140 2024-04-08 16:25:50.042580 novelai_python-0.4.7/src/novelai_python/tokenizer/gpt2-genji_tokenizer.json
--rw-r--r--   0        0        0  1355257 2024-04-08 16:25:50.050581 novelai_python-0.4.7/src/novelai_python/tokenizer/gpt2_tokenizer.json
--rw-r--r--   0        0        0  1033724 2024-04-08 16:25:50.054581 novelai_python-0.4.7/src/novelai_python/tokenizer/nerdstash_v1.model
--rw-r--r--   0        0        0  1033744 2024-04-08 16:25:50.058581 novelai_python-0.4.7/src/novelai_python/tokenizer/nerdstash_v2.model
--rw-r--r--   0        0        0  1033724 2024-04-08 16:25:50.058581 novelai_python-0.4.7/src/novelai_python/tokenizer/novelai.model
--rw-r--r--   0        0        0  1033744 2024-04-08 16:25:50.062581 novelai_python-0.4.7/src/novelai_python/tokenizer/novelai_v2.model
--rw-r--r--   0        0        0  1357239 2024-04-08 16:25:50.066581 novelai_python-0.4.7/src/novelai_python/tokenizer/pile_tokenizer.json
--rw-r--r--   0        0        0     4854 2024-04-08 16:25:50.066581 novelai_python-0.4.7/src/novelai_python/tokenizer/simple_tokenizer.py
--rw-r--r--   0        0        0       24 2024-04-08 16:25:50.066581 novelai_python-0.4.7/src/novelai_python/tool/__init__.py
--rw-r--r--   0        0        0     7948 2024-04-08 16:25:50.066581 novelai_python-0.4.7/src/novelai_python/tool/image_metadata/__init__.py
--rw-r--r--   0        0        0     3316 2024-04-08 16:25:50.066581 novelai_python-0.4.7/src/novelai_python/tool/image_metadata/lsb_extractor.py
--rw-r--r--   0        0        0     2211 2024-04-08 16:25:50.066581 novelai_python-0.4.7/src/novelai_python/tool/image_metadata/lsb_injector.py
--rw-r--r--   0        0        0     3181 2024-04-08 16:25:50.066581 novelai_python-0.4.7/src/novelai_python/tool/paint_mask/__init__.py
--rw-r--r--   0        0        0    17162 2024-04-08 16:25:50.070581 novelai_python-0.4.7/src/novelai_python/tool/random_prompt/__init__.py
--rw-r--r--   0        0        0    84988 2024-04-08 16:25:50.070581 novelai_python-0.4.7/src/novelai_python/tool/random_prompt/tag.py
--rw-r--r--   0        0        0    21015 2024-04-08 16:25:50.070581 novelai_python-0.4.7/src/novelai_python/tool/random_prompt/tag_character.py
--rw-r--r--   0        0        0    15814 2024-04-08 16:25:50.070581 novelai_python-0.4.7/src/novelai_python/tool/random_prompt/tag_nsfw.py
--rwxr-xr-x   0        0        0      525 2024-04-08 16:25:50.070581 novelai_python-0.4.7/src/novelai_python/utils/__init__.py
--rwxr-xr-x   0        0        0     2419 2024-04-08 16:25:50.070581 novelai_python-0.4.7/src/novelai_python/utils/encode.py
--rwxr-xr-x   0        0        0     1243 2024-04-08 16:25:50.070581 novelai_python-0.4.7/src/novelai_python/utils/useful.py
--rwxr-xr-x   0        0        0        0 2024-04-08 16:25:50.070581 novelai_python-0.4.7/tests/__init__.py
--rw-r--r--   0        0        0      870 2024-04-08 16:25:50.070581 novelai_python-0.4.7/tests/test_generate_voice.py
--rwxr-xr-x   0        0        0     2273 2024-04-08 16:25:50.070581 novelai_python-0.4.7/tests/test_random_prompt.py
--rwxr-xr-x   0        0        0      422 2024-04-08 16:25:50.070581 novelai_python-0.4.7/tests/test_server.py
--rwxr-xr-x   0        0        0     1375 2024-04-08 16:25:50.070581 novelai_python-0.4.7/tests/test_server_run.py
--rwxr-xr-x   0        0        0     2772 2024-04-08 16:25:50.070581 novelai_python-0.4.7/tests/test_upscale.py
--rwxr-xr-x   0        0        0     2592 2024-04-08 16:25:50.070581 novelai_python-0.4.7/tests/test_user_information.py
--rwxr-xr-x   0        0        0     3244 2024-04-08 16:25:50.070581 novelai_python-0.4.7/tests/test_user_login.py
--rwxr-xr-x   0        0        0     3270 2024-04-08 16:25:50.070581 novelai_python-0.4.7/tests/test_user_subscription.py
--rw-r--r--   0        0        0     4578 1970-01-01 00:00:00.000000 novelai_python-0.4.7/PKG-INFO
+-rwxr-xr-x   0        0        0    11357 2024-04-13 16:05:24.422073 novelai_python-0.4.8/LICENSE
+-rwxr-xr-x   0        0        0      522 2024-04-13 16:05:24.422073 novelai_python-0.4.8/NOTICE.MD
+-rwxr-xr-x   0        0        0     3490 2024-04-13 16:05:24.422073 novelai_python-0.4.8/README.md
+-rw-r--r--   0        0        0     1201 2024-04-13 16:05:37.270084 novelai_python-0.4.8/pyproject.toml
+-rwxr-xr-x   0        0        0     1239 2024-04-13 16:05:24.438073 novelai_python-0.4.8/src/novelai_python/__init__.py
+-rwxr-xr-x   0        0        0     1761 2024-04-13 16:05:24.438073 novelai_python-0.4.8/src/novelai_python/_exceptions.py
+-rwxr-xr-x   0        0        0      410 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/_response/__init__.py
+-rwxr-xr-x   0        0        0      127 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/_response/ai/__init__.py
+-rw-r--r--   0        0        0      659 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/_response/ai/generate.py
+-rwxr-xr-x   0        0        0      828 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/_response/ai/generate_image.py
+-rw-r--r--   0        0        0      724 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/_response/ai/generate_stream.py
+-rw-r--r--   0        0        0      185 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/_response/ai/generate_voice.py
+-rwxr-xr-x   0        0        0      397 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/_response/ai/upscale.py
+-rwxr-xr-x   0        0        0      195 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/_response/schema.py
+-rwxr-xr-x   0        0        0      128 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/_response/user/__init__.py
+-rwxr-xr-x   0        0        0      721 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/_response/user/information.py
+-rwxr-xr-x   0        0        0      204 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/_response/user/login.py
+-rwxr-xr-x   0        0        0     2359 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/_response/user/subscription.py
+-rwxr-xr-x   0        0        0     1548 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/credential/ApiToken.py
+-rwxr-xr-x   0        0        0     1628 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/credential/JwtToken.py
+-rwxr-xr-x   0        0        0     1701 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/credential/UserAuth.py
+-rwxr-xr-x   0        0        0      424 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/credential/__init__.py
+-rwxr-xr-x   0        0        0      462 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/credential/_base.py
+-rwxr-xr-x   0        0        0      743 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/sdk/__init__.py
+-rwxr-xr-x   0        0        0     1082 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/sdk/ai/LICENSE
+-rwxr-xr-x   0        0        0      130 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/sdk/ai/__init__.py
+-rw-r--r--   0        0        0     9477 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/sdk/ai/generate/__init__.py
+-rw-r--r--   0        0        0     1249 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/sdk/ai/generate/_const.py
+-rw-r--r--   0        0        0     1827 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/sdk/ai/generate/_enum.py
+-rw-r--r--   0        0        0     6467 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/sdk/ai/generate/_preset.py
+-rwxr-xr-x   0        0        0    34778 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/sdk/ai/generate_image/__init__.py
+-rw-r--r--   0        0        0    52850 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/sdk/ai/generate_image/_const.py
+-rwxr-xr-x   0        0        0     3578 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/sdk/ai/generate_image/_enum.py
+-rwxr-xr-x   0        0        0     5306 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/sdk/ai/generate_image/suggest_tags.py
+-rw-r--r--   0        0        0     7170 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/sdk/ai/generate_stream.py
+-rw-r--r--   0        0        0     7379 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/sdk/ai/generate_voice/__init__.py
+-rw-r--r--   0        0        0     2008 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/sdk/ai/generate_voice/_enum.py
+-rwxr-xr-x   0        0        0     8223 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/sdk/ai/upscale.py
+-rwxr-xr-x   0        0        0      945 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/sdk/schema.py
+-rwxr-xr-x   0        0        0      130 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/sdk/user/__init__.py
+-rwxr-xr-x   0        0        0     4772 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/sdk/user/information.py
+-rwxr-xr-x   0        0        0     5285 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/sdk/user/login.py
+-rwxr-xr-x   0        0        0     5045 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/sdk/user/subscription.py
+-rwxr-xr-x   0        0        0     7466 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/server.py
+-rw-r--r--   0        0        0      534 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/tokenizer/NOTICE.MD
+-rw-r--r--   0        0        0     8173 2024-04-13 16:05:24.442073 novelai_python-0.4.8/src/novelai_python/tokenizer/__init__.py
+-rw-r--r--   0        0        0  1356917 2024-04-13 16:05:24.446073 novelai_python-0.4.8/src/novelai_python/tokenizer/bpe_simple_vocab_16e6.txt.gz
+-rw-r--r--   0        0        0  1494140 2024-04-13 16:05:24.454074 novelai_python-0.4.8/src/novelai_python/tokenizer/gpt2-genji_tokenizer.json
+-rw-r--r--   0        0        0  1355257 2024-04-13 16:05:24.458073 novelai_python-0.4.8/src/novelai_python/tokenizer/gpt2_tokenizer.json
+-rw-r--r--   0        0        0  1033724 2024-04-13 16:05:24.466073 novelai_python-0.4.8/src/novelai_python/tokenizer/nerdstash_v1.model
+-rw-r--r--   0        0        0  1033744 2024-04-13 16:05:24.470074 novelai_python-0.4.8/src/novelai_python/tokenizer/nerdstash_v2.model
+-rw-r--r--   0        0        0  1033724 2024-04-13 16:05:24.470074 novelai_python-0.4.8/src/novelai_python/tokenizer/novelai.model
+-rw-r--r--   0        0        0  1033744 2024-04-13 16:05:24.470074 novelai_python-0.4.8/src/novelai_python/tokenizer/novelai_v2.model
+-rw-r--r--   0        0        0  1357239 2024-04-13 16:05:24.478073 novelai_python-0.4.8/src/novelai_python/tokenizer/pile_tokenizer.json
+-rw-r--r--   0        0        0     4854 2024-04-13 16:05:24.478073 novelai_python-0.4.8/src/novelai_python/tokenizer/simple_tokenizer.py
+-rw-r--r--   0        0        0       24 2024-04-13 16:05:24.478073 novelai_python-0.4.8/src/novelai_python/tool/__init__.py
+-rw-r--r--   0        0        0     9084 2024-04-13 16:05:24.478073 novelai_python-0.4.8/src/novelai_python/tool/image_metadata/__init__.py
+-rw-r--r--   0        0        0     3316 2024-04-13 16:05:24.478073 novelai_python-0.4.8/src/novelai_python/tool/image_metadata/lsb_extractor.py
+-rw-r--r--   0        0        0     2211 2024-04-13 16:05:24.478073 novelai_python-0.4.8/src/novelai_python/tool/image_metadata/lsb_injector.py
+-rw-r--r--   0        0        0     3082 2024-04-13 16:05:24.478073 novelai_python-0.4.8/src/novelai_python/tool/paint_mask/__init__.py
+-rw-r--r--   0        0        0    17162 2024-04-13 16:05:24.478073 novelai_python-0.4.8/src/novelai_python/tool/random_prompt/__init__.py
+-rw-r--r--   0        0        0    84988 2024-04-13 16:05:24.478073 novelai_python-0.4.8/src/novelai_python/tool/random_prompt/tag.py
+-rw-r--r--   0        0        0    21015 2024-04-13 16:05:24.478073 novelai_python-0.4.8/src/novelai_python/tool/random_prompt/tag_character.py
+-rw-r--r--   0        0        0    15814 2024-04-13 16:05:24.478073 novelai_python-0.4.8/src/novelai_python/tool/random_prompt/tag_nsfw.py
+-rwxr-xr-x   0        0        0      525 2024-04-13 16:05:24.478073 novelai_python-0.4.8/src/novelai_python/utils/__init__.py
+-rwxr-xr-x   0        0        0     2419 2024-04-13 16:05:24.478073 novelai_python-0.4.8/src/novelai_python/utils/encode.py
+-rwxr-xr-x   0        0        0     1243 2024-04-13 16:05:24.478073 novelai_python-0.4.8/src/novelai_python/utils/useful.py
+-rwxr-xr-x   0        0        0        0 2024-04-13 16:05:24.478073 novelai_python-0.4.8/tests/__init__.py
+-rw-r--r--   0        0        0      870 2024-04-13 16:05:24.478073 novelai_python-0.4.8/tests/test_generate_voice.py
+-rwxr-xr-x   0        0        0     2273 2024-04-13 16:05:24.478073 novelai_python-0.4.8/tests/test_random_prompt.py
+-rwxr-xr-x   0        0        0      422 2024-04-13 16:05:24.478073 novelai_python-0.4.8/tests/test_server.py
+-rwxr-xr-x   0        0        0     1375 2024-04-13 16:05:24.478073 novelai_python-0.4.8/tests/test_server_run.py
+-rwxr-xr-x   0        0        0     2772 2024-04-13 16:05:24.478073 novelai_python-0.4.8/tests/test_upscale.py
+-rwxr-xr-x   0        0        0     2592 2024-04-13 16:05:24.478073 novelai_python-0.4.8/tests/test_user_information.py
+-rwxr-xr-x   0        0        0     3244 2024-04-13 16:05:24.482073 novelai_python-0.4.8/tests/test_user_login.py
+-rwxr-xr-x   0        0        0     3270 2024-04-13 16:05:24.482073 novelai_python-0.4.8/tests/test_user_subscription.py
+-rw-r--r--   0        0        0     4663 1970-01-01 00:00:00.000000 novelai_python-0.4.8/PKG-INFO
```

### Comparing `novelai_python-0.4.7/LICENSE` & `novelai_python-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.7/NOTICE.MD` & `novelai_python-0.4.8/NOTICE.MD`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.7/README.md` & `novelai_python-0.4.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 [![PyPI version](https://badge.fury.io/py/novelai-python.svg)](https://badge.fury.io/py/novelai-python)
 [![Downloads](https://pepy.tech/badge/novelai_python)](https://pepy.tech/project/novelai_python)
 
 ✨ NovelAI api python sdk with Pydantic, modern and user-friendly.
 
 The goal of this repository is to use Pydantic to build legitimate requests to access the NovelAI API service.
 
+> Python >= 3.9 is required.
+
 ### Roadmap 🚧
 
 - [x] tool.random_prompt
 - [x] tool.paint_mask
 - [x] tool.image_metadata
 - [x] /ai/generate-image
 - [x] /user/subscription
@@ -75,25 +77,26 @@
 #### LLM
 
 ```python
 import asyncio
 import os
 
 from dotenv import load_dotenv
+from pydantic import SecretStr
 
-from novelai_python import APIError, Login
+from novelai_python import APIError, LoginCredential
 from novelai_python.sdk.ai.generate import TextLLMModel, LLM
 
 load_dotenv()
 username = os.getenv("NOVELAI_USER", None)
 assert username is not None
 # credential = JwtCredential(jwt_token=SecretStr(jwt))
-login_credential = Login.build(
-    user_name=os.getenv("NOVELAI_USER"),
-    password=os.getenv("NOVELAI_PASS")
+login_credential = LoginCredential(
+    username=os.getenv("NOVELAI_USER"),
+    password=SecretStr(os.getenv("NOVELAI_PASS"))
 )
 
 
 async def chat(prompt: str):
     try:
         agent = LLM.build(prompt=prompt, model=TextLLMModel.Kayra)
         result = await agent.request(session=login_credential)
```

### Comparing `novelai_python-0.4.7/pyproject.toml` & `novelai_python-0.4.8/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "novelai-python"
-version = "0.4.7"
+version = "0.4.8"
 description = "NovelAI Python Binding With Pydantic"
 authors = [
     { name = "sudoskys", email = "coldlando@hotmail.com" },
 ]
 dependencies = [
     "elara>=0.5.5",
     "loguru>=0.7.2",
@@ -23,15 +23,15 @@
     "tenacity>=8.2.3",
     "sentencepiece>=0.2.0",
     "pynacl>=1.5.0",
     "ftfy>=6.2.0",
     "regex>=2023.12.25",
     "tokenizers>=0.15.2",
 ]
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 readme = "README.md"
 
 [project.license]
 text = "Apache License 2.0"
 
 [project.urls]
 Repository = "https://github.com/LlmKira/novelai-python/"
```

### Comparing `novelai_python-0.4.7/src/novelai_python/__init__.py` & `novelai_python-0.4.8/src/novelai_python/__init__.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.7/src/novelai_python/_exceptions.py` & `novelai_python-0.4.8/src/novelai_python/_exceptions.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.7/src/novelai_python/_response/ai/generate.py` & `novelai_python-0.4.8/src/novelai_python/_response/ai/generate.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.7/src/novelai_python/_response/ai/generate_image.py` & `novelai_python-0.4.8/src/novelai_python/_response/ai/generate_image.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.7/src/novelai_python/_response/ai/generate_stream.py` & `novelai_python-0.4.8/src/novelai_python/_response/ai/generate_stream.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.7/src/novelai_python/_response/user/information.py` & `novelai_python-0.4.8/src/novelai_python/_response/user/information.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.7/src/novelai_python/_response/user/subscription.py` & `novelai_python-0.4.8/src/novelai_python/_response/user/subscription.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.7/src/novelai_python/credential/ApiToken.py` & `novelai_python-0.4.8/src/novelai_python/credential/ApiToken.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.7/src/novelai_python/credential/JwtToken.py` & `novelai_python-0.4.8/src/novelai_python/credential/JwtToken.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.7/src/novelai_python/credential/UserAuth.py` & `novelai_python-0.4.8/src/novelai_python/credential/UserAuth.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.7/src/novelai_python/sdk/__init__.py` & `novelai_python-0.4.8/src/novelai_python/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.7/src/novelai_python/sdk/ai/LICENSE` & `novelai_python-0.4.8/src/novelai_python/sdk/ai/LICENSE`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.7/src/novelai_python/sdk/ai/generate/__init__.py` & `novelai_python-0.4.8/src/novelai_python/sdk/ai/generate/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from ....credential import CredentialBase
 from ....tokenizer import LLMTokenizer
 from ....utils.encode import tokens_to_b64
 
 
 class LLM(ApiBaseModel):
     """
-    LLM Stream for /ai/generate-stream
+    LLM for /ai/generate
     """
     _endpoint: str = PrivateAttr("https://api.novelai.net")
     input: str = Field(..., description="Base64 encoded token text")
     model: Union[TextLLMModel, str] = TextLLMModel.Kayra
     """Model to use"""
     parameters: Params = Params()
 
@@ -180,36 +180,36 @@
                     _msg = response.json()
                 except Exception as e:
                     _msg = {"statusCode": response.status_code, "message": response.content}
                 status_code = _msg.get("statusCode", response.status_code)
                 message = _msg.get("message", "Unknown error")
                 if status_code == 400:
                     raise APIError(
-                        "A validation error occured.",
+                        f"A validation error occured. {message}",
                         request=request_data, code=status_code, response=_msg
                     )
 
                 elif status_code == 401:
                     raise APIError(
-                        "Access Token is incorrect.",
+                        f"Access Token is incorrect. {message}",
                         request=request_data, code=status_code, response=_msg
                     )
                 elif status_code == 402:
                     raise APIError(
-                        "An active subscription is required to access this endpoint.",
+                        f"An active subscription is required to access this endpoint. {message}",
                         request=request_data, code=status_code, response=_msg
                     )
                 elif status_code == 409:
                     raise APIError(
-                        "A conflict error occured.",
+                        f"A conflict error occured. {message}",
                         request=request_data, code=status_code, response=_msg
                     )
                 else:
                     raise APIError(
-                        f"An unknown error occured.{response.status_code}",
+                        f"An unknown error occured. {response.status_code} {message}",
                         request=request_data, code=status_code, response=_msg
                     )
             else:
                 output = response.json().get("output", None)
                 assert output, APIError("No Content Returned",
                                         request=request_data, code=response.status_code, response=response.content
                                         )
```

### Comparing `novelai_python-0.4.7/src/novelai_python/sdk/ai/generate/_const.py` & `novelai_python-0.4.8/src/novelai_python/sdk/ai/generate/_const.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.7/src/novelai_python/sdk/ai/generate/_enum.py` & `novelai_python-0.4.8/src/novelai_python/sdk/ai/generate/_enum.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,11 +67,11 @@
     Mirostat = ("mirostat", 8)
 
 
 def generate_order(request_body: dict) -> List[int]:
     order_list = []
     for member in Order:
         key, order = member.value
-        if key in request_body and request_body[key]:
+        if key in request_body and request_body[key] is None:
             order_list.append(order)
     order_list.sort()  # ensures the order list is properly sorted according to the true order
     return order_list
```

### Comparing `novelai_python-0.4.7/src/novelai_python/sdk/ai/generate/_preset.py` & `novelai_python-0.4.8/src/novelai_python/sdk/ai/generate/_preset.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.7/src/novelai_python/sdk/ai/generate_image/__init__.py` & `novelai_python-0.4.8/src/novelai_python/sdk/ai/generate_image/__init__.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.7/src/novelai_python/sdk/ai/generate_image/_const.py` & `novelai_python-0.4.8/src/novelai_python/sdk/ai/generate_image/_const.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.7/src/novelai_python/sdk/ai/generate_image/_enum.py` & `novelai_python-0.4.8/src/novelai_python/sdk/ai/generate_image/_enum.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.7/src/novelai_python/sdk/ai/generate_image/suggest_tags.py` & `novelai_python-0.4.8/src/novelai_python/sdk/ai/generate_image/suggest_tags.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.7/src/novelai_python/sdk/ai/generate_stream.py` & `novelai_python-0.4.8/src/novelai_python/sdk/ai/generate_stream.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.7/src/novelai_python/sdk/ai/generate_voice/__init__.py` & `novelai_python-0.4.8/src/novelai_python/sdk/ai/generate_voice/__init__.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.7/src/novelai_python/sdk/ai/generate_voice/_enum.py` & `novelai_python-0.4.8/src/novelai_python/sdk/ai/generate_voice/_enum.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.7/src/novelai_python/sdk/ai/upscale.py` & `novelai_python-0.4.8/src/novelai_python/sdk/ai/upscale.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.7/src/novelai_python/sdk/schema.py` & `novelai_python-0.4.8/src/novelai_python/sdk/schema.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.7/src/novelai_python/sdk/user/information.py` & `novelai_python-0.4.8/src/novelai_python/sdk/user/information.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.7/src/novelai_python/sdk/user/login.py` & `novelai_python-0.4.8/src/novelai_python/sdk/user/login.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.7/src/novelai_python/sdk/user/subscription.py` & `novelai_python-0.4.8/src/novelai_python/sdk/user/subscription.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.7/src/novelai_python/server.py` & `novelai_python-0.4.8/src/novelai_python/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,15 +186,14 @@
 
     async def generator():
         agent = req
         session = await get_session(current_token)  # Assume 'get_session()' is a function to get session by token
         generator = agent.request(session=session)
         async for data in generator:
             data: LLMStreamResp
-            print(data)  # 或者做其他需要的处理
             yield data.text  # Yield data for streaming response
 
     return StreamingResponse(generator())
 
 
 @app.post("/ai/generate")
 async def generate(
```

### Comparing `novelai_python-0.4.7/src/novelai_python/tokenizer/NOTICE.MD` & `novelai_python-0.4.8/src/novelai_python/tokenizer/NOTICE.MD`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.7/src/novelai_python/tokenizer/__init__.py` & `novelai_python-0.4.8/src/novelai_python/tokenizer/__init__.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.7/src/novelai_python/tokenizer/bpe_simple_vocab_16e6.txt.gz` & `novelai_python-0.4.8/src/novelai_python/tokenizer/bpe_simple_vocab_16e6.txt.gz`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.7/src/novelai_python/tokenizer/gpt2-genji_tokenizer.json` & `novelai_python-0.4.8/src/novelai_python/tokenizer/gpt2-genji_tokenizer.json`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.7/src/novelai_python/tokenizer/gpt2_tokenizer.json` & `novelai_python-0.4.8/src/novelai_python/tokenizer/gpt2_tokenizer.json`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.7/src/novelai_python/tokenizer/nerdstash_v1.model` & `novelai_python-0.4.8/src/novelai_python/tokenizer/nerdstash_v1.model`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.7/src/novelai_python/tokenizer/nerdstash_v2.model` & `novelai_python-0.4.8/src/novelai_python/tokenizer/nerdstash_v2.model`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.7/src/novelai_python/tokenizer/novelai.model` & `novelai_python-0.4.8/src/novelai_python/tokenizer/novelai.model`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.7/src/novelai_python/tokenizer/novelai_v2.model` & `novelai_python-0.4.8/src/novelai_python/tokenizer/novelai_v2.model`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.7/src/novelai_python/tokenizer/pile_tokenizer.json` & `novelai_python-0.4.8/src/novelai_python/tokenizer/pile_tokenizer.json`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.7/src/novelai_python/tokenizer/simple_tokenizer.py` & `novelai_python-0.4.8/src/novelai_python/tokenizer/simple_tokenizer.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.7/src/novelai_python/tool/image_metadata/__init__.py` & `novelai_python-0.4.8/src/novelai_python/tool/image_metadata/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 import base64
 import json
 from io import BytesIO
 from pathlib import Path
-from typing import Union
+from typing import Union, Optional, List
 
 import numpy as np
 from PIL import Image
 from PIL.PngImagePlugin import PngInfo
 from loguru import logger
 from nacl.encoding import Base64Encoder
 from nacl.signing import VerifyKey
@@ -32,16 +32,18 @@
         uncond_scale: float = None
         cfg_rescale: float = None
         seed: int = None
         n_samples: int = None
         hide_debug_overlay: bool = None
         noise_schedule: str = None
         legacy_v3_extend: bool = None
-        reference_information_extracted: float = None
-        reference_strength: float = None
+        reference_information_extracted: Optional[float] = None
+        reference_strength: Optional[float] = None
+        reference_strength_multiple: Optional[List[float]] = None
+        reference_information_extracted_multiple: Optional[List[float]] = None
         sampler: str = None
         controlnet_strength: float = None
         controlnet_model: Union[None, str] = None
         dynamic_thresholding: bool = None
         dynamic_thresholding_percentile: float = None
         dynamic_thresholding_mimic_scale: float = None
         sm: bool = None
@@ -54,14 +56,37 @@
         signed_hash: str = None
         model_config = ConfigDict(extra="allow")
 
         @property
         def negative_prompt(self):
             return self.uc
 
+        @property
+        def vibe_transfer_strength(self) -> List[float]:
+            """
+            Get the vibe transfer strength totally
+            :return: List[float]
+            """
+            if self.reference_strength_multiple:
+                return self.reference_strength_multiple
+            reference_strength = [] if self.reference_strength is None else [self.reference_strength]
+            return reference_strength
+
+        @property
+        def vibe_transfer_information(self) -> List[float]:
+            """
+            Get the vibe transfer information totally
+            :return: List[float]
+            """
+            if self.reference_information_extracted_multiple:
+                return self.reference_information_extracted_multiple
+            reference_information = [] if self.reference_information_extracted is None else [
+                self.reference_information_extracted]
+            return reference_information
+
     Title: str = "AI generated image"
     Software: str = "NovelAI"
     Source: str = None
     Description: str
     Comment: CommentModel
     """
     AI generated image
```

### Comparing `novelai_python-0.4.7/src/novelai_python/tool/image_metadata/lsb_extractor.py` & `novelai_python-0.4.8/src/novelai_python/tool/image_metadata/lsb_extractor.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.7/src/novelai_python/tool/image_metadata/lsb_injector.py` & `novelai_python-0.4.8/src/novelai_python/tool/image_metadata/lsb_injector.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.7/src/novelai_python/tool/paint_mask/__init__.py` & `novelai_python-0.4.8/src/novelai_python/tool/paint_mask/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import cv2 as cv
 import numpy as np
 
 
-def create_mask_from_sketch(original_img_bytes: bytes,
-                            sketch_img_bytes: bytes,
-                            min_block_size: int = 15,
-                            jagged_edges: bool = True,
-                            output_format: str = '.png'
-                            ) -> bytes:
+def create_mask_from_sketch(
+        original_img_bytes: bytes,
+        sketch_img_bytes: bytes,
+        min_block_size: int = 15,
+        jagged_edges: bool = True,
+        output_format: str = '.png'
+) -> bytes:
     """
     Function to create a mask from original and sketch images input as bytes. Returns BytesIO object.
 
     :param original_img_bytes:  Bytes corresponding to the original image.
     :param sketch_img_bytes:  Bytes corresponding to the sketch image.
     :param min_block_size:  The minimum size of the pixel blocks. Default is 1, i.e., no pixelation.
     :param jagged_edges:  If set to True, the edges of the resulting mask will be more jagged.
```

### Comparing `novelai_python-0.4.7/src/novelai_python/tool/random_prompt/__init__.py` & `novelai_python-0.4.8/src/novelai_python/tool/random_prompt/__init__.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.7/src/novelai_python/tool/random_prompt/tag.py` & `novelai_python-0.4.8/src/novelai_python/tool/random_prompt/tag.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.7/src/novelai_python/tool/random_prompt/tag_character.py` & `novelai_python-0.4.8/src/novelai_python/tool/random_prompt/tag_character.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.7/src/novelai_python/tool/random_prompt/tag_nsfw.py` & `novelai_python-0.4.8/src/novelai_python/tool/random_prompt/tag_nsfw.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.7/src/novelai_python/utils/__init__.py` & `novelai_python-0.4.8/src/novelai_python/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.7/src/novelai_python/utils/encode.py` & `novelai_python-0.4.8/src/novelai_python/utils/encode.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.7/src/novelai_python/utils/useful.py` & `novelai_python-0.4.8/src/novelai_python/utils/useful.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.7/tests/test_generate_voice.py` & `novelai_python-0.4.8/tests/test_generate_voice.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.7/tests/test_random_prompt.py` & `novelai_python-0.4.8/tests/test_random_prompt.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.7/tests/test_server_run.py` & `novelai_python-0.4.8/tests/test_server_run.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.7/tests/test_upscale.py` & `novelai_python-0.4.8/tests/test_upscale.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.7/tests/test_user_information.py` & `novelai_python-0.4.8/tests/test_user_information.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.7/tests/test_user_login.py` & `novelai_python-0.4.8/tests/test_user_login.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.7/tests/test_user_subscription.py` & `novelai_python-0.4.8/tests/test_user_subscription.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.7/PKG-INFO` & `novelai_python-0.4.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: novelai-python
-Version: 0.4.7
+Version: 0.4.8
 Summary: NovelAI Python Binding With Pydantic
 Author-Email: sudoskys <coldlando@hotmail.com>
 License: Apache License 2.0
 Project-URL: Repository, https://github.com/LlmKira/novelai-python/
 Project-URL: Issues, https://github.com/LlmKira/novelai-python/issues
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Requires-Dist: elara>=0.5.5
 Requires-Dist: loguru>=0.7.2
 Requires-Dist: pydantic-settings>=2.1.0
 Requires-Dist: pydantic>=2.5.3
 Requires-Dist: httpx>=0.26.0
 Requires-Dist: shortuuid>=1.0.11
 Requires-Dist: Pillow>=10.2.0
@@ -39,14 +39,16 @@
 [![PyPI version](https://badge.fury.io/py/novelai-python.svg)](https://badge.fury.io/py/novelai-python)
 [![Downloads](https://pepy.tech/badge/novelai_python)](https://pepy.tech/project/novelai_python)
 
 ✨ NovelAI api python sdk with Pydantic, modern and user-friendly.
 
 The goal of this repository is to use Pydantic to build legitimate requests to access the NovelAI API service.
 
+> Python >= 3.9 is required.
+
 ### Roadmap 🚧
 
 - [x] tool.random_prompt
 - [x] tool.paint_mask
 - [x] tool.image_metadata
 - [x] /ai/generate-image
 - [x] /user/subscription
@@ -109,25 +111,26 @@
 #### LLM
 
 ```python
 import asyncio
 import os
 
 from dotenv import load_dotenv
+from pydantic import SecretStr
 
-from novelai_python import APIError, Login
+from novelai_python import APIError, LoginCredential
 from novelai_python.sdk.ai.generate import TextLLMModel, LLM
 
 load_dotenv()
 username = os.getenv("NOVELAI_USER", None)
 assert username is not None
 # credential = JwtCredential(jwt_token=SecretStr(jwt))
-login_credential = Login.build(
-    user_name=os.getenv("NOVELAI_USER"),
-    password=os.getenv("NOVELAI_PASS")
+login_credential = LoginCredential(
+    username=os.getenv("NOVELAI_USER"),
+    password=SecretStr(os.getenv("NOVELAI_PASS"))
 )
 
 
 async def chat(prompt: str):
     try:
         agent = LLM.build(prompt=prompt, model=TextLLMModel.Kayra)
         result = await agent.request(session=login_credential)
```

