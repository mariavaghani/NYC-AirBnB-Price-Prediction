# NYC AirBnB Price Prediction
Repository containing Python script to predict prices for AirBnb listings in NYC based on the listing details, host characteristics, and location

# Installation

The notebook uses Python Python 3.6.9. Other libraries used within the code are:

Data Analysis

-   numpy (1.19.5)
-   pandas (1.1.5)
-   sklearn (0.22.2.post1)

Data Visualization

-   matplotlib (3.3.4)
-   seaborn (0.11.1)
-   cufflinks (0.17.3)
-   plotly (4.14.3)

Others:
-   pprint (3.9.2)
-   datetime (3.9.2)
-   time (3.9.2)
-   geopy (2.1.0)
-   Scipy (1.4.0)

The main code for this project is divided into chapters. The second chapter deals with importing datasets that would be used in this project: Open_Air_bnb dataset, most visited tourist places in New York City taken as a table from a wikipedia page, and major NYC airports.
The Open_Air_bnb is a modified dataset with an added feature - proximity to the closest subway station. The method to obtain this feature is describes in the very last chapter: 'Prep that was done one time, downloaded and used as an input'. This step takes a very long time, like hours (any suggestions how to speed this step up is very welcome). it was performed once, downloaded, and used as input for the analysis. If you already have the dataset with the "proximity to the closest subway station" feature (included in the repository), you do not need to run the code from the last chapter. But in case you need it - it is there.

# Project motivation
The model tries to predict a nightly price based on listing details, host characteristics, and location and proximity to landmarks. Using this model Airbnb could suggest host recommended prices for their listings. Having the most optimal prices, hosts could rent out more listings, which would generate more profit to Airbnb.

# File Description
The files included in this project are:

- Open_AirBnB_data.ipynb - Jupyter Notebook including the main project code.

Data folder:
- AB_NYC_2019.csv - the origianl csv file downloaded from [Kaggle](https://www.kaggle.com/dgomonov/new-york-city-airbnb-open-data)
- AIRPORT_POINT.xlsx - xlsx file containing airport locations in NYC. taken from [data.gov](https://catalog.data.gov/en_AU/dataset/airport-point). [This wikipedia](https://en.wikipedia.org/wiki/Newark_Liberty_International_Airport) was used to add Newark airport manually.
- Top_attractions_nyc.xlsx - xlsx containing list of top NYC landmarks. taken from [wikipedia](https://en.wikipedia.org/wiki/Tourism_in_New_York_City)
- NYC_Transit_Subway_Entrance_And_Exit_Data.csv - csv files containing data on NYC subway exits. taken from [kaggle](NYC_Transit_Subway_Entrance_And_Exit_Data.csv)
- Open_Airbnb_ver.1.csv - modified csv containing the original data and proximity to the nearest subway exit feature

# Project Summary
This project aims to predict daily price for each Airbnb listing in NYC based on listing features. Since I was provided with location data, I decided to take a closer look at how this information could be used. Before living in NYC, I was coming to visit and I still remember what my criteria were for choosing the right place to stay and with that - the price I was willing to pay. Reconstructing mindset of a tourist is the key to build the ML model. What is important when you are a tourist in a new city? How am I going to get to the place from airport, how easy it would be commute to most famous landmarks and how close I am to said landmarks? These questions determined three features: proximity to the nearest airport, proximity to the nearest subway station, and distance to most famous landmarks.
The proximity to the nearest subway station feature was rendered once and later imported into the script for the sake of saving runtime. 
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTA5NDM0MTYxNF19
-->
