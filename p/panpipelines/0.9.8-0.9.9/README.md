# Comparing `tmp/panpipelines-0.9.8.tar.gz` & `tmp/panpipelines-0.9.9.tar.gz`

## Comparing `panpipelines-0.9.8.tar` & `panpipelines-0.9.9.tar`

### file list

```diff
@@ -1,179 +1,179 @@
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 panpipelines-0.9.8/.github/workflows/python-package.yml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 panpipelines-0.9.8/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     5401 2020-02-02 00:00:00.000000 panpipelines-0.9.8/PAN250_Deployment/README.md
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 panpipelines-0.9.8/PAN250_Deployment/run_pan250.sh
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 panpipelines-0.9.8/PAN250_Deployment/atlas/Arterial/README.md
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 panpipelines-0.9.8/PAN250_Deployment/atlas/Arterial/res-02_atlas-Arterial_dseg.tsv
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 panpipelines-0.9.8/PAN250_Deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.json
--rw-r--r--   0        0        0    37861 2020-02-02 00:00:00.000000 panpipelines-0.9.8/PAN250_Deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.nii.gz
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 panpipelines-0.9.8/PAN250_Deployment/atlas/XTRACT/README.md
--rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 panpipelines-0.9.8/PAN250_Deployment/atlas/XTRACT/res-02_atlas-XTRACT_dseg.txt
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 panpipelines-0.9.8/PAN250_Deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.json
--rw-r--r--   0        0        0    42696 2020-02-02 00:00:00.000000 panpipelines-0.9.8/PAN250_Deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.nii.gz
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 panpipelines-0.9.8/PAN250_Deployment/batch_scripts/group_template.pbs
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 panpipelines-0.9.8/PAN250_Deployment/batch_scripts/participant_template.pbs
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 panpipelines-0.9.8/PAN250_Deployment/batch_scripts/headers/slurm_cpu.pbs
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 panpipelines-0.9.8/PAN250_Deployment/batch_scripts/headers/slurm_cpu_highpri.pbs
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 panpipelines-0.9.8/PAN250_Deployment/batch_scripts/headers/slurm_cpu_highpri_long.pbs
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 panpipelines-0.9.8/PAN250_Deployment/batch_scripts/headers/slurm_cpu_highpri_medium.pbs
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 panpipelines-0.9.8/PAN250_Deployment/batch_scripts/headers/slurm_cpu_highpri_small.pbs
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 panpipelines-0.9.8/PAN250_Deployment/batch_scripts/headers/slurm_cpu_highpri_tiny.pbs
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 panpipelines-0.9.8/PAN250_Deployment/batch_scripts/headers/slurm_cpu_highpri_verylong.pbs
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 panpipelines-0.9.8/PAN250_Deployment/batch_scripts/headers/slurm_cpu_small.pbs
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 panpipelines-0.9.8/PAN250_Deployment/batch_scripts/headers/slurm_cpu_tiny.pbs
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 panpipelines-0.9.8/PAN250_Deployment/batch_scripts/headers/slurm_gpu.pbs
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 panpipelines-0.9.8/PAN250_Deployment/config/license.txt
--rw-r--r--   0        0        0    10449 2020-02-02 00:00:00.000000 panpipelines-0.9.8/PAN250_Deployment/config/pan250.config
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 panpipelines-0.9.8/PAN250_Deployment/config/pan250_eddyparams.json
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 panpipelines-0.9.8/PAN250_Deployment/config/credentials/credentials.json
--rw-r--r--   0        0        0    10047 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/README.md
--rwxr-xr-x   0        0        0     1471 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/run_pan_slurm.sh
--rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/AAL3/AAL3v1_1mm_index.txt
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/AAL3/README.md
--rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/AAL3/res-01_atlas-AAL3_dseg.tsv
--rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/AAL3/res-02_atlas-AAL3_dseg.tsv
--rw-r--r--   0        0        0   119500 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/AAL3/MNI152NLin6Asym/AAL3v1_1mm_MNI152NLin6Asym.nii.gz
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-AAL3_dseg.json
--rw-r--r--   0        0        0   119500 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-AAL3_dseg.nii.gz
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-AAL3_dseg.json
--rw-r--r--   0        0        0    38695 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-AAL3_dseg.nii.gz
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/AAL3/MNI152NLin6Asym/Development/convert.sh
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/AAL3/MNI152NLin6Asym/Development/eye.mat
--rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/AAL3/MNI152NLin6Asym/Development/getTemplate.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/Arterial/ArterialAtlasLabels.txt
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/Arterial/README.md
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/Arterial/res-01_atlas-Arterial_dseg.tsv
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/Arterial/res-02_atlas-Arterial_dseg.tsv
--rw-r--r--   0        0        0   182712 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/Arterial/MNI152NLin6Asym/ArterialAtlas_int.nii.gz
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-Arterial_dseg.json
--rw-r--r--   0        0        0   182309 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-Arterial_dseg.nii.gz
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.json
--rw-r--r--   0        0        0    37861 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.nii.gz
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/HARVCORT/HarvardOxford-Cortical_index.txt
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/HARVCORT/README.md
--rwxr-xr-x   0        0        0   138203 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/HARVCORT/MNI152NLinAsym/HarvardOxford-cort-maxprob-thr25-1mm.nii.gz
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/HARVSUBCORT/HarvardOxford-Subcortical_index.txt
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/HARVSUBCORT/README.md
--rwxr-xr-x   0        0        0   166519 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/HARVSUBCORT/MNI152NLinAsym/HarvardOxford-sub-maxprob-thr25-1mm.nii.gz
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/HCPMMP1_FREESURFER/README.md
--rwxr-xr-x   0        0        0    14105 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/HCPMMP1_FREESURFER/hcpmmp1_ordered.txt
--rwxr-xr-x   0        0        0    12646 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/HCPMMP1_FREESURFER/hcpmmp1_original.txt
--rw-r--r--   0        0        0  1316983 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/HCPMMP1_FREESURFER/lh.HCP-MMP1.annot
--rw-r--r--   0        0        0  1316984 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/HCPMMP1_FREESURFER/rh.HCP-MMP1.annot
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/JHU/JHU-labels_index.txt
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/JHU/JHU-tracts_index.txt
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/JHU/README.md
--rwxr-xr-x   0        0        0    47474 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/JHU/MNI152NLinAsym/JHU-ICBM-labels-1mm.nii.gz
--rwxr-xr-x   0        0        0    47922 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/JHU/MNI152NLinAsym/JHU-ICBM-tracts-maxprob-thr25-1mm.nii.gz
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/XTRACT/README.md
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/XTRACT/XTRACT_index.txt
--rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/XTRACT/res-01_atlas-XTRACT_dseg.txt
--rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/XTRACT/res-02_atlas-XTRACT_dseg.txt
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-XTRACT_dseg.json
--rw-r--r--   0        0        0   191828 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-XTRACT_dseg.nii.gz
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.json
--rw-r--r--   0        0        0    42696 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.nii.gz
--rw-r--r--   0        0        0   196623 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/XTRACT/MNI152NLin6Asym/xtract-tract-atlases-maxprob5-1mm.nii.gz
--rwxr-xr-x   0        0        0    89181 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/freesurfer_atlas/FreeSurferColorLUT.txt
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/freesurfer_atlas/README.md
--rwxr-xr-x   0        0        0    10131 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/freesurfer_atlas/fs_a2009s.txt
--rw-r--r--   0        0        0     6193 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/freesurfer_atlas/fs_default.txt
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/hcpmmp1_subfields_atlas/README.md
--rwxr-xr-x   0        0        0    14879 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/hcpmmp1_subfields_atlas/hcpmmp1_subfields_ordered.txt
--rwxr-xr-x   0        0        0    13454 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/hcpmmp1_subfields_atlas/hcpmmp1_subfields_original.txt
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/batch_scripts/group_template.pbs
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/batch_scripts/participant_template.pbs
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/batch_scripts/headers/slurm_cpu.pbs
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/batch_scripts/headers/slurm_cpu_fmriprep.pbs
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/batch_scripts/headers/slurm_cpu_highpri.pbs
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/batch_scripts/headers/slurm_cpu_highpri_fmriprep.pbs
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/batch_scripts/headers/slurm_gpu.pbs
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/batch_scripts/headers/slurm_gpu_highpri.pbs
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/batch_scripts/headers/slurm_gpu_windfall.pbs
--rwxr-xr-x   0        0        0      384 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/config/eddy_params.json
--rwxr-xr-x   0        0        0      379 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/config/eddy_params_cpu.json
--rwxr-xr-x   0        0        0      124 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/config/freebash.sh
--rwxr-xr-x   0        0        0       66 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/config/license.txt
--rw-r--r--   0        0        0    23977 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/config/panpipeconfig_expanded_slurm.config
--rw-r--r--   0        0        0    28701 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/config/panpipeconfig_slurm.config
--rwxr-xr-x   0        0        0       59 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/config/credentials/credentials.json
--rwxr-xr-x   0        0        0      215 2020-02-02 00:00:00.000000 panpipelines-0.9.8/example/run_pan_example.sh
--rw-r--r--   0        0        0     3641 2020-02-02 00:00:00.000000 panpipelines-0.9.8/example/config/panpipeconfig_example.config
--rwxr-xr-x   0        0        0       59 2020-02-02 00:00:00.000000 panpipelines-0.9.8/example/config/credentials/credentials_example.json
--rw-r--r--   0        0        0     5085 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/Factory.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/__init__.py
--rw-r--r--   0        0        0     5016 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/group_subjects.py
--rwxr-xr-x   0        0        0    18596 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/pan_processing.py
--rw-r--r--   0        0        0     9022 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/single_subject.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/version.py
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/nodes/__init__.py
--rw-r--r--   0        0        0    14132 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/nodes/antstransform.py
--rw-r--r--   0        0        0     6406 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/nodes/aslprep.py
--rw-r--r--   0        0        0     5264 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/nodes/atlascreate.py
--rw-r--r--   0        0        0    22503 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/nodes/basil.py
--rw-r--r--   0        0        0     7549 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/nodes/collate_csv_group.py
--rw-r--r--   0        0        0     6288 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/nodes/collate_csv_single.py
--rw-r--r--   0        0        0     4563 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/nodes/dummy.py
--rw-r--r--   0        0        0    10177 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/nodes/fmriprep.py
--rw-r--r--   0        0        0    10720 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/nodes/freesurfer.py
--rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/nodes/fslanat.py
--rw-r--r--   0        0        0     7191 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/nodes/glm_randomize_group.py
--rw-r--r--   0        0        0     7622 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/nodes/lst.py
--rw-r--r--   0        0        0     6175 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/nodes/noddi.py
--rw-r--r--   0        0        0     8370 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/nodes/parse_textdata.py
--rw-r--r--   0        0        0    16867 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/nodes/preproc.py
--rw-r--r--   0        0        0     7806 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/nodes/qsiprep.py
--rw-r--r--   0        0        0    16463 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/nodes/roi_extract.py
--rw-r--r--   0        0        0     5324 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/nodes/roi_mean_group.py
--rw-r--r--   0        0        0    11130 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/nodes/roi_mean_single.py
--rw-r--r--   0        0        0    10201 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/nodes/tensor.py
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/pipelines/__init__.py
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/pipelines/aslprep_panpipeline.py
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/pipelines/basil_panpipeline.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/pipelines/collatecsv_panpipeline.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/pipelines/collatecsvgroup_panpipeline.py
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/pipelines/dummy_panpipeline.py
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/pipelines/fmriprep_panpipeline.py
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/pipelines/freesurfer_panpipeline.py
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/pipelines/lst_panpipeline.py
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/pipelines/noddi_panpipeline.py
--rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/pipelines/panpipeline.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/pipelines/preproc_panpipeline.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/pipelines/qsiprep_panpipeline.py
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/pipelines/roiextract_panpipeline.py
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/pipelines/tensor_panpipeline.py
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/pipelines/textmeasures_panpipeline.py
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/pipelines/volmeasures_panpipeline.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/scripts/__init__.py
--rw-r--r--   0        0        0     7141 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/scripts/aslprep_panscript.py
--rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/scripts/fmriprep_panscript.py
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/scripts/mne_make_surfaces.py
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/scripts/pancontainer_panscript.py
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/scripts/panscript.py
--rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/scripts/sdcflows_fieldmap.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/utils/__init__.py
--rw-r--r--   0        0        0    31963 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/utils/transformer.py
--rw-r--r--   0        0        0    73934 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/utils/util_functions.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/workflows/__init__.py
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/workflows/aslprep_workflow.py
--rw-r--r--   0        0        0     4783 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/workflows/basil_workflow.py
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/workflows/collatecsv_workflow.py
--rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/workflows/collatecsvgroup_workflow.py
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/workflows/dummy_workflow.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/workflows/fmriprep_workflow.py
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/workflows/freesurfer_workflow.py
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/workflows/lst_workflow.py
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/workflows/noddi_workflow.py
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/workflows/preproc_workflow.py
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/workflows/qsiprep_workflow.py
--rw-r--r--   0        0        0     7525 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/workflows/roiextract_workflow.py
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/workflows/tensor_workflow.py
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/workflows/textmeasures_workflow.py
--rw-r--r--   0        0        0     4946 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/workflows/volmeasures_workflow.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpipelines-0.9.8/tests/__init__.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 panpipelines-0.9.8/tests/test_PANFactory.py
--rw-r--r--   0        0        0     3152 2020-02-02 00:00:00.000000 panpipelines-0.9.8/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 panpipelines-0.9.8/LICENSE
--rw-r--r--   0        0        0    12997 2020-02-02 00:00:00.000000 panpipelines-0.9.8/README.md
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 panpipelines-0.9.8/pyproject.toml
--rw-r--r--   0        0        0    15188 2020-02-02 00:00:00.000000 panpipelines-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 panpipelines-0.9.9/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 panpipelines-0.9.9/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     5401 2020-02-02 00:00:00.000000 panpipelines-0.9.9/PAN250_Deployment/README.md
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 panpipelines-0.9.9/PAN250_Deployment/run_pan250.sh
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 panpipelines-0.9.9/PAN250_Deployment/atlas/Arterial/README.md
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 panpipelines-0.9.9/PAN250_Deployment/atlas/Arterial/res-02_atlas-Arterial_dseg.tsv
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 panpipelines-0.9.9/PAN250_Deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.json
+-rw-r--r--   0        0        0    37861 2020-02-02 00:00:00.000000 panpipelines-0.9.9/PAN250_Deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.nii.gz
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 panpipelines-0.9.9/PAN250_Deployment/atlas/XTRACT/README.md
+-rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 panpipelines-0.9.9/PAN250_Deployment/atlas/XTRACT/res-02_atlas-XTRACT_dseg.txt
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 panpipelines-0.9.9/PAN250_Deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.json
+-rw-r--r--   0        0        0    42696 2020-02-02 00:00:00.000000 panpipelines-0.9.9/PAN250_Deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.nii.gz
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 panpipelines-0.9.9/PAN250_Deployment/batch_scripts/group_template.pbs
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 panpipelines-0.9.9/PAN250_Deployment/batch_scripts/participant_template.pbs
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 panpipelines-0.9.9/PAN250_Deployment/batch_scripts/headers/slurm_cpu.pbs
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 panpipelines-0.9.9/PAN250_Deployment/batch_scripts/headers/slurm_cpu_highpri.pbs
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 panpipelines-0.9.9/PAN250_Deployment/batch_scripts/headers/slurm_cpu_highpri_long.pbs
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 panpipelines-0.9.9/PAN250_Deployment/batch_scripts/headers/slurm_cpu_highpri_medium.pbs
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 panpipelines-0.9.9/PAN250_Deployment/batch_scripts/headers/slurm_cpu_highpri_small.pbs
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 panpipelines-0.9.9/PAN250_Deployment/batch_scripts/headers/slurm_cpu_highpri_tiny.pbs
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 panpipelines-0.9.9/PAN250_Deployment/batch_scripts/headers/slurm_cpu_highpri_verylong.pbs
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 panpipelines-0.9.9/PAN250_Deployment/batch_scripts/headers/slurm_cpu_small.pbs
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 panpipelines-0.9.9/PAN250_Deployment/batch_scripts/headers/slurm_cpu_tiny.pbs
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 panpipelines-0.9.9/PAN250_Deployment/batch_scripts/headers/slurm_gpu.pbs
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 panpipelines-0.9.9/PAN250_Deployment/config/license.txt
+-rw-r--r--   0        0        0    10449 2020-02-02 00:00:00.000000 panpipelines-0.9.9/PAN250_Deployment/config/pan250.config
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 panpipelines-0.9.9/PAN250_Deployment/config/pan250_eddyparams.json
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 panpipelines-0.9.9/PAN250_Deployment/config/credentials/credentials.json
+-rw-r--r--   0        0        0    10047 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/README.md
+-rwxr-xr-x   0        0        0     1471 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/run_pan_slurm.sh
+-rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/AAL3/AAL3v1_1mm_index.txt
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/AAL3/README.md
+-rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/AAL3/res-01_atlas-AAL3_dseg.tsv
+-rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/AAL3/res-02_atlas-AAL3_dseg.tsv
+-rw-r--r--   0        0        0   119500 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/AAL3/MNI152NLin6Asym/AAL3v1_1mm_MNI152NLin6Asym.nii.gz
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-AAL3_dseg.json
+-rw-r--r--   0        0        0   119500 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-AAL3_dseg.nii.gz
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-AAL3_dseg.json
+-rw-r--r--   0        0        0    38695 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-AAL3_dseg.nii.gz
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/AAL3/MNI152NLin6Asym/Development/convert.sh
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/AAL3/MNI152NLin6Asym/Development/eye.mat
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/AAL3/MNI152NLin6Asym/Development/getTemplate.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/Arterial/ArterialAtlasLabels.txt
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/Arterial/README.md
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/Arterial/res-01_atlas-Arterial_dseg.tsv
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/Arterial/res-02_atlas-Arterial_dseg.tsv
+-rw-r--r--   0        0        0   182712 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/Arterial/MNI152NLin6Asym/ArterialAtlas_int.nii.gz
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-Arterial_dseg.json
+-rw-r--r--   0        0        0   182309 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-Arterial_dseg.nii.gz
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.json
+-rw-r--r--   0        0        0    37861 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.nii.gz
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/HARVCORT/HarvardOxford-Cortical_index.txt
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/HARVCORT/README.md
+-rwxr-xr-x   0        0        0   138203 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/HARVCORT/MNI152NLinAsym/HarvardOxford-cort-maxprob-thr25-1mm.nii.gz
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/HARVSUBCORT/HarvardOxford-Subcortical_index.txt
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/HARVSUBCORT/README.md
+-rwxr-xr-x   0        0        0   166519 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/HARVSUBCORT/MNI152NLinAsym/HarvardOxford-sub-maxprob-thr25-1mm.nii.gz
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/HCPMMP1_FREESURFER/README.md
+-rwxr-xr-x   0        0        0    14105 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/HCPMMP1_FREESURFER/hcpmmp1_ordered.txt
+-rwxr-xr-x   0        0        0    12646 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/HCPMMP1_FREESURFER/hcpmmp1_original.txt
+-rw-r--r--   0        0        0  1316983 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/HCPMMP1_FREESURFER/lh.HCP-MMP1.annot
+-rw-r--r--   0        0        0  1316984 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/HCPMMP1_FREESURFER/rh.HCP-MMP1.annot
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/JHU/JHU-labels_index.txt
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/JHU/JHU-tracts_index.txt
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/JHU/README.md
+-rwxr-xr-x   0        0        0    47474 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/JHU/MNI152NLinAsym/JHU-ICBM-labels-1mm.nii.gz
+-rwxr-xr-x   0        0        0    47922 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/JHU/MNI152NLinAsym/JHU-ICBM-tracts-maxprob-thr25-1mm.nii.gz
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/XTRACT/README.md
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/XTRACT/XTRACT_index.txt
+-rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/XTRACT/res-01_atlas-XTRACT_dseg.txt
+-rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/XTRACT/res-02_atlas-XTRACT_dseg.txt
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-XTRACT_dseg.json
+-rw-r--r--   0        0        0   191828 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-XTRACT_dseg.nii.gz
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.json
+-rw-r--r--   0        0        0    42696 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.nii.gz
+-rw-r--r--   0        0        0   196623 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/XTRACT/MNI152NLin6Asym/xtract-tract-atlases-maxprob5-1mm.nii.gz
+-rwxr-xr-x   0        0        0    89181 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/freesurfer_atlas/FreeSurferColorLUT.txt
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/freesurfer_atlas/README.md
+-rwxr-xr-x   0        0        0    10131 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/freesurfer_atlas/fs_a2009s.txt
+-rw-r--r--   0        0        0     6193 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/freesurfer_atlas/fs_default.txt
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/hcpmmp1_subfields_atlas/README.md
+-rwxr-xr-x   0        0        0    14879 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/hcpmmp1_subfields_atlas/hcpmmp1_subfields_ordered.txt
+-rwxr-xr-x   0        0        0    13454 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/hcpmmp1_subfields_atlas/hcpmmp1_subfields_original.txt
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/batch_scripts/group_template.pbs
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/batch_scripts/participant_template.pbs
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/batch_scripts/headers/slurm_cpu.pbs
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/batch_scripts/headers/slurm_cpu_fmriprep.pbs
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/batch_scripts/headers/slurm_cpu_highpri.pbs
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/batch_scripts/headers/slurm_cpu_highpri_fmriprep.pbs
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/batch_scripts/headers/slurm_gpu.pbs
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/batch_scripts/headers/slurm_gpu_highpri.pbs
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/batch_scripts/headers/slurm_gpu_windfall.pbs
+-rwxr-xr-x   0        0        0      384 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/config/eddy_params.json
+-rwxr-xr-x   0        0        0      379 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/config/eddy_params_cpu.json
+-rwxr-xr-x   0        0        0      124 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/config/freebash.sh
+-rwxr-xr-x   0        0        0       66 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/config/license.txt
+-rw-r--r--   0        0        0    23977 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/config/panpipeconfig_expanded_slurm.config
+-rw-r--r--   0        0        0    28701 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/config/panpipeconfig_slurm.config
+-rwxr-xr-x   0        0        0       59 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/config/credentials/credentials.json
+-rwxr-xr-x   0        0        0      215 2020-02-02 00:00:00.000000 panpipelines-0.9.9/example/run_pan_example.sh
+-rw-r--r--   0        0        0     3641 2020-02-02 00:00:00.000000 panpipelines-0.9.9/example/config/panpipeconfig_example.config
+-rwxr-xr-x   0        0        0       59 2020-02-02 00:00:00.000000 panpipelines-0.9.9/example/config/credentials/credentials_example.json
+-rw-r--r--   0        0        0     5085 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/Factory.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/__init__.py
+-rw-r--r--   0        0        0     5016 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/group_subjects.py
+-rwxr-xr-x   0        0        0    18596 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/pan_processing.py
+-rw-r--r--   0        0        0     9022 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/single_subject.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/version.py
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/nodes/__init__.py
+-rw-r--r--   0        0        0    14132 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/nodes/antstransform.py
+-rw-r--r--   0        0        0     6406 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/nodes/aslprep.py
+-rw-r--r--   0        0        0     5264 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/nodes/atlascreate.py
+-rw-r--r--   0        0        0    22715 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/nodes/basil.py
+-rw-r--r--   0        0        0     7549 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/nodes/collate_csv_group.py
+-rw-r--r--   0        0        0     6288 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/nodes/collate_csv_single.py
+-rw-r--r--   0        0        0     4563 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/nodes/dummy.py
+-rw-r--r--   0        0        0    10177 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/nodes/fmriprep.py
+-rw-r--r--   0        0        0    10720 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/nodes/freesurfer.py
+-rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/nodes/fslanat.py
+-rw-r--r--   0        0        0     7191 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/nodes/glm_randomize_group.py
+-rw-r--r--   0        0        0     7622 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/nodes/lst.py
+-rw-r--r--   0        0        0     6175 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/nodes/noddi.py
+-rw-r--r--   0        0        0     8370 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/nodes/parse_textdata.py
+-rw-r--r--   0        0        0    27239 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/nodes/preproc.py
+-rw-r--r--   0        0        0     7806 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/nodes/qsiprep.py
+-rw-r--r--   0        0        0    16463 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/nodes/roi_extract.py
+-rw-r--r--   0        0        0     5324 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/nodes/roi_mean_group.py
+-rw-r--r--   0        0        0    11130 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/nodes/roi_mean_single.py
+-rw-r--r--   0        0        0    10201 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/nodes/tensor.py
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/pipelines/__init__.py
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/pipelines/aslprep_panpipeline.py
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/pipelines/basil_panpipeline.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/pipelines/collatecsv_panpipeline.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/pipelines/collatecsvgroup_panpipeline.py
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/pipelines/dummy_panpipeline.py
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/pipelines/fmriprep_panpipeline.py
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/pipelines/freesurfer_panpipeline.py
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/pipelines/lst_panpipeline.py
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/pipelines/noddi_panpipeline.py
+-rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/pipelines/panpipeline.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/pipelines/preproc_panpipeline.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/pipelines/qsiprep_panpipeline.py
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/pipelines/roiextract_panpipeline.py
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/pipelines/tensor_panpipeline.py
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/pipelines/textmeasures_panpipeline.py
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/pipelines/volmeasures_panpipeline.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/scripts/__init__.py
+-rw-r--r--   0        0        0     7141 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/scripts/aslprep_panscript.py
+-rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/scripts/fmriprep_panscript.py
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/scripts/mne_make_surfaces.py
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/scripts/pancontainer_panscript.py
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/scripts/panscript.py
+-rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/scripts/sdcflows_fieldmap.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/utils/__init__.py
+-rw-r--r--   0        0        0    31963 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/utils/transformer.py
+-rw-r--r--   0        0        0    74620 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/utils/util_functions.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/workflows/__init__.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/workflows/aslprep_workflow.py
+-rw-r--r--   0        0        0     6185 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/workflows/basil_workflow.py
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/workflows/collatecsv_workflow.py
+-rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/workflows/collatecsvgroup_workflow.py
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/workflows/dummy_workflow.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/workflows/fmriprep_workflow.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/workflows/freesurfer_workflow.py
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/workflows/lst_workflow.py
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/workflows/noddi_workflow.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/workflows/preproc_workflow.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/workflows/qsiprep_workflow.py
+-rw-r--r--   0        0        0     7525 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/workflows/roiextract_workflow.py
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/workflows/tensor_workflow.py
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/workflows/textmeasures_workflow.py
+-rw-r--r--   0        0        0     4946 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/workflows/volmeasures_workflow.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpipelines-0.9.9/tests/__init__.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 panpipelines-0.9.9/tests/test_PANFactory.py
+-rw-r--r--   0        0        0     3152 2020-02-02 00:00:00.000000 panpipelines-0.9.9/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 panpipelines-0.9.9/LICENSE
+-rw-r--r--   0        0        0    12997 2020-02-02 00:00:00.000000 panpipelines-0.9.9/README.md
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 panpipelines-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0    15188 2020-02-02 00:00:00.000000 panpipelines-0.9.9/PKG-INFO
```

