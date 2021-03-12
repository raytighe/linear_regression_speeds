# Fastest Way to Fit OLS Regression Models in Python

In this analysis I compare the runtimes of different methods to fit an ordinary least squares regression model. I fit a multivariate normal random sample using Scikit-Learn’s Linear Model module, statsmodels’ sm module, and with simple matrix multiplication. The result was three clear runtime distributions with simple matrix multiplication having the fastest mean runtime, followed by the Scikit-Learn then statsmodels methods. The results suggest that the most computationally efficient method for fitting ordinary least squares regression models with 0 intercept is using Numpy’s vectorized matrix multiplication. However, in practice, the average runtimes differ by hundredths of seconds so the relevant efficiency gains may be negligible.

![alt text](https://github.com/raytighe/linear_regression_speeds/blob/main/figures/results.png)
