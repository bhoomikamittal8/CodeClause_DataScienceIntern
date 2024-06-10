# Stock_Market_Prediction

Here's a description of what each part of the code does:

1. **Importing Libraries**: The script starts by importing the necessary Python libraries, including Pandas, NumPy, and Matplotlib for data manipulation and visualization. It also imports Plotly for interactive plotting, as well as some modules for offline Plotly usage.

2. **Reading Data**: It reads stock price data from a CSV file named 'TSLA.csv' into a Pandas DataFrame called 'tesla'.

3. **Data Inspection**: The code performs some initial data inspection tasks:
   - It prints information about the DataFrame, including data types and non-null counts.
   - Converts the 'Date' column to datetime format.
   - Prints the range of dates in the dataset and the total number of days covered.

4. **Descriptive Statistics**: It displays descriptive statistics (mean, standard deviation, etc.) for the columns 'Open', 'High', 'Low', 'Close', and 'Adj Close' using the `describe()` method.

5. **Box Plot**: It creates a box plot for the columns 'Open', 'High', 'Low', 'Close', and 'Adj Close' to visualize the distribution of these values.

6. **Interactive Time Series Plot**: The script creates an interactive time series plot using Plotly to visualize the closing stock prices of Tesla over time. The plot is configured with a title and labeled axes.

7. **Data Splitting**: The code prepares the data for building a regression model. It splits the data into training and testing sets using the `train_test_split` function from scikit-learn.

8. **Feature Scaling**: It performs feature scaling on the training data using standardization (StandardScaler) from scikit-learn.

9. **Linear Regression Model**: It creates a linear regression model using scikit-learn's `LinearRegression` class and fits it to the training data.

10. **Plotting Predictions**: The code creates a plot showing both the actual and predicted closing stock prices on the training data.

11. **Model Evaluation**: It computes and prints the model evaluation metrics, including the R-squared score and Mean Squared Error (MSE), for both the training and testing datasets.

In summary, this script loads and analyzes Tesla stock price data, performs data visualization, builds a simple linear regression model to predict stock prices based on the day index, and evaluates the model's performance on training and testing data. The results of the model evaluation are printed at the end of the script.
