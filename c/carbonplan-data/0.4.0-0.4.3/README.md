# Comparing `tmp/carbonplan-data-0.4.0.tar.gz` & `tmp/carbonplan_data-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carbonplan-data-0.4.0.tar", last modified: Wed Sep 15 20:19:50 2021, max compression
+gzip compressed data, was "carbonplan_data-0.4.3.tar", last modified: Fri Apr 12 21:52:15 2024, max compression
```

## Comparing `carbonplan-data-0.4.0.tar` & `carbonplan_data-0.4.3.tar`

### file list

```diff
@@ -1,134 +1,102 @@
-drwxr-xr-x   0 jhamman    (501) staff       (20)        0 2021-09-15 20:19:50.764026 carbonplan-data-0.4.0/
-drwxr-xr-x   0 jhamman    (501) staff       (20)        0 2021-09-15 20:19:50.740007 carbonplan-data-0.4.0/.github/
--rw-r--r--   0 jhamman    (501) staff       (20)      277 2020-11-27 23:32:42.000000 carbonplan-data-0.4.0/.github/dependabot.yml
-drwxr-xr-x   0 jhamman    (501) staff       (20)        0 2021-09-15 20:19:50.740591 carbonplan-data-0.4.0/.github/workflows/
--rw-r--r--   0 jhamman    (501) staff       (20)     1998 2021-09-15 15:02:44.000000 carbonplan-data-0.4.0/.github/workflows/main.yaml
--rw-r--r--   0 jhamman    (501) staff       (20)      998 2020-09-14 20:58:37.000000 carbonplan-data-0.4.0/.github/workflows/rclone.yaml
--rw-r--r--   0 jhamman    (501) staff       (20)     1847 2020-09-04 15:20:19.000000 carbonplan-data-0.4.0/.gitignore
--rw-r--r--   0 jhamman    (501) staff       (20)     1461 2021-04-28 23:53:56.000000 carbonplan-data-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0 jhamman    (501) staff       (20)      135 2020-09-04 15:20:19.000000 carbonplan-data-0.4.0/.prettierrc.json
--rw-r--r--   0 jhamman    (501) staff       (20)     1067 2020-06-05 03:00:04.000000 carbonplan-data-0.4.0/LICENSE
--rw-r--r--   0 jhamman    (501) staff       (20)       45 2020-10-19 16:59:06.000000 carbonplan-data-0.4.0/MANIFEST.in
--rw-r--r--   0 jhamman    (501) staff       (20)     3418 2021-09-15 20:19:50.764128 carbonplan-data-0.4.0/PKG-INFO
--rw-r--r--   0 jhamman    (501) staff       (20)     2452 2021-03-05 22:30:27.000000 carbonplan-data-0.4.0/README.md
-drwxr-xr-x   0 jhamman    (501) staff       (20)        0 2021-09-15 20:19:50.741359 carbonplan-data-0.4.0/carbonplan_data/
--rw-r--r--   0 jhamman    (501) staff       (20)      940 2020-11-03 20:51:19.000000 carbonplan-data-0.4.0/carbonplan_data/__init__.py
-drwxr-xr-x   0 jhamman    (501) staff       (20)        0 2021-09-15 20:19:50.745429 carbonplan-data-0.4.0/carbonplan_data/catalogs/
--rw-r--r--   0 jhamman    (501) staff       (20)     2895 2020-10-19 21:22:43.000000 carbonplan-data-0.4.0/carbonplan_data/catalogs/fia.yaml
--rw-r--r--   0 jhamman    (501) staff       (20)     3797 2020-10-19 16:59:06.000000 carbonplan-data-0.4.0/carbonplan_data/catalogs/fluxnet.yaml
--rw-r--r--   0 jhamman    (501) staff       (20)     1634 2020-10-19 16:59:06.000000 carbonplan-data-0.4.0/carbonplan_data/catalogs/gcp.yaml
--rw-r--r--   0 jhamman    (501) staff       (20)     1787 2020-10-19 16:59:06.000000 carbonplan-data-0.4.0/carbonplan_data/catalogs/gridmet.yaml
--rw-r--r--   0 jhamman    (501) staff       (20)     1081 2021-03-05 19:44:11.000000 carbonplan-data-0.4.0/carbonplan_data/catalogs/grids.yaml
--rw-r--r--   0 jhamman    (501) staff       (20)     1869 2020-10-19 16:59:06.000000 carbonplan-data-0.4.0/carbonplan_data/catalogs/maca.yaml
--rw-r--r--   0 jhamman    (501) staff       (20)     3269 2020-10-19 21:26:19.000000 carbonplan-data-0.4.0/carbonplan_data/catalogs/master.yaml
--rw-r--r--   0 jhamman    (501) staff       (20)     6882 2020-11-07 23:00:54.000000 carbonplan-data-0.4.0/carbonplan_data/catalogs/mtbs.yaml
--rw-r--r--   0 jhamman    (501) staff       (20)     3519 2020-10-19 21:25:00.000000 carbonplan-data-0.4.0/carbonplan_data/catalogs/nftd.yaml
--rw-r--r--   0 jhamman    (501) staff       (20)     6417 2020-10-19 16:59:06.000000 carbonplan-data-0.4.0/carbonplan_data/catalogs/nlcd.yaml
--rw-r--r--   0 jhamman    (501) staff       (20)      784 2020-10-19 16:59:06.000000 carbonplan-data-0.4.0/carbonplan_data/catalogs/projects.yaml
--rw-r--r--   0 jhamman    (501) staff       (20)     2266 2020-10-19 21:26:59.000000 carbonplan-data-0.4.0/carbonplan_data/catalogs/spawnetal2020.yaml
--rw-r--r--   0 jhamman    (501) staff       (20)     2452 2020-10-26 03:34:39.000000 carbonplan-data-0.4.0/carbonplan_data/catalogs/terraclimate.yaml
--rw-r--r--   0 jhamman    (501) staff       (20)      658 2021-09-15 15:02:44.000000 carbonplan-data-0.4.0/carbonplan_data/metadata.py
-drwxr-xr-x   0 jhamman    (501) staff       (20)        0 2021-09-15 20:19:50.746121 carbonplan-data-0.4.0/carbonplan_data/tests/
--rw-r--r--   0 jhamman    (501) staff       (20)     4092 2020-10-19 16:59:06.000000 carbonplan-data-0.4.0/carbonplan_data/tests/__init__.py
--rw-r--r--   0 jhamman    (501) staff       (20)      283 2020-10-19 18:43:25.000000 carbonplan-data-0.4.0/carbonplan_data/tests/test_catalogs.py
--rw-r--r--   0 jhamman    (501) staff       (20)      791 2021-09-15 15:02:44.000000 carbonplan-data-0.4.0/carbonplan_data/tests/test_utils.py
--rw-r--r--   0 jhamman    (501) staff       (20)     7756 2021-09-15 15:06:19.000000 carbonplan-data-0.4.0/carbonplan_data/utils.py
-drwxr-xr-x   0 jhamman    (501) staff       (20)        0 2021-09-15 20:19:50.742128 carbonplan-data-0.4.0/carbonplan_data.egg-info/
--rw-r--r--   0 jhamman    (501) staff       (20)     3418 2021-09-15 20:19:50.000000 carbonplan-data-0.4.0/carbonplan_data.egg-info/PKG-INFO
--rw-r--r--   0 jhamman    (501) staff       (20)     3182 2021-09-15 20:19:50.000000 carbonplan-data-0.4.0/carbonplan_data.egg-info/SOURCES.txt
--rw-r--r--   0 jhamman    (501) staff       (20)        1 2021-09-15 20:19:50.000000 carbonplan-data-0.4.0/carbonplan_data.egg-info/dependency_links.txt
--rw-r--r--   0 jhamman    (501) staff       (20)       24 2021-09-15 20:19:50.000000 carbonplan-data-0.4.0/carbonplan_data.egg-info/requires.txt
--rw-r--r--   0 jhamman    (501) staff       (20)       16 2021-09-15 20:19:50.000000 carbonplan-data-0.4.0/carbonplan_data.egg-info/top_level.txt
-drwxr-xr-x   0 jhamman    (501) staff       (20)        0 2021-09-15 20:19:50.746359 carbonplan-data-0.4.0/ci/
--rw-r--r--   0 jhamman    (501) staff       (20)      358 2020-10-26 03:43:40.000000 carbonplan-data-0.4.0/ci/environment.yaml
--rw-r--r--   0 jhamman    (501) staff       (20)       24 2020-09-12 18:27:00.000000 carbonplan-data-0.4.0/requirements.txt
-drwxr-xr-x   0 jhamman    (501) staff       (20)        0 2021-09-15 20:19:50.737218 carbonplan-data-0.4.0/scripts/
-drwxr-xr-x   0 jhamman    (501) staff       (20)        0 2021-09-15 20:19:50.747141 carbonplan-data-0.4.0/scripts/fia/
--rw-r--r--   0 jhamman    (501) staff       (20)     3173 2021-04-29 00:01:12.000000 carbonplan-data-0.4.0/scripts/fia/00_download.ipynb
--rw-r--r--   0 jhamman    (501) staff       (20)     5085 2021-04-29 00:01:12.000000 carbonplan-data-0.4.0/scripts/fia/01_raw_to_parquet.ipynb
--rw-r--r--   0 jhamman    (501) staff       (20)    10017 2021-04-29 00:01:12.000000 carbonplan-data-0.4.0/scripts/fia/01_raw_to_parquet_part2.ipynb
-drwxr-xr-x   0 jhamman    (501) staff       (20)        0 2021-09-15 20:19:50.747653 carbonplan-data-0.4.0/scripts/fluxnet/
--rw-r--r--   0 jhamman    (501) staff       (20)     3537 2021-04-29 00:01:12.000000 carbonplan-data-0.4.0/scripts/fluxnet/01_raw_to_parquet.ipynb
--rw-r--r--   0 jhamman    (501) staff       (20)    26846 2020-08-15 17:09:46.000000 carbonplan-data-0.4.0/scripts/fluxnet/download.sh
-drwxr-xr-x   0 jhamman    (501) staff       (20)        0 2021-09-15 20:19:50.748058 carbonplan-data-0.4.0/scripts/gcp/
--rw-r--r--   0 jhamman    (501) staff       (20)     5376 2021-04-29 00:01:13.000000 carbonplan-data-0.4.0/scripts/gcp/01_raw_to_parquet.ipynb
-drwxr-xr-x   0 jhamman    (501) staff       (20)        0 2021-09-15 20:19:50.748300 carbonplan-data-0.4.0/scripts/glas/
--rw-r--r--   0 jhamman    (501) staff       (20)    16759 2021-04-29 00:01:13.000000 carbonplan-data-0.4.0/scripts/glas/01_cache_glas_data.ipynb
-drwxr-xr-x   0 jhamman    (501) staff       (20)        0 2021-09-15 20:19:50.748724 carbonplan-data-0.4.0/scripts/global-biomass/
--rw-r--r--   0 jhamman    (501) staff       (20)     3045 2021-04-29 00:01:12.000000 carbonplan-data-0.4.0/scripts/global-biomass/01_biomass_to_cogs.ipynb
-drwxr-xr-x   0 jhamman    (501) staff       (20)        0 2021-09-15 20:19:50.748979 carbonplan-data-0.4.0/scripts/gridmet/
--rw-r--r--   0 jhamman    (501) staff       (20)     4242 2021-04-29 00:01:12.000000 carbonplan-data-0.4.0/scripts/gridmet/01_gridmet_to_zarr.ipynb
-drwxr-xr-x   0 jhamman    (501) staff       (20)        0 2021-09-15 20:19:50.749280 carbonplan-data-0.4.0/scripts/grids/
--rw-r--r--   0 jhamman    (501) staff       (20)    11152 2021-04-29 00:01:12.000000 carbonplan-data-0.4.0/scripts/grids/make_grid.ipynb
-drwxr-xr-x   0 jhamman    (501) staff       (20)        0 2021-09-15 20:19:50.749553 carbonplan-data-0.4.0/scripts/iiasa/
--rw-r--r--   0 jhamman    (501) staff       (20)     4159 2021-04-29 00:01:13.000000 carbonplan-data-0.4.0/scripts/iiasa/01_raw_to_parquet.ipynb
-drwxr-xr-x   0 jhamman    (501) staff       (20)        0 2021-09-15 20:19:50.752535 carbonplan-data-0.4.0/scripts/mtbs/
--rw-r--r--   0 jhamman    (501) staff       (20)     4763 2021-04-29 00:01:12.000000 carbonplan-data-0.4.0/scripts/mtbs/01_raw_to_cogs.ipynb
--rw-r--r--   0 jhamman    (501) staff       (20)     4394 2021-04-29 00:01:11.000000 carbonplan-data-0.4.0/scripts/mtbs/02_downsampling_and_reprojection.ipynb
--rw-r--r--   0 jhamman    (501) staff       (20)     9366 2021-04-29 00:01:12.000000 carbonplan-data-0.4.0/scripts/mtbs/02_mtbs_to_zarr.ipynb
--rw-r--r--   0 jhamman    (501) staff       (20)     9366 2021-04-29 00:01:12.000000 carbonplan-data-0.4.0/scripts/mtbs/03_mtbs_to_zarr.ipynb
--rw-r--r--   0 jhamman    (501) staff       (20)     9129 2021-04-29 00:01:12.000000 carbonplan-data-0.4.0/scripts/mtbs/04_mtbs_perims_to_raster.ipynb
--rw-r--r--   0 jhamman    (501) staff       (20)     7129 2021-04-29 00:01:11.000000 carbonplan-data-0.4.0/scripts/mtbs/05_monthly_downsampling.ipynb
--rw-r--r--   0 jhamman    (501) staff       (20)     9602 2021-04-29 00:01:13.000000 carbonplan-data-0.4.0/scripts/mtbs/05_monthly_mtbs_to_zarr.ipynb
--rw-r--r--   0 jhamman    (501) staff       (20)     5618 2021-02-08 19:32:03.000000 carbonplan-data-0.4.0/scripts/mtbs/05_monthly_mtbs_to_zarr.py
--rw-r--r--   0 jhamman    (501) staff       (20)      901 2021-02-08 19:32:03.000000 carbonplan-data-0.4.0/scripts/mtbs/06_annual_downsampling.py
--rw-r--r--   0 jhamman    (501) staff       (20)     5238 2021-02-08 19:32:03.000000 carbonplan-data-0.4.0/scripts/mtbs/06_annual_mtbs_to_zarr.py
--rw-r--r--   0 jhamman    (501) staff       (20)       19 2020-06-18 02:58:30.000000 carbonplan-data-0.4.0/scripts/mtbs/README.md
--rw-r--r--   0 jhamman    (501) staff       (20)     3434 2020-06-05 18:34:44.000000 carbonplan-data-0.4.0/scripts/mtbs/prepare.py
-drwxr-xr-x   0 jhamman    (501) staff       (20)        0 2021-09-15 20:19:50.753144 carbonplan-data-0.4.0/scripts/nftd/
--rw-r--r--   0 jhamman    (501) staff       (20)     2756 2021-04-29 00:01:11.000000 carbonplan-data-0.4.0/scripts/nftd/00_download.ipynb
--rw-r--r--   0 jhamman    (501) staff       (20)     5835 2021-04-29 00:01:12.000000 carbonplan-data-0.4.0/scripts/nftd/01_nftd_to_cogs.ipynb
--rw-r--r--   0 jhamman    (501) staff       (20)     7152 2021-04-29 00:01:13.000000 carbonplan-data-0.4.0/scripts/nftd/02_downsampling_and_reprojection.ipynb
-drwxr-xr-x   0 jhamman    (501) staff       (20)        0 2021-09-15 20:19:50.754032 carbonplan-data-0.4.0/scripts/nlcd/
--rw-r--r--   0 jhamman    (501) staff       (20)     2843 2021-04-29 00:01:13.000000 carbonplan-data-0.4.0/scripts/nlcd/00_download.ipynb
--rw-r--r--   0 jhamman    (501) staff       (20)     5309 2021-04-29 00:01:13.000000 carbonplan-data-0.4.0/scripts/nlcd/01_nlcd_to_cogs.ipynb
--rw-r--r--   0 jhamman    (501) staff       (20)     9787 2021-04-29 00:01:13.000000 carbonplan-data-0.4.0/scripts/nlcd/02_downsampling_and_reprojection.ipynb
--rw-r--r--   0 jhamman    (501) staff       (20)       38 2020-07-07 17:11:54.000000 carbonplan-data-0.4.0/scripts/nlcd/README.md
-drwxr-xr-x   0 jhamman    (501) staff       (20)        0 2021-09-15 20:19:50.754668 carbonplan-data-0.4.0/scripts/prism/
--rw-r--r--   0 jhamman    (501) staff       (20)     2122 2021-04-29 00:01:11.000000 carbonplan-data-0.4.0/scripts/prism/00_download.ipynb
--rw-r--r--   0 jhamman    (501) staff       (20)     4209 2021-04-29 00:01:12.000000 carbonplan-data-0.4.0/scripts/prism/01_prism_to_cogs.ipynb
--rw-r--r--   0 jhamman    (501) staff       (20)     3459 2021-04-29 00:01:11.000000 carbonplan-data-0.4.0/scripts/prism/02_downsample_and_reproject.ipynb
-drwxr-xr-x   0 jhamman    (501) staff       (20)        0 2021-09-15 20:19:50.754910 carbonplan-data-0.4.0/scripts/statsgo/
--rw-r--r--   0 jhamman    (501) staff       (20)      757 2020-10-19 16:59:06.000000 carbonplan-data-0.4.0/scripts/statsgo/01_raw_to_tif.py
-drwxr-xr-x   0 jhamman    (501) staff       (20)        0 2021-09-15 20:19:50.755859 carbonplan-data-0.4.0/scripts/terraclimate/
--rw-r--r--   0 jhamman    (501) staff       (20)     2848 2021-04-29 00:01:13.000000 carbonplan-data-0.4.0/scripts/terraclimate/01_terraclimate_aux_fileds_to_zarr.ipynb
--rw-r--r--   0 jhamman    (501) staff       (20)    12290 2021-04-29 00:01:12.000000 carbonplan-data-0.4.0/scripts/terraclimate/01_terraclimate_to_zarr3.ipynb
--rw-r--r--   0 jhamman    (501) staff       (20)     6256 2021-04-29 00:01:12.000000 carbonplan-data-0.4.0/scripts/terraclimate/02_terraclimate_regrid.ipynb
--rw-r--r--   0 jhamman    (501) staff       (20)     8352 2021-04-29 00:01:12.000000 carbonplan-data-0.4.0/scripts/terraclimate/02_terraclimate_to_fiaplots.ipynb
-drwxr-xr-x   0 jhamman    (501) staff       (20)        0 2021-09-15 20:19:50.756128 carbonplan-data-0.4.0/scripts/worldclim/
--rw-r--r--   0 jhamman    (501) staff       (20)    72360 2021-09-15 15:02:44.000000 carbonplan-data-0.4.0/scripts/worldclim/01_raw_to_zarr.ipynb
--rw-r--r--   0 jhamman    (501) staff       (20)      485 2021-09-15 20:19:50.764413 carbonplan-data-0.4.0/setup.cfg
--rw-r--r--   0 jhamman    (501) staff       (20)     1387 2020-10-19 16:59:27.000000 carbonplan-data-0.4.0/setup.py
--rw-r--r--   0 jhamman    (501) staff       (20)     4389 2020-09-04 15:20:19.000000 carbonplan-data-0.4.0/sources.yaml
-drwxr-xr-x   0 jhamman    (501) staff       (20)        0 2021-09-15 20:19:50.759241 carbonplan-data-0.4.0/web/
--rw-r--r--   0 jhamman    (501) staff       (20)        4 2020-09-04 15:20:19.000000 carbonplan-data-0.4.0/web/.vercelignore
-drwxr-xr-x   0 jhamman    (501) staff       (20)        0 2021-09-15 20:19:50.762342 carbonplan-data-0.4.0/web/components/
--rw-r--r--   0 jhamman    (501) staff       (20)     3211 2020-09-24 17:48:58.000000 carbonplan-data-0.4.0/web/components/browser.js
--rw-r--r--   0 jhamman    (501) staff       (20)     1971 2020-09-10 16:54:53.000000 carbonplan-data-0.4.0/web/components/catalog.js
--rw-r--r--   0 jhamman    (501) staff       (20)     1851 2020-09-11 15:13:12.000000 carbonplan-data-0.4.0/web/components/code-block.js
--rw-r--r--   0 jhamman    (501) staff       (20)      755 2020-09-04 15:20:19.000000 carbonplan-data-0.4.0/web/components/expander.js
--rw-r--r--   0 jhamman    (501) staff       (20)     3792 2020-09-24 17:52:28.000000 carbonplan-data-0.4.0/web/components/filter.js
--rw-r--r--   0 jhamman    (501) staff       (20)     4177 2020-09-24 17:52:12.000000 carbonplan-data-0.4.0/web/components/header.js
--rw-r--r--   0 jhamman    (501) staff       (20)     1300 2020-09-10 16:04:46.000000 carbonplan-data-0.4.0/web/components/layout.js
--rw-r--r--   0 jhamman    (501) staff       (20)     6386 2020-09-04 15:20:19.000000 carbonplan-data-0.4.0/web/components/logo.js
--rw-r--r--   0 jhamman    (501) staff       (20)     1655 2020-09-04 15:20:19.000000 carbonplan-data-0.4.0/web/components/seo.js
--rw-r--r--   0 jhamman    (501) staff       (20)     5705 2020-10-19 16:59:06.000000 carbonplan-data-0.4.0/web/components/source.js
--rw-r--r--   0 jhamman    (501) staff       (20)     3042 2020-09-09 14:47:52.000000 carbonplan-data-0.4.0/web/components/switch.js
--rw-r--r--   0 jhamman    (501) staff       (20)    44041 2020-10-19 21:41:14.000000 carbonplan-data-0.4.0/web/data.js
--rw-r--r--   0 jhamman    (501) staff       (20)      527 2020-10-19 16:59:06.000000 carbonplan-data-0.4.0/web/intake-to-js.py
--rw-r--r--   0 jhamman    (501) staff       (20)      168 2020-09-04 15:20:19.000000 carbonplan-data-0.4.0/web/next.config.js
--rw-r--r--   0 jhamman    (501) staff       (20)   138963 2021-04-28 23:18:14.000000 carbonplan-data-0.4.0/web/package-lock.json
--rw-r--r--   0 jhamman    (501) staff       (20)     1323 2021-02-08 19:32:03.000000 carbonplan-data-0.4.0/web/package.json
-drwxr-xr-x   0 jhamman    (501) staff       (20)        0 2021-09-15 20:19:50.762819 carbonplan-data-0.4.0/web/pages/
--rw-r--r--   0 jhamman    (501) staff       (20)      315 2020-09-24 17:50:40.000000 carbonplan-data-0.4.0/web/pages/_app.js
--rw-r--r--   0 jhamman    (501) staff       (20)      536 2020-09-04 15:20:19.000000 carbonplan-data-0.4.0/web/pages/_document.js
-drwxr-xr-x   0 jhamman    (501) staff       (20)        0 2021-09-15 20:19:50.737581 carbonplan-data-0.4.0/web/pages/api/
-drwxr-xr-x   0 jhamman    (501) staff       (20)        0 2021-09-15 20:19:50.763312 carbonplan-data-0.4.0/web/pages/api/intake/
--rw-r--r--   0 jhamman    (501) staff       (20)      575 2020-09-09 19:51:11.000000 carbonplan-data-0.4.0/web/pages/api/intake/[id].js
--rw-r--r--   0 jhamman    (501) staff       (20)      208 2020-09-09 19:38:00.000000 carbonplan-data-0.4.0/web/pages/api/intake/index.js
-drwxr-xr-x   0 jhamman    (501) staff       (20)        0 2021-09-15 20:19:50.763557 carbonplan-data-0.4.0/web/pages/data/
--rw-r--r--   0 jhamman    (501) staff       (20)     1630 2020-09-24 17:56:35.000000 carbonplan-data-0.4.0/web/pages/data/index.js
--rw-r--r--   0 jhamman    (501) staff       (20)     2246 2020-09-24 17:58:09.000000 carbonplan-data-0.4.0/web/theme.js
-drwxr-xr-x   0 jhamman    (501) staff       (20)        0 2021-09-15 20:19:50.763815 carbonplan-data-0.4.0/web/utils/
--rw-r--r--   0 jhamman    (501) staff       (20)      971 2020-09-24 17:59:10.000000 carbonplan-data-0.4.0/web/utils/search.js
--rw-r--r--   0 jhamman    (501) staff       (20)      166 2020-09-04 15:20:19.000000 carbonplan-data-0.4.0/web/vercel.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:52:15.064181 carbonplan_data-0.4.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:52:15.056181 carbonplan_data-0.4.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:52:15.056181 carbonplan_data-0.4.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/.github/workflows/main.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/.github/workflows/pypi-release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/.prettierrc.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-04-12 21:52:15.064181 carbonplan_data-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:52:15.056181 carbonplan_data-0.4.3/carbonplan_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/carbonplan_data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:52:15.060181 carbonplan_data-0.4.3/carbonplan_data/catalogs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/carbonplan_data/catalogs/fia.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/carbonplan_data/catalogs/fluxnet.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/carbonplan_data/catalogs/gcp.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/carbonplan_data/catalogs/gridmet.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/carbonplan_data/catalogs/grids.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/carbonplan_data/catalogs/maca.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/carbonplan_data/catalogs/master.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6882 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/carbonplan_data/catalogs/mtbs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/carbonplan_data/catalogs/nftd.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6417 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/carbonplan_data/catalogs/nlcd.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/carbonplan_data/catalogs/projects.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/carbonplan_data/catalogs/spawnetal2020.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/carbonplan_data/catalogs/terraclimate.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/carbonplan_data/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:52:15.060181 carbonplan_data-0.4.3/carbonplan_data/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4080 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/carbonplan_data/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/carbonplan_data/tests/test_catalogs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/carbonplan_data/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7815 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/carbonplan_data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:52:15.064181 carbonplan_data-0.4.3/carbonplan_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-04-12 21:52:15.000000 carbonplan_data-0.4.3/carbonplan_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-04-12 21:52:15.000000 carbonplan_data-0.4.3/carbonplan_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 21:52:15.000000 carbonplan_data-0.4.3/carbonplan_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-12 21:52:15.000000 carbonplan_data-0.4.3/carbonplan_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-12 21:52:15.000000 carbonplan_data-0.4.3/carbonplan_data.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:52:15.060181 carbonplan_data-0.4.3/ci/
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/ci/environment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:52:15.052181 carbonplan_data-0.4.3/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:52:15.060181 carbonplan_data-0.4.3/scripts/fia/
+-rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/scripts/fia/00_download.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5075 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/scripts/fia/01_raw_to_parquet.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    10017 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/scripts/fia/01_raw_to_parquet_part2.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:52:15.060181 carbonplan_data-0.4.3/scripts/fluxnet/
+-rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/scripts/fluxnet/01_raw_to_parquet.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    26846 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/scripts/fluxnet/download.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:52:15.060181 carbonplan_data-0.4.3/scripts/gcp/
+-rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/scripts/gcp/01_raw_to_parquet.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:52:15.060181 carbonplan_data-0.4.3/scripts/glas/
+-rw-r--r--   0 runner    (1001) docker     (127)    16528 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/scripts/glas/01_cache_glas_data.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:52:15.060181 carbonplan_data-0.4.3/scripts/global-biomass/
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/scripts/global-biomass/01_biomass_to_cogs.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:52:15.060181 carbonplan_data-0.4.3/scripts/gridmet/
+-rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/scripts/gridmet/01_gridmet_to_zarr.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:52:15.060181 carbonplan_data-0.4.3/scripts/grids/
+-rw-r--r--   0 runner    (1001) docker     (127)    10956 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/scripts/grids/make_grid.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:52:15.060181 carbonplan_data-0.4.3/scripts/iiasa/
+-rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/scripts/iiasa/01_raw_to_parquet.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:52:15.064181 carbonplan_data-0.4.3/scripts/mtbs/
+-rw-r--r--   0 runner    (1001) docker     (127)     4763 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/scripts/mtbs/01_raw_to_cogs.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4196 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/scripts/mtbs/02_downsampling_and_reprojection.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9142 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/scripts/mtbs/02_mtbs_to_zarr.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9142 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/scripts/mtbs/03_mtbs_to_zarr.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9058 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/scripts/mtbs/04_mtbs_perims_to_raster.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6573 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/scripts/mtbs/05_monthly_downsampling.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9578 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/scripts/mtbs/05_monthly_mtbs_to_zarr.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5618 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/scripts/mtbs/05_monthly_mtbs_to_zarr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/scripts/mtbs/06_annual_downsampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/scripts/mtbs/06_annual_mtbs_to_zarr.py
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/scripts/mtbs/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/scripts/mtbs/prepare.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:52:15.064181 carbonplan_data-0.4.3/scripts/nftd/
+-rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/scripts/nftd/00_download.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5769 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/scripts/nftd/01_nftd_to_cogs.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6758 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/scripts/nftd/02_downsampling_and_reprojection.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:52:15.064181 carbonplan_data-0.4.3/scripts/nlcd/
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/scripts/nlcd/00_download.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/scripts/nlcd/01_nlcd_to_cogs.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9477 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/scripts/nlcd/02_downsampling_and_reprojection.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/scripts/nlcd/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:52:15.064181 carbonplan_data-0.4.3/scripts/prism/
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/scripts/prism/00_download.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/scripts/prism/01_prism_to_cogs.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/scripts/prism/02_downsample_and_reproject.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:52:15.064181 carbonplan_data-0.4.3/scripts/statsgo/
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/scripts/statsgo/01_raw_to_tif.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:52:15.064181 carbonplan_data-0.4.3/scripts/terraclimate/
+-rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/scripts/terraclimate/01_terraclimate_aux_fileds_to_zarr.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    12218 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/scripts/terraclimate/01_terraclimate_to_zarr3.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/scripts/terraclimate/02_terraclimate_regrid.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8352 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/scripts/terraclimate/02_terraclimate_to_fiaplots.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:52:15.064181 carbonplan_data-0.4.3/scripts/worldclim/
+-rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/scripts/worldclim/01_raw_to_zarr.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 21:52:15.064181 carbonplan_data-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4389 2024-04-12 21:52:05.000000 carbonplan_data-0.4.3/sources.yaml
```

### Comparing `carbonplan-data-0.4.0/.gitignore` & `carbonplan_data-0.4.3/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 wheels/
 pip-wheel-metadata/
 share/python-wheels/
 *.egg-info/
 .installed.cfg
 *.egg
 MANIFEST
