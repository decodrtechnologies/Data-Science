## Lasso and Ridge Regression: A comprehensive guide

### Overview

    Ridge and Lasso Regression are types of Regularization techniques
    Regularization techniques are used to deal with overfitting and when the dataset is large
    Ridge and Lasso Regression involve adding penalties to the regression function
    
    
### Introduction

When we talk about Regression, we often end up discussing Linear and Logistic Regression. But, that’s not the end. Do you know there are 7 types of Regressions?

Linear and logistic regression is just the most loved members from the family of regressions.  Last week, I saw a recorded talk at NYC Data Science Academy from Owen Zhang, Chief Product Officer at DataRobot. He said, ‘if you are using regression without regularization, you have to be very special!’. I hope you get what a person of his stature referred to.

The overall idea of regression remains the same. It’s the way in which the model coefficients are determined which makes all the difference.
Ridge and Lasso regression are powerful techniques generally used for creating parsimonious models in presence of a ‘large’ number of features. Here ‘large’ can typically mean either of two things:

Large enough to enhance the tendency of a model to overfit (as low as 10 variables might cause overfitting)
Large enough to cause computational challenges. With modern systems, this situation might arise in case of millions or billions of features

Though Ridge and Lasso might appear to work towards a common goal, the inherent properties and practical use cases differ substantially. If you’ve heard of them before, you must know that they work by penalizing the magnitude of coefficients of features along with minimizing the error between predicted and actual observations. These are called ‘regularization’ techniques. The key difference is in how they assign penalty to the coefficients:

Ridge Regression:<br>

        Performs L2 regularization, i.e. adds penalty equivalent to square of the magnitude of coefficients
        Minimization objective = LS Obj + α * (sum of square of coefficients)
Lasso Regression:<br>

        Performs L1 regularization, i.e. adds penalty equivalent to absolute value of the magnitude of coefficients
        Minimization objective = LS Obj + α * (sum of absolute value of coefficients)

Note that here ‘LS Obj’ refers to ‘least squares objective’, i.e. the linear regression objective without regularization.


### Installation
 
1. Clone the repo
```sh
git clone https://github.com/github_username/repo.git
```
2. Install Jupyter notebook
3. Install Python packages


### Contributing

Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

<br>
Project Link: [https://github.com/decodrtechnologies/Data-Science](https://github.com/decodrtechnologies/Data-Science)