### Comparing `panpipelines-0.9.8/.github/workflows/python-package.yml` & `panpipelines-0.9.9/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/.github/workflows/python-publish.yml` & `panpipelines-0.9.9/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/PAN250_Deployment/README.md` & `panpipelines-0.9.9/PAN250_Deployment/README.md`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/PAN250_Deployment/run_pan250.sh` & `panpipelines-0.9.9/PAN250_Deployment/run_pan250.sh`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/PAN250_Deployment/atlas/Arterial/README.md` & `panpipelines-0.9.9/PAN250_Deployment/atlas/Arterial/README.md`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/PAN250_Deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.json` & `panpipelines-0.9.9/PAN250_Deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.json`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/PAN250_Deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.nii.gz` & `panpipelines-0.9.9/PAN250_Deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/PAN250_Deployment/atlas/XTRACT/README.md` & `panpipelines-0.9.9/PAN250_Deployment/atlas/XTRACT/README.md`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/PAN250_Deployment/atlas/XTRACT/res-02_atlas-XTRACT_dseg.txt` & `panpipelines-0.9.9/PAN250_Deployment/atlas/XTRACT/res-02_atlas-XTRACT_dseg.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/PAN250_Deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.json` & `panpipelines-0.9.9/PAN250_Deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.json`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/PAN250_Deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.nii.gz` & `panpipelines-0.9.9/PAN250_Deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/PAN250_Deployment/batch_scripts/group_template.pbs` & `panpipelines-0.9.9/PAN250_Deployment/batch_scripts/group_template.pbs`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/PAN250_Deployment/batch_scripts/participant_template.pbs` & `panpipelines-0.9.9/PAN250_Deployment/batch_scripts/participant_template.pbs`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/PAN250_Deployment/config/pan250.config` & `panpipelines-0.9.9/PAN250_Deployment/config/pan250.config`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/deployment/README.md` & `panpipelines-0.9.9/deployment/README.md`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/deployment/run_pan_slurm.sh` & `panpipelines-0.9.9/deployment/run_pan_slurm.sh`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/deployment/atlas/AAL3/AAL3v1_1mm_index.txt` & `panpipelines-0.9.9/deployment/atlas/AAL3/AAL3v1_1mm_index.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/deployment/atlas/AAL3/README.md` & `panpipelines-0.9.9/deployment/atlas/AAL3/README.md`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/deployment/atlas/AAL3/res-01_atlas-AAL3_dseg.tsv` & `panpipelines-0.9.9/deployment/atlas/AAL3/res-01_atlas-AAL3_dseg.tsv`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/deployment/atlas/AAL3/res-02_atlas-AAL3_dseg.tsv` & `panpipelines-0.9.9/deployment/atlas/AAL3/res-02_atlas-AAL3_dseg.tsv`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/deployment/atlas/AAL3/MNI152NLin6Asym/AAL3v1_1mm_MNI152NLin6Asym.nii.gz` & `panpipelines-0.9.9/deployment/atlas/AAL3/MNI152NLin6Asym/AAL3v1_1mm_MNI152NLin6Asym.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-AAL3_dseg.json` & `panpipelines-0.9.9/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-AAL3_dseg.json`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-AAL3_dseg.nii.gz` & `panpipelines-0.9.9/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-AAL3_dseg.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-AAL3_dseg.json` & `panpipelines-0.9.9/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-AAL3_dseg.json`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-AAL3_dseg.nii.gz` & `panpipelines-0.9.9/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-AAL3_dseg.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/deployment/atlas/AAL3/MNI152NLin6Asym/Development/convert.sh` & `panpipelines-0.9.9/deployment/atlas/AAL3/MNI152NLin6Asym/Development/convert.sh`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/deployment/atlas/AAL3/MNI152NLin6Asym/Development/getTemplate.py` & `panpipelines-0.9.9/deployment/atlas/AAL3/MNI152NLin6Asym/Development/getTemplate.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/deployment/atlas/Arterial/README.md` & `panpipelines-0.9.9/deployment/atlas/Arterial/README.md`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/deployment/atlas/Arterial/MNI152NLin6Asym/ArterialAtlas_int.nii.gz` & `panpipelines-0.9.9/deployment/atlas/Arterial/MNI152NLin6Asym/ArterialAtlas_int.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-Arterial_dseg.json` & `panpipelines-0.9.9/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-Arterial_dseg.json`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-Arterial_dseg.nii.gz` & `panpipelines-0.9.9/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-Arterial_dseg.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.json` & `panpipelines-0.9.9/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.json`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.nii.gz` & `panpipelines-0.9.9/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/deployment/atlas/HARVCORT/HarvardOxford-Cortical_index.txt` & `panpipelines-0.9.9/deployment/atlas/HARVCORT/HarvardOxford-Cortical_index.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/deployment/atlas/HARVCORT/MNI152NLinAsym/HarvardOxford-cort-maxprob-thr25-1mm.nii.gz` & `panpipelines-0.9.9/deployment/atlas/HARVCORT/MNI152NLinAsym/HarvardOxford-cort-maxprob-thr25-1mm.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/deployment/atlas/HARVSUBCORT/MNI152NLinAsym/HarvardOxford-sub-maxprob-thr25-1mm.nii.gz` & `panpipelines-0.9.9/deployment/atlas/HARVSUBCORT/MNI152NLinAsym/HarvardOxford-sub-maxprob-thr25-1mm.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/deployment/atlas/HCPMMP1_FREESURFER/README.md` & `panpipelines-0.9.9/deployment/atlas/HCPMMP1_FREESURFER/README.md`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/deployment/atlas/HCPMMP1_FREESURFER/hcpmmp1_ordered.txt` & `panpipelines-0.9.9/deployment/atlas/HCPMMP1_FREESURFER/hcpmmp1_ordered.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/deployment/atlas/HCPMMP1_FREESURFER/hcpmmp1_original.txt` & `panpipelines-0.9.9/deployment/atlas/HCPMMP1_FREESURFER/hcpmmp1_original.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/deployment/atlas/HCPMMP1_FREESURFER/lh.HCP-MMP1.annot` & `panpipelines-0.9.9/deployment/atlas/HCPMMP1_FREESURFER/lh.HCP-MMP1.annot`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/deployment/atlas/HCPMMP1_FREESURFER/rh.HCP-MMP1.annot` & `panpipelines-0.9.9/deployment/atlas/HCPMMP1_FREESURFER/rh.HCP-MMP1.annot`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/deployment/atlas/JHU/JHU-labels_index.txt` & `panpipelines-0.9.9/deployment/atlas/JHU/JHU-labels_index.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/deployment/atlas/JHU/JHU-tracts_index.txt` & `panpipelines-0.9.9/deployment/atlas/JHU/JHU-tracts_index.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/deployment/atlas/JHU/MNI152NLinAsym/JHU-ICBM-labels-1mm.nii.gz` & `panpipelines-0.9.9/deployment/atlas/JHU/MNI152NLinAsym/JHU-ICBM-labels-1mm.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/deployment/atlas/JHU/MNI152NLinAsym/JHU-ICBM-tracts-maxprob-thr25-1mm.nii.gz` & `panpipelines-0.9.9/deployment/atlas/JHU/MNI152NLinAsym/JHU-ICBM-tracts-maxprob-thr25-1mm.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/deployment/atlas/XTRACT/README.md` & `panpipelines-0.9.9/deployment/atlas/XTRACT/README.md`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/deployment/atlas/XTRACT/XTRACT_index.txt` & `panpipelines-0.9.9/deployment/atlas/XTRACT/XTRACT_index.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/deployment/atlas/XTRACT/res-01_atlas-XTRACT_dseg.txt` & `panpipelines-0.9.9/deployment/atlas/XTRACT/res-01_atlas-XTRACT_dseg.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/deployment/atlas/XTRACT/res-02_atlas-XTRACT_dseg.txt` & `panpipelines-0.9.9/deployment/atlas/XTRACT/res-02_atlas-XTRACT_dseg.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-XTRACT_dseg.json` & `panpipelines-0.9.9/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-XTRACT_dseg.json`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-XTRACT_dseg.nii.gz` & `panpipelines-0.9.9/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-XTRACT_dseg.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.json` & `panpipelines-0.9.9/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.json`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.nii.gz` & `panpipelines-0.9.9/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/deployment/atlas/XTRACT/MNI152NLin6Asym/xtract-tract-atlases-maxprob5-1mm.nii.gz` & `panpipelines-0.9.9/deployment/atlas/XTRACT/MNI152NLin6Asym/xtract-tract-atlases-maxprob5-1mm.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/deployment/atlas/freesurfer_atlas/FreeSurferColorLUT.txt` & `panpipelines-0.9.9/deployment/atlas/freesurfer_atlas/FreeSurferColorLUT.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/deployment/atlas/freesurfer_atlas/fs_a2009s.txt` & `panpipelines-0.9.9/deployment/atlas/freesurfer_atlas/fs_a2009s.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/deployment/atlas/freesurfer_atlas/fs_default.txt` & `panpipelines-0.9.9/deployment/atlas/freesurfer_atlas/fs_default.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/deployment/atlas/hcpmmp1_subfields_atlas/hcpmmp1_subfields_ordered.txt` & `panpipelines-0.9.9/deployment/atlas/hcpmmp1_subfields_atlas/hcpmmp1_subfields_ordered.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/deployment/atlas/hcpmmp1_subfields_atlas/hcpmmp1_subfields_original.txt` & `panpipelines-0.9.9/deployment/atlas/hcpmmp1_subfields_atlas/hcpmmp1_subfields_original.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/deployment/batch_scripts/group_template.pbs` & `panpipelines-0.9.9/deployment/batch_scripts/group_template.pbs`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/deployment/batch_scripts/participant_template.pbs` & `panpipelines-0.9.9/deployment/batch_scripts/participant_template.pbs`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/deployment/config/panpipeconfig_expanded_slurm.config` & `panpipelines-0.9.9/deployment/config/panpipeconfig_expanded_slurm.config`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/deployment/config/panpipeconfig_slurm.config` & `panpipelines-0.9.9/deployment/config/panpipeconfig_slurm.config`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/example/config/panpipeconfig_example.config` & `panpipelines-0.9.9/example/config/panpipeconfig_example.config`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/src/panpipelines/Factory.py` & `panpipelines-0.9.9/src/panpipelines/Factory.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/src/panpipelines/group_subjects.py` & `panpipelines-0.9.9/src/panpipelines/group_subjects.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/src/panpipelines/pan_processing.py` & `panpipelines-0.9.9/src/panpipelines/pan_processing.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/src/panpipelines/single_subject.py` & `panpipelines-0.9.9/src/panpipelines/single_subject.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/src/panpipelines/nodes/antstransform.py` & `panpipelines-0.9.9/src/panpipelines/nodes/antstransform.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/src/panpipelines/nodes/aslprep.py` & `panpipelines-0.9.9/src/panpipelines/nodes/aslprep.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/src/panpipelines/nodes/atlascreate.py` & `panpipelines-0.9.9/src/panpipelines/nodes/atlascreate.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/src/panpipelines/nodes/basil.py` & `panpipelines-0.9.9/src/panpipelines/nodes/basil.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,14 +88,18 @@
     if not fmapjson:
         fmapjson = os.path.join(fieldmap_dir,f"sub-{subject}_ses-{session}_desc-preproc_fieldmap.json")
         fmapdict={}
         if fmap_mode == "phasediff":
             fmapdict["RawSources"] = getPhaseDiffSources(bids_dir,subject,session)
             fmapdict["Units"] = "Hz"
             export_labels(fmapdict,fmapjson)
