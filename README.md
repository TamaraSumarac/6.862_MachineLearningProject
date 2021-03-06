## 6.862 Applied Machine Learning Project


### Predicting energy consumption of a building based on historic usage rates and weather data 


#### Project motivation:

One of the biggest problems facing the world today is global warming. Production of carbon dioxide and other greenhouse gases is heating up the atmosphere and this could be very dangerous for human life. With electricity and heat production being one of the biggest contributors to the greenhouse gases, there is a demand in constructing a more energy-efficient buildings for our growing human population and increasing number of commercial buildings. In addition to creating new buildings, there is an interest in renovating existing buildings into a more energy- efficient ones. An estimate of how much energy would improved building consume relative to the old one can incentivize investors to pursue these renovations. For this purpose it is useful to have an accurate prediction of how much energy would a building consume in future given how much that same building was consuming in the past. 

In this project I used the data: https://www.kaggle.com/c/ashrae-energy-prediction/data of historic usage rates and observed weather over one year period across hundreads of buildings in order to predict how much energy would these buildings consume in the future. Buildings are labeled by their primary use (e.g. office, educational building), square footage and year they were built, and we have historic data on the usage of these buildings across the areas such as chilled water, electricity, hot water, and steam meters. In addition to building usage data, we also have a data on weather features such as temperature, humidity and wind, that could be linked to the building usage data given building site id. In this project, I used several regression and LSTM based model in order to make this prediction.


#### GitHub repository structure:
This Github repository is organized in the following way:
* **Writeup folder**:  
This folder contants the writeups I did for the project that contains Project_preproposal, Project_proposal, Project_milestone_report and Project_report with Project_report containing the final results. Detailed writeup on the motivation, data description, methods used and results could be found in those files. I encourage reader of this repository to do that before looking at the codes.
* **BuildingEnergyConsumption folder**:  
This folder is split into Data folder and Code folder:
  * **Data** folder in this repository is empty, just because the data is really large (~2GB-3GB). The data can be downloaded from the following website: https://www.kaggle.com/c/ashrae-energy-prediction/data and for this code to work, one would have to place downloaded data into the Data folder. When data is downloaded from the website it is downloaded into the folder called: ashrae-energy-prediction, and this entire folder should be placed in Data folder for this code to work. 
  * **Code** folder contains all the codes I wrote for this project. Files ending in .py contain helper functions I use in my main codes. RegressionModels is the main code I used to make predictions with different regression models including linear regression, decision tree regression, random forest regression and autosklearn regression. LSTMmodels is the main code I used to make predictions using plain LSTM and CNN-LSTM model.



