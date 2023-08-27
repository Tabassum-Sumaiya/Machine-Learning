# Ecommerce company
Ecommerce company based in New York City that sells clothing online but they also have in-store style and clothing advice sessions.

## Task
Customers spending behaviour prediction.

## Steps:

### Importing Dependencies
1. Import pandas, numpy, matplotlib,and seaborn. Then set %matplotlib inline 
2. Imports Ecommerce Customers csv file as a DataFrame called df.
3. Check the head of customers, and check out its info() and describe() methods.

### Exploratory Data Analysis
1. Use seaborn to create a jointplot to compare the Time on Website and Yearly Amount Spent columns.
2. Do the same but with the Time on App column instead of Time on Website.
3. Use jointplot to create a 2D hex bin plot comparing Time on App and Length of Membership.
4. Find relationships across the entire data set and use pairplot to recreate the plot.
5. Based off this plot what looks to be the most correlated feature with Yearly Amount Spent?
6. Create a linear model plot (using seaborn's lmplot) of Yearly Amount Spent vs. Length of Membership.

### Training and Testing Data
1.Set a variable X equal to the numerical features of the customers and a variable y equal to the "Yearly Amount Spent" column.
2.Use model_selection.train_test_split from sklearn to split the data into training and testing sets. Set test_size=0.3 and random_state=101

### Training the Model
1.Import LinearRegression from sklearn.linear_model
2.Create an instance of a LinearRegression() model named lm
3. Train/fit lm on the training data.
4.Print out the coefficients of the model

### Predicting Test Data
1.Use lm.predict() to predict off the X_test set of the data
2.Create a scatterplot of the real test values versus the predicted values

### Evaluating the Model
1. Calculate the Mean Absolute Error, Mean Squared Error, and the Root Mean Squared Error. Refer to the lecture or to Wikipedia for the formulas
2.calculating the residual sum of squares and the explained variance score

### Residuals
Plot a histogram of the residuals and make sure it looks normally distributed. Use either seaborn distplot, or just plt.hist()

###  interpret the coefficients
1.Recreate the dataframe below
2.How can you interpret these coefficients?
