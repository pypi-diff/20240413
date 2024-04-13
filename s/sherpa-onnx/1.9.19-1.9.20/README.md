# Comparing `tmp/sherpa-onnx-1.9.19.tar.gz` & `tmp/sherpa-onnx-1.9.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sherpa-onnx-1.9.19.tar", last modified: Sat Apr 13 10:59:17 2024, max compression
+gzip compressed data, was "sherpa-onnx-1.9.20.tar", last modified: Sat Apr 13 12:30:27 2024, max compression
```

## Comparing `sherpa-onnx-1.9.19.tar` & `sherpa-onnx-1.9.20.tar`

### file list

```diff
@@ -1,495 +1,495 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:59:17.664098 sherpa-onnx-1.9.19/
--rw-r--r--   0 runner    (1001) docker     (127)    10654 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-04-13 10:59:17.664098 sherpa-onnx-1.9.19/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:59:17.592097 sherpa-onnx-1.9.19/c-api-examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/c-api-examples/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/c-api-examples/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:59:17.592097 sherpa-onnx-1.9.19/c-api-examples/asr-microphone-example/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/c-api-examples/asr-microphone-example/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/c-api-examples/asr-microphone-example/CPPLINT.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/c-api-examples/asr-microphone-example/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/c-api-examples/asr-microphone-example/alsa.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/c-api-examples/asr-microphone-example/alsa.h
--rw-r--r--   0 runner    (1001) docker     (127)     7252 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/c-api-examples/asr-microphone-example/c-api-alsa.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/c-api-examples/audio-tagging-c-api.c
--rw-r--r--   0 runner    (1001) docker     (127)     7060 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/c-api-examples/decode-file-c-api.c
--rw-r--r--   0 runner    (1001) docker     (127)     7720 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/c-api-examples/offline-tts-c-api.c
--rwxr-xr-x   0 runner    (1001) docker     (127)     1952 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/c-api-examples/run.sh
--rw-r--r--   0 runner    (1001) docker     (127)     8117 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/c-api-examples/speaker-identification-c-api.c
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/c-api-examples/spoken-language-identification-c-api.c
--rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/c-api-examples/streaming-hlg-decode-file-c-api.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:59:17.596097 sherpa-onnx-1.9.19/cmake/
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/cmake/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/cmake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/cmake/asio.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/cmake/cargs.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     7281 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/cmake/cmake_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/cmake/eigen.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/cmake/espeak-ng-for-piper.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/cmake/googletest.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/cmake/kaldi-decoder.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/cmake/kaldi-native-fbank.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/cmake/kaldifst.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/cmake/onnxruntime-linux-aarch64-static.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/cmake/onnxruntime-linux-aarch64.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/cmake/onnxruntime-linux-arm-static.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/cmake/onnxruntime-linux-arm.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/cmake/onnxruntime-linux-riscv64-static.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/cmake/onnxruntime-linux-riscv64.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     3712 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/cmake/onnxruntime-linux-x86_64-gpu.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/cmake/onnxruntime-linux-x86_64-static.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/cmake/onnxruntime-linux-x86_64.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/cmake/onnxruntime-osx-arm64-static.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/cmake/onnxruntime-osx-arm64.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/cmake/onnxruntime-osx-universal-static.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/cmake/onnxruntime-osx-universal.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/cmake/onnxruntime-osx-x86_64-static.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/cmake/onnxruntime-osx-x86_64.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/cmake/onnxruntime-wasm-simd.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/cmake/onnxruntime-win-x64-gpu.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/cmake/onnxruntime-win-x64-static-debug.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/cmake/onnxruntime-win-x64-static.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/cmake/onnxruntime-win-x64.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/cmake/onnxruntime-win-x86-static-debug.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/cmake/onnxruntime-win-x86-static.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/cmake/onnxruntime-win-x86.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     7797 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/cmake/onnxruntime.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/cmake/openfst.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/cmake/piper-phonemize.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/cmake/portaudio.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/cmake/pybind11.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/cmake/sherpa-onnx-no-tts.pc.in
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/cmake/sherpa-onnx.pc.in
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/cmake/websocketpp.cmake
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 10:59:17.664098 sherpa-onnx-1.9.19/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:59:17.600097 sherpa-onnx-1.9.19/sherpa-onnx/
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:59:17.600097 sherpa-onnx-1.9.19/sherpa-onnx/c-api/
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/c-api/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)    40773 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/c-api/c-api.cc
--rw-r--r--   0 runner    (1001) docker     (127)    44392 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/c-api/c-api.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:59:17.648098 sherpa-onnx-1.9.19/sherpa-onnx/csrc/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    15121 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/CPPLINT.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/alsa-play.cc
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/alsa-play.h
--rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/alsa.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/alsa.h
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/audio-tagging-impl.cc
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/audio-tagging-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/audio-tagging-label-file.cc
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/audio-tagging-label-file.h
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/audio-tagging-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/audio-tagging-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/audio-tagging-zipformer-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/audio-tagging.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/audio-tagging.h
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/base64-decode.cc
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/base64-decode.h
--rw-r--r--   0 runner    (1001) docker     (127)     7523 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/cat-test.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/cat.cc
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/cat.h
--rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/circular-buffer-test.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4782 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/circular-buffer.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/circular-buffer.h
--rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/context-graph-test.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/context-graph.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/context-graph.h
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/display.h
--rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/endpoint.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/endpoint.h
--rw-r--r--   0 runner    (1001) docker     (127)     6929 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/features.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/features.h
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/file-utils.cc
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/file-utils.h
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/hypothesis.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/hypothesis.h
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/keyword-spotter-impl.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/keyword-spotter-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)    11531 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/keyword-spotter-transducer-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     4412 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/keyword-spotter.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/keyword-spotter.h
--rw-r--r--   0 runner    (1001) docker     (127)     9821 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/lexicon.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/lexicon.h
--rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/log.cc
--rw-r--r--   0 runner    (1001) docker     (127)    11480 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/log.h
--rw-r--r--   0 runner    (1001) docker     (127)    10445 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/macros.h
--rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/math.h
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/microphone.cc
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/microphone.h
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-ct-transformer-model-meta-data.h
--rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-ct-transformer-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-ct-transformer-model.h
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-ctc-decoder.h
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-ctc-fst-decoder-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-ctc-fst-decoder-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-ctc-fst-decoder.cc
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-ctc-fst-decoder.h
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-ctc-greedy-search-decoder.cc
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-ctc-greedy-search-decoder.h
--rw-r--r--   0 runner    (1001) docker     (127)     5187 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-ctc-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-ctc-model.h
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-lm-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-lm-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-lm.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-lm.h
--rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-nemo-enc-dec-ctc-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-nemo-enc-dec-ctc-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-nemo-enc-dec-ctc-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-nemo-enc-dec-ctc-model.h
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-paraformer-decoder.h
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-paraformer-greedy-search-decoder.cc
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-paraformer-greedy-search-decoder.h
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-paraformer-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-paraformer-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-paraformer-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-paraformer-model.h
--rw-r--r--   0 runner    (1001) docker     (127)     5223 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-punctuation-ct-transformer-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-punctuation-impl.cc
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-punctuation-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-punctuation-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-punctuation-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-punctuation.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-punctuation.h
--rw-r--r--   0 runner    (1001) docker     (127)     8003 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-recognizer-ctc-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)    10422 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-recognizer-impl.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-recognizer-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     8284 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-recognizer-paraformer-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     7881 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-recognizer-transducer-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-recognizer-whisper-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-recognizer.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-recognizer.h
--rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-rnn-lm.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-rnn-lm.h
--rw-r--r--   0 runner    (1001) docker     (127)     9147 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-stream.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-stream.h
--rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-tdnn-ctc-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-tdnn-ctc-model.h
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-tdnn-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-tdnn-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-transducer-decoder.h
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-transducer-greedy-search-decoder.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-transducer-greedy-search-decoder.h
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-transducer-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-transducer-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     9835 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-transducer-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-transducer-model.h
--rw-r--r--   0 runner    (1001) docker     (127)     6183 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-transducer-modified-beam-search-decoder.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-transducer-modified-beam-search-decoder.h
--rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-tts-character-frontend.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-tts-character-frontend.h
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-tts-frontend.h
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-tts-impl.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-tts-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-tts-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-tts-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)    12205 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-tts-vits-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-tts-vits-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-tts-vits-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-tts-vits-model-metadata.h
--rw-r--r--   0 runner    (1001) docker     (127)     8924 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-tts-vits-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-tts-vits-model.h
--rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-tts.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-tts.h
--rw-r--r--   0 runner    (1001) docker     (127)     9471 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-websocket-server-impl.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6835 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-websocket-server-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-websocket-server.cc
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-wenet-ctc-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-wenet-ctc-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-wenet-ctc-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-wenet-ctc-model.h
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-whisper-decoder.h
--rw-r--r--   0 runner    (1001) docker     (127)     4604 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-whisper-greedy-search-decoder.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-whisper-greedy-search-decoder.h
--rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-whisper-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-whisper-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)    14260 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-whisper-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-whisper-model.h
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-zipformer-audio-tagging-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-zipformer-audio-tagging-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-zipformer-audio-tagging-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-zipformer-audio-tagging-model.h
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-zipformer-ctc-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-zipformer-ctc-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-zipformer-ctc-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-zipformer-ctc-model.h
--rw-r--r--   0 runner    (1001) docker     (127)     9094 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-conformer-transducer-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-conformer-transducer-model.h
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-ctc-decoder.h
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-ctc-fst-decoder-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-ctc-fst-decoder-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-ctc-fst-decoder.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-ctc-fst-decoder.h
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-ctc-greedy-search-decoder.cc
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-ctc-greedy-search-decoder.h
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-ctc-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-ctc-model.h
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-lm-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-lm-config.h
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-lm.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-lm.h
--rw-r--r--   0 runner    (1001) docker     (127)     8601 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-lstm-transducer-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-lstm-transducer-model.h
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-paraformer-decoder.h
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-paraformer-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-paraformer-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     8223 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-paraformer-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-paraformer-model.h
--rw-r--r--   0 runner    (1001) docker     (127)     9936 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-recognizer-ctc-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-recognizer-impl.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-recognizer-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)    14461 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-recognizer-paraformer-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)    12666 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-recognizer-transducer-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     6172 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-recognizer.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5811 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-recognizer.h
--rw-r--r--   0 runner    (1001) docker     (127)     5599 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-rnn-lm.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-rnn-lm.h
--rw-r--r--   0 runner    (1001) docker     (127)     7318 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-stream.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-stream.h
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-transducer-decoder.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-transducer-decoder.h
--rw-r--r--   0 runner    (1001) docker     (127)     5610 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-transducer-greedy-search-decoder.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-transducer-greedy-search-decoder.h
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-transducer-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-transducer-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     6821 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-transducer-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-transducer-model.h
--rw-r--r--   0 runner    (1001) docker     (127)     8410 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-transducer-modified-beam-search-decoder.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-transducer-modified-beam-search-decoder.h
--rw-r--r--   0 runner    (1001) docker     (127)     8504 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-websocket-client.cc
--rw-r--r--   0 runner    (1001) docker     (127)    10312 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-websocket-server-impl.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5138 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-websocket-server-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-websocket-server.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-wenet-ctc-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-wenet-ctc-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     8208 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-wenet-ctc-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-wenet-ctc-model.h
--rw-r--r--   0 runner    (1001) docker     (127)    15426 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-zipformer-transducer-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-zipformer-transducer-model.h
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-zipformer2-ctc-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-zipformer2-ctc-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)    13906 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-zipformer2-ctc-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-zipformer2-ctc-model.h
--rw-r--r--   0 runner    (1001) docker     (127)    14574 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-zipformer2-transducer-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-zipformer2-transducer-model.h
--rw-r--r--   0 runner    (1001) docker     (127)    10500 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/onnx-utils.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/onnx-utils.h
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/packed-sequence-test.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/packed-sequence.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/packed-sequence.h
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/pad-sequence-test.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/pad-sequence.cc
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/pad-sequence.h
--rw-r--r--   0 runner    (1001) docker     (127)    23979 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/parse-options.cc
--rw-r--r--   0 runner    (1001) docker     (127)    10321 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/parse-options.h
--rw-r--r--   0 runner    (1001) docker     (127)     6904 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/piper-phonemize-lexicon.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/piper-phonemize-lexicon.h
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/piper-phonemize-test.cc
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/provider.cc
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/provider.h
--rw-r--r--   0 runner    (1001) docker     (127)    12517 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/resample.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6695 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/resample.h
--rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/session.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/session.h
--rw-r--r--   0 runner    (1001) docker     (127)     5110 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/sherpa-onnx-alsa-offline-audio-tagging.cc
--rw-r--r--   0 runner    (1001) docker     (127)     7781 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/sherpa-onnx-alsa-offline-speaker-identification.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/sherpa-onnx-alsa-offline.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/sherpa-onnx-alsa.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/sherpa-onnx-keyword-spotter-alsa.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/sherpa-onnx-keyword-spotter-microphone.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3322 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/sherpa-onnx-keyword-spotter.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6764 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/sherpa-onnx-microphone-offline-audio-tagging.cc
--rw-r--r--   0 runner    (1001) docker     (127)     9546 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/sherpa-onnx-microphone-offline-speaker-identification.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6802 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/sherpa-onnx-microphone-offline.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5422 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/sherpa-onnx-microphone.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/sherpa-onnx-offline-audio-tagging.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/sherpa-onnx-offline-language-identification.cc
--rw-r--r--   0 runner    (1001) docker     (127)    10267 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/sherpa-onnx-offline-parallel.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/sherpa-onnx-offline-punctuation.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6382 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/sherpa-onnx-offline-tts-play-alsa.cc
--rw-r--r--   0 runner    (1001) docker     (127)     9362 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/sherpa-onnx-offline-tts-play.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/sherpa-onnx-offline-tts.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/sherpa-onnx-offline.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/sherpa-onnx-vad-alsa.cc
--rw-r--r--   0 runner    (1001) docker     (127)     7215 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/sherpa-onnx-vad-microphone-offline-asr.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6436 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/sherpa-onnx-vad-microphone.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5558 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/sherpa-onnx.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/silero-vad-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/silero-vad-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     8246 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/silero-vad-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/silero-vad-model.h
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/slice-test.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/slice.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/slice.h
--rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/speaker-embedding-extractor-general-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/speaker-embedding-extractor-impl.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/speaker-embedding-extractor-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/speaker-embedding-extractor-model-meta-data.h
--rw-r--r--   0 runner    (1001) docker     (127)     4095 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/speaker-embedding-extractor-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/speaker-embedding-extractor-model.h
--rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/speaker-embedding-extractor-nemo-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/speaker-embedding-extractor-nemo-model-meta-data.h
--rw-r--r--   0 runner    (1001) docker     (127)     4733 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/speaker-embedding-extractor-nemo-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/speaker-embedding-extractor-nemo-model.h
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/speaker-embedding-extractor.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/speaker-embedding-extractor.h
--rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/speaker-embedding-manager-test.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5842 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/speaker-embedding-manager.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/speaker-embedding-manager.h
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/spoken-language-identification-impl.cc
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/spoken-language-identification-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/spoken-language-identification-whisper-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/spoken-language-identification.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/spoken-language-identification.h
--rw-r--r--   0 runner    (1001) docker     (127)     7388 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/stack-test.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/stack.cc
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/stack.h
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/symbol-table.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/symbol-table.h
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/tee-stream.h
--rw-r--r--   0 runner    (1001) docker     (127)    10670 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/text-utils.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/text-utils.h
--rw-r--r--   0 runner    (1001) docker     (127)     6484 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/transducer-keyword-decoder.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/transducer-keyword-decoder.h
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/transpose-test.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/transpose.cc
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/transpose.h
--rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/unbind-test.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/unbind.cc
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/unbind.h
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/utfcpp-test.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/utils.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/utils.h
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/vad-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/vad-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/vad-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/vad-model.h
--rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/voice-activity-detector.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/voice-activity-detector.h
--rw-r--r--   0 runner    (1001) docker     (127)     4454 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/wave-reader.cc
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/wave-reader.h
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/wave-writer.cc
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/csrc/wave-writer.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:59:17.648098 sherpa-onnx-1.9.19/sherpa-onnx/jni/
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/jni/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)    71560 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/jni/jni.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:59:17.648098 sherpa-onnx-1.9.19/sherpa-onnx/python/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:59:17.660098 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/alsa.cc
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/alsa.h
--rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/audio-tagging.cc
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/audio-tagging.h
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/circular-buffer.cc
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/circular-buffer.h
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/display.cc
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/display.h
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/endpoint.cc
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/endpoint.h
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/faked-alsa.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/features.cc
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/features.h
--rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/keyword-spotter.cc
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/keyword-spotter.h
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/offline-ctc-fst-decoder-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/offline-ctc-fst-decoder-config.h
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/offline-lm-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/offline-lm-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/offline-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/offline-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/offline-nemo-enc-dec-ctc-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/offline-nemo-enc-dec-ctc-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/offline-paraformer-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/offline-paraformer-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/offline-punctuation.cc
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/offline-punctuation.h
--rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/offline-recognizer.cc
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/offline-recognizer.h
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/offline-stream.cc
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/offline-stream.h
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/offline-tdnn-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/offline-tdnn-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/offline-transducer-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/offline-transducer-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/offline-tts-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/offline-tts-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/offline-tts-vits-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/offline-tts-vits-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/offline-tts.cc
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/offline-tts.h
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/offline-wenet-ctc-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/offline-wenet-ctc-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/offline-whisper-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/offline-whisper-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/offline-zipformer-ctc-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/offline-zipformer-ctc-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/online-ctc-fst-decoder-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/online-ctc-fst-decoder-config.h
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/online-lm-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/online-lm-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/online-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/online-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/online-paraformer-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/online-paraformer-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/online-recognizer.cc
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/online-recognizer.h
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/online-stream.cc
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/online-stream.h
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/online-transducer-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/online-transducer-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/online-wenet-ctc-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/online-wenet-ctc-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/online-zipformer2-ctc-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/online-zipformer2-ctc-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/sherpa-onnx.cc
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/sherpa-onnx.h
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/silero-vad-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/silero-vad-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/speaker-embedding-extractor.cc
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/speaker-embedding-extractor.h
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/speaker-embedding-manager.cc
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/speaker-embedding-manager.h
--rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/spoken-language-identification.cc
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/spoken-language-identification.h
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/vad-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/vad-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/vad-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/vad-model.h
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/voice-activity-detector.cc
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/voice-activity-detector.h
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/wave-writer.cc
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/wave-writer.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:59:17.664098 sherpa-onnx-1.9.19/sherpa-onnx/python/sherpa_onnx/
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-13 10:59:17.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/sherpa_onnx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/sherpa_onnx/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4956 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/sherpa_onnx/keyword_spotter.py
--rw-r--r--   0 runner    (1001) docker     (127)    15670 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/sherpa_onnx/offline_recognizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    20336 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/sherpa_onnx/online_recognizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/sherpa_onnx/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:59:17.664098 sherpa-onnx-1.9.19/sherpa-onnx/python/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/tests/CMakeLists.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      851 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/tests/test_feature_extractor_config.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7548 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/tests/test_keyword_spotter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12338 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/tests/test_offline_recognizer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10928 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/tests/test_online_recognizer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      772 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/tests/test_online_transducer_model_config.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7132 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/tests/test_speaker_recognition.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3905 2024-04-13 10:49:51.000000 sherpa-onnx-1.9.19/sherpa-onnx/python/tests/test_text2token.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:59:17.664098 sherpa-onnx-1.9.19/sherpa_onnx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-04-13 10:59:17.000000 sherpa-onnx-1.9.19/sherpa_onnx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20346 2024-04-13 10:59:17.000000 sherpa-onnx-1.9.19/sherpa_onnx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 10:59:17.000000 sherpa-onnx-1.9.19/sherpa_onnx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-13 10:59:17.000000 sherpa-onnx-1.9.19/sherpa_onnx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 10:59:17.000000 sherpa-onnx-1.9.19/sherpa_onnx.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-13 10:59:17.000000 sherpa-onnx-1.9.19/sherpa_onnx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 12:30:27.652385 sherpa-onnx-1.9.20/
+-rw-r--r--   0 runner    (1001) docker     (127)    10654 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-04-13 12:30:27.652385 sherpa-onnx-1.9.20/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 12:30:27.588384 sherpa-onnx-1.9.20/c-api-examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/c-api-examples/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/c-api-examples/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 12:30:27.588384 sherpa-onnx-1.9.20/c-api-examples/asr-microphone-example/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/c-api-examples/asr-microphone-example/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/c-api-examples/asr-microphone-example/CPPLINT.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/c-api-examples/asr-microphone-example/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/c-api-examples/asr-microphone-example/alsa.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/c-api-examples/asr-microphone-example/alsa.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7252 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/c-api-examples/asr-microphone-example/c-api-alsa.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/c-api-examples/audio-tagging-c-api.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7060 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/c-api-examples/decode-file-c-api.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7720 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/c-api-examples/offline-tts-c-api.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1952 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/c-api-examples/run.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     8117 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/c-api-examples/speaker-identification-c-api.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/c-api-examples/spoken-language-identification-c-api.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/c-api-examples/streaming-hlg-decode-file-c-api.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 12:30:27.596384 sherpa-onnx-1.9.20/cmake/
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/cmake/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/cmake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/cmake/asio.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/cmake/cargs.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     7281 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/cmake/cmake_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/cmake/eigen.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/cmake/espeak-ng-for-piper.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/cmake/googletest.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/cmake/kaldi-decoder.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/cmake/kaldi-native-fbank.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/cmake/kaldifst.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/cmake/onnxruntime-linux-aarch64-static.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/cmake/onnxruntime-linux-aarch64.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/cmake/onnxruntime-linux-arm-static.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/cmake/onnxruntime-linux-arm.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/cmake/onnxruntime-linux-riscv64-static.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/cmake/onnxruntime-linux-riscv64.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     3712 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/cmake/onnxruntime-linux-x86_64-gpu.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/cmake/onnxruntime-linux-x86_64-static.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/cmake/onnxruntime-linux-x86_64.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/cmake/onnxruntime-osx-arm64-static.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/cmake/onnxruntime-osx-arm64.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/cmake/onnxruntime-osx-universal-static.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/cmake/onnxruntime-osx-universal.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/cmake/onnxruntime-osx-x86_64-static.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/cmake/onnxruntime-osx-x86_64.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/cmake/onnxruntime-wasm-simd.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/cmake/onnxruntime-win-x64-gpu.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/cmake/onnxruntime-win-x64-static-debug.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/cmake/onnxruntime-win-x64-static.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/cmake/onnxruntime-win-x64.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/cmake/onnxruntime-win-x86-static-debug.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/cmake/onnxruntime-win-x86-static.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/cmake/onnxruntime-win-x86.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     7797 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/cmake/onnxruntime.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/cmake/openfst.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/cmake/piper-phonemize.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/cmake/portaudio.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/cmake/pybind11.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/cmake/sherpa-onnx-no-tts.pc.in
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/cmake/sherpa-onnx.pc.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/cmake/websocketpp.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 12:30:27.652385 sherpa-onnx-1.9.20/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 12:30:27.596384 sherpa-onnx-1.9.20/sherpa-onnx/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 12:30:27.596384 sherpa-onnx-1.9.20/sherpa-onnx/c-api/
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/c-api/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    40773 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/c-api/c-api.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    44392 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/c-api/c-api.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 12:30:27.640385 sherpa-onnx-1.9.20/sherpa-onnx/csrc/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    15121 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/CPPLINT.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/alsa-play.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/alsa-play.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/alsa.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/alsa.h
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/audio-tagging-impl.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/audio-tagging-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/audio-tagging-label-file.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/audio-tagging-label-file.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/audio-tagging-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/audio-tagging-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/audio-tagging-zipformer-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/audio-tagging.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/audio-tagging.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/base64-decode.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/base64-decode.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7523 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/cat-test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/cat.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/cat.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/circular-buffer-test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4782 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/circular-buffer.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/circular-buffer.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/context-graph-test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/context-graph.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/context-graph.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/display.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/endpoint.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/endpoint.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6929 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/features.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/features.h
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/file-utils.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/file-utils.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/hypothesis.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/hypothesis.h
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/keyword-spotter-impl.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/keyword-spotter-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11531 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/keyword-spotter-transducer-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4412 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/keyword-spotter.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/keyword-spotter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9821 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/lexicon.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/lexicon.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/log.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    11480 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/log.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10445 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/macros.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/math.h
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/microphone.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/microphone.h
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-ct-transformer-model-meta-data.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-ct-transformer-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-ct-transformer-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-ctc-decoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-ctc-fst-decoder-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-ctc-fst-decoder-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-ctc-fst-decoder.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-ctc-fst-decoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-ctc-greedy-search-decoder.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-ctc-greedy-search-decoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5187 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-ctc-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-ctc-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-lm-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-lm-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-lm.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-lm.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-nemo-enc-dec-ctc-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-nemo-enc-dec-ctc-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-nemo-enc-dec-ctc-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-nemo-enc-dec-ctc-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-paraformer-decoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-paraformer-greedy-search-decoder.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-paraformer-greedy-search-decoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-paraformer-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-paraformer-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-paraformer-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-paraformer-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5689 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-punctuation-ct-transformer-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-punctuation-impl.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-punctuation-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-punctuation-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-punctuation-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-punctuation.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-punctuation.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8003 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-recognizer-ctc-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10422 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-recognizer-impl.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-recognizer-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8284 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-recognizer-paraformer-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7881 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-recognizer-transducer-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-recognizer-whisper-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-recognizer.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-recognizer.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-rnn-lm.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-rnn-lm.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9147 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-stream.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-stream.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-tdnn-ctc-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-tdnn-ctc-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-tdnn-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-tdnn-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-transducer-decoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-transducer-greedy-search-decoder.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-transducer-greedy-search-decoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-transducer-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-transducer-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9835 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-transducer-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-transducer-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6183 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-transducer-modified-beam-search-decoder.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-transducer-modified-beam-search-decoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-tts-character-frontend.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-tts-character-frontend.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-tts-frontend.h
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-tts-impl.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-tts-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-tts-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-tts-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12205 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-tts-vits-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-tts-vits-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-tts-vits-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-tts-vits-model-metadata.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8924 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-tts-vits-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-tts-vits-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-tts.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-tts.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9471 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-websocket-server-impl.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6835 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-websocket-server-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-websocket-server.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-wenet-ctc-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-wenet-ctc-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-wenet-ctc-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-wenet-ctc-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-whisper-decoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4604 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-whisper-greedy-search-decoder.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-whisper-greedy-search-decoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-whisper-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-whisper-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14260 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-whisper-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-whisper-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-zipformer-audio-tagging-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-zipformer-audio-tagging-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-zipformer-audio-tagging-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-zipformer-audio-tagging-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-zipformer-ctc-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-zipformer-ctc-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-zipformer-ctc-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-zipformer-ctc-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9094 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-conformer-transducer-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-conformer-transducer-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-ctc-decoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-ctc-fst-decoder-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-ctc-fst-decoder-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-ctc-fst-decoder.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-ctc-fst-decoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-ctc-greedy-search-decoder.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-ctc-greedy-search-decoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-ctc-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-ctc-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-lm-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-lm-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-lm.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-lm.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8601 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-lstm-transducer-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-lstm-transducer-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-paraformer-decoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-paraformer-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-paraformer-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8223 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-paraformer-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-paraformer-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9936 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-recognizer-ctc-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-recognizer-impl.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-recognizer-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14461 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-recognizer-paraformer-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12666 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-recognizer-transducer-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6172 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-recognizer.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5811 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-recognizer.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5599 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-rnn-lm.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-rnn-lm.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7318 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-stream.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-stream.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-transducer-decoder.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-transducer-decoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5610 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-transducer-greedy-search-decoder.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-transducer-greedy-search-decoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-transducer-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-transducer-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6821 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-transducer-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-transducer-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8410 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-transducer-modified-beam-search-decoder.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-transducer-modified-beam-search-decoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8504 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-websocket-client.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    10312 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-websocket-server-impl.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5138 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-websocket-server-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-websocket-server.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-wenet-ctc-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-wenet-ctc-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8208 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-wenet-ctc-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-wenet-ctc-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15426 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-zipformer-transducer-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-zipformer-transducer-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-zipformer2-ctc-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-zipformer2-ctc-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13906 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-zipformer2-ctc-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-zipformer2-ctc-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14574 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-zipformer2-transducer-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-zipformer2-transducer-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10500 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/onnx-utils.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/onnx-utils.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/packed-sequence-test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/packed-sequence.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/packed-sequence.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/pad-sequence-test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/pad-sequence.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/pad-sequence.h
+-rw-r--r--   0 runner    (1001) docker     (127)    23979 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/parse-options.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    10321 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/parse-options.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6904 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/piper-phonemize-lexicon.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/piper-phonemize-lexicon.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/piper-phonemize-test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/provider.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/provider.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12517 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/resample.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6695 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/resample.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/session.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/session.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5110 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/sherpa-onnx-alsa-offline-audio-tagging.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     7781 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/sherpa-onnx-alsa-offline-speaker-identification.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/sherpa-onnx-alsa-offline.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/sherpa-onnx-alsa.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/sherpa-onnx-keyword-spotter-alsa.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/sherpa-onnx-keyword-spotter-microphone.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3322 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/sherpa-onnx-keyword-spotter.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6764 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/sherpa-onnx-microphone-offline-audio-tagging.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     9546 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/sherpa-onnx-microphone-offline-speaker-identification.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6802 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/sherpa-onnx-microphone-offline.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5422 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/sherpa-onnx-microphone.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/sherpa-onnx-offline-audio-tagging.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/sherpa-onnx-offline-language-identification.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    10267 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/sherpa-onnx-offline-parallel.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/sherpa-onnx-offline-punctuation.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6382 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/sherpa-onnx-offline-tts-play-alsa.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     9362 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/sherpa-onnx-offline-tts-play.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/sherpa-onnx-offline-tts.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/sherpa-onnx-offline.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/sherpa-onnx-vad-alsa.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     7215 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/sherpa-onnx-vad-microphone-offline-asr.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6436 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/sherpa-onnx-vad-microphone.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5558 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/sherpa-onnx.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/silero-vad-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/silero-vad-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8246 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/silero-vad-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/silero-vad-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/slice-test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/slice.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/slice.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/speaker-embedding-extractor-general-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/speaker-embedding-extractor-impl.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/speaker-embedding-extractor-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/speaker-embedding-extractor-model-meta-data.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4095 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/speaker-embedding-extractor-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/speaker-embedding-extractor-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/speaker-embedding-extractor-nemo-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/speaker-embedding-extractor-nemo-model-meta-data.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4733 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/speaker-embedding-extractor-nemo-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/speaker-embedding-extractor-nemo-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/speaker-embedding-extractor.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/speaker-embedding-extractor.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/speaker-embedding-manager-test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5842 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/speaker-embedding-manager.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/speaker-embedding-manager.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/spoken-language-identification-impl.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/spoken-language-identification-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/spoken-language-identification-whisper-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/spoken-language-identification.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/spoken-language-identification.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7388 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/stack-test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/stack.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/stack.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/symbol-table.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/symbol-table.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/tee-stream.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10670 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/text-utils.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/text-utils.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6484 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/transducer-keyword-decoder.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/transducer-keyword-decoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/transpose-test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/transpose.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/transpose.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/unbind-test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/unbind.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/unbind.h
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/utfcpp-test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/utils.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/utils.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/vad-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/vad-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/vad-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/vad-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/voice-activity-detector.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/voice-activity-detector.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4454 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/wave-reader.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/wave-reader.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/wave-writer.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/csrc/wave-writer.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 12:30:27.640385 sherpa-onnx-1.9.20/sherpa-onnx/jni/
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/jni/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    71560 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/jni/jni.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 12:30:27.640385 sherpa-onnx-1.9.20/sherpa-onnx/python/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 12:30:27.652385 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/alsa.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/alsa.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/audio-tagging.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/audio-tagging.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/circular-buffer.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/circular-buffer.h
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/display.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/display.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/endpoint.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/endpoint.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/faked-alsa.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/features.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/features.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/keyword-spotter.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/keyword-spotter.h
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/offline-ctc-fst-decoder-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/offline-ctc-fst-decoder-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/offline-lm-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/offline-lm-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/offline-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/offline-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/offline-nemo-enc-dec-ctc-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/offline-nemo-enc-dec-ctc-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/offline-paraformer-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/offline-paraformer-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/offline-punctuation.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/offline-punctuation.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/offline-recognizer.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/offline-recognizer.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/offline-stream.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/offline-stream.h
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/offline-tdnn-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/offline-tdnn-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/offline-transducer-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/offline-transducer-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/offline-tts-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/offline-tts-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/offline-tts-vits-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/offline-tts-vits-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/offline-tts.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/offline-tts.h
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/offline-wenet-ctc-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/offline-wenet-ctc-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/offline-whisper-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/offline-whisper-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/offline-zipformer-ctc-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/offline-zipformer-ctc-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/online-ctc-fst-decoder-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/online-ctc-fst-decoder-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/online-lm-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/online-lm-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/online-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/online-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/online-paraformer-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/online-paraformer-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/online-recognizer.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/online-recognizer.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/online-stream.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/online-stream.h
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/online-transducer-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/online-transducer-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/online-wenet-ctc-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/online-wenet-ctc-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/online-zipformer2-ctc-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/online-zipformer2-ctc-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/sherpa-onnx.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/sherpa-onnx.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/silero-vad-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/silero-vad-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/speaker-embedding-extractor.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/speaker-embedding-extractor.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/speaker-embedding-manager.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/speaker-embedding-manager.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/spoken-language-identification.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/spoken-language-identification.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/vad-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/vad-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/vad-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/vad-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/voice-activity-detector.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/voice-activity-detector.h
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/wave-writer.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/wave-writer.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 12:30:27.652385 sherpa-onnx-1.9.20/sherpa-onnx/python/sherpa_onnx/
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-13 12:30:27.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/sherpa_onnx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/sherpa_onnx/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4956 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/sherpa_onnx/keyword_spotter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15670 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/sherpa_onnx/offline_recognizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20336 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/sherpa_onnx/online_recognizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/sherpa_onnx/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 12:30:27.652385 sherpa-onnx-1.9.20/sherpa-onnx/python/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/tests/CMakeLists.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      851 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/tests/test_feature_extractor_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7548 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/tests/test_keyword_spotter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12338 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/tests/test_offline_recognizer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10928 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/tests/test_online_recognizer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      772 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/tests/test_online_transducer_model_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7132 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/tests/test_speaker_recognition.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3905 2024-04-13 12:20:31.000000 sherpa-onnx-1.9.20/sherpa-onnx/python/tests/test_text2token.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 12:30:27.652385 sherpa-onnx-1.9.20/sherpa_onnx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-04-13 12:30:27.000000 sherpa-onnx-1.9.20/sherpa_onnx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20346 2024-04-13 12:30:27.000000 sherpa-onnx-1.9.20/sherpa_onnx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 12:30:27.000000 sherpa-onnx-1.9.20/sherpa_onnx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-13 12:30:27.000000 sherpa-onnx-1.9.20/sherpa_onnx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 12:30:27.000000 sherpa-onnx-1.9.20/sherpa_onnx.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-13 12:30:27.000000 sherpa-onnx-1.9.20/sherpa_onnx.egg-info/top_level.txt
```

### Comparing `sherpa-onnx-1.9.19/CMakeLists.txt` & `sherpa-onnx-1.9.20/CMakeLists.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 cmake_minimum_required(VERSION 3.13 FATAL_ERROR)
 project(sherpa-onnx)
 