+carbonplan_data/_version.py
 
 # PyInstaller
 #  Usually these files are written by a python script from a template
 #  before PyInstaller builds the exe, so as to inject date/other infos into it.
 *.manifest
 *.spec
```

### Comparing `carbonplan-data-0.4.0/LICENSE` & `carbonplan_data-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `carbonplan-data-0.4.0/README.md` & `carbonplan_data-0.4.3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,154 +1,164 @@
-00000000: 3c69 6d67 0a20 2073 7263 3d27 6874 7470  <img.  src='http
-00000010: 733a 2f2f 6361 7262 6f6e 706c 616e 2d61  s://carbonplan-a
-00000020: 7373 6574 732e 7333 2e61 6d61 7a6f 6e61  ssets.s3.amazona
-00000030: 7773 2e63 6f6d 2f6d 6f6e 6f67 7261 6d2f  ws.com/monogram/
-00000040: 6461 726b 2d73 6d61 6c6c 2e70 6e67 270a  dark-small.png'.
-00000050: 2020 6865 6967 6874 3d27 3438 270a 2f3e    height='48'./>
-00000060: 0a0a 2320 6361 7262 6f6e 706c 616e 202f  ..# carbonplan /
-00000070: 2064 6174 610a 0a2a 2a64 6174 6120 6361   data..**data ca
-00000080: 7461 6c6f 6720 616e 6420 6375 7261 7469  talog and curati
-00000090: 6f6e 2a2a 0a0a 5b21 5b47 6974 4875 625d  on**..[![GitHub]
-000000a0: 5b67 6974 6875 622d 6261 6467 655d 5d5b  [github-badge]][
-000000b0: 6769 7468 7562 5d0a 5b21 5b42 7569 6c64  github].[![Build
-000000c0: 2053 7461 7475 735d 5d5b 6163 7469 6f6e   Status]][action
-000000d0: 735d 0a21 5b4d 4954 204c 6963 656e 7365  s].![MIT License
-000000e0: 5d5b 5d0a 0a5b 6769 7468 7562 5d3a 2068  ][]..[github]: h
-000000f0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000100: 6d2f 6361 7262 6f6e 706c 616e 2f64 6174  m/carbonplan/dat
-00000110: 610a 5b67 6974 6875 622d 6261 6467 655d  a.[github-badge]
-00000120: 3a20 6874 7470 733a 2f2f 6261 6467 656e  : https://badgen
-00000130: 2e6e 6574 2f62 6164 6765 2f2d 2f67 6974  .net/badge/-/git
-00000140: 6875 623f 6963 6f6e 3d67 6974 6875 6226  hub?icon=github&
-00000150: 6c61 6265 6c0a 5b62 7569 6c64 2073 7461  label.[build sta
-00000160: 7475 735d 3a20 6874 7470 733a 2f2f 6769  tus]: https://gi
-00000170: 7468 7562 2e63 6f6d 2f63 6172 626f 6e70  thub.com/carbonp
-00000180: 6c61 6e2f 6461 7461 2f61 6374 696f 6e73  lan/data/actions
-00000190: 2f77 6f72 6b66 6c6f 7773 2f6d 6169 6e2e  /workflows/main.
-000001a0: 7961 6d6c 2f62 6164 6765 2e73 7667 0a5b  yaml/badge.svg.[
-000001b0: 6163 7469 6f6e 735d 3a20 6874 7470 733a  actions]: https:
-000001c0: 2f2f 6769 7468 7562 2e63 6f6d 2f63 6172  //github.com/car
-000001d0: 626f 6e70 6c61 6e2f 6461 7461 2f61 6374  bonplan/data/act
-000001e0: 696f 6e73 2f77 6f72 6b66 6c6f 7773 2f6d  ions/workflows/m
-000001f0: 6169 6e2e 7961 6d6c 0a5b 6d69 7420 6c69  ain.yaml.[mit li
-00000200: 6365 6e73 655d 3a20 6874 7470 733a 2f2f  cense]: https://
-00000210: 6261 6467 656e 2e6e 6574 2f62 6164 6765  badgen.net/badge
-00000220: 2f6c 6963 656e 7365 2f4d 4954 2f62 6c75  /license/MIT/blu
-00000230: 650a 0a54 6869 7320 7265 706f 7369 746f  e..This reposito
-00000240: 7279 2069 6e63 6c75 6465 7320 6f75 7220  ry includes our 
-00000250: 6d61 696e 2064 6174 6120 6361 7461 6c6f  main data catalo
-00000260: 6720 6173 2077 656c 6c20 6173 206f 7572  g as well as our
-00000270: 2070 7265 2d70 726f 6365 7373 696e 6720   pre-processing 
-00000280: 7574 696c 6974 6965 732e 0a0a 2323 2069  utilities...## i
-00000290: 6e73 7461 6c6c 0a0a 6060 6073 6865 6c6c  nstall..```shell
-000002a0: 0a70 6970 2063 6172 626f 6e70 6c61 6e5b  .pip carbonplan[
-000002b0: 6461 7461 5d0a 6060 600a 0a23 2320 7573  data].```..## us
-000002c0: 6167 650a 0a54 6865 2043 6172 626f 6e50  age..The CarbonP
-000002d0: 6c61 6e20 6461 7461 2061 7263 6869 7665  lan data archive
-000002e0: 7320 6172 6520 6375 7272 656e 746c 7920  s are currently 
-000002f0: 6d69 7272 6f72 6564 206f 6e20 476f 6f67  mirrored on Goog
-00000300: 6c65 2043 6c6f 7564 2053 746f 7261 6765  le Cloud Storage
-00000310: 2028 5553 2d43 656e 7472 616c 2920 616e   (US-Central) an
-00000320: 640a 4d69 6372 6f73 6f66 7420 417a 7572  d.Microsoft Azur
-00000330: 6520 2855 532d 5765 7374 292e 2053 6574  e (US-West). Set
-00000340: 2074 6865 2060 4341 5242 4f4e 504c 414e   the `CARBONPLAN
-00000350: 5f44 4154 4160 2065 6e76 6972 6f6e 6d65  _DATA` environme
-00000360: 6e74 2076 6172 6961 626c 6520 6265 666f  nt variable befo
-00000370: 7265 2075 7369 6e67 2074 6865 0a49 6e74  re using the.Int
-00000380: 616b 6520 6361 7461 6c6f 6720 6265 6c6f  ake catalog belo
-00000390: 773a 0a0a 6060 6073 6865 6c6c 0a23 2067  w:..```shell.# g
-000003a0: 6f6f 676c 6520 2875 732d 6365 6e74 7261  oogle (us-centra
-000003b0: 6c29 0a65 7870 6f72 7420 4341 5242 4f4e  l).export CARBON
-000003c0: 504c 414e 5f44 4154 413d 2268 7474 7073  PLAN_DATA="https
-000003d0: 3a2f 2f73 746f 7261 6765 2e67 6f6f 676c  ://storage.googl
-000003e0: 6561 7069 732e 636f 6d2f 6361 7262 6f6e  eapis.com/carbon
-000003f0: 706c 616e 2d64 6174 6122 0a23 206f 720a  plan-data".# or.
-00000400: 2320 617a 7572 6520 2875 732d 7765 7374  # azure (us-west
-00000410: 290a 6578 706f 7274 2043 4152 424f 4e50  ).export CARBONP
-00000420: 4c41 4e5f 4441 5441 3d22 6874 7470 733a  LAN_DATA="https:
-00000430: 2f2f 6361 7262 6f6e 706c 616e 2e62 6c6f  //carbonplan.blo
-00000440: 622e 636f 7265 2e77 696e 646f 7773 2e6e  b.core.windows.n
-00000450: 6574 2f63 6172 626f 6e70 6c61 6e2d 6461  et/carbonplan-da
-00000460: 7461 220a 6060 600a 0a60 6060 7079 7468  ta".```..```pyth
-00000470: 6f6e 0a23 206f 7065 6e20 7468 6520 746f  on.# open the to
-00000480: 7020 6c65 7665 6c20 6361 7461 6c6f 670a  p level catalog.
-00000490: 6672 6f6d 2063 6172 626f 6e70 6c61 6e2e  from carbonplan.
-000004a0: 6461 7461 2069 6d70 6f72 7420 6361 740a  data import cat.
-000004b0: 0a23 2065 7874 7261 6374 2061 6e20 656e  .# extract an en
-000004c0: 7472 7920 6173 2061 2044 6173 6b2d 6261  try as a Dask-ba
-000004d0: 636b 6564 2058 6172 7261 7920 4461 7461  cked Xarray Data
-000004e0: 7365 740a 6361 742e 6d74 6273 5b22 7261  set.cat.mtbs["ra
-000004f0: 7374 6572 225d 2872 6567 696f 6e3d 2263  ster"](region="c
-00000500: 6f6e 7573 222c 2072 6573 6f6c 7574 696f  onus", resolutio
-00000510: 6e3d 2234 3030 306d 2229 2e74 6f5f 6461  n="4000m").to_da
-00000520: 736b 2829 0a60 6060 0a0a 2d2d 2d0a 0a23  sk().```..---..#
-00000530: 2320 6465 7665 6c6f 7065 7220 646f 6375  # developer docu
-00000540: 6d65 6e74 6174 696f 6e0a 0a54 6f20 7275  mentation..To ru
-00000550: 6e20 7468 6520 756e 6974 2061 6e64 2069  n the unit and i
-00000560: 6e74 6567 7261 7469 6f6e 2074 6573 7473  ntegration tests
-00000570: 2066 6f72 2074 6869 7320 4150 492c 2072   for this API, r
-00000580: 756e 3a0a 0a60 6060 7368 656c 6c0a 2420  un:..```shell.$ 
-00000590: 7079 2e74 6573 7420 2d76 0a60 6060 0a0a  py.test -v.```..
-000005a0: 4361 7461 6c6f 6720 656e 7472 6965 7320  Catalog entries 
-000005b0: 7363 616e 2062 6520 6d61 726b 6564 2061  scan be marked a
-000005c0: 7320 6569 7468 6572 205f 736b 6970 5f20  s either _skip_ 
-000005d0: 6f72 205f 7866 6169 6c5f 2062 7920 7365  or _xfail_ by se
-000005e0: 7474 696e 6720 7468 6520 6063 6960 206b  tting the `ci` k
-000005f0: 6579 2069 6e20 7468 6520 6d65 7461 6461  ey in the metada
-00000600: 7461 2064 6963 7469 6f6e 6172 793a 0a0a  ta dictionary:..
-00000610: 6060 6079 616d 6c0a 666f 6f3a 0a20 2064  ```yaml.foo:.  d
-00000620: 6573 6372 6970 7469 6f6e 3a20 2773 6b69  escription: 'ski
-00000630: 7020 7468 6973 2065 6e74 7279 2069 6e20  p this entry in 
-00000640: 7468 6520 4349 2074 6573 7473 270a 2020  the CI tests'.  
-00000650: 6d65 7461 6461 7461 3a0a 2020 2020 6369  metadata:.    ci
-00000660: 3a20 736b 6970 0a60 6060 0a0a 2323 206c  : skip.```..## l
-00000670: 6963 656e 7365 0a0a 416c 6c20 7468 6520  icense..All the 
-00000680: 636f 6465 2069 6e20 7468 6973 2072 6570  code in this rep
-00000690: 6f73 6974 6f72 7920 6973 205b 4d49 545d  ository is [MIT]
-000006a0: 2868 7474 7073 3a2f 2f63 686f 6f73 6561  (https://choosea
-000006b0: 6c69 6365 6e73 652e 636f 6d2f 6c69 6365  license.com/lice
-000006c0: 6e73 6573 2f6d 6974 2f29 206c 6963 656e  nses/mit/) licen
-000006d0: 7365 642e 2057 6865 6e20 706f 7373 6962  sed. When possib
-000006e0: 6c65 2c20 7468 6520 6461 7461 2069 7320  le, the data is 
-000006f0: 6c69 6365 6e73 6564 2075 7369 6e67 2074  licensed using t
-00000700: 6865 205b 4343 2d42 592d 342e 305d 2868  he [CC-BY-4.0](h
-00000710: 7474 7073 3a2f 2f63 686f 6f73 6561 6c69  ttps://chooseali
-00000720: 6365 6e73 652e 636f 6d2f 6c69 6365 6e73  cense.com/licens
-00000730: 6573 2f63 632d 6279 2d34 2e30 2f29 206c  es/cc-by-4.0/) l
-00000740: 6963 656e 7365 2e20 5765 2069 6e63 6c75  icense. We inclu
-00000750: 6465 2061 7474 7269 6275 7469 6f6e 2061  de attribution a
-00000760: 6e64 2061 6464 6974 696f 6e61 6c20 6c69  nd additional li
-00000770: 6365 6e73 6520 696e 666f 726d 6174 696f  cense informatio
-00000780: 6e20 666f 7220 7468 6972 6420 7061 7274  n for third part
-00000790: 7920 6461 7461 7365 7473 2c20 616e 6420  y datasets, and 
-000007a0: 7765 2072 6571 7565 7374 2074 6861 7420  we request that 
-000007b0: 796f 7520 616c 736f 206d 6169 6e74 6169  you also maintai
-000007c0: 6e20 7468 6174 2061 7474 7269 6275 7469  n that attributi
-000007d0: 6f6e 2069 6620 7573 696e 6720 7468 6973  on if using this
-000007e0: 2064 6174 612e 0a0a 2323 2061 626f 7574   data...## about
-000007f0: 2075 730a 0a43 6172 626f 6e50 6c61 6e20   us..CarbonPlan 
-00000800: 6973 2061 206e 6f6e 2d70 726f 6669 7420  is a non-profit 
-00000810: 6f72 6761 6e69 7a61 7469 6f6e 2074 6861  organization tha
-00000820: 7420 7573 6573 2064 6174 6120 616e 6420  t uses data and 
-00000830: 7363 6965 6e63 6520 666f 7220 636c 696d  science for clim
-00000840: 6174 6520 6163 7469 6f6e 2e20 5765 2061  ate action. We a
-00000850: 696d 2074 6f20 696d 7072 6f76 6520 7468  im to improve th
-00000860: 6520 7472 616e 7370 6172 656e 6379 2061  e transparency a
-00000870: 6e64 2073 6369 656e 7469 6669 6320 696e  nd scientific in
-00000880: 7465 6772 6974 7920 6f66 2063 6172 626f  tegrity of carbo
-00000890: 6e20 7265 6d6f 7661 6c20 616e 6420 636c  n removal and cl
-000008a0: 696d 6174 6520 736f 6c75 7469 6f6e 7320  imate solutions 
-000008b0: 7468 726f 7567 6820 6f70 656e 2064 6174  through open dat
-000008c0: 6120 616e 6420 746f 6f6c 732e 2046 696e  a and tools. Fin
-000008d0: 6420 6f75 7420 6d6f 7265 2061 7420 5b63  d out more at [c
-000008e0: 6172 626f 6e70 6c61 6e2e 6f72 675d 2868  arbonplan.org](h
-000008f0: 7474 7073 3a2f 2f63 6172 626f 6e70 6c61  ttps://carbonpla
-00000900: 6e2e 6f72 672f 2920 6f72 2067 6574 2069  n.org/) or get i
-00000910: 6e20 746f 7563 6820 6279 205b 6f70 656e  n touch by [open
-00000920: 696e 6720 616e 2069 7373 7565 5d28 6874  ing an issue](ht
-00000930: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000940: 2f63 6172 626f 6e70 6c61 6e2f 6461 7461  /carbonplan/data
-00000950: 2f69 7373 7565 732f 6e65 7729 206f 7220  /issues/new) or 
-00000960: 5b73 656e 6469 6e67 2075 7320 616e 2065  [sending us an e
-00000970: 6d61 696c 5d28 6d61 696c 746f 3a68 656c  mail](mailto:hel
-00000980: 6c6f 4063 6172 626f 6e70 6c61 6e2e 6f72  lo@carbonplan.or
-00000990: 6729 2e0a                                g)..
+00000000: 3c70 2061 6c69 676e 3d22 6c65 6674 2220  <p align="left" 
+00000010: 3e0a 3c61 2068 7265 663d 2768 7474 7073  >.<a href='https
+00000020: 3a2f 2f63 6172 626f 6e70 6c61 6e2e 6f72  ://carbonplan.or
+00000030: 6727 3e0a 3c70 6963 7475 7265 3e0a 2020  g'>.<picture>.  
+00000040: 3c73 6f75 7263 6520 6d65 6469 613d 2228  <source media="(
+00000050: 7072 6566 6572 732d 636f 6c6f 722d 7363  prefers-color-sc
+00000060: 6865 6d65 3a20 6461 726b 2922 2073 7263  heme: dark)" src
+00000070: 7365 743d 2268 7474 7073 3a2f 2f63 6172  set="https://car
+00000080: 626f 6e70 6c61 6e2d 6173 7365 7473 2e73  bonplan-assets.s
+00000090: 332e 616d 617a 6f6e 6177 732e 636f 6d2f  3.amazonaws.com/
+000000a0: 6d6f 6e6f 6772 616d 2f6c 6967 6874 2d73  monogram/light-s
+000000b0: 6d61 6c6c 2e70 6e67 223e 0a20 203c 696d  mall.png">.  <im
+000000c0: 6720 616c 743d 2243 6172 626f 6e50 6c61  g alt="CarbonPla
+000000d0: 6e20 6d6f 6e6f 6772 616d 2e22 2068 6569  n monogram." hei
+000000e0: 6768 743d 2234 3822 2073 7263 3d22 6874  ght="48" src="ht
+000000f0: 7470 733a 2f2f 6361 7262 6f6e 706c 616e  tps://carbonplan
+00000100: 2d61 7373 6574 732e 7333 2e61 6d61 7a6f  -assets.s3.amazo
+00000110: 6e61 7773 2e63 6f6d 2f6d 6f6e 6f67 7261  naws.com/monogra
+00000120: 6d2f 6461 726b 2d73 6d61 6c6c 2e70 6e67  m/dark-small.png
+00000130: 223e 0a3c 2f70 6963 7475 7265 3e0a 3c2f  ">.</picture>.</
+00000140: 613e 0a3c 2f70 3e0a 0a23 2063 6172 626f  a>.</p>..# carbo
+00000150: 6e70 6c61 6e20 2f20 6461 7461 0a0a 2a2a  nplan / data..**
+00000160: 6461 7461 2063 6174 616c 6f67 2061 6e64  data catalog and
+00000170: 2063 7572 6174 696f 6e2a 2a0a 0a5b 215b   curation**..[![
+00000180: 4349 5d28 6874 7470 733a 2f2f 6769 7468  CI](https://gith
+00000190: 7562 2e63 6f6d 2f63 6172 626f 6e70 6c61  ub.com/carbonpla
+000001a0: 6e2f 6461 7461 2f61 6374 696f 6e73 2f77  n/data/actions/w
+000001b0: 6f72 6b66 6c6f 7773 2f6d 6169 6e2e 7961  orkflows/main.ya
+000001c0: 6d6c 2f62 6164 6765 2e73 7667 295d 2868  ml/badge.svg)](h
+000001d0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000001e0: 6d2f 6361 7262 6f6e 706c 616e 2f64 6174  m/carbonplan/dat
+000001f0: 612f 6163 7469 6f6e 732f 776f 726b 666c  a/actions/workfl
+00000200: 6f77 732f 6d61 696e 2e79 616d 6c29 0a5b  ows/main.yaml).[
+00000210: 215b 5079 5049 5d28 6874 7470 733a 2f2f  ![PyPI](https://
+00000220: 696d 672e 7368 6965 6c64 732e 696f 2f70  img.shields.io/p
+00000230: 7970 692f 762f 6361 7262 6f6e 706c 616e  ypi/v/carbonplan
+00000240: 2d64 6174 6129 5d28 6874 7470 733a 2f2f  -data)](https://
+00000250: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
+00000260: 2f63 6172 626f 6e70 6c61 6e2d 6461 7461  /carbonplan-data
+00000270: 2f29 0a5b 215b 4c69 6365 6e73 653a 204d  /).[![License: M
+00000280: 4954 5d28 6874 7470 733a 2f2f 696d 672e  IT](https://img.
+00000290: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
+000002a0: 2f4c 6963 656e 7365 2d4d 4954 2d62 6c75  /License-MIT-blu
+000002b0: 652e 7376 6729 5d28 6874 7470 733a 2f2f  e.svg)](https://
+000002c0: 6f70 656e 736f 7572 6365 2e6f 7267 2f6c  opensource.org/l
+000002d0: 6963 656e 7365 732f 4d49 5429 0a0a 5468  icenses/MIT)..Th
+000002e0: 6973 2072 6570 6f73 6974 6f72 7920 696e  is repository in
+000002f0: 636c 7564 6573 206f 7572 206d 6169 6e20  cludes our main 
+00000300: 6461 7461 2063 6174 616c 6f67 2061 7320  data catalog as 
+00000310: 7765 6c6c 2061 7320 6f75 7220 7072 652d  well as our pre-
+00000320: 7072 6f63 6573 7369 6e67 2075 7469 6c69  processing utili
+00000330: 7469 6573 2e0a 0a23 2320 696e 7374 616c  ties...## instal
+00000340: 6c0a 0a60 6060 7368 656c 6c0a 7079 7468  l..```shell.pyth
+00000350: 6f6e 202d 6d20 7069 7020 696e 7374 616c  on -m pip instal
+00000360: 6c20 6361 7262 6f6e 706c 616e 5b64 6174  l carbonplan[dat
+00000370: 615d 0a60 6060 0a0a 2323 2075 7361 6765  a].```..## usage
+00000380: 0a0a 5468 6520 4361 7262 6f6e 506c 616e  ..The CarbonPlan
+00000390: 2064 6174 6120 6172 6368 6976 6573 2061   data archives a
+000003a0: 7265 2063 7572 7265 6e74 6c79 206d 6972  re currently mir
+000003b0: 726f 7265 6420 6f6e 2047 6f6f 676c 6520  rored on Google 
+000003c0: 436c 6f75 6420 5374 6f72 6167 6520 2855  Cloud Storage (U
+000003d0: 532d 4365 6e74 7261 6c29 2061 6e64 0a4d  S-Central) and.M
+000003e0: 6963 726f 736f 6674 2041 7a75 7265 2028  icrosoft Azure (
+000003f0: 5553 2d57 6573 7429 2e20 5365 7420 7468  US-West). Set th
+00000400: 6520 6043 4152 424f 4e50 4c41 4e5f 4441  e `CARBONPLAN_DA
+00000410: 5441 6020 656e 7669 726f 6e6d 656e 7420  TA` environment 
+00000420: 7661 7269 6162 6c65 2062 6566 6f72 6520  variable before 
+00000430: 7573 696e 6720 7468 650a 496e 7461 6b65  using the.Intake
+00000440: 2063 6174 616c 6f67 2062 656c 6f77 3a0a   catalog below:.
+00000450: 0a60 6060 7368 656c 6c0a 2320 676f 6f67  .```shell.# goog
+00000460: 6c65 2028 7573 2d63 656e 7472 616c 290a  le (us-central).
+00000470: 6578 706f 7274 2043 4152 424f 4e50 4c41  export CARBONPLA
+00000480: 4e5f 4441 5441 3d22 6874 7470 733a 2f2f  N_DATA="https://
+00000490: 7374 6f72 6167 652e 676f 6f67 6c65 6170  storage.googleap
+000004a0: 6973 2e63 6f6d 2f63 6172 626f 6e70 6c61  is.com/carbonpla
+000004b0: 6e2d 6461 7461 220a 2320 6f72 0a23 2061  n-data".# or.# a
+000004c0: 7a75 7265 2028 7573 2d77 6573 7429 0a65  zure (us-west).e
+000004d0: 7870 6f72 7420 4341 5242 4f4e 504c 414e  xport CARBONPLAN
+000004e0: 5f44 4154 413d 2268 7474 7073 3a2f 2f63  _DATA="https://c
+000004f0: 6172 626f 6e70 6c61 6e2e 626c 6f62 2e63  arbonplan.blob.c
+00000500: 6f72 652e 7769 6e64 6f77 732e 6e65 742f  ore.windows.net/
+00000510: 6361 7262 6f6e 706c 616e 2d64 6174 6122  carbonplan-data"
+00000520: 0a60 6060 0a0a 6060 6070 7974 686f 6e0a  .```..```python.
+00000530: 2320 6f70 656e 2074 6865 2074 6f70 206c  # open the top l
+00000540: 6576 656c 2063 6174 616c 6f67 0a66 726f  evel catalog.fro
+00000550: 6d20 6361 7262 6f6e 706c 616e 2e64 6174  m carbonplan.dat
+00000560: 6120 696d 706f 7274 2063 6174 0a0a 2320  a import cat..# 
+00000570: 6578 7472 6163 7420 616e 2065 6e74 7279  extract an entry
+00000580: 2061 7320 6120 4461 736b 2d62 6163 6b65   as a Dask-backe
+00000590: 6420 5861 7272 6179 2044 6174 6173 6574  d Xarray Dataset
+000005a0: 0a63 6174 2e6d 7462 735b 2272 6173 7465  .cat.mtbs["raste
+000005b0: 7222 5d28 7265 6769 6f6e 3d22 636f 6e75  r"](region="conu
+000005c0: 7322 2c20 7265 736f 6c75 7469 6f6e 3d22  s", resolution="
+000005d0: 3430 3030 6d22 292e 746f 5f64 6173 6b28  4000m").to_dask(
+000005e0: 290a 6060 600a 0a2d 2d2d 0a0a 2323 2064  ).```..---..## d
+000005f0: 6576 656c 6f70 6572 2064 6f63 756d 656e  eveloper documen
+00000600: 7461 7469 6f6e 0a0a 546f 2072 756e 2074  tation..To run t
+00000610: 6865 2075 6e69 7420 616e 6420 696e 7465  he unit and inte
+00000620: 6772 6174 696f 6e20 7465 7374 7320 666f  gration tests fo
+00000630: 7220 7468 6973 2041 5049 2c20 7275 6e3a  r this API, run:
+00000640: 0a0a 6060 6073 6865 6c6c 0a24 2070 7974  ..```shell.$ pyt
+00000650: 6573 7420 2d76 0a60 6060 0a0a 4361 7461  est -v.```..Cata
+00000660: 6c6f 6720 656e 7472 6965 7320 7363 616e  log entries scan
+00000670: 2062 6520 6d61 726b 6564 2061 7320 6569   be marked as ei
+00000680: 7468 6572 205f 736b 6970 5f20 6f72 205f  ther _skip_ or _
+00000690: 7866 6169 6c5f 2062 7920 7365 7474 696e  xfail_ by settin
+000006a0: 6720 7468 6520 6063 6960 206b 6579 2069  g the `ci` key i
+000006b0: 6e20 7468 6520 6d65 7461 6461 7461 2064  n the metadata d
+000006c0: 6963 7469 6f6e 6172 793a 0a0a 6060 6079  ictionary:..```y
+000006d0: 616d 6c0a 666f 6f3a 0a20 2064 6573 6372  aml.foo:.  descr
+000006e0: 6970 7469 6f6e 3a20 2273 6b69 7020 7468  iption: "skip th
+000006f0: 6973 2065 6e74 7279 2069 6e20 7468 6520  is entry in the 
+00000700: 4349 2074 6573 7473 220a 2020 6d65 7461  CI tests".  meta
+00000710: 6461 7461 3a0a 2020 2020 6369 3a20 736b  data:.    ci: sk
+00000720: 6970 0a60 6060 0a0a 2323 206c 6963 656e  ip.```..## licen
+00000730: 7365 0a0a 416c 6c20 7468 6520 636f 6465  se..All the code
+00000740: 2069 6e20 7468 6973 2072 6570 6f73 6974   in this reposit
+00000750: 6f72 7920 6973 205b 4d49 545d 2868 7474  ory is [MIT](htt
+00000760: 7073 3a2f 2f63 686f 6f73 6561 6c69 6365  ps://choosealice
+00000770: 6e73 652e 636f 6d2f 6c69 6365 6e73 6573  nse.com/licenses
+00000780: 2f6d 6974 2f29 2d6c 6963 656e 7365 642e  /mit/)-licensed.
+00000790: 2057 6865 6e20 706f 7373 6962 6c65 2c20   When possible, 
+000007a0: 7468 6520 6461 7461 2069 7320 6c69 6365  the data is lice
+000007b0: 6e73 6564 2075 7369 6e67 2074 6865 205b  nsed using the [
+000007c0: 4343 2d42 592d 342e 305d 2868 7474 7073  CC-BY-4.0](https
+000007d0: 3a2f 2f63 686f 6f73 6561 6c69 6365 6e73  ://choosealicens
+000007e0: 652e 636f 6d2f 6c69 6365 6e73 6573 2f63  e.com/licenses/c
+000007f0: 632d 6279 2d34 2e30 2f29 206c 6963 656e  c-by-4.0/) licen
+00000800: 7365 2e20 5765 2069 6e63 6c75 6465 2061  se. We include a
+00000810: 7474 7269 6275 7469 6f6e 2061 6e64 2061  ttribution and a
+00000820: 6464 6974 696f 6e61 6c20 6c69 6365 6e73  dditional licens
+00000830: 6520 696e 666f 726d 6174 696f 6e20 666f  e information fo
+00000840: 7220 7468 6972 6420 7061 7274 7920 6461  r third party da
+00000850: 7461 7365 7473 2c20 616e 6420 7765 2072  tasets, and we r
+00000860: 6571 7565 7374 2074 6861 7420 796f 7520  equest that you 
+00000870: 616c 736f 206d 6169 6e74 6169 6e20 7468  also maintain th
+00000880: 6174 2061 7474 7269 6275 7469 6f6e 2069  at attribution i
+00000890: 6620 7573 696e 6720 7468 6973 2064 6174  f using this dat
+000008a0: 612e 0a0a 2323 2061 626f 7574 2075 730a  a...## about us.
+000008b0: 0a43 6172 626f 6e50 6c61 6e20 6973 2061  .CarbonPlan is a
+000008c0: 206e 6f6e 7072 6f66 6974 206f 7267 616e   nonprofit organ
+000008d0: 697a 6174 696f 6e20 7468 6174 2075 7365  ization that use
+000008e0: 7320 6461 7461 2061 6e64 2073 6369 656e  s data and scien
+000008f0: 6365 2066 6f72 2063 6c69 6d61 7465 2061  ce for climate a
+00000900: 6374 696f 6e2e 2057 6520 6169 6d20 746f  ction. We aim to
+00000910: 2069 6d70 726f 7665 2074 6865 2074 7261   improve the tra
+00000920: 6e73 7061 7265 6e63 7920 616e 6420 7363  nsparency and sc
+00000930: 6965 6e74 6966 6963 2069 6e74 6567 7269  ientific integri
+00000940: 7479 206f 6620 636c 696d 6174 6520 736f  ty of climate so
+00000950: 6c75 7469 6f6e 7320 7769 7468 206f 7065  lutions with ope
+00000960: 6e20 6461 7461 2061 6e64 2074 6f6f 6c73  n data and tools
+00000970: 2e20 4669 6e64 206f 7574 206d 6f72 6520  . Find out more 
+00000980: 6174 205b 6361 7262 6f6e 706c 616e 2e6f  at [carbonplan.o
+00000990: 7267 5d28 6874 7470 733a 2f2f 6361 7262  rg](https://carb
+000009a0: 6f6e 706c 616e 2e6f 7267 2f29 206f 7220  onplan.org/) or 
+000009b0: 6765 7420 696e 2074 6f75 6368 2062 7920  get in touch by 
+000009c0: 5b6f 7065 6e69 6e67 2061 6e20 6973 7375  [opening an issu
+000009d0: 655d 2868 7474 7073 3a2f 2f67 6974 6875  e](https://githu
+000009e0: 622e 636f 6d2f 6361 7262 6f6e 706c 616e  b.com/carbonplan
+000009f0: 2f64 6174 612f 6973 7375 6573 2f6e 6577  /data/issues/new
+00000a00: 2920 6f72 205b 7365 6e64 696e 6720 7573  ) or [sending us
+00000a10: 2061 6e20 656d 6169 6c5d 286d 6169 6c74   an email](mailt
+00000a20: 6f3a 6865 6c6c 6f40 6361 7262 6f6e 706c  o:hello@carbonpl
+00000a30: 616e 2e6f 7267 292e 0a                   an.org)..
```

