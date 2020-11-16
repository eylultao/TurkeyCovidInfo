# TurkeyCovidInfo
Turkey has not been transparent with its covid data since the beginning of pandemic. This repo will be a naive attempt to make sense of the limited available data and make a prediction for the population parameter


# Data Source
## Daily number of deaths in Istanbul:
Data is scraped from Istanbul Municipality website https://www.turkiye.gov.tr/istanbul-buyuksehir-belediyesi-vefat-sorgulama by Yaprak Özışık for Sarkac.
The dataset originally included valuable information such as age of the deceased and cause of death. These columns have mysteriously vanished after the pandemic, and are no longer available to the public.
https://sarkac.org/2020/11/istanbulda-haftalik-vefat-sayilari/ 
## Daily Cases:
The initial intention was to use the data shared by turkish gov, but it is speculated to be heavily manipulated, so I will use the ECDC data (even though they also have to use the numbers shared by Turkish Gov, I believe having access to other countries' data will be a good method to validate the accuracy and demonstrate how "likely" it is that the Turkish data is accurate.)

Data Published by: European Centre for Disease Prevention and Control (ECDC)
https://www.ecdc.europa.eu/en/publications-data/download-todays-data-geographic-distribution-covid-19-cases-worldwide

# Whats wrong with the data disclosed by the Turkish Gov?
Turkeys definiton of a "Case" has not been consistent with the rest of the World. 
WHO defines daily new cases as number of patients who tested positive. Turkish citizens were initially under the assumption that "the daily number of new cases" shared by the ministery of health were also reflecting the number of daily positive test results. It became apparent in Sep 30, 2020 that these numbers were only reflecting the "number of daily sick cases" which lightly implies that Turkey only accounts for people who tested posivite and has symptoms.
In other words, 

WHO definition:
if(isPositive) numCases++;

Turkish definition:
if(isPositive & hasSymptoms) numCases++;


https://www.aa.com.tr/en/latest-on-coronavirus-outbreak/turkey-measures-taken-against-false-covid-19-info/1984375

"Her vaka hasta degildir" roughly translated as: "Not all cases are sick people" 
https://www.aa.com.tr/tr/koronavirus/saglik-bakani-koca-her-vaka-hasta-degildir/1991187