-set(SHERPA_ONNX_VERSION "1.9.19")
+set(SHERPA_ONNX_VERSION "1.9.20")
 
 # Disable warning about
 #
 # "The DOWNLOAD_EXTRACT_TIMESTAMP option was not given and policy CMP0135 is
 #  not set.
 if (CMAKE_VERSION VERSION_GREATER_EQUAL "3.24.0")
   cmake_policy(SET CMP0135 NEW)
```

### Comparing `sherpa-onnx-1.9.19/LICENSE` & `sherpa-onnx-1.9.20/LICENSE`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/PKG-INFO` & `sherpa-onnx-1.9.20/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sherpa-onnx
-Version: 1.9.19
+Version: 1.9.20
 Summary: UNKNOWN
 Home-page: https://github.com/k2-fsa/sherpa-onnx
 Author: The sherpa-onnx development team
 Author-email: dpovey@gmail.com
 License: Apache licensed, as found in the LICENSE file
 Platform: UNKNOWN
 Classifier: Programming Language :: C++
```

### Comparing `sherpa-onnx-1.9.19/README.md` & `sherpa-onnx-1.9.20/README.md`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/c-api-examples/CMakeLists.txt` & `sherpa-onnx-1.9.20/c-api-examples/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/c-api-examples/README.md` & `sherpa-onnx-1.9.20/c-api-examples/README.md`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/c-api-examples/asr-microphone-example/alsa.cc` & `sherpa-onnx-1.9.20/c-api-examples/asr-microphone-example/alsa.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/c-api-examples/asr-microphone-example/alsa.h` & `sherpa-onnx-1.9.20/c-api-examples/asr-microphone-example/alsa.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/c-api-examples/asr-microphone-example/c-api-alsa.cc` & `sherpa-onnx-1.9.20/c-api-examples/asr-microphone-example/c-api-alsa.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/c-api-examples/audio-tagging-c-api.c` & `sherpa-onnx-1.9.20/c-api-examples/audio-tagging-c-api.c`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/c-api-examples/decode-file-c-api.c` & `sherpa-onnx-1.9.20/c-api-examples/decode-file-c-api.c`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/c-api-examples/offline-tts-c-api.c` & `sherpa-onnx-1.9.20/c-api-examples/offline-tts-c-api.c`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/c-api-examples/run.sh` & `sherpa-onnx-1.9.20/c-api-examples/run.sh`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/c-api-examples/speaker-identification-c-api.c` & `sherpa-onnx-1.9.20/c-api-examples/speaker-identification-c-api.c`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/c-api-examples/spoken-language-identification-c-api.c` & `sherpa-onnx-1.9.20/c-api-examples/spoken-language-identification-c-api.c`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/c-api-examples/streaming-hlg-decode-file-c-api.c` & `sherpa-onnx-1.9.20/c-api-examples/streaming-hlg-decode-file-c-api.c`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/cmake/asio.cmake` & `sherpa-onnx-1.9.20/cmake/asio.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/cmake/cargs.cmake` & `sherpa-onnx-1.9.20/cmake/cargs.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/cmake/cmake_extension.py` & `sherpa-onnx-1.9.20/cmake/cmake_extension.py`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/cmake/eigen.cmake` & `sherpa-onnx-1.9.20/cmake/eigen.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/cmake/espeak-ng-for-piper.cmake` & `sherpa-onnx-1.9.20/cmake/espeak-ng-for-piper.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/cmake/googletest.cmake` & `sherpa-onnx-1.9.20/cmake/googletest.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/cmake/kaldi-decoder.cmake` & `sherpa-onnx-1.9.20/cmake/kaldi-decoder.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/cmake/kaldi-native-fbank.cmake` & `sherpa-onnx-1.9.20/cmake/kaldi-native-fbank.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/cmake/kaldifst.cmake` & `sherpa-onnx-1.9.20/cmake/kaldifst.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/cmake/onnxruntime-linux-aarch64-static.cmake` & `sherpa-onnx-1.9.20/cmake/onnxruntime-linux-aarch64-static.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/cmake/onnxruntime-linux-aarch64.cmake` & `sherpa-onnx-1.9.20/cmake/onnxruntime-linux-aarch64.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/cmake/onnxruntime-linux-arm-static.cmake` & `sherpa-onnx-1.9.20/cmake/onnxruntime-linux-arm-static.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/cmake/onnxruntime-linux-arm.cmake` & `sherpa-onnx-1.9.20/cmake/onnxruntime-linux-arm.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/cmake/onnxruntime-linux-riscv64-static.cmake` & `sherpa-onnx-1.9.20/cmake/onnxruntime-linux-riscv64-static.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/cmake/onnxruntime-linux-riscv64.cmake` & `sherpa-onnx-1.9.20/cmake/onnxruntime-linux-riscv64.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/cmake/onnxruntime-linux-x86_64-gpu.cmake` & `sherpa-onnx-1.9.20/cmake/onnxruntime-linux-x86_64-gpu.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/cmake/onnxruntime-linux-x86_64-static.cmake` & `sherpa-onnx-1.9.20/cmake/onnxruntime-linux-x86_64-static.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/cmake/onnxruntime-linux-x86_64.cmake` & `sherpa-onnx-1.9.20/cmake/onnxruntime-linux-x86_64.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/cmake/onnxruntime-osx-arm64-static.cmake` & `sherpa-onnx-1.9.20/cmake/onnxruntime-osx-arm64-static.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/cmake/onnxruntime-osx-arm64.cmake` & `sherpa-onnx-1.9.20/cmake/onnxruntime-osx-arm64.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/cmake/onnxruntime-osx-universal-static.cmake` & `sherpa-onnx-1.9.20/cmake/onnxruntime-osx-universal-static.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/cmake/onnxruntime-osx-universal.cmake` & `sherpa-onnx-1.9.20/cmake/onnxruntime-osx-universal.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/cmake/onnxruntime-osx-x86_64-static.cmake` & `sherpa-onnx-1.9.20/cmake/onnxruntime-osx-x86_64-static.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/cmake/onnxruntime-osx-x86_64.cmake` & `sherpa-onnx-1.9.20/cmake/onnxruntime-osx-x86_64.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/cmake/onnxruntime-wasm-simd.cmake` & `sherpa-onnx-1.9.20/cmake/onnxruntime-wasm-simd.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/cmake/onnxruntime-win-x64-gpu.cmake` & `sherpa-onnx-1.9.20/cmake/onnxruntime-win-x64-gpu.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/cmake/onnxruntime-win-x64-static-debug.cmake` & `sherpa-onnx-1.9.20/cmake/onnxruntime-win-x64-static-debug.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/cmake/onnxruntime-win-x64-static.cmake` & `sherpa-onnx-1.9.20/cmake/onnxruntime-win-x64-static.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/cmake/onnxruntime-win-x64.cmake` & `sherpa-onnx-1.9.20/cmake/onnxruntime-win-x64.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/cmake/onnxruntime-win-x86-static-debug.cmake` & `sherpa-onnx-1.9.20/cmake/onnxruntime-win-x86-static-debug.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/cmake/onnxruntime-win-x86-static.cmake` & `sherpa-onnx-1.9.20/cmake/onnxruntime-win-x86-static.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/cmake/onnxruntime-win-x86.cmake` & `sherpa-onnx-1.9.20/cmake/onnxruntime-win-x86.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/cmake/onnxruntime.cmake` & `sherpa-onnx-1.9.20/cmake/onnxruntime.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/cmake/openfst.cmake` & `sherpa-onnx-1.9.20/cmake/openfst.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/cmake/piper-phonemize.cmake` & `sherpa-onnx-1.9.20/cmake/piper-phonemize.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/cmake/portaudio.cmake` & `sherpa-onnx-1.9.20/cmake/portaudio.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/cmake/pybind11.cmake` & `sherpa-onnx-1.9.20/cmake/pybind11.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/cmake/sherpa-onnx-no-tts.pc.in` & `sherpa-onnx-1.9.20/cmake/sherpa-onnx-no-tts.pc.in`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/cmake/sherpa-onnx.pc.in` & `sherpa-onnx-1.9.20/cmake/sherpa-onnx.pc.in`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/cmake/websocketpp.cmake` & `sherpa-onnx-1.9.20/cmake/websocketpp.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/setup.py` & `sherpa-onnx-1.9.20/setup.py`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/c-api/c-api.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/c-api/c-api.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/c-api/c-api.h` & `sherpa-onnx-1.9.20/sherpa-onnx/c-api/c-api.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/CMakeLists.txt` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/README.md` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/README.md`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/alsa-play.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/alsa-play.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/alsa-play.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/alsa-play.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/alsa.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/alsa.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/alsa.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/alsa.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/audio-tagging-impl.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/audio-tagging-impl.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/audio-tagging-impl.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/audio-tagging-impl.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/audio-tagging-label-file.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/audio-tagging-label-file.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/audio-tagging-label-file.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/audio-tagging-label-file.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/audio-tagging-model-config.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/audio-tagging-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/audio-tagging-model-config.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/audio-tagging-model-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/audio-tagging-zipformer-impl.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/audio-tagging-zipformer-impl.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/audio-tagging.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/audio-tagging.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/audio-tagging.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/audio-tagging.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/base64-decode.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/base64-decode.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/cat-test.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/cat-test.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/cat.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/cat.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/cat.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/cat.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/circular-buffer-test.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/circular-buffer-test.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/circular-buffer.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/circular-buffer.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/circular-buffer.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/circular-buffer.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/context-graph-test.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/context-graph-test.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/context-graph.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/context-graph.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/context-graph.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/context-graph.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/display.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/display.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/endpoint.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/endpoint.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/endpoint.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/endpoint.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/features.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/features.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/features.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/features.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/file-utils.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/file-utils.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/hypothesis.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/hypothesis.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/hypothesis.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/hypothesis.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/keyword-spotter-impl.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/keyword-spotter-impl.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/keyword-spotter-impl.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/keyword-spotter-impl.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/keyword-spotter-transducer-impl.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/keyword-spotter-transducer-impl.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/keyword-spotter.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/keyword-spotter.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/keyword-spotter.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/keyword-spotter.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/lexicon.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/lexicon.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/lexicon.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/lexicon.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/log.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/log.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/log.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/log.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/macros.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/macros.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/math.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/math.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/microphone.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/microphone.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-ct-transformer-model-meta-data.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-ct-transformer-model-meta-data.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-ct-transformer-model.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-ct-transformer-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-ct-transformer-model.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-ct-transformer-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-ctc-decoder.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-ctc-decoder.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-ctc-fst-decoder-config.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-ctc-fst-decoder-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-ctc-fst-decoder-config.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-ctc-fst-decoder-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-ctc-fst-decoder.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-ctc-fst-decoder.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-ctc-fst-decoder.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-ctc-fst-decoder.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-ctc-greedy-search-decoder.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-ctc-greedy-search-decoder.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-ctc-greedy-search-decoder.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-ctc-greedy-search-decoder.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-ctc-model.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-ctc-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-ctc-model.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-ctc-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-lm-config.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-lm-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-lm-config.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-lm-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-lm.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-lm.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-lm.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-lm.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-model-config.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-model-config.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-model-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-nemo-enc-dec-ctc-model-config.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-nemo-enc-dec-ctc-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-nemo-enc-dec-ctc-model-config.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-nemo-enc-dec-ctc-model-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-nemo-enc-dec-ctc-model.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-nemo-enc-dec-ctc-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-nemo-enc-dec-ctc-model.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-nemo-enc-dec-ctc-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-paraformer-decoder.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-paraformer-decoder.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-paraformer-greedy-search-decoder.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-paraformer-greedy-search-decoder.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-paraformer-greedy-search-decoder.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-paraformer-greedy-search-decoder.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-paraformer-model-config.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-paraformer-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-paraformer-model-config.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-paraformer-model-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-paraformer-model.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-paraformer-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-paraformer-model.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-paraformer-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-punctuation-ct-transformer-impl.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-punctuation-ct-transformer-impl.h`

 * *Files 5% similar despite different names*

```diff
@@ -130,33 +130,45 @@
 
       if (dot_index != 1) {
         punctuations.insert(punctuations.end(), this_punctuations.begin(),
                             this_punctuations.begin() + (dot_index + 1));
       }
     }  // for (int32_t i = 0; i != num_segments; ++i)
 
-    std::string ans;
+    std::vector<std::string> words_punct;
 
     for (int32_t i = 0; i != static_cast<int32_t>(punctuations.size()); ++i) {
-      if (i > tokens.size()) {
+      if (i >= tokens.size()) {
         break;
       }
-      const std::string &w = tokens[i];
-      if (i > 0 && !(ans.back() & 0x80) && !(w[0] & 0x80)) {
-        ans.push_back(' ');
+      std::string &w = tokens[i];
+      if (i > 0 && !(words_punct.back()[0] & 0x80) && !(w[0] & 0x80)) {
+        words_punct.push_back(" ");
       }
-      ans.append(w);
+      words_punct.push_back(std::move(w));
+
       if (punctuations[i] != meta_data.underline_id) {
-        ans.append(meta_data.id2punct[punctuations[i]]);
+        words_punct.push_back(meta_data.id2punct[punctuations[i]]);
       }
     }
-    if (ans.back() != meta_data.dot_id && ans.back() != meta_data.quest_id) {
-      ans.push_back(meta_data.dot_id);
+
+    if (words_punct.back() == meta_data.id2punct[meta_data.comma_id] ||
+        words_punct.back() == meta_data.id2punct[meta_data.pause_id]) {
+      words_punct.back() = meta_data.id2punct[meta_data.dot_id];
     }
 
+    if (words_punct.back() != meta_data.id2punct[meta_data.dot_id] &&
+        words_punct.back() != meta_data.id2punct[meta_data.quest_id]) {
+      words_punct.push_back(meta_data.id2punct[meta_data.dot_id]);
+    }
+
+    std::string ans;
+    for (const auto &w : words_punct) {
+      ans.append(w);
+    }
     return ans;
   }
 
  private:
   OfflinePunctuationConfig config_;
   OfflineCtTransformerModel model_;
 };
```

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-punctuation-impl.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-punctuation-impl.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-punctuation-impl.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-punctuation-impl.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-punctuation-model-config.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-punctuation-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-punctuation-model-config.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-punctuation-model-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-punctuation.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-punctuation.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-punctuation.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-punctuation.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-recognizer-ctc-impl.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-recognizer-ctc-impl.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-recognizer-impl.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-recognizer-impl.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-recognizer-impl.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-recognizer-impl.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-recognizer-paraformer-impl.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-recognizer-paraformer-impl.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-recognizer-transducer-impl.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-recognizer-transducer-impl.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-recognizer-whisper-impl.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-recognizer-whisper-impl.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-recognizer.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-recognizer.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-recognizer.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-recognizer.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-rnn-lm.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-rnn-lm.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-rnn-lm.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-rnn-lm.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-stream.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-stream.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-stream.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-stream.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-tdnn-ctc-model.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-tdnn-ctc-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-tdnn-ctc-model.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-tdnn-ctc-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-tdnn-model-config.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-tdnn-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-tdnn-model-config.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-tdnn-model-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-transducer-decoder.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-transducer-decoder.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-transducer-greedy-search-decoder.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-transducer-greedy-search-decoder.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-transducer-greedy-search-decoder.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-transducer-greedy-search-decoder.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-transducer-model-config.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-transducer-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-transducer-model-config.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-transducer-model-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-transducer-model.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-transducer-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-transducer-model.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-transducer-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-transducer-modified-beam-search-decoder.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-transducer-modified-beam-search-decoder.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-transducer-modified-beam-search-decoder.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-transducer-modified-beam-search-decoder.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-tts-character-frontend.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-tts-character-frontend.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-tts-character-frontend.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-tts-character-frontend.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-tts-frontend.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-tts-frontend.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-tts-impl.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-tts-impl.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-tts-impl.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-tts-impl.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-tts-model-config.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-tts-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-tts-model-config.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-tts-model-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-tts-vits-impl.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-tts-vits-impl.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-tts-vits-model-config.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-tts-vits-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-tts-vits-model-config.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-tts-vits-model-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-tts-vits-model-metadata.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-tts-vits-model-metadata.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-tts-vits-model.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-tts-vits-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-tts-vits-model.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-tts-vits-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-tts.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-tts.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-tts.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-tts.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-websocket-server-impl.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-websocket-server-impl.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-websocket-server-impl.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-websocket-server-impl.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-websocket-server.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-websocket-server.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-wenet-ctc-model-config.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-wenet-ctc-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-wenet-ctc-model-config.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-wenet-ctc-model-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-wenet-ctc-model.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-wenet-ctc-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-wenet-ctc-model.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-wenet-ctc-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-whisper-decoder.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-whisper-decoder.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-whisper-greedy-search-decoder.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-whisper-greedy-search-decoder.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-whisper-greedy-search-decoder.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-whisper-greedy-search-decoder.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-whisper-model-config.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-whisper-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-whisper-model-config.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-whisper-model-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-whisper-model.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-whisper-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-whisper-model.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-whisper-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-zipformer-audio-tagging-model-config.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-zipformer-audio-tagging-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-zipformer-audio-tagging-model-config.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-zipformer-audio-tagging-model-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-zipformer-audio-tagging-model.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-zipformer-audio-tagging-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-zipformer-audio-tagging-model.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-zipformer-audio-tagging-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-zipformer-ctc-model-config.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-zipformer-ctc-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-zipformer-ctc-model-config.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-zipformer-ctc-model-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-zipformer-ctc-model.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-zipformer-ctc-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/offline-zipformer-ctc-model.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/offline-zipformer-ctc-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-conformer-transducer-model.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-conformer-transducer-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-conformer-transducer-model.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-conformer-transducer-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-ctc-decoder.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-ctc-decoder.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-ctc-fst-decoder-config.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-ctc-fst-decoder-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-ctc-fst-decoder-config.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-ctc-fst-decoder-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-ctc-fst-decoder.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-ctc-fst-decoder.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-ctc-fst-decoder.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-ctc-fst-decoder.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-ctc-greedy-search-decoder.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-ctc-greedy-search-decoder.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-ctc-greedy-search-decoder.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-ctc-greedy-search-decoder.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-ctc-model.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-ctc-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-ctc-model.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-ctc-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-lm-config.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-lm-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-lm-config.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-lm-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-lm.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-lm.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-lstm-transducer-model.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-lstm-transducer-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-lstm-transducer-model.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-lstm-transducer-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-model-config.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-model-config.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-model-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-paraformer-decoder.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-paraformer-decoder.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-paraformer-model-config.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-paraformer-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-paraformer-model-config.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-paraformer-model-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-paraformer-model.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-paraformer-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-paraformer-model.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-paraformer-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-recognizer-ctc-impl.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-recognizer-ctc-impl.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-recognizer-impl.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-recognizer-impl.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-recognizer-impl.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-recognizer-impl.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-recognizer-paraformer-impl.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-recognizer-paraformer-impl.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-recognizer-transducer-impl.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-recognizer-transducer-impl.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-recognizer.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-recognizer.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-recognizer.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-recognizer.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-rnn-lm.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-rnn-lm.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-rnn-lm.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-rnn-lm.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-stream.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-stream.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-stream.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-stream.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-transducer-decoder.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-transducer-decoder.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-transducer-decoder.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-transducer-decoder.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-transducer-greedy-search-decoder.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-transducer-greedy-search-decoder.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-transducer-greedy-search-decoder.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-transducer-greedy-search-decoder.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-transducer-model-config.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-transducer-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-transducer-model-config.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-transducer-model-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-transducer-model.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-transducer-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-transducer-model.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-transducer-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-transducer-modified-beam-search-decoder.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-transducer-modified-beam-search-decoder.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-transducer-modified-beam-search-decoder.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-transducer-modified-beam-search-decoder.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-websocket-client.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-websocket-client.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-websocket-server-impl.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-websocket-server-impl.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-websocket-server-impl.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-websocket-server-impl.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-websocket-server.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-websocket-server.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-wenet-ctc-model-config.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-wenet-ctc-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-wenet-ctc-model-config.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-wenet-ctc-model-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-wenet-ctc-model.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-wenet-ctc-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-wenet-ctc-model.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-wenet-ctc-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-zipformer-transducer-model.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-zipformer-transducer-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-zipformer-transducer-model.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-zipformer-transducer-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-zipformer2-ctc-model-config.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-zipformer2-ctc-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-zipformer2-ctc-model-config.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-zipformer2-ctc-model-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-zipformer2-ctc-model.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-zipformer2-ctc-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-zipformer2-ctc-model.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-zipformer2-ctc-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-zipformer2-transducer-model.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-zipformer2-transducer-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/online-zipformer2-transducer-model.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/online-zipformer2-transducer-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/onnx-utils.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/onnx-utils.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/onnx-utils.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/onnx-utils.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/packed-sequence-test.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/packed-sequence-test.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/packed-sequence.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/packed-sequence.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/packed-sequence.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/packed-sequence.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/pad-sequence-test.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/pad-sequence-test.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/pad-sequence.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/pad-sequence.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/pad-sequence.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/pad-sequence.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/parse-options.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/parse-options.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/parse-options.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/parse-options.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/piper-phonemize-lexicon.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/piper-phonemize-lexicon.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/piper-phonemize-lexicon.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/piper-phonemize-lexicon.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/piper-phonemize-test.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/piper-phonemize-test.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/provider.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/provider.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/provider.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/provider.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/resample.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/resample.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/resample.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/resample.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/session.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/session.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/session.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/session.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/sherpa-onnx-alsa-offline-audio-tagging.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/sherpa-onnx-alsa-offline-audio-tagging.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/sherpa-onnx-alsa-offline-speaker-identification.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/sherpa-onnx-alsa-offline-speaker-identification.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/sherpa-onnx-alsa-offline.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/sherpa-onnx-alsa-offline.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/sherpa-onnx-alsa.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/sherpa-onnx-alsa.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/sherpa-onnx-keyword-spotter-alsa.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/sherpa-onnx-keyword-spotter-alsa.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/sherpa-onnx-keyword-spotter-microphone.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/sherpa-onnx-keyword-spotter-microphone.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/sherpa-onnx-keyword-spotter.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/sherpa-onnx-keyword-spotter.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/sherpa-onnx-microphone-offline-audio-tagging.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/sherpa-onnx-microphone-offline-audio-tagging.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/sherpa-onnx-microphone-offline-speaker-identification.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/sherpa-onnx-microphone-offline-speaker-identification.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/sherpa-onnx-microphone-offline.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/sherpa-onnx-microphone-offline.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/sherpa-onnx-microphone.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/sherpa-onnx-microphone.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/sherpa-onnx-offline-audio-tagging.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/sherpa-onnx-offline-audio-tagging.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/sherpa-onnx-offline-language-identification.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/sherpa-onnx-offline-language-identification.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/sherpa-onnx-offline-parallel.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/sherpa-onnx-offline-parallel.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/sherpa-onnx-offline-punctuation.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/sherpa-onnx-offline-punctuation.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/sherpa-onnx-offline-tts-play-alsa.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/sherpa-onnx-offline-tts-play-alsa.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/sherpa-onnx-offline-tts-play.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/sherpa-onnx-offline-tts-play.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/sherpa-onnx-offline-tts.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/sherpa-onnx-offline-tts.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/sherpa-onnx-offline.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/sherpa-onnx-offline.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/sherpa-onnx-vad-alsa.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/sherpa-onnx-vad-alsa.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/sherpa-onnx-vad-microphone-offline-asr.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/sherpa-onnx-vad-microphone-offline-asr.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/sherpa-onnx-vad-microphone.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/sherpa-onnx-vad-microphone.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/sherpa-onnx.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/sherpa-onnx.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/silero-vad-model-config.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/silero-vad-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/silero-vad-model-config.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/silero-vad-model-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/silero-vad-model.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/silero-vad-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/silero-vad-model.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/silero-vad-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/slice-test.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/slice-test.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/slice.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/slice.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/slice.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/slice.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/speaker-embedding-extractor-general-impl.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/speaker-embedding-extractor-general-impl.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/speaker-embedding-extractor-impl.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/speaker-embedding-extractor-impl.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/speaker-embedding-extractor-impl.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/speaker-embedding-extractor-impl.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/speaker-embedding-extractor-model-meta-data.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/speaker-embedding-extractor-model-meta-data.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/speaker-embedding-extractor-model.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/speaker-embedding-extractor-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/speaker-embedding-extractor-model.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/speaker-embedding-extractor-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/speaker-embedding-extractor-nemo-impl.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/speaker-embedding-extractor-nemo-impl.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/speaker-embedding-extractor-nemo-model-meta-data.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/speaker-embedding-extractor-nemo-model-meta-data.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/speaker-embedding-extractor-nemo-model.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/speaker-embedding-extractor-nemo-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/speaker-embedding-extractor-nemo-model.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/speaker-embedding-extractor-nemo-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/speaker-embedding-extractor.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/speaker-embedding-extractor.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/speaker-embedding-extractor.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/speaker-embedding-extractor.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/speaker-embedding-manager-test.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/speaker-embedding-manager-test.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/speaker-embedding-manager.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/speaker-embedding-manager.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/speaker-embedding-manager.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/speaker-embedding-manager.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/spoken-language-identification-impl.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/spoken-language-identification-impl.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/spoken-language-identification-impl.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/spoken-language-identification-impl.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/spoken-language-identification-whisper-impl.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/spoken-language-identification-whisper-impl.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/spoken-language-identification.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/spoken-language-identification.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/spoken-language-identification.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/spoken-language-identification.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/stack-test.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/stack-test.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/stack.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/stack.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/stack.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/stack.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/symbol-table.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/symbol-table.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/symbol-table.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/symbol-table.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/tee-stream.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/tee-stream.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/text-utils.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/text-utils.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/text-utils.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/text-utils.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/transducer-keyword-decoder.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/transducer-keyword-decoder.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/transducer-keyword-decoder.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/transducer-keyword-decoder.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/transpose-test.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/transpose-test.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/transpose.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/transpose.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/transpose.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/transpose.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/unbind-test.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/unbind-test.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/unbind.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/unbind.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/unbind.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/unbind.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/utils.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/utils.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/utils.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/utils.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/vad-model-config.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/vad-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/vad-model-config.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/vad-model-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/vad-model.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/vad-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/vad-model.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/vad-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/voice-activity-detector.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/voice-activity-detector.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/voice-activity-detector.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/voice-activity-detector.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/wave-reader.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/wave-reader.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/wave-reader.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/wave-reader.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/wave-writer.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/wave-writer.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/csrc/wave-writer.h` & `sherpa-onnx-1.9.20/sherpa-onnx/csrc/wave-writer.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/jni/jni.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/jni/jni.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/CMakeLists.txt` & `sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/alsa.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/alsa.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/audio-tagging.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/audio-tagging.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/circular-buffer.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/circular-buffer.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/endpoint.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/endpoint.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/faked-alsa.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/faked-alsa.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/features.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/features.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/keyword-spotter.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/keyword-spotter.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/offline-ctc-fst-decoder-config.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/offline-ctc-fst-decoder-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/offline-lm-config.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/offline-lm-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/offline-model-config.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/offline-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/offline-nemo-enc-dec-ctc-model-config.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/offline-nemo-enc-dec-ctc-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/offline-paraformer-model-config.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/offline-paraformer-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/offline-punctuation.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/offline-punctuation.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/offline-recognizer.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/offline-recognizer.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/offline-stream.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/offline-stream.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/offline-tdnn-model-config.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/offline-tdnn-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/offline-transducer-model-config.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/offline-transducer-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/offline-tts-model-config.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/offline-tts-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/offline-tts-vits-model-config.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/offline-tts-vits-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/offline-tts.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/offline-tts.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/offline-wenet-ctc-model-config.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/offline-wenet-ctc-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/offline-whisper-model-config.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/offline-whisper-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/offline-zipformer-ctc-model-config.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/offline-zipformer-ctc-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/online-ctc-fst-decoder-config.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/online-ctc-fst-decoder-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/online-lm-config.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/online-lm-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/online-model-config.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/online-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/online-paraformer-model-config.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/online-paraformer-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/online-recognizer.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/online-recognizer.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/online-stream.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/online-stream.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/online-transducer-model-config.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/online-transducer-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/online-wenet-ctc-model-config.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/online-wenet-ctc-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/online-zipformer2-ctc-model-config.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/online-zipformer2-ctc-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/sherpa-onnx.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/sherpa-onnx.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/silero-vad-model-config.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/silero-vad-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/speaker-embedding-extractor.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/speaker-embedding-extractor.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/speaker-embedding-manager.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/speaker-embedding-manager.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/spoken-language-identification.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/spoken-language-identification.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/vad-model-config.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/vad-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/vad-model.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/vad-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/voice-activity-detector.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/voice-activity-detector.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/python/csrc/wave-writer.cc` & `sherpa-onnx-1.9.20/sherpa-onnx/python/csrc/wave-writer.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/python/sherpa_onnx/__init__.py` & `sherpa-onnx-1.9.20/sherpa-onnx/python/sherpa_onnx/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,8 +30,8 @@
     write_wave,
 )
 
 from .keyword_spotter import KeywordSpotter
 from .offline_recognizer import OfflineRecognizer
 from .online_recognizer import OnlineRecognizer
 from .utils import text2token
