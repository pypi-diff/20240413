# Comparing `tmp/inewave-1.7.3.tar.gz` & `tmp/inewave-1.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inewave-1.7.3.tar", last modified: Fri Mar  1 13:48:26 2024, max compression
+gzip compressed data, was "inewave-1.7.4.tar", last modified: Fri Apr 12 14:58:12 2024, max compression
```

## Comparing `inewave-1.7.3.tar` & `inewave-1.7.4.tar`

### file list

```diff
@@ -1,880 +1,880 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 13:48:26.652419 inewave-1.7.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-01 13:44:52.000000 inewave-1.7.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-03-01 13:48:26.652419 inewave-1.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-03-01 13:44:52.000000 inewave-1.7.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 13:48:26.436420 inewave-1.7.3/examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 13:44:52.000000 inewave-1.7.3/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-03-01 13:44:52.000000 inewave-1.7.3/examples/plot_dger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-03-01 13:44:52.000000 inewave-1.7.3/examples/plot_modif.py
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-03-01 13:44:52.000000 inewave-1.7.3/examples/plot_pmo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-03-01 13:44:52.000000 inewave-1.7.3/examples/plot_sistema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 13:48:26.436420 inewave-1.7.3/inewave/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 13:48:26.436420 inewave-1.7.3/inewave/_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5930 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/_utils/formatacao.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 13:48:26.436420 inewave-1.7.3/inewave/libs/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13324 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/libs/eolica.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 13:48:26.436420 inewave-1.7.3/inewave/libs/modelos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/libs/modelos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14151 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/libs/modelos/eolica.py
--rw-r--r--   0 runner    (1001) docker     (127)    19601 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/libs/modelos/restricoes.py
--rw-r--r--   0 runner    (1001) docker     (127)    19927 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/libs/modelos/usinas_hidreletricas.py
--rw-r--r--   0 runner    (1001) docker     (127)    16485 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/libs/restricoes.py
--rw-r--r--   0 runner    (1001) docker     (127)    16373 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/libs/usinas_hidreletricas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 13:48:26.452420 inewave-1.7.3/inewave/newave/
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/abertura.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/adterm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/agrint.py
--rw-r--r--   0 runner    (1001) docker     (127)    15168 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/arquivos.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/avl_cortesfpha_nwv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/avl_desvfpha_s.py
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/avl_desvfpha_v_q.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/bid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/cadic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/caso.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/clasgas.py
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/clast.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/confhd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/conft.py
--rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/cortes.py
--rw-r--r--   0 runner    (1001) docker     (127)    12982 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/cortesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     6744 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/curva.py
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/cvar.py
--rw-r--r--   0 runner    (1001) docker     (127)    83959 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/dger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/dsvagua.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/eafpast.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/eco_fpha.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/elnino.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/enavazb.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/enavazf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/energiab.py
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/energiaf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/energias.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/engnat.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/ensoaux.py
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/exph.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/expt.py
--rw-r--r--   0 runner    (1001) docker     (127)    38978 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/forward.py
--rw-r--r--   0 runner    (1001) docker     (127)     9876 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/forwarh.py
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/gee.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/ghmin.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/gtminpat.py
--rw-r--r--   0 runner    (1001) docker     (127)    11647 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/hidr.py
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/itaipu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/manutt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 13:48:26.460420 inewave-1.7.3/inewave/newave/modelos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/abertura.py
--rw-r--r--   0 runner    (1001) docker     (127)     4977 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/adterm.py
--rw-r--r--   0 runner    (1001) docker     (127)     7846 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/agrint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/arquivos.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 13:48:26.464420 inewave-1.7.3/inewave/newave/modelos/arquivoscsv/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/arquivoscsv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/arquivoscsv/arquivocsv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/avl_cortesfpha_nwv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/avl_desvfpha_s.py
--rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/avl_desvfpha_v_q.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/bid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 13:48:26.464420 inewave-1.7.3/inewave/newave/modelos/blocos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/blocos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/blocos/tabelacsv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/blocos/versaomodelo.py
--rw-r--r--   0 runner    (1001) docker     (127)     5531 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/cadic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/caso.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/clasgas.py
--rw-r--r--   0 runner    (1001) docker     (127)     7549 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/clast.py
--rw-r--r--   0 runner    (1001) docker     (127)     3940 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/confhd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/conft.py
--rw-r--r--   0 runner    (1001) docker     (127)     7388 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/cortes.py
--rw-r--r--   0 runner    (1001) docker     (127)    30466 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/cortesh.py
--rw-r--r--   0 runner    (1001) docker     (127)    13812 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/curva.py
--rw-r--r--   0 runner    (1001) docker     (127)     7547 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/cvar.py
--rw-r--r--   0 runner    (1001) docker     (127)   140730 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/dger.py
--rw-r--r--   0 runner    (1001) docker     (127)     5560 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/dsvagua.py
--rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/eafpast.py
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/eco_fpha.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/elnino.py
--rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/enavazb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/enavazf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/energiab.py
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/energiaf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/energias.py
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/engnat.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/ensoaux.py
--rw-r--r--   0 runner    (1001) docker     (127)     5520 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/exph.py
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/expt.py
--rw-r--r--   0 runner    (1001) docker     (127)    87572 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/forward.py
--rw-r--r--   0 runner    (1001) docker     (127)     8200 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/forwarh.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/gee.py
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/ghmin.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/gtminpat.py
--rw-r--r--   0 runner    (1001) docker     (127)    15742 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/hidr.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/itaipu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/manutt.py
--rw-r--r--   0 runner    (1001) docker     (127)    16691 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/modif.py
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/newavetim.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/nwv_avl_evap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/nwv_cortes_evap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/nwv_eco_evap.py
--rw-r--r--   0 runner    (1001) docker     (127)    32022 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/parp.py
--rw-r--r--   0 runner    (1001) docker     (127)    17352 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/parpeol.py
--rw-r--r--   0 runner    (1001) docker     (127)    24383 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/parpvaz.py
--rw-r--r--   0 runner    (1001) docker     (127)    21478 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/patamar.py
--rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/penalid.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/perda.py
--rw-r--r--   0 runner    (1001) docker     (127)    55106 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/pmo.py
--rw-r--r--   0 runner    (1001) docker     (127)     6574 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/re.py
--rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/ree.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/sar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/selcor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/shist.py
--rw-r--r--   0 runner    (1001) docker     (127)    23431 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/sistema.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/tecno.py
--rw-r--r--   0 runner    (1001) docker     (127)     4762 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/term.py
--rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/vazaob.py
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/vazaof.py
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/vazaos.py
--rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/vazinat.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/vazoes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/vazpast.py
--rw-r--r--   0 runner    (1001) docker     (127)     3459 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modelos/volref_saz.py
--rw-r--r--   0 runner    (1001) docker     (127)    13947 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/modif.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/newavetim.py
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/nwv_avl_evap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/nwv_cortes_evap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/nwv_eco_evap.py
--rw-r--r--   0 runner    (1001) docker     (127)    18425 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/parp.py
--rw-r--r--   0 runner    (1001) docker     (127)    12841 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/parpeol.py
--rw-r--r--   0 runner    (1001) docker     (127)    15859 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/parpvaz.py
--rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/patamar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/penalid.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/perda.py
--rw-r--r--   0 runner    (1001) docker     (127)    19079 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/pmo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/re.py
--rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/ree.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/sar.py
--rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/selcor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/shist.py
--rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/sistema.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/tecno.py
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/term.py
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/vazaob.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/vazaof.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/vazaos.py
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/vazinat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/vazoes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/vazpast.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/newave/volref_saz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 13:48:26.464420 inewave-1.7.3/inewave/nwlistcf/
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistcf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6739 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistcf/arquivos.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistcf/caso.py
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistcf/estados.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 13:48:26.464420 inewave-1.7.3/inewave/nwlistcf/modelos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistcf/modelos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistcf/modelos/arquivos.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistcf/modelos/caso.py
--rw-r--r--   0 runner    (1001) docker     (127)     4300 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistcf/modelos/estados.py
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistcf/modelos/nwlistcfdat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistcf/modelos/nwlistcfrel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistcf/nwlistcfdat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistcf/nwlistcfrel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 13:48:26.488420 inewave-1.7.3/inewave/nwlistop/
--rw-r--r--   0 runner    (1001) docker     (127)     4915 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/c_v_rhq.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/c_v_rhq_s.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/c_v_rhv.py
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/c_v_rhv_s.py
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/cbomb.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/cbombsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/cdef.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/cdefsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/celetricas.py
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/cmarg.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/cmargmed.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/coper.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/corteolm.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/cterm.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/ctermsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/deficit.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/defsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/deletricas.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/depminuh.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/desvuh.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/dfphauh.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/dlppdfmax.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/dlppdfmaxm.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/dlppdfmaxs.py
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/dlpptbmax.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/dlpptbmaxm.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/dlpptbmaxs.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/dnegevap.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/dposevap.py
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/dtbmax.py
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/dtbmin.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/dvazmax.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/eaf.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/eafb.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/eafbm.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/eafbsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/eafm.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/earmf.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/earmfm.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/earmfp.py
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/earmfpm.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/earmfpsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/earmfsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/edesvc.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/edesvcm.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/edesvcsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/evapo.py
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/evapom.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/evaporsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/evert.py
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/evertm.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/evertsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/exces.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/excessin.py
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/form_rhq.py
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/form_rhv.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/fteolm.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/fteolsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/geol.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/geolm.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/geolsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/gh_fphexat.py
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/ghidr.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/ghidrm.py
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/ghidrsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/ghiduh.py
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/ghmax.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/ghmax_fpha.py
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/ghmax_fphc.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/ghmaxm.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/ghmaxmr.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/ghmaxr.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/ghmaxrsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/ghmaxsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/ghtot.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/ghtotm.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/ghtotsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/gtert.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/gttot.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/gttotsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/hjus.py
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/hliq.py
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/hmont.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/intercambio.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/invade.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/invadem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/mediasmerc.py
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/mediasree.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/mediasrep.py
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/mediasrhq.py
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/mediasrhv.py
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/mediassin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/mediasusie.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/mediasusih.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/mediasusit.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/mercl.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/merclsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/mevmin.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/mevminm.py
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/mevminsin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 13:48:26.512420 inewave-1.7.3/inewave/nwlistop/modelos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 13:48:26.516420 inewave-1.7.3/inewave/nwlistop/modelos/arquivos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/arquivos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/arquivos/arquivoclassetermicasubmercadopatamar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/arquivos/arquivoestacaobombeamentopatamar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/arquivos/arquivoparsubmercadopatamar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/arquivos/arquivoree.py
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/arquivos/arquivoreepatamar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/arquivos/arquivorestricao.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/arquivos/arquivorestricaopatamar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/arquivos/arquivosin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/arquivos/arquivosinpatamar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/arquivos/arquivosubmercado.py
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/arquivos/arquivosubmercadopatamar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/arquivos/arquivousina.py
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/arquivos/arquivousinapatamar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 13:48:26.516420 inewave-1.7.3/inewave/nwlistop/modelos/blocos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/blocos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/blocos/estacaobombeamento.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/blocos/parsubmercados.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/blocos/ree.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/blocos/restricao.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/blocos/submercado.py
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/blocos/usina.py
--rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/blocos/valoresclassetermicaseriepatamar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/blocos/valoresserie.py
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/blocos/valoresseriepatamar.py
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/c_v_rhq.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/c_v_rhq_s.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/c_v_rhv.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/c_v_rhv_s.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/cbomb.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/cbombsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/cdef.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/cdefsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/celetricas.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/cmarg.py
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/cmargmed.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/coper.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/corteolm.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/cterm.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/ctermsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/def.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/defsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/deletricas.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/depminuh.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/desvuh.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/dflppdfmaxm.py
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/dflpptbmaxm.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/dfphauh.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/dlppdfmax.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/dlppdfmaxs.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/dlpptbmax.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/dlpptbmaxs.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/dnegevap.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/dposevap.py
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/dtbmax.py
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/dtbmin.py
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/dvazmax.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/eaf.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/eafb.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/eafbm.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/eafbsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/eafm.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/earmf.py
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/earmfm.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/earmfp.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/earmfpm.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/earmfpsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/earmfsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/edesvc.py
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/edesvcm.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/edesvcsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/evapo.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/evapom.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/evaporsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/evert.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/evertm.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/evertsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/exces.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/excessin.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/form_rhq.py
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/form_rhv.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/fteolm.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/fteolsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/geol.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/geolm.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/geolsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/gh_fphexat.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/ghidr.py
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/ghidrm.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/ghidrsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/ghiduh.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/ghmax.py
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/ghmax_fpha.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/ghmax_fphc.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/ghmaxm.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/ghmaxmr.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/ghmaxr.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/ghmaxrsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/ghmaxsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/ghtot.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/ghtotm.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/ghtotsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/gtert.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/gttot.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/gttotsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/hjus.py
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/hliq.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/hmont.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/intercambio.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/invade.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/invadem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/mediasmerc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/mediasree.py
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/mediasrep.py
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/mediasrhq.py
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/mediasrhv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/mediassin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/mediasusie.py
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/mediasusih.py
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/mediasusit.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/mercl.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/merclsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/mevmin.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/mevminm.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/mevminsin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6752 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/nwlistopdat.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/perdf.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/perdfm.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/perdfsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/pivarm.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/pivarmincr.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/qafluh.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/qincruh.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/rhslppdf.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/rhslpptb.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/vagua.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/varmpuh.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/varmuh.py
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/vbomb.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/vdesviouh.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/vento.py
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/vertuh.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/verturb.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/verturbm.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/verturbsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/vevapuh.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/vevmin.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/vevminm.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/vevminsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/vghmin.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/vghminm.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/vghminsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/vghminuh.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/viol_rhq.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/viol_rhv.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/vmort.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/vmortm.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/vmortsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/modelos/vturuh.py
--rw-r--r--   0 runner    (1001) docker     (127)     7672 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/nwlistopdat.py
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/perdf.py
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/perdfm.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/perdfsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/pivarm.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/pivarmincr.py
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/qafluh.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/qincruh.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/rhslppdf.py
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/rhslpptb.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/vagua.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/varmpuh.py
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/varmuh.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/vbomb.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/vdesviouh.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/vento.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/vertuh.py
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/verturb.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/verturbm.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/verturbsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/vevapuh.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/vevmin.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/vevminm.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/vevminsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/vghmin.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/vghminm.py
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/vghminsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/vghminuh.py
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/viol_rhq.py
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/viol_rhv.py
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/vmort.py
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/vmortm.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/vmortsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/nwlistop/vturuh.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 13:44:52.000000 inewave-1.7.3/inewave/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 13:48:26.652419 inewave-1.7.3/inewave.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-03-01 13:48:26.000000 inewave-1.7.3/inewave.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    27157 2024-03-01 13:48:26.000000 inewave-1.7.3/inewave.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 13:48:26.000000 inewave-1.7.3/inewave.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-01 13:48:26.000000 inewave-1.7.3/inewave.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-01 13:48:26.000000 inewave-1.7.3/inewave.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-01 13:48:26.652419 inewave-1.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-03-01 13:44:52.000000 inewave-1.7.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 13:48:26.516420 inewave-1.7.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 13:48:26.516420 inewave-1.7.3/tests/_arquivos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/_arquivos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 13:48:26.516420 inewave-1.7.3/tests/libs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8406 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/libs/test_eolica.py
--rw-r--r--   0 runner    (1001) docker     (127)     9990 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/libs/test_restricoes.py
--rw-r--r--   0 runner    (1001) docker     (127)    16413 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/libs/test_usinas_hidreletricas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 13:48:26.516420 inewave-1.7.3/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 13:48:26.616420 inewave-1.7.3/tests/mocks/arquivos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/adterm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/agrint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/arquivos.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/arquivos_nwlistcf.py
--rw-r--r--   0 runner    (1001) docker     (127)    10255 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/avl_cortesfpha_nwv.py
--rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/avl_desvfpha_s.py
--rw-r--r--   0 runner    (1001) docker     (127)    46951 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/avl_desvfpha_v_q.py
--rw-r--r--   0 runner    (1001) docker     (127)    24307 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/c_v_rhq.py
--rw-r--r--   0 runner    (1001) docker     (127)    24306 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/c_v_rhq_s.py
--rw-r--r--   0 runner    (1001) docker     (127)     9455 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/c_v_rhv.py
--rw-r--r--   0 runner    (1001) docker     (127)     9463 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/c_v_rhv_s.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/cadic.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/caso.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/caso_nwlistcf_nwlistop.py
--rw-r--r--   0 runner    (1001) docker     (127)    24307 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/cbomb.py
--rw-r--r--   0 runner    (1001) docker     (127)    24310 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/cbombsin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/cdef.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/cdefsin.py
--rw-r--r--   0 runner    (1001) docker     (127)    24312 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/celetricas.py
--rw-r--r--   0 runner    (1001) docker     (127)    30063 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/clast.py
--rw-r--r--   0 runner    (1001) docker     (127)   847210 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/cmarg.py
--rw-r--r--   0 runner    (1001) docker     (127)   295249 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/cmargmed.py
--rw-r--r--   0 runner    (1001) docker     (127)    13487 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/confhd.py
--rw-r--r--   0 runner    (1001) docker     (127)     6262 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/conft.py
--rw-r--r--   0 runner    (1001) docker     (127)   295245 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/coper.py
--rw-r--r--   0 runner    (1001) docker     (127)  1105146 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/corteolm.py
--rw-r--r--   0 runner    (1001) docker     (127)   295190 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/cterm.py
--rw-r--r--   0 runner    (1001) docker     (127)   295196 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/ctermsin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/curva.py
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/cvar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/deficit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/defsin.py
--rw-r--r--   0 runner    (1001) docker     (127)    24311 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/deletricas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/depminuh.py
--rw-r--r--   0 runner    (1001) docker     (127)   283211 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/desvuh.py
--rw-r--r--   0 runner    (1001) docker     (127)   847164 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/dfphauh.py
--rw-r--r--   0 runner    (1001) docker     (127)    15257 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/dger.py
--rw-r--r--   0 runner    (1001) docker     (127)  1105161 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/dlppdfmax.py
--rw-r--r--   0 runner    (1001) docker     (127)  1105169 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/dlppdfmaxm.py
--rw-r--r--   0 runner    (1001) docker     (127)  1105154 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/dlppdfmaxs.py
--rw-r--r--   0 runner    (1001) docker     (127)  1105161 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/dlpptbmax.py
--rw-r--r--   0 runner    (1001) docker     (127)  1105169 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/dlpptbmaxm.py
--rw-r--r--   0 runner    (1001) docker     (127)  1105154 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/dlpptbmaxs.py
--rw-r--r--   0 runner    (1001) docker     (127)    15309 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/dneg_evap.py
--rw-r--r--   0 runner    (1001) docker     (127)    15309 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/dpos_evap.py
--rw-r--r--   0 runner    (1001) docker     (127)   120243 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/dsvagua.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/dtbmax.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/dtbmin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/dvazmax.py
--rw-r--r--   0 runner    (1001) docker     (127)   267099 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/eaf.py
--rw-r--r--   0 runner    (1001) docker     (127)   267152 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/eafb.py
--rw-r--r--   0 runner    (1001) docker     (127)   267153 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/eafbm.py
--rw-r--r--   0 runner    (1001) docker     (127)   267155 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/eafbsin.py
--rw-r--r--   0 runner    (1001) docker     (127)   267101 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/eafm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/eafpast.py
--rw-r--r--   0 runner    (1001) docker     (127)   267101 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/earmf.py
--rw-r--r--   0 runner    (1001) docker     (127)   267144 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/earmfm.py
--rw-r--r--   0 runner    (1001) docker     (127)   291239 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/earmfp.py
--rw-r--r--   0 runner    (1001) docker     (127)   291240 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/earmfpm.py
--rw-r--r--   0 runner    (1001) docker     (127)    14002 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/earmfpsin.py
--rw-r--r--   0 runner    (1001) docker     (127)   267156 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/earmfsin.py
--rw-r--r--   0 runner    (1001) docker     (127)   232674 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/eco_fpha.py
--rw-r--r--   0 runner    (1001) docker     (127)   267116 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/edesvc.py
--rw-r--r--   0 runner    (1001) docker     (127)   267119 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/edesvcm.py
--rw-r--r--   0 runner    (1001) docker     (127)   267121 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/edesvcsin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/eolica.py
--rw-r--r--   0 runner    (1001) docker     (127)    56476 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/estados.py
--rw-r--r--   0 runner    (1001) docker     (127)   267117 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/evapo.py
--rw-r--r--   0 runner    (1001) docker     (127)   267118 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/evapom.py
--rw-r--r--   0 runner    (1001) docker     (127)   267121 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/evaporsin.py
--rw-r--r--   0 runner    (1001) docker     (127)   267137 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/evert.py
--rw-r--r--   0 runner    (1001) docker     (127)   267138 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/evertm.py
--rw-r--r--   0 runner    (1001) docker     (127)   267139 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/evertsin.py
--rw-r--r--   0 runner    (1001) docker     (127)  1104654 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/exces.py
--rw-r--r--   0 runner    (1001) docker     (127)  1104652 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/excessin.py
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/exph.py
--rw-r--r--   0 runner    (1001) docker     (127)   120990 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/expt.py
--rw-r--r--   0 runner    (1001) docker     (127)    24311 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/form_rhq.py
--rw-r--r--   0 runner    (1001) docker     (127)     9464 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/form_rhv.py
--rw-r--r--   0 runner    (1001) docker     (127)  1104650 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/fteolm.py
--rw-r--r--   0 runner    (1001) docker     (127)  1104652 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/fteolsin.py
--rw-r--r--   0 runner    (1001) docker     (127)  1105178 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/geol.py
--rw-r--r--   0 runner    (1001) docker     (127)  1105179 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/geolm.py
--rw-r--r--   0 runner    (1001) docker     (127)  1105181 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/geolsin.py
--rw-r--r--   0 runner    (1001) docker     (127)    19859 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/gh_fphexat.py
--rw-r--r--   0 runner    (1001) docker     (127)  1105153 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/ghidr.py
--rw-r--r--   0 runner    (1001) docker     (127)  1105154 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/ghidrm.py
--rw-r--r--   0 runner    (1001) docker     (127)  1105156 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/ghidrsin.py
--rw-r--r--   0 runner    (1001) docker     (127)   847144 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/ghiduh.py
--rw-r--r--   0 runner    (1001) docker     (127)  1105136 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/ghmax.py
--rw-r--r--   0 runner    (1001) docker     (127)    19895 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/ghmax_fpha.py
--rw-r--r--   0 runner    (1001) docker     (127)    19898 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/ghmax_fphc.py
--rw-r--r--   0 runner    (1001) docker     (127)  1105138 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/ghmaxm.py
--rw-r--r--   0 runner    (1001) docker     (127)  1105139 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/ghmaxmr.py
--rw-r--r--   0 runner    (1001) docker     (127)  1105138 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/ghmaxr.py
--rw-r--r--   0 runner    (1001) docker     (127)  1105141 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/ghmaxrsin.py
--rw-r--r--   0 runner    (1001) docker     (127)  1105140 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/ghmaxsin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/ghmin.py
--rw-r--r--   0 runner    (1001) docker     (127)  1105189 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/ghtot.py
--rw-r--r--   0 runner    (1001) docker     (127)  1105190 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/ghtotm.py
--rw-r--r--   0 runner    (1001) docker     (127)    49768 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/ghtotsin.py
--rw-r--r--   0 runner    (1001) docker     (127)    26457 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/gtert.py
--rw-r--r--   0 runner    (1001) docker     (127)  1105188 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/gttot.py
--rw-r--r--   0 runner    (1001) docker     (127)  1105191 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/gttotsin.py
--rw-r--r--   0 runner    (1001) docker     (127)   846407 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/hjus.py
--rw-r--r--   0 runner    (1001) docker     (127)   846407 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/hliq.py
--rw-r--r--   0 runner    (1001) docker     (127)   425676 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/hmont.py
--rw-r--r--   0 runner    (1001) docker     (127)  1087195 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/intercambio.py
--rw-r--r--   0 runner    (1001) docker     (127)   267122 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/invade.py
--rw-r--r--   0 runner    (1001) docker     (127)   267130 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/invadem.py
--rw-r--r--   0 runner    (1001) docker     (127)    49720 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/manutt.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/mercl.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/merclsin.py
--rw-r--r--   0 runner    (1001) docker     (127)   267116 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/mevmin.py
--rw-r--r--   0 runner    (1001) docker     (127)   267117 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/mevminm.py
--rw-r--r--   0 runner    (1001) docker     (127)   267118 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/mevminsin.py
--rw-r--r--   0 runner    (1001) docker     (127)    57012 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/modif.py
--rw-r--r--   0 runner    (1001) docker     (127)    45543 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/newavetim.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/nwlistcfdat.py
--rw-r--r--   0 runner    (1001) docker     (127)    76521 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/nwlistcfrel.py
--rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/nwlistopdat.py
--rw-r--r--   0 runner    (1001) docker     (127)     9502 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/nwv_avl_evap.py
--rw-r--r--   0 runner    (1001) docker     (127)    12629 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/nwv_cortes_evap.py
--rw-r--r--   0 runner    (1001) docker     (127)    10775 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/nwv_eco_evap.py
--rw-r--r--   0 runner    (1001) docker     (127)   378349 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/parp.py
--rw-r--r--   0 runner    (1001) docker     (127)    50087 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/parpeol.py
--rw-r--r--   0 runner    (1001) docker     (127)    38585 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/parpvaz.py
--rw-r--r--   0 runner    (1001) docker     (127)    52098 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/patamar.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/penalid.py
--rw-r--r--   0 runner    (1001) docker     (127)   267136 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/perdf.py
--rw-r--r--   0 runner    (1001) docker     (127)   267137 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/perdfm.py
--rw-r--r--   0 runner    (1001) docker     (127)   267139 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/perdfsin.py
--rw-r--r--   0 runner    (1001) docker     (127)   425677 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/pivarm.py
--rw-r--r--   0 runner    (1001) docker     (127)    14847 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/pivarmincr.py
--rw-r--r--   0 runner    (1001) docker     (127)   655644 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/pmo.py
--rw-r--r--   0 runner    (1001) docker     (127)   283145 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/qafluh.py
--rw-r--r--   0 runner    (1001) docker     (127)   283145 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/qincruh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/re.py
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/ree.py
--rw-r--r--   0 runner    (1001) docker     (127)     4426 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/restricoes.py
--rw-r--r--   0 runner    (1001) docker     (127)  1105160 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/rhslppdf.py
--rw-r--r--   0 runner    (1001) docker     (127)  1105160 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/rhslpptb.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/selcor.py
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/shist.py
--rw-r--r--   0 runner    (1001) docker     (127)    20855 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/sistema.py
--rw-r--r--   0 runner    (1001) docker     (127)    18692 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/term.py
--rw-r--r--   0 runner    (1001) docker     (127)    38821 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/usinas_hidreletricas.py
--rw-r--r--   0 runner    (1001) docker     (127)   271157 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/vagua.py
--rw-r--r--   0 runner    (1001) docker     (127)   283139 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/varmpuh.py
--rw-r--r--   0 runner    (1001) docker     (127)   283209 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/varmuh.py
--rw-r--r--   0 runner    (1001) docker     (127)    32259 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/vazpast.py
--rw-r--r--   0 runner    (1001) docker     (127)    24306 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/vbomb.py
--rw-r--r--   0 runner    (1001) docker     (127)   847213 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/vdesviouh.py
--rw-r--r--   0 runner    (1001) docker     (127)   267101 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/vento.py
--rw-r--r--   0 runner    (1001) docker     (127)   847200 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/vertuh.py
--rw-r--r--   0 runner    (1001) docker     (127)   267155 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/verturb.py
--rw-r--r--   0 runner    (1001) docker     (127)   267156 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/verturbm.py
--rw-r--r--   0 runner    (1001) docker     (127)   267158 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/verturbsin.py
--rw-r--r--   0 runner    (1001) docker     (127)    15308 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/vevapuh.py
--rw-r--r--   0 runner    (1001) docker     (127)   267122 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/vevmin.py
--rw-r--r--   0 runner    (1001) docker     (127)   267130 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/vevminm.py
--rw-r--r--   0 runner    (1001) docker     (127)   267117 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/vevminsin.py
--rw-r--r--   0 runner    (1001) docker     (127)  1105173 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/vghmin.py
--rw-r--r--   0 runner    (1001) docker     (127)  1105174 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/vghminm.py
--rw-r--r--   0 runner    (1001) docker     (127)  1105176 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/vghminsin.py
--rw-r--r--   0 runner    (1001) docker     (127)   847195 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/vghminuh.py
--rw-r--r--   0 runner    (1001) docker     (127)    24310 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/viol_rhq.py
--rw-r--r--   0 runner    (1001) docker     (127)     9463 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/viol_rhv.py
--rw-r--r--   0 runner    (1001) docker     (127)   267115 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/vmort.py
--rw-r--r--   0 runner    (1001) docker     (127)   267116 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/vmortm.py
--rw-r--r--   0 runner    (1001) docker     (127)   267118 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/vmortsin.py
--rw-r--r--   0 runner    (1001) docker     (127)    25446 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/volref_saz.py
--rw-r--r--   0 runner    (1001) docker     (127)   847135 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/arquivos/vturuh.py
--rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/mocks/mock_open.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 13:48:26.628419 inewave-1.7.3/tests/newave/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/newave/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/newave/test_adterm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/newave/test_agrint.py
--rw-r--r--   0 runner    (1001) docker     (127)     5298 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/newave/test_arquivos.py
--rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/newave/test_avl_cortesfpha_nwv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/newave/test_avl_desvfpha_s.py
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/newave/test_avl_desvfpha_v_q.py
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/newave/test_cadic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/newave/test_caso.py
--rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/newave/test_clast.py
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/newave/test_confhd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/newave/test_conft.py
--rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/newave/test_cortes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/newave/test_cortesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/newave/test_curva.py
--rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/newave/test_cvar.py
--rw-r--r--   0 runner    (1001) docker     (127)    52070 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/newave/test_dger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/newave/test_dsvagua.py
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/newave/test_eafpast.py
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/newave/test_eco_fpha.py
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/newave/test_enavazb.py
--rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/newave/test_enavazf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/newave/test_energiab.py
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/newave/test_energiaf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/newave/test_energias.py
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/newave/test_engnat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/newave/test_exph.py
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/newave/test_expt.py
--rw-r--r--   0 runner    (1001) docker     (127)    36320 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/newave/test_forward.py
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/newave/test_forwarh.py
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/newave/test_ghmin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/newave/test_hidr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/newave/test_manutt.py
--rw-r--r--   0 runner    (1001) docker     (127)     8825 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/newave/test_modif.py
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/newave/test_newavetim.py
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/newave/test_nwv_avl_evap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/newave/test_nwv_cortes_evap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/newave/test_nwv_eco_evap.py
--rw-r--r--   0 runner    (1001) docker     (127)     7467 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/newave/test_parp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/newave/test_parpeol.py
--rw-r--r--   0 runner    (1001) docker     (127)     5896 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/newave/test_parpvaz.py
--rw-r--r--   0 runner    (1001) docker     (127)     6766 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/newave/test_patamar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/newave/test_penalid.py
--rw-r--r--   0 runner    (1001) docker     (127)    15289 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/newave/test_pmo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/newave/test_re.py
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/newave/test_ree.py
--rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/newave/test_selcor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/newave/test_shist.py
--rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/newave/test_sistema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/newave/test_term.py
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/newave/test_vazaob.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/newave/test_vazaof.py
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/newave/test_vazaos.py
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/newave/test_vazinat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/newave/test_vazoes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/newave/test_vazpast.py
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/newave/test_volrefsaz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 13:48:26.628419 inewave-1.7.3/tests/nwlistcf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistcf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistcf/test_arquivos.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistcf/test_caso.py
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistcf/test_estados.py
--rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistcf/test_nwlistcfdat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistcf/test_nwlistcfrel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 13:48:26.652419 inewave-1.7.3/tests/nwlistop/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_c_v_rhq.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_c_v_rhq_s.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_c_v_rhv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_c_v_rhv_s.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_cbomb.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_cbombsin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_cdef.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_cdefsin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_celetricas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_cmarg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_cmargmed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_coper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_corteolm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_cterm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_ctermsin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_deficit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_defsin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_deletricas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_depminuh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_desvuh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_dfphauh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_dlppdfmax.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_dlppdfmaxm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_dlppdfmaxs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_dlpptbmax.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_dlpptbmaxm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_dlpptbmaxs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_dnegevap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_dposevap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_dtbmax.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_dtbmin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_dvazmax.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_eaf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_eafb.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_eafbm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_eafbsin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_eafm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_earmf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_earmfm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_earmfp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_earmfpm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_earmfpsin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_earmfsin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_edesvc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_edesvcm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_edesvcsin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_evapo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_evapom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_evaporsin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_evert.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_evertm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_evertsin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_exces.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_excessin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_form_rhq.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_form_rhv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_fteolm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_fteolsin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_geol.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_geolm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_geolsin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_ghfphexat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_ghidr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_ghidrm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_ghidrsin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_ghiduh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_ghmax.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_ghmax_fpha.py
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_ghmax_fphc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_ghmaxm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_ghmaxmr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_ghmaxr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_ghmaxrsin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_ghmaxsin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_ghtot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_ghtotm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_ghtotsin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_gtert.py
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_gttot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_gttotsin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_hjus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_hliq.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_hmont.py
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_intercambio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_invade.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_invadem.py
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_mediasmerc.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_mediasree.py
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_mediasrep.py
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_mediasrhq.py
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_mediasrhv.py
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_mediassin.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_mediasusie.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_mediasusih.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_mediasusit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_mercl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_merclsin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_mevmin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_mevminm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_mevminsin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_nwlistopdat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_perdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_perdfm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_perdfsin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_pivarm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_pivarmincr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_qafluh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_qincruh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_rhslppdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_rhslpptb.py
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_vagua.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_varmpuh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_varmuh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_vbomb.py
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_vdesviouh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_vento.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_vertuh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_verturb.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_verturbm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_verturbsin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_vevapuh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_vevmin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_vevminm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_vevminsin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_vghmin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_vghminm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_vghminsin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_vghminuh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_viol_rhq.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_viol_rhv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_vmort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_vmortm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_vmortsin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-03-01 13:44:52.000000 inewave-1.7.3/tests/nwlistop/test_vturuh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:58:12.511383 inewave-1.7.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-12 14:54:32.000000 inewave-1.7.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-12 14:58:12.511383 inewave-1.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-12 14:54:32.000000 inewave-1.7.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:58:12.299381 inewave-1.7.4/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 14:54:32.000000 inewave-1.7.4/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-12 14:54:32.000000 inewave-1.7.4/examples/plot_dger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-04-12 14:54:32.000000 inewave-1.7.4/examples/plot_modif.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-12 14:54:32.000000 inewave-1.7.4/examples/plot_pmo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-12 14:54:32.000000 inewave-1.7.4/examples/plot_sistema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:58:12.299381 inewave-1.7.4/inewave/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:58:12.299381 inewave-1.7.4/inewave/_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5930 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/_utils/formatacao.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:58:12.299381 inewave-1.7.4/inewave/libs/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13324 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/libs/eolica.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:58:12.303381 inewave-1.7.4/inewave/libs/modelos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/libs/modelos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14151 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/libs/modelos/eolica.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19601 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/libs/modelos/restricoes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19927 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/libs/modelos/usinas_hidreletricas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16485 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/libs/restricoes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16373 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/libs/usinas_hidreletricas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:58:12.311381 inewave-1.7.4/inewave/newave/
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/abertura.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/adterm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/agrint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15168 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/arquivos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/avl_cortesfpha_nwv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/avl_desvfpha_s.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/avl_desvfpha_v_q.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/bid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/cadic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/caso.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/clasgas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/clast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/confhd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/conft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/cortes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12982 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/cortesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6744 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/curva.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/cvar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83959 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/dger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/dsvagua.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/eafpast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/eco_fpha.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/elnino.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/enavazb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/enavazf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/energiab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/energiaf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/energias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/engnat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/ensoaux.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/exph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/expt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38978 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/forward.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9876 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/forwarh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/gee.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/ghmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/gtminpat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11647 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/hidr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/itaipu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/manutt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:58:12.323381 inewave-1.7.4/inewave/newave/modelos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/abertura.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4977 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/adterm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7846 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/agrint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/arquivos.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:58:12.323381 inewave-1.7.4/inewave/newave/modelos/arquivoscsv/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/arquivoscsv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/arquivoscsv/arquivocsv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/avl_cortesfpha_nwv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/avl_desvfpha_s.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/avl_desvfpha_v_q.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/bid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:58:12.323381 inewave-1.7.4/inewave/newave/modelos/blocos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/blocos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/blocos/tabelacsv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/blocos/versaomodelo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5531 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/cadic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/caso.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/clasgas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7549 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/clast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3940 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/confhd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/conft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7388 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/cortes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30466 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/cortesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13812 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/curva.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7547 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/cvar.py
+-rw-r--r--   0 runner    (1001) docker     (127)   140730 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/dger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5560 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/dsvagua.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/eafpast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/eco_fpha.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/elnino.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/enavazb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/enavazf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/energiab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/energiaf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/energias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/engnat.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/ensoaux.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5520 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/exph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/expt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    87572 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/forward.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8200 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/forwarh.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/gee.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/ghmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/gtminpat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15742 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/hidr.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/itaipu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/manutt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16691 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/modif.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/newavetim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/nwv_avl_evap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/nwv_cortes_evap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/nwv_eco_evap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32022 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/parp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17352 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/parpeol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24383 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/parpvaz.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21478 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/patamar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/penalid.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/perda.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55244 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/pmo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6574 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/re.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/ree.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/sar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/selcor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/shist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23431 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/sistema.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/tecno.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4762 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/term.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/vazaob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/vazaof.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/vazaos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/vazinat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/vazoes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/vazpast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3459 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modelos/volref_saz.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13947 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/modif.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/newavetim.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/nwv_avl_evap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/nwv_cortes_evap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/nwv_eco_evap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18425 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/parp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12841 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/parpeol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15859 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/parpvaz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/patamar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/penalid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/perda.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19079 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/pmo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/re.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/ree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/sar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/selcor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/shist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/sistema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/tecno.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/term.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/vazaob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/vazaof.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/vazaos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/vazinat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/vazoes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/vazpast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/newave/volref_saz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:58:12.327381 inewave-1.7.4/inewave/nwlistcf/
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistcf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6739 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistcf/arquivos.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistcf/caso.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistcf/estados.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:58:12.327381 inewave-1.7.4/inewave/nwlistcf/modelos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistcf/modelos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistcf/modelos/arquivos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistcf/modelos/caso.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4300 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistcf/modelos/estados.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistcf/modelos/nwlistcfdat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistcf/modelos/nwlistcfrel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistcf/nwlistcfdat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistcf/nwlistcfrel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:58:12.347381 inewave-1.7.4/inewave/nwlistop/
+-rw-r--r--   0 runner    (1001) docker     (127)     4915 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/c_v_rhq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/c_v_rhq_s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/c_v_rhv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/c_v_rhv_s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/cbomb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/cbombsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/cdef.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/cdefsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/celetricas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/cmarg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/cmargmed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/coper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/corteolm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/cterm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/ctermsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/deficit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/defsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/deletricas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/depminuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/desvuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/dfphauh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/dlppdfmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/dlppdfmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/dlppdfmaxs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/dlpptbmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/dlpptbmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/dlpptbmaxs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/dnegevap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/dposevap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/dtbmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/dtbmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/dvazmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/eaf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/eafb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/eafbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/eafbsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/eafm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/earmf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/earmfm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/earmfp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/earmfpm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/earmfpsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/earmfsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/edesvc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/edesvcm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/edesvcsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/evapo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/evapom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/evaporsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/evert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/evertm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/evertsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/exces.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/excessin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/form_rhq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/form_rhv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/fteolm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/fteolsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/geol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/geolm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/geolsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/gh_fphexat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/ghidr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/ghidrm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/ghidrsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/ghiduh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/ghmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/ghmax_fpha.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/ghmax_fphc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/ghmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/ghmaxmr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/ghmaxr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/ghmaxrsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/ghmaxsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/ghtot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/ghtotm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/ghtotsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/gtert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/gttot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/gttotsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/hjus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/hliq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/hmont.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/intercambio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/invade.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/invadem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/mediasmerc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/mediasree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/mediasrep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/mediasrhq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/mediasrhv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/mediassin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/mediasusie.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/mediasusih.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/mediasusit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/mercl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/merclsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/mevmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/mevminm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/mevminsin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:58:12.375381 inewave-1.7.4/inewave/nwlistop/modelos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:58:12.375381 inewave-1.7.4/inewave/nwlistop/modelos/arquivos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/arquivos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/arquivos/arquivoclassetermicasubmercadopatamar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/arquivos/arquivoestacaobombeamentopatamar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/arquivos/arquivoparsubmercadopatamar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/arquivos/arquivoree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/arquivos/arquivoreepatamar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/arquivos/arquivorestricao.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/arquivos/arquivorestricaopatamar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/arquivos/arquivosin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/arquivos/arquivosinpatamar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/arquivos/arquivosubmercado.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/arquivos/arquivosubmercadopatamar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/arquivos/arquivousina.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/arquivos/arquivousinapatamar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:58:12.379382 inewave-1.7.4/inewave/nwlistop/modelos/blocos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/blocos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/blocos/estacaobombeamento.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/blocos/parsubmercados.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/blocos/ree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/blocos/restricao.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/blocos/submercado.py
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/blocos/usina.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/blocos/valoresclassetermicaseriepatamar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/blocos/valoresserie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/blocos/valoresseriepatamar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/c_v_rhq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/c_v_rhq_s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/c_v_rhv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/c_v_rhv_s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/cbomb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/cbombsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/cdef.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/cdefsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/celetricas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/cmarg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/cmargmed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/coper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/corteolm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/cterm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/ctermsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/def.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/defsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/deletricas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/depminuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/desvuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/dflppdfmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/dflpptbmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/dfphauh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/dlppdfmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/dlppdfmaxs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/dlpptbmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/dlpptbmaxs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/dnegevap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/dposevap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/dtbmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/dtbmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/dvazmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/eaf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/eafb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/eafbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/eafbsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/eafm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/earmf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/earmfm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/earmfp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/earmfpm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/earmfpsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/earmfsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/edesvc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/edesvcm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/edesvcsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/evapo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/evapom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/evaporsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/evert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/evertm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/evertsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/exces.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/excessin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/form_rhq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/form_rhv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/fteolm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/fteolsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/geol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/geolm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/geolsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/gh_fphexat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/ghidr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/ghidrm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/ghidrsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/ghiduh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/ghmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/ghmax_fpha.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/ghmax_fphc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/ghmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/ghmaxmr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/ghmaxr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/ghmaxrsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/ghmaxsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/ghtot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/ghtotm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/ghtotsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/gtert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/gttot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/gttotsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/hjus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/hliq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/hmont.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/intercambio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/invade.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/invadem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/mediasmerc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/mediasree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/mediasrep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/mediasrhq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/mediasrhv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/mediassin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/mediasusie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/mediasusih.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/mediasusit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/mercl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/merclsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/mevmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/mevminm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/mevminsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6752 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/nwlistopdat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/perdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/perdfm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/perdfsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/pivarm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/pivarmincr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/qafluh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/qincruh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/rhslppdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/rhslpptb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/vagua.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/varmpuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/varmuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/vbomb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/vdesviouh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/vento.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/vertuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/verturb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/verturbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/verturbsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/vevapuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/vevmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/vevminm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/vevminsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/vghmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/vghminm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/vghminsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/vghminuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/viol_rhq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/viol_rhv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/vmort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/vmortm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/vmortsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/modelos/vturuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7672 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/nwlistopdat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/perdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/perdfm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/perdfsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/pivarm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/pivarmincr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/qafluh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/qincruh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/rhslppdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/rhslpptb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/vagua.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/varmpuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/varmuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/vbomb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/vdesviouh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/vento.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/vertuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/verturb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/verturbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/verturbsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/vevapuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/vevmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/vevminm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/vevminsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/vghmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/vghminm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/vghminsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/vghminuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/viol_rhq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/viol_rhv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/vmort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/vmortm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/vmortsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/nwlistop/vturuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 14:54:32.000000 inewave-1.7.4/inewave/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:58:12.511383 inewave-1.7.4/inewave.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-12 14:58:12.000000 inewave-1.7.4/inewave.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    27157 2024-04-12 14:58:12.000000 inewave-1.7.4/inewave.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 14:58:12.000000 inewave-1.7.4/inewave.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-12 14:58:12.000000 inewave-1.7.4/inewave.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-12 14:58:12.000000 inewave-1.7.4/inewave.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 14:58:12.511383 inewave-1.7.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-12 14:54:32.000000 inewave-1.7.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:58:12.379382 inewave-1.7.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:58:12.379382 inewave-1.7.4/tests/_arquivos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/_arquivos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:58:12.379382 inewave-1.7.4/tests/libs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8406 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/libs/test_eolica.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9990 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/libs/test_restricoes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16413 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/libs/test_usinas_hidreletricas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:58:12.379382 inewave-1.7.4/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:58:12.479382 inewave-1.7.4/tests/mocks/arquivos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/adterm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/agrint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/arquivos.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/arquivos_nwlistcf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10255 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/avl_cortesfpha_nwv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/avl_desvfpha_s.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46951 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/avl_desvfpha_v_q.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24307 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/c_v_rhq.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24306 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/c_v_rhq_s.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9455 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/c_v_rhv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9463 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/c_v_rhv_s.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/cadic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/caso.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/caso_nwlistcf_nwlistop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24307 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/cbomb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24310 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/cbombsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/cdef.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/cdefsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24312 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/celetricas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30063 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/clast.py
+-rw-r--r--   0 runner    (1001) docker     (127)   847210 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/cmarg.py
+-rw-r--r--   0 runner    (1001) docker     (127)   295249 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/cmargmed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13487 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/confhd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6262 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/conft.py
+-rw-r--r--   0 runner    (1001) docker     (127)   295245 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/coper.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1105146 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/corteolm.py
+-rw-r--r--   0 runner    (1001) docker     (127)   295190 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/cterm.py
+-rw-r--r--   0 runner    (1001) docker     (127)   295196 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/ctermsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/curva.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/cvar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/deficit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/defsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24311 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/deletricas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/depminuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)   283211 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/desvuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)   847164 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/dfphauh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15257 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/dger.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1105161 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/dlppdfmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1105169 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/dlppdfmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1105154 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/dlppdfmaxs.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1105161 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/dlpptbmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1105169 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/dlpptbmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1105154 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/dlpptbmaxs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15309 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/dneg_evap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15309 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/dpos_evap.py
+-rw-r--r--   0 runner    (1001) docker     (127)   120243 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/dsvagua.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/dtbmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/dtbmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/dvazmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267099 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/eaf.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267152 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/eafb.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267153 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/eafbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267155 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/eafbsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267101 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/eafm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/eafpast.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267101 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/earmf.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267144 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/earmfm.py
+-rw-r--r--   0 runner    (1001) docker     (127)   291239 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/earmfp.py
+-rw-r--r--   0 runner    (1001) docker     (127)   291240 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/earmfpm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14002 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/earmfpsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267156 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/earmfsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)   232674 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/eco_fpha.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267116 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/edesvc.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267119 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/edesvcm.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267121 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/edesvcsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/eolica.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56476 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/estados.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267117 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/evapo.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267118 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/evapom.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267121 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/evaporsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267137 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/evert.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267138 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/evertm.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267139 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/evertsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1104654 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/exces.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1104652 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/excessin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/exph.py
+-rw-r--r--   0 runner    (1001) docker     (127)   120990 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/expt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24311 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/form_rhq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9464 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/form_rhv.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1104650 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/fteolm.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1104652 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/fteolsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1105178 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/geol.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1105179 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/geolm.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1105181 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/geolsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19859 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/gh_fphexat.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1105153 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/ghidr.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1105154 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/ghidrm.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1105156 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/ghidrsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)   847144 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/ghiduh.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1105136 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/ghmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19895 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/ghmax_fpha.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19898 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/ghmax_fphc.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1105138 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/ghmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1105139 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/ghmaxmr.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1105138 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/ghmaxr.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1105141 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/ghmaxrsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1105140 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/ghmaxsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/ghmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1105189 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/ghtot.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1105190 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/ghtotm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49768 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/ghtotsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26457 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/gtert.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1105188 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/gttot.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1105191 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/gttotsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)   846407 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/hjus.py
+-rw-r--r--   0 runner    (1001) docker     (127)   846407 2024-04-12 14:54:32.000000 inewave-1.7.4/tests/mocks/arquivos/hliq.py
+-rw-r--r--   0 runner    (1001) docker     (127)   425676 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/mocks/arquivos/hmont.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1087195 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/mocks/arquivos/intercambio.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267122 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/mocks/arquivos/invade.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267130 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/mocks/arquivos/invadem.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49720 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/mocks/arquivos/manutt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/mocks/arquivos/mercl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/mocks/arquivos/merclsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267116 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/mocks/arquivos/mevmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267117 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/mocks/arquivos/mevminm.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267118 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/mocks/arquivos/mevminsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57012 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/mocks/arquivos/modif.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45543 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/mocks/arquivos/newavetim.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/mocks/arquivos/nwlistcfdat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    76521 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/mocks/arquivos/nwlistcfrel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/mocks/arquivos/nwlistopdat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9502 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/mocks/arquivos/nwv_avl_evap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12629 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/mocks/arquivos/nwv_cortes_evap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10775 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/mocks/arquivos/nwv_eco_evap.py
+-rw-r--r--   0 runner    (1001) docker     (127)   378349 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/mocks/arquivos/parp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50087 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/mocks/arquivos/parpeol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38585 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/mocks/arquivos/parpvaz.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52098 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/mocks/arquivos/patamar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/mocks/arquivos/penalid.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267136 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/mocks/arquivos/perdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267137 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/mocks/arquivos/perdfm.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267139 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/mocks/arquivos/perdfsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)   425677 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/mocks/arquivos/pivarm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14847 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/mocks/arquivos/pivarmincr.py
+-rw-r--r--   0 runner    (1001) docker     (127)   657056 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/mocks/arquivos/pmo.py
+-rw-r--r--   0 runner    (1001) docker     (127)   283145 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/mocks/arquivos/qafluh.py
+-rw-r--r--   0 runner    (1001) docker     (127)   283145 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/mocks/arquivos/qincruh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/mocks/arquivos/re.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/mocks/arquivos/ree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4426 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/mocks/arquivos/restricoes.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1105160 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/mocks/arquivos/rhslppdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1105160 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/mocks/arquivos/rhslpptb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/mocks/arquivos/selcor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/mocks/arquivos/shist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20855 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/mocks/arquivos/sistema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18692 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/mocks/arquivos/term.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38821 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/mocks/arquivos/usinas_hidreletricas.py
+-rw-r--r--   0 runner    (1001) docker     (127)   271157 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/mocks/arquivos/vagua.py
+-rw-r--r--   0 runner    (1001) docker     (127)   283139 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/mocks/arquivos/varmpuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)   283209 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/mocks/arquivos/varmuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32259 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/mocks/arquivos/vazpast.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24306 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/mocks/arquivos/vbomb.py
+-rw-r--r--   0 runner    (1001) docker     (127)   847213 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/mocks/arquivos/vdesviouh.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267101 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/mocks/arquivos/vento.py
+-rw-r--r--   0 runner    (1001) docker     (127)   847200 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/mocks/arquivos/vertuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267155 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/mocks/arquivos/verturb.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267156 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/mocks/arquivos/verturbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267158 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/mocks/arquivos/verturbsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15308 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/mocks/arquivos/vevapuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267122 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/mocks/arquivos/vevmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267130 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/mocks/arquivos/vevminm.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267117 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/mocks/arquivos/vevminsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1105173 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/mocks/arquivos/vghmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1105174 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/mocks/arquivos/vghminm.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1105176 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/mocks/arquivos/vghminsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)   847195 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/mocks/arquivos/vghminuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24310 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/mocks/arquivos/viol_rhq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9463 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/mocks/arquivos/viol_rhv.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267115 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/mocks/arquivos/vmort.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267116 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/mocks/arquivos/vmortm.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267118 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/mocks/arquivos/vmortsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25446 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/mocks/arquivos/volref_saz.py
+-rw-r--r--   0 runner    (1001) docker     (127)   847135 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/mocks/arquivos/vturuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/mocks/mock_open.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:58:12.487383 inewave-1.7.4/tests/newave/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/newave/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/newave/test_adterm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/newave/test_agrint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5298 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/newave/test_arquivos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/newave/test_avl_cortesfpha_nwv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/newave/test_avl_desvfpha_s.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/newave/test_avl_desvfpha_v_q.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/newave/test_cadic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/newave/test_caso.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/newave/test_clast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/newave/test_confhd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/newave/test_conft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/newave/test_cortes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/newave/test_cortesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/newave/test_curva.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/newave/test_cvar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52070 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/newave/test_dger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/newave/test_dsvagua.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/newave/test_eafpast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/newave/test_eco_fpha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/newave/test_enavazb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/newave/test_enavazf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/newave/test_energiab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/newave/test_energiaf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/newave/test_energias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/newave/test_engnat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/newave/test_exph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/newave/test_expt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36320 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/newave/test_forward.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/newave/test_forwarh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/newave/test_ghmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/newave/test_hidr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/newave/test_manutt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8825 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/newave/test_modif.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/newave/test_newavetim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/newave/test_nwv_avl_evap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/newave/test_nwv_cortes_evap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/newave/test_nwv_eco_evap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7467 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/newave/test_parp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/newave/test_parpeol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5896 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/newave/test_parpvaz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6766 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/newave/test_patamar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/newave/test_penalid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15289 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/newave/test_pmo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/newave/test_re.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/newave/test_ree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/newave/test_selcor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/newave/test_shist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/newave/test_sistema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/newave/test_term.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/newave/test_vazaob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/newave/test_vazaof.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/newave/test_vazaos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/newave/test_vazinat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/newave/test_vazoes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/newave/test_vazpast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/newave/test_volrefsaz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:58:12.491382 inewave-1.7.4/tests/nwlistcf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistcf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistcf/test_arquivos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistcf/test_caso.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistcf/test_estados.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistcf/test_nwlistcfdat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistcf/test_nwlistcfrel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:58:12.511383 inewave-1.7.4/tests/nwlistop/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_c_v_rhq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_c_v_rhq_s.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_c_v_rhv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_c_v_rhv_s.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_cbomb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_cbombsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_cdef.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_cdefsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_celetricas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_cmarg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_cmargmed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_coper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_corteolm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_cterm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_ctermsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_deficit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_defsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_deletricas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_depminuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_desvuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_dfphauh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_dlppdfmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_dlppdfmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_dlppdfmaxs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_dlpptbmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_dlpptbmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_dlpptbmaxs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_dnegevap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_dposevap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_dtbmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_dtbmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_dvazmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_eaf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_eafb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_eafbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_eafbsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_eafm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_earmf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_earmfm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_earmfp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_earmfpm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_earmfpsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_earmfsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_edesvc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_edesvcm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_edesvcsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_evapo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_evapom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_evaporsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_evert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_evertm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_evertsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_exces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_excessin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_form_rhq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_form_rhv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_fteolm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_fteolsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_geol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_geolm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_geolsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_ghfphexat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_ghidr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_ghidrm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_ghidrsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_ghiduh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_ghmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_ghmax_fpha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_ghmax_fphc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_ghmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_ghmaxmr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_ghmaxr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_ghmaxrsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_ghmaxsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_ghtot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_ghtotm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_ghtotsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_gtert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_gttot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_gttotsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_hjus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_hliq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_hmont.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_intercambio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_invade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_invadem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_mediasmerc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_mediasree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_mediasrep.py
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_mediasrhq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_mediasrhv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_mediassin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_mediasusie.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_mediasusih.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_mediasusit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_mercl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_merclsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_mevmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_mevminm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_mevminsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_nwlistopdat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_perdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_perdfm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_perdfsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_pivarm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_pivarmincr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_qafluh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_qincruh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_rhslppdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_rhslpptb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_vagua.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_varmpuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_varmuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_vbomb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_vdesviouh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_vento.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_vertuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_verturb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_verturbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_verturbsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_vevapuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_vevmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_vevminm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_vevminsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_vghmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_vghminm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_vghminsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_vghminuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_viol_rhq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_viol_rhv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_vmort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_vmortm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_vmortsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-12 14:54:33.000000 inewave-1.7.4/tests/nwlistop/test_vturuh.py
```

### Comparing `inewave-1.7.3/LICENSE.md` & `inewave-1.7.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/PKG-INFO` & `inewave-1.7.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inewave
-Version: 1.7.3
+Version: 1.7.4
 Summary: Interface para arquivos do NEWAVE
 Home-page: https://github.com/rjmalves/inewave
 Author: Rogerio Alves
 Author-email: rogerioalves.ee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `inewave-1.7.3/README.md` & `inewave-1.7.4/README.md`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/examples/plot_dger.py` & `inewave-1.7.4/examples/plot_dger.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/examples/plot_modif.py` & `inewave-1.7.4/examples/plot_modif.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/examples/plot_pmo.py` & `inewave-1.7.4/examples/plot_pmo.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/examples/plot_sistema.py` & `inewave-1.7.4/examples/plot_sistema.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/_utils/formatacao.py` & `inewave-1.7.4/inewave/_utils/formatacao.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/config.py` & `inewave-1.7.4/inewave/config.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/libs/eolica.py` & `inewave-1.7.4/inewave/libs/eolica.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/libs/modelos/eolica.py` & `inewave-1.7.4/inewave/libs/modelos/eolica.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/libs/modelos/restricoes.py` & `inewave-1.7.4/inewave/libs/modelos/restricoes.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/libs/modelos/usinas_hidreletricas.py` & `inewave-1.7.4/inewave/libs/modelos/usinas_hidreletricas.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/libs/restricoes.py` & `inewave-1.7.4/inewave/libs/restricoes.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/libs/usinas_hidreletricas.py` & `inewave-1.7.4/inewave/libs/usinas_hidreletricas.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/__init__.py` & `inewave-1.7.4/inewave/newave/__init__.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/adterm.py` & `inewave-1.7.4/inewave/newave/adterm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/agrint.py` & `inewave-1.7.4/inewave/newave/agrint.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/arquivos.py` & `inewave-1.7.4/inewave/newave/arquivos.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/avl_cortesfpha_nwv.py` & `inewave-1.7.4/inewave/newave/avl_cortesfpha_nwv.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/avl_desvfpha_s.py` & `inewave-1.7.4/inewave/newave/avl_desvfpha_s.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/avl_desvfpha_v_q.py` & `inewave-1.7.4/inewave/newave/avl_desvfpha_v_q.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/cadic.py` & `inewave-1.7.4/inewave/newave/cadic.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/caso.py` & `inewave-1.7.4/inewave/newave/caso.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/clast.py` & `inewave-1.7.4/inewave/newave/clast.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/confhd.py` & `inewave-1.7.4/inewave/newave/confhd.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/conft.py` & `inewave-1.7.4/inewave/newave/conft.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/cortes.py` & `inewave-1.7.4/inewave/newave/cortes.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/cortesh.py` & `inewave-1.7.4/inewave/newave/cortesh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/curva.py` & `inewave-1.7.4/inewave/newave/curva.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/cvar.py` & `inewave-1.7.4/inewave/newave/cvar.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/dger.py` & `inewave-1.7.4/inewave/newave/dger.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/dsvagua.py` & `inewave-1.7.4/inewave/newave/dsvagua.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/eafpast.py` & `inewave-1.7.4/inewave/newave/eafpast.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/eco_fpha.py` & `inewave-1.7.4/inewave/newave/eco_fpha.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/enavazb.py` & `inewave-1.7.4/inewave/newave/enavazb.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/enavazf.py` & `inewave-1.7.4/inewave/newave/enavazf.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/energiab.py` & `inewave-1.7.4/inewave/newave/energiab.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/energiaf.py` & `inewave-1.7.4/inewave/newave/energiaf.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/energias.py` & `inewave-1.7.4/inewave/newave/energias.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/engnat.py` & `inewave-1.7.4/inewave/newave/engnat.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/exph.py` & `inewave-1.7.4/inewave/newave/exph.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/expt.py` & `inewave-1.7.4/inewave/newave/expt.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/forward.py` & `inewave-1.7.4/inewave/newave/forward.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/forwarh.py` & `inewave-1.7.4/inewave/newave/forwarh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/ghmin.py` & `inewave-1.7.4/inewave/newave/ghmin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/hidr.py` & `inewave-1.7.4/inewave/newave/hidr.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/manutt.py` & `inewave-1.7.4/inewave/newave/manutt.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/modelos/adterm.py` & `inewave-1.7.4/inewave/newave/modelos/adterm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/modelos/agrint.py` & `inewave-1.7.4/inewave/newave/modelos/agrint.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/modelos/arquivos.py` & `inewave-1.7.4/inewave/newave/modelos/arquivos.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/modelos/arquivoscsv/arquivocsv.py` & `inewave-1.7.4/inewave/newave/modelos/arquivoscsv/arquivocsv.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/modelos/avl_cortesfpha_nwv.py` & `inewave-1.7.4/inewave/newave/modelos/avl_cortesfpha_nwv.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/modelos/avl_desvfpha_s.py` & `inewave-1.7.4/inewave/newave/modelos/avl_desvfpha_s.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/modelos/avl_desvfpha_v_q.py` & `inewave-1.7.4/inewave/newave/modelos/avl_desvfpha_v_q.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/modelos/blocos/tabelacsv.py` & `inewave-1.7.4/inewave/newave/modelos/blocos/tabelacsv.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/modelos/blocos/versaomodelo.py` & `inewave-1.7.4/inewave/newave/modelos/blocos/versaomodelo.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/modelos/cadic.py` & `inewave-1.7.4/inewave/newave/modelos/cadic.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/modelos/caso.py` & `inewave-1.7.4/inewave/newave/modelos/caso.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/modelos/clast.py` & `inewave-1.7.4/inewave/newave/modelos/clast.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/modelos/confhd.py` & `inewave-1.7.4/inewave/newave/modelos/confhd.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/modelos/conft.py` & `inewave-1.7.4/inewave/newave/modelos/conft.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/modelos/cortes.py` & `inewave-1.7.4/inewave/newave/modelos/cortes.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/modelos/cortesh.py` & `inewave-1.7.4/inewave/newave/modelos/cortesh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/modelos/curva.py` & `inewave-1.7.4/inewave/newave/modelos/curva.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/modelos/cvar.py` & `inewave-1.7.4/inewave/newave/modelos/cvar.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/modelos/dger.py` & `inewave-1.7.4/inewave/newave/modelos/dger.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/modelos/dsvagua.py` & `inewave-1.7.4/inewave/newave/modelos/dsvagua.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/modelos/eafpast.py` & `inewave-1.7.4/inewave/newave/modelos/eafpast.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/modelos/eco_fpha.py` & `inewave-1.7.4/inewave/newave/modelos/eco_fpha.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/modelos/enavazb.py` & `inewave-1.7.4/inewave/newave/modelos/enavazb.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/modelos/enavazf.py` & `inewave-1.7.4/inewave/newave/modelos/enavazf.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/modelos/energiab.py` & `inewave-1.7.4/inewave/newave/modelos/energiab.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/modelos/energiaf.py` & `inewave-1.7.4/inewave/newave/modelos/energiaf.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/modelos/energias.py` & `inewave-1.7.4/inewave/newave/modelos/vazaos.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,76 +2,76 @@
 from cfinterface.components.line import Line
 from cfinterface.components.floatfield import FloatField
 from typing import IO
 import pandas as pd  # type: ignore
 import numpy as np  # type: ignore
 
 
