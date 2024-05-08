Car-Price-Prediction
The purpose of this investigation is to identify the variables that influence automobile prices and to develop machine learning models that forecast current car prices depending on variables like mileage driven, selling price, fuel type, and so on.


Method of Analysis:

Data Investigation:

Dataset 'car_data.csv' is loaded from a CSV file.
To gain an understanding of the dataset's structure and contents, the first five rows are shown.
Analysis of Correlation:

To see the correlation between the dataset's numerical columns, a heatmap is made. This aids in determining possible connections between the target variable and characteristics.
Information Visualization:

To comprehend the distribution of the 'Present_Price' column, a distribution plot is made.
To see how different categorical features—like "Car Name," "Driven kms," and "Fuel Type"—relate to the objective variable, "Present Price," bar charts are made.

The link between 'Present_Price' and 'Car_Name' across several categories is shown using a violin plot.
A scatter plot featuring a regression line is designed to investigate the correlation between 'Driven_kms' and 'Present_Price'.
Preparing Data:

The variables 'Present_Price' and 'Driven_kms' are chosen for machine learning, together with 'Selling_Price' and 'Fuel_Type' as the target variable.
The train test split function from sklearn.model selection divides the data into training and testing sets.

Model Construction and Forecasting:

The DecisionTreeRegressor class from sklearn.tree is used to construct a Decision Tree Regressor model. Using the training data, the model is trained and then applied to the test data to provide predictions.
The LinearRegression class from sklearn.linear_model is used to construct a linear regression model. In a similar way, predictions are made and the model is trained.

Assessment of the Model:

The score approach is used to assess the models' performance. Nevertheless, there is an error in the evaluation procedure since the score between the test data and the test data predictions is calculated incorrectly. This has to be fixed.

