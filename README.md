# Data-Science-Capstone-Project

## Summary of methodologies
### 1. Data Collection through API 
Used the get request to the SpaceX API to collect data, clean the requested data and did some basic data wrangling and formatting.
### 2. Data Collection with Web Scraping 
Applied web scrapping to webscrap Falcon 9 launch records with BeautifulSoup. Parsed the table and converted it into a pandas dataframe.
### 3. Data Wrangling
Performed exploratory data analysis and determined the training labels. Calculated the number of launches at each site, and the number and occurrence of each orbits. Created landing outcome label from outcome column and exported the results to csv.
### 4. Exploratory Data Analysis with SQL
Loaded the SpaceX dataset into a PostgreSQL database without leaving the jupyter notebook. Applied EDA with SQL to get insight from the data. Wrote queries to find out for instance:
  - The names of unique launch sites in the space mission.
  - The total payload mass carried by boosters launched by NASA (CRS)
  - The average payload mass carried by booster version F9 v1.1
  - The total number of successful and failure mission outcomes
  - The failed landing outcomes in drone ship, their booster version and launch site names.
### 5. Exploratory Data Analysis with Data Visualization: 
Explored the data by visualizing the relationship between flight number and launch Site, payload and launch site, success rate of each orbit type, flight number and orbit type, the launch success yearly trend.
### 6. Interactive Visual Analytics with Folium: 
Marked all launch sites, and added map objects such as markers, circles, lines to mark the success or failure of launches for each site on the folium map. Assigned the feature launch outcomes (failure or success) to class 0 and 1.i.e., 0 for failure, and 1 for success. Using the color-labeled marker clusters, identified which launch sites have relatively high success rate. Calculated the distances between a launch site to its proximities. Answered some question for instance:
  - Are launch sites near railways, highways and coastlines.
  - Do launch sites keep certain distance away from cities.
### 7. Prective Analysis (Classification):
Loaded the data using numpy and pandas, transformed the data, split our data into training and testing. Built different machine learning models and tune different hyperparameters using GridSearchCV. Used accuracy as the metric for our model, improved the model using feature engineering and algorithm tuning and found the best performing classification model.
### 8. Dashboard using Plotly:
Built an interactive dashboard with Plotly dash. Plotted pie charts showing the total launches by a certain sites. Plotted scatter graph showing the relationship with Outcome and Payload Mass (Kg) for the different booster version.


## Project background and context
Space X advertises Falcon 9 rocket launches on its website with a cost of 62 million dollars; other providers cost upward of 165 million dollars each, much of the savings is because Space X can reuse the first stage. Therefore, if we can determine if the first stage will land, we can determine the cost of a launch. This information can be used if an alternate company wants to bid against space X for a rocket launch. This goal of the project is to create a machine learning pipeline to predict if the first stage will land successfully.

## Problems you want to find answers
1. What factors determine if the rocket will land successfully?
2. The interaction amongst various features that determine the success rate of a successful landing.
3. What operating conditions needs to be in place to ensure a successful landing program.

