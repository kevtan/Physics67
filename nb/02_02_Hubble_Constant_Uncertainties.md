# Questions for Discussion

## 4.1

> What do we learn from the figure with the error bars included as opposed to the histogram? Does it change your estimate of what the true value of the Hubble parameter is?

The figure with the error bars give us an intuitive notion of the fidelity/confidence of each measurement, as opposed to the measurements themselves. Yes, looking at the figure with the error bars, I update my estimate for the true value of the Hubble constant is around 72 km/s/Mpc (as opposed to "somewhere in the range 68-77 km/s/Mpc").

## 4.2

> There is no single true value that is consistent with all (or even most) of the measured values. What do you think that means?

That doesn't mean too much; just because a value doesn't lie within the error bars of a measurement doesn't mean it's fundamentally incompatible with the measurement! Instead, it just means that, given the measurement, the probability the true value is outside the error bars is rather low.

## 4.3

> Before proceeding, describe a way that you might derive an estimate of the true value of the Hubble parameter (and an uncertainty on that value) that uses both the measured values and their stated uncertainties.

One way is to turn each of the measurement-uncertainty pairs into an appropriate probability distribution. Then, in order to combine all the probability distributions together, we can multiply them together and normalize the result. The result would also be a probability distribution; the estimate of the true value could be the expected value and the uncertainty could be the standard deviation or variance.

## 5.0

> Even though all of the measurements are being simulated from the same distribution, the different groups of scientists are reporting different uncertainties for their best estimates. Why is that?

Because the different groups of scientists made different numbers of measurements. The groups that made more measurements had more certainty and vice versa.

## 5.1

> In your own words, describe what is being presented in the previous plot and the two cells before that.

The previous plot and the two cells before that explore different ways we can reconstruct the true mean and error given only the means and errors from the different groups of scientists. The plot makes it rather obvious to see that the weighted mean was much closer to the true mean than the straight mean.

## 5.2

> In this case, the different methods of combining the results give quite similar, but not identical, final answers.

I think the results obtained from using the full sample and weighted mean are "consistent enough" because the true mean falls within their error bars. However, applying the same logic, I wouldn't say the straight mean is "consistent enough."

## 5.3

> The usual convention for combining results is to use variance weighting (i.e., the weighted mean as computed here). Does that seem like a sensible convention to you? Why or why not?

Yes, because each sample mean is effectively given the weight $\frac{n_i}{\sigma_i^2}$ where $n_i$ is the number of measurements that went into the sample mean and $\sigma_i^2$ is the variance. The effect of this is that the weight increases when $n_i$ increases and decreases when $\sigma_i^2$ increases which, intuitively, are the behaviors we'd like to see.

## 6.1

> In this case the weighted mean doesn't quite agree with the straight mean. Looking at the plot, why do you think that is?

I think it's because there are few measurements with extremely short error bars at around 67.5 km/s/Mpc. These measurements would be given exceedingly large weights and thus pull the weighted mean leftwards.

## 6.2

> Does this change what you think about what the best estimate of the Hubble parameter (and it's uncertainty) might be? Why? What about the uncertainty on the Hubble parameter?

No, I still think the best estimate of the Hubble parameter is around 72 km/s/Mpc (i.e., close to the true mean) because the measurements with extremely short error bars seem to disagree with the vast majority of the other measurements and, so, were potentially subject to some systematic biasing errors. As I didn't have a concrete notion of how large the uncertainty should be in the first place, these findings didn't change my thoughts on the uncertainty in the measurements.
