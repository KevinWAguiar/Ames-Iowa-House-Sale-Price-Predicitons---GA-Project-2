Problem Statement:

		As a new hire for Zillow, a home real estate website, we've been asked to create a
	predictive model for home sale prices for Aimes, Iowa.  Fortunately, the data has been
	collected and is being provided in the form of two datasets: 1. the 'training' dataset
	(train.csv); 2. the 'testing' dataset (test.csv).  
		Zillow's Data Analytics team and I plan first to do some Exploratory Data Analysis
	(EDA) to search for any outliers or otherwise apprehensive data.  Next, we will clean
	the data for any detected errors and deal with null values.  Finally, we will iteratively
	run different regression models on selected features, or variable inputs, to build a 
	model that predicts the home sale price of home listings in Aimes, Iowa.
		The different regression models used will include: 1. Linear Regression; 2. Lasso
	Regression; 3. Ridge Regression; and 4. Elastic Net Regression.  Lasso, Ridge, and
	Elastic Net Regression are methods that perform feature selection, each to different 
	degrees.  They also regularize, or scale, the Beta coefficient of each feature, mani-
	pulating the model to minimize the affect 'noise' or meaningless data has on its pre-
	dictions, increasing the model's predictive accuracy.
		Fortunately for us, Kaggle, the Data Science website, has a 'holdout' data set, or
	a collection of unseen data, for Aimes, Iowa, which we will be able to test our model
	against.  After building our models, we will run them on the 'test' set, and upload
	the resulting predictions to Kaggle.  Kaggle will then return the Root Mean Squared
	Error of those predictions against the true home sale prices.  The Root Mean Squared
	Error, essentially, is the average difference between a home's actual sale price and
	its predicted sale price.  This being said, we want our model to have an RMSE as close
	to 0 as possible.  The model with the lowest RMSE will be chosen as our winner!
	
	
	Why Do We Care?
	
		Great question! Zillow's management team, after consulting the Data Analytics
	team, has realized a clear connection between the accuracy of the predicted home sale
	price it lists on its website and user traffic.  Therefore, the better predictive model
	Zillow has to predict home sale prices, the more traffic it can generate!  Of course, 
	greater user traffic equals greater Ad Revenue, a win for everyone at Zillow!
	
	
Conclusions and Recommendations:

	As we built our models, changed the features that were incorporated/not incorporated
in the model, changed the model's paramters, like its alpha level, we were able to find
a clear winning model.  First, we dropped columns that were 'zerod out' by Lasso's 'noise
cancellation' effect.  Then, we experimented with the alpha level, until we realized that
the Lasso model with alpha set to 1050 was our strongest model, according to Kaggle.
It should be mentioned, though, that this model did not provide the strongest performance
metrics when measured prior to Kaggle submission.
	We were somewhat limited with regards to time; Kaggle only allows 10 submissions per
day.  If we had more time, we would be able to experiment further and submit more models
to improve the model further.  We would also appreciate exposure to data from other cit-
ies, states, and/or regions, as we believe they can provide further insight in to what 
features should be considered most/least when building a home sale price model.
