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
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTA5NDM0MTYxNF19
-->
