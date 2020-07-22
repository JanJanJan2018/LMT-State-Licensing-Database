This folder is the original, some folders are created when you run the scripts. You have to run all the scripts separately in the three folders: 

- Alternate Jobs Each State Indeed
- apartments Dot Com
- number of businesses

They are from Indeed.com, apartments.com, and yellopages.com respectively.

Also, the folder, 'Over Time Changes' has periodic snap shots of the changes over time in this table with updated data by date. The Zillow file in these folders is different than the one in this folder. 

The latest Zillow home values, that changes monthly to add the last completed month to the time series for monthly values, is the 
"Zip_zhvi_bdrmcnt_2_uc_sfrcondo_tier_0.33_0.67_sm_sa_mon.csv" file, the zillow script for "copy-find3zillowCitiesFunctionMean2BRHomeValues.Rmd" file will use this downloaded zillow file to get the mean of the three top populated cities in each state.

The "Find3TopCitiesEachState.Rmd" file is the script to get the three top populated cities in each state, I want to modify and duplicated this Rmd file to extract the 10 top populated cities, but didn't do anything with it other than create a table with the 10 most populated cities in it. I would like to adjust all scripts from the three folders above to get the jobs available with salary, 2BR prices, the zillow 2BR home values in the script not folder, and the number of businesses from 10 cities instead of 3, but need a work around for the three arguments of the functions used in scraping data to loop, list/table apply for 2-3 arguments depending on if it is Indeeds or yellowpages irrespectively. I could manually just write the individual functions for all 500+ in each script, but that is tedious. Depending on options, I might do that.

Also note, that the "dataGovEthnicAgeDemos.Rmd" file puts all tables together and adds the demographic information from data.census.gov for 2018 as the latest median income for each state, and also the demographics for each state. Those tables have to be built with maps inside their site and downloaded. That site isn't scraped, same as with Zillow's 2BR house prices timeline data. The "copy-indeed_webscrape_funciton-altered.Rmd" file creates the original LMT jobs available and salary information, and puts those columns in the table before the later scripts in the 'Alternate Jobs Each State Indeed', that creates a 'statesRates.csv' table to use in the "dataGovEthnicAgeDemos.Rmd' file. Also, that file creates the 'stateLicensingRequirementsUpdatedandAdded.csv' file but uses the stateLicensingRequirements.csv file that the new added info for state licensing requirements is updated and added to before running the dataGov... Rmd file.

