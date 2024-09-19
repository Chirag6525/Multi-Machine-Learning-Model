# Multi-Machine-Learning-Model
The comparison of multiple Machine Learning models refers to training, evaluating, and analyzing the performance of different algorithms on the same dataset to identify which model performs best for a specific predictive task. 
By comparing multiple models, we aim to select the most effective algorithm that offers the optimal balance of accuracy, complexity, and performance for their specific problem. 

## DataSet
The dataset consists of 414 entries and 7 columns, with no missing values. Here’s a brief overview of the columns:

- Transaction date: The date of the house sale (object type, which suggests it might need conversion or extraction of useful features like year, month, etc.).
- House age: The age of the house in years (float).
- Distance to the nearest MRT station: The distance to the nearest mass rapid transit station in meters (float).
- Number of convenience stores: The number of convenience stores in the living circle on foot (integer).
- Latitude: The geographic coordinate that specifies the north-south position (float).
- Longitude: The geographic coordinate that specifies the east-west position (float).
- House price of unit area: Price of the house per unit area (float), which is likely our target variable for prediction.

## Model Training and Comparison
- **Linear Regression:** A good baseline model for regression tasks.
- **Decision Tree Regressor:** To see how a simple tree-based model performs.
- **Random Forest Regressor:** An ensemble method to improve upon the decision tree’s performance.
- **Gradient Boosting Regressor:** Another powerful ensemble method for regression.

## Evaluation Metrics
- Mean Absolute Error
- R-squared

## Result
	**Model**       **MAE**	        **R2 Score**
LinearRegression	9.748246	      0.529615
Decision Tree	    11.760342	      0.204962
Random Forest	    9.887601	      0.509547
Gradient Boosting	10.000117	      0.476071

## Conclusion
- Linear Regression has the lowest MAE (9.75) and the highest R² (0.53), making it the best-performing model among those evaluated. It suggests that, despite its simplicity, Linear Regression is quite effective for this dataset.
- Decision Tree Regressor shows the highest MAE (11.76) and the lowest R² (0.20), indicating it may be overfitting to the training data and performing poorly on the test data.
- Random Forest Regressor and Gradient Boosting Regressor have similar MAEs (9.89 and 10.00, respectively) and R² scores (0.51 and 0.48, respectively), performing slightly worse than the Linear Regression model but better than the Decision Tree.