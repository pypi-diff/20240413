# Comparing `tmp/glitter_proto-0.5.0.tar.gz` & `tmp/glitter_proto-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glitter_proto-0.5.0.tar", max compression
+gzip compressed data, was "glitter_proto-0.6.0.tar", max compression
```

## Comparing `glitter_proto-0.5.0.tar` & `glitter_proto-0.6.0.tar`

### file list

```diff
@@ -1,139 +1,139 @@
--rw-r--r--   0        0        0       33 2023-08-26 03:12:16.545137 glitter_proto-0.5.0/README.md
--rw-r--r--   0        0        0        0 2024-04-07 08:06:03.444587 glitter_proto-0.5.0/glitter_proto/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 08:06:03.444655 glitter_proto-0.5.0/glitter_proto/blockved/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 08:06:03.444695 glitter_proto-0.5.0/glitter_proto/blockved/glitterchain/__init__.py
--rw-r--r--   0        0        0    29786 2024-04-07 08:06:03.446132 glitter_proto-0.5.0/glitter_proto/blockved/glitterchain/index/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 08:06:03.446200 glitter_proto-0.5.0/glitter_proto/cosmos/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 08:06:03.446241 glitter_proto-0.5.0/glitter_proto/cosmos/auth/__init__.py
--rw-r--r--   0        0        0     8257 2024-04-07 08:06:03.446907 glitter_proto-0.5.0/glitter_proto/cosmos/auth/v1beta1/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 08:06:03.446957 glitter_proto-0.5.0/glitter_proto/cosmos/authz/__init__.py
--rw-r--r--   0        0        0    15411 2024-04-07 08:06:03.447550 glitter_proto-0.5.0/glitter_proto/cosmos/authz/v1beta1/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 08:06:03.447600 glitter_proto-0.5.0/glitter_proto/cosmos/bank/__init__.py
--rw-r--r--   0        0        0    25810 2024-04-07 08:06:03.447722 glitter_proto-0.5.0/glitter_proto/cosmos/bank/v1beta1/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 08:06:03.447770 glitter_proto-0.5.0/glitter_proto/cosmos/base/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 08:06:03.447808 glitter_proto-0.5.0/glitter_proto/cosmos/base/abci/__init__.py
--rw-r--r--   0        0        0     6011 2024-04-07 08:06:03.448535 glitter_proto-0.5.0/glitter_proto/cosmos/base/abci/v1beta1/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 08:06:03.448638 glitter_proto-0.5.0/glitter_proto/cosmos/base/kv/__init__.py
--rw-r--r--   0        0        0      632 2024-04-07 08:06:03.449638 glitter_proto-0.5.0/glitter_proto/cosmos/base/kv/v1beta1/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 08:06:03.449700 glitter_proto-0.5.0/glitter_proto/cosmos/base/query/__init__.py
--rw-r--r--   0        0        0     2275 2024-04-07 08:06:03.449813 glitter_proto-0.5.0/glitter_proto/cosmos/base/query/v1beta1/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 08:06:03.449863 glitter_proto-0.5.0/glitter_proto/cosmos/base/reflection/__init__.py
--rw-r--r--   0        0        0     4758 2024-04-07 08:06:03.449989 glitter_proto-0.5.0/glitter_proto/cosmos/base/reflection/v1beta1/__init__.py
--rw-r--r--   0        0        0    20944 2024-04-07 08:06:03.450664 glitter_proto-0.5.0/glitter_proto/cosmos/base/reflection/v2alpha1/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 08:06:03.450717 glitter_proto-0.5.0/glitter_proto/cosmos/base/snapshots/__init__.py
--rw-r--r--   0        0        0     2402 2024-04-07 08:06:03.450827 glitter_proto-0.5.0/glitter_proto/cosmos/base/snapshots/v1beta1/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 08:06:03.450877 glitter_proto-0.5.0/glitter_proto/cosmos/base/store/__init__.py
--rw-r--r--   0        0        0     1714 2024-04-07 08:06:03.451151 glitter_proto-0.5.0/glitter_proto/cosmos/base/store/v1beta1/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 08:06:03.451203 glitter_proto-0.5.0/glitter_proto/cosmos/base/tendermint/__init__.py
--rw-r--r--   0        0        0    14434 2024-04-07 08:06:03.451322 glitter_proto-0.5.0/glitter_proto/cosmos/base/tendermint/v1beta1/__init__.py
--rw-r--r--   0        0        0     1289 2024-04-07 08:06:03.451491 glitter_proto-0.5.0/glitter_proto/cosmos/base/v1beta1/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 08:06:03.451537 glitter_proto-0.5.0/glitter_proto/cosmos/capability/__init__.py
--rw-r--r--   0        0        0     1960 2024-04-07 08:06:03.451638 glitter_proto-0.5.0/glitter_proto/cosmos/capability/v1beta1/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 08:06:03.451682 glitter_proto-0.5.0/glitter_proto/cosmos/crisis/__init__.py
--rw-r--r--   0        0        0     2933 2024-04-07 08:06:03.451798 glitter_proto-0.5.0/glitter_proto/cosmos/crisis/v1beta1/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 08:06:03.451842 glitter_proto-0.5.0/glitter_proto/cosmos/crypto/__init__.py
--rw-r--r--   0        0        0     1012 2024-04-07 08:06:03.451938 glitter_proto-0.5.0/glitter_proto/cosmos/crypto/ed25519/__init__.py
--rw-r--r--   0        0        0      711 2024-04-07 08:06:03.452052 glitter_proto-0.5.0/glitter_proto/cosmos/crypto/multisig/__init__.py
--rw-r--r--   0        0        0     1045 2024-04-07 08:06:03.452162 glitter_proto-0.5.0/glitter_proto/cosmos/crypto/multisig/v1beta1/__init__.py
--rw-r--r--   0        0        0      838 2024-04-07 08:06:03.452273 glitter_proto-0.5.0/glitter_proto/cosmos/crypto/secp256k1/__init__.py
--rw-r--r--   0        0        0      812 2024-04-07 08:06:03.452383 glitter_proto-0.5.0/glitter_proto/cosmos/crypto/secp256r1/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 08:06:03.452427 glitter_proto-0.5.0/glitter_proto/cosmos/distribution/__init__.py
--rw-r--r--   0        0        0    40219 2024-04-07 08:06:03.453691 glitter_proto-0.5.0/glitter_proto/cosmos/distribution/v1beta1/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 08:06:03.453739 glitter_proto-0.5.0/glitter_proto/cosmos/evidence/__init__.py
--rw-r--r--   0        0        0     7859 2024-04-07 08:06:03.453846 glitter_proto-0.5.0/glitter_proto/cosmos/evidence/v1beta1/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 08:06:03.453890 glitter_proto-0.5.0/glitter_proto/cosmos/feegrant/__init__.py
--rw-r--r--   0        0        0    15250 2024-04-07 08:06:03.454011 glitter_proto-0.5.0/glitter_proto/cosmos/feegrant/v1beta1/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 08:06:03.454055 glitter_proto-0.5.0/glitter_proto/cosmos/genutil/__init__.py
--rw-r--r--   0        0        0      498 2024-04-07 08:06:03.454447 glitter_proto-0.5.0/glitter_proto/cosmos/genutil/v1beta1/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 08:06:03.454491 glitter_proto-0.5.0/glitter_proto/cosmos/gov/__init__.py
--rw-r--r--   0        0        0    31135 2024-04-07 08:06:03.454898 glitter_proto-0.5.0/glitter_proto/cosmos/gov/v1beta1/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 08:06:03.454946 glitter_proto-0.5.0/glitter_proto/cosmos/mint/__init__.py
--rw-r--r--   0        0        0     7573 2024-04-07 08:06:03.455052 glitter_proto-0.5.0/glitter_proto/cosmos/mint/v1beta1/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 08:06:03.455145 glitter_proto-0.5.0/glitter_proto/cosmos/params/__init__.py
--rw-r--r--   0        0        0     3278 2024-04-07 08:06:03.455247 glitter_proto-0.5.0/glitter_proto/cosmos/params/v1beta1/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 08:06:03.455290 glitter_proto-0.5.0/glitter_proto/cosmos/slashing/__init__.py
--rw-r--r--   0        0        0    11818 2024-04-07 08:06:03.455399 glitter_proto-0.5.0/glitter_proto/cosmos/slashing/v1beta1/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 08:06:03.455442 glitter_proto-0.5.0/glitter_proto/cosmos/staking/__init__.py
--rw-r--r--   0        0        0    58934 2024-04-07 08:06:03.456457 glitter_proto-0.5.0/glitter_proto/cosmos/staking/v1beta1/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 08:06:03.456506 glitter_proto-0.5.0/glitter_proto/cosmos/tx/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 08:06:03.456541 glitter_proto-0.5.0/glitter_proto/cosmos/tx/signing/__init__.py
--rw-r--r--   0        0        0     4010 2024-04-07 08:06:03.456657 glitter_proto-0.5.0/glitter_proto/cosmos/tx/signing/v1beta1/__init__.py
--rw-r--r--   0        0        0    21893 2024-04-07 08:06:03.456789 glitter_proto-0.5.0/glitter_proto/cosmos/tx/v1beta1/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 08:06:03.456841 glitter_proto-0.5.0/glitter_proto/cosmos/upgrade/__init__.py
--rw-r--r--   0        0        0    12565 2024-04-07 08:06:03.456948 glitter_proto-0.5.0/glitter_proto/cosmos/upgrade/v1beta1/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 08:06:03.456992 glitter_proto-0.5.0/glitter_proto/cosmos/vesting/__init__.py
--rw-r--r--   0        0        0     9706 2024-04-07 08:06:03.457668 glitter_proto-0.5.0/glitter_proto/cosmos/vesting/v1beta1/__init__.py
--rw-r--r--   0        0        0      212 2024-04-07 08:06:03.457811 glitter_proto-0.5.0/glitter_proto/cosmos_proto/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 08:06:03.457859 glitter_proto-0.5.0/glitter_proto/cosmwasm/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 08:06:03.457900 glitter_proto-0.5.0/glitter_proto/cosmwasm/wasm/__init__.py
--rw-r--r--   0        0        0    47983 2024-04-07 08:06:03.458432 glitter_proto-0.5.0/glitter_proto/cosmwasm/wasm/v1/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 08:06:03.458496 glitter_proto-0.5.0/glitter_proto/ethermint/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 08:06:03.458537 glitter_proto-0.5.0/glitter_proto/ethermint/crypto/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 08:06:03.458572 glitter_proto-0.5.0/glitter_proto/ethermint/crypto/v1/__init__.py
--rw-r--r--   0        0        0      771 2024-04-07 08:06:03.458697 glitter_proto-0.5.0/glitter_proto/ethermint/crypto/v1/ethsecp256k1/__init__.py
--rw-r--r--   0        0        0      558 2023-08-26 03:12:16.627000 glitter_proto-0.5.0/glitter_proto/ethermint/crypto/v1/ethsecp256k1/keys.proto
--rw-r--r--   0        0        0        0 2024-04-07 08:06:03.458746 glitter_proto-0.5.0/glitter_proto/ethermint/evm/__init__.py
--rw-r--r--   0        0        0    40331 2024-04-07 08:06:03.459387 glitter_proto-0.5.0/glitter_proto/ethermint/evm/v1/__init__.py
--rw-r--r--   0        0        0     9239 2023-08-26 03:12:16.634744 glitter_proto-0.5.0/glitter_proto/ethermint/evm/v1/evm.proto
--rw-r--r--   0        0        0     1098 2023-08-26 03:12:16.634241 glitter_proto-0.5.0/glitter_proto/ethermint/evm/v1/genesis.proto
--rw-r--r--   0        0        0     9727 2023-08-26 03:12:16.633838 glitter_proto-0.5.0/glitter_proto/ethermint/evm/v1/query.proto
--rw-r--r--   0        0        0     6114 2023-08-26 03:12:16.632908 glitter_proto-0.5.0/glitter_proto/ethermint/evm/v1/tx.proto
--rw-r--r--   0        0        0        0 2024-04-07 08:06:03.459437 glitter_proto-0.5.0/glitter_proto/ethermint/feemarket/__init__.py
--rw-r--r--   0        0        0     7355 2024-04-07 08:06:03.459549 glitter_proto-0.5.0/glitter_proto/ethermint/feemarket/v1/__init__.py
--rw-r--r--   0        0        0     1403 2023-08-26 03:12:16.632005 glitter_proto-0.5.0/glitter_proto/ethermint/feemarket/v1/feemarket.proto
--rw-r--r--   0        0        0      662 2023-08-26 03:12:16.631581 glitter_proto-0.5.0/glitter_proto/ethermint/feemarket/v1/genesis.proto
--rw-r--r--   0        0        0     1840 2023-08-26 03:12:16.631277 glitter_proto-0.5.0/glitter_proto/ethermint/feemarket/v1/query.proto
--rw-r--r--   0        0        0        0 2024-04-07 08:06:03.459596 glitter_proto-0.5.0/glitter_proto/ethermint/types/__init__.py
--rw-r--r--   0        0        0     2725 2024-04-07 08:06:03.459706 glitter_proto-0.5.0/glitter_proto/ethermint/types/v1/__init__.py
--rw-r--r--   0        0        0      835 2023-08-26 03:12:16.628425 glitter_proto-0.5.0/glitter_proto/ethermint/types/v1/account.proto
--rw-r--r--   0        0        0      479 2023-08-26 03:12:16.627945 glitter_proto-0.5.0/glitter_proto/ethermint/types/v1/dynamic_fee.proto
--rw-r--r--   0        0        0      877 2023-08-26 03:12:16.629609 glitter_proto-0.5.0/glitter_proto/ethermint/types/v1/indexer.proto
--rw-r--r--   0        0        0      891 2023-08-26 03:12:16.629208 glitter_proto-0.5.0/glitter_proto/ethermint/types/v1/web3.proto
--rw-r--r--   0        0        0      207 2024-04-07 08:06:03.459815 glitter_proto-0.5.0/glitter_proto/gogoproto/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 08:06:03.459857 glitter_proto-0.5.0/glitter_proto/google/__init__.py
--rw-r--r--   0        0        0    13671 2024-04-07 08:06:03.459959 glitter_proto-0.5.0/glitter_proto/google/api/__init__.py
--rw-r--r--   0        0        0        0 2023-08-26 03:12:16.553884 glitter_proto-0.5.0/glitter_proto/google/protobuf/__init__.py
--rw-r--r--   0        0        0     6214 2023-08-26 03:12:16.554550 glitter_proto-0.5.0/glitter_proto/google/protobuf/compiler/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 08:06:03.460001 glitter_proto-0.5.0/glitter_proto/ibc/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 08:06:03.460039 glitter_proto-0.5.0/glitter_proto/ibc/applications/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 08:06:03.460073 glitter_proto-0.5.0/glitter_proto/ibc/applications/fee/__init__.py
--rw-r--r--   0        0        0    33167 2024-04-07 08:06:03.460467 glitter_proto-0.5.0/glitter_proto/ibc/applications/fee/v1/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 08:06:03.460571 glitter_proto-0.5.0/glitter_proto/ibc/applications/interchain_accounts/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 08:06:03.460609 glitter_proto-0.5.0/glitter_proto/ibc/applications/interchain_accounts/controller/__init__.py
--rw-r--r--   0        0        0     2892 2024-04-07 08:06:03.460723 glitter_proto-0.5.0/glitter_proto/ibc/applications/interchain_accounts/controller/v1/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 08:06:03.460775 glitter_proto-0.5.0/glitter_proto/ibc/applications/interchain_accounts/host/__init__.py
--rw-r--r--   0        0        0     3027 2024-04-07 08:06:03.460890 glitter_proto-0.5.0/glitter_proto/ibc/applications/interchain_accounts/host/v1/__init__.py
--rw-r--r--   0        0        0     5211 2024-04-07 08:06:03.461012 glitter_proto-0.5.0/glitter_proto/ibc/applications/interchain_accounts/v1/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 08:06:03.461058 glitter_proto-0.5.0/glitter_proto/ibc/applications/transfer/__init__.py
--rw-r--r--   0        0        0    13022 2024-04-07 08:06:03.461168 glitter_proto-0.5.0/glitter_proto/ibc/applications/transfer/v1/__init__.py
--rw-r--r--   0        0        0      916 2024-04-07 08:06:03.461515 glitter_proto-0.5.0/glitter_proto/ibc/applications/transfer/v2/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 08:06:03.461571 glitter_proto-0.5.0/glitter_proto/ibc/core/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 08:06:03.461621 glitter_proto-0.5.0/glitter_proto/ibc/core/channel/__init__.py
--rw-r--r--   0        0        0    61493 2024-04-07 08:06:03.462831 glitter_proto-0.5.0/glitter_proto/ibc/core/channel/v1/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 08:06:03.462896 glitter_proto-0.5.0/glitter_proto/ibc/core/client/__init__.py
--rw-r--r--   0        0        0    32886 2024-04-07 08:06:03.463729 glitter_proto-0.5.0/glitter_proto/ibc/core/client/v1/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 08:06:03.463790 glitter_proto-0.5.0/glitter_proto/ibc/core/commitment/__init__.py
--rw-r--r--   0        0        0     1643 2024-04-07 08:06:03.463913 glitter_proto-0.5.0/glitter_proto/ibc/core/commitment/v1/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 08:06:03.463963 glitter_proto-0.5.0/glitter_proto/ibc/core/connection/__init__.py
--rw-r--r--   0        0        0    28130 2024-04-07 08:06:03.464817 glitter_proto-0.5.0/glitter_proto/ibc/core/connection/v1/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 08:06:03.464875 glitter_proto-0.5.0/glitter_proto/ibc/core/types/__init__.py
--rw-r--r--   0        0        0      874 2024-04-07 08:06:03.464985 glitter_proto-0.5.0/glitter_proto/ibc/core/types/v1/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 08:06:03.465032 glitter_proto-0.5.0/glitter_proto/ibc/lightclients/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 08:06:03.465070 glitter_proto-0.5.0/glitter_proto/ibc/lightclients/localhost/__init__.py
--rw-r--r--   0        0        0      684 2024-04-07 08:06:03.465171 glitter_proto-0.5.0/glitter_proto/ibc/lightclients/localhost/v1/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 08:06:03.465219 glitter_proto-0.5.0/glitter_proto/ibc/lightclients/solomachine/__init__.py
--rw-r--r--   0        0        0     7740 2024-04-07 08:06:03.465331 glitter_proto-0.5.0/glitter_proto/ibc/lightclients/solomachine/v1/__init__.py
--rw-r--r--   0        0        0     7733 2024-04-07 08:06:03.465454 glitter_proto-0.5.0/glitter_proto/ibc/lightclients/solomachine/v2/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 08:06:03.465500 glitter_proto-0.5.0/glitter_proto/ibc/lightclients/tendermint/__init__.py
--rw-r--r--   0        0        0     5136 2024-04-07 08:06:03.465606 glitter_proto-0.5.0/glitter_proto/ibc/lightclients/tendermint/v1/__init__.py
--rw-r--r--   0        0        0    10180 2024-04-07 08:06:03.465780 glitter_proto-0.5.0/glitter_proto/ics23/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 08:06:03.465821 glitter_proto-0.5.0/glitter_proto/tendermint/__init__.py
--rw-r--r--   0        0        0    33422 2024-04-07 08:06:03.465973 glitter_proto-0.5.0/glitter_proto/tendermint/abci/__init__.py
--rw-r--r--   0        0        0     1849 2024-04-07 08:06:03.466098 glitter_proto-0.5.0/glitter_proto/tendermint/crypto/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 08:06:03.466143 glitter_proto-0.5.0/glitter_proto/tendermint/libs/__init__.py
--rw-r--r--   0        0        0      409 2024-04-07 08:06:03.466262 glitter_proto-0.5.0/glitter_proto/tendermint/libs/bits/__init__.py
--rw-r--r--   0        0        0     1320 2024-04-07 08:06:03.466369 glitter_proto-0.5.0/glitter_proto/tendermint/p2p/__init__.py
--rw-r--r--   0        0        0    11130 2024-04-07 08:06:03.466503 glitter_proto-0.5.0/glitter_proto/tendermint/types/__init__.py
--rw-r--r--   0        0        0      949 2024-04-07 08:06:03.466624 glitter_proto-0.5.0/glitter_proto/tendermint/version/__init__.py
--rw-r--r--   0        0        0      352 2024-04-07 09:16:59.042346 glitter_proto-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      564 1970-01-01 00:00:00.000000 glitter_proto-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0       33 2023-08-26 03:12:16.545137 glitter_proto-0.6.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-13 04:32:41.797205 glitter_proto-0.6.0/glitter_proto/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 04:32:41.797283 glitter_proto-0.6.0/glitter_proto/blockved/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 04:32:41.797330 glitter_proto-0.6.0/glitter_proto/blockved/glitterchain/__init__.py
+-rw-r--r--   0        0        0    32618 2024-04-13 04:32:41.797474 glitter_proto-0.6.0/glitter_proto/blockved/glitterchain/index/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 04:32:41.797582 glitter_proto-0.6.0/glitter_proto/cosmos/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 04:32:41.797625 glitter_proto-0.6.0/glitter_proto/cosmos/auth/__init__.py
+-rw-r--r--   0        0        0     8257 2024-04-13 04:32:41.797749 glitter_proto-0.6.0/glitter_proto/cosmos/auth/v1beta1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 04:32:41.797881 glitter_proto-0.6.0/glitter_proto/cosmos/authz/__init__.py
+-rw-r--r--   0        0        0    15411 2024-04-13 04:32:41.798012 glitter_proto-0.6.0/glitter_proto/cosmos/authz/v1beta1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 04:32:41.798115 glitter_proto-0.6.0/glitter_proto/cosmos/bank/__init__.py
+-rw-r--r--   0        0        0    25810 2024-04-13 04:32:41.798232 glitter_proto-0.6.0/glitter_proto/cosmos/bank/v1beta1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 04:32:41.798315 glitter_proto-0.6.0/glitter_proto/cosmos/base/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 04:32:41.798360 glitter_proto-0.6.0/glitter_proto/cosmos/base/abci/__init__.py
+-rw-r--r--   0        0        0     6011 2024-04-13 04:32:41.798535 glitter_proto-0.6.0/glitter_proto/cosmos/base/abci/v1beta1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 04:32:41.798660 glitter_proto-0.6.0/glitter_proto/cosmos/base/kv/__init__.py
+-rw-r--r--   0        0        0      632 2024-04-13 04:32:41.798794 glitter_proto-0.6.0/glitter_proto/cosmos/base/kv/v1beta1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 04:32:41.798941 glitter_proto-0.6.0/glitter_proto/cosmos/base/query/__init__.py
+-rw-r--r--   0        0        0     2275 2024-04-13 04:32:41.799048 glitter_proto-0.6.0/glitter_proto/cosmos/base/query/v1beta1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 04:32:41.799135 glitter_proto-0.6.0/glitter_proto/cosmos/base/reflection/__init__.py
+-rw-r--r--   0        0        0     4758 2024-04-13 04:32:41.799247 glitter_proto-0.6.0/glitter_proto/cosmos/base/reflection/v1beta1/__init__.py
+-rw-r--r--   0        0        0    20944 2024-04-13 04:32:41.799434 glitter_proto-0.6.0/glitter_proto/cosmos/base/reflection/v2alpha1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 04:32:41.799520 glitter_proto-0.6.0/glitter_proto/cosmos/base/snapshots/__init__.py
+-rw-r--r--   0        0        0     2402 2024-04-13 04:32:41.799623 glitter_proto-0.6.0/glitter_proto/cosmos/base/snapshots/v1beta1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 04:32:41.799707 glitter_proto-0.6.0/glitter_proto/cosmos/base/store/__init__.py
+-rw-r--r--   0        0        0     1714 2024-04-13 04:32:41.799817 glitter_proto-0.6.0/glitter_proto/cosmos/base/store/v1beta1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 04:32:41.799899 glitter_proto-0.6.0/glitter_proto/cosmos/base/tendermint/__init__.py
+-rw-r--r--   0        0        0    14434 2024-04-13 04:32:41.800006 glitter_proto-0.6.0/glitter_proto/cosmos/base/tendermint/v1beta1/__init__.py
+-rw-r--r--   0        0        0     1289 2024-04-13 04:32:41.800181 glitter_proto-0.6.0/glitter_proto/cosmos/base/v1beta1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 04:32:41.800260 glitter_proto-0.6.0/glitter_proto/cosmos/capability/__init__.py
+-rw-r--r--   0        0        0     1960 2024-04-13 04:32:41.800360 glitter_proto-0.6.0/glitter_proto/cosmos/capability/v1beta1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 04:32:41.800438 glitter_proto-0.6.0/glitter_proto/cosmos/crisis/__init__.py
+-rw-r--r--   0        0        0     2933 2024-04-13 04:32:41.800537 glitter_proto-0.6.0/glitter_proto/cosmos/crisis/v1beta1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 04:32:41.800616 glitter_proto-0.6.0/glitter_proto/cosmos/crypto/__init__.py
+-rw-r--r--   0        0        0     1012 2024-04-13 04:32:41.800714 glitter_proto-0.6.0/glitter_proto/cosmos/crypto/ed25519/__init__.py
+-rw-r--r--   0        0        0      711 2024-04-13 04:32:41.800848 glitter_proto-0.6.0/glitter_proto/cosmos/crypto/multisig/__init__.py
+-rw-r--r--   0        0        0     1045 2024-04-13 04:32:41.800988 glitter_proto-0.6.0/glitter_proto/cosmos/crypto/multisig/v1beta1/__init__.py
+-rw-r--r--   0        0        0      838 2024-04-13 04:32:41.801120 glitter_proto-0.6.0/glitter_proto/cosmos/crypto/secp256k1/__init__.py
+-rw-r--r--   0        0        0      812 2024-04-13 04:32:41.801249 glitter_proto-0.6.0/glitter_proto/cosmos/crypto/secp256r1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 04:32:41.801325 glitter_proto-0.6.0/glitter_proto/cosmos/distribution/__init__.py
+-rw-r--r--   0        0        0    40219 2024-04-13 04:32:41.801437 glitter_proto-0.6.0/glitter_proto/cosmos/distribution/v1beta1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 04:32:41.801520 glitter_proto-0.6.0/glitter_proto/cosmos/evidence/__init__.py
+-rw-r--r--   0        0        0     7859 2024-04-13 04:32:41.801629 glitter_proto-0.6.0/glitter_proto/cosmos/evidence/v1beta1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 04:32:41.801716 glitter_proto-0.6.0/glitter_proto/cosmos/feegrant/__init__.py
+-rw-r--r--   0        0        0    15250 2024-04-13 04:32:41.801816 glitter_proto-0.6.0/glitter_proto/cosmos/feegrant/v1beta1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 04:32:41.801901 glitter_proto-0.6.0/glitter_proto/cosmos/genutil/__init__.py
+-rw-r--r--   0        0        0      498 2024-04-13 04:32:41.801996 glitter_proto-0.6.0/glitter_proto/cosmos/genutil/v1beta1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 04:32:41.802075 glitter_proto-0.6.0/glitter_proto/cosmos/gov/__init__.py
+-rw-r--r--   0        0        0    31135 2024-04-13 04:32:41.802185 glitter_proto-0.6.0/glitter_proto/cosmos/gov/v1beta1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 04:32:41.802266 glitter_proto-0.6.0/glitter_proto/cosmos/mint/__init__.py
+-rw-r--r--   0        0        0     7573 2024-04-13 04:32:41.802366 glitter_proto-0.6.0/glitter_proto/cosmos/mint/v1beta1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 04:32:41.802453 glitter_proto-0.6.0/glitter_proto/cosmos/params/__init__.py
+-rw-r--r--   0        0        0     3278 2024-04-13 04:32:41.802547 glitter_proto-0.6.0/glitter_proto/cosmos/params/v1beta1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 04:32:41.802624 glitter_proto-0.6.0/glitter_proto/cosmos/slashing/__init__.py
+-rw-r--r--   0        0        0    11818 2024-04-13 04:32:41.802727 glitter_proto-0.6.0/glitter_proto/cosmos/slashing/v1beta1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 04:32:41.802886 glitter_proto-0.6.0/glitter_proto/cosmos/staking/__init__.py
+-rw-r--r--   0        0        0    58934 2024-04-13 04:32:41.803000 glitter_proto-0.6.0/glitter_proto/cosmos/staking/v1beta1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 04:32:41.803085 glitter_proto-0.6.0/glitter_proto/cosmos/tx/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 04:32:41.803128 glitter_proto-0.6.0/glitter_proto/cosmos/tx/signing/__init__.py
+-rw-r--r--   0        0        0     4010 2024-04-13 04:32:41.803231 glitter_proto-0.6.0/glitter_proto/cosmos/tx/signing/v1beta1/__init__.py
+-rw-r--r--   0        0        0    21893 2024-04-13 04:32:41.803380 glitter_proto-0.6.0/glitter_proto/cosmos/tx/v1beta1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 04:32:41.803460 glitter_proto-0.6.0/glitter_proto/cosmos/upgrade/__init__.py
+-rw-r--r--   0        0        0    12565 2024-04-13 04:32:41.803561 glitter_proto-0.6.0/glitter_proto/cosmos/upgrade/v1beta1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 04:32:41.803646 glitter_proto-0.6.0/glitter_proto/cosmos/vesting/__init__.py
+-rw-r--r--   0        0        0     9706 2024-04-13 04:32:41.803752 glitter_proto-0.6.0/glitter_proto/cosmos/vesting/v1beta1/__init__.py
+-rw-r--r--   0        0        0      212 2024-04-13 04:32:41.803936 glitter_proto-0.6.0/glitter_proto/cosmos_proto/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 04:32:41.804036 glitter_proto-0.6.0/glitter_proto/cosmwasm/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 04:32:41.804076 glitter_proto-0.6.0/glitter_proto/cosmwasm/wasm/__init__.py
+-rw-r--r--   0        0        0    47983 2024-04-13 04:32:41.804190 glitter_proto-0.6.0/glitter_proto/cosmwasm/wasm/v1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 04:32:41.804274 glitter_proto-0.6.0/glitter_proto/ethermint/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 04:32:41.804317 glitter_proto-0.6.0/glitter_proto/ethermint/crypto/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 04:32:41.804357 glitter_proto-0.6.0/glitter_proto/ethermint/crypto/v1/__init__.py
+-rw-r--r--   0        0        0      771 2024-04-13 04:32:41.804497 glitter_proto-0.6.0/glitter_proto/ethermint/crypto/v1/ethsecp256k1/__init__.py
+-rw-r--r--   0        0        0      558 2023-08-26 03:12:16.627000 glitter_proto-0.6.0/glitter_proto/ethermint/crypto/v1/ethsecp256k1/keys.proto
+-rw-r--r--   0        0        0        0 2024-04-13 04:32:41.804585 glitter_proto-0.6.0/glitter_proto/ethermint/evm/__init__.py
+-rw-r--r--   0        0        0    40331 2024-04-13 04:32:41.804743 glitter_proto-0.6.0/glitter_proto/ethermint/evm/v1/__init__.py
+-rw-r--r--   0        0        0     9239 2023-08-26 03:12:16.634744 glitter_proto-0.6.0/glitter_proto/ethermint/evm/v1/evm.proto
+-rw-r--r--   0        0        0     1098 2023-08-26 03:12:16.634241 glitter_proto-0.6.0/glitter_proto/ethermint/evm/v1/genesis.proto
+-rw-r--r--   0        0        0     9727 2023-08-26 03:12:16.633838 glitter_proto-0.6.0/glitter_proto/ethermint/evm/v1/query.proto
+-rw-r--r--   0        0        0     6114 2023-08-26 03:12:16.632908 glitter_proto-0.6.0/glitter_proto/ethermint/evm/v1/tx.proto
+-rw-r--r--   0        0        0        0 2024-04-13 04:32:41.804835 glitter_proto-0.6.0/glitter_proto/ethermint/feemarket/__init__.py
+-rw-r--r--   0        0        0     7355 2024-04-13 04:32:41.805065 glitter_proto-0.6.0/glitter_proto/ethermint/feemarket/v1/__init__.py
+-rw-r--r--   0        0        0     1403 2023-08-26 03:12:16.632005 glitter_proto-0.6.0/glitter_proto/ethermint/feemarket/v1/feemarket.proto
+-rw-r--r--   0        0        0      662 2023-08-26 03:12:16.631581 glitter_proto-0.6.0/glitter_proto/ethermint/feemarket/v1/genesis.proto
+-rw-r--r--   0        0        0     1840 2023-08-26 03:12:16.631277 glitter_proto-0.6.0/glitter_proto/ethermint/feemarket/v1/query.proto
+-rw-r--r--   0        0        0        0 2024-04-13 04:32:41.805235 glitter_proto-0.6.0/glitter_proto/ethermint/types/__init__.py
+-rw-r--r--   0        0        0     2725 2024-04-13 04:32:41.805415 glitter_proto-0.6.0/glitter_proto/ethermint/types/v1/__init__.py
+-rw-r--r--   0        0        0      835 2023-08-26 03:12:16.628425 glitter_proto-0.6.0/glitter_proto/ethermint/types/v1/account.proto
+-rw-r--r--   0        0        0      479 2023-08-26 03:12:16.627945 glitter_proto-0.6.0/glitter_proto/ethermint/types/v1/dynamic_fee.proto
+-rw-r--r--   0        0        0      877 2023-08-26 03:12:16.629609 glitter_proto-0.6.0/glitter_proto/ethermint/types/v1/indexer.proto
+-rw-r--r--   0        0        0      891 2023-08-26 03:12:16.629208 glitter_proto-0.6.0/glitter_proto/ethermint/types/v1/web3.proto
+-rw-r--r--   0        0        0      207 2024-04-13 04:32:41.805635 glitter_proto-0.6.0/glitter_proto/gogoproto/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 04:32:41.805764 glitter_proto-0.6.0/glitter_proto/google/__init__.py
+-rw-r--r--   0        0        0    13671 2024-04-13 04:32:41.805911 glitter_proto-0.6.0/glitter_proto/google/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-26 03:12:16.553884 glitter_proto-0.6.0/glitter_proto/google/protobuf/__init__.py
+-rw-r--r--   0        0        0     6214 2023-08-26 03:12:16.554550 glitter_proto-0.6.0/glitter_proto/google/protobuf/compiler/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 04:32:41.806069 glitter_proto-0.6.0/glitter_proto/ibc/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 04:32:41.806139 glitter_proto-0.6.0/glitter_proto/ibc/applications/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 04:32:41.806207 glitter_proto-0.6.0/glitter_proto/ibc/applications/fee/__init__.py
+-rw-r--r--   0        0        0    33167 2024-04-13 04:32:41.806425 glitter_proto-0.6.0/glitter_proto/ibc/applications/fee/v1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 04:32:41.806632 glitter_proto-0.6.0/glitter_proto/ibc/applications/interchain_accounts/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 04:32:41.806715 glitter_proto-0.6.0/glitter_proto/ibc/applications/interchain_accounts/controller/__init__.py
+-rw-r--r--   0        0        0     2892 2024-04-13 04:32:41.806895 glitter_proto-0.6.0/glitter_proto/ibc/applications/interchain_accounts/controller/v1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 04:32:41.807040 glitter_proto-0.6.0/glitter_proto/ibc/applications/interchain_accounts/host/__init__.py
+-rw-r--r--   0        0        0     3027 2024-04-13 04:32:41.807235 glitter_proto-0.6.0/glitter_proto/ibc/applications/interchain_accounts/host/v1/__init__.py
+-rw-r--r--   0        0        0     5211 2024-04-13 04:32:41.807489 glitter_proto-0.6.0/glitter_proto/ibc/applications/interchain_accounts/v1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 04:32:41.807644 glitter_proto-0.6.0/glitter_proto/ibc/applications/transfer/__init__.py
+-rw-r--r--   0        0        0    13022 2024-04-13 04:32:41.807890 glitter_proto-0.6.0/glitter_proto/ibc/applications/transfer/v1/__init__.py
+-rw-r--r--   0        0        0      916 2024-04-13 04:32:41.808126 glitter_proto-0.6.0/glitter_proto/ibc/applications/transfer/v2/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 04:32:41.808267 glitter_proto-0.6.0/glitter_proto/ibc/core/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 04:32:41.808339 glitter_proto-0.6.0/glitter_proto/ibc/core/channel/__init__.py
+-rw-r--r--   0        0        0    61493 2024-04-13 04:32:41.808495 glitter_proto-0.6.0/glitter_proto/ibc/core/channel/v1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 04:32:41.808590 glitter_proto-0.6.0/glitter_proto/ibc/core/client/__init__.py
+-rw-r--r--   0        0        0    32886 2024-04-13 04:32:41.808718 glitter_proto-0.6.0/glitter_proto/ibc/core/client/v1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 04:32:41.808810 glitter_proto-0.6.0/glitter_proto/ibc/core/commitment/__init__.py
+-rw-r--r--   0        0        0     1643 2024-04-13 04:32:41.808978 glitter_proto-0.6.0/glitter_proto/ibc/core/commitment/v1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 04:32:41.809142 glitter_proto-0.6.0/glitter_proto/ibc/core/connection/__init__.py
+-rw-r--r--   0        0        0    28130 2024-04-13 04:32:41.809370 glitter_proto-0.6.0/glitter_proto/ibc/core/connection/v1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 04:32:41.809500 glitter_proto-0.6.0/glitter_proto/ibc/core/types/__init__.py
+-rw-r--r--   0        0        0      874 2024-04-13 04:32:41.809667 glitter_proto-0.6.0/glitter_proto/ibc/core/types/v1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 04:32:41.809800 glitter_proto-0.6.0/glitter_proto/ibc/lightclients/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 04:32:41.809873 glitter_proto-0.6.0/glitter_proto/ibc/lightclients/localhost/__init__.py
+-rw-r--r--   0        0        0      684 2024-04-13 04:32:41.810051 glitter_proto-0.6.0/glitter_proto/ibc/lightclients/localhost/v1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 04:32:41.810187 glitter_proto-0.6.0/glitter_proto/ibc/lightclients/solomachine/__init__.py
+-rw-r--r--   0        0        0     7740 2024-04-13 04:32:41.810375 glitter_proto-0.6.0/glitter_proto/ibc/lightclients/solomachine/v1/__init__.py
+-rw-r--r--   0        0        0     7733 2024-04-13 04:32:41.810625 glitter_proto-0.6.0/glitter_proto/ibc/lightclients/solomachine/v2/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 04:32:41.810734 glitter_proto-0.6.0/glitter_proto/ibc/lightclients/tendermint/__init__.py
+-rw-r--r--   0        0        0     5136 2024-04-13 04:32:41.810876 glitter_proto-0.6.0/glitter_proto/ibc/lightclients/tendermint/v1/__init__.py
+-rw-r--r--   0        0        0    10180 2024-04-13 04:32:41.811108 glitter_proto-0.6.0/glitter_proto/ics23/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 04:32:41.811254 glitter_proto-0.6.0/glitter_proto/tendermint/__init__.py
+-rw-r--r--   0        0        0    33422 2024-04-13 04:32:41.811373 glitter_proto-0.6.0/glitter_proto/tendermint/abci/__init__.py
+-rw-r--r--   0        0        0     1849 2024-04-13 04:32:41.811528 glitter_proto-0.6.0/glitter_proto/tendermint/crypto/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 04:32:41.811619 glitter_proto-0.6.0/glitter_proto/tendermint/libs/__init__.py
+-rw-r--r--   0        0        0      409 2024-04-13 04:32:41.811790 glitter_proto-0.6.0/glitter_proto/tendermint/libs/bits/__init__.py
+-rw-r--r--   0        0        0     1320 2024-04-13 04:32:41.812050 glitter_proto-0.6.0/glitter_proto/tendermint/p2p/__init__.py
+-rw-r--r--   0        0        0    11130 2024-04-13 04:32:41.812281 glitter_proto-0.6.0/glitter_proto/tendermint/types/__init__.py
+-rw-r--r--   0        0        0      949 2024-04-13 04:32:41.812498 glitter_proto-0.6.0/glitter_proto/tendermint/version/__init__.py
+-rw-r--r--   0        0        0      352 2024-04-13 04:30:01.153914 glitter_proto-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      564 1970-01-01 00:00:00.000000 glitter_proto-0.6.0/PKG-INFO
```

### Comparing `glitter_proto-0.5.0/glitter_proto/blockved/glitterchain/index/__init__.py` & `glitter_proto-0.6.0/glitter_proto/blockved/glitterchain/index/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -156,14 +156,57 @@
 
 @dataclass(eq=False, repr=False)
 class SqlGrantResponse(betterproto.Message):
     pass
 
 
 @dataclass(eq=False, repr=False)