+        elif fmap_mode == "pepolar":
+            fmapdict["RawSources"] = getPepolarSources(bids_dir,subject,session)
+            fmapdict["Units"] = "Hz"
+            export_labels(fmapdict,fmapjson)
 
     return process_fmriprep_fieldmap(fieldmap_dir,layout, asljson , asl_acq, basil_dict, labels_dict, command_base, work_dir,fmap_mode=fmap_mode)
 
 
 def process_fmriprep_fieldmap(fmriprep_fieldmap_dir,layout, asljson , asl_acq, basil_dict, labels_dict, command_base, work_dir,fmap_mode="fmriprep"):
     IFLOGGER.info(f"Preparing fieldmap from {fmap_mode} for use in SDC.")
     fmap = getGlob(os.path.join(fmriprep_fieldmap_dir,"*desc-preproc_fieldmap.nii.gz"))
@@ -447,18 +451,18 @@
         for basil_tag, basil_value in basil_dict.items():
             if "--" in basil_tag and "---" not in basil_tag:
                 if basil_value == IS_PRESENT:
                     params=params + " " + basil_tag
                 elif basil_value == IGNORE:
                     IFLOGGER.info(f"Parameter {basil_tag} is being skipped. This has been explicitly required in configuration.")
                 else:
-                    params = params + " " + basil_tag+"="+basil_value
+                    params = params + " " + basil_tag+"=" + str(basil_value)
 
             elif "-" in basil_tag and "--" not in basil_tag:
