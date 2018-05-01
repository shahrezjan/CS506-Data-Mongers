# CS506-Data-Mongers
CS506 Project 

#### Data_Exploration.ipynb
This file was used as part of our initial data exploratory analysis. The script begins by parsing our data and converting it to a dataframe, where missing fields were replaced with “None” and additional boolean columns were added to indicate if a particular contact field was missing.

#### We used this dataframe to create a couple of bar graphs to observe some interesting findings including the distribution of license violation types and the distribution of missing contact information. Additionally, we found information regarding any ownership groups that may exist and how many violations they have obtained. 

Since we decided to perform logistic regression based on the distribution of missing contact information, we later added the regression code into this file. 

#### get_coords.ipynb
Python libraries required: geopy
This script gets the latitude and longitude coordinates for all the labor brokers and a boolean value to represent whether or not each broker had a license violation. The results were written to three different csv files (all_places.csv, negative_statuses.csv, and positive_statuses.csv) and were used to create our map visualizations.

Five different API keys for the Google Maps API were used in order to not violate daily usage limits. 

#### get_status_types.ipynb
Python libraries required: geopy
This script gets the latitude and longitude coordinates for all labor brokers with a license violation, and it grabs the type of license violation that each broker has listed (ex: Banned Forever). The results were written to a csv file (places_and_status_types.csv) and were used to create a map visualization. 

Five different API keys for the Google Maps API were used in order to not violate daily usage limits. 

#### ThrillerInManilla.ipynb
Python Libraries required: gmaps

pip install gmaps

This script will install the library we used to make the google maps visualizations.

Load jupyter extension:
jupyter nbextension enable --py --sys-prefix gmaps
This script will load the jupyter extension required to view the google map visualizations inside jupyter notebook.
