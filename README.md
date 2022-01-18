# Redfin Linear Regression
![Screen Shot 2022-01-18 at 1 24 55 PM](https://user-images.githubusercontent.com/88032642/150004826-f55bf2a1-072e-4951-856a-22e77f7dbaf7.png)

# Abstract
A client reached who is thinking of buying a single family home and doesnt know which area is best. They wanted me to build them a regression to allow them to not overpay for a home and provide analysis on the types of homes they would find in each neighborhood. My objective was to Web Scrape Redfin for various home features and analyze the home prices based on those features. Then build a predictive regression model to predict the price of a home. After refining my model, I built dashboards to visualize and communicate my results. Which I will present to my client with my predictions. 

# Design 
Lasso and Ridge lambda tuning models were applied to standardized data, as well as Step Ordinary Least Squares modeling, removing influential points and outliers. A Lasso model was chosen for final testing in order to avoid overfitting and data loss while achieving a maximal fit.

# Objective
Web Scrape  Redfin for various home features and analyze the home prices based on those features. Then build a predictive regressive model to predict the price of a home. 

# Data
1000+ data points were scraped from redfin targeting 22 cities in Illinois. The variables I scrapped included Price/Sq.Ft, Lot Size, Year Built, Tax Annual Amount, Tax Year, Tax Exemptions, bedrooms, bathrooms, sq_footage, price, address, City, Zip Code, and State. 

During the exploratory analysis I saw a large correlation between square footage and price. 
![Screen Shot 2022-01-18 at 1 29 47 PM](https://user-images.githubusercontent.com/88032642/150005503-e6cf0664-04fa-4f71-b131-9da68059e6a0.png)

I extracted data from 2018 Tax Returns provided by the IRS database. I used that data to pull adjusted gross income by zip code and incorporated that into my analysis. 
![Screen Shot 2022-01-18 at 1 34 36 PM](https://user-images.githubusercontent.com/88032642/150006221-59cd1f72-0c1e-436e-8a6f-30779fe9d27e.png)


# Features
* Price/Sq.Ft
* Lot Size
* Year Built
* Tax Annual Amount
* Tax Year
* Tax Exemptions
* Bedrooms
* Bathrooms
* Sq_Footage
* Price
* City
* Zip Code

# Algorithms
* Linear Regression
* Lasso Regression- To remove unnecessary features
* Ridge Regression- To reduce effects of collinear feature
* Polynomial Regression 
* Feature Engineering & Selection
* Hyperparameter Tuning 
* Supervised Machine Learning
* 80/20 Test/Train Split

# Feature Engineering
* Converting categorical features to binary dummy variables
* Using imputation to drop data points that were missing significant information 
* Limiting outliers by reducing my range of certain features 
* Examining graphical discontinuity in the prices and square footage
* Categorical column grouping to identify trends by city

# Tools

* NumPy and Pandas for data manipulation
* Matplotlib and Seaborn for plotting
* SKLearn, Statsmodels for modeling
* Beautiful soup for web scraping and data ingestion

# Models
My model was fairly accurate at making predictions with only a mean scared error of $71,983 and R2 adjusted of .72. With more tuning I can get this model to be even more accurate.
![Screen Shot 2022-01-18 at 1 29 57 PM](https://user-images.githubusercontent.com/88032642/150005523-f6641587-3baa-468c-8ed6-7aca5bdc0796.png)

Overall my model was best at predicting homes in Niles, Park Ridge and Buffalo Grove. 

![Screen Shot 2022-01-18 at 1 30 06 PM](https://user-images.githubusercontent.com/88032642/150005552-6a9bf870-8d3e-4335-8dce-59df749bb00d.png)

