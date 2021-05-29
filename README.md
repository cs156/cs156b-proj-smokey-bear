# Team Smokey Bear COVID-19 Prediction Project
### Team members: Hannah Chen, Alexandra Lai, Shenyi Li, Felianne Teng

## Project Overview 
For our project, we decided to answer a prevailing question in many of our minds during this pandemic: “Will we be able to reach herd immunity, and if so, when?” After experimenting with different features and data, the features we chose to use were number of deaths, people fully vaccinated, incident rate (the number of cases per 100,000 persons), and people tested in order to predict the number of COVID-19 cases at a future date. We defined herd immunity to occur when the number of cases converges, as that would indicate when the population becomes effectively immune. We separated the data by state and predicted the cases and date at which each state will reach herd immunity.

We tested several models such as the LSTM, Random Forest Regressor, and Linear Regressor, but decided to use the LSTM as our final model, because it produced the most reasonable predictions for future data. Our final model, as well as our previous data and model explorations, can be found and run on the Google Colab. 

## Code Files
Final_CS156b.ipynb includes:
* Data Preprocessing and Data Visualization
* Feature Selection
* Random Forest Regressor model
* Linear Models (logistic regression, linear regression, etc.)
* Final LSTM model
* LSTM prediction graphs
* Deprecated LSTM model

sort_time_covid.ipynb includes:
* Sorted table based on convergence date predicted from LSTM 
* Sorted table based on proportions predicted from LSTM

## Datasets
We sourced our data from several different datasets. Our data for people fully vaccinated per state as well as the data we used for our preliminary data exploration was from the Our World in Data dataset (https://github.com/owid/covid-19-data). The incident rate and people tested data was from the JHU Center for Systems Science and Engineering dataset (https://github.com/CSSEGISandData/COVID-19), while the number of cases and deaths was sourced from the New York Times (https://github.com/nytimes/covid-19-data). We obtained the state population data from the World Population Review website (https://worldpopulationreview.com/states). In our predictions, we used data from January 12, 2021 to May 22, 2021. For ease of access, we compiled the data from different states in the CSSEGISandData GitHub into a single file. This file, along with the state population data, can be found in a separate GitHub repository (https://github.com/fteng1/CS156b_data). 

## Results
Overall, we predicted that 76% of states reached a convergence in the number of cases, with most reaching herd immunity in 6-12 months from now. We created a visualization of our final predictions per state using a map of the United States, which can be found at the following link: https://datawrapper.dwcdn.net/NX3M0/2/. Hovering over each state will show the predicted proportions of each state’s population that has contracted the virus after the predictions converged. 
