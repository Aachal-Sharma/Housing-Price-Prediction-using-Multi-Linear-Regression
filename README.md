# Housing-Price-Prediction-using-Multi-Linear-Regression
his repository demonstrates how to predict housing prices using multi-linear regression. The goal is to predict the price of a house based on various features such as area, number of bedrooms, bathrooms, stories, and other categorical features.
Dataset

The dataset used in this project is the Housing Prices Dataset. It includes the following columns:

    price: The target variable representing the price of the house.
    area: The area of the house in square feet.
    bedrooms: The number of bedrooms in the house.
    bathrooms: The number of bathrooms in the house.
    stories: The number of stories in the house.
    mainroad: Whether the house is located on a main road (yes/no).
    guestroom: Whether the house has a guestroom (yes/no).
    basement: Whether the house has a basement (yes/no).
    hotwaterheating: Whether the house has hot water heating (yes/no).
    airconditioning: Whether the house has air conditioning (yes/no).
    prefarea: Whether the house is in a preferred area (yes/no).
    furnishingstatus: The level of furnishing (furnished/semi-furnished/unfurnished).

Data Preprocessing

Categorical variables, such as mainroad, guestroom, basement, hotwaterheating, airconditioning, prefarea, and furnishingstatus, are mapped to numeric values to prepare the dataset for model training. For example:

    yes/no values are converted to 1/0.
    furnishingstatus is mapped to numerical values like 1 (furnished), 2 (semi-furnished), and 3 (unfurnished).

Model Overview

In this project, we use multi-linear regression to predict house prices. Multi-linear regression is a statistical technique where multiple independent variables (such as area, number of bedrooms, and others) are used to predict the dependent variable (price).
Workflow:

    Data Loading: The dataset is loaded from a CSV file that contains all the relevant features and target variables.
    Data Preprocessing: Convert categorical variables into numerical values, normalize data if required, and handle missing values if necessary.
    Data Splitting: The dataset is split into 80% for training and 20% for testing to evaluate model performance.
    Model Training: A linear regression model is trained using the training data.
    Model Evaluation: The model’s performance is evaluated using the R-squared score. The R-squared score indicates how well the model explains the variability of the target variable.

Key Model Evaluation Metrics:

    R-squared (R²) Score: This score is used to evaluate the accuracy of the model. It tells us what percentage of the variance in the dependent variable (price) is explained by the independent variables. A higher R² value indicates better model performance.

Expected Results:

    A reasonable R-squared score around 0.65 suggests that 65% of the variance in house prices can be explained by the model. However, improvements can be made by adding more features or using more advanced techniques

All the details of the model implementation, including the data preprocessing, model training, and evaluation, are provided in the Jupyter notebook file:

multi_linear_regression_for_house_prediction.ipynb

This file contains the complete code and explanation of each step involved in building the regression model.
Conclusion

The multi-linear regression model serves as a basic yet effective way to predict housing prices. The model achieves a moderate performance with an R-squared score of approximately 65%, indicating that there is room for improvement. Further improvements can be made by incorporating additional features, trying other regression techniques, or fine-tuning the existing model
