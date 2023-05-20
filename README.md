# Gold-Price-Prediction-using-Random-Forest-Regression
This project aims to predict the price of gold (GLD) using a Random Forest Regression model. The data used for this project is collected from Kaggle. The project involves data collection, data exploration, model training, model evaluation, and visualization of the predicted and actual gold prices.


#Libraries
The following libraries are required for this project:

sklearn.model_selection for train-test splitting
sklearn.ensemble for Random Forest Regression
sklearn for metrics evaluation
numpy for numerical operations
pandas for data manipulation
matplotlib.pyplot for data visualization
seaborn for data visualization
Data Collection
The gold price data is collected from Kaggle and loaded into a Pandas DataFrame using the pd.read_csv() function.

#Data Exploration
Overview
The dataset is explored to gain insights into its structure and content. The first 5 rows of the DataFrame are displayed using the head() function, while the last 5 rows are displayed using the tail() function. The shape of the DataFrame is obtained using the shape attribute, and information about the DataFrame is displayed using the info() method. Missing values in the DataFrame are checked using the isnull().sum() method, and descriptive statistics are calculated using the describe() method.

#Correlation Analysis
The correlation between features is analyzed using a correlation matrix. The correlation matrix is computed using the corr() method, and a heatmap is created using sns.heatmap() to visualize the correlations. The correlation values for the target variable (GLD) are printed using the print() function.

#Data Distribution
The distribution of the target variable (GLD) is visualized using a histogram plot created with sns.distplot().

#Data Preprocessing
Splitting Features and Target
The features and target variable are separated. The features are obtained by dropping the 'Date' and 'GLD' columns from the DataFrame using the drop() method, while the target variable is extracted using indexing.

#Splitting into Training and Test Data
The dataset is split into training and test sets using the train_test_split() function from the sklearn.model_selection module. The features and target variables are passed as input, along with the desired test size and random state.

#Model Training
Random Forest Regression
A Random Forest Regression model is created using the RandomForestRegressor() class from the sklearn.ensemble module. The number of estimators (trees) is set to 100. The model is then trained on the training data using the fit() method.

#Model Evaluation
The trained model is evaluated using the test data. Predictions are made on the test data using the predict() method, and the predicted values are printed. The R-squared error is calculated using the r2_score() function from the sklearn.metrics module, and the error score is printed.

#Visualization
A plot is created to compare the actual and predicted values of the gold price. The actual values are plotted as a blue line using plt.plot(), and the predicted values are plotted as a green line. The plot is given a title and axis labels, and a legend is added to distinguish between the actual and predicted





