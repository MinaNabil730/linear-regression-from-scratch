# Linear Regression with Gradient Descent

This project demonstrates the implementation of linear regression using gradient descent to predict profits based on population data. The code reads data from a CSV file, visualizes it, and uses gradient descent to find the best-fit line. The performance of the model is tracked and visualized over iterations.

## Prerequisites

To run this code, you need to have the following libraries installed:
- `pandas`
- `numpy`
- `matplotlib`

## Data

The data is expected to be in a CSV file named `data.csv` with no header. It should contain two columns:
- **Population**: The population of the city.
- **Profit**: The profit of the city.

## Code Overview

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

## Output

The code will generate the following outputs:

1. A scatter plot of the training data (Population vs. Profit).

![image](https://github.com/MinaNabil730/linear-regression-from-scratch/assets/109760458/3f86c326-41d3-4d69-8d22-f3c9d9cb54c1)

2. A plot showing the fitted regression line over the training data.

![image](https://github.com/MinaNabil730/linear-regression-from-scratch/assets/109760458/37494be7-463f-4e1f-9fb0-62c281c4a400)
 
3. A plot of the cost function over the iterations of gradient descent.

![image](https://github.com/MinaNabil730/linear-regression-from-scratch/assets/109760458/93156554-9dc9-4284-bff9-7c100a94fb4b)


## License

This project is licensed under the Creative Commons Attribution 4.0 International (CC BY 4.0) License. 

## Acknowledgments

This implementation is inspired by the linear regression exercise from the Andrew Ng Machine Learning course on Coursera.