-class SecaoDadosEnergias(Section):
+class SecaoDadosVazaos(Section):
     """
-    Registro com os dados das séries sintéticas de energia existentes
-    no arquivo energias.dat.
+    Registro com os dados das séries sintéticas de vazão existentes
+    no arquivo vazaos.dat.
     """
 
     def __init__(self, previous=None, next=None, data=None) -> None:
         super().__init__(previous, next, data)
 
     def __eq__(self, o: object) -> bool:
-        if not isinstance(o, SecaoDadosEnergias):
+        if not isinstance(o, SecaoDadosVazaos):
             return False
-        bloco: SecaoDadosEnergias = o
+        bloco: SecaoDadosVazaos = o
         if not all(
             [
                 isinstance(self.data, pd.DataFrame),
                 isinstance(o.data, pd.DataFrame),
             ]
         ):
             return False
         else:
             return self.data.equals(bloco.data)
 
     def read(
         self,
         file: IO,
         numero_series: int = 2000,
-        numero_rees: int = 12,
+        numero_uhes: int = 164,
         numero_estagios: int = 60,
         numero_estagios_th: int = 12,
         *args,
         **kwargs,
     ):
         numero_registros = (
             (numero_estagios + numero_estagios_th)
-            * numero_rees
+            * numero_uhes
             * numero_series
         )
         self.__linha = Line(
             [
                 FloatField(size=8, starting_position=8 * i)
                 for i in range(numero_registros)
             ],
             storage="BINARY",
         )
         dados = self.__linha.read(file.read(self.__linha.size))
         indices_estagios = np.arange(
             1 - numero_estagios_th, numero_estagios + 1
         )