-__version__ = '1.9.19'
+__version__ = '1.9.20'
```

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/python/sherpa_onnx/cli.py` & `sherpa-onnx-1.9.20/sherpa-onnx/python/sherpa_onnx/cli.py`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/python/sherpa_onnx/keyword_spotter.py` & `sherpa-onnx-1.9.20/sherpa-onnx/python/sherpa_onnx/keyword_spotter.py`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/python/sherpa_onnx/offline_recognizer.py` & `sherpa-onnx-1.9.20/sherpa-onnx/python/sherpa_onnx/offline_recognizer.py`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/python/sherpa_onnx/online_recognizer.py` & `sherpa-onnx-1.9.20/sherpa-onnx/python/sherpa_onnx/online_recognizer.py`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/python/sherpa_onnx/utils.py` & `sherpa-onnx-1.9.20/sherpa-onnx/python/sherpa_onnx/utils.py`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/python/tests/CMakeLists.txt` & `sherpa-onnx-1.9.20/sherpa-onnx/python/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/python/tests/test_feature_extractor_config.py` & `sherpa-onnx-1.9.20/sherpa-onnx/python/tests/test_feature_extractor_config.py`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/python/tests/test_keyword_spotter.py` & `sherpa-onnx-1.9.20/sherpa-onnx/python/tests/test_keyword_spotter.py`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/python/tests/test_offline_recognizer.py` & `sherpa-onnx-1.9.20/sherpa-onnx/python/tests/test_offline_recognizer.py`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/python/tests/test_online_recognizer.py` & `sherpa-onnx-1.9.20/sherpa-onnx/python/tests/test_online_recognizer.py`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/python/tests/test_online_transducer_model_config.py` & `sherpa-onnx-1.9.20/sherpa-onnx/python/tests/test_online_transducer_model_config.py`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/python/tests/test_speaker_recognition.py` & `sherpa-onnx-1.9.20/sherpa-onnx/python/tests/test_speaker_recognition.py`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa-onnx/python/tests/test_text2token.py` & `sherpa-onnx-1.9.20/sherpa-onnx/python/tests/test_text2token.py`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.19/sherpa_onnx.egg-info/PKG-INFO` & `sherpa-onnx-1.9.20/sherpa_onnx.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sherpa-onnx
-Version: 1.9.19
+Version: 1.9.20
 Summary: UNKNOWN
 Home-page: https://github.com/k2-fsa/sherpa-onnx
 Author: The sherpa-onnx development team
 Author-email: dpovey@gmail.com
 License: Apache licensed, as found in the LICENSE file
 Platform: UNKNOWN
 Classifier: Programming Language :: C++
```

### Comparing `sherpa-onnx-1.9.19/sherpa_onnx.egg-info/SOURCES.txt` & `sherpa-onnx-1.9.20/sherpa_onnx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

