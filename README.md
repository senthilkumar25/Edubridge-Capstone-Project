# Edubridge-Capstone-Project
## Name:M.senthil kumar
## Enrollment Number : EBEON0322580623
## Batch : 2021-7229
### Tittle: Body fat Prediction using ML
#### Dataset:
Lists estimates of the percentage of body fat determined by underwater weighing and various body circumference measurements for 257 men.
### Motive:
We can Find body Fat using DXA scan or Underwater weighing test, using this we can find density and Apply it Siris equation,
but both of them highly Expensive all are above $150, and in India DXA scan costs in range of 6000rs-15000rs,to eliminate highly Expensive Method 
to find body fat ,I tried to build an accurate method at no cost and simple in Home, using Ml Model.
### Process:
	Data Clean 

  •	check null if exists drop an row otherwise replace with mean
  •	check outlieres using box plot in our data set, if it present we want remove outlieres

	Creating EDA for the dataset

        •	Bar plot
        •	Pairplot
        •	Corelation Matrix
	Feature Engineering

        •	remove outlieres using IQR(Interquartile range)

        •	Checking multicolinearity and if exists then use VIF(variance inflation factor)

        •	Using power transform to make it normaly distributed

	Creating prediction M.L model to predict Density

        •	The dataset  is very small(252 men), so linear Regression and ridge regression model is 
          performing better than  any other M.L. Models.
          
        •	Using Bagging and Boosting concept which doesn’t make any sense in this project.
        
        •	Linear regression is performing well with accuracy of 76%

	Finaly , Using Siri formula predict body fat by predicted density()