-        estagios_df = np.repeat(indices_estagios, numero_series * numero_rees)
-        rees_df = np.tile(
-            np.repeat(np.arange(1, numero_rees + 1), numero_series),
+        estagios_df = np.repeat(indices_estagios, numero_series * numero_uhes)
+        uhes_df = np.tile(
+            np.repeat(np.arange(1, numero_uhes + 1), numero_series),
             numero_estagios + numero_estagios_th,
         )
         series_df = np.tile(
             np.arange(1, numero_series + 1),
-            numero_rees * (numero_estagios + numero_estagios_th),
+            numero_uhes * (numero_estagios + numero_estagios_th),
         )
         df = pd.DataFrame(
             data={
                 "estagio": estagios_df,
-                "ree": rees_df,
+                "uhe": uhes_df,
                 "serie": series_df,
                 "valor": dados,
             }
         )
         self.data = df
 
     def write(self, file: IO, *args, **kwargs):
```

### Comparing `inewave-1.7.3/inewave/newave/modelos/engnat.py` & `inewave-1.7.4/inewave/newave/modelos/engnat.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/modelos/exph.py` & `inewave-1.7.4/inewave/newave/modelos/exph.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/modelos/expt.py` & `inewave-1.7.4/inewave/newave/modelos/expt.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/modelos/forward.py` & `inewave-1.7.4/inewave/newave/modelos/forward.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/modelos/forwarh.py` & `inewave-1.7.4/inewave/newave/modelos/forwarh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/modelos/ghmin.py` & `inewave-1.7.4/inewave/newave/modelos/ghmin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/modelos/hidr.py` & `inewave-1.7.4/inewave/newave/modelos/hidr.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/modelos/manutt.py` & `inewave-1.7.4/inewave/newave/modelos/manutt.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/modelos/modif.py` & `inewave-1.7.4/inewave/newave/modelos/modif.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/modelos/newavetim.py` & `inewave-1.7.4/inewave/newave/modelos/newavetim.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/modelos/nwv_avl_evap.py` & `inewave-1.7.4/inewave/newave/modelos/nwv_avl_evap.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/modelos/nwv_cortes_evap.py` & `inewave-1.7.4/inewave/newave/modelos/nwv_cortes_evap.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/modelos/nwv_eco_evap.py` & `inewave-1.7.4/inewave/newave/modelos/nwv_eco_evap.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/modelos/parp.py` & `inewave-1.7.4/inewave/newave/modelos/parp.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/modelos/parpeol.py` & `inewave-1.7.4/inewave/newave/modelos/parpeol.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/modelos/parpvaz.py` & `inewave-1.7.4/inewave/newave/modelos/parpvaz.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/modelos/patamar.py` & `inewave-1.7.4/inewave/newave/modelos/patamar.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/modelos/penalid.py` & `inewave-1.7.4/inewave/newave/modelos/penalid.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/modelos/pmo.py` & `inewave-1.7.4/inewave/newave/modelos/pmo.py`

 * *Files 1% similar despite different names*

```diff
@@ -412,15 +412,17 @@
         )
         i = 0
         while True:
             linha: str = file.readline()
             # Confere se acabou
             if len(linha) < 3 or "X--------------------" in linha:
                 tabela = tabela[:i, :]