### Comparing `carbonplan-data-0.4.0/carbonplan_data/catalogs/fia.yaml` & `carbonplan_data-0.4.3/carbonplan_data/catalogs/fia.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -89,9 +89,9 @@
             veg_plot_species,
             veg_quadrat,
             veg_subplot,
             veg_subplot_spp,
             veg_visit,
           ]
     args:
-      urlpath: '{{env(CARBONPLAN_DATA)}}/raw/fia/{{ name }}.parquet'
-      engine: 'pyarrow'
+      urlpath: "{{env(CARBONPLAN_DATA)}}/raw/fia/{{ name }}.parquet"
+      engine: "pyarrow"
```

### Comparing `carbonplan-data-0.4.0/carbonplan_data/catalogs/fluxnet.yaml` & `carbonplan_data-0.4.3/carbonplan_data/catalogs/fluxnet.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
       kind:
         description: fluxnet data stream
         type: str
         default: auxmeteo
         allowed: [auxmeteo, auxnee]
     driver: parquet
     args:
-      urlpath: '{{env(CARBONPLAN_DATA)}}/raw/fluxnet/{{ station }}_{{ kind }}.parquet'
+      urlpath: "{{env(CARBONPLAN_DATA)}}/raw/fluxnet/{{ station }}_{{ kind }}.parquet"
 
   raw_fullset:
     metadata:
       title: FLUXNET FULLSET Data (raw)
       summary: Global network of micrometeorological flux measurement measuring carbon, energy and water cycles.
       description: |
         The preparation of this FLUXNET Dataset has been possible thanks only to the efforts of
@@ -78,8 +78,8 @@
       freq:
         description: temporal frequency
         type: str
         default: dd
         allowed: [dd, hh, mm, ww, yy]
     driver: parquet
     args:
-      urlpath: '{{env(CARBONPLAN_DATA)}}/raw/fluxnet/{{ station }}_{{ kind }}_{{ freq }}.parquet'
+      urlpath: "{{env(CARBONPLAN_DATA)}}/raw/fluxnet/{{ station }}_{{ kind }}_{{ freq }}.parquet"
```

### Comparing `carbonplan-data-0.4.0/carbonplan_data/catalogs/gcp.yaml` & `carbonplan_data-0.4.3/carbonplan_data/catalogs/gcp.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -34,8 +34,8 @@
             historical_budget,
             consumption_emissions,
             territorial_emissions,
             transfer_emissions,
           ]
     driver: parquet
     args:
-      urlpath: '{{env(CARBONPLAN_DATA)}}/raw/gcp/{{ name }}.parquet'
+      urlpath: "{{env(CARBONPLAN_DATA)}}/raw/gcp/{{ name }}.parquet"
```

### Comparing `carbonplan-data-0.4.0/carbonplan_data/catalogs/gridmet.yaml` & `carbonplan_data-0.4.3/carbonplan_data/catalogs/gridmet.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -24,31 +24,31 @@
     parameters:
       variable:
         description: climate variable
         type: str
         default: pr
         allowed:
           [
-            'pr',
-            'tmmn',
-            'tmmx',
-            'rmax',
-            'rmin',
-            'sph',
-            'srad',
-            'th',
-            'vs',
-            'bi',
-            'fm100',
-            'fm1000',
-            'erc',
-            'pdsi',
-            'etr',
-            'pet',
-            'vpd',
+            "pr",
+            "tmmn",
+            "tmmx",
+            "rmax",
+            "rmin",
+            "sph",
+            "srad",
+            "th",
+            "vs",
+            "bi",
+            "fm100",
+            "fm1000",
+            "erc",
+            "pdsi",
+            "etr",
+            "pet",
+            "vpd",
           ]
       year:
         description: year
         type: int
         default: 2000
     args:
       urlpath: http://thredds.northwestknowledge.net:8080/thredds/dodsC/MET/{{ variable }}/{{ variable }}_{{ '%04d' % year }}.nc
```

### Comparing `carbonplan-data-0.4.0/carbonplan_data/catalogs/grids.yaml` & `carbonplan_data-0.4.3/carbonplan_data/catalogs/grids.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -24,9 +24,9 @@
       region:
         description: conus or ak
         type: str
         default: conus
         allowed: [conus, ak]
     driver: zarr
     args:
-      urlpath: '{{env(CARBONPLAN_DATA)}}/processed/grids/{{ region }}/4000m/domain.zarr/'
+      urlpath: "{{env(CARBONPLAN_DATA)}}/processed/grids/{{ region }}/4000m/domain.zarr/"
       consolidated: True
```

### Comparing `carbonplan-data-0.4.0/carbonplan_data/catalogs/maca.yaml` & `carbonplan_data-0.4.3/carbonplan_data/catalogs/maca.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -23,34 +23,34 @@
     parameters:
       variable:
         description: climate variable
         type: str
         default: pr
         allowed:
           [
-            'huss',
-            'pr',
-            'rhsmin',
-            'rhsmax',
-            'rsds',
-            'tasmax',
-            'tasmin',
-            'uas',
-            'vas',
-            'vpd',
+            "huss",
+            "pr",
+            "rhsmin",
+            "rhsmax",
+            "rsds",
+            "tasmax",
+            "tasmin",
+            "uas",
+            "vas",
+            "vpd",
           ]
       gcm:
         description: climate model
         type: str
         default: IPSL-CM5A-LR
         # allowed: TODO: add list of defaults
       scenario:
         description: climate scenario
         type: str
         default: historical_1950_2005
-        allowed: ['historical_1950_2005', 'rcp45_2006_2099', 'rcp85_2006_2099']
+        allowed: ["historical_1950_2005", "rcp45_2006_2099", "rcp85_2006_2099"]
     args:
       urlpath: http://thredds.northwestknowledge.net:8080/thredds/dodsC/agg_macav2metdata_{{ variable }}_{{ gcm }}_r1i1p1_{{ scenario }}_CONUS_daily.nc
       auth: null
       chunks:
         lat: 585
         lon: 1386
```

### Comparing `carbonplan-data-0.4.0/carbonplan_data/catalogs/master.yaml` & `carbonplan_data-0.4.3/carbonplan_data/catalogs/master.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,109 +1,109 @@
-description: 'CarbonPlan Master Data Catalog'
+description: "CarbonPlan Master Data Catalog"
 sources:
   gridmet:
-    name: 'gridMET'
-    description: 'Gridded daily surface meteorological data covering the continental US'
+    name: "gridMET"
+    description: "Gridded daily surface meteorological data covering the continental US"
     metadata:
       tags: [climate]
     driver: intake.catalog.local.YAMLFileCatalog
     args:
-      path: '{{CATALOG_DIR}}/gridmet.yaml'
+      path: "{{CATALOG_DIR}}/gridmet.yaml"
 
   terraclimate:
-    name: 'TerraClimate'
-    description: 'Global gridded monthly climate and hydroclimate data from 1958-present.'
+    name: "TerraClimate"
+    description: "Global gridded monthly climate and hydroclimate data from 1958-present."
     metadata:
       tags: [climate]
     driver: intake.catalog.local.YAMLFileCatalog
     args:
-      path: '{{CATALOG_DIR}}/terraclimate.yaml'
+      path: "{{CATALOG_DIR}}/terraclimate.yaml"
 
   maca:
-    name: 'MACA'
-    description: 'Statistically downscaled climate data using the MACA method.'
+    name: "MACA"
+    description: "Statistically downscaled climate data using the MACA method."
     metadata:
       tags: [climate]
     driver: intake.catalog.local.YAMLFileCatalog
     args:
-      path: '{{CATALOG_DIR}}/maca.yaml'
+      path: "{{CATALOG_DIR}}/maca.yaml"
 
   fia:
-    name: 'Forest Inventory Analysis (FIA)'
-    description: 'Catalog for data from Forest Inventory Analysis (FIA) database'
+    name: "Forest Inventory Analysis (FIA)"
+    description: "Catalog for data from Forest Inventory Analysis (FIA) database"
     metadata:
       tags: [forests]
     driver: intake.catalog.local.YAMLFileCatalog
     args:
