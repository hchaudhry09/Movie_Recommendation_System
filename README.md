# Movie_Recommendation_System
This code snippet is part of a movie recommendation system project aimed at predicting movie revenues based on various features. The prediction of movie revenues is an important aspect as it helps in understanding the potential success of a movie, which can influence recommendations for users based on popular and high-revenue movies. Here is a detailed explanation of each step:

-We start by importing essential libraries for data manipulation, visualization, model training, and evaluation. pandas is used for data handling, matplotlib and seaborn for visualization, and sklearn for machine learning tasks.
-The dataset containing movie information is loaded from a CSV file into a pandas DataFrame.
-We define the target variable (y) as Movie_Revenue, which we aim to predict. The feature variables (X) include Movie_Budget, Movie_Popularity, Movie_Runtime, and Movie_Vote. These features are selected based on their potential impact on movie revenue.
-Missing values in the feature variables are handled using a SimpleImputer. We use the mean of each column to fill in missing values, ensuring that the dataset is complete and ready for model training.
-The dataset is split into training and testing sets using an 80-20 split. This allows us to train the model on one part of the data and test its performance on another, ensuring a robust evaluation.
-A linear regression model is defined and trained on the training data. This model learns the relationship between the feature variables and the target variable.
-The trained model is used to make predictions on the test set, providing an estimate of the movie revenues for the test data.
-The model's performance is evaluated using the Mean Squared Error (MSE) and R-squared (R²) metrics. MSE measures the average squared difference between the actual and predicted values, while R² indicates the proportion of variance in the dependent variable that is predictable from the independent variables.
-A scatter plot is created to visualize the actual vs predicted movie revenues, allowing us to visually assess the model's performance.
