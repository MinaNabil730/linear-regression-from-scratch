# Linear Regression Projects

This repository contains two projects demonstrating the implementation of linear regression using gradient descent: one with a single variable and another with multiple variables. Each project includes data visualization, cost function computation, and model training with results visualized for better understanding.

## Projects

### 1. Linear Regression with One Variable

#### Description

This project predicts profits based on population data using linear regression with one variable.

#### Prerequisites

To run this code, you need to have the following libraries installed:
- `pandas`
- `numpy`
- `matplotlib`

#### Data

The data is expected to be in a CSV file named `one-variable-data.csv` with no header. It should contain two columns:
- **Population**: The population of the city.
- **Profit**: The profit of the city.

#### Code Overview

1. **Importing Libraries**: The necessary libraries are imported.
2. **Reading Data**: The CSV file is read into a DataFrame and the first few rows are displayed.
3. **Data Visualization**: A scatter plot is created to visualize the relationship between population and profit.
4. **Data Preparation**: A column of ones is added to the DataFrame to account for the intercept term in the linear regression model.
5. **Matrix Conversion**: The feature matrix `X` and target vector `y` are converted to numpy matrices.
6. **Initial Parameters**: The initial parameters (theta values) are set to zero.
7. **Cost Function**: A function `computecost` is defined to compute the cost for given `X`, `y`, and `theta`.
8. **Gradient Descent**: The `gradientDescent` function performs gradient descent to minimize the cost function.
9. **Model Training**: The model is trained by running gradient descent for a specified number of iterations.
10. **Results Visualization**: The fitted line is plotted against the training data, and the cost over iterations is visualized.

#### Output

The code will generate the following outputs:

1. A scatter plot of the training data (Population vs. Profit).

   ![image](https://github.com/MinaNabil730/linear-regression-from-scratch/assets/109760458/887d0ac8-1c92-473d-b4c5-75f9c957c5c6)
2. A plot showing the fitted regression line over the training data.
   
   ![image](https://github.com/MinaNabil730/linear-regression-from-scratch/assets/109760458/5e3e47fb-b8cb-44b7-9e1c-8a4c2101396b)
3. A plot of the cost function over the iterations of gradient descent.
   
   ![image](https://github.com/MinaNabil730/linear-regression-from-scratch/assets/109760458/bd2bcceb-6aa7-4334-aa73-814473b9c6e8)


### 2. Linear Regression with Multiple Variables

#### Description

This project predicts house prices based on various features using linear regression with multiple variables.

#### Prerequisites

To run this code, you need to have the following libraries installed:
- `pandas`
- `numpy`
- `matplotlib`

#### Data

The data is expected to be in a CSV file named `multi-variable-data.csv` with no header. It should contain multiple columns representing different features, with the last column being the target variable (e.g., house price).

#### Code Overview

1. **Importing Libraries**: The necessary libraries are imported.
2. **Reading Data**: The CSV file is read into a DataFrame and the first few rows are displayed.
3. **Data Preparation**: A column of ones is added to the DataFrame to account for the intercept term in the linear regression model.
4. **Feature Normalization**: The feature values are normalized to ensure efficient gradient descent.
5. **Matrix Conversion**: The feature matrix `X` and target vector `y` are converted to numpy matrices.
6. **Initial Parameters**: The initial parameters (theta values) are set to zero.
7. **Cost Function**: A function `computecost` is defined to compute the cost for given `X`, `y`, and `theta`.
8. **Gradient Descent**: The `gradientDescent` function performs gradient descent to minimize the cost function.
9. **Model Training**: The model is trained by running gradient descent for a specified number of iterations.
10. **Results Visualization**: scatter plot and fitted regression line for Size vs. Price, scatter plot and fitted regression line for Beds No. vs. Price, and The cost over iterations is visualized.

#### Output

The code will generate the following outputs:

1. A scatter plot and fitted regression line for Size vs. Price.
 
   ![image](https://github.com/MinaNabil730/linear-regression-from-scratch/assets/109760458/ab3b5e62-4af8-4211-99cc-66acf2c27e9f)
2. A scatter plot and fitted regression line for Beds No. vs. Price.
   
   ![image](https://github.com/MinaNabil730/linear-regression-from-scratch/assets/109760458/3206a079-d37a-4274-b5ef-94b20c91448a)
3. A plot of the cost function over the iterations of gradient descent.
   
   ![image](https://github.com/MinaNabil730/linear-regression-from-scratch/assets/109760458/e0c805ff-8b97-49ed-92de-f2c2e5d02327)


#### Observations

- The relationship between the number of beds and house prices does not show a strong linear correlation, as evidenced by the resulting plot:
  
   ![image](https://github.com/MinaNabil730/linear-regression-from-scratch/assets/109760458/c60f84b6-351b-45ff-a620-0c42578b92ae)

## License

This project is licensed under the Creative Commons Attribution 4.0 International (CC BY 4.0) License.

## Acknowledgments

This implementation is inspired by the linear regression exercises from the Andrew Ng Machine Learning course on Coursera.