+class SqlAnalyzerRequest(betterproto.Message):
+    uid: str = betterproto.string_field(1)
+    op_type: str = betterproto.string_field(2)
+    is_delete: bool = betterproto.bool_field(3)
+    token_filter: "TokenFilter" = betterproto.message_field(4)
+    tokenizer: "Tokenizer" = betterproto.message_field(5)
+    analyzer: "Analyzer" = betterproto.message_field(6)
+
+
+@dataclass(eq=False, repr=False)
+class TokenFilter(betterproto.Message):
+    token_filter_name: str = betterproto.string_field(1)
+    token_filter_en_name: str = betterproto.string_field(2)
+    token_filter_type: int = betterproto.int64_field(3)
+    dict_file_cid: str = betterproto.string_field(4)
+    comment: str = betterproto.string_field(5)
+
+
+@dataclass(eq=False, repr=False)
+class Tokenizer(betterproto.Message):
+    tokenizer_name: str = betterproto.string_field(1)
+    tokenizer_en_name: str = betterproto.string_field(2)
+    tokenizer_type: int = betterproto.int64_field(3)
+    dict_file_cid: str = betterproto.string_field(4)
+    comment: str = betterproto.string_field(5)
+
+
+@dataclass(eq=False, repr=False)
+class Analyzer(betterproto.Message):
+    analyzer_name: str = betterproto.string_field(1)
+    analyzer_en_name: str = betterproto.string_field(2)
+    char_filters: str = betterproto.string_field(3)
+    tokenizer: str = betterproto.string_field(4)
+    token_filters: str = betterproto.string_field(5)
+    comment: str = betterproto.string_field(6)
+
+
+@dataclass(eq=False, repr=False)
+class SqlAnalyzerResponse(betterproto.Message):
+    pass
+
+
+@dataclass(eq=False, repr=False)
 class Params(betterproto.Message):
     """Params defines the parameters for the module."""
 
     pass
 
 
 @dataclass(eq=False, repr=False)
