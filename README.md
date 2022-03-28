# Airbnb_Price_Prediction
# Context
Since 2008, guests and hosts have used Airbnb to expand on traveling possibilities and present more unique, personalized way of experiencing the world. This dataset describes the listing activity and metrics in NYC, NY for 2019. I want to predict the price of the listings based on the given features. <br />

Content<br />

This data file includes all needed information to find out more about hosts, geographical availability, necessary metrics to make predictions and draw conclusions.<br />

Acknowledgements<br />

This public dataset is part of Airbnb, and the original source can be found on this link: <br />
http://insideairbnb.com

# Goal
The goal is to predict the listing price for any given Airbnb Listing. For example, a potential owner of a house/apartment wants to list their unit, what should they consider doing to determine their listing prices and what factors affect the prices the most?

# Key Metrics
-Prediction accuracy of the model <br />
-Variable importance<br />
-Average Listing Prices of units that share similar characteristics<br />

# Results
All of the results are produced from Python.

## Exploratory Analysis: 
### Unit Listing Plot from longitude and latitude
![Xnip2022-03-28_01-16-03](https://user-images.githubusercontent.com/33715191/160359197-9802c239-7e85-4417-a469-4477f92f5887.jpg)
### Clusters the units can be broken into:
![Xnip2022-03-28_01-16-15](https://user-images.githubusercontent.com/33715191/160359524-44306916-34ac-45c6-ada7-e181373a7188.jpg)


![Xnip2022-02-06_23-56-12](https://user-images.githubusercontent.com/33715191/152747518-983b67e3-9c62-4363-94fd-fa1b8a1f97a1.jpg) <br />

### Listing Price Distribution
![Xnip2022-03-28_01-16-34](https://user-images.githubusercontent.com/33715191/160359306-13eb0d9d-c34a-41a5-afa3-dcd17d1dcdad.jpg)
![Xnip2022-03-28_01-17-50](https://user-images.githubusercontent.com/33715191/160359323-45bdaf8c-2a52-4b40-97f7-5becc1c6d1b7.jpg)


## Count of units in different neighborhoods and neighborhood groups
![Xnip2022-03-28_01-18-08](https://user-images.githubusercontent.com/33715191/160359407-f86f7841-9648-4bed-a4eb-4d205b2279f6.jpg)
![Xnip2022-03-28_01-18-21](https://user-images.githubusercontent.com/33715191/160359413-a47562da-5b4d-4008-873a-094045d2822b.jpg)
![Xnip2022-03-28_01-17-12](https://user-images.githubusercontent.com/33715191/160359502-3f371ac6-b470-4d86-ad18-097bdf23f064.jpg)

### Scatterplots of Number of Reviews Against Price
![Xnip2022-03-28_01-18-39](https://user-images.githubusercontent.com/33715191/160359682-d7b34177-0963-4245-a445-4c39600ca79d.jpg)

### Linear Regression and Feature Importance
![Xnip2022-03-28_01-20-11](https://user-images.githubusercontent.com/33715191/160360072-519691df-ab8e-49cc-98ae-0bf1045738e4.jpg)
![Xnip2022-03-28_01-19-57](https://user-images.githubusercontent.com/33715191/160359969-7744c5cc-2080-4d65-ba35-75235ac35482.jpg)

### Find The Features That Have the Highest Interactions With Each Other
![Xnip2022-03-28_01-20-33](https://user-images.githubusercontent.com/33715191/160360169-6bec0a47-7d41-4592-9a46-3bbbbec4df5e.jpg)

### Linear Regression After Generating Interaction Featuures
![Xnip2022-03-28_01-42-10](https://user-images.githubusercontent.com/33715191/160360775-f09705ae-50bd-4846-8bce-965e8f93a28e.jpg)

### Gradient Boosting Regressor Results
![Xnip2022-03-28_01-43-46](https://user-images.githubusercontent.com/33715191/160360962-e78ab740-4b6e-4924-becb-0255070b0d14.jpg)

Gradient Boosting Regressor has the highest accuracy![Uploading Xnip2022-03-28_01-43-46.jpg…]()


## Conclusion:
### Modeling Conclusions: 
Originally, this model only had about 10% accuracy due to having a high number of features in the dataset. After cleaning the data, taking out outliers of the numeric features, the model's accuracy improved to about 45%. Then I engineered new features including location cluster, availability level, and whether a dataset has a high number of reviews. Also, I categorized the low frequency count neighborhoods into one category 'other.' The linear regression model's accuracy increased to 53%. Gradient Boosting Regressor was able to generate 60% accuracy. 

### Additional Relevant Data Needed & Future Improvements:
There are also other factors to consider such as seasonlity, demand, number of photos that the Airbnb listing has, and the review ratings of the listings. Some of these factors are not included in this particular dataset. However, this model can also be applied to other datasets to capture more accurate results. <br />
This project is really fun to work on. It really emphasizes the importance of feature engineering and interpreting the data before building any predictive models. <br />

# Reference For The Dataset
https://www.kaggle.com/datasets/dgomonov/new-york-city-airbnb-open-data