-                params = params + " " + basil_tag + " " + basil_value
+                params = params + " " + basil_tag + " " + str(basil_value)
 
             else:
                 print(f"Basil tag {basil_tag} not valid.")
 
 
         command=f"{command_base} oxford_asl"\
             " "+params
```

### Comparing `panpipelines-0.9.8/src/panpipelines/nodes/collate_csv_group.py` & `panpipelines-0.9.9/src/panpipelines/nodes/collate_csv_group.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/src/panpipelines/nodes/collate_csv_single.py` & `panpipelines-0.9.9/src/panpipelines/nodes/collate_csv_single.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/src/panpipelines/nodes/dummy.py` & `panpipelines-0.9.9/src/panpipelines/nodes/dummy.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/src/panpipelines/nodes/fmriprep.py` & `panpipelines-0.9.9/src/panpipelines/nodes/fmriprep.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/src/panpipelines/nodes/freesurfer.py` & `panpipelines-0.9.9/src/panpipelines/nodes/freesurfer.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/src/panpipelines/nodes/fslanat.py` & `panpipelines-0.9.9/src/panpipelines/nodes/fslanat.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/src/panpipelines/nodes/glm_randomize_group.py` & `panpipelines-0.9.9/src/panpipelines/nodes/glm_randomize_group.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/src/panpipelines/nodes/lst.py` & `panpipelines-0.9.9/src/panpipelines/nodes/lst.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/src/panpipelines/nodes/noddi.py` & `panpipelines-0.9.9/src/panpipelines/nodes/noddi.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/src/panpipelines/nodes/parse_textdata.py` & `panpipelines-0.9.9/src/panpipelines/nodes/parse_textdata.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/src/panpipelines/nodes/qsiprep.py` & `panpipelines-0.9.9/src/panpipelines/nodes/qsiprep.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/src/panpipelines/nodes/roi_extract.py` & `panpipelines-0.9.9/src/panpipelines/nodes/roi_extract.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/src/panpipelines/nodes/roi_mean_group.py` & `panpipelines-0.9.9/src/panpipelines/nodes/roi_mean_group.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/src/panpipelines/nodes/roi_mean_single.py` & `panpipelines-0.9.9/src/panpipelines/nodes/roi_mean_single.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/src/panpipelines/nodes/tensor.py` & `panpipelines-0.9.9/src/panpipelines/nodes/tensor.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/src/panpipelines/pipelines/aslprep_panpipeline.py` & `panpipelines-0.9.9/src/panpipelines/pipelines/aslprep_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/src/panpipelines/pipelines/basil_panpipeline.py` & `panpipelines-0.9.9/src/panpipelines/pipelines/basil_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/src/panpipelines/pipelines/collatecsv_panpipeline.py` & `panpipelines-0.9.9/src/panpipelines/pipelines/collatecsv_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/src/panpipelines/pipelines/collatecsvgroup_panpipeline.py` & `panpipelines-0.9.9/src/panpipelines/pipelines/collatecsvgroup_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/src/panpipelines/pipelines/dummy_panpipeline.py` & `panpipelines-0.9.9/src/panpipelines/pipelines/dummy_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/src/panpipelines/pipelines/fmriprep_panpipeline.py` & `panpipelines-0.9.9/src/panpipelines/pipelines/fmriprep_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/src/panpipelines/pipelines/freesurfer_panpipeline.py` & `panpipelines-0.9.9/src/panpipelines/pipelines/freesurfer_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/src/panpipelines/pipelines/lst_panpipeline.py` & `panpipelines-0.9.9/src/panpipelines/pipelines/lst_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/src/panpipelines/pipelines/noddi_panpipeline.py` & `panpipelines-0.9.9/src/panpipelines/pipelines/noddi_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/src/panpipelines/pipelines/panpipeline.py` & `panpipelines-0.9.9/src/panpipelines/pipelines/panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/src/panpipelines/pipelines/preproc_panpipeline.py` & `panpipelines-0.9.9/src/panpipelines/pipelines/preproc_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/src/panpipelines/pipelines/qsiprep_panpipeline.py` & `panpipelines-0.9.9/src/panpipelines/pipelines/qsiprep_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/src/panpipelines/pipelines/roiextract_panpipeline.py` & `panpipelines-0.9.9/src/panpipelines/pipelines/roiextract_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/src/panpipelines/pipelines/tensor_panpipeline.py` & `panpipelines-0.9.9/src/panpipelines/pipelines/tensor_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/src/panpipelines/pipelines/textmeasures_panpipeline.py` & `panpipelines-0.9.9/src/panpipelines/pipelines/textmeasures_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/src/panpipelines/pipelines/volmeasures_panpipeline.py` & `panpipelines-0.9.9/src/panpipelines/pipelines/volmeasures_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/src/panpipelines/scripts/aslprep_panscript.py` & `panpipelines-0.9.9/src/panpipelines/scripts/aslprep_panscript.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/src/panpipelines/scripts/fmriprep_panscript.py` & `panpipelines-0.9.9/src/panpipelines/scripts/fmriprep_panscript.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/src/panpipelines/scripts/mne_make_surfaces.py` & `panpipelines-0.9.9/src/panpipelines/scripts/mne_make_surfaces.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/src/panpipelines/scripts/pancontainer_panscript.py` & `panpipelines-0.9.9/src/panpipelines/scripts/pancontainer_panscript.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/src/panpipelines/scripts/panscript.py` & `panpipelines-0.9.9/src/panpipelines/scripts/panscript.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/src/panpipelines/scripts/sdcflows_fieldmap.py` & `panpipelines-0.9.9/src/panpipelines/scripts/sdcflows_fieldmap.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,17 +12,41 @@
 
 def parse_params():
     parser = ArgumentParser(description="SDCflows fieldmap workflow")
     parser.add_argument("--fmap_sources", nargs="+", help="Fmap sources")
     parser.add_argument("--subject", help="Subject")
     parser.add_argument("--session", help="Session")
     parser.add_argument("--fieldmap_dir", type=Path, help="Fieldmap directory")
