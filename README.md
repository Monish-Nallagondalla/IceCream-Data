# Ice Cream Sales Prediction using Decision Tree Regression

This project uses a Decision Tree Regression model to predict ice cream sales revenue based on temperature data. The dataset contains two features: `Temperature` (independent variable) and `Revenue` (dependent variable). The code demonstrates data preprocessing, model training, evaluation, and visualization of results.

## Project Overview

- **Objective**: Predict ice cream revenue based on temperature using a Decision Tree Regression model.
- **Dataset**: `icecreamdata.csv` - Contains temperature and revenue data for ice cream sales.
- **Model**: Decision Tree Regressor from scikit-learn.
- **Evaluation Metrics**: Mean Absolute Error (MAE), Mean Squared Error (MSE), and Root Mean Squared Error (RMSE).
- **Visualizations**: Scatter plots for real vs. predicted values and a regression line plot.

## Dataset

The dataset (`icecreamdata.csv`) includes the following columns:
- `Temperature`: The temperature in degrees (independent variable).
- `Revenue`: The revenue from ice cream sales in dollars (dependent variable).

Sample data:

| Temperature | Revenue    |
|-------------|------------|
| 24.566884   | 534.799028 |
| 26.005191   | 625.190122 |
| 27.790554   | 660.632289 |
| 20.595335   | 487.706960 |
| 11.503498   | 316.240194 |

Alternatively, the dataset can be fetched from this [GitHub URL](https://raw.githubusercontent.com/mk-gurucharan/Regression/master/IceCreamData.csv).

## Prerequisites

To run this project, you need the following Python libraries:
- `numpy`
- `pandas`
- `matplotlib`
- `scikit-learn`

Install the dependencies using pip:
```bash
pip install numpy pandas matplotlib scikit-learn
```

## How to Run

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/your-repo-name.git
   cd your-repo-name
   ```

2. **Prepare the Dataset**:
   - Place `icecreamdata.csv` in the project directory, or
   - Update the code to use the online dataset URL by uncommenting the respective line:
     ```python
     dataset = pd.read_csv('https://raw.githubusercontent.com/mk-gurucharan/Regression/master/IceCreamData.csv')
     ```

3. **Run the Code**:
   - Open the `.ipynb` file in Jupyter Notebook or any compatible IDE:
     ```bash
     jupyter notebook Ice_Cream_Sales_Prediction.ipynb
     ```
   - Alternatively, convert it to a `.py` file and run it with Python:
     ```bash
     python ice_cream_sales_prediction.py
     ```

4. **Output**:
   - Visualizations: Two plots will be displayed:
     1. Scatter plot comparing real vs. predicted revenue values.
     2. Regression line showing the model's predictions across the temperature range.
   - Metrics: MAE, MSE, and RMSE will be printed to evaluate model performance.

## Code Breakdown

- **Data Loading**: Reads the CSV file into a pandas DataFrame.
- **Preprocessing**: Splits the data into training (95%) and testing (5%) sets.
- **Model Training**: Fits a Decision Tree Regressor to the training data.
- **Prediction**: Predicts revenue for the test set.
- **Evaluation**: Computes MAE, MSE, and RMSE.
- **Visualization**: Plots the results using matplotlib.

## Results

The model's performance on the test set is as follows:
- **Mean Absolute Error (MAE)**: 33.98
- **Mean Squared Error (MSE)**: 1851.92
- **Root Mean Squared Error (RMSE)**: 43.03

Example predictions:

| Real Values | Predicted Values |
|-------------|------------------|
| 421.621505  | 430.343903       |
| 570.990932  | 542.608070       |
| 629.893792  | 682.752869       |
| 642.227291  | 719.471701       |

## Visualizations

1. **Scatter Plot**: Red dots represent real revenue values, and green dots represent predicted values.
2. **Regression Line**: A black line shows the model's predictions across a range of temperatures.

## Future Improvements

- Experiment with other regression models (e.g., Linear Regression, Random Forest).
- Tune hyperparameters of the Decision Tree Regressor (e.g., max_depth, min_samples_split).
- Increase the test set size for a more robust evaluation.
- Add feature engineering to incorporate additional variables (e.g., day of the week, location).

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

- Built with Python, scikit-learn, and matplotlib.
```

### Instructions
1. Copy the entire code block above.
2. Open your `README.md` file in your GitHub repository (create one if it doesn’t exist).
3. Paste the code into the file.
4. Replace `your-username` and `your-repo-name` in the "Clone the Repository" section with your actual GitHub username and repository name.
5. Save and commit the file to your repository.

That’s it! Your README will be ready to go. Let me know if you need further assistance!
