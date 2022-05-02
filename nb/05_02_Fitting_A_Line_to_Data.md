# Questions for Discussion

## 4.1

> What do you think about our model? Is this a sensible model? What would it mean if $p_0$ were very different from 0? What about if $p_1$ were different from zero?

I have no qualms with the model so far; I think it's a sensible starting point because linear models are simple and, following the philosophy of Occam's razor, make few assumptions. If $p_0$ were very different from zero, then the excess in mid-2014 would be very different from zero. The more $p_1$ is different from zero, the more that the excess either increases or decreases over time.

## 5.1

> Using what we learned last week about Gaussian distributions and p-values, explain why the two plots with the scaled residuals are much more useful than the two plots with the unscaled residuals.

The plots with the scaled residuals are much more useful than those with the unscaled residuals because measuring spread in terms of $\sigma$ is far more semantically meaningful; it's easier to convert between $\sigma$ values and probabilities.

## 5.2

> Given the plot above, do you think that there is any chance that the true value of $p_1$ is actually 20 counts/year? Explain why or why not.

No, I highly doubt the true value of $p_1$ is actually 20 counts per year because there's a clear linear relationship in the scatter plot of residuals. Generally speaking, this is a telltale sign that the model is a poor fit for the data; we want there to be no noticeable pattern in the residuals. This is also corroborated by the histogram of residuals, where the spread of residuals is much higher for the $p_1 = 20$ model than it is for the $p_1 = 0$ model. This is undesirable because we want to residuals—a measure of the error in model predictions—to be as low as possible.

## 6.1

> We just saw that in an idealized case, the chance of seeing the observed data given model parameters (0.,20.) is astonishingly less likely (by a factor of $10^{126}$ than the change of seeing the observed data if the model parameters were (0., 0.). Explain why this is, using information from the plots above question 5.2.

This is because the residuals for the $(p_0, p_1) = (0, 20)$ model were much larger than those for the $(p_0, p_1) = (0, 0)$ model. This contributed to a larger $\chi^2$ value and a smaller survival function value (which corresponds to the probability of seeing the observed data given the model parameters).

## 7.1

> Estimate numerical values for the best-fit values and 1 $\sigma$ uncertainties on $p_0$ and $p_1$ using the two plots above.

* The best-fit value for $p_0$ is around -2 and the $1\sigma$ uncertainty for that parameter is around 2.
* The best-fit value for $p_1$ is around 0 and the $1\sigma$ uncertainty for that parameter is around 0.5.

## 8.1

> Is this result statistically significant? I.e., should we write a paper saying that Vela is getting dimmer? Why or why not?

No we should not because the probably of observing $p_1 = 0.13$ given that the true value is $0$ is too high: $0.82$. That is, it's very likely that the slope is actually zero and that the Vela Pulsar is not actually getting dimmer.