-    parser.add_argument("--workdir", type=Path, help="Workflow directort")
+    parser.add_argument("--workdir", type=Path, help="Workflow directory")
+    parser.add_argument("--fmap_mode", help="Fieldmap type",default="phasediff")
     return parser
 
+def sdcflows_pepolar_fieldmap(fmap_sources, subject, session,fieldmap_dir,workdir):
+    estimator = sfm.FieldmapEstimation (
+        sources = fmap_sources
+    )
+
+    pepolar_wf = estimator.get_workflow()
+
+    fm_wf = Workflow(name = "sdcflows_pepolar_wf", base_dir=workdir)
+    sinker = Node(DataSink(),name='fmap_sink')
+    sinker.inputs.base_directory = os.path.dirname(fieldmap_dir)
+    sinker.inputs.substitutions = [
+        ('reoriented',f"sub-{subject}_ses-{session}_desc-preproc_fieldmap"),
+        ('dir-AP_epi_average_merged_padded_sliced_volreg_base_fieldcoef_fixed',f"desc-coeff_fieldmap"),
+        ('clipped',f"sub-{subject}_ses-{session}_desc-magnitude_fieldmap")
+    ]
+    basename = os.path.basename(fieldmap_dir)
+    fm_wf.connect( pepolar_wf,"outputnode.fmap",sinker,f"{basename}")
+    fm_wf.connect( pepolar_wf,"outputnode.fmap_coeff",sinker,f"{basename}.@coeff")
+    fm_wf.connect( pepolar_wf,"outputnode.fmap_mask",sinker,f"{basename}.@mask")
+    fm_wf.connect( pepolar_wf,"outputnode.fmap_ref",sinker,f"{basename}.@ref")
+
+    fm_wf.run()
+
 def sdcflows_phdiff_fieldmap(fmap_sources, subject, session,fieldmap_dir,workdir):
     estimator = sfm.FieldmapEstimation (
         sources = fmap_sources
     )
 
     phdiff_wf = estimator.get_workflow()
 
