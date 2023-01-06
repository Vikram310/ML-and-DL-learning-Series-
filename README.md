**Linear Regression :**

- Linear regression is a statistical method used to model the linear relationship between a dependent variable and an independent variable by fitting a linear equation to the observed data
- The goal of linear regression is to find the line equation that best fits the data, called the “line of best fit” 
- Equation of Linear regression -> y = w0 + w1x, where w0 and w1 are the weights/coefficients, which need to be calculated and are chosen to minimise the error between the predicted value and observed value 

**Loss Functions:**
- In linear regression, the most commonly used loss function is the mean squared error(MSE), given by the equation, **loss = (1/n) * ∑(predicted-actual)^2**
-  Another commonly used loss function is the Mean Absolute error (MAE), given by the equation, **loss = (1/n) * ∑|predicted-actual|**

🎯 Choosing the loss function completely depends on the problem one is trying to solve.

🎯 In general, MSE is more commonly used because it penalises large errors more heavily than MAEmwhich can be helpful in certain areas, and also MAE is computationally more expensive than MSE

🎯 MAE is less sensitive to outliers in the data and can be used in cases where there are a few substantial errors, that should not heavily influence overall loss 
