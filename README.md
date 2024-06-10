# Movie Rating Prediction
## Project Overview
The goal of this project is to predict the rating of a movie based on features such as genre, director, and actors. By analyzing historical movie data, we aim to develop a regression model that accurately estimates the ratings given to movies by users or critics. This project provides insights into the factors that influence movie ratings and explores various data analysis, preprocessing, feature engineering, and machine learning modeling techniques.

## Dataset Overview
The dataset used for this project is (https://www.kaggle.com/datasets/adrianmcmahon/imdb-india-movies) which contains information about various movies. The key features in the dataset include:

* Name: The name of the movie.
* Year: The release year of the movie.
* Duration: The duration of the movie in minutes.
* Genre: The genre(s) of the movie.
* Rating: The IMDb rating of the movie.
* Votes: The number of votes the movie received.
* Director: The director of the movie.
* Actor 1, Actor 2, Actor 3: The main actors in the movie.

## Project Structure
### 1. Data Collection
- The dataset is loaded from a CSV file using pandas.
### 2. Data Preprocessing
The preprocessing pipeline involves handling missing values and encoding categorical variables using SimpleImputer, OneHotEncoder, ColumnTransformer, and Pipeline.
* Handling Missing Values and Encoding:
  - Numeric features (Year, Duration) are imputed using the median strategy.
  - Categorical features (Genre, Director, Actor 1, Actor 2, Actor 3) are imputed using the most frequent strategy and then one-hot encoded.

### 3. Data Visualization
- Visualizations are created to understand the data distribution and the relationships between features and the target variable.

### 4. Data Splitting
- The dataset is split into training and testing sets to evaluate the model's performance on unseen data.

### 5. Model Training
- A linear regression model is trained using the processed features.

### 6. Model Evaluation
- The model's performance is evaluated using metrics such as Mean Squared Error (MSE) and R-squared (R2) score. Additionally, residual plots are created to visualize the distribution of residuals and check for patterns or biases.

##  Libraries Used
* pandas
* numpy
* scikit-learn
* matplotlib

## Results
The trained linear regression model provides predictions for movie ratings. The performance is evaluated using MSE and R2 score. Residual plots help in understanding the distribution and patterns of errors in the predictions.

## Conclusion
This project demonstrates the process of building a movie rating prediction model using linear regression. It involves data collection, preprocessing, feature engineering, model training, and evaluation. The results provide insights into the factors that influence movie ratings and highlight areas for potential improvement in the model.