-      path: '{{CATALOG_DIR}}/fia.yaml'
+      path: "{{CATALOG_DIR}}/fia.yaml"
 
   fluxnet:
-    name: 'FLUXNET'
-    description: 'Catalog for data from the FLUXNET dataset'
+    name: "FLUXNET"
+    description: "Catalog for data from the FLUXNET dataset"
     metadata:
       tags: [climate, carbon]
     driver: intake.catalog.local.YAMLFileCatalog
     args:
-      path: '{{CATALOG_DIR}}/fluxnet.yaml'
+      path: "{{CATALOG_DIR}}/fluxnet.yaml"
 
   gcp:
-    name: 'Global Carbon Project (GCP)'
-    description: 'Catalog for data from the Global Carbon Project'
+    name: "Global Carbon Project (GCP)"
+    description: "Catalog for data from the Global Carbon Project"
     metadata:
       tags: [climate, carbon]
     driver: intake.catalog.local.YAMLFileCatalog
     args:
-      path: '{{CATALOG_DIR}}/gcp.yaml'
+      path: "{{CATALOG_DIR}}/gcp.yaml"
 
   mtbs:
-    name: 'Monitoring Trends in Burn Severity (MTBS)'
-    description: 'Catalog for data from the Monitoring Trends in Burn Severity (MTBS) dataset'
+    name: "Monitoring Trends in Burn Severity (MTBS)"
+    description: "Catalog for data from the Monitoring Trends in Burn Severity (MTBS) dataset"
     metadata:
       tags: [forests]
     driver: intake.catalog.local.YAMLFileCatalog
     args:
-      path: '{{CATALOG_DIR}}/mtbs.yaml'
+      path: "{{CATALOG_DIR}}/mtbs.yaml"
 
   nftd:
-    name: 'National Forest Type Database (NFTD)'
-    description: 'Catalog for data from the National Forest Type Database (NFTD)'
+    name: "National Forest Type Database (NFTD)"
+    description: "Catalog for data from the National Forest Type Database (NFTD)"
     metadata:
       tags: [forests]
     driver: intake.catalog.local.YAMLFileCatalog
     args:
-      path: '{{CATALOG_DIR}}/nftd.yaml'
+      path: "{{CATALOG_DIR}}/nftd.yaml"
 
   nlcd:
-    name: 'National Land Cover Database (NLCD)'
-    description: 'Catalog for data from the National Land Cover Database (NLCD)'
+    name: "National Land Cover Database (NLCD)"
+    description: "Catalog for data from the National Land Cover Database (NLCD)"
     metadata:
       tags: [forests]
     driver: intake.catalog.local.YAMLFileCatalog
     args:
-      path: '{{CATALOG_DIR}}/nlcd.yaml'
+      path: "{{CATALOG_DIR}}/nlcd.yaml"
 
   projects:
-    name: 'CarbonPlan Project Reports'
-    description: 'CarbonPlan Projects Dataset Catalog'
+    name: "CarbonPlan Project Reports"
+    description: "CarbonPlan Projects Dataset Catalog"
     metadata:
       tags: [carbon]
     driver: intake.catalog.local.YAMLFileCatalog
     args:
-      path: '{{CATALOG_DIR}}/projects.yaml'
+      path: "{{CATALOG_DIR}}/projects.yaml"
 
   spawnetal2020:
-    name: 'Global Above- and Belowground Biomass'
-    description: 'Catalog for data from Global Aboveground and Belowground Biomass Carbon Density Maps for the Year 2010 from Spawn et al (2020)'
+    name: "Global Above- and Belowground Biomass"
+    description: "Catalog for data from Global Aboveground and Belowground Biomass Carbon Density Maps for the Year 2010 from Spawn et al (2020)"
     metadata:
       tags: [forests]
     driver: intake.catalog.local.YAMLFileCatalog
     args:
-      path: '{{CATALOG_DIR}}/spawnetal2020.yaml'
+      path: "{{CATALOG_DIR}}/spawnetal2020.yaml"
 
   grids:
-    name: 'Project Grids'
-    description: 'Catalog grid files and domain definitions.'
+    name: "Project Grids"
+    description: "Catalog grid files and domain definitions."
     metadata:
       tags: [meta]
     driver: intake.catalog.local.YAMLFileCatalog
     args:
-      path: '{{CATALOG_DIR}}/grids.yaml'
+      path: "{{CATALOG_DIR}}/grids.yaml"
```

### Comparing `carbonplan-data-0.4.0/carbonplan_data/catalogs/mtbs.yaml` & `carbonplan_data-0.4.3/carbonplan_data/catalogs/mtbs.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         type: str
         default: conus
         allowed: [conus, ak]
     driver: rasterio
     args:
       # urlpath: "https://storage.googleapis.com/carbonplan-data/raw/mtbs/{{ region }}/30m/{{ '%d' % year }}.tif"
       urlpath: "{{env(CARBONPLAN_DATA)}}/raw/mtbs/{{ region }}/30m/{{ '%d' % year }}.tif"
-      chunks: { 'y': 5120, 'x': 5120 }
+      chunks: { "y": 5120, "x": 5120 }
 
   raster:
     metadata:
       title: MTBS (processed)
       summary: Annual burn severity mosaics for the continental United States and Alaska.
       description: |
         Monitoring Trends in Burn Severity (MTBS) is an interagency program whose goal is to
@@ -69,19 +69,19 @@
         description: conus or ak
         type: str
         default: conus
         allowed: [conus, ak]
       resolution:
         description: Pixel resolution in meters
         type: str
-        default: '4000m'
-        allowed: ['4000m']
+        default: "4000m"
+        allowed: ["4000m"]
     driver: zarr
     args:
-      urlpath: '{{env(CARBONPLAN_DATA)}}/processed/mtbs/{{ region }}/{{ resolution }}/raster.zarr'
+      urlpath: "{{env(CARBONPLAN_DATA)}}/processed/mtbs/{{ region }}/{{ resolution }}/raster.zarr"
       consolidated: True
 
   rasterized_perims:
     metadata:
       title: MTBS Rasterized Fire Perimeters (processed)
       summary: Monthly burned area rasters for the continental United States and Alaska.
       description: |
@@ -103,29 +103,29 @@
         description: conus or ak
         type: str
         default: conus
         allowed: [conus, ak]
       resolution:
         description: Pixel resolution in meters
         type: str
-        default: '30m'
-        allowed: ['30m']
+        default: "30m"
+        allowed: ["30m"]
       size:
         description: Fire size
         type: str
-        default: 'lf'
-        allowed: ['lf', 'vlf']
+        default: "lf"
+        allowed: ["lf", "vlf"]
       date:
-        description: 'Year and month (format: YYYY.MM)'
+        description: "Year and month (format: YYYY.MM)"
         type: str
-        default: '2018.11'
+        default: "2018.11"
     driver: rasterio
     args:
-      urlpath: '{{env(CARBONPLAN_DATA)}}/processed/mtbs/{{ region }}/{{ resolution }}/{{ size }}_{{ date }}.tif'
-      chunks: { 'y': 5120, 'x': 5120 }
+      urlpath: "{{env(CARBONPLAN_DATA)}}/processed/mtbs/{{ region }}/{{ resolution }}/{{ size }}_{{ date }}.tif"
+      chunks: { "y": 5120, "x": 5120 }
 
   fod_shp:
     metadata:
       title: MTBS Occurance (vector data)
       summary: Fire occurance location dataset in vector/point format.
       description: |
         The fire occurrence location dataset is a vector point ESRI shapefile of the centroids of
@@ -137,15 +137,15 @@
       providers:
         - name: Monitoring Trends in Burn Severity
           description: Monitoring Trends in Burn Severity (MTBS) is an interagency program that includes the USGS, NASA, USFS, USDI, and USDA.
           url: https://www.mtbs.gov/
       ci: skip
     driver: shapefile
     args:
-      urlpath: '{{env(CARBONPLAN_DATA)}}/raw/mtbs/mtbs_fod_pts_data/mtbs_fod_pts_DD.shp'
+      urlpath: "{{env(CARBONPLAN_DATA)}}/raw/mtbs/mtbs_fod_pts_data/mtbs_fod_pts_DD.shp"
 
   perims_shp:
     metadata:
       title: MTBS Boundaries (vector data)
       summary: Burned area boundaries data in vector/polygon format.
       description: |
         The burned area boundaries dataset is a vector polygon ESRI shapefile of the extent of the
@@ -157,8 +157,8 @@
       providers:
         - name: Monitoring Trends in Burn Severity
           description: Monitoring Trends in Burn Severity (MTBS) is an interagency program that includes the USGS, NASA, USFS, USDI, and USDA.
           url: https://www.mtbs.gov/
       ci: skip
     driver: shapefile
     args:
-      urlpath: '{{env(CARBONPLAN_DATA)}}/raw/mtbs/mtbs_perimeter_data/mtbs_perims_DD.shp'
+      urlpath: "{{env(CARBONPLAN_DATA)}}/raw/mtbs/mtbs_perimeter_data/mtbs_perims_DD.shp"
```

### Comparing `carbonplan-data-0.4.0/carbonplan_data/catalogs/nftd.yaml` & `carbonplan_data-0.4.3/carbonplan_data/catalogs/nftd.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -39,16 +39,16 @@
       variable:
         description: foresttype or forestgroup
         type: str
         default: foresttype
         allowed: [foresttype, forestgroup]
     driver: rasterio
     args:
-      urlpath: '{{env(CARBONPLAN_DATA)}}/raw/nftd/{{ region }}_{{ variable }}/250m/{{ option }}.tif'
-      chunks: { 'y': 5120, 'x': 5120 }
+      urlpath: "{{env(CARBONPLAN_DATA)}}/raw/nftd/{{ region }}_{{ variable }}/250m/{{ option }}.tif"
+      chunks: { "y": 5120, "x": 5120 }
 
   raster:
     metadata:
       title: National Forest Type Dataset (processed)
       summary: Extent, distribution, and forest type composition of the nation’s forests.
       description: |
         This geospatial dataset was created by the USFS Forest Inventory and Analysis (FIA) program
@@ -84,9 +84,9 @@
       resolution:
         description: pixel resolution in meters
         type: str
         default: 4000m
         allowed: [250m, 4000m]
     driver: rasterio
     args:
-      urlpath: '{{env(CARBONPLAN_DATA)}}/processed/nftd/{{ region }}/{{ resolution }}/{{ option }}.tif'
-      chunks: { 'y': 5120, 'x': 5120 }
+      urlpath: "{{env(CARBONPLAN_DATA)}}/processed/nftd/{{ region }}/{{ resolution }}/{{ option }}.tif"
+      chunks: { "y": 5120, "x": 5120 }
```

### Comparing `carbonplan-data-0.4.0/carbonplan_data/catalogs/nlcd.yaml` & `carbonplan_data-0.4.3/carbonplan_data/catalogs/nlcd.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -44,16 +44,16 @@
       region:
         description: conus or ak
         type: str
         default: conus
         allowed: [conus, ak]
     driver: rasterio
     args:
-      urlpath: '{{env(CARBONPLAN_DATA)}}/raw/nlcd/{{ region }}/30m/{{ option }}.tif'
-      chunks: { 'y': 5120, 'x': 5120 }
+      urlpath: "{{env(CARBONPLAN_DATA)}}/raw/nlcd/{{ region }}/30m/{{ option }}.tif"
+      chunks: { "y": 5120, "x": 5120 }
 
   raster:
     metadata:
       title: National Land Cover Database (processed)
       summary: The National Land Cover Database - 2001 to 2016.
       description: |
         The U.S. Geological Survey (USGS), in partnership with several federal agencies, has
@@ -99,9 +99,9 @@
       region:
         description: conus or ak
         type: str
         default: conus
         allowed: [conus, ak]
     driver: rasterio
     args:
-      urlpath: '{{env(CARBONPLAN_DATA)}}/processed/nlcd/{{ region }}/{{ resolution }}/{{ option }}.tif'
-      chunks: { 'y': 5120, 'x': 5120 }
+      urlpath: "{{env(CARBONPLAN_DATA)}}/processed/nlcd/{{ region }}/{{ resolution }}/{{ option }}.tif"
+      chunks: { "y": 5120, "x": 5120 }
```

### Comparing `carbonplan-data-0.4.0/carbonplan_data/catalogs/projects.yaml` & `carbonplan_data-0.4.3/carbonplan_data/catalogs/projects.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -13,8 +13,8 @@
         - name: CarbonPlan
           description: |
             CarbonPlan is a registered non-profit public benefit corporation working on
             the science and data of carbon removal.
           url: https://carbonplan.org
     driver: csv
     args:
-      urlpath: 'https://api.carbonplan.org/projects.csv'
+      urlpath: "https://api.carbonplan.org/projects.csv"
```

### Comparing `carbonplan-data-0.4.0/carbonplan_data/catalogs/spawnetal2020.yaml` & `carbonplan_data-0.4.3/carbonplan_data/catalogs/spawnetal2020.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -40,9 +40,9 @@
             aboveground,
             aboveground_uncertainty,
             belowground,
             belowground_uncertainty,
           ]
     driver: rasterio
     args:
-      urlpath: '{{env(CARBONPLAN_DATA)}}/raw/2010-harmonized-biomass/global/300m/{{ variable }}.tif'
-      chunks: { 'y': 5120, 'x': 5120 }
+      urlpath: "{{env(CARBONPLAN_DATA)}}/raw/2010-harmonized-biomass/global/300m/{{ variable }}.tif"
+      chunks: { "y": 5120, "x": 5120 }
```

### Comparing `carbonplan-data-0.4.0/carbonplan_data/catalogs/terraclimate.yaml` & `carbonplan_data-0.4.3/carbonplan_data/catalogs/terraclimate.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
       license: Creative Commons Public Domain (CC0)
       providers:
         - name: Climatology Lab, University of California, Merced
           description: Data provided by Dr. John Abatzoglou's Climatology Lab at the University of California, Merced.
           url: http://www.climatologylab.org
     driver: zarr
     args:
-      urlpath: '{{env(CARBONPLAN_DATA)}}/raw/terraclimate/4000m/raster.zarr'
+      urlpath: "{{env(CARBONPLAN_DATA)}}/raw/terraclimate/4000m/raster.zarr"
       consolidated: True
 
   raster:
     metadata:
       title: TerraClimate (processed)
       summary: Climate and climaticwater balance data from 1958-2019.
       description: |
@@ -48,13 +48,13 @@
         description: conus or ak
         type: str
         default: conus
         allowed: [conus, ak]
       resolution:
         description: Pixel resolution in meters
         type: str
-        default: '4000m'
-        allowed: ['4000m']
+        default: "4000m"
+        allowed: ["4000m"]
     driver: zarr
     args:
-      urlpath: '{{env(CARBONPLAN_DATA)}}/processed/terraclimate/{{ region }}/{{ resolution }}/raster.zarr'
+      urlpath: "{{env(CARBONPLAN_DATA)}}/processed/terraclimate/{{ region }}/{{ resolution }}/raster.zarr"
       consolidated: True
```

### Comparing `carbonplan-data-0.4.0/carbonplan_data/metadata.py` & `carbonplan_data-0.4.3/carbonplan_data/metadata.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,21 @@
+from __future__ import annotations
+
 import getpass
 import os
 import socket
 import sys
 import time
 
 from . import __version__
 
 
 def get_cf_global_attrs(**attrs):
-
     if "history" not in attrs:
-        attrs["history"] = "Created: {}".format(time.ctime(time.time()))
+        attrs["history"] = f"Created: {time.ctime(time.time())}"
 
     if "insitution" not in attrs:
         attrs["institution"] = "CarbonPlan"
 
     if "source" not in attrs:
         attrs["source"] = sys.argv[0]
```

### Comparing `carbonplan-data-0.4.0/carbonplan_data/tests/__init__.py` & `carbonplan_data-0.4.3/carbonplan_data/tests/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,16 +47,16 @@
     if callable(obj):
         if not isinstance(obj, partial):
             return obj.__name__
 
         if not obj.keywords:
             return obj.func.__name__
 
-        kwstring = ",".join(["{}={}".format(k, v) for k, v in obj.keywords.items()])
-        return "{}({})".format(obj.func.__name__, kwstring)
+        kwstring = ",".join([f"{k}={v}" for k, v in obj.keywords.items()])
+        return f"{obj.func.__name__}({kwstring})"
 
 
 def parametrize_with_checks(catalog):
     """Pytest specific decorator for parametrizing catalog checks.
     The `id` of each check is set to be a pprint version of the catalog
     and the name of the check with its keyword arguments.
     This allows to use `pytest -k` to specify which tests to run::
@@ -74,14 +74,15 @@
     Examples
     --------
     >>> from carbonplan.data.tests import parametrize_with_checks
     >>> from carbonplan.data import cat
     >>> @parametrize_with_checks(cat)
     ... def test_catalog(entry, check):
     ...     check(entry)
+    ...
 
     """
     import pytest
 
     checks_generator = itertools.chain.from_iterable(
         check_entry(name, entry) for name, entry in dict(catalog.walk(depth=10)).items()
     )
```

### Comparing `carbonplan-data-0.4.0/carbonplan_data/tests/test_utils.py` & `carbonplan_data-0.4.3/carbonplan_data/tests/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,14 @@
     ds = set_zarr_encoding(temperature)
     ds.to_zarr(store)
     assert "foo" not in ds.air.encoding
     assert ds.air.encoding.get("compressor", None)
     assert ds.air.encoding.get("_FillValue", None)
 
     ds = set_zarr_encoding(temperature, float_dtype="float16")
-    ds.to_zarr(store, mode='w')
+    ds.to_zarr(store, mode="w")
     assert "f2" in ds.air.dtype.str
 
 
-
 def test_get_versions():
     versions = get_versions()
     assert versions["carbonplan_data"]
```

### Comparing `carbonplan-data-0.4.0/carbonplan_data/utils.py` & `carbonplan_data-0.4.3/carbonplan_data/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+from __future__ import annotations
+
 import importlib
 import os
 import pathlib
 import zipfile
-from typing import Dict, Optional
 
 import numpy as np
-import urlpath
+import validators
 import wget
 import xarray as xr
 import yaml
 from numpy.typing import DTypeLike
 
 root = pathlib.Path(__file__).parents[2]
 
@@ -119,23 +120,21 @@
         blob = bucket.blob(target)
         blob.upload_from_filename(src)
 
     return workdir, upload
 
 
 def get_sources():
-
     with open(root / "sources.yaml") as f:
         sources = yaml.load(f, Loader=yaml.FullLoader)
 
     return sources
 
 
 def get_workdir(workdir):
-
     # fallback to cwd
     if workdir is None:
         workdir = os.getcwd()
 
     # cast to pathlib obj
     if isinstance(workdir, str):
         workdir = pathlib.Path(workdir)
@@ -143,26 +142,25 @@
     # make sure workdir exists
     workdir.mkdir(parents=True, exist_ok=True)
 
     return workdir
 
 
 def process_sources(name, workdir=None):
-
     sources = get_sources()
     workdir = get_workdir(workdir)
 
     results = {"download": [], "unzip": []}
 
     for key, dset in sources[name]["data"].items():
-
         # download
         if "download" in dset["actions"]:
             for url in dset["urlpath"]:
-                url = urlpath.URL(url)
+                if not validators.url(url):
+                    raise ValueError(f'url "{url}" not valid')
                 out = workdir / url.name
                 if not out.exists():
                     print(f"downloading {url}")
                     wget.download(str(url), out=str(out))
 
                 results["download"].append(out)
 
@@ -178,17 +176,17 @@
                     results["unzip"].append(outdir.glob("**/*"))
 
     return results
 
 
 def set_zarr_encoding(
     ds: xr.Dataset,
-    codec_config: Optional[Dict] = None,
-    float_dtype: Optional[DTypeLike] = None,
-    int_dtype: Optional[DTypeLike] = None,
+    codec_config: dict | None = None,
+    float_dtype: DTypeLike | None = None,
+    int_dtype: DTypeLike | None = None,
 ) -> xr.Dataset:
     """Set zarr encoding for each variable in the dataset
 
     Parameters
     ----------
     ds : xr.Dataset
         Input dataset
@@ -207,15 +205,14 @@
     ds = ds.copy()
 
     if codec_config is None:
         codec_config = {"id": "zlib", "level": 1}
     compressor = numcodecs.get_codec(codec_config)
 
     for k, da in ds.variables.items():
-
         # maybe cast float type
         if np.issubdtype(da.dtype, np.floating) and float_dtype is not None:
             da = da.astype(float_dtype)
 
         if np.issubdtype(da.dtype, np.integer) and int_dtype is not None:
             da = da.astype(int_dtype)
 
@@ -246,15 +243,15 @@
         "numpy",
         "scipy",
         "fsspec",
         "intake",
         "rasterio",
         "zarr",
     ]
-) -> Dict[str, str]:
+) -> dict[str, str]:
     """Helper to fetch commonly used package versions
     Parameters
     ----------
     packages : list
         List of packages to fetch versions for
     Returns
     -------
```

### Comparing `carbonplan-data-0.4.0/scripts/fia/00_download.ipynb` & `carbonplan_data-0.4.3/scripts/fia/00_download.ipynb`

 * *Files identical despite different names*

### Comparing `carbonplan-data-0.4.0/scripts/fia/01_raw_to_parquet.ipynb` & `carbonplan_data-0.4.3/scripts/fia/01_raw_to_parquet.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998931623931624%*

 * *Differences: {"'cells'": "{4: {'source': {delete: [4]}}}"}*

```diff
@@ -72,15 +72,14 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "\n",
                 "\n",
                 "def force_float32(fname):\n",
-                "\n",
                 "    memmap = fname.stat().st_size > 1e8\n",
                 "\n",
                 "    df = pd.read_csv(fname, engine=\"c\", low_memory=False, memory_map=memmap)\n",
                 "    for c in df:\n",
                 "        if \"f8\" in df[c].dtype.str:\n",
                 "            df[c] = df[c].astype(np.float32)\n",
                 "\n",
```

### Comparing `carbonplan-data-0.4.0/scripts/fia/01_raw_to_parquet_part2.ipynb` & `carbonplan_data-0.4.3/scripts/fia/01_raw_to_parquet_part2.ipynb`

 * *Files identical despite different names*

### Comparing `carbonplan-data-0.4.0/scripts/fluxnet/01_raw_to_parquet.ipynb` & `carbonplan_data-0.4.3/scripts/fluxnet/01_raw_to_parquet.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9984274193548387%*

 * *Differences: {"'cells'": "{4: {'metadata': {delete: ['collapsed']}, 'source': {insert: [(24, '        ddf = "*

 * *            'dd.from_pandas(df, chunksize=1000).repartition(partition_size="50MB")\\n\')], delete: '*

 * *            '[26, 25, 24]}}}'}*

```diff
@@ -66,15 +66,14 @@
                 "storage_options = {\"token\": fs.session.credentials, \"project\": \"carbonplan\"}"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
-                "collapsed": true,
                 "jupyter": {
                     "outputs_hidden": true
                 }
             },
             "outputs": [],
             "source": [
                 "zips = (workdir / \"fluxnet\").glob(\"*zip\")\n",
@@ -97,17 +96,15 @@
                 "\n",
                 "    for csv in csvs:\n",
                 "        fname = pathlib.PosixPath(csv)\n",
                 "        name = make_fname(fname.stem)\n",
                 "        blob = blob = f\"gcs://carbonplan-data/raw/fluxnet/{name}.parquet\"\n",
                 "\n",
                 "        df = pd.read_csv(zipfs.open(csv, mode=\"rb\"))\n",
-                "        ddf = dd.from_pandas(df, chunksize=1000).repartition(\n",
-                "            partition_size=\"50MB\"\n",
-                "        )\n",
+                "        ddf = dd.from_pandas(df, chunksize=1000).repartition(partition_size=\"50MB\")\n",
                 "        ddf.to_parquet(blob, storage_options=storage_options)\n",
                 "\n",
                 "        print(\"--> \", blob)"
             ]
         }
     ],
     "metadata": {
```

