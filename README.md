## Linear Regression

- Linear regression is a statistical method used to model the linear relationship between a dependent variable and an independent variable by fitting a linear equation to the observed data
- The goal of linear regression is to find the line equation that best fits the data, called the “line of best fit” 
- Equation of Linear regression -> y = w0 + w1x, where w0 and w1 are the weights/coefficients, which need to be calculated and are chosen to minimise the error between the predicted value and observed value 

**Implementing Linear Regression from Scratch**

- Collect and prepare the data: You will need to have a dataset that includes both the independent variables (x) and the dependent variable (y). You may need to clean and preprocess the data to handle missing values or to transform the variables as needed.

- Initialize the model parameters: You will need to choose the values for the coefficients b0 and b1. It is common to initialize them to 0 or to small random values.

- Define the loss function: The loss function is used to measure how well the model is doing at predicting the dependent variable. For linear regression, a common loss function is the mean squared error (MSE).

- Calculate the gradient of the loss function: You will need to calculate the partial derivative of the loss function with respect to each of the model parameters (b0 and b1). This will tell you the direction and amount that the parameters need to change to reduce the loss.

- Update the model parameters: Using the gradients calculated in the previous step, you can update the model parameters using gradient descent. This involves updating the parameters by subtracting a small fraction of the gradient from each parameter.

- Repeat steps 3-5 until convergence: You will need to repeat these steps until the model converges, meaning that the parameters are no longer changing significantly with each iteration. This can be determined by checking the change in the loss function from one iteration to the next


**Loss Functions:**
- In linear regression, the most commonly used loss function is the mean squared error(MSE), given by the equation, **loss = (1/n) * ∑(predicted-actual)^2**
-  Another commonly used loss function is the Mean Absolute error (MAE), given by the equation, **loss = (1/n) * ∑|predicted-actual|**

🎯 Choosing the loss function completely depends on the problem one is trying to solve.

🎯 In general, MSE is more commonly used because it penalises large errors more heavily than MAEmwhich can be helpful in certain areas, and also MAE is computationally more expensive than MSE

🎯 MAE is less sensitive to outliers in the data and can be used in cases where there are a few substantial errors, that should not heavily influence overall loss 
