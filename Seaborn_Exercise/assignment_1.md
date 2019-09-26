# Explain the difference in the normalization constant in variance/covariance formula


The logic of doing that is to compensate our lack of information about the population data.
This correction is made to correct for the fact that these sample statistics tend to underestimate the actual parameters found in the population. they tend to contain a little bias. subtracting 1 from the sample size correct the bias.
when you work with a sample you’ve only got a small fraction of the population to work with. Therefore, your answers aren’t going to be as accurate as those you would have got, if you had the entire set of data to work with.

In the case of the sample variance the particular statistic you are working with is the sample mean (x̄) instead of the population mean(μ). Any x-value in your sample is going to be closer to x̄ than to μ.

sample calculations with n in the denominator are almost always going to be higher than calculations with n-1 in the denominator (Warne, 2017). When you subtract 1 from your sample size, it happens to turn out you’re making a fairly good adjustment for the deflated sum of squares figure as long as n isn’t huge (Edelman, 2018)


![Image result for covariance formula](https://cdn.educba.com/academy/wp-content/uploads/2019/05/Covariance-Formula.jpg)
In python the covariance matrix can be easily calculated with
## np.cov

Covariance measure  how much two random variables vary together. It’s similar to variance, but where variance tells you how a single variable varies, co variance tells you how two variables vary together.
The formula is:
<p>Cov(X,Y) = Σ E((X-μ)E(Y-ν)) / n-1 where:</p>
<p>X is a random variable</p>
<p>E(X) = μ is the expected value (the mean) of the random variable X and</p>
<p>E(Y) = ν is the expected value (the mean) of the random variable Y</p>
<p>n = the number of items in the data set</p>

# example

##  Calculate covariance for the following data set:

<p>x: 2.1, 2.5, 3.6, 4.0 (mean = 3.1)</p>
<p>y: 8, 10, 12, 14 (mean = 11)</p>

Substitute the values into the formula and solve:
<p>Cov(X,Y) = ΣE((X-μ)(Y-ν)) / n-1 </p>
<p>= (2.1-3.1)(8-11)+(2.5-3.1)(10-11)+(3.6-3.1)(12-11)+(4.0-3.1)(14-11) /(4-1)</p>
<p>= (-1)(-3) + (-0.6)(-1)+(.5)(1)+(0.9)(3) / 3</p>
<p>= 3 + 0.6 + .5 + 2.7 / 3</p>
<p>= 6.8/3</p>
<p>= 2.267</p>

The result is positive, meaning that the variables are positively related.

