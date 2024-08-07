[![License](https://img.shields.io/badge/License-GPL%203.0-green)](https://opensource.org/licenses/GPL-3.0)

# cancer-trial-match  
  
## Contents
  
This repository contains R files to derive data for cancer clinical trials, plus web viewer to visualise results.  
  
The following files are required to derive data and deploy web viewer:  
* **trialMatchConfiguration.json:**	configuration file, defines values for country/countries, contact information, "about us" description and privacy policy
	* if configuring for >1 country, separate country names by commas (e.g. Switzerland, France)
* **conditionSynonyms6.csv:**  	defines mappings between cancer types of interest and condition names (as used by clinicaltrials.gov)  
* **digitalECMTlogo48px.PNG:**	icon for digital Experimental Cancer Medicine Team (creators of this tool)  
* **indexTrialData.Rmd:**		R script to download and store data required by user interface  
	* a username and password for a Clinical Trials Transformation Initiative account
	* see https://aact.ctti-clinicaltrials.org/ for how to create an account  
	* it is recommended to run this script daily to ensure all data remain as current as possible  
	* configurable by country according to the country specified in configuration file  
* **TRIAL_MATCH_SHINY.Rmd:**		R Shiny app, provides an interface to query and display trial data  
	* parameters may be passed via URL, for example if linking out from a patient electronic health record
* **trial_report.Rmd:**			R script for downloading and storing results as a static html file  