@@ -457,14 +500,31 @@
             sql_grant_request,
             SqlGrantResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
+    async def sql_analyzer(
+        self,
+        sql_analyzer_request: "SqlAnalyzerRequest",
+        *,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None
+    ) -> "SqlAnalyzerResponse":
+        return await self._unary_unary(
+            "/blockved.glitterchain.index.Msg/SQLAnalyzer",
+            sql_analyzer_request,
+            SqlAnalyzerResponse,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        )
+
 
 class QueryStub(betterproto.ServiceStub):
     async def list_schema(
         self,
         list_schema_request: "ListSchemaRequest",
         *,
         timeout: Optional[float] = None,
@@ -645,14 +705,19 @@
         raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
 
     async def sql_grant(
         self, sql_grant_request: "SqlGrantRequest"
     ) -> "SqlGrantResponse":
         raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
 
+    async def sql_analyzer(
+        self, sql_analyzer_request: "SqlAnalyzerRequest"
+    ) -> "SqlAnalyzerResponse":
+        raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
+
     async def __rpc_manage_schema(
         self, stream: "grpclib.server.Stream[MsgSchema, MsgSchemaResponse]"
     ) -> None:
         request = await stream.recv_message()
         response = await self.manage_schema(request)
         await stream.send_message(response)
 
@@ -673,14 +738,21 @@
     async def __rpc_sql_grant(
         self, stream: "grpclib.server.Stream[SqlGrantRequest, SqlGrantResponse]"
     ) -> None:
         request = await stream.recv_message()
         response = await self.sql_grant(request)
         await stream.send_message(response)
 
+    async def __rpc_sql_analyzer(
+        self, stream: "grpclib.server.Stream[SqlAnalyzerRequest, SqlAnalyzerResponse]"
+    ) -> None:
+        request = await stream.recv_message()
+        response = await self.sql_analyzer(request)
+        await stream.send_message(response)
+
     def __mapping__(self) -> Dict[str, grpclib.const.Handler]:
         return {
             "/blockved.glitterchain.index.Msg/ManageSchema": grpclib.const.Handler(
                 self.__rpc_manage_schema,
                 grpclib.const.Cardinality.UNARY_UNARY,
                 MsgSchema,
                 MsgSchemaResponse,
@@ -699,14 +771,20 @@
             ),
             "/blockved.glitterchain.index.Msg/SQLGrant": grpclib.const.Handler(
                 self.__rpc_sql_grant,
                 grpclib.const.Cardinality.UNARY_UNARY,
                 SqlGrantRequest,
                 SqlGrantResponse,
             ),
+            "/blockved.glitterchain.index.Msg/SQLAnalyzer": grpclib.const.Handler(
+                self.__rpc_sql_analyzer,
+                grpclib.const.Cardinality.UNARY_UNARY,
+                SqlAnalyzerRequest,
+                SqlAnalyzerResponse,
+            ),
         }
 
 
 class QueryBase(ServiceBase):
     async def list_schema(
         self, list_schema_request: "ListSchemaRequest"
     ) -> "ListSchemaResponse":
```

### Comparing `glitter_proto-0.5.0/glitter_proto/cosmos/auth/v1beta1/__init__.py` & `glitter_proto-0.6.0/glitter_proto/cosmos/auth/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/cosmos/authz/v1beta1/__init__.py` & `glitter_proto-0.6.0/glitter_proto/cosmos/authz/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/cosmos/bank/v1beta1/__init__.py` & `glitter_proto-0.6.0/glitter_proto/cosmos/bank/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/cosmos/base/abci/v1beta1/__init__.py` & `glitter_proto-0.6.0/glitter_proto/cosmos/base/abci/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/cosmos/base/kv/v1beta1/__init__.py` & `glitter_proto-0.6.0/glitter_proto/cosmos/base/kv/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/cosmos/base/query/v1beta1/__init__.py` & `glitter_proto-0.6.0/glitter_proto/cosmos/base/query/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/cosmos/base/reflection/v1beta1/__init__.py` & `glitter_proto-0.6.0/glitter_proto/cosmos/base/reflection/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/cosmos/base/reflection/v2alpha1/__init__.py` & `glitter_proto-0.6.0/glitter_proto/cosmos/base/reflection/v2alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/cosmos/base/snapshots/v1beta1/__init__.py` & `glitter_proto-0.6.0/glitter_proto/cosmos/base/snapshots/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/cosmos/base/store/v1beta1/__init__.py` & `glitter_proto-0.6.0/glitter_proto/cosmos/base/store/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/cosmos/base/tendermint/v1beta1/__init__.py` & `glitter_proto-0.6.0/glitter_proto/cosmos/base/tendermint/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/cosmos/base/v1beta1/__init__.py` & `glitter_proto-0.6.0/glitter_proto/cosmos/base/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/cosmos/capability/v1beta1/__init__.py` & `glitter_proto-0.6.0/glitter_proto/cosmos/capability/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/cosmos/crisis/v1beta1/__init__.py` & `glitter_proto-0.6.0/glitter_proto/cosmos/crisis/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/cosmos/crypto/ed25519/__init__.py` & `glitter_proto-0.6.0/glitter_proto/cosmos/crypto/ed25519/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/cosmos/crypto/multisig/__init__.py` & `glitter_proto-0.6.0/glitter_proto/cosmos/crypto/multisig/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/cosmos/crypto/multisig/v1beta1/__init__.py` & `glitter_proto-0.6.0/glitter_proto/cosmos/crypto/multisig/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/cosmos/crypto/secp256k1/__init__.py` & `glitter_proto-0.6.0/glitter_proto/cosmos/crypto/secp256k1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/cosmos/crypto/secp256r1/__init__.py` & `glitter_proto-0.6.0/glitter_proto/cosmos/crypto/secp256r1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/cosmos/distribution/v1beta1/__init__.py` & `glitter_proto-0.6.0/glitter_proto/cosmos/distribution/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/cosmos/evidence/v1beta1/__init__.py` & `glitter_proto-0.6.0/glitter_proto/cosmos/evidence/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/cosmos/feegrant/v1beta1/__init__.py` & `glitter_proto-0.6.0/glitter_proto/cosmos/feegrant/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/cosmos/gov/v1beta1/__init__.py` & `glitter_proto-0.6.0/glitter_proto/cosmos/gov/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/cosmos/mint/v1beta1/__init__.py` & `glitter_proto-0.6.0/glitter_proto/cosmos/mint/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/cosmos/params/v1beta1/__init__.py` & `glitter_proto-0.6.0/glitter_proto/cosmos/params/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/cosmos/slashing/v1beta1/__init__.py` & `glitter_proto-0.6.0/glitter_proto/cosmos/slashing/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/cosmos/staking/v1beta1/__init__.py` & `glitter_proto-0.6.0/glitter_proto/cosmos/staking/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/cosmos/tx/signing/v1beta1/__init__.py` & `glitter_proto-0.6.0/glitter_proto/cosmos/tx/signing/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/cosmos/tx/v1beta1/__init__.py` & `glitter_proto-0.6.0/glitter_proto/cosmos/tx/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/cosmos/upgrade/v1beta1/__init__.py` & `glitter_proto-0.6.0/glitter_proto/cosmos/upgrade/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/cosmos/vesting/v1beta1/__init__.py` & `glitter_proto-0.6.0/glitter_proto/cosmos/vesting/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/cosmwasm/wasm/v1/__init__.py` & `glitter_proto-0.6.0/glitter_proto/cosmwasm/wasm/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/ethermint/crypto/v1/ethsecp256k1/__init__.py` & `glitter_proto-0.6.0/glitter_proto/ethermint/crypto/v1/ethsecp256k1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/ethermint/crypto/v1/ethsecp256k1/keys.proto` & `glitter_proto-0.6.0/glitter_proto/ethermint/crypto/v1/ethsecp256k1/keys.proto`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/ethermint/evm/v1/__init__.py` & `glitter_proto-0.6.0/glitter_proto/ethermint/evm/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/ethermint/evm/v1/evm.proto` & `glitter_proto-0.6.0/glitter_proto/ethermint/evm/v1/evm.proto`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/ethermint/evm/v1/genesis.proto` & `glitter_proto-0.6.0/glitter_proto/ethermint/evm/v1/genesis.proto`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/ethermint/evm/v1/query.proto` & `glitter_proto-0.6.0/glitter_proto/ethermint/evm/v1/query.proto`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/ethermint/evm/v1/tx.proto` & `glitter_proto-0.6.0/glitter_proto/ethermint/evm/v1/tx.proto`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/ethermint/feemarket/v1/__init__.py` & `glitter_proto-0.6.0/glitter_proto/ethermint/feemarket/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/ethermint/feemarket/v1/feemarket.proto` & `glitter_proto-0.6.0/glitter_proto/ethermint/feemarket/v1/feemarket.proto`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/ethermint/feemarket/v1/genesis.proto` & `glitter_proto-0.6.0/glitter_proto/ethermint/feemarket/v1/genesis.proto`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/ethermint/feemarket/v1/query.proto` & `glitter_proto-0.6.0/glitter_proto/ethermint/feemarket/v1/query.proto`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/ethermint/types/v1/__init__.py` & `glitter_proto-0.6.0/glitter_proto/ethermint/types/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/ethermint/types/v1/account.proto` & `glitter_proto-0.6.0/glitter_proto/ethermint/types/v1/account.proto`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/ethermint/types/v1/indexer.proto` & `glitter_proto-0.6.0/glitter_proto/ethermint/types/v1/indexer.proto`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/ethermint/types/v1/web3.proto` & `glitter_proto-0.6.0/glitter_proto/ethermint/types/v1/web3.proto`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/google/api/__init__.py` & `glitter_proto-0.6.0/glitter_proto/google/api/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/google/protobuf/compiler/__init__.py` & `glitter_proto-0.6.0/glitter_proto/google/protobuf/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/ibc/applications/fee/v1/__init__.py` & `glitter_proto-0.6.0/glitter_proto/ibc/applications/fee/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/ibc/applications/interchain_accounts/controller/v1/__init__.py` & `glitter_proto-0.6.0/glitter_proto/ibc/applications/interchain_accounts/controller/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/ibc/applications/interchain_accounts/host/v1/__init__.py` & `glitter_proto-0.6.0/glitter_proto/ibc/applications/interchain_accounts/host/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/ibc/applications/interchain_accounts/v1/__init__.py` & `glitter_proto-0.6.0/glitter_proto/ibc/applications/interchain_accounts/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/ibc/applications/transfer/v1/__init__.py` & `glitter_proto-0.6.0/glitter_proto/ibc/applications/transfer/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/ibc/applications/transfer/v2/__init__.py` & `glitter_proto-0.6.0/glitter_proto/ibc/applications/transfer/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/ibc/core/channel/v1/__init__.py` & `glitter_proto-0.6.0/glitter_proto/ibc/core/channel/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/ibc/core/client/v1/__init__.py` & `glitter_proto-0.6.0/glitter_proto/ibc/core/client/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/ibc/core/commitment/v1/__init__.py` & `glitter_proto-0.6.0/glitter_proto/ibc/core/commitment/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/ibc/core/connection/v1/__init__.py` & `glitter_proto-0.6.0/glitter_proto/ibc/core/connection/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/ibc/core/types/v1/__init__.py` & `glitter_proto-0.6.0/glitter_proto/ibc/core/types/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/ibc/lightclients/localhost/v1/__init__.py` & `glitter_proto-0.6.0/glitter_proto/ibc/lightclients/localhost/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/ibc/lightclients/solomachine/v1/__init__.py` & `glitter_proto-0.6.0/glitter_proto/ibc/lightclients/solomachine/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/ibc/lightclients/solomachine/v2/__init__.py` & `glitter_proto-0.6.0/glitter_proto/ibc/lightclients/solomachine/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/ibc/lightclients/tendermint/v1/__init__.py` & `glitter_proto-0.6.0/glitter_proto/ibc/lightclients/tendermint/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/ics23/__init__.py` & `glitter_proto-0.6.0/glitter_proto/ics23/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/tendermint/abci/__init__.py` & `glitter_proto-0.6.0/glitter_proto/tendermint/abci/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/tendermint/crypto/__init__.py` & `glitter_proto-0.6.0/glitter_proto/tendermint/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/tendermint/p2p/__init__.py` & `glitter_proto-0.6.0/glitter_proto/tendermint/p2p/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/tendermint/types/__init__.py` & `glitter_proto-0.6.0/glitter_proto/tendermint/types/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/glitter_proto/tendermint/version/__init__.py` & `glitter_proto-0.6.0/glitter_proto/tendermint/version/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.5.0/PKG-INFO` & `glitter_proto-0.6.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glitter-proto
-Version: 0.5.0
+Version: 0.6.0
 Summary: The proto files of glitter-chain
 Author: Glitter Protocol
 Author-email: ted@glitterprotocol.io
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

