# Analyzing-Resale-Housing-Prices-with-Tableau
This repository contains a school project I submitted the module - Data Visualization. In this project, I was tasked to analyze the Housing Resale Prices in Singapore between 1990 - 2020 using the Tableau Software.

The dataset "Housing Resale Dataset.csv" included the housing resale prices in Singapore between 2012 - 2019 - this dataset was provided as part of the assignment. However, I found a similar dataset "resale prices from 1990-2020.csv" (The dataset included is in the "resale prices from 1990-2020.zip" file) in [Data.Gov](https://data.gov.sg/dataset/resale-flat-prices) and used that instead. The dataset included Housing Resale Prices from 1990 - 2020 and included the following attributes: 
 * Location
 * Flat Model
 * Floor Area (sqm)
 * Lease Commencement Date
 * Month of Resale
 * Resale Price (SGD)
 * Remaining Lease Duration
 * Storey Range
 * Street Name
 * Town

To complement my analysis, I included the following datasets: 
 * "uAddresses.csv" - includes the unique addresses of each housing location. To create this file, I used numpy and pandas to read and manipulate the data as well as urllib - to send a request to the url: http://py4e-data.dr-chuck.net/?json= (I learnt of this technique from the Coursera Specialization [Python for Everybody](https://www.coursera.org/specializations/python?skipBrowseRedirect=true)) - to transform the locations into latitude and longitude data.
 * "facillities.csv" - includes all the malls and their locations in Singapore, which i scrapped from [wikipedia](https://en.wikipedia.org/wiki/List_of_shopping_malls_in_Singapore) then fed into urllib, calling the api http://py4e-data.dr-chuck.net/?json= to transform it into lat and long. This is to evaluate housing price with respect to its proximity from Shopping Malls.
 * "mrt_lrt_info.csv" - MRT and LRT names and Locations, an additional resource provided by my then lecturer. This is to evaluate housing price with respect to its proximity from MRT/LRT stations.