-                self.data = converte_tabela_em_df()
+                self.data = (
+                    converte_tabela_em_df() if i > 0 else pd.DataFrame()
+                )
                 break
             # Lê mais uma linha
             dados = self.__line.read(linha)
             if dados[0] is not None:
                 codigo_atual = dados[0]
             if len(dados[1]) > 0:
                 nome_atual = dados[1]
@@ -496,15 +498,17 @@
         )
         i = 0
         while True:
             linha: str = file.readline()
             # Confere se acabou
             if len(linha) < 3 or "X--------------------" in linha:
                 tabela = tabela[:i, :]
-                self.data = converte_tabela_em_df()
+                self.data = (
+                    converte_tabela_em_df() if i > 0 else pd.DataFrame()
+                )
                 break
             # Lê mais uma linha
             dados = self.__line.read(linha)
             if dados[0] is not None:
                 codigo_atual = dados[0]
             if len(dados[1]) > 0:
                 nome_atual = dados[1]
```

### Comparing `inewave-1.7.3/inewave/newave/modelos/re.py` & `inewave-1.7.4/inewave/newave/modelos/re.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/modelos/ree.py` & `inewave-1.7.4/inewave/newave/modelos/ree.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/modelos/selcor.py` & `inewave-1.7.4/inewave/newave/modelos/selcor.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/modelos/shist.py` & `inewave-1.7.4/inewave/newave/modelos/shist.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/modelos/sistema.py` & `inewave-1.7.4/inewave/newave/modelos/sistema.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/modelos/term.py` & `inewave-1.7.4/inewave/newave/modelos/term.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/modelos/vazaob.py` & `inewave-1.7.4/inewave/newave/modelos/vazaob.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/modelos/vazaof.py` & `inewave-1.7.4/inewave/newave/modelos/vazaof.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/modelos/vazinat.py` & `inewave-1.7.4/inewave/newave/modelos/vazinat.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/modelos/vazoes.py` & `inewave-1.7.4/inewave/newave/modelos/vazoes.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/modelos/vazpast.py` & `inewave-1.7.4/inewave/newave/modelos/vazpast.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/modelos/volref_saz.py` & `inewave-1.7.4/inewave/newave/modelos/volref_saz.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/modif.py` & `inewave-1.7.4/inewave/newave/modif.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/newavetim.py` & `inewave-1.7.4/inewave/newave/newavetim.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/nwv_avl_evap.py` & `inewave-1.7.4/inewave/newave/nwv_avl_evap.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/nwv_cortes_evap.py` & `inewave-1.7.4/inewave/newave/nwv_cortes_evap.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/nwv_eco_evap.py` & `inewave-1.7.4/inewave/newave/nwv_eco_evap.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/parp.py` & `inewave-1.7.4/inewave/newave/parp.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/parpeol.py` & `inewave-1.7.4/inewave/newave/parpeol.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/parpvaz.py` & `inewave-1.7.4/inewave/newave/parpvaz.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/patamar.py` & `inewave-1.7.4/inewave/newave/patamar.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/penalid.py` & `inewave-1.7.4/inewave/newave/penalid.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/pmo.py` & `inewave-1.7.4/inewave/newave/pmo.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/re.py` & `inewave-1.7.4/inewave/newave/re.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/ree.py` & `inewave-1.7.4/inewave/newave/ree.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/selcor.py` & `inewave-1.7.4/inewave/newave/selcor.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/shist.py` & `inewave-1.7.4/inewave/newave/shist.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/sistema.py` & `inewave-1.7.4/inewave/newave/sistema.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/term.py` & `inewave-1.7.4/inewave/newave/term.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/vazaob.py` & `inewave-1.7.4/inewave/newave/vazaob.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/vazaof.py` & `inewave-1.7.4/inewave/newave/vazaof.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/vazaos.py` & `inewave-1.7.4/inewave/newave/vazaos.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/vazinat.py` & `inewave-1.7.4/inewave/newave/vazinat.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/vazoes.py` & `inewave-1.7.4/inewave/newave/vazoes.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/vazpast.py` & `inewave-1.7.4/inewave/newave/vazpast.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/newave/volref_saz.py` & `inewave-1.7.4/inewave/newave/volref_saz.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistcf/arquivos.py` & `inewave-1.7.4/inewave/nwlistcf/arquivos.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistcf/caso.py` & `inewave-1.7.4/inewave/nwlistcf/caso.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistcf/estados.py` & `inewave-1.7.4/inewave/nwlistcf/estados.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistcf/modelos/arquivos.py` & `inewave-1.7.4/inewave/nwlistcf/modelos/arquivos.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistcf/modelos/caso.py` & `inewave-1.7.4/inewave/nwlistcf/modelos/caso.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistcf/modelos/estados.py` & `inewave-1.7.4/inewave/nwlistcf/modelos/estados.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistcf/modelos/nwlistcfdat.py` & `inewave-1.7.4/inewave/nwlistcf/modelos/nwlistcfdat.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistcf/modelos/nwlistcfrel.py` & `inewave-1.7.4/inewave/nwlistcf/modelos/nwlistcfrel.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistcf/nwlistcfdat.py` & `inewave-1.7.4/inewave/nwlistcf/nwlistcfdat.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistcf/nwlistcfrel.py` & `inewave-1.7.4/inewave/nwlistcf/nwlistcfrel.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/__init__.py` & `inewave-1.7.4/inewave/nwlistop/__init__.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/c_v_rhq.py` & `inewave-1.7.4/inewave/nwlistop/c_v_rhq.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/c_v_rhv.py` & `inewave-1.7.4/inewave/nwlistop/c_v_rhv.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/cbomb.py` & `inewave-1.7.4/inewave/nwlistop/cbomb.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/cmarg.py` & `inewave-1.7.4/inewave/nwlistop/cmarg.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/cmargmed.py` & `inewave-1.7.4/inewave/nwlistop/cmargmed.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/corteolm.py` & `inewave-1.7.4/inewave/nwlistop/corteolm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/cterm.py` & `inewave-1.7.4/inewave/nwlistop/cterm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/deficit.py` & `inewave-1.7.4/inewave/nwlistop/deficit.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/depminuh.py` & `inewave-1.7.4/inewave/nwlistop/depminuh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/desvuh.py` & `inewave-1.7.4/inewave/nwlistop/desvuh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/dfphauh.py` & `inewave-1.7.4/inewave/nwlistop/dfphauh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/dlppdfmax.py` & `inewave-1.7.4/inewave/nwlistop/dlppdfmax.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/dlppdfmaxm.py` & `inewave-1.7.4/inewave/nwlistop/dlppdfmaxm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/dlpptbmax.py` & `inewave-1.7.4/inewave/nwlistop/dlpptbmax.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/dlpptbmaxm.py` & `inewave-1.7.4/inewave/nwlistop/dlpptbmaxm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/dnegevap.py` & `inewave-1.7.4/inewave/nwlistop/dnegevap.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/dposevap.py` & `inewave-1.7.4/inewave/nwlistop/dposevap.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/dtbmax.py` & `inewave-1.7.4/inewave/nwlistop/dtbmax.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/dtbmin.py` & `inewave-1.7.4/inewave/nwlistop/dtbmin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/dvazmax.py` & `inewave-1.7.4/inewave/nwlistop/dvazmax.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/eafb.py` & `inewave-1.7.4/inewave/nwlistop/eafb.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/eafbm.py` & `inewave-1.7.4/inewave/nwlistop/eafbm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/eafm.py` & `inewave-1.7.4/inewave/nwlistop/eafm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/earmf.py` & `inewave-1.7.4/inewave/nwlistop/earmf.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/earmfm.py` & `inewave-1.7.4/inewave/nwlistop/earmfm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/earmfp.py` & `inewave-1.7.4/inewave/nwlistop/earmfp.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/earmfpm.py` & `inewave-1.7.4/inewave/nwlistop/earmfpm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/earmfpsin.py` & `inewave-1.7.4/inewave/nwlistop/earmfpsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/edesvc.py` & `inewave-1.7.4/inewave/nwlistop/edesvc.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/edesvcm.py` & `inewave-1.7.4/inewave/nwlistop/edesvcm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/evapo.py` & `inewave-1.7.4/inewave/nwlistop/evapo.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/evapom.py` & `inewave-1.7.4/inewave/nwlistop/evapom.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/evert.py` & `inewave-1.7.4/inewave/nwlistop/evert.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/evertm.py` & `inewave-1.7.4/inewave/nwlistop/evertm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/exces.py` & `inewave-1.7.4/inewave/nwlistop/exces.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/form_rhq.py` & `inewave-1.7.4/inewave/nwlistop/form_rhq.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/form_rhv.py` & `inewave-1.7.4/inewave/nwlistop/form_rhv.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/fteolm.py` & `inewave-1.7.4/inewave/nwlistop/fteolm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/geol.py` & `inewave-1.7.4/inewave/nwlistop/geol.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/geolm.py` & `inewave-1.7.4/inewave/nwlistop/geolm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/gh_fphexat.py` & `inewave-1.7.4/inewave/nwlistop/gh_fphexat.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/ghidr.py` & `inewave-1.7.4/inewave/nwlistop/ghidr.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/ghidrm.py` & `inewave-1.7.4/inewave/nwlistop/ghidrm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/ghiduh.py` & `inewave-1.7.4/inewave/nwlistop/ghiduh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/ghmax.py` & `inewave-1.7.4/inewave/nwlistop/ghmax.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/ghmax_fpha.py` & `inewave-1.7.4/inewave/nwlistop/ghmax_fpha.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/ghmax_fphc.py` & `inewave-1.7.4/inewave/nwlistop/ghmax_fphc.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/ghmaxm.py` & `inewave-1.7.4/inewave/nwlistop/ghmaxm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/ghmaxmr.py` & `inewave-1.7.4/inewave/nwlistop/ghmaxmr.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/ghmaxr.py` & `inewave-1.7.4/inewave/nwlistop/ghmaxr.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/ghtot.py` & `inewave-1.7.4/inewave/nwlistop/ghtot.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/ghtotm.py` & `inewave-1.7.4/inewave/nwlistop/ghtotm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/gtert.py` & `inewave-1.7.4/inewave/nwlistop/gtert.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/gttot.py` & `inewave-1.7.4/inewave/nwlistop/gttot.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/hjus.py` & `inewave-1.7.4/inewave/nwlistop/hjus.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/hliq.py` & `inewave-1.7.4/inewave/nwlistop/hliq.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/hmont.py` & `inewave-1.7.4/inewave/nwlistop/hmont.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/intercambio.py` & `inewave-1.7.4/inewave/nwlistop/intercambio.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/invade.py` & `inewave-1.7.4/inewave/nwlistop/invade.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/invadem.py` & `inewave-1.7.4/inewave/nwlistop/invadem.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/mediasmerc.py` & `inewave-1.7.4/inewave/nwlistop/mediasmerc.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/mediasree.py` & `inewave-1.7.4/inewave/nwlistop/mediasree.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/mediasrep.py` & `inewave-1.7.4/inewave/nwlistop/mediasrep.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/mediasrhq.py` & `inewave-1.7.4/inewave/nwlistop/mediasrhq.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/mediasrhv.py` & `inewave-1.7.4/inewave/nwlistop/mediasrhv.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/mediassin.py` & `inewave-1.7.4/inewave/nwlistop/mediassin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/mediasusie.py` & `inewave-1.7.4/inewave/nwlistop/mediasusie.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/mediasusih.py` & `inewave-1.7.4/inewave/nwlistop/mediasusih.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/mediasusit.py` & `inewave-1.7.4/inewave/nwlistop/mediasusit.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/mercl.py` & `inewave-1.7.4/inewave/nwlistop/mercl.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/mevmin.py` & `inewave-1.7.4/inewave/nwlistop/mevmin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/mevminm.py` & `inewave-1.7.4/inewave/nwlistop/mevminm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/arquivos/arquivoclassetermicasubmercadopatamar.py` & `inewave-1.7.4/inewave/nwlistop/modelos/arquivos/arquivoclassetermicasubmercadopatamar.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/arquivos/arquivoestacaobombeamentopatamar.py` & `inewave-1.7.4/inewave/nwlistop/modelos/arquivos/arquivoestacaobombeamentopatamar.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/arquivos/arquivoparsubmercadopatamar.py` & `inewave-1.7.4/inewave/nwlistop/modelos/arquivos/arquivoparsubmercadopatamar.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/arquivos/arquivoree.py` & `inewave-1.7.4/inewave/nwlistop/modelos/arquivos/arquivoree.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/arquivos/arquivoreepatamar.py` & `inewave-1.7.4/inewave/nwlistop/modelos/arquivos/arquivoreepatamar.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/arquivos/arquivorestricao.py` & `inewave-1.7.4/inewave/nwlistop/modelos/arquivos/arquivorestricao.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/arquivos/arquivorestricaopatamar.py` & `inewave-1.7.4/inewave/nwlistop/modelos/arquivos/arquivorestricaopatamar.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/arquivos/arquivosin.py` & `inewave-1.7.4/inewave/nwlistop/modelos/arquivos/arquivosin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/arquivos/arquivosinpatamar.py` & `inewave-1.7.4/inewave/nwlistop/modelos/arquivos/arquivosinpatamar.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/arquivos/arquivosubmercado.py` & `inewave-1.7.4/inewave/nwlistop/modelos/arquivos/arquivosubmercado.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/arquivos/arquivosubmercadopatamar.py` & `inewave-1.7.4/inewave/nwlistop/modelos/arquivos/arquivosubmercadopatamar.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/arquivos/arquivousina.py` & `inewave-1.7.4/inewave/nwlistop/modelos/arquivos/arquivousina.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/arquivos/arquivousinapatamar.py` & `inewave-1.7.4/inewave/nwlistop/modelos/arquivos/arquivousinapatamar.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/blocos/estacaobombeamento.py` & `inewave-1.7.4/inewave/nwlistop/modelos/blocos/estacaobombeamento.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/blocos/parsubmercados.py` & `inewave-1.7.4/inewave/nwlistop/modelos/blocos/parsubmercados.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/blocos/ree.py` & `inewave-1.7.4/inewave/nwlistop/modelos/blocos/ree.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/blocos/restricao.py` & `inewave-1.7.4/inewave/nwlistop/modelos/blocos/restricao.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/blocos/submercado.py` & `inewave-1.7.4/inewave/nwlistop/modelos/blocos/submercado.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/blocos/usina.py` & `inewave-1.7.4/inewave/nwlistop/modelos/blocos/usina.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/blocos/valoresclassetermicaseriepatamar.py` & `inewave-1.7.4/inewave/nwlistop/modelos/blocos/valoresclassetermicaseriepatamar.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/blocos/valoresserie.py` & `inewave-1.7.4/inewave/nwlistop/modelos/blocos/valoresserie.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/blocos/valoresseriepatamar.py` & `inewave-1.7.4/inewave/nwlistop/modelos/blocos/valoresseriepatamar.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/c_v_rhq.py` & `inewave-1.7.4/inewave/nwlistop/modelos/c_v_rhq.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/c_v_rhq_s.py` & `inewave-1.7.4/inewave/nwlistop/modelos/c_v_rhq_s.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/c_v_rhv.py` & `inewave-1.7.4/inewave/nwlistop/modelos/c_v_rhv.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/c_v_rhv_s.py` & `inewave-1.7.4/inewave/nwlistop/modelos/c_v_rhv_s.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/cbomb.py` & `inewave-1.7.4/inewave/nwlistop/modelos/cbomb.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/cbombsin.py` & `inewave-1.7.4/inewave/nwlistop/modelos/cbombsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/cdef.py` & `inewave-1.7.4/inewave/nwlistop/modelos/cdef.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/cdefsin.py` & `inewave-1.7.4/inewave/nwlistop/modelos/cdefsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/celetricas.py` & `inewave-1.7.4/inewave/nwlistop/modelos/celetricas.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/cmarg.py` & `inewave-1.7.4/inewave/nwlistop/modelos/cmarg.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/cmargmed.py` & `inewave-1.7.4/inewave/nwlistop/modelos/cmargmed.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/coper.py` & `inewave-1.7.4/inewave/nwlistop/modelos/coper.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/corteolm.py` & `inewave-1.7.4/inewave/nwlistop/modelos/corteolm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/cterm.py` & `inewave-1.7.4/inewave/nwlistop/modelos/cterm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/ctermsin.py` & `inewave-1.7.4/inewave/nwlistop/modelos/ctermsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/def.py` & `inewave-1.7.4/inewave/nwlistop/modelos/def.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/defsin.py` & `inewave-1.7.4/inewave/nwlistop/modelos/defsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/deletricas.py` & `inewave-1.7.4/inewave/nwlistop/modelos/deletricas.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/depminuh.py` & `inewave-1.7.4/inewave/nwlistop/modelos/depminuh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/desvuh.py` & `inewave-1.7.4/inewave/nwlistop/modelos/desvuh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/dflppdfmaxm.py` & `inewave-1.7.4/inewave/nwlistop/modelos/dflppdfmaxm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/dflpptbmaxm.py` & `inewave-1.7.4/inewave/nwlistop/modelos/dflpptbmaxm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/dfphauh.py` & `inewave-1.7.4/inewave/nwlistop/modelos/dfphauh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/dlppdfmax.py` & `inewave-1.7.4/inewave/nwlistop/modelos/dlppdfmax.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/dlppdfmaxs.py` & `inewave-1.7.4/inewave/nwlistop/modelos/dlppdfmaxs.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/dlpptbmax.py` & `inewave-1.7.4/inewave/nwlistop/modelos/dlpptbmax.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/dlpptbmaxs.py` & `inewave-1.7.4/inewave/nwlistop/modelos/dlpptbmaxs.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/dnegevap.py` & `inewave-1.7.4/inewave/nwlistop/modelos/dnegevap.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/dposevap.py` & `inewave-1.7.4/inewave/nwlistop/modelos/dposevap.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/dtbmax.py` & `inewave-1.7.4/inewave/nwlistop/modelos/dtbmax.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/dtbmin.py` & `inewave-1.7.4/inewave/nwlistop/modelos/dtbmin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/dvazmax.py` & `inewave-1.7.4/inewave/nwlistop/modelos/dvazmax.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/eaf.py` & `inewave-1.7.4/inewave/nwlistop/modelos/eaf.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/eafb.py` & `inewave-1.7.4/inewave/nwlistop/modelos/eafb.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/eafbm.py` & `inewave-1.7.4/inewave/nwlistop/modelos/eafbm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/eafbsin.py` & `inewave-1.7.4/inewave/nwlistop/modelos/eafbsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/eafm.py` & `inewave-1.7.4/inewave/nwlistop/modelos/eafm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/earmf.py` & `inewave-1.7.4/inewave/nwlistop/modelos/earmf.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/earmfm.py` & `inewave-1.7.4/inewave/nwlistop/modelos/earmfm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/earmfp.py` & `inewave-1.7.4/inewave/nwlistop/modelos/earmfp.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/earmfpm.py` & `inewave-1.7.4/inewave/nwlistop/modelos/earmfpm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/earmfpsin.py` & `inewave-1.7.4/inewave/nwlistop/modelos/earmfpsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/earmfsin.py` & `inewave-1.7.4/inewave/nwlistop/modelos/earmfsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/edesvc.py` & `inewave-1.7.4/inewave/nwlistop/modelos/edesvc.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/edesvcm.py` & `inewave-1.7.4/inewave/nwlistop/modelos/edesvcm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/edesvcsin.py` & `inewave-1.7.4/inewave/nwlistop/modelos/edesvcsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/evapo.py` & `inewave-1.7.4/inewave/nwlistop/modelos/evapo.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/evapom.py` & `inewave-1.7.4/inewave/nwlistop/modelos/evapom.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/evaporsin.py` & `inewave-1.7.4/inewave/nwlistop/modelos/evaporsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/evert.py` & `inewave-1.7.4/inewave/nwlistop/modelos/evert.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/evertm.py` & `inewave-1.7.4/inewave/nwlistop/modelos/evertm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/evertsin.py` & `inewave-1.7.4/inewave/nwlistop/modelos/evertsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/exces.py` & `inewave-1.7.4/inewave/nwlistop/modelos/exces.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/excessin.py` & `inewave-1.7.4/inewave/nwlistop/modelos/excessin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/form_rhq.py` & `inewave-1.7.4/inewave/nwlistop/modelos/form_rhq.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/form_rhv.py` & `inewave-1.7.4/inewave/nwlistop/modelos/form_rhv.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/fteolm.py` & `inewave-1.7.4/inewave/nwlistop/modelos/fteolm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/fteolsin.py` & `inewave-1.7.4/inewave/nwlistop/modelos/fteolsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/geol.py` & `inewave-1.7.4/inewave/nwlistop/modelos/geol.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/geolm.py` & `inewave-1.7.4/inewave/nwlistop/modelos/geolm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/geolsin.py` & `inewave-1.7.4/inewave/nwlistop/modelos/geolsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/gh_fphexat.py` & `inewave-1.7.4/inewave/nwlistop/modelos/gh_fphexat.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/ghidr.py` & `inewave-1.7.4/inewave/nwlistop/modelos/ghidr.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/ghidrm.py` & `inewave-1.7.4/inewave/nwlistop/modelos/ghidrm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/ghidrsin.py` & `inewave-1.7.4/inewave/nwlistop/modelos/ghidrsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/ghiduh.py` & `inewave-1.7.4/inewave/nwlistop/modelos/ghiduh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/ghmax.py` & `inewave-1.7.4/inewave/nwlistop/modelos/ghmax.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/ghmax_fpha.py` & `inewave-1.7.4/inewave/nwlistop/modelos/ghmax_fpha.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/ghmax_fphc.py` & `inewave-1.7.4/inewave/nwlistop/modelos/ghmax_fphc.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/ghmaxm.py` & `inewave-1.7.4/inewave/nwlistop/modelos/ghmaxm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/ghmaxmr.py` & `inewave-1.7.4/inewave/nwlistop/modelos/ghmaxmr.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/ghmaxr.py` & `inewave-1.7.4/inewave/nwlistop/modelos/ghmaxr.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/ghmaxrsin.py` & `inewave-1.7.4/inewave/nwlistop/modelos/ghmaxrsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/ghmaxsin.py` & `inewave-1.7.4/inewave/nwlistop/modelos/ghmaxsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/ghtot.py` & `inewave-1.7.4/inewave/nwlistop/modelos/ghtot.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/ghtotm.py` & `inewave-1.7.4/inewave/nwlistop/modelos/ghtotm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/ghtotsin.py` & `inewave-1.7.4/inewave/nwlistop/modelos/ghtotsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/gtert.py` & `inewave-1.7.4/inewave/nwlistop/modelos/gtert.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/gttot.py` & `inewave-1.7.4/inewave/nwlistop/modelos/gttot.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/gttotsin.py` & `inewave-1.7.4/inewave/nwlistop/modelos/gttotsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/hjus.py` & `inewave-1.7.4/inewave/nwlistop/modelos/hjus.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/hliq.py` & `inewave-1.7.4/inewave/nwlistop/modelos/hliq.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/hmont.py` & `inewave-1.7.4/inewave/nwlistop/modelos/hmont.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/intercambio.py` & `inewave-1.7.4/inewave/nwlistop/modelos/intercambio.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/invade.py` & `inewave-1.7.4/inewave/nwlistop/modelos/invade.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/invadem.py` & `inewave-1.7.4/inewave/nwlistop/modelos/invadem.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/mediasmerc.py` & `inewave-1.7.4/inewave/nwlistop/modelos/mediasmerc.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/mediasree.py` & `inewave-1.7.4/inewave/nwlistop/modelos/mediasree.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/mediasrep.py` & `inewave-1.7.4/inewave/nwlistop/modelos/mediasrep.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/mediasrhq.py` & `inewave-1.7.4/inewave/nwlistop/modelos/mediasrhq.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/mediasrhv.py` & `inewave-1.7.4/inewave/nwlistop/modelos/mediasrhv.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/mediassin.py` & `inewave-1.7.4/inewave/nwlistop/modelos/mediassin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/mediasusie.py` & `inewave-1.7.4/inewave/nwlistop/modelos/mediasusie.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/mediasusih.py` & `inewave-1.7.4/inewave/nwlistop/modelos/mediasusih.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/mediasusit.py` & `inewave-1.7.4/inewave/nwlistop/modelos/mediasusit.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/mercl.py` & `inewave-1.7.4/inewave/nwlistop/modelos/mercl.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/merclsin.py` & `inewave-1.7.4/inewave/nwlistop/modelos/merclsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/mevmin.py` & `inewave-1.7.4/inewave/nwlistop/modelos/mevmin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/mevminm.py` & `inewave-1.7.4/inewave/nwlistop/modelos/mevminm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/mevminsin.py` & `inewave-1.7.4/inewave/nwlistop/modelos/mevminsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/nwlistopdat.py` & `inewave-1.7.4/inewave/nwlistop/modelos/nwlistopdat.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/perdf.py` & `inewave-1.7.4/inewave/nwlistop/modelos/perdf.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/perdfm.py` & `inewave-1.7.4/inewave/nwlistop/modelos/perdfm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/perdfsin.py` & `inewave-1.7.4/inewave/nwlistop/modelos/perdfsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/pivarm.py` & `inewave-1.7.4/inewave/nwlistop/modelos/pivarm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/pivarmincr.py` & `inewave-1.7.4/inewave/nwlistop/modelos/pivarmincr.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/qafluh.py` & `inewave-1.7.4/inewave/nwlistop/modelos/qafluh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/qincruh.py` & `inewave-1.7.4/inewave/nwlistop/modelos/qincruh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/rhslppdf.py` & `inewave-1.7.4/inewave/nwlistop/modelos/rhslppdf.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/rhslpptb.py` & `inewave-1.7.4/inewave/nwlistop/modelos/rhslpptb.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/vagua.py` & `inewave-1.7.4/inewave/nwlistop/modelos/vagua.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/varmpuh.py` & `inewave-1.7.4/inewave/nwlistop/modelos/varmpuh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/varmuh.py` & `inewave-1.7.4/inewave/nwlistop/modelos/varmuh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/vbomb.py` & `inewave-1.7.4/inewave/nwlistop/modelos/vbomb.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/vdesviouh.py` & `inewave-1.7.4/inewave/nwlistop/modelos/vdesviouh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/vento.py` & `inewave-1.7.4/inewave/nwlistop/modelos/vento.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/vertuh.py` & `inewave-1.7.4/inewave/nwlistop/modelos/vertuh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/verturb.py` & `inewave-1.7.4/inewave/nwlistop/modelos/verturb.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/verturbm.py` & `inewave-1.7.4/inewave/nwlistop/modelos/verturbm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/verturbsin.py` & `inewave-1.7.4/inewave/nwlistop/modelos/verturbsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/vevapuh.py` & `inewave-1.7.4/inewave/nwlistop/modelos/vevapuh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/vevmin.py` & `inewave-1.7.4/inewave/nwlistop/modelos/vevmin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/vevminm.py` & `inewave-1.7.4/inewave/nwlistop/modelos/vevminm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/vevminsin.py` & `inewave-1.7.4/inewave/nwlistop/modelos/vevminsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/vghmin.py` & `inewave-1.7.4/inewave/nwlistop/modelos/vghmin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/vghminm.py` & `inewave-1.7.4/inewave/nwlistop/modelos/vghminm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/vghminsin.py` & `inewave-1.7.4/inewave/nwlistop/modelos/vghminsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/vghminuh.py` & `inewave-1.7.4/inewave/nwlistop/modelos/vghminuh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/viol_rhq.py` & `inewave-1.7.4/inewave/nwlistop/modelos/viol_rhq.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/viol_rhv.py` & `inewave-1.7.4/inewave/nwlistop/modelos/viol_rhv.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/vmort.py` & `inewave-1.7.4/inewave/nwlistop/modelos/vmort.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/vmortm.py` & `inewave-1.7.4/inewave/nwlistop/modelos/vmortm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/vmortsin.py` & `inewave-1.7.4/inewave/nwlistop/modelos/vmortsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/modelos/vturuh.py` & `inewave-1.7.4/inewave/nwlistop/modelos/vturuh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/nwlistopdat.py` & `inewave-1.7.4/inewave/nwlistop/nwlistopdat.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/perdf.py` & `inewave-1.7.4/inewave/nwlistop/perdf.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/perdfm.py` & `inewave-1.7.4/inewave/nwlistop/perdfm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/pivarm.py` & `inewave-1.7.4/inewave/nwlistop/pivarm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/pivarmincr.py` & `inewave-1.7.4/inewave/nwlistop/pivarmincr.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/qafluh.py` & `inewave-1.7.4/inewave/nwlistop/qafluh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/qincruh.py` & `inewave-1.7.4/inewave/nwlistop/qincruh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/rhslppdf.py` & `inewave-1.7.4/inewave/nwlistop/rhslppdf.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/rhslpptb.py` & `inewave-1.7.4/inewave/nwlistop/rhslpptb.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/varmpuh.py` & `inewave-1.7.4/inewave/nwlistop/varmpuh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/varmuh.py` & `inewave-1.7.4/inewave/nwlistop/varmuh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/vbomb.py` & `inewave-1.7.4/inewave/nwlistop/vbomb.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/vdesviouh.py` & `inewave-1.7.4/inewave/nwlistop/vdesviouh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/vento.py` & `inewave-1.7.4/inewave/nwlistop/vento.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/vertuh.py` & `inewave-1.7.4/inewave/nwlistop/vertuh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/verturb.py` & `inewave-1.7.4/inewave/nwlistop/verturb.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/verturbm.py` & `inewave-1.7.4/inewave/nwlistop/verturbm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/vevapuh.py` & `inewave-1.7.4/inewave/nwlistop/vevapuh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/vevmin.py` & `inewave-1.7.4/inewave/nwlistop/vevmin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/vevminm.py` & `inewave-1.7.4/inewave/nwlistop/vevminm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/vghmin.py` & `inewave-1.7.4/inewave/nwlistop/vghmin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/vghminm.py` & `inewave-1.7.4/inewave/nwlistop/vghminm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/vghminuh.py` & `inewave-1.7.4/inewave/nwlistop/vghminuh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/viol_rhq.py` & `inewave-1.7.4/inewave/nwlistop/viol_rhq.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/viol_rhv.py` & `inewave-1.7.4/inewave/nwlistop/viol_rhv.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/vmort.py` & `inewave-1.7.4/inewave/nwlistop/vmort.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/vmortm.py` & `inewave-1.7.4/inewave/nwlistop/vmortm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave/nwlistop/vturuh.py` & `inewave-1.7.4/inewave/nwlistop/vturuh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/inewave.egg-info/PKG-INFO` & `inewave-1.7.4/inewave.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inewave
-Version: 1.7.3
+Version: 1.7.4
 Summary: Interface para arquivos do NEWAVE
 Home-page: https://github.com/rjmalves/inewave
 Author: Rogerio Alves
 Author-email: rogerioalves.ee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `inewave-1.7.3/inewave.egg-info/SOURCES.txt` & `inewave-1.7.4/inewave.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/setup.py` & `inewave-1.7.4/setup.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/libs/test_eolica.py` & `inewave-1.7.4/tests/libs/test_eolica.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/libs/test_restricoes.py` & `inewave-1.7.4/tests/libs/test_restricoes.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/libs/test_usinas_hidreletricas.py` & `inewave-1.7.4/tests/libs/test_usinas_hidreletricas.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/adterm.py` & `inewave-1.7.4/tests/mocks/arquivos/adterm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/agrint.py` & `inewave-1.7.4/tests/mocks/arquivos/agrint.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/arquivos.py` & `inewave-1.7.4/tests/mocks/arquivos/arquivos.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/arquivos_nwlistcf.py` & `inewave-1.7.4/tests/mocks/arquivos/arquivos_nwlistcf.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/avl_cortesfpha_nwv.py` & `inewave-1.7.4/tests/mocks/arquivos/avl_cortesfpha_nwv.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/avl_desvfpha_s.py` & `inewave-1.7.4/tests/mocks/arquivos/avl_desvfpha_s.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/avl_desvfpha_v_q.py` & `inewave-1.7.4/tests/mocks/arquivos/avl_desvfpha_v_q.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/c_v_rhq.py` & `inewave-1.7.4/tests/mocks/arquivos/c_v_rhq.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/c_v_rhq_s.py` & `inewave-1.7.4/tests/mocks/arquivos/c_v_rhq_s.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/c_v_rhv.py` & `inewave-1.7.4/tests/mocks/arquivos/c_v_rhv.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/c_v_rhv_s.py` & `inewave-1.7.4/tests/mocks/arquivos/c_v_rhv_s.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/cadic.py` & `inewave-1.7.4/tests/mocks/arquivos/cadic.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/cbomb.py` & `inewave-1.7.4/tests/mocks/arquivos/cbomb.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/cbombsin.py` & `inewave-1.7.4/tests/mocks/arquivos/cbombsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/cdef.py` & `inewave-1.7.4/tests/mocks/arquivos/cdef.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/cdefsin.py` & `inewave-1.7.4/tests/mocks/arquivos/cdefsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/celetricas.py` & `inewave-1.7.4/tests/mocks/arquivos/celetricas.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/clast.py` & `inewave-1.7.4/tests/mocks/arquivos/clast.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/cmarg.py` & `inewave-1.7.4/tests/mocks/arquivos/cmarg.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/cmargmed.py` & `inewave-1.7.4/tests/mocks/arquivos/cmargmed.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/confhd.py` & `inewave-1.7.4/tests/mocks/arquivos/confhd.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/conft.py` & `inewave-1.7.4/tests/mocks/arquivos/conft.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/coper.py` & `inewave-1.7.4/tests/mocks/arquivos/coper.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/corteolm.py` & `inewave-1.7.4/tests/mocks/arquivos/corteolm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/cterm.py` & `inewave-1.7.4/tests/mocks/arquivos/cterm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/ctermsin.py` & `inewave-1.7.4/tests/mocks/arquivos/ctermsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/curva.py` & `inewave-1.7.4/tests/mocks/arquivos/curva.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/cvar.py` & `inewave-1.7.4/tests/mocks/arquivos/cvar.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/deficit.py` & `inewave-1.7.4/tests/mocks/arquivos/deficit.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/defsin.py` & `inewave-1.7.4/tests/mocks/arquivos/defsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/deletricas.py` & `inewave-1.7.4/tests/mocks/arquivos/deletricas.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/depminuh.py` & `inewave-1.7.4/tests/mocks/arquivos/depminuh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/desvuh.py` & `inewave-1.7.4/tests/mocks/arquivos/desvuh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/dfphauh.py` & `inewave-1.7.4/tests/mocks/arquivos/dfphauh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/dger.py` & `inewave-1.7.4/tests/mocks/arquivos/dger.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/dlppdfmax.py` & `inewave-1.7.4/tests/mocks/arquivos/dlppdfmax.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/dlppdfmaxm.py` & `inewave-1.7.4/tests/mocks/arquivos/dlppdfmaxm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/dlppdfmaxs.py` & `inewave-1.7.4/tests/mocks/arquivos/dlppdfmaxs.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/dlpptbmax.py` & `inewave-1.7.4/tests/mocks/arquivos/dlpptbmax.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/dlpptbmaxm.py` & `inewave-1.7.4/tests/mocks/arquivos/dlpptbmaxm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/dlpptbmaxs.py` & `inewave-1.7.4/tests/mocks/arquivos/dlpptbmaxs.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/dneg_evap.py` & `inewave-1.7.4/tests/mocks/arquivos/dneg_evap.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/dpos_evap.py` & `inewave-1.7.4/tests/mocks/arquivos/dpos_evap.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/dsvagua.py` & `inewave-1.7.4/tests/mocks/arquivos/dsvagua.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/dtbmax.py` & `inewave-1.7.4/tests/mocks/arquivos/dtbmax.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/dtbmin.py` & `inewave-1.7.4/tests/mocks/arquivos/dtbmin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/dvazmax.py` & `inewave-1.7.4/tests/mocks/arquivos/dvazmax.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/eaf.py` & `inewave-1.7.4/tests/mocks/arquivos/eaf.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/eafb.py` & `inewave-1.7.4/tests/mocks/arquivos/eafb.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/eafbm.py` & `inewave-1.7.4/tests/mocks/arquivos/eafbm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/eafbsin.py` & `inewave-1.7.4/tests/mocks/arquivos/eafbsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/eafm.py` & `inewave-1.7.4/tests/mocks/arquivos/eafm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/eafpast.py` & `inewave-1.7.4/tests/mocks/arquivos/eafpast.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/earmf.py` & `inewave-1.7.4/tests/mocks/arquivos/earmf.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/earmfm.py` & `inewave-1.7.4/tests/mocks/arquivos/earmfm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/earmfp.py` & `inewave-1.7.4/tests/mocks/arquivos/earmfp.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/earmfpm.py` & `inewave-1.7.4/tests/mocks/arquivos/earmfpm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/earmfpsin.py` & `inewave-1.7.4/tests/mocks/arquivos/earmfpsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/earmfsin.py` & `inewave-1.7.4/tests/mocks/arquivos/earmfsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/eco_fpha.py` & `inewave-1.7.4/tests/mocks/arquivos/eco_fpha.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/edesvc.py` & `inewave-1.7.4/tests/mocks/arquivos/edesvc.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/edesvcm.py` & `inewave-1.7.4/tests/mocks/arquivos/edesvcm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/edesvcsin.py` & `inewave-1.7.4/tests/mocks/arquivos/edesvcsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/eolica.py` & `inewave-1.7.4/tests/mocks/arquivos/eolica.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/estados.py` & `inewave-1.7.4/tests/mocks/arquivos/estados.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/evapo.py` & `inewave-1.7.4/tests/mocks/arquivos/evapo.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/evapom.py` & `inewave-1.7.4/tests/mocks/arquivos/evapom.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/evaporsin.py` & `inewave-1.7.4/tests/mocks/arquivos/evaporsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/evert.py` & `inewave-1.7.4/tests/mocks/arquivos/evert.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/evertm.py` & `inewave-1.7.4/tests/mocks/arquivos/evertm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/evertsin.py` & `inewave-1.7.4/tests/mocks/arquivos/evertsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/exces.py` & `inewave-1.7.4/tests/mocks/arquivos/exces.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/excessin.py` & `inewave-1.7.4/tests/mocks/arquivos/excessin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/exph.py` & `inewave-1.7.4/tests/mocks/arquivos/exph.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/expt.py` & `inewave-1.7.4/tests/mocks/arquivos/expt.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/form_rhq.py` & `inewave-1.7.4/tests/mocks/arquivos/form_rhq.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/form_rhv.py` & `inewave-1.7.4/tests/mocks/arquivos/form_rhv.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/fteolm.py` & `inewave-1.7.4/tests/mocks/arquivos/fteolm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/fteolsin.py` & `inewave-1.7.4/tests/mocks/arquivos/fteolsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/geol.py` & `inewave-1.7.4/tests/mocks/arquivos/geol.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/geolm.py` & `inewave-1.7.4/tests/mocks/arquivos/geolm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/geolsin.py` & `inewave-1.7.4/tests/mocks/arquivos/geolsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/gh_fphexat.py` & `inewave-1.7.4/tests/mocks/arquivos/gh_fphexat.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/ghidr.py` & `inewave-1.7.4/tests/mocks/arquivos/ghidr.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/ghidrm.py` & `inewave-1.7.4/tests/mocks/arquivos/ghidrm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/ghidrsin.py` & `inewave-1.7.4/tests/mocks/arquivos/ghidrsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/ghiduh.py` & `inewave-1.7.4/tests/mocks/arquivos/ghiduh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/ghmax.py` & `inewave-1.7.4/tests/mocks/arquivos/ghmax.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/ghmax_fpha.py` & `inewave-1.7.4/tests/mocks/arquivos/ghmax_fpha.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/ghmax_fphc.py` & `inewave-1.7.4/tests/mocks/arquivos/ghmax_fphc.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/ghmaxm.py` & `inewave-1.7.4/tests/mocks/arquivos/ghmaxm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/ghmaxmr.py` & `inewave-1.7.4/tests/mocks/arquivos/ghmaxmr.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/ghmaxr.py` & `inewave-1.7.4/tests/mocks/arquivos/ghmaxr.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/ghmaxrsin.py` & `inewave-1.7.4/tests/mocks/arquivos/ghmaxrsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/ghmaxsin.py` & `inewave-1.7.4/tests/mocks/arquivos/ghmaxsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/ghmin.py` & `inewave-1.7.4/tests/mocks/arquivos/ghmin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/ghtot.py` & `inewave-1.7.4/tests/mocks/arquivos/ghtot.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/ghtotm.py` & `inewave-1.7.4/tests/mocks/arquivos/ghtotm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/ghtotsin.py` & `inewave-1.7.4/tests/mocks/arquivos/ghtotsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/gtert.py` & `inewave-1.7.4/tests/mocks/arquivos/gtert.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/gttot.py` & `inewave-1.7.4/tests/mocks/arquivos/gttot.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/gttotsin.py` & `inewave-1.7.4/tests/mocks/arquivos/gttotsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/hjus.py` & `inewave-1.7.4/tests/mocks/arquivos/hjus.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/hliq.py` & `inewave-1.7.4/tests/mocks/arquivos/hliq.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/hmont.py` & `inewave-1.7.4/tests/mocks/arquivos/hmont.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/intercambio.py` & `inewave-1.7.4/tests/mocks/arquivos/intercambio.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/invade.py` & `inewave-1.7.4/tests/mocks/arquivos/invade.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/invadem.py` & `inewave-1.7.4/tests/mocks/arquivos/invadem.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/manutt.py` & `inewave-1.7.4/tests/mocks/arquivos/manutt.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/mercl.py` & `inewave-1.7.4/tests/mocks/arquivos/mercl.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/merclsin.py` & `inewave-1.7.4/tests/mocks/arquivos/merclsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/mevmin.py` & `inewave-1.7.4/tests/mocks/arquivos/mevmin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/mevminm.py` & `inewave-1.7.4/tests/mocks/arquivos/mevminm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/mevminsin.py` & `inewave-1.7.4/tests/mocks/arquivos/mevminsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/modif.py` & `inewave-1.7.4/tests/mocks/arquivos/modif.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/newavetim.py` & `inewave-1.7.4/tests/mocks/arquivos/newavetim.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/nwlistcfrel.py` & `inewave-1.7.4/tests/mocks/arquivos/nwlistcfrel.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/nwlistopdat.py` & `inewave-1.7.4/tests/mocks/arquivos/nwlistopdat.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/nwv_avl_evap.py` & `inewave-1.7.4/tests/mocks/arquivos/nwv_avl_evap.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/nwv_cortes_evap.py` & `inewave-1.7.4/tests/mocks/arquivos/nwv_cortes_evap.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/nwv_eco_evap.py` & `inewave-1.7.4/tests/mocks/arquivos/nwv_eco_evap.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/parp.py` & `inewave-1.7.4/tests/mocks/arquivos/parp.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/parpeol.py` & `inewave-1.7.4/tests/mocks/arquivos/parpeol.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/parpvaz.py` & `inewave-1.7.4/tests/mocks/arquivos/parpvaz.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/patamar.py` & `inewave-1.7.4/tests/mocks/arquivos/patamar.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/penalid.py` & `inewave-1.7.4/tests/mocks/arquivos/penalid.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/perdf.py` & `inewave-1.7.4/tests/mocks/arquivos/perdf.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/perdfm.py` & `inewave-1.7.4/tests/mocks/arquivos/perdfm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/perdfsin.py` & `inewave-1.7.4/tests/mocks/arquivos/perdfsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/pivarm.py` & `inewave-1.7.4/tests/mocks/arquivos/pivarm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/pivarmincr.py` & `inewave-1.7.4/tests/mocks/arquivos/pivarmincr.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/pmo.py` & `inewave-1.7.4/tests/mocks/arquivos/pmo.py`

 * *Files 0% similar despite different names*

