<h1>Polynomial Regression</h1>

<h3>Introduction To Polynomial Regression</h3>

In statistics, polynomial regression is a form of regression analysis in which the relationship between the independent variable x and the dependent variable y is modelled as an nth degree polynomial in x. Polynomial regression fits a nonlinear relationship between the value of x and the corresponding conditional mean of y, denoted E(y |x).
Although polynomial regression fits a nonlinear model to the data, as a statistical estimation problem it is linear, in the sense that the regression function E(y | x) is linear in the unknown parameters that are estimated from the data. For this reason, polynomial regression is considered to be a special case of multiple linear regression.

<h3>Advantages of using Polynomial Regression</h3>

Polynomial provides the best approximation of the relationship between the dependent and independent variable. A Broad range of function can be fit under it. Polynomial basically fits a wide range of curvature.

<h3> Uses of Polynomial Regression</h3>

These are basically used to define or describe non-linear phenomenon such as
 - Growth rate of tissues.
 - Progression of disease epidemics
 - Distribution of carbon isotopes in lake sediments
The basic goal of regression analysis is to model the expected value of a dependent variable y in terms of the value of an independent variable x. In simple regression, we used following equation –
 - y = a + bx + e
Here y is dependent variable, a is y intercept, b is the slope and e is the error rate.

In many cases, this linear model will not work out For example if we analyzing the production of chemical synthesis in terms of temperature at which the synthesis take place in such cases we use quadratic model
 - y = a + b1x + b2^2 + e
Here y is dependent variable on x, a is y intercept and e is the error rate.

In general, we can model it for nth value.
 - y = a + b1x + b2x^2 +....+ bnx^n

Since regression function is linear in terms of unknown variables, hence these models are linear from the point of estimation.
Hence through Least Square technique, let’s compute the response value that is y.

<h3>Problem Defination</h3>
 
The main aim to this project is to how to implement Polynomial Regression From Scratch. Here i have took example of A person approaches with a job application towards HR team. At the time of Salary negotition the applicant demands some amount for assigned job. Then the HR team look up at his past data and using this algorithm can predict his actual value and guess wether the person is saying Truth or Bluffing.

<h3>Install</h3>
- Supported Python version - Python version used in this Project : 3.5+

<h3>Run</h3>
 - To run this project use - Anaconda, which provides support for running .ipynb files (Jupyter Notebook)
  - After making sure you have that, you can run from a terminal or cmd next lines
  - ipython notebook Poly_Reg_Test.ipynb