@@ -45,15 +69,20 @@
     parser=parse_params()
     args, unknown_args = parser.parse_known_args()
     fmap_sources = args.fmap_sources
     subject = args.subject
     session = args.session
     fieldmap_dir = str(args.fieldmap_dir)
     workdir = str(args.workdir)
+    fmap_mode = args.fmap_mode
 
-    sdcflows_phdiff_fieldmap(fmap_sources, subject, session,fieldmap_dir,workdir)
+    if fmap_mode == "phasediff":
+        sdcflows_phdiff_fieldmap(fmap_sources, subject, session,fieldmap_dir,workdir)
+    elif fmap_mode == "pepolar":
+        sdcflows_pepolar_fieldmap(fmap_sources, subject, session,fieldmap_dir,workdir)
+        
 
 # This is the standard boilerplate that calls the main() function.
 if __name__ == '__main__':
     main()
```

### Comparing `panpipelines-0.9.8/src/panpipelines/utils/transformer.py` & `panpipelines-0.9.9/src/panpipelines/utils/transformer.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/src/panpipelines/utils/util_functions.py` & `panpipelines-0.9.9/src/panpipelines/utils/util_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1811,15 +1811,27 @@
                     LOGGER.info(f"Container not defined for {nodename} node. Required commands should be accessible on local path for pipeline to succeed")
                     if container_run_options:
                         LOGGER.info(f"Note that '{container_run_options}' set as run options for non-existing container. This may cause the pipeline to fail.")
                     
                     if container_prerun:
                         LOGGER.info(f"Note that '{container_prerun}' set as pre-run options for non-existing container. This may cause the pipeline to fail.")
 
