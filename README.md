# Predicting Turbidity in Lake Superior



## Objective
The purpose of this project is to investigate the water quality of Lake Superior. We chose to predict turbidity because high turbidity can significantly reduce the aesthetic quality of any body of water. 

## Data Source 
NOAA’s National Estuarine Research Reserve System identifies and tracks short-term variability and long-term changes in the integrity and biodiversity of representative estuarine ecosystems and coastal watersheds for the purpose of contributing to effective national, regional and site-specific coastal zone management.Our team chose to look at water quality at the Barker’s Island station with weather data from the Pokegama Bay in Lake Superior and used the available water quality data, meteorlogical data, and nutrient and pigment data to creata a machine learning model to predict turbidity.

![image](https://github.com/keywalsh/National_Estuarine_Research_Reserve/assets/119438532/ad3cd092-d072-4146-b6b2-3ddc2cbae116)
![image](https://github.com/keywalsh/National_Estuarine_Research_Reserve/assets/119438532/94213cf4-b7b7-4a78-a603-0ad079697515)


## Data Model Implementation

### K-Nearest Neighbors
We initially used K-Nearest Neighbors (KNN) Classification tested a regression model to predict 2023 turbidity from the data from 2018 – 2022. We used the following data:

Average Air Temperature, 
Total Precipitation,
Water Temperature,
Salinity,
Depth Measured,
and pH

This was not very effective at predicting turbidity. Our instructor suggested trying either Logistic Regression or Random Forest.

### Random Forest Model
Random Forest was a much better model for our data. We were quickly able to see which data was more important and then could replace lesser important data with other data to see which one was more important.

### Model Optimization
Four models were created. The models were optimized by refining and updating the input data based on feature importances. Model 2 was the highest performing model with a 0.95 accuracy F-1 Score. The data features included in Model 2 were month, water temperature, depth, pH and chlorophyll fluorescence.

![image](https://github.com/keywalsh/National_Estuarine_Research_Reserve/assets/119438532/c8003a8a-fe30-4a71-af4f-6ba5710d09c4)


## Files

Raw data contained within the Bakers_Island_Data folder 

Predictions folder contains:    

Data cleaning files   
-data_cleaning_notebook.ipynb  
-PySpark_Summer.ipynb  

Cleaned CSV files  
-cleaned.csv  
-cleaned_groupby_date.csv  
-summer_all_days.csv  
-summer_groupby_date.csv  

Model optimization files  
-model_1_random_forest.ipynb  
-model_2_random_forest.ipynb  
-model_3_random_forest.ipynb  
-model_4_random_forest.ipynb  

Resource folder contains: 

-non-merged datasets used for initial understanding and scoping of analysis 

Barkers_Island_Data:

-merged csv used in analysis and supporting metadata details for data included in csv.

Visualizations used in presentation:

https://public.tableau.com/views/Turbidityandwaterfeaturesovertime/Dashboard3?:language=en-US&publish=yes&:display_count=n&:origin=viz_share_link

https://public.tableau.com/app/profile/eugenia.volscaia/viz/WaterQuality

## Presentation 
https://docs.google.com/presentation/d/16jH0MtC1k8bn-wj_fRicU09ObhF5Fw55vKubftov-gI/edit#slide=id.p1

## Contributing Members

Robert Bentz, Colleen Karwoski, Laura Murray, Eugenia Volscaia and Katelyn Walsh

## Data Source
NOAA National Estuarine Research Reserve System (NERRS). System-wide Monitoring Program. Data accessed from the NOAA NERRS Centralized Data Management Office website: http://www.nerrsdata.org; accessed 1 June 2023.