```diff
@@ -1063,14 +1063,22 @@
     "    209  TAMBAQUI       2023    63.00   63.00   63.01   63.01   63.01   63.01   63.01   63.01   63.01   63.01   63.01   63.01\n",
     "                        2024    63.01   63.01   63.01   63.01   63.01   63.01   63.01   63.01   63.01   63.01   63.01   63.01\n",
     "                        2025    63.01   63.01   63.01   63.01    0.00    0.00    0.00    0.00    0.00    0.00    0.00    0.00\n",
     "                        2026     0.00    0.00    0.00    0.00    0.00    0.00    0.00    0.00    0.00    0.00    0.00    0.00\n",
     "                        2027     0.00    0.00    0.00    0.00    0.00    0.00    0.00    0.00    0.00    0.00    0.00    0.00\n",
     " X---------------------------------------------------------------------------------------------------------------------------X\n",
     "\n",
+    "\n",
+    "   GERACAO TERMICA MAXIMA POR USINA (MWmed)\n",
+    " X---------------------------------------------------------------------------------------------------------------------------X\n",
+    "\n",
+    "  NUMERO     NOME       ANO                                               ESTAGIOS\n",
+    "                                  1       2       3       4       5       6       7       8       9      10      11      12\n",
+    " X------X------------X-------X-------X-------X-------X-------X-------X-------X-------X-------X-------X-------X-------X-------X\n",
+    " X---------------------------------------------------------------------------------------------------------------------------X\n",
 ]
 
 MockBlocoGeracaoMinimaUsinasTermicasPMO = [
     "   GERACAO TERMICA MINIMA POR USINA (MWmed)\n",
     " X---------------------------------------------------------------------------------------------------------------------------X\n",
     "\n",
     "  NUMERO     NOME       ANO                                               ESTAGIOS\n",
@@ -1826,14 +1834,22 @@
     "    209  TAMBAQUI       2023    62.99   62.99   62.99   62.99   62.99   62.99   62.99   62.99   62.99   62.99   62.99   62.99\n",
     "                        2024    62.99   62.99   62.99   62.99   62.99   62.99   62.99   62.99   62.99   62.99   62.99   62.99\n",
     "                        2025    62.99   62.99   62.99   62.99    0.00    0.00    0.00    0.00    0.00    0.00    0.00    0.00\n",
     "                        2026     0.00    0.00    0.00    0.00    0.00    0.00    0.00    0.00    0.00    0.00    0.00    0.00\n",
     "                        2027     0.00    0.00    0.00    0.00    0.00    0.00    0.00    0.00    0.00    0.00    0.00    0.00\n",
     " X---------------------------------------------------------------------------------------------------------------------------X\n",
     "\n",
+    "   GERACAO TERMICA MINIMA POR USINA (MWmed)\n",
+    " X---------------------------------------------------------------------------------------------------------------------------X\n",
+    "\n",
+    "  NUMERO     NOME       ANO                                               ESTAGIOS\n",
+    "                                  1       2       3       4       5       6       7       8       9      10      11      12\n",
+    " X------X------------X-------X-------X-------X-------X-------X-------X-------X-------X-------X-------X-------X-------X-------X\n",
+    " X---------------------------------------------------------------------------------------------------------------------------X\n",
+    "\n",
 ]
 
 
 MockBlocoConvergenciaPMO = [
     "    ITER               LIM.INF.                   ZINF               LIM.SUP.                   ZSUP                  DZINF             ZSUP ITER.\n",
     "                        ($10^6)                ($10^6)                ($10^6)                ($10^6)                    (%)                ($10^6)\n",
     "   X----X----------------------X----------------------X----------------------X----------------------X----------------------X----------------------X------------------------------------------------------------------------------------------------------------------------------------------------X\n",
```