### Comparing `carbonplan-data-0.4.0/scripts/fluxnet/download.sh` & `carbonplan_data-0.4.3/scripts/fluxnet/download.sh`

 * *Files identical despite different names*

### Comparing `carbonplan-data-0.4.0/scripts/gcp/01_raw_to_parquet.ipynb` & `carbonplan_data-0.4.3/scripts/gcp/01_raw_to_parquet.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9992379597642755%*

 * *Differences: {"'cells'": "{4: {'source': {insert: [(0, 'fname = (\\n'), (1, '    "*

 * *            '"/Users/jhamman/workdir/carbonplan_data_downloads/gcp/National_Carbon_Emissions_2019v1.0.xlsx"\\n\'), '*

 * *            "(2, ')\\n')], delete: [0]}}, 6: {'source': {insert: [(9, 'open_kwargs = "*

 * *            'dict(sheet_name="Fossil Emissions by Fuel Type", skiprows=12, index_col=0)\\n\'), '*

 * *            '(14, \'open_kwargs = dict(sheet_name="Land-Use Change Emissions", skiprows=25, '*

 * *            "index_col=0)\\n')], delete: [18, 1 […]*

```diff
@@ -69,15 +69,17 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "fname = \"/Users/jhamman/workdir/carbonplan_data_downloads/gcp/National_Carbon_Emissions_2019v1.0.xlsx\"\n",
+                "fname = (\n",
+                "    \"/Users/jhamman/workdir/carbonplan_data_downloads/gcp/National_Carbon_Emissions_2019v1.0.xlsx\"\n",
+                ")\n",
                 "\n",
                 "# Territorial Emissions\n",
                 "target = \"gs://carbonplan-data/raw/gcp/consumption_emissions.parquet\"\n",
                 "open_kwargs = dict(sheet_name=\"Territorial Emissions\", skiprows=16, index_col=0)\n",
                 "process(fname, target, **open_kwargs)\n",
                 "\n",
                 "# Consumption Emissions\n",
@@ -109,24 +111,20 @@
                 "# Global Carbon Budget\n",
                 "target = \"gs://carbonplan-data/raw/gcp/global_carbon_budget.parquet\"\n",
                 "open_kwargs = dict(sheet_name=\"Global Carbon Budget\", skiprows=18, index_col=0)\n",
                 "process(fname, target, **open_kwargs)\n",
                 "\n",
                 "# Fossil Emissions by Fuel Type\n",
                 "target = \"gs://carbonplan-data/raw/gcp/fossil_emissions_by_fuel_type.parquet\"\n",
-                "open_kwargs = dict(\n",
-                "    sheet_name=\"Fossil Emissions by Fuel Type\", skiprows=12, index_col=0\n",
-                ")\n",
+                "open_kwargs = dict(sheet_name=\"Fossil Emissions by Fuel Type\", skiprows=12, index_col=0)\n",
                 "process(fname, target, **open_kwargs)\n",
                 "\n",
                 "# Land-Use Change Emissions\n",
                 "target = \"gs://carbonplan-data/raw/gcp/land_use_change_emissions.parquet\"\n",
-                "open_kwargs = dict(\n",
-                "    sheet_name=\"Land-Use Change Emissions\", skiprows=25, index_col=0\n",
-                ")\n",
+                "open_kwargs = dict(sheet_name=\"Land-Use Change Emissions\", skiprows=25, index_col=0)\n",
                 "process(fname, target, **open_kwargs)\n",
                 "\n",
                 "# Ocean Sink\n",
                 "target = \"gs://carbonplan-data/raw/gcp/ocean_sink.parquet\"\n",
                 "open_kwargs = dict(sheet_name=\"Ocean Sink\", skiprows=22, index_col=0)\n",
                 "process(fname, target, **open_kwargs)\n",
                 "\n",
```

### Comparing `carbonplan-data-0.4.0/scripts/glas/01_cache_glas_data.ipynb` & `carbonplan_data-0.4.3/scripts/glas/01_cache_glas_data.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9993550368550368%*

 * *Differences: {"'cells'": "{0: {'metadata': {delete: ['collapsed']}}, 1: {'source': {insert: [(116, '        "*

 * *            "username, account, password = info.authenticators(urlparse(URS_URL).hostname)\\n'), "*

 * *            "(129, '        credentials = "*

 * *            'base64.b64encode(credentials.encode("ascii")).decode("ascii")\\n\'), (181, \'        '*

 * *            'params += "&producer_granule_id[]={0}{1}".format(filename_filter, option)\\n\'), '*

 * *            '(190, \'    entries = [e["links"] for e in search_results["feed […]*

```diff
@@ -1,14 +1,13 @@
 {
     "cells": [
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
-                "collapsed": true,
                 "jupyter": {
                     "outputs_hidden": true
                 }
             },
             "outputs": [],
             "source": [
                 "pip install git+https://github.com/pangeo-forge/pangeo-forge.git"
@@ -132,32 +131,28 @@
                 "\n",
                 "def get_credentials(url):\n",
                 "    \"\"\"Get user credentials from .netrc or prompt for input.\"\"\"\n",
                 "    credentials = None\n",
                 "    errprefix = \"\"\n",
                 "    try:\n",
                 "        info = netrc.netrc()\n",
-                "        username, account, password = info.authenticators(\n",
-                "            urlparse(URS_URL).hostname\n",
-                "        )\n",
+                "        username, account, password = info.authenticators(urlparse(URS_URL).hostname)\n",
                 "        errprefix = \"netrc error: \"\n",
                 "    except Exception as e:\n",
                 "        if not (\"No such file\" in str(e)):\n",
                 "            print(\"netrc error: {0}\".format(str(e)))\n",
                 "        username = None\n",
                 "        password = None\n",
                 "\n",
                 "    while not credentials:\n",
                 "        if not username:\n",
                 "            username = get_username()\n",
                 "            password = get_password()\n",
                 "        credentials = \"{0}:{1}\".format(username, password)\n",
-                "        credentials = base64.b64encode(credentials.encode(\"ascii\")).decode(\n",
-                "            \"ascii\"\n",
-                "        )\n",
+                "        credentials = base64.b64encode(credentials.encode(\"ascii\")).decode(\"ascii\")\n",
                 "\n",
                 "        if url:\n",
                 "            try:\n",
                 "                req = Request(url)\n",
                 "                req.add_header(\"Authorization\", \"Basic {0}\".format(credentials))\n",
                 "                opener = build_opener(HTTPCookieProcessor())\n",
                 "                opener.open(req)\n",
@@ -201,28 +196,24 @@
                 "    params += \"&temporal[]={0},{1}\".format(time_start, time_end)\n",
                 "    if polygon:\n",
                 "        params += \"&polygon={0}\".format(polygon)\n",
                 "    elif bounding_box:\n",
                 "        params += \"&bounding_box={0}\".format(bounding_box)\n",
                 "    if filename_filter:\n",
                 "        option = \"&options[producer_granule_id][pattern]=true\"\n",
-                "        params += \"&producer_granule_id[]={0}{1}\".format(\n",
-                "            filename_filter, option\n",
-                "        )\n",
+                "        params += \"&producer_granule_id[]={0}{1}\".format(filename_filter, option)\n",
                 "    return CMR_FILE_URL + params\n",
                 "\n",
                 "\n",
                 "def cmr_filter_urls(search_results):\n",
                 "    \"\"\"Select only the desired data files from CMR response.\"\"\"\n",
                 "    if \"feed\" not in search_results or \"entry\" not in search_results[\"feed\"]:\n",
                 "        return []\n",
                 "\n",
-                "    entries = [\n",
-                "        e[\"links\"] for e in search_results[\"feed\"][\"entry\"] if \"links\" in e\n",
-                "    ]\n",
+                "    entries = [e[\"links\"] for e in search_results[\"feed\"][\"entry\"] if \"links\" in e]\n",
                 "    # Flatten \"entries\" to a simple list of links\n",
                 "    links = list(itertools.chain(*entries))\n",
                 "\n",
                 "    urls = []\n",
                 "    unique_filenames = set()\n",
                 "    for link in links:\n",
                 "        if \"href\" not in link:\n",
@@ -283,17 +274,15 @@
                 "        while True:\n",
                 "            req = Request(cmr_query_url)\n",
                 "            if cmr_scroll_id:\n",
                 "                req.add_header(\"cmr-scroll-id\", cmr_scroll_id)\n",
                 "            response = urlopen(req, context=ctx)\n",
                 "            if not cmr_scroll_id:\n",
                 "                # Python 2 and 3 have different case for the http headers\n",
-                "                headers = {\n",
-                "                    k.lower(): v for k, v in dict(response.info()).items()\n",
-                "                }\n",
+                "                headers = {k.lower(): v for k, v in dict(response.info()).items()}\n",
                 "                cmr_scroll_id = headers[\"cmr-scroll-id\"]\n",
                 "                hits = int(headers[\"cmr-hits\"])\n",
                 "                if hits > 0:\n",
                 "                    print(\"Found {0} matches.\".format(hits))\n",
                 "                else:\n",
                 "                    print(\"Found no matches.\")\n",
                 "            search_page = response.read()\n",
```

### Comparing `carbonplan-data-0.4.0/scripts/global-biomass/01_biomass_to_cogs.ipynb` & `carbonplan_data-0.4.3/scripts/global-biomass/01_biomass_to_cogs.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998798076923077%*

 * *Differences: {"'cells'": "{3: {'source': {delete: [8]}}}"}*

```diff
@@ -66,15 +66,14 @@
                 "    \"aboveground_biomass_carbon_2010\": \"aboveground\",\n",
                 "    \"aboveground_biomass_carbon_2010_uncertainty\": \"aboveground_uncertainty\",\n",
                 "    \"belowground_biomass_carbon_2010\": \"belowground\",\n",
                 "    \"belowground_biomass_carbon_2010_uncertainty\": \"belowground_uncertainty\",\n",
                 "}\n",
                 "\n",
                 "for skey, tkey in keys.items():\n",
-                "\n",
                 "    # raw file\n",
                 "    source = workdir / f\"Global_Maps_C_Density_2010_1763/data/{skey}.tif\"\n",
                 "\n",
                 "    # local target\n",
                 "    target = \"./raster.tif\"\n",
                 "\n",
                 "    # This is where we'll write the COGs when we're done\n",
```

### Comparing `carbonplan-data-0.4.0/scripts/gridmet/01_gridmet_to_zarr.ipynb` & `carbonplan_data-0.4.3/scripts/gridmet/01_gridmet_to_zarr.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9977430555555555%*

 * *Differences: {"'cells'": "{3: {'source': ['source_pattern = "*

 * *            '"https://www.northwestknowledge.net/metdata/data/{var}_{year}.nc"\']}, 4: '*

 * *            "{'metadata': {delete: ['collapsed']}, 'source': {insert: [(3, '    "*

 * *            'ds_list.append(xr.concat([source(variable=v, year=y).to_dask() for y in years], '*

 * *            'dim="day"))\')], delete: [7, 6, 5, 4, 3]}}}'}*

```diff
@@ -73,38 +73,31 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "source_pattern = (\n",
-                "    \"https://www.northwestknowledge.net/metdata/data/{var}_{year}.nc\"\n",
-                ")"
+                "source_pattern = \"https://www.northwestknowledge.net/metdata/data/{var}_{year}.nc\""
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
-                "collapsed": true,
                 "jupyter": {
                     "outputs_hidden": true
                 }
             },
             "outputs": [],
             "source": [
                 "ds_list = []\n",
                 "for v in variables:\n",
                 "    print(v)\n",
-                "    ds_list.append(\n",
-                "        xr.concat(\n",
-                "            [source(variable=v, year=y).to_dask() for y in years], dim=\"day\"\n",
-                "        )\n",
-                "    )"
+                "    ds_list.append(xr.concat([source(variable=v, year=y).to_dask() for y in years], dim=\"day\"))"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `carbonplan-data-0.4.0/scripts/grids/make_grid.ipynb` & `carbonplan_data-0.4.3/scripts/grids/make_grid.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.998112084379888%*

 * *Differences: {"'cells'": '{3: {\'source\': {insert: [(13, \'        lon, lat = transform(riods.crs, {"init": '*

 * *            '"EPSG:4326"}, tempx.flatten(), tempy.flatten())\\n\')], delete: [16, 15, 14, 1]}}, 8: '*

 * *            '{\'source\': {insert: [(1, \'grid["lon"] = xr.DataArray(lons["center"], name="lon", '*

 * *            'dims=("y", "x"), attrs=attrs["lon"])\\n\'), (2, \'grid["lat"] = '*

 * *            'xr.DataArray(lats["center"], name="lat", dims=("y", "x"), attrs=attrs["lat"])\\n\')], '*

 * *            'delete: [6, 5, 4, 3,  […]*

```diff
@@ -92,30 +92,27 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "def extract_grid_coords(tiff_url):\n",
-                "\n",
                 "    out_lon = {}\n",
                 "    out_lat = {}\n",
                 "\n",
                 "    for offset in [\"center\", \"ul\", \"ll\", \"ur\", \"lr\"]:\n",
                 "        tempx = np.empty(shape=riods.shape, dtype=float)\n",
                 "        tempy = np.empty(shape=riods.shape, dtype=float)\n",
                 "\n",
                 "        for (row, col), _ in np.ndenumerate(tempx):\n",
                 "            x, y = riods.xy(row, col, offset=offset)\n",
                 "            tempx[(row, col)] = x\n",
                 "            tempy[(row, col)] = y\n",
                 "\n",
-                "        lon, lat = transform(\n",
-                "            riods.crs, {\"init\": \"EPSG:4326\"}, tempx.flatten(), tempy.flatten()\n",
-                "        )\n",
+                "        lon, lat = transform(riods.crs, {\"init\": \"EPSG:4326\"}, tempx.flatten(), tempy.flatten())\n",
                 "\n",
                 "        out_lon[offset] = np.asarray(lon).reshape(riods.shape)\n",
                 "        out_lat[offset] = np.asarray(lat).reshape(riods.shape)\n",
                 "\n",
                 "    return out_lon, out_lat"
             ]
         },
@@ -224,20 +221,16 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "lons, lats = nlcd_coords\n",
-                "grid[\"lon\"] = xr.DataArray(\n",
-                "    lons[\"center\"], name=\"lon\", dims=(\"y\", \"x\"), attrs=attrs[\"lon\"]\n",
-                ")\n",
-                "grid[\"lat\"] = xr.DataArray(\n",
-                "    lats[\"center\"], name=\"lat\", dims=(\"y\", \"x\"), attrs=attrs[\"lat\"]\n",
-                ")\n",
+                "grid[\"lon\"] = xr.DataArray(lons[\"center\"], name=\"lon\", dims=(\"y\", \"x\"), attrs=attrs[\"lon\"])\n",
+                "grid[\"lat\"] = xr.DataArray(lats[\"center\"], name=\"lat\", dims=(\"y\", \"x\"), attrs=attrs[\"lat\"])\n",
                 "\n",
                 "grid"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -256,20 +249,16 @@
                 "\n",
                 "lat_b = np.full(shape, np.nan)\n",
                 "lat_b[:-1, :-1] = lats[\"ul\"]\n",
                 "lat_b[:-1, -1] = lats[\"ur\"][:, -1]\n",
                 "lat_b[-1, :-1] = lats[\"ll\"][-1, :]\n",
                 "lat_b[-1, -1] = lats[\"lr\"][-1, -1]\n",
                 "\n",
-                "grid[\"lon_b\"] = xr.DataArray(\n",
-                "    lon_b, name=\"lon_b\", dims=(\"y_b\", \"x_b\"), attrs=attrs[\"lon_b\"]\n",
-                ")\n",
-                "grid[\"lat_b\"] = xr.DataArray(\n",
-                "    lat_b, name=\"lat_b\", dims=(\"y_b\", \"x_b\"), attrs=attrs[\"lat_b\"]\n",
-                ")\n",
+                "grid[\"lon_b\"] = xr.DataArray(lon_b, name=\"lon_b\", dims=(\"y_b\", \"x_b\"), attrs=attrs[\"lon_b\"])\n",
+                "grid[\"lat_b\"] = xr.DataArray(lat_b, name=\"lat_b\", dims=(\"y_b\", \"x_b\"), attrs=attrs[\"lat_b\"])\n",
                 "\n",
                 "# uncomment to use (i, j, 4) notation\n",
                 "# grid['xv'] = xr.DataArray(np.stack([lons[k] for k in ['ul', 'ur', 'lr', 'll']], axis=2), name='xv', dims=('nj', 'ni', 'nv'), attrs=attrs['xv'])\n",
                 "# grid['yv'] = xr.DataArray(np.stack([lats[k] for k in ['ul', 'ur', 'lr', 'll']], axis=2), name='yv', dims=('nj', 'ni', 'nv'), attrs=attrs['yv'])\n",
                 "grid"
             ]
         },
@@ -277,15 +266,15 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "da = cat.nlcd.raster(region=region).read()\n",
                 "grid[\"mask\"] = xr.where(da.squeeze(drop=True), 1, 0).astype(np.int)\n",
-                "grid[\"area\"] = xr.zeros_like(grid[\"mask\"]) + (dxdy ** 2)\n",
+                "grid[\"area\"] = xr.zeros_like(grid[\"mask\"]) + (dxdy**2)\n",
                 "grid[\"x\"] = da.coords[\"x\"]\n",
                 "grid[\"y\"] = da.coords[\"y\"]\n",
                 "grid[\"crs\"] = xr.DataArray(1, name=\"crs\")\n",
                 "\n",
                 "for var in [\"mask\", \"area\", \"x\", \"y\", \"crs\"]:\n",
                 "    grid[var].attrs = attrs[var]\n",
                 "\n",
@@ -305,20 +294,16 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import gcsfs\n",
                 "\n",
-                "fs = gcsfs.GCSFileSystem(\n",
-                "    project=\"carbonplan\", token=\"cloud\", requester_pays=True\n",
-                ")\n",
-                "mapper = fs.get_mapper(\n",
-                "    f\"carbonplan-data/processed/grids/{region}/4000m/domain.zarr\"\n",
-                ")\n",
+                "fs = gcsfs.GCSFileSystem(project=\"carbonplan\", token=\"cloud\", requester_pays=True)\n",
+                "mapper = fs.get_mapper(f\"carbonplan-data/processed/grids/{region}/4000m/domain.zarr\")\n",
                 "grid.to_zarr(mapper, mode=\"w\", consolidated=True)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
```

### Comparing `carbonplan-data-0.4.0/scripts/iiasa/01_raw_to_parquet.ipynb` & `carbonplan_data-0.4.3/scripts/iiasa/01_raw_to_parquet.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9978806907378336%*

 * *Differences: {"'cells'": '{2: {\'source\': {insert: [(9, \'    df.to_parquet(blob, compression="gzip", '*

 * *            'open_with=fs.open, engine="fastparquet")\')], delete: [11, 10, 9]}}, 3: {\'source\': '*

 * *            '{insert: [(9, \'    df.to_parquet(blob, compression="gzip", open_with=fs.open, '*

 * *            'engine="fastparquet")\')], delete: [11, 10, 9]}}, 5: {\'source\': {insert: [(1, '*

 * *            "'blob = "*

 * *            '"carbonplan-data-restricted/raw/iiasa/SspDb_country_data_2013-06-12.parquet"\\n\')], '*

 * *         […]*

```diff
@@ -58,17 +58,15 @@
                 "csvs = source_dir.glob(\"*csv\")\n",
                 "\n",
                 "for csv in csvs:\n",
                 "    blob = f\"{blob_prefix}/{csv.stem.lower()}.parquet\"\n",
                 "    print(blob)\n",
                 "\n",
                 "    df = pd.read_csv(csv)\n",
-                "    df.to_parquet(\n",
-                "        blob, compression=\"gzip\", open_with=fs.open, engine=\"fastparquet\"\n",
-                "    )"
+                "    df.to_parquet(blob, compression=\"gzip\", open_with=fs.open, engine=\"fastparquet\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -78,17 +76,15 @@
                 "csvs = source_dir.glob(\"*csv\")\n",
                 "\n",
                 "for csv in csvs:\n",
                 "    blob = f\"{blob_prefix}/{csv.stem.lower()}.parquet\"\n",
                 "    print(blob)\n",
                 "\n",
                 "    df = pd.read_csv(csv)\n",
-                "    df.to_parquet(\n",
-                "        blob, compression=\"gzip\", open_with=fs.open, engine=\"fastparquet\"\n",
-                "    )"
+                "    df.to_parquet(blob, compression=\"gzip\", open_with=fs.open, engine=\"fastparquet\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -102,17 +98,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "source = \"../../carbonplan_data/iiasa/SspDb_country_data_2013-06-12.csv\"\n",
-                "blob = (\n",
-                "    \"carbonplan-data-restricted/raw/iiasa/SspDb_country_data_2013-06-12.parquet\"\n",
-                ")\n",
+                "blob = \"carbonplan-data-restricted/raw/iiasa/SspDb_country_data_2013-06-12.parquet\"\n",
                 "df = pd.read_csv(source)\n",
                 "df.to_parquet(blob, compression=\"gzip\", open_with=fs.open, engine=\"fastparquet\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
```

### Comparing `carbonplan-data-0.4.0/scripts/mtbs/01_raw_to_cogs.ipynb` & `carbonplan_data-0.4.3/scripts/mtbs/01_raw_to_cogs.ipynb`

 * *Files identical despite different names*

### Comparing `carbonplan-data-0.4.0/scripts/mtbs/02_downsampling_and_reprojection.ipynb` & `carbonplan_data-0.4.3/scripts/mtbs/02_downsampling_and_reprojection.ipynb`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9993686868686869%*

 * *Differences: {"'cells'": '{5: {\'source\': {insert: [(11, \'            cmd = ("gdalwarp " "-t_srs \\\'%s\\\' " '*

 * *            '"-te %s " "-tr %s %s " "-r %s " "%s " "%s") % (\\n\')], delete: [19, 18, 17, 16, 15, '*

 * *            '14, 13, 12, 11]}}}'}*

```diff
@@ -99,23 +99,15 @@
                 "        for f in files:\n",
                 "            if \"error\" in str(f[\"source\"]):\n",
                 "                resampling = \"average\"\n",
                 "            elif resolution == 4000:\n",
                 "                resampling = \"mode\"\n",
                 "            else:\n",
                 "                resampling = \"near\"\n",
-                "            cmd = (\n",
-                "                \"gdalwarp \"\n",
-                "                \"-t_srs '%s' \"\n",
-                "                \"-te %s \"\n",
-                "                \"-tr %s %s \"\n",
-                "                \"-r %s \"\n",
-                "                \"%s \"\n",
-                "                \"%s\"\n",
-                "            ) % (\n",
+                "            cmd = (\"gdalwarp \" \"-t_srs '%s' \" \"-te %s \" \"-tr %s %s \" \"-r %s \" \"%s \" \"%s\") % (\n",
                 "                crs,\n",
                 "                extent,\n",
                 "                resolution,\n",
                 "                resolution,\n",
                 "                resampling,\n",
                 "                f[\"source\"],\n",
                 "                \"./raster.tif\",\n",
```

### Comparing `carbonplan-data-0.4.0/scripts/mtbs/02_mtbs_to_zarr.ipynb` & `carbonplan_data-0.4.3/scripts/mtbs/02_mtbs_to_zarr.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9992933723196882%*

 * *Differences: {"'cells'": "{3: {'source': {insert: [(48, '        dst_band, dst_transform, dst_crs, dst_shape = "*

 * *            "make_dst_band(src_band, src_resolution)\\n'), (62, '            dst_band = "*

 * *            'dst_band.astype("float32")  # convert to float for averaging\\n\'), (90, \'    ds = '*

 * *            'xr.DataArray(dst_band, dims=("y", "x"), attrs=meta).to_dataset(name=varname)\\n\'), '*

 * *            '(96, \'        fs = gcsfs.GCSFileSystem(project="carbonplan", token="cloud", '*

 * *            'requester_pays=True […]*

```diff
@@ -130,33 +130,29 @@
                 "    src_path = f\"gs://carbonplan-data/raw/MTBS/30m/{year}.tif\"\n",
                 "    with rasterio.open(src_path, \"r\") as src_raster:\n",
                 "        src_transform = src_raster.meta[\"transform\"]\n",
                 "        src_crs = src_raster.meta[\"crs\"]\n",
                 "        src_band = src_raster.read(1)\n",
                 "        src_resolution = resolution\n",
                 "\n",
-                "        dst_band, dst_transform, dst_crs, dst_shape = make_dst_band(\n",
-                "            src_band, src_resolution\n",
-                "        )\n",
+                "        dst_band, dst_transform, dst_crs, dst_shape = make_dst_band(src_band, src_resolution)\n",
                 "        print(\"calc_coords\")\n",
                 "        coords = calc_coords(dst_shape, dst_transform, dst_crs)\n",
                 "\n",
                 "        src_nodata = 6\n",
                 "        if resolution == 30:\n",
                 "            resampling = Resampling.nearest\n",
                 "        elif resolution > 30:\n",
                 "            resampling = Resampling.average\n",
                 "            # set moderate or high burn severity to 1 and others to 1\n",
                 "            src_band_tmp = ((src_band == 3) | (src_band == 4)).astype(\"uint8\")\n",
                 "            # set masked regions to nodata value\n",
                 "            src_band_tmp[src_band == src_nodata] = src_nodata\n",
                 "            src_band = src_band_tmp\n",
-                "            dst_band = dst_band.astype(\n",
-                "                \"float32\"\n",
-                "            )  # convert to float for averaging\n",
+                "            dst_band = dst_band.astype(\"float32\")  # convert to float for averaging\n",
                 "\n",
                 "        print(\"reproject\")\n",
                 "        # this seems to require rasterio=1.0.25 and gdal=2.4.2\n",
                 "        reproject(\n",
                 "            src_band,\n",
                 "            dst_band,\n",
                 "            src_transform=src_transform,\n",
@@ -176,29 +172,23 @@
                 "            crs=dst_crs.to_wkt(),\n",
                 "            transform=list(dst_transform),\n",
                 "            nodata=src_raster.meta[\"nodata\"],\n",
                 "        )\n",
                 "\n",
                 "    varname = f\"{year}\"\n",
                 "    chunks = {\"x\": 512, \"y\": 512}\n",
-                "    ds = xr.DataArray(dst_band, dims=(\"y\", \"x\"), attrs=meta).to_dataset(\n",
-                "        name=varname\n",
-                "    )\n",
+                "    ds = xr.DataArray(dst_band, dims=(\"y\", \"x\"), attrs=meta).to_dataset(name=varname)\n",
                 "    ds = ds.assign_coords(coords).chunk(chunks)\n",
                 "\n",
                 "    if return_ds:\n",
                 "        return ds\n",
                 "    else:\n",
-                "        fs = gcsfs.GCSFileSystem(\n",
-                "            project=\"carbonplan\", token=\"cloud\", requester_pays=True\n",
-                "        )\n",
+                "        fs = gcsfs.GCSFileSystem(project=\"carbonplan\", token=\"cloud\", requester_pays=True)\n",
                 "        mapper = fs.get_mapper(scratch + f\"/MTBS.{year}.{resolution}m.zarr\")\n",
-                "        ds.to_zarr(\n",
-                "            store=mapper, mode=\"w\", encoding={varname: {\"compressor\": Zlib()}}\n",
-                "        )"
+                "        ds.to_zarr(store=mapper, mode=\"w\", encoding={varname: {\"compressor\": Zlib()}})"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -224,17 +214,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "fs = gcsfs.GCSFileSystem(\n",
-                "    project=\"carbonplan\", token=\"cloud\", requester_pays=True\n",
-                ")\n",
+                "fs = gcsfs.GCSFileSystem(project=\"carbonplan\", token=\"cloud\", requester_pays=True)\n",
                 "mapper = fs.get_mapper(\"carbonplan-data/processed/MTBS/raster.zarr\")\n",
                 "\n",
                 "ds.to_zarr(\n",
                 "    store=mapper,\n",
                 "    group=\"4000m\",\n",
                 "    mode=\"w\",\n",
                 "    encoding={varname: {\"compressor\": Zlib()}},\n",
```

### Comparing `carbonplan-data-0.4.0/scripts/mtbs/03_mtbs_to_zarr.ipynb` & `carbonplan_data-0.4.3/scripts/mtbs/03_mtbs_to_zarr.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9992933723196882%*

 * *Differences: {"'cells'": "{3: {'source': {insert: [(48, '        dst_band, dst_transform, dst_crs, dst_shape = "*

 * *            "make_dst_band(src_band, src_resolution)\\n'), (62, '            dst_band = "*

 * *            'dst_band.astype("float32")  # convert to float for averaging\\n\'), (90, \'    ds = '*

 * *            'xr.DataArray(dst_band, dims=("y", "x"), attrs=meta).to_dataset(name=varname)\\n\'), '*

 * *            '(96, \'        fs = gcsfs.GCSFileSystem(project="carbonplan", token="cloud", '*

 * *            'requester_pays=True […]*

```diff
@@ -130,33 +130,29 @@
                 "    src_path = f\"gs://carbonplan-data/raw/MTBS/30m/{year}.tif\"\n",
                 "    with rasterio.open(src_path, \"r\") as src_raster:\n",
                 "        src_transform = src_raster.meta[\"transform\"]\n",
                 "        src_crs = src_raster.meta[\"crs\"]\n",
                 "        src_band = src_raster.read(1)\n",
                 "        src_resolution = resolution\n",
                 "\n",
-                "        dst_band, dst_transform, dst_crs, dst_shape = make_dst_band(\n",
-                "            src_band, src_resolution\n",
-                "        )\n",
+                "        dst_band, dst_transform, dst_crs, dst_shape = make_dst_band(src_band, src_resolution)\n",
                 "        print(\"calc_coords\")\n",
                 "        coords = calc_coords(dst_shape, dst_transform, dst_crs)\n",
                 "\n",
                 "        src_nodata = 6\n",
                 "        if resolution == 30:\n",
                 "            resampling = Resampling.nearest\n",
                 "        elif resolution > 30:\n",
                 "            resampling = Resampling.average\n",
                 "            # set moderate or high burn severity to 1 and others to 1\n",
                 "            src_band_tmp = ((src_band == 3) | (src_band == 4)).astype(\"uint8\")\n",
                 "            # set masked regions to nodata value\n",
                 "            src_band_tmp[src_band == src_nodata] = src_nodata\n",
                 "            src_band = src_band_tmp\n",
-                "            dst_band = dst_band.astype(\n",
-                "                \"float32\"\n",
-                "            )  # convert to float for averaging\n",
+                "            dst_band = dst_band.astype(\"float32\")  # convert to float for averaging\n",
                 "\n",
                 "        print(\"reproject\")\n",
                 "        # this seems to require rasterio=1.0.25 and gdal=2.4.2\n",
                 "        reproject(\n",
                 "            src_band,\n",
                 "            dst_band,\n",
                 "            src_transform=src_transform,\n",
@@ -176,29 +172,23 @@
                 "            crs=dst_crs.to_wkt(),\n",
                 "            transform=list(dst_transform),\n",
                 "            nodata=src_raster.meta[\"nodata\"],\n",
                 "        )\n",
                 "\n",
                 "    varname = f\"{year}\"\n",
                 "    chunks = {\"x\": 512, \"y\": 512}\n",
-                "    ds = xr.DataArray(dst_band, dims=(\"y\", \"x\"), attrs=meta).to_dataset(\n",
-                "        name=varname\n",
-                "    )\n",
+                "    ds = xr.DataArray(dst_band, dims=(\"y\", \"x\"), attrs=meta).to_dataset(name=varname)\n",
                 "    ds = ds.assign_coords(coords).chunk(chunks)\n",
                 "\n",
                 "    if return_ds:\n",
                 "        return ds\n",
                 "    else:\n",
-                "        fs = gcsfs.GCSFileSystem(\n",
-                "            project=\"carbonplan\", token=\"cloud\", requester_pays=True\n",
-                "        )\n",
+                "        fs = gcsfs.GCSFileSystem(project=\"carbonplan\", token=\"cloud\", requester_pays=True)\n",
                 "        mapper = fs.get_mapper(scratch + f\"/MTBS.{year}.{resolution}m.zarr\")\n",
-                "        ds.to_zarr(\n",
-                "            store=mapper, mode=\"w\", encoding={varname: {\"compressor\": Zlib()}}\n",
-                "        )"
+                "        ds.to_zarr(store=mapper, mode=\"w\", encoding={varname: {\"compressor\": Zlib()}})"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -224,17 +214,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "fs = gcsfs.GCSFileSystem(\n",
-                "    project=\"carbonplan\", token=\"cloud\", requester_pays=True\n",
-                ")\n",
+                "fs = gcsfs.GCSFileSystem(project=\"carbonplan\", token=\"cloud\", requester_pays=True)\n",
                 "mapper = fs.get_mapper(\"carbonplan-data/processed/MTBS/raster.zarr\")\n",
                 "\n",
                 "ds.to_zarr(\n",
                 "    store=mapper,\n",
                 "    group=\"4000m\",\n",
                 "    mode=\"w\",\n",
                 "    encoding={varname: {\"compressor\": Zlib()}},\n",
```

### Comparing `carbonplan-data-0.4.0/scripts/mtbs/04_mtbs_perims_to_raster.ipynb` & `carbonplan_data-0.4.3/scripts/mtbs/04_mtbs_perims_to_raster.ipynb`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9992609550942884%*

 * *Differences: {"'cells'": "{3: {'source': {insert: [(10, 'perims = "*

 * *            'geopandas.GeoDataFrame.from_file("mtbs_perimeter_data/mtbs_perims_DD/mtbs_perims_DD.shp")\')], '*

 * *            "delete: [12, 11, 10]}}, 6: {'source': {delete: [1]}}, 9: {'source': {delete: [4]}}, "*

 * *            "12: {'source': {insert: [(4, '        out_fname = (\\n'), (5, '            "*

 * *            'f"carbonplan-data/processed/mtbs/{region}/30m/{name}_{month.strftime(\\\'%Y.%m\\\')}.tif"\\n\'), '*

 * *            "(6, '        )\\n')], delete: [6, […]*

```diff
@@ -83,17 +83,15 @@
                 "\n",
                 "mask = rasterio.open(cat.mtbs.raw_raster._urlpath)\n",
                 "transform = mask.transform\n",
                 "shape = mask.shape\n",
                 "src_profile = mask.profile\n",
                 "\n",
                 "# TODO: replace with intake use\n",
-                "perims = geopandas.GeoDataFrame.from_file(\n",
-                "    \"mtbs_perimeter_data/mtbs_perims_DD/mtbs_perims_DD.shp\"\n",
-                ")"
+                "perims = geopandas.GeoDataFrame.from_file(\"mtbs_perimeter_data/mtbs_perims_DD/mtbs_perims_DD.shp\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -127,15 +125,14 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "def rasterize_geom(geoms):\n",
-                "\n",
                 "    r = rasterize(\n",
                 "        [(geom, 1) for geom in geoms],\n",
                 "        out_shape=shape,\n",
                 "        transform=transform,\n",
                 "        fill=0,\n",
                 "        merge_alg=rasterio.enums.MergeAlg.replace,\n",
                 "        all_touched=True,\n",
@@ -172,15 +169,14 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "from gcsfs import GCSFileSystem\n",
                 "\n",
                 "\n",
                 "def copy_to_fs(source, dst, fs):\n",
-                "\n",
                 "    with open(source, \"rb\") as fsource:\n",
                 "        with fs.open(dst, \"wb\") as fdst:\n",
                 "            fdst.write(fsource.read())\n",
                 "\n",
                 "\n",
                 "def numpy_to_cog(data, out_fname=\"temp_cog.tif\"):\n",
                 "    with MemoryFile() as memfile:\n",
@@ -228,18 +224,18 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "dst_profile = cog_profiles.get(\"deflate\")\n",
                 "\n",
                 "for month in months:\n",
-                "\n",
                 "    for name, df in [(\"lf\", perims_lf), (\"vlf\", perims_vlf)]:\n",
-                "\n",
-                "        out_fname = f\"carbonplan-data/processed/mtbs/{region}/30m/{name}_{month.strftime('%Y.%m')}.tif\"\n",
+                "        out_fname = (\n",
+                "            f\"carbonplan-data/processed/mtbs/{region}/30m/{name}_{month.strftime('%Y.%m')}.tif\"\n",
+                "        )\n",
                 "\n",
                 "        if fs.exists(out_fname):\n",
                 "            print(f\"{out_fname} exists, skipping...\")\n",
                 "            continue\n",
                 "\n",
                 "        try:\n",
                 "            geom = df.loc[[month]].geometry\n",
@@ -265,18 +261,15 @@
                 "from dask.diagnostics import ProgressBar\n",
                 "\n",
                 "cat2 = intake.open_catalog(\n",
                 "    \"https://raw.githubusercontent.com/carbonplan/data/master/carbonplan_data/catalogs/mtbs.yaml\"\n",
                 ")\n",
                 "dates = [f\"2018.{m:02d}\" for m in range(1, 13)]\n",
                 "da = xr.concat(\n",
-                "    [\n",
-                "        cat2.rasterized_perims(size=\"vlf\", date=d).to_dask().squeeze(drop=True)\n",
-                "        for d in dates\n",
-                "    ],\n",
+                "    [cat2.rasterized_perims(size=\"vlf\", date=d).to_dask().squeeze(drop=True) for d in dates],\n",
                 "    dim=xr.Variable(\"time\", dates),\n",
                 ")\n",
                 "\n",
                 "with ProgressBar():\n",
                 "    da_sum = da.sum(\"time\").coarsen(x=133, y=133, boundary=\"trim\").mean().load()\n",
                 "da_sum"
             ]
```

### Comparing `carbonplan-data-0.4.0/scripts/mtbs/05_monthly_downsampling.ipynb` & `carbonplan_data-0.4.3/scripts/mtbs/05_monthly_downsampling.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9988390368094668%*

 * *Differences: {"'cells'": "{4: {'source': {insert: [(3, '            workdir / "*

 * *            'f"processed/mtbs/{region}/30m/{fire}_{year}.{month:02g}.tif"\\n\')], delete: [4, '*

 * *            '3]}}, 5: {\'source\': {insert: [(9, \'                cmd = ("gdalwarp " "-t_srs '*

 * *            '\\\'%s\\\' " "-te %s " "-tr %s %s " "-r %s " "%s " "%s") % (\\n\')], delete: [17, 16, '*

 * *            "15, 14, 13, 12, 11, 10, 9]}}, 7: {'source': {insert: [(5, '            files = "*

 * *            '[get_file("conus", "vlf", year, month + 1)["s […]*

```diff
@@ -64,16 +64,15 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "def get_file(region, fire, year, month):\n",
                 "    return {\n",
                 "        \"source\": (\n",
-                "            workdir\n",
-                "            / f\"processed/mtbs/{region}/30m/{fire}_{year}.{month:02g}.tif\"\n",
+                "            workdir / f\"processed/mtbs/{region}/30m/{fire}_{year}.{month:02g}.tif\"\n",
                 "        ).as_posix(),\n",
                 "        \"target\": f\"processed/mtbs/{region}/4000m/tif/{fire}.{month:02g}.tif\",\n",
                 "    }"
             ]
         },
         {
             "cell_type": "code",
@@ -86,23 +85,15 @@
                 "for year in [1984]:\n",
                 "    for month in [1]:\n",
                 "        for fire in [\"vlf\"]:\n",
                 "            for region in [\"ak\", \"conus\"]:\n",
                 "                f = get_file(region, fire, year, month)\n",
                 "                crs, extent = projections(\"albers\", region)\n",
                 "                resampling = \"average\"\n",
-                "                cmd = (\n",
-                "                    \"gdalwarp \"\n",
-                "                    \"-t_srs '%s' \"\n",
-                "                    \"-te %s \"\n",
-                "                    \"-tr %s %s \"\n",
-                "                    \"-r %s \"\n",
-                "                    \"%s \"\n",
-                "                    \"%s\"\n",
-                "                ) % (\n",
+                "                cmd = (\"gdalwarp \" \"-t_srs '%s' \" \"-te %s \" \"-tr %s %s \" \"-r %s \" \"%s \" \"%s\") % (\n",
                 "                    crs,\n",
                 "                    extent,\n",
                 "                    resolution,\n",
                 "                    resolution,\n",
                 "                    resampling,\n",
                 "                    f[\"source\"],\n",
                 "                    \"./raster.tif\",\n",
@@ -128,31 +119,19 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "resolution = 4000\n",
                 "\n",
                 "for year in [2017]:\n",
                 "    for region in [\"conus\"]:\n",
-                "\n",
                 "        for fire in [\"vlf\"]:\n",
-                "            files = [\n",
-                "                get_file(\"conus\", \"vlf\", year, month + 1)[\"source\"]\n",
-                "                for month in range(12)\n",
-                "            ]\n",
+                "            files = [get_file(\"conus\", \"vlf\", year, month + 1)[\"source\"] for month in range(12)]\n",
                 "            crs, extent = projections(\"albers\", region)\n",
                 "            resampling = \"sum\"\n",
-                "            cmd = (\n",
-                "                \"gdalwarp \"\n",
-                "                \"-t_srs '%s' \"\n",
-                "                \"-te %s \"\n",
-                "                \"-tr %s %s \"\n",
-                "                \"-r %s \"\n",
-                "                \"%s \"\n",
-                "                \"%s\"\n",
-                "            ) % (\n",
+                "            cmd = (\"gdalwarp \" \"-t_srs '%s' \" \"-te %s \" \"-tr %s %s \" \"-r %s \" \"%s \" \"%s\") % (\n",
                 "                crs,\n",
                 "                extent,\n",
                 "                resolution,\n",
                 "                resolution,\n",
                 "                resampling,\n",
                 "                \" \".join(files),\n",
                 "                \"./raster.tif\",\n",
@@ -168,17 +147,15 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import rasterio\n",
                 "\n",
-                "r = rasterio.open(\n",
-                "    \"/Users/freeman/workdir/carbonplan-data/processed/mtbs/conus/30m/vlf_2018.09.tif\"\n",
-                ")\n",
+                "r = rasterio.open(\"/Users/freeman/workdir/carbonplan-data/processed/mtbs/conus/30m/vlf_2018.09.tif\")\n",
                 "im = r.read(1)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
```

### Comparing `carbonplan-data-0.4.0/scripts/mtbs/05_monthly_mtbs_to_zarr.ipynb` & `carbonplan_data-0.4.3/scripts/mtbs/05_monthly_mtbs_to_zarr.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995370370370371%*

 * *Differences: {"'cells'": '{6: {\'source\': {insert: [(0, \'fs = gcsfs.GCSFileSystem(project="carbonplan", '*

 * *            'token="cloud", requester_pays=True)\\n\')], delete: [2, 1, 0]}}}'}*

```diff
@@ -222,17 +222,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "fs = gcsfs.GCSFileSystem(\n",
-                "    project=\"carbonplan\", token=\"cloud\", requester_pays=True\n",
-                ")\n",
+                "fs = gcsfs.GCSFileSystem(project=\"carbonplan\", token=\"cloud\", requester_pays=True)\n",
                 "mapper = fs.get_mapper(\"carbonplan-data/processed/MTBS/raster.zarr\")\n",
                 "\n",
                 "ds.to_zarr(\n",
                 "    store=mapper,\n",
                 "    group=\"4000m\",\n",
                 "    mode=\"w\",\n",
                 "    encoding={varname: {\"compressor\": Zlib()}},\n",
```

### Comparing `carbonplan-data-0.4.0/scripts/mtbs/05_monthly_mtbs_to_zarr.py` & `carbonplan_data-0.4.3/scripts/mtbs/05_monthly_mtbs_to_zarr.py`

 * *Files identical despite different names*

### Comparing `carbonplan-data-0.4.0/scripts/mtbs/06_annual_downsampling.py` & `carbonplan_data-0.4.3/scripts/mtbs/06_annual_downsampling.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 for region in ["conus"]:
     for year in np.arange(1984, 2019):
         source = (workdir / f"raw/mtbs/{region}/30m/{year}.tif").as_posix()
         print(source)
         crs, extent = projections("albers", region)
         resampling = "nearest"
-        cmd = ("gdalwarp " "-t_srs '%s' " "-te %s " "-tr %s %s " "-r %s " "%s " "%s") % (
+        cmd = ("gdalwarp " "-t_srs '{}' " "-te {} " "-tr {} {} " "-r {} " "{} " "{}").format(
             crs,
             extent,
             resolution,
             resolution,
             resampling,
             source,
             "./raster.tif",
```

### Comparing `carbonplan-data-0.4.0/scripts/mtbs/06_annual_mtbs_to_zarr.py` & `carbonplan_data-0.4.3/scripts/mtbs/06_annual_mtbs_to_zarr.py`

 * *Files identical despite different names*

### Comparing `carbonplan-data-0.4.0/scripts/mtbs/prepare.py` & `carbonplan_data-0.4.3/scripts/mtbs/prepare.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     ]
 
     dst_band = zeros(dst_shape, src_band.dtype)
     return dst_band, dst_transform, dst_crs, dst_shape
 
 
 def prepare_mtbs(year, resolution):
-    src_path = RAW_PATH + "MTBS/%s/mtbs_CONUS_%s.tif" % (year, year)
+    src_path = RAW_PATH + f"MTBS/{year}/mtbs_CONUS_{year}.tif"
     src_raster = rasterio.open(src_path)
     src_transform = src_raster.meta["transform"]
     src_crs = src_raster.meta["crs"]
     src_band = src_raster.read(1)
     src_resolution = resolution
 
     dst_band, dst_transform, dst_crs, dst_shape = make_dst_band(src_band, src_resolution)
@@ -92,14 +92,14 @@
         height=dst_shape[1],
         dtype=str(dst_band.dtype),
         crs=dst_crs.to_wkt(),
         transform=list(dst_transform),
         nodata=src_raster.meta["nodata"],
     )
 
-    store = zarr.open(PROCESSED_PATH + "MTBS.%s.%sm.zarr" % (year, resolution), "w")
+    store = zarr.open(PROCESSED_PATH + f"MTBS.{year}.{resolution}m.zarr", "w")
     store.attrs.put(meta)
     store.array("0", dst_band, chunks=(512, 512), compressor=Zlib())
 
 
 years = ["%s" % (d + 1984) for d in range(2018 - 1984)]
 [prepare_mtbs(year, 500) for year in years]
```

### Comparing `carbonplan-data-0.4.0/scripts/nftd/00_download.ipynb` & `carbonplan_data-0.4.3/scripts/nftd/00_download.ipynb`

 * *Files identical despite different names*

### Comparing `carbonplan-data-0.4.0/scripts/nftd/01_nftd_to_cogs.ipynb` & `carbonplan_data-0.4.3/scripts/nftd/01_nftd_to_cogs.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9991732804232805%*

 * *Differences: {"'cells'": '{3: {\'source\': {insert: [(1, \'os.environ["GOOGLE_APPLICATION_CREDENTIALS"] = '*

 * *            "(\\n'), (2, '    "*

 * *            '"/Users/freeman/.config/gcloud/legacy_credentials/jeremy@carbonplan.org/adc.json"\\n\'), '*

 * *            "(3, ')\\n')], delete: [3, 2, 1]}}, 6: {'source': {insert: [(27, '        "*

 * *            '"source": workdir / "ak_forestgroup" / '*

 * *            '"alaska_forestgroup_confidence_63360.img",\\n\'), (37, \'        "source": workdir / '*

 * *            '"ak_forest-type" / "alaska […]*

```diff
@@ -55,17 +55,17 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "dst_profile = cog_profiles.get(\"deflate\")\n",
-                "os.environ[\n",
-                "    \"GOOGLE_APPLICATION_CREDENTIALS\"\n",
-                "] = \"/Users/freeman/.config/gcloud/legacy_credentials/jeremy@carbonplan.org/adc.json\"\n",
+                "os.environ[\"GOOGLE_APPLICATION_CREDENTIALS\"] = (\n",
+                "    \"/Users/freeman/.config/gcloud/legacy_credentials/jeremy@carbonplan.org/adc.json\"\n",
+                ")\n",
                 "\n",
                 "\n",
                 "def upload(src, target, bucket=\"carbonplan-data\"):\n",
                 "    storage_client = storage.Client(\"carbonplan\")\n",
                 "    bucket = storage_client.bucket(bucket)\n",
                 "    blob = bucket.blob(target)\n",
                 "    blob.upload_from_filename(src)"
@@ -120,29 +120,25 @@
                 "    },\n",
                 "    {\n",
                 "        \"source\": workdir / \"ak_forestgroup\" / \"alaska_forestgroup_63360.img\",\n",
                 "        \"target\": workdir / \"ak_forestgroup\" / \"raster.tif\",\n",
                 "        \"cloud\": \"raw/nftd/ak_forestgroup/250m/raster.tif\",\n",
                 "    },\n",
                 "    {\n",
-                "        \"source\": workdir\n",
-                "        / \"ak_forestgroup\"\n",
-                "        / \"alaska_forestgroup_confidence_63360.img\",\n",
+                "        \"source\": workdir / \"ak_forestgroup\" / \"alaska_forestgroup_confidence_63360.img\",\n",
                 "        \"target\": workdir / \"ak_forestgroup\" / \"error.tif\",\n",
                 "        \"cloud\": \"raw/nftd/ak_forestgroup/250m/error.tif\",\n",
                 "    },\n",
                 "    {\n",
                 "        \"source\": workdir / \"ak_forest-type\" / \"alaska_foresttype_63360.img\",\n",
                 "        \"target\": workdir / \"ak_forest-type\" / \"raster.tif\",\n",
                 "        \"cloud\": \"raw/nftd/ak_foresttype/250m/raster.tif\",\n",
                 "    },\n",
                 "    {\n",
-                "        \"source\": workdir\n",
-                "        / \"ak_forest-type\"\n",
-                "        / \"alaska_foresttype_confidence_63360.img\",\n",
+                "        \"source\": workdir / \"ak_forest-type\" / \"alaska_foresttype_confidence_63360.img\",\n",
                 "        \"target\": workdir / \"ak_forest-type\" / \"error.tif\",\n",
                 "        \"cloud\": \"raw/nftd/ak_foresttype/250m/error.tif\",\n",
                 "    },\n",
                 "]"
             ]
         },
         {
```

### Comparing `carbonplan-data-0.4.0/scripts/nftd/02_downsampling_and_reprojection.ipynb` & `carbonplan_data-0.4.3/scripts/nlcd/02_downsampling_and_reprojection.ipynb`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9463920578332343%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(2, '# NLCD downsampling and reprojection\\n'), (6, 'This "*

 * *            "notebook downsamples and reprojects NLCD 30m rasters stored in Cloud\\n'), (7, "*

 * *            "'Optimized GeoTIFF into 30m, 250m, and 4000m GeoTIFFs.\\n'), (11, '- COG outputs from "*

 * *            "`01_nlcd_to_cogs.ipynb`\\n')], delete: [11, 7, 6, 2]}}, 3: {'source': {delete: [2]}}, "*

 * *            "6: {'source': ['def loadrio(f):\\n', '    src = rasterio.open(f)\\n', '    return "*

 * *            "src.read […]*

```diff
@@ -2,24 +2,24 @@
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "<img width=\"50\" src=\"https://carbonplan-assets.s3.amazonaws.com/monogram/dark-small.png\" style=\"margin-left:0px;margin-top:20px\"/>\n",
                 "\n",
-                "# NFTD downsampling and reprojection\n",
+                "# NLCD downsampling and reprojection\n",
                 "\n",
                 "_by Jeremy Freeman (CarbonPlan), August 2, 2020_\n",
                 "\n",
-                "This notebook downsamples and reprojects NFTD 250m yearly rasters stored in\n",
-                "Cloud Optimized GeoTIFF into 250m and 4000m GeoTIFFs.\n",
+                "This notebook downsamples and reprojects NLCD 30m rasters stored in Cloud\n",
+                "Optimized GeoTIFF into 30m, 250m, and 4000m GeoTIFFs.\n",
                 "\n",
                 "**Inputs:**\n",
                 "\n",
-                "- COG outputs from `01_nftd_to_cogs.ipynb`\n",
+                "- COG outputs from `01_nlcd_to_cogs.ipynb`\n",
                 "\n",
                 "**Outputs:**\n",
                 "\n",
                 "- COG outputs after downsampling and reprojection\n",
                 "\n",
                 "**Notes:**\n",
                 "\n",
@@ -50,73 +50,83 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from rio_cogeo.cogeo import cog_translate\n",
                 "from rio_cogeo.profiles import cog_profiles\n",
-                "import rasterio\n",
                 "\n",
                 "dst_profile = cog_profiles.get(\"deflate\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "def get_files(region, resolution):\n",
-                "    return [\n",
-                "        {\n",
-                "            \"source\": workdir / f\"raw/nftd/{region}_foresttype/250m/raster.tif\",\n",
-                "            \"target\": f\"processed/nftd/{region}/{resolution}m/type.tif\",\n",
-                "        },\n",
-                "        {\n",
-                "            \"source\": workdir\n",
-                "            / f\"raw/nftd/{region}_forestgroup/250m/raster.tif\",\n",
-                "            \"target\": f\"processed/nftd/{region}/{resolution}m/group.tif\",\n",
-                "        },\n",
-                "        {\n",
-                "            \"source\": workdir / f\"raw/nftd/{region}_foresttype/250m/error.tif\",\n",
-                "            \"target\": f\"processed/nftd/{region}/{resolution}m/type_error.tif\",\n",
-                "        },\n",
-                "        {\n",
-                "            \"source\": workdir / f\"raw/nftd/{region}_forestgroup/250m/error.tif\",\n",
-                "            \"target\": f\"processed/nftd/{region}/{resolution}m/group_error.tif\",\n",
-                "        },\n",
-                "    ]"
+                "import rasterio\n",
+                "from numpy import asarray, argmax"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "def get_file(region, year, resolution, c=None):\n",
+                "    if c is not None:\n",
+                "        target = f\"processed/nlcd/{region}/{resolution}m/{year}_c{c}.tif\"\n",
+                "    else:\n",
+                "        target = f\"processed/nlcd/{region}/{resolution}m/{year}.tif\"\n",
+                "    return {\n",
+                "        \"source\": workdir / f\"nlcd/{region}/30m/{year}.tif\",\n",
+                "        \"target\": target,\n",
+                "    }"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "def loadrio(f):\n",
+                "    src = rasterio.open(f)\n",
+                "    return src.read(1)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "### downsample using mode\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "for resolution in [250, 4000]:\n",
+                "for resolution in [4000]:\n",
                 "    for region in [\"ak\", \"conus\"]:\n",
-                "        files = get_files(region, resolution)\n",
-                "        crs, extent = projections(\"albers\", region)\n",
-                "        for f in files:\n",
-                "            if \"error\" in str(f[\"source\"]):\n",
-                "                resampling = \"average\"\n",
-                "            elif resolution == 4000:\n",
-                "                resampling = \"mode\"\n",
-                "            else:\n",
+                "        if region == \"ak\":\n",
+                "            years = [2011, 2016]\n",
+                "        if region == \"conus\":\n",
+                "            years = [2001, 2004, 2006, 2008, 2011, 2013, 2016]\n",
+                "        for year in years:\n",
+                "            f = get_file(region, year, resolution)\n",
+                "            crs, extent = projections(\"albers\", region)\n",
+                "            if resolution == 30:\n",
                 "                resampling = \"near\"\n",
-                "            cmd = (\n",
-                "                \"gdalwarp \"\n",
-                "                \"-t_srs '%s' \"\n",
-                "                \"-te %s \"\n",
-                "                \"-tr %s %s \"\n",
-                "                \"-r %s \"\n",
-                "                \"%s \"\n",
-                "                \"%s\"\n",
-                "            ) % (\n",
+                "            else:\n",
+                "                resampling = \"mode\"\n",
+                "            cmd = (\"gdalwarp \" \"-t_srs '%s' \" \"-te %s \" \"-tr %s %s \" \"-r %s \" \"%s \" \"%s\") % (\n",
                 "                crs,\n",
                 "                extent,\n",
                 "                resolution,\n",
                 "                resolution,\n",
                 "                resampling,\n",
                 "                f[\"source\"],\n",
                 "                \"./raster.tif\",\n",
@@ -136,94 +146,169 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "groups = [\n",
-                "    100,\n",
-                "    120,\n",
-                "    140,\n",
-                "    160,\n",
-                "    180,\n",
-                "    200,\n",
-                "    220,\n",
-                "    240,\n",
-                "    260,\n",
-                "    280,\n",
-                "    300,\n",
-                "    320,\n",
-                "    340,\n",
-                "    360,\n",
-                "    370,\n",
-                "    380,\n",
-                "    400,\n",
-                "    500,\n",
-                "    600,\n",
-                "    700,\n",
-                "    800,\n",
-                "    900,\n",
-                "    910,\n",
-                "    920,\n",
-                "    940,\n",
-                "    950,\n",
-                "    980,\n",
-                "    990,\n",
+                "categories = [\n",
+                "    11,\n",
+                "    12,\n",
+                "    21,\n",
+                "    22,\n",
+                "    23,\n",
+                "    24,\n",
+                "    31,\n",
+                "    41,\n",
+                "    42,\n",
+                "    43,\n",
+                "    51,\n",
+                "    52,\n",
+                "    71,\n",
+                "    72,\n",
+                "    73,\n",
+                "    74,\n",
+                "    81,\n",
+                "    82,\n",
+                "    90,\n",
+                "    95,\n",
                 "]"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "for resolution in [4000]:\n",
                 "    for region in [\"ak\", \"conus\"]:\n",
-                "        src = rasterio.open(workdir / f\"processed/nftd/{region}/250m/group.tif\")\n",
-                "        band = src.read(1)\n",
-                "        profile = src.profile\n",
-                "        profile[\"dtype\"] = \"uint8\"\n",
-                "\n",
-                "        for group in groups:\n",
-                "            print(f\"region {region} cat {group}\")\n",
-                "            crs, extent = projections(\"albers\", region)\n",
-                "            out = (band == group).astype(rasterio.uint8)\n",
-                "            resampling = \"average\"\n",
+                "        if region == \"ak\":\n",
+                "            years = [2011, 2016]\n",
+                "        if region == \"conus\":\n",
+                "            years = [2001, 2004, 2006, 2008, 2011, 2013, 2016]\n",
+                "        for year in years:\n",
+                "            fbase = get_file(region, year, resolution)\n",
+                "            src = rasterio.open(fbase[\"source\"])\n",
+                "            band = src.read(1)\n",
+                "            profile = src.profile\n",
+                "\n",
+                "            for category in categories:\n",
+                "                print(f\"region {region} year {year} cat {category}\")\n",
+                "                f = get_file(region, year, resolution, category)\n",
+                "                crs, extent = projections(\"albers\", region)\n",
+                "                if resolution == 30:\n",
+                "                    resampling = \"near\"\n",
+                "                else:\n",
+                "                    resampling = \"average\"\n",
+                "\n",
+                "                out = (band == category).astype(rasterio.uint8)\n",
+                "\n",
+                "                with rasterio.open(\"./thresholded.tif\", \"w\", **profile) as dst:\n",
+                "                    dst.write(out, 1)\n",
+                "\n",
+                "                cmd = (\n",
+                "                    \"gdalwarp \"\n",
+                "                    \"-t_srs '%s' \"\n",
+                "                    \"-te %s \"\n",
+                "                    \"-tr %s %s \"\n",
+                "                    \"-r %s \"\n",
+                "                    \"-ot Float32 \"\n",
+                "                    \"%s \"\n",
+                "                    \"%s\"\n",
+                "                ) % (\n",
+                "                    crs,\n",
+                "                    extent,\n",
+                "                    resolution,\n",
+                "                    resolution,\n",
+                "                    resampling,\n",
+                "                    \"./thresholded.tif\",\n",
+                "                    \"./raster.tif\",\n",
+                "                )\n",
+                "\n",
+                "                os.system(cmd)\n",
+                "                cog_translate(\"./raster.tif\", \"./raster.tif\", dst_profile)\n",
+                "                upload(\"./raster.tif\", f[\"target\"])\n",
+                "                os.remove(\"./thresholded.tif\")\n",
+                "                os.remove(\"./raster.tif\")"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "## recreate mode using max\n"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "categories = [\n",
+                "    11,\n",
+                "    12,\n",
+                "    21,\n",
+                "    22,\n",
+                "    23,\n",
+                "    24,\n",
+                "    31,\n",
+                "    41,\n",
+                "    42,\n",
+                "    43,\n",
+                "    51,\n",
+                "    52,\n",
+                "    71,\n",
+                "    72,\n",
+                "    73,\n",
+                "    74,\n",
+                "    81,\n",
+                "    82,\n",
+                "    90,\n",
+                "    95,\n",
+                "]"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "for resolution in [4000]:\n",
+                "    for region in [\"ak\"]:\n",
+                "        if region == \"ak\":\n",
+                "            years = [2011, 2016]\n",
+                "        if region == \"conus\":\n",
+                "            years = [2001, 2004, 2006, 2008, 2011, 2013, 2016]\n",
+                "        for year in years:\n",
+                "            bands = asarray(\n",
+                "                [\n",
+                "                    loadrio(workdir / f\"nlcd/{region}/{resolution}m/{year}_c{c}.tif\")\n",
+                "                    for c in categories\n",
+                "                ]\n",
+                "            )\n",
+                "            out = argmax(bands, axis=0)\n",
+                "            out_reindexed = argmax(bands, axis=0).astype(rasterio.uint8)\n",
+                "            for i, c in enumerate(categories):\n",
+                "                out_reindexed[out == i] = c\n",
+                "            out_reindexed[bands.sum(axis=0) == 0] = 0\n",
+                "\n",
+                "            src = rasterio.open(workdir / f\"nlcd/{region}/{resolution}m/{year}_c11.tif\")\n",
+                "            profile = src.profile\n",
+                "            profile.update(dtype=rasterio.uint8)\n",
                 "\n",
-                "            with rasterio.open(\"./thresholded.tif\", \"w\", **profile) as dst:\n",
-                "                dst.write(out, 1)\n",
+                "            with rasterio.open(\"raster.tif\", \"w\", **profile) as dst:\n",
+                "                dst.write(out_reindexed, 1)\n",
                 "\n",
-                "            cmd = (\n",
-                "                \"gdalwarp \"\n",
-                "                \"-t_srs '%s' \"\n",
-                "                \"-te %s \"\n",
-                "                \"-tr %s %s \"\n",
-                "                \"-r %s \"\n",
-                "                \"-ot Float32 \"\n",
-                "                \"%s \"\n",
-                "                \"%s\"\n",
-                "            ) % (\n",
-                "                crs,\n",
-                "                extent,\n",
-                "                resolution,\n",
-                "                resolution,\n",
-                "                resampling,\n",
-                "                \"./thresholded.tif\",\n",
-                "                \"./raster.tif\",\n",
-                "            )\n",
+                "            cog_translate(\"./raster.tif\", f\"./{year}_cmax.tif\", dst_profile)\n",
                 "\n",
-                "            os.system(cmd)\n",
-                "            cog_translate(\"./raster.tif\", \"./raster.tif\", dst_profile)\n",
-                "            upload(\n",
-                "                \"./raster.tif\",\n",
-                "                f\"processed/nftd/{region}/{resolution}m/group_g{group}.tif\",\n",
-                "            )\n",
-                "            os.remove(\"./thresholded.tif\")\n",
+                "            f = get_file(region, year, resolution, \"max\")\n",
+                "            upload(f\"./{year}_cmax.tif\", f[\"target\"])\n",
                 "            os.remove(\"./raster.tif\")"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3",
```

### Comparing `carbonplan-data-0.4.0/scripts/nlcd/00_download.ipynb` & `carbonplan_data-0.4.3/scripts/nlcd/00_download.ipynb`

 * *Files identical despite different names*

### Comparing `carbonplan-data-0.4.0/scripts/nlcd/01_nlcd_to_cogs.ipynb` & `carbonplan_data-0.4.3/scripts/nlcd/01_nlcd_to_cogs.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9987009604978355%*

 * *Differences: {"'cells'": '{2: {\'source\': {insert: [(2, \'os.environ["GOOGLE_APPLICATION_CREDENTIALS"] = '*

 * *            "(\\n'), (3, '    "*

 * *            '"/Users/freeman/.config/gcloud/legacy_credentials/jeremy@carbonplan.org/adc.json"\\n\'), '*

 * *            "(4, ')\\n')], delete: [8, 4, 3, 2]}}, 4: {'source': {insert: [(7, 'cloud_target = "*

 * *            '"raw/mlrc/NLCD_Land_Cover_Change_Index_L48_20190424/30m/raster.tif"\')], delete: [9, '*

 * *            "8, 7]}}, 9: {'source': {insert: [(6, '    source = workdir / "*

 * *         […]*

```diff
@@ -51,21 +51,20 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# This is the COG profile:\n",
                 "dst_profile = cog_profiles.get(\"deflate\")\n",
-                "os.environ[\n",
-                "    \"GOOGLE_APPLICATION_CREDENTIALS\"\n",
-                "] = \"/Users/freeman/.config/gcloud/legacy_credentials/jeremy@carbonplan.org/adc.json\"\n",
+                "os.environ[\"GOOGLE_APPLICATION_CREDENTIALS\"] = (\n",
+                "    \"/Users/freeman/.config/gcloud/legacy_credentials/jeremy@carbonplan.org/adc.json\"\n",
+                ")\n",
                 "\n",
                 "\n",
                 "def upload(src, target, bucket=\"carbonplan-data\"):\n",
-                "\n",
                 "    storage_client = storage.Client(\"carbonplan\")\n",
                 "    bucket = storage_client.bucket(bucket)\n",
                 "    blob = bucket.blob(target)\n",
                 "    blob.upload_from_filename(src)"
             ]
         },
         {
@@ -84,17 +83,15 @@
                 "# raw file\n",
                 "source = \"/Users/jhamman/workdir/carbonplan_data_downloads/mlrc/NLCD_Land_Cover_Change_Index_L48_20190424/NLCD_Land_Cover_Change_Index_L48_20190424.img\"\n",
                 "\n",
                 "# local target\n",
                 "target = \"./raster.tif\"\n",
                 "\n",
                 "# This is where we'll write the COGs when we're done\n",
-                "cloud_target = (\n",
-                "    \"raw/mlrc/NLCD_Land_Cover_Change_Index_L48_20190424/30m/raster.tif\"\n",
-                ")"
+                "cloud_target = \"raw/mlrc/NLCD_Land_Cover_Change_Index_L48_20190424/30m/raster.tif\""
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -154,18 +151,15 @@
             "source": [
                 "workdir = pathlib.Path(\"/Users/freeman/workdir/carbonplan_data_downloads/nlcd/\")\n",
                 "\n",
                 "target = \"./raster.tif\"\n",
                 "\n",
                 "for year in [2016]:\n",
                 "    print(year)\n",
-                "    source = (\n",
-                "        workdir\n",
-                "        / f\"NLCD_{year}_Land_Cover_AK_20200213/NLCD_{year}_Land_Cover_AK_20200213.img\"\n",
-                "    )\n",
+                "    source = workdir / f\"NLCD_{year}_Land_Cover_AK_20200213/NLCD_{year}_Land_Cover_AK_20200213.img\"\n",
                 "    cloud_target = f\"raw/nlcd/NLCD_Land_Cover_AK_20200213/30m/{year}.tif\"\n",
                 "\n",
                 "    # translate to COG\n",
                 "    cog_translate(source, target, dst_profile)\n",
                 "\n",
                 "    # Upload to GCS\n",
                 "    upload(target, cloud_target)\n",
```

### Comparing `carbonplan-data-0.4.0/scripts/nlcd/02_downsampling_and_reprojection.ipynb` & `carbonplan_data-0.4.3/scripts/terraclimate/02_terraclimate_to_fiaplots.ipynb`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.915212539877062%*

 * *Differences: {"'cells'": "{1: {'cell_type': 'code', 'source': {insert: [(0, '# from dask.distributed import "*

 * *            "Client\\n'), (1, '# setup a local dask cluster\\n'), (2, '# client = Client()\\n'), "*

 * *            "(3, '# client\\n'), (5, 'from dask_gateway import Gateway\\n'), (7, 'gateway = "*

 * *            "Gateway()\\n'), (8, 'options = gateway.cluster_options()\\n'), (9, "*

 * *            "'options.worker_cores = 4\\n'), (10, 'options.worker_memory = 16\\n'), (11, 'cluster "*

 * *            "= gateway.new_cluster(clust […]*

```diff
@@ -1,327 +1,382 @@
 {
     "cells": [
         {
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": null,
             "metadata": {},
+            "outputs": [],
             "source": [
-                "<img width=\"50\" src=\"https://carbonplan-assets.s3.amazonaws.com/monogram/dark-small.png\" style=\"margin-left:0px;margin-top:20px\"/>\n",
-                "\n",
-                "# NLCD downsampling and reprojection\n",
-                "\n",
-                "_by Jeremy Freeman (CarbonPlan), August 2, 2020_\n",
-                "\n",
-                "This notebook downsamples and reprojects NLCD 30m rasters stored in Cloud\n",
-                "Optimized GeoTIFF into 30m, 250m, and 4000m GeoTIFFs.\n",
+                "import xarray as xr\n",
+                "import pandas as pd\n",
+                "import fsspec\n",
+                "import dask\n",
                 "\n",
-                "**Inputs:**\n",
+                "dask.config.set({\"distributed.logging.distributed\": \"critical\"})"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# from dask.distributed import Client\n",
+                "# setup a local dask cluster\n",
+                "# client = Client()\n",
+                "# client\n",
                 "\n",
-                "- COG outputs from `01_nlcd_to_cogs.ipynb`\n",
+                "from dask_gateway import Gateway\n",
                 "\n",
-                "**Outputs:**\n",
+                "gateway = Gateway()\n",
+                "options = gateway.cluster_options()\n",
+                "options.worker_cores = 4\n",
+                "options.worker_memory = 16\n",
+                "cluster = gateway.new_cluster(cluster_options=options)\n",
+                "cluster.adapt(minimum=1, maximum=40)\n",
+                "cluster"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "client = cluster.get_client()\n",
+                "client"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "bucket = \"gs://carbonplan-data/raw/terraclimate/4000m/raster.zarr\"\n",
+                "mapper = fsspec.get_mapper(bucket)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "%%time\n",
+                "ds = xr.open_zarr(mapper, consolidated=True)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "ds"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "ds.dims"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "null_count = ds.isnull().mean(\"time\")\n",
+                "null_count = null_count.where(null_count != 1)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "pdsi = null_count.pdsi.load()\n",
                 "\n",
-                "- COG outputs after downsampling and reprojection\n",
+                "# [::50, ::50].plot()"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "pdsi.coarsen(lat=2, lon=2).mean().plot(robust=True)\n",
+                "# pdsi"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "df = pd.read_csv(\"FIA_forBill_DroughtRiskV1_08182020.csv\")  # .iloc[0:10000]\n",
+                "df.head()"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "import math\n",
                 "\n",
-                "**Notes:**\n",
+                "n = 5\n",
                 "\n",
-                "- Source CRS and projection extent come from NLCD\n"
+                "size = math.ceil(len(df) / n)\n",
+                "assert len(df) <= size * n\n",
+                "print(size)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "import os"
+                "index_ds = df[[\"lat\", \"lon\"]].to_xarray()\n",
+                "index_ds"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from carbonplan_data.utils import projections, setup\n",
-                "\n",
-                "workdir, upload = setup(\"jeremy\")"
+                "# %%time\n",
+                "# ds_cond = ds.sel(lat=index_ds['lat'], lon=index_ds['lon'], method='nearest')\n",
+                "# ds_cond"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from rio_cogeo.cogeo import cog_translate\n",
-                "from rio_cogeo.profiles import cog_profiles\n",
-                "\n",
-                "dst_profile = cog_profiles.get(\"deflate\")"
+                "from tqdm import tqdm"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "import rasterio\n",
-                "from numpy import asarray, argmax"
+                "ds_list = []\n",
+                "for k, ids in tqdm(index_ds.groupby(index_ds.index // size)):\n",
+                "    ds_list.append(ds.sel(lat=ids[\"lat\"], lon=ids[\"lon\"], method=\"nearest\"))"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "def get_file(region, year, resolution, c=None):\n",
-                "    if c is not None:\n",
-                "        target = f\"processed/nlcd/{region}/{resolution}m/{year}_c{c}.tif\"\n",
-                "    else:\n",
-                "        target = f\"processed/nlcd/{region}/{resolution}m/{year}.tif\"\n",
-                "    return {\n",
-                "        \"source\": workdir / f\"nlcd/{region}/30m/{year}.tif\",\n",
-                "        \"target\": target,\n",
-                "    }"
+                "# ds_list[:2]"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "def loadrio(f):\n",
-                "    src = rasterio.open(f)\n",
-                "    return src.read(1)"
+                "sum(d.nbytes for d in ds_list) / 1e9"
             ]
         },
         {
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": null,
             "metadata": {},
+            "outputs": [],
             "source": [
-                "### downsample using mode\n"
+                "parts = []\n",
+                "for d in tqdm(ds_list):\n",
+                "    part = d.compute()\n",
+                "    parts.append(part)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "for resolution in [4000]:\n",
-                "    for region in [\"ak\", \"conus\"]:\n",
-                "        if region == \"ak\":\n",
-                "            years = [2011, 2016]\n",
-                "        if region == \"conus\":\n",
-                "            years = [2001, 2004, 2006, 2008, 2011, 2013, 2016]\n",
-                "        for year in years:\n",
-                "            f = get_file(region, year, resolution)\n",
-                "            crs, extent = projections(\"albers\", region)\n",
-                "            if resolution == 30:\n",
-                "                resampling = \"near\"\n",
-                "            else:\n",
-                "                resampling = \"mode\"\n",
-                "            cmd = (\n",
-                "                \"gdalwarp \"\n",
-                "                \"-t_srs '%s' \"\n",
-                "                \"-te %s \"\n",
-                "                \"-tr %s %s \"\n",
-                "                \"-r %s \"\n",
-                "                \"%s \"\n",
-                "                \"%s\"\n",
-                "            ) % (\n",
-                "                crs,\n",
-                "                extent,\n",
-                "                resolution,\n",
-                "                resolution,\n",
-                "                resampling,\n",
-                "                f[\"source\"],\n",
-                "                \"./raster.tif\",\n",
-                "            )\n",
-                "            os.system(cmd)\n",
-                "            cog_translate(\"./raster.tif\", \"./raster.tif\", dst_profile)\n",
-                "            upload(\"./raster.tif\", f[\"target\"])\n",
-                "            os.remove(\"./raster.tif\")"
+                "ds_cond = xr.concat(parts, dim=\"index\")\n",
+                "# ds_cond = ds_cond.chunk({'index': 40000, 'time': 240})"
             ]
         },
         {
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": null,
             "metadata": {},
+            "outputs": [],
             "source": [
-                "### downsample using thresholding\n"
+                "ds_cond.PDSI.isnull().sum(\"index\").plot()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "categories = [\n",
-                "    11,\n",
-                "    12,\n",
-                "    21,\n",
-                "    22,\n",
-                "    23,\n",
-                "    24,\n",
-                "    31,\n",
-                "    41,\n",
-                "    42,\n",
-                "    43,\n",
-                "    51,\n",
-                "    52,\n",
-                "    71,\n",
-                "    72,\n",
-                "    73,\n",
-                "    74,\n",
-                "    81,\n",
-                "    82,\n",
-                "    90,\n",
-                "    95,\n",
-                "]"
+                "ds_cond = xr.concat(parts, dim=\"index\")\n",
+                "ds_cond = ds_cond.chunk({\"index\": 40000, \"time\": 240})"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "for resolution in [4000]:\n",
-                "    for region in [\"ak\", \"conus\"]:\n",
-                "        if region == \"ak\":\n",
-                "            years = [2011, 2016]\n",
-                "        if region == \"conus\":\n",
-                "            years = [2001, 2004, 2006, 2008, 2011, 2013, 2016]\n",
-                "        for year in years:\n",
-                "            fbase = get_file(region, year, resolution)\n",
-                "            src = rasterio.open(fbase[\"source\"])\n",
-                "            band = src.read(1)\n",
-                "            profile = src.profile\n",
+                "from dask.distributed import Client\n",
                 "\n",
-                "            for category in categories:\n",
-                "                print(f\"region {region} year {year} cat {category}\")\n",
-                "                f = get_file(region, year, resolution, category)\n",
-                "                crs, extent = projections(\"albers\", region)\n",
-                "                if resolution == 30:\n",
-                "                    resampling = \"near\"\n",
-                "                else:\n",
-                "                    resampling = \"average\"\n",
+                "client = Client()\n",
+                "client"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "bucket = \"gs://carbonplan-scratch/terraclimate-fia-cond.zarr\"\n",
+                "mapper2 = fsspec.get_mapper(bucket)\n",
                 "\n",
-                "                out = (band == category).astype(rasterio.uint8)\n",
+                "ds_cond.to_zarr(mapper2, mode=\"w\")"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# bucket = \"gs://carbonplan-scratch/terraclimate-fia-cond.zarr\"\n",
+                "# mapper2 = fsspec.get_mapper(bucket)\n",
                 "\n",
-                "                with rasterio.open(\"./thresholded.tif\", \"w\", **profile) as dst:\n",
-                "                    dst.write(out, 1)\n",
+                "# ds_cond = xr.open_zarr(mapper2)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# ds_cond_ann = ds_cond.resample(time='AS').mean()\n",
+                "# ds_cond_ann"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "def weighted_mean(ds, *args, **kwargs):\n",
+                "    weights = ds.time.dt.days_in_month\n",
+                "    return ds.weighted(weights).mean(dim=\"time\")\n",
                 "\n",
-                "                cmd = (\n",
-                "                    \"gdalwarp \"\n",
-                "                    \"-t_srs '%s' \"\n",
-                "                    \"-te %s \"\n",
-                "                    \"-tr %s %s \"\n",
-                "                    \"-r %s \"\n",
-                "                    \"-ot Float32 \"\n",
-                "                    \"%s \"\n",
-                "                    \"%s\"\n",
-                "                ) % (\n",
-                "                    crs,\n",
-                "                    extent,\n",
-                "                    resolution,\n",
-                "                    resolution,\n",
-                "                    resampling,\n",
-                "                    \"./thresholded.tif\",\n",
-                "                    \"./raster.tif\",\n",
-                "                )\n",
                 "\n",
-                "                os.system(cmd)\n",
-                "                cog_translate(\"./raster.tif\", \"./raster.tif\", dst_profile)\n",
-                "                upload(\"./raster.tif\", f[\"target\"])\n",
-                "                os.remove(\"./thresholded.tif\")\n",
-                "                os.remove(\"./raster.tif\")"
+                "ds_cond_ann = ds_cond.resample(time=\"AS\").map(weighted_mean, dim=\"time\")"
             ]
         },
         {
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": null,
             "metadata": {},
+            "outputs": [],
             "source": [
-                "## recreate mode using max\n"
+                "ds_cond_ann = ds_cond_ann.chunk({\"index\": -1, \"time\": -1})\n",
+                "ds_cond_ann[\"lon\"] = ds_cond_ann[\"lon\"].load()\n",
+                "ds_cond_ann[\"lat\"] = ds_cond_ann[\"lat\"].load()\n",
+                "ds_cond_ann"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "categories = [\n",
-                "    11,\n",
-                "    12,\n",
-                "    21,\n",
-                "    22,\n",
-                "    23,\n",
-                "    24,\n",
-                "    31,\n",
-                "    41,\n",
-                "    42,\n",
-                "    43,\n",
-                "    51,\n",
-                "    52,\n",
-                "    71,\n",
-                "    72,\n",
-                "    73,\n",
-                "    74,\n",
-                "    81,\n",
-                "    82,\n",
-                "    90,\n",
-                "    95,\n",
-                "]"
+                "# from zarr.storage import ZipStore\n",
+                "\n",
+                "# store = ZipStore('terraclimate-fia-cond-ann.zarr.zip', mode='w')"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "for resolution in [4000]:\n",
-                "    for region in [\"ak\"]:\n",
-                "        if region == \"ak\":\n",
-                "            years = [2011, 2016]\n",
-                "        if region == \"conus\":\n",
-                "            years = [2001, 2004, 2006, 2008, 2011, 2013, 2016]\n",
-                "        for year in years:\n",
-                "            bands = asarray(\n",
-                "                [\n",
-                "                    loadrio(\n",
-                "                        workdir / f\"nlcd/{region}/{resolution}m/{year}_c{c}.tif\"\n",
-                "                    )\n",
-                "                    for c in categories\n",
-                "                ]\n",
-                "            )\n",
-                "            out = argmax(bands, axis=0)\n",
-                "            out_reindexed = argmax(bands, axis=0).astype(rasterio.uint8)\n",
-                "            for i, c in enumerate(categories):\n",
-                "                out_reindexed[out == i] = c\n",
-                "            out_reindexed[bands.sum(axis=0) == 0] = 0\n",
-                "\n",
-                "            src = rasterio.open(\n",
-                "                workdir / f\"nlcd/{region}/{resolution}m/{year}_c11.tif\"\n",
-                "            )\n",
-                "            profile = src.profile\n",
-                "            profile.update(dtype=rasterio.uint8)\n",
-                "\n",
-                "            with rasterio.open(\"raster.tif\", \"w\", **profile) as dst:\n",
-                "                dst.write(out_reindexed, 1)\n",
+                "encoding = {k: {} for k in ds_cond_ann.data_vars}\n",
+                "encoding"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "bucket = \"gs://carbonplan-scratch/terraclimate-fia-cond-ann-3.zarr\"\n",
+                "mapper3 = fsspec.get_mapper(bucket, create=True)\n",
                 "\n",
-                "            cog_translate(\"./raster.tif\", f\"./{year}_cmax.tif\", dst_profile)\n",
+                "from dask.diagnostics import ProgressBar\n",
                 "\n",
-                "            f = get_file(region, year, resolution, \"max\")\n",
-                "            upload(f\"./{year}_cmax.tif\", f[\"target\"])\n",
-                "            os.remove(\"./raster.tif\")"
+                "with ProgressBar():\n",
+                "    ds_cond_ann.to_zarr(mapper3, mode=\"w\", consolidated=True, encoding=encoding)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "da = ds_cond_ann.PDSI.load()"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "da.isel(index=slice(20000))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "da.isnull().sum(\"index\").plot()"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3",
             "language": "python",
@@ -333,13 +388,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.7.8"
+            "version": "3.8.6"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `carbonplan-data-0.4.0/scripts/prism/00_download.ipynb` & `carbonplan_data-0.4.3/scripts/prism/00_download.ipynb`

 * *Files identical despite different names*

### Comparing `carbonplan-data-0.4.0/scripts/prism/01_prism_to_cogs.ipynb` & `carbonplan_data-0.4.3/scripts/prism/01_prism_to_cogs.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999348958333334%*

 * *Differences: {"'cells'": "{5: {'source': {delete: [11]}}}"}*

```diff
@@ -99,15 +99,14 @@
                 "    \"/Users/jhamman/workdir/carbonplan_data_downloads/PRISM_ppt_ak_30yr_normal_800mM1_annual_asc/ak_ppt_1981_2010.14.tif\",\n",
                 "]\n",
                 "\n",
                 "# local target\n",
                 "target = \"./raster.tif\"\n",
                 "\n",
                 "for source in sources:\n",
-                "\n",
                 "    for var in [\"ppt\", \"tmean\"]:\n",
                 "        if var in source:\n",
                 "            break\n",
                 "\n",
                 "    if \"ak\" in source:\n",
                 "        region = \"ak\"\n",
                 "    else:\n",
```

### Comparing `carbonplan-data-0.4.0/scripts/prism/02_downsample_and_reproject.ipynb` & `carbonplan_data-0.4.3/scripts/prism/02_downsample_and_reproject.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996448863636364%*

 * *Differences: {"'cells'": "{3: {'source': {insert: [(10, '        cloud_target = "*

 * *            'f"processed/prism/normals/{region}/{resolution}m/{var}.tif"\\n\')], delete: [13, 12, '*

 * *            '11, 7]}}}'}*

```diff
@@ -62,21 +62,18 @@
                 "resampling = \"average\"\n",
                 "resolution = 4000\n",
                 "\n",
                 "for region in [\"conus\", \"ak\"]:\n",
                 "    crs, extent = projections(\"albers\", region)\n",
                 "\n",
                 "    for var in [\"ppt\", \"tmean\"]:\n",
-                "\n",
                 "        print(region, var)\n",
                 "\n",
                 "        source = f\"carbonplan-data/raw/prism/normals/{region}/800m/{var}.tif\"\n",
-                "        cloud_target = (\n",
-                "            f\"processed/prism/normals/{region}/{resolution}m/{var}.tif\"\n",
-                "        )\n",
+                "        cloud_target = f\"processed/prism/normals/{region}/{resolution}m/{var}.tif\"\n",
                 "\n",
                 "        local_source = \"./local_source.tif\"\n",
                 "        fs.get_file(source, local_source)\n",
                 "\n",
                 "        cmd = (\n",
                 "            \"gdalwarp\",\n",
                 "            \"-t_srs\",\n",
```

### Comparing `carbonplan-data-0.4.0/scripts/statsgo/01_raw_to_tif.py` & `carbonplan_data-0.4.3/scripts/statsgo/01_raw_to_tif.py`

 * *Files identical despite different names*

### Comparing `carbonplan-data-0.4.0/scripts/terraclimate/01_terraclimate_aux_fileds_to_zarr.ipynb` & `carbonplan_data-0.4.3/scripts/terraclimate/01_terraclimate_aux_fileds_to_zarr.ipynb`

 * *Files identical despite different names*

### Comparing `carbonplan-data-0.4.0/scripts/terraclimate/01_terraclimate_to_zarr3.ipynb` & `carbonplan_data-0.4.3/scripts/terraclimate/01_terraclimate_to_zarr3.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9990707059780985%*

 * *Differences: {"'cells'": '{6: {\'source\': {insert: [(1, \'zarrs = [fn + ".zarr" for fn in '*

 * *            'fs.glob("carbonplan-scratch/terraclimate-cache/*nc")]\\n\')], delete: [3, 2, 1]}}, 8: '*

 * *            "{'source': {insert: [(82, '    fs = "*

 * *            'fsspec.get_filesystem_class(cache_location.split(":")[0])(token="cloud")\\n\')], '*

 * *            "delete: [114, 84, 83, 82]}}, 9: {'source': {insert: [(0, 'source_url_pattern = "*

 * *            "(\\n'), (1, '    "*

 * *            '"https://climate.northwestknowledge.net/TERRA […]*

```diff
@@ -101,17 +101,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# # uncomment to remove all temporary zarr stores\n",
-                "zarrs = [\n",
-                "    fn + \".zarr\" for fn in fs.glob(\"carbonplan-scratch/terraclimate-cache/*nc\")\n",
-                "]\n",
+                "zarrs = [fn + \".zarr\" for fn in fs.glob(\"carbonplan-scratch/terraclimate-cache/*nc\")]\n",
                 "fs.rm(zarrs, recursive=True)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
@@ -242,17 +240,15 @@
                 "    cache_location : str\n",
                 "        Path or url to the target location for the source file.\n",
                 "    Returns\n",
                 "    -------\n",
                 "    target_url : str\n",
                 "        Path or url in the form of `{cache_location}/hash({source_url})`.\n",
                 "    \"\"\"\n",
-                "    fs = fsspec.get_filesystem_class(cache_location.split(\":\")[0])(\n",
-                "        token=\"cloud\"\n",
-                "    )\n",
+                "    fs = fsspec.get_filesystem_class(cache_location.split(\":\")[0])(token=\"cloud\")\n",
                 "\n",
                 "    name = urlpath.URL(source_url).name\n",
                 "    target_url = os.path.join(cache_location, name)\n",
                 "\n",
                 "    # there is probably a better way to do caching!\n",
                 "    try:\n",
                 "        fs.open(target_url)\n",
@@ -274,15 +270,14 @@
                 "\n",
                 "    target_url = source_url + \".zarr\"\n",
                 "\n",
                 "    if fs.exists(urlpath.URL(target_url) / \".zmetadata\"):\n",
                 "        return target_url\n",
                 "\n",
                 "    with dask.config.set(scheduler=\"single-threaded\"):\n",
-                "\n",
                 "        try:\n",
                 "            ds = (\n",
                 "                xr.open_dataset(fs.open(source_url), engine=\"h5netcdf\")\n",
                 "                .pipe(preproc)\n",
                 "                .pipe(postproc)\n",
                 "                .load()\n",
                 "                .chunk(chunks)\n",
@@ -298,15 +293,17 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "source_url_pattern = \"https://climate.northwestknowledge.net/TERRACLIMATE-DATA/TerraClimate_{var}_{year}.nc\"\n",
+                "source_url_pattern = (\n",
+                "    \"https://climate.northwestknowledge.net/TERRACLIMATE-DATA/TerraClimate_{var}_{year}.nc\"\n",
+                ")\n",
                 "source_urls = []\n",
                 "\n",
                 "for var in variables:\n",
                 "    for year in years:\n",
                 "        source_urls.append(source_url_pattern.format(var=var, year=year))\n",
                 "source_urls[:4]"
             ]
@@ -354,17 +351,15 @@
                 "    temp = []\n",
                 "    for year in tqdm(years):\n",
                 "        mapper = fsspec.get_mapper(\n",
                 "            f\"gs://carbonplan-scratch/terraclimate-cache/TerraClimate_{var}_{year}.nc.zarr\"\n",
                 "        )\n",
                 "        temp.append(xr.open_zarr(mapper, consolidated=True))\n",
                 "    print(f\"concat {var}\")\n",
-                "    ds_list.append(\n",
-                "        xr.concat(temp, dim=\"time\", coords=\"minimal\", compat=\"override\")\n",
-                "    )"
+                "    ds_list.append(xr.concat(temp, dim=\"time\", coords=\"minimal\", compat=\"override\"))"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `carbonplan-data-0.4.0/scripts/terraclimate/02_terraclimate_regrid.ipynb` & `carbonplan_data-0.4.3/scripts/terraclimate/02_terraclimate_regrid.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.998140589569161%*

 * *Differences: {"'cells'": "{4: {'source': {insert: [(5, 'target_location = "*

 * *            'f"gs://carbonplan-data/processed/{name}/conus/4000m/raster.zarr"\')], delete: [7, 6, '*

 * *            '5]}}, 5: {\'source\': {insert: [(1, "target_ds = xr.open_zarr(mapper, '*

 * *            'consolidated=True)  # .rename({\'xc\': \'lon\', \'yc\': \'lat\'})\\n")], delete: [3, '*

 * *            "2, 1]}}, 7: {'source': {insert: [(2, 'global_grid = global_grid.isel(y=slice(None, "*

 * *            "None, -1)).isel(y_b=slice(None, None, -1))\\n'), (13, […]*

```diff
@@ -90,29 +90,25 @@
             "outputs": [],
             "source": [
                 "# options\n",
                 "name = \"terraclimate\"\n",
                 "raw_location = f\"gs://carbonplan-data/raw/terraclimate/4000m/raster.zarr\"\n",
                 "target_grid = \"gs://carbonplan-data/processed/grids/conus/4000m/domain.zarr\"\n",
                 "# getting weird errors when writing to carbonplan-data\n",
-                "target_location = (\n",
-                "    f\"gs://carbonplan-data/processed/{name}/conus/4000m/raster.zarr\"\n",
-                ")"
+                "target_location = f\"gs://carbonplan-data/processed/{name}/conus/4000m/raster.zarr\""
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "mapper = fsspec.get_mapper(target_grid)\n",
-                "target_ds = xr.open_zarr(\n",
-                "    mapper, consolidated=True\n",
-                ")  # .rename({'xc': 'lon', 'yc': 'lat'})\n",
+                "target_ds = xr.open_zarr(mapper, consolidated=True)  # .rename({'xc': 'lon', 'yc': 'lat'})\n",
                 "target_ds"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
@@ -127,44 +123,38 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "step = 360 / 8640 + 1e-9\n",
                 "global_grid = xe.util.grid_global(step, step)\n",
-                "global_grid = global_grid.isel(y=slice(None, None, -1)).isel(\n",
-                "    y_b=slice(None, None, -1)\n",
-                ")\n",
+                "global_grid = global_grid.isel(y=slice(None, None, -1)).isel(y_b=slice(None, None, -1))\n",
                 "global_grid[\"lat_b\"].values = np.clip(global_grid[\"lat_b\"].values, -90, 90)\n",
                 "display(global_grid)\n",
                 "\n",
                 "# check that this grid is a drop in replacement for the source grid\n",
                 "assert np.abs(global_grid.lat.isel(x=0).values - ds.lat.values).max() < 1e-5\n",
                 "assert np.abs(global_grid.lon.isel(y=0).values - ds.lon.values).max() < 1e-5\n",
                 "assert np.abs(global_grid.lat).max().item() <= 90\n",
                 "assert np.abs(global_grid.lat_b).max().item() <= 90\n",
                 "\n",
                 "# rename grid variables\n",
-                "source_ds = ds.rename({\"lon\": \"x\", \"lat\": \"y\"}).assign_coords(\n",
-                "    coords=global_grid.coords\n",
-                ")"
+                "source_ds = ds.rename({\"lon\": \"x\", \"lat\": \"y\"}).assign_coords(coords=global_grid.coords)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "regridders = {}\n",
                 "\n",
                 "for method in variables:\n",
-                "    regridders[method] = xe.Regridder(\n",
-                "        source_ds, target_ds, method, reuse_weights=True\n",
-                "    )"
+                "    regridders[method] = xe.Regridder(source_ds, target_ds, method, reuse_weights=True)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `carbonplan-data-0.4.0/sources.yaml` & `carbonplan_data-0.4.3/sources.yaml`

 * *Files identical despite different names*

