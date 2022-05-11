# Questions for Discussion

## 4.1

> About far away is this object? You can estimate it based on Hubble's law $v = H_0 d$. You can use the Hubble parameter is about $H_0 = 70 \frac{{\rm km}}{{\rm s}}{\rm Mpc}^{-1}$. The speed of light is about $c = 3 \times 10^8 m/s$ and $1 {\rm pc} = 3.26 {\rm ly}$.

$$
d = \frac{v}{H_0} = 169.714 \texttt{ Mpc} = 553.269 \texttt{ Mly}
$$
## 5.1

> Before going further, it is important to make sure you understand the previous plot and what we did to make it. So, describe the plot and how we made it, and what it means. What is the difference between this plot and the plot we made for the initial guess of the model parameters?

The plot shows that that our fitted model approximates the observed data far better than our initial guess. We obtained the fitted model by minimizing the $\chi^2$ value w.r.t. our 5 model parameters. The difference between this plot and the previous one is that this one has a much lower $\chi^2$ value because we explicitly minimized it w.r.t. to our model parameters.

## 6.1

> How would you interpret the fit result? Do the parameters make sense? What might have happened? Don't worry if you aren't sure. Just guess.

The fit is pretty good at the peak, but bad everywhere else. This is due to the fact that we're not accounting for the baseline light flux across the entire spectrum.

## 7.1

> What happened? How would you interpret the fit result? Do the parameters make sense?

This time, the optimizer returned a terrible, nonsensical result. The parameters don't make any sense (e.g., "Line Width: -1228.2635 \[nm\]").

## 7.2

> Try to guess about why we got this result. What might have happened? Don't worry if you aren't sure. Just guess.

This must be because the cost function is not convex and there are many local optima, which makes the optimization result very sensitive to the specific choice of initialization.

## 7.3

> This illustrates that it is often important to start with a reasonable initial guess. If we were fitting millions of spectra, we would want the program to make the initial guess instead of having to do it by hand. How might you make an initial guess for the a) Line Peak, b) the Line Width, c) the Background at 500 nm, d) the Background slope?

* a) I might guess the difference between the largest and smallest flux values in the wavelength band of interest.
* b) I might guess half the distance between the left and right sides of the peak.
* c) I might guess the minimum value in the wavelength band of interest.
* d) I might just make this 0.
