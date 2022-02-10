[![License](https://img.shields.io/badge/License-GPL%203.0-green)](https://opensource.org/licenses/GPL-3.0)

# cancer-trial-match
These files derive data for cancer clinical trials, plus web viewer to visualise results.  

Mappings between synonyms (cancer types specified in clinicaltrials.gov condition.name field) and controlled cancer types are specified by the file conditionSynonyms4.csv.  

List of human genes and their synonyms is downloaded from https://www.ncbi.nlm.nih.gov/gene  

The script trialMatchDataRefresh.Rmd generates data - it is recommended to run this script daily to ensure data remain as current as possible.  

Data are ingested and visualised using the script TRIAL_MATCH_SHINY.Rmd.  

The file trialMatchConfiguration.json includes configuration details - a username and password for a Clinical Trials Transformation Initiative account, and a contact email for web viewer will need to be added to this file before running.  

