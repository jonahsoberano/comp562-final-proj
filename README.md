# comp562-final-proj
The code for our final project for COMP 562 Spring 2019 class at UNC

<br />

## The Real Deal with Real Estate: Holistically Predicting Housing Prices
#### Jonah Soberano, Josh Kennedy, Surya Poddutoori, and Hamzah Chaudhry
[Kaggle Link](https://www.kaggle.com/c/house-prices-advanced-regression-techniques/overview)

<br />

### Description
Our main dataset consists of real world housing data from Ames, Iowa from 2006 to 2010. The data was found and cleaned by Dean de Cock of Truman State University, and is available on Kaggle as a competition. The data set has 2930 observations (representing individual houses), which has been split into equal sized training and test sets by Kaggle. Each observation consists of eighty parameters, and the training set also includes a field for the sales price of the house. (See [1] for further details).

### Motivation and Goals
For future homeowners and homesellers, the buying and selling process can be stressful. Homeowners want to know how much their house typically would sell for and homebuyers want to know what kind of house they can buy given their budget. Knowing this can bring vital financial perspective to sellers and a realistic goal for prospective buyers. We plan to start off by predicting the eventual sale price of each house by utilizing the other parameters provided in the data set.

### Ideas and Techniques
As the target variable (sale price) is continuous, we will most likely start with linear regression, including ridge regularization. Determining which of the 80 parameters are needed to model sale price effectively will be one of the main challenges of this project. In order to improve upon our model, we will likely need to utilize feature engineering to create new, useful features based upon the parameters we currently have. After creating a basic regression model, we will explore more advanced techniques such as gradient boosting, which is a gradient descent algorithm. An open source library (XGBoost) provides the functionality needed to implement this algorithm. Additionally, we plan to utilize k-fold cross-validation on the training data in order to develop our model before testing on the test data. This should reduce the risk of overfitting our model on the training data and will hopefully result in greater accuracy on the unseen test data.

<br />

[1]: Journal of Statistics Education Volume 19, Number3(2011), www.amstat.org/publications/jse/v19n3/decock.pdf