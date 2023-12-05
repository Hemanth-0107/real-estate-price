# real-estate-price
## Availed data set from kaggle.com and analysis:
1. cleaned the data
2. Eliminated null values from data
3. Removed the outliers in the data
4. Applied linear regression to the cleaned data
5. Compared with other models like lasso, decision tree
6. Performances are observed using GridSearchCV and k-fold-cross-validation to observe the scores
7. For this data set linear regression gave better results. 
8. Pickle file of model and the columns.json file are generated and used in the server
![image](https://github.com/Hemanth-0107/real-estate-price/assets/78348403/abc5985f-3606-47b1-ad9f-af55c820f49f)


## Creation of Flask api and frontend:
1. created a static html,css,javascript frontend form
2. Parsed the data in flask routes
3. Using pickle and json files estimated the prices for the combination in form
4. Returned the results and fetched them in the ui
5. Locations can be accessed using url: http://127.0.0.1:5000/get_location_names (various places in banglore from dataset)
6. Predictions are availed from: http://127.0.0.1:5000/predict_home_prices  (post)
7. Example of form inputs: (request.form)
   {
    "total_sqft":1000,
    "location":"Whitefield",
    "bhk":3,
    "bath":3
  }