-    command_base = f"{container_run_options} {container} {container_prerun}"
+
+    # replace None by empty string
+    if container is None:
+        container=""
+    
+    if container_run_options is None:
+        container_run_options=""
+
+    if container_prerun is None:
+        container_prerun=""
+
+    command_base = f"{container_run_options} {container} {container_prerun} "
+    command_base = command_base.lstrip()
     LOGGER.info("Container base run command is:")
     LOGGER.info(f"{command_base}")
 
     return command_base, container
 
 def runCommand(command,LOGGER=UTLOGGER,suppress="",interactive=False):
     if suppress:
@@ -1849,12 +1861,19 @@
         if "acquisition" in entities.keys():
             acq = "acq-" + entities["acquisition"]
         else:
             acq = get_bidstag("acq",bidsfile.filename)
 
     return acq
 
-def getPhaseDiffSources(bids_dir,participant_label,participant_session=None,datatype="fmap",suffix=['phase1','phase2','magnitude1','magnitude2','phasediff','magnitude'],extension="nii.gz"):   
+def getPhaseDiffSources(bids_dir,participant_label,participant_session=None,acquisition=None,datatype="fmap",suffix=['phase1','phase2','magnitude1','magnitude2','phasediff','magnitude'],extension="nii.gz"):   
+    layout = BIDSLayout(bids_dir)
+    bidslist = layout.get(return_type='file',subject=participant_label,session=participant_session,acquisition=acquisition,datatype=datatype,suffix=suffix,extension=extension)
+
+    return bidslist
+
+
+def getPepolarSources(bids_dir,participant_label,participant_session=None,acquisition="fmri",datatype="fmap",suffix=['epi'],extension="nii.gz"):   
     layout = BIDSLayout(bids_dir)