### Comparing `inewave-1.7.3/tests/mocks/arquivos/qafluh.py` & `inewave-1.7.4/tests/mocks/arquivos/qafluh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/qincruh.py` & `inewave-1.7.4/tests/mocks/arquivos/qincruh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/re.py` & `inewave-1.7.4/tests/mocks/arquivos/re.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/ree.py` & `inewave-1.7.4/tests/mocks/arquivos/ree.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/restricoes.py` & `inewave-1.7.4/tests/mocks/arquivos/restricoes.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/rhslppdf.py` & `inewave-1.7.4/tests/mocks/arquivos/rhslppdf.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/rhslpptb.py` & `inewave-1.7.4/tests/mocks/arquivos/rhslpptb.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/selcor.py` & `inewave-1.7.4/tests/mocks/arquivos/selcor.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/sistema.py` & `inewave-1.7.4/tests/mocks/arquivos/sistema.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/term.py` & `inewave-1.7.4/tests/mocks/arquivos/term.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/usinas_hidreletricas.py` & `inewave-1.7.4/tests/mocks/arquivos/usinas_hidreletricas.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/vagua.py` & `inewave-1.7.4/tests/mocks/arquivos/vagua.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/varmpuh.py` & `inewave-1.7.4/tests/mocks/arquivos/varmpuh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/varmuh.py` & `inewave-1.7.4/tests/mocks/arquivos/varmuh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/vazpast.py` & `inewave-1.7.4/tests/mocks/arquivos/vazpast.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/vbomb.py` & `inewave-1.7.4/tests/mocks/arquivos/vbomb.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/vdesviouh.py` & `inewave-1.7.4/tests/mocks/arquivos/vdesviouh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/vento.py` & `inewave-1.7.4/tests/mocks/arquivos/vento.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/vertuh.py` & `inewave-1.7.4/tests/mocks/arquivos/vertuh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/verturb.py` & `inewave-1.7.4/tests/mocks/arquivos/verturb.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/verturbm.py` & `inewave-1.7.4/tests/mocks/arquivos/verturbm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/verturbsin.py` & `inewave-1.7.4/tests/mocks/arquivos/verturbsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/vevapuh.py` & `inewave-1.7.4/tests/mocks/arquivos/vevapuh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/vevmin.py` & `inewave-1.7.4/tests/mocks/arquivos/vevmin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/vevminm.py` & `inewave-1.7.4/tests/mocks/arquivos/vevminm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/vevminsin.py` & `inewave-1.7.4/tests/mocks/arquivos/vevminsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/vghmin.py` & `inewave-1.7.4/tests/mocks/arquivos/vghmin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/vghminm.py` & `inewave-1.7.4/tests/mocks/arquivos/vghminm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/vghminsin.py` & `inewave-1.7.4/tests/mocks/arquivos/vghminsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/vghminuh.py` & `inewave-1.7.4/tests/mocks/arquivos/vghminuh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/viol_rhq.py` & `inewave-1.7.4/tests/mocks/arquivos/viol_rhq.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/viol_rhv.py` & `inewave-1.7.4/tests/mocks/arquivos/viol_rhv.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/vmort.py` & `inewave-1.7.4/tests/mocks/arquivos/vmort.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/vmortm.py` & `inewave-1.7.4/tests/mocks/arquivos/vmortm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/vmortsin.py` & `inewave-1.7.4/tests/mocks/arquivos/vmortsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/volref_saz.py` & `inewave-1.7.4/tests/mocks/arquivos/volref_saz.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/arquivos/vturuh.py` & `inewave-1.7.4/tests/mocks/arquivos/vturuh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/mocks/mock_open.py` & `inewave-1.7.4/tests/mocks/mock_open.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/newave/test_adterm.py` & `inewave-1.7.4/tests/newave/test_adterm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/newave/test_agrint.py` & `inewave-1.7.4/tests/newave/test_agrint.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/newave/test_arquivos.py` & `inewave-1.7.4/tests/newave/test_arquivos.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/newave/test_avl_cortesfpha_nwv.py` & `inewave-1.7.4/tests/newave/test_avl_cortesfpha_nwv.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/newave/test_avl_desvfpha_s.py` & `inewave-1.7.4/tests/newave/test_avl_desvfpha_s.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/newave/test_avl_desvfpha_v_q.py` & `inewave-1.7.4/tests/newave/test_avl_desvfpha_v_q.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/newave/test_cadic.py` & `inewave-1.7.4/tests/newave/test_cadic.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/newave/test_caso.py` & `inewave-1.7.4/tests/newave/test_caso.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/newave/test_clast.py` & `inewave-1.7.4/tests/newave/test_clast.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/newave/test_confhd.py` & `inewave-1.7.4/tests/newave/test_confhd.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/newave/test_conft.py` & `inewave-1.7.4/tests/newave/test_conft.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/newave/test_cortes.py` & `inewave-1.7.4/tests/newave/test_cortes.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/newave/test_cortesh.py` & `inewave-1.7.4/tests/newave/test_cortesh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/newave/test_curva.py` & `inewave-1.7.4/tests/newave/test_curva.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/newave/test_cvar.py` & `inewave-1.7.4/tests/newave/test_cvar.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/newave/test_dger.py` & `inewave-1.7.4/tests/newave/test_dger.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/newave/test_dsvagua.py` & `inewave-1.7.4/tests/newave/test_dsvagua.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/newave/test_eafpast.py` & `inewave-1.7.4/tests/newave/test_eafpast.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/newave/test_eco_fpha.py` & `inewave-1.7.4/tests/newave/test_eco_fpha.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/newave/test_enavazb.py` & `inewave-1.7.4/tests/newave/test_enavazb.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/newave/test_enavazf.py` & `inewave-1.7.4/tests/newave/test_enavazf.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/newave/test_energiab.py` & `inewave-1.7.4/tests/newave/test_energiab.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/newave/test_energiaf.py` & `inewave-1.7.4/tests/newave/test_energiaf.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/newave/test_energias.py` & `inewave-1.7.4/tests/newave/test_energias.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 
 ARQ_TESTE = "./tests/mocks/arquivos/energias.dat"
 
