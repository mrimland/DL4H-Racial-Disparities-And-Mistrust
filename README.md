# DL4H-Racial-Disparities-And-Mistrust
The following python notebooks are meant to be run within Google Colab to reproduce the work found in [Racial Disparities and Mistrust in End-of-Life Care](https://proceedings.mlr.press/v85/boag18a/boag18a.pdf) (Boag et al. 2018)
[Original Code](https://github.com/wboag/eol-mistrust/tree/master)

## Data requirements
You should first attain credentials, the required training, and access to [MIMIC-III](https://physionet.org/content/mimiciii/1.4/) and to [MIMIC-IV](https://physionet.org/content/mimiciv/3.1/) This code was run on MIMIC-III version 1.4 and MIMIC-IV version 3.1

The notebooks expect the tables to be loaded into BigQuery. You should also replace any instance of project_id with your own project id for your Google Colab project

If you plan to run DisparityInMimic.ipynb, a few notes
1. Some columns/names are different between MIMIC-III and MIMIC-IV. Some columns to check are ethnicity:race, ventdurations:vent_durations, intime:icu_intime, outtime:icu_outtime, icu_stayid:stay_id, vasopressordurations:vasopressor_durations
2. If you plan to run DisparityInMimic.ipynb for MIMIC-IV, you can run GenerateVentVasoTables.ipynb to generate the necessary ventilation and vasopressor tables until these tables are officially derived directly from [MIMIC-IV](https://physionet.org/content/mimiciv/3.1/)
   

## Running