-    bidslist = layout.get(return_type='file',subject=participant_label,session=participant_session,datatype=datatype,suffix=suffix,extension=extension)
+    bidslist = layout.get(return_type='file',subject=participant_label,session=participant_session,acquisition=acquisition,datatype=datatype,suffix=suffix,extension=extension)
 
     return bidslist
```

### Comparing `panpipelines-0.9.8/src/panpipelines/workflows/aslprep_workflow.py` & `panpipelines-0.9.9/src/panpipelines/workflows/aslprep_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/src/panpipelines/workflows/basil_workflow.py` & `panpipelines-0.9.9/src/panpipelines/workflows/basil_workflow.py`

 * *Files 22% similar despite different names*

```diff
@@ -54,16 +54,28 @@
             # we have to mnanually substitute items from DICTs until we also check these in update_labels
             SDCFLOWS_FMAP_DIR=substitute_labels(SDCFLOWS_FMAP_DIR,labels_dict)
     
             SDCFLOWS_FMAP_MODE = getParams(labels_dict,"SDCFLOWS_FIELDMAP_MODE") 
             if SDCFLOWS_FMAP_MODE:
                 sdcflows_fmap_mode = SDCFLOWS_FMAP_MODE
             else:
+                sdcflows_fmap_mode="phasediff"          
+
+            use_pepolar_fmap = getParams(labels_dict,'USE_PEPOLAR_FMAP')
+            if use_pepolar_fmap and participant_label in use_pepolar_fmap:
+                sdcflows_fmap_mode="pepolar"
+            elif use_pepolar_fmap and f"{participant_label}_{participant_session}" in use_pepolar_fmap:
+                sdcflows_fmap_mode="pepolar"
+
+            use_phasediff_fmap = getParams(labels_dict,'USE_PHASEDIFF_FMAP')
+            if use_phasediff_fmap and participant_label in use_phasediff_fmap:
                 sdcflows_fmap_mode="phasediff"
-                labels_dict = updateParams(labels_dict,"SDCFLOWS_FIELDMAP_MODE",sdcflows_fmap_mode)
+            elif use_phasediff_fmap and f"{participant_label}_{participant_session}" in use_phasediff_fmap:
+                sdcflows_fmap_mode="phasediff"
+            labels_dict = updateParams(labels_dict,"SDCFLOWS_FIELDMAP_MODE",sdcflows_fmap_mode)
             
             sdcflows_workdir = os.path.dirname(SDCFLOWS_FMAP_DIR)
             if not os.path.exists(sdcflows_workdir):
                 os.makedirs(sdcflows_workdir)
 
             sdcflows_fmap_parentdir = os.path.dirname(SDCFLOWS_FMAP_DIR)
             if not os.path.exists(sdcflows_fmap_parentdir):
@@ -74,14 +86,25 @@
                 sources = getPhaseDiffSources(bids_dir,participant_label,participant_session)
                 sources_String = " ".join(sources)
                 params = f"--fmap_sources {sources_String}" \
                     f" --subject {participant_label}" \
                     f" --session {participant_session}" \
                     f" --fieldmap_dir {SDCFLOWS_FMAP_DIR }" \
                     f" --workdir {sdcflows_workdir}"
+            elif sdcflows_fmap_mode == "pepolar":               
+                sources = getPepolarSources(bids_dir,participant_label,participant_session)
+                sources_String = " ".join(sources)
+                params = f"--fmap_sources {sources_String}" \
+                    f" --subject {participant_label}" \
+                    f" --session {participant_session}" \
+                    f" --fieldmap_dir {SDCFLOWS_FMAP_DIR }" \
+                    f" --workdir {sdcflows_workdir}" \
+                    f" --fmap_mode {sdcflows_fmap_mode}"
+            elif LOGGER:
+                    LOGGER.warn(f"{sdcflows_fmap_mode} not recognized as a field map option.")                
 
             if sources:
                 SDCFLOWS_CONTAINER_TO_USE = getParams(labels_dict,"SDCFLOWS_CONTAINER_TO_USE")
                 if SDCFLOWS_CONTAINER_TO_USE:
                     panscript = pancontainer_script.pancontainer_panscript(labels_dict,params=params,command=f"python {sdcflows_fieldmap.__file__}",container_img=SDCFLOWS_CONTAINER_TO_USE)
                 else: 
                     panscript = pancontainer_script.pancontainer_panscript(labels_dict,params=params,command=f"python {sdcflows_fieldmap.__file__}")
```

### Comparing `panpipelines-0.9.8/src/panpipelines/workflows/collatecsv_workflow.py` & `panpipelines-0.9.9/src/panpipelines/workflows/collatecsv_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/src/panpipelines/workflows/collatecsvgroup_workflow.py` & `panpipelines-0.9.9/src/panpipelines/workflows/collatecsvgroup_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/src/panpipelines/workflows/dummy_workflow.py` & `panpipelines-0.9.9/src/panpipelines/workflows/dummy_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/src/panpipelines/workflows/fmriprep_workflow.py` & `panpipelines-0.9.9/src/panpipelines/workflows/fmriprep_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/src/panpipelines/workflows/freesurfer_workflow.py` & `panpipelines-0.9.9/src/panpipelines/workflows/freesurfer_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/src/panpipelines/workflows/lst_workflow.py` & `panpipelines-0.9.9/src/panpipelines/workflows/lst_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/src/panpipelines/workflows/noddi_workflow.py` & `panpipelines-0.9.9/src/panpipelines/workflows/noddi_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/src/panpipelines/workflows/preproc_workflow.py` & `panpipelines-0.9.9/src/panpipelines/workflows/preproc_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/src/panpipelines/workflows/qsiprep_workflow.py` & `panpipelines-0.9.9/src/panpipelines/workflows/qsiprep_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/src/panpipelines/workflows/roiextract_workflow.py` & `panpipelines-0.9.9/src/panpipelines/workflows/roiextract_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/src/panpipelines/workflows/tensor_workflow.py` & `panpipelines-0.9.9/src/panpipelines/workflows/tensor_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/src/panpipelines/workflows/textmeasures_workflow.py` & `panpipelines-0.9.9/src/panpipelines/workflows/textmeasures_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/src/panpipelines/workflows/volmeasures_workflow.py` & `panpipelines-0.9.9/src/panpipelines/workflows/volmeasures_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/.gitignore` & `panpipelines-0.9.9/.gitignore`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/LICENSE` & `panpipelines-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/README.md` & `panpipelines-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/pyproject.toml` & `panpipelines-0.9.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.8/PKG-INFO` & `panpipelines-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: panpipelines
-Version: 0.9.8
+Version: 0.9.9
 Summary: MRI Processing Pipelines for PAN Healthy Minds for Life Study
 Project-URL: Homepage, https://github.com/MRIresearch/PANpipelines
 Project-URL: Bug Tracker, https://github.com/MRIresearch/PANpipelines/issues
 Author-email: Chidi Ugonna <chidiugonna@arizona.edu>
 License: MIT License
         
         Copyright (c) 2023 MRIresearch
```

