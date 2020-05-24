## T- Test
T-test is mostly used to check the difference in the means of two samples

Two sample t-test independent sample t-test is used to check whether the means of two samples(group) are same or different. We want to check whether the number of bikes rented on working day are different then number of bikes rented on non-working days.

**Steps for performing hypothesis testing**
1. set up Null Hypothesis (H0)
2. State the alternate hypothesis (H1)
3. Set a significance level (alpha)
4. Calculate test Statistics.
5. Decision to accept or reject null hypothesis.

## Assumption for T-Test
1. The variances of the 2 samples are equal(We will use Levene's test to check this assumption).
2. The distrubtion of the residuals b/w the two groups should follow the normal distribution. We can plot histogram and see whether the distribution follows the normal distribution or not. We can also plot a Q-Q plot. We can check the normality using shapiro-wilks test as well.

## License
[Dataset Link](http://archive.ics.uci.edu/ml/datasets/Bike+Sharing+Dataset)

**CITATION** 

Fanaee-T, Hadi, and Gama, Joao, 'Event labeling combining ensemble detectors and background knowledge', Progress in Artificial Intelligence (2013): pp. 1-15, Springer Berlin Heidelberg.

    @article{
    year={2013},
    issn={2192-6352},
    journal={Progress in Artificial Intelligence},
    doi={10.1007/s13748-013-0040-3},
    title={Event labeling combining ensemble detectors and background knowledge},
    url={[Web Link]},
    publisher={Springer Berlin Heidelberg},
    keywords={Event labeling; Event detection; Ensemble learning; Background knowledge},
    author={Fanaee-T, Hadi and Gama, Joao},
    pages={1-15}
    }
