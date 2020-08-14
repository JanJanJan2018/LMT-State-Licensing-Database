This folder is the original, some folders are created when you run the scripts. You have to run all the scripts separately in the three folders: 


- Find10TopCitiesEachState.Rmd or .R will pull the 10 most populated cities from the worldpopulation site for each state and create the table10cities.csv file, but I changed the file and it hasn't changed, so it will keep the same population a while and the file to use.
- Top 10 Cities (This folder is created when you run the script dataGovEthnicAgeDemos-editsAug 10-2020.Rmd file but uses table10cities-altered)
- Apartments 2BR (run the apts-com-2BR2BA.Rmd file in this folder to generate some files)
- The Zillow data is from zillow.com/research/data for the zip codes of multihome 2bedroom. Zip_zhvi_bdrmcnt_2_uc_sfrcondo_tier_0.33_0.67_sm_sa_mon
- Yellow Pages Businesses (folder that you run the Rmd scripts for each business class searched and it generates a folder with supplementary city listings and a larger combined csv file of the number of businesses per state based on the 10 cities per state table that is 'statesRates-...' for the business name searched. Time consuming for each business)
- Indeed 10 (folder that has the files to run on each job searching for pay and number of advertised listings to calculate, will create separate folders for each job, with supplementary files, and a combined output file that is 'jobListings_...' the job searched for the ellipses replacement. These scripts .Rmd are the 'TenCities_Indeed_5pages_jobListings-...' for the ellipse filled job listing.

Note that there may be minute errors and some other files generated. Didn't use timeout of httr setting or any of that confusing stuff to offset the loops ending with a timeout, and filled in time by manually reading in tables or combining them or having the loops do something before speedily downloading each search because it could kick the user off the site and it was good to let other user enjoy their site. No data governance was applied in reading terms of conditions, I assumed it was on the web, didn't need an API and they didn't kick my API off or have some blocker in place, or captchas in place and that implied freely available. Its not my data and I'm not selling it, and anybody can access the data from these sources. 

These sources are from Indeed.com, apartments.com, https://worldpopulationreview.com/states/cities/, and yellowpages.com 