-NUM_SERIES = 2
-NUM_REES = 1
-NUM_ESTAGIOS = 16
-NUM_ESTAGIOS_TH = 12
+NUM_SERIES = 3
+NUM_REES = 2
+NUM_ESTAGIOS = 3
+NUM_ESTAGIOS_TH = 3
 NUM_ENTRADAS = NUM_SERIES * NUM_REES * (NUM_ESTAGIOS_TH + NUM_ESTAGIOS)
 
 
 def test_secao_energia():
     r = SecaoDadosEnergias()
     with open(ARQ_TESTE, "rb") as fp:
         r.read(
```

### Comparing `inewave-1.7.3/tests/newave/test_engnat.py` & `inewave-1.7.4/tests/newave/test_engnat.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/newave/test_exph.py` & `inewave-1.7.4/tests/newave/test_exph.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/newave/test_expt.py` & `inewave-1.7.4/tests/newave/test_expt.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/newave/test_forward.py` & `inewave-1.7.4/tests/newave/test_forward.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/newave/test_forwarh.py` & `inewave-1.7.4/tests/newave/test_forwarh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/newave/test_ghmin.py` & `inewave-1.7.4/tests/newave/test_ghmin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/newave/test_hidr.py` & `inewave-1.7.4/tests/newave/test_hidr.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/newave/test_manutt.py` & `inewave-1.7.4/tests/newave/test_manutt.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/newave/test_modif.py` & `inewave-1.7.4/tests/newave/test_modif.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/newave/test_newavetim.py` & `inewave-1.7.4/tests/newave/test_newavetim.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/newave/test_nwv_avl_evap.py` & `inewave-1.7.4/tests/newave/test_nwv_avl_evap.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/newave/test_nwv_cortes_evap.py` & `inewave-1.7.4/tests/newave/test_nwv_cortes_evap.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/newave/test_nwv_eco_evap.py` & `inewave-1.7.4/tests/newave/test_nwv_eco_evap.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/newave/test_parp.py` & `inewave-1.7.4/tests/newave/test_parp.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/newave/test_parpeol.py` & `inewave-1.7.4/tests/newave/test_parpeol.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/newave/test_parpvaz.py` & `inewave-1.7.4/tests/newave/test_parpvaz.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/newave/test_patamar.py` & `inewave-1.7.4/tests/newave/test_patamar.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/newave/test_penalid.py` & `inewave-1.7.4/tests/newave/test_penalid.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/newave/test_pmo.py` & `inewave-1.7.4/tests/newave/test_pmo.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/newave/test_re.py` & `inewave-1.7.4/tests/newave/test_re.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/newave/test_ree.py` & `inewave-1.7.4/tests/newave/test_ree.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/newave/test_selcor.py` & `inewave-1.7.4/tests/newave/test_selcor.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/newave/test_shist.py` & `inewave-1.7.4/tests/newave/test_shist.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/newave/test_sistema.py` & `inewave-1.7.4/tests/newave/test_sistema.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/newave/test_term.py` & `inewave-1.7.4/tests/newave/test_term.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/newave/test_vazaob.py` & `inewave-1.7.4/tests/newave/test_vazaob.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/newave/test_vazaof.py` & `inewave-1.7.4/tests/newave/test_vazaof.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/newave/test_vazaos.py` & `inewave-1.7.4/tests/newave/test_vazaos.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/newave/test_vazinat.py` & `inewave-1.7.4/tests/newave/test_vazinat.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/newave/test_vazoes.py` & `inewave-1.7.4/tests/newave/test_vazoes.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/newave/test_vazpast.py` & `inewave-1.7.4/tests/newave/test_vazpast.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/newave/test_volrefsaz.py` & `inewave-1.7.4/tests/newave/test_volrefsaz.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistcf/test_arquivos.py` & `inewave-1.7.4/tests/nwlistcf/test_arquivos.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistcf/test_caso.py` & `inewave-1.7.4/tests/nwlistcf/test_caso.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistcf/test_estados.py` & `inewave-1.7.4/tests/nwlistcf/test_estados.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistcf/test_nwlistcfdat.py` & `inewave-1.7.4/tests/nwlistcf/test_nwlistcfdat.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistcf/test_nwlistcfrel.py` & `inewave-1.7.4/tests/nwlistcf/test_nwlistcfrel.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_c_v_rhq.py` & `inewave-1.7.4/tests/nwlistop/test_c_v_rhq.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_c_v_rhq_s.py` & `inewave-1.7.4/tests/nwlistop/test_c_v_rhq_s.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_c_v_rhv.py` & `inewave-1.7.4/tests/nwlistop/test_c_v_rhv.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_c_v_rhv_s.py` & `inewave-1.7.4/tests/nwlistop/test_c_v_rhv_s.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_cbomb.py` & `inewave-1.7.4/tests/nwlistop/test_cbomb.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_cbombsin.py` & `inewave-1.7.4/tests/nwlistop/test_cbombsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_cdef.py` & `inewave-1.7.4/tests/nwlistop/test_cdef.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_cdefsin.py` & `inewave-1.7.4/tests/nwlistop/test_cdefsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_celetricas.py` & `inewave-1.7.4/tests/nwlistop/test_celetricas.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_cmarg.py` & `inewave-1.7.4/tests/nwlistop/test_cmarg.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_cmargmed.py` & `inewave-1.7.4/tests/nwlistop/test_cmargmed.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_coper.py` & `inewave-1.7.4/tests/nwlistop/test_coper.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_corteolm.py` & `inewave-1.7.4/tests/nwlistop/test_corteolm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_cterm.py` & `inewave-1.7.4/tests/nwlistop/test_cterm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_ctermsin.py` & `inewave-1.7.4/tests/nwlistop/test_ctermsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_deficit.py` & `inewave-1.7.4/tests/nwlistop/test_deficit.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_defsin.py` & `inewave-1.7.4/tests/nwlistop/test_defsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_deletricas.py` & `inewave-1.7.4/tests/nwlistop/test_deletricas.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_depminuh.py` & `inewave-1.7.4/tests/nwlistop/test_depminuh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_desvuh.py` & `inewave-1.7.4/tests/nwlistop/test_desvuh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_dfphauh.py` & `inewave-1.7.4/tests/nwlistop/test_dfphauh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_dlppdfmax.py` & `inewave-1.7.4/tests/nwlistop/test_dlppdfmax.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_dlppdfmaxm.py` & `inewave-1.7.4/tests/nwlistop/test_dlppdfmaxm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_dlppdfmaxs.py` & `inewave-1.7.4/tests/nwlistop/test_dlppdfmaxs.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_dlpptbmax.py` & `inewave-1.7.4/tests/nwlistop/test_dlpptbmax.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_dlpptbmaxm.py` & `inewave-1.7.4/tests/nwlistop/test_dlpptbmaxm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_dlpptbmaxs.py` & `inewave-1.7.4/tests/nwlistop/test_dlpptbmaxs.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_dnegevap.py` & `inewave-1.7.4/tests/nwlistop/test_dnegevap.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_dposevap.py` & `inewave-1.7.4/tests/nwlistop/test_dposevap.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_dtbmax.py` & `inewave-1.7.4/tests/nwlistop/test_dtbmax.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_dtbmin.py` & `inewave-1.7.4/tests/nwlistop/test_dtbmin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_dvazmax.py` & `inewave-1.7.4/tests/nwlistop/test_dvazmax.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_eaf.py` & `inewave-1.7.4/tests/nwlistop/test_eaf.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_eafb.py` & `inewave-1.7.4/tests/nwlistop/test_eafb.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_eafbm.py` & `inewave-1.7.4/tests/nwlistop/test_eafbm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_eafbsin.py` & `inewave-1.7.4/tests/nwlistop/test_eafbsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_eafm.py` & `inewave-1.7.4/tests/nwlistop/test_eafm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_earmf.py` & `inewave-1.7.4/tests/nwlistop/test_earmf.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_earmfm.py` & `inewave-1.7.4/tests/nwlistop/test_earmfm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_earmfp.py` & `inewave-1.7.4/tests/nwlistop/test_earmfp.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_earmfpm.py` & `inewave-1.7.4/tests/nwlistop/test_earmfpm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_earmfpsin.py` & `inewave-1.7.4/tests/nwlistop/test_earmfpsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_earmfsin.py` & `inewave-1.7.4/tests/nwlistop/test_earmfsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_edesvc.py` & `inewave-1.7.4/tests/nwlistop/test_edesvc.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_edesvcm.py` & `inewave-1.7.4/tests/nwlistop/test_edesvcm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_edesvcsin.py` & `inewave-1.7.4/tests/nwlistop/test_edesvcsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_evapo.py` & `inewave-1.7.4/tests/nwlistop/test_evapo.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_evapom.py` & `inewave-1.7.4/tests/nwlistop/test_evapom.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_evaporsin.py` & `inewave-1.7.4/tests/nwlistop/test_evaporsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_evert.py` & `inewave-1.7.4/tests/nwlistop/test_evert.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_evertm.py` & `inewave-1.7.4/tests/nwlistop/test_evertm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_evertsin.py` & `inewave-1.7.4/tests/nwlistop/test_evertsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_exces.py` & `inewave-1.7.4/tests/nwlistop/test_exces.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_excessin.py` & `inewave-1.7.4/tests/nwlistop/test_excessin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_form_rhq.py` & `inewave-1.7.4/tests/nwlistop/test_form_rhq.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_form_rhv.py` & `inewave-1.7.4/tests/nwlistop/test_form_rhv.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_fteolm.py` & `inewave-1.7.4/tests/nwlistop/test_fteolm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_fteolsin.py` & `inewave-1.7.4/tests/nwlistop/test_fteolsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_geol.py` & `inewave-1.7.4/tests/nwlistop/test_geol.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_geolm.py` & `inewave-1.7.4/tests/nwlistop/test_geolm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_geolsin.py` & `inewave-1.7.4/tests/nwlistop/test_geolsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_ghfphexat.py` & `inewave-1.7.4/tests/nwlistop/test_ghfphexat.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_ghidr.py` & `inewave-1.7.4/tests/nwlistop/test_ghidr.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_ghidrm.py` & `inewave-1.7.4/tests/nwlistop/test_ghidrm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_ghidrsin.py` & `inewave-1.7.4/tests/nwlistop/test_ghidrsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_ghiduh.py` & `inewave-1.7.4/tests/nwlistop/test_ghiduh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_ghmax.py` & `inewave-1.7.4/tests/nwlistop/test_ghmax.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_ghmax_fpha.py` & `inewave-1.7.4/tests/nwlistop/test_ghmax_fpha.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_ghmax_fphc.py` & `inewave-1.7.4/tests/nwlistop/test_ghmax_fphc.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_ghmaxm.py` & `inewave-1.7.4/tests/nwlistop/test_ghmaxm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_ghmaxmr.py` & `inewave-1.7.4/tests/nwlistop/test_ghmaxmr.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_ghmaxr.py` & `inewave-1.7.4/tests/nwlistop/test_ghmaxr.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_ghmaxrsin.py` & `inewave-1.7.4/tests/nwlistop/test_ghmaxrsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_ghmaxsin.py` & `inewave-1.7.4/tests/nwlistop/test_ghmaxsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_ghtot.py` & `inewave-1.7.4/tests/nwlistop/test_ghtot.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_ghtotm.py` & `inewave-1.7.4/tests/nwlistop/test_ghtotm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_ghtotsin.py` & `inewave-1.7.4/tests/nwlistop/test_ghtotsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_gtert.py` & `inewave-1.7.4/tests/nwlistop/test_gtert.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_gttot.py` & `inewave-1.7.4/tests/nwlistop/test_gttot.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_gttotsin.py` & `inewave-1.7.4/tests/nwlistop/test_gttotsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_hjus.py` & `inewave-1.7.4/tests/nwlistop/test_hjus.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_hliq.py` & `inewave-1.7.4/tests/nwlistop/test_hliq.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_hmont.py` & `inewave-1.7.4/tests/nwlistop/test_hmont.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_intercambio.py` & `inewave-1.7.4/tests/nwlistop/test_intercambio.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_invade.py` & `inewave-1.7.4/tests/nwlistop/test_invade.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_invadem.py` & `inewave-1.7.4/tests/nwlistop/test_invadem.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_mercl.py` & `inewave-1.7.4/tests/nwlistop/test_mercl.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_merclsin.py` & `inewave-1.7.4/tests/nwlistop/test_merclsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_mevmin.py` & `inewave-1.7.4/tests/nwlistop/test_mevmin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_mevminm.py` & `inewave-1.7.4/tests/nwlistop/test_mevminm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_mevminsin.py` & `inewave-1.7.4/tests/nwlistop/test_mevminsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_nwlistopdat.py` & `inewave-1.7.4/tests/nwlistop/test_nwlistopdat.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_perdf.py` & `inewave-1.7.4/tests/nwlistop/test_perdf.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_perdfm.py` & `inewave-1.7.4/tests/nwlistop/test_perdfm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_perdfsin.py` & `inewave-1.7.4/tests/nwlistop/test_perdfsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_pivarm.py` & `inewave-1.7.4/tests/nwlistop/test_pivarm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_pivarmincr.py` & `inewave-1.7.4/tests/nwlistop/test_pivarmincr.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_qafluh.py` & `inewave-1.7.4/tests/nwlistop/test_qafluh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_qincruh.py` & `inewave-1.7.4/tests/nwlistop/test_qincruh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_rhslppdf.py` & `inewave-1.7.4/tests/nwlistop/test_rhslppdf.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_rhslpptb.py` & `inewave-1.7.4/tests/nwlistop/test_rhslpptb.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_vagua.py` & `inewave-1.7.4/tests/nwlistop/test_vagua.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_varmpuh.py` & `inewave-1.7.4/tests/nwlistop/test_varmpuh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_varmuh.py` & `inewave-1.7.4/tests/nwlistop/test_varmuh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_vbomb.py` & `inewave-1.7.4/tests/nwlistop/test_vbomb.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_vdesviouh.py` & `inewave-1.7.4/tests/nwlistop/test_vdesviouh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_vento.py` & `inewave-1.7.4/tests/nwlistop/test_vento.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_vertuh.py` & `inewave-1.7.4/tests/nwlistop/test_vertuh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_verturb.py` & `inewave-1.7.4/tests/nwlistop/test_verturb.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_verturbm.py` & `inewave-1.7.4/tests/nwlistop/test_verturbm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_verturbsin.py` & `inewave-1.7.4/tests/nwlistop/test_verturbsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_vevapuh.py` & `inewave-1.7.4/tests/nwlistop/test_vevapuh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_vevmin.py` & `inewave-1.7.4/tests/nwlistop/test_vevmin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_vevminm.py` & `inewave-1.7.4/tests/nwlistop/test_vevminm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_vevminsin.py` & `inewave-1.7.4/tests/nwlistop/test_vevminsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_vghmin.py` & `inewave-1.7.4/tests/nwlistop/test_vghmin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_vghminm.py` & `inewave-1.7.4/tests/nwlistop/test_vghminm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_vghminsin.py` & `inewave-1.7.4/tests/nwlistop/test_vghminsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_vghminuh.py` & `inewave-1.7.4/tests/nwlistop/test_vghminuh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_viol_rhq.py` & `inewave-1.7.4/tests/nwlistop/test_viol_rhq.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_viol_rhv.py` & `inewave-1.7.4/tests/nwlistop/test_viol_rhv.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_vmort.py` & `inewave-1.7.4/tests/nwlistop/test_vmort.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_vmortm.py` & `inewave-1.7.4/tests/nwlistop/test_vmortm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_vmortsin.py` & `inewave-1.7.4/tests/nwlistop/test_vmortsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.3/tests/nwlistop/test_vturuh.py` & `inewave-1.7.4/tests/nwlistop/test_vturuh.py`

 * *Files identical despite different names*

