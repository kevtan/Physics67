# Final Project for PHYSICS 67

For the final project, I learned more about model fitting using a very simple constant model. In particular, I practiced taking the first and second derivatives of a summation expression (i.e., the $\chi^2$ value) in order to derive closed-form expressions for the minimum value and uncertainty.

## First Derivative

Recall that $\chi^2 = \sum_i \left( \frac{n_i - p_0}{\sigma_i} \right)^2$. Thus, $\frac{d}{dp_0} \chi^2 = \sum_i 2 \left( \frac{n_i - p_0}{\sigma_i} \right) \left( -\frac{1}{\sigma_i} \right) = -2 \sum_i \frac{n_i - p_0}{\sigma_i^2}$.

## Second Derivative

From above, $\frac{d}{dp_0} \chi^2 = -2 \sum_i \frac{n_i - p_0}{\sigma^2}$. Thus, $\frac{d^2}{dp_0^2} = 2 \sum_i \frac{1}{\sigma_i^2}$.

## Discussion I

By visual inspection, the plots I came up with by deriving the closed-form expressions for the first- and second-derivatives match the ones produced using numerical methods for derivative computation.

## Optimizing $\chi^2$

$$
\begin{align*}
  \frac{d}{dp_0} \chi^2 &= 0\\
  -2 \sum_i \frac{n_i - p_0}{\sigma_i^2} &= 0\\
  \sum_i \frac{n_i - p_0}{\sigma_i^2} &= 0\\
  \sum_i \frac{n_i}{\sigma_i^2} - \sum_i \frac{p_0}{\sigma_i^2} &= 0\\
  \sum_i \frac{n_i}{\sigma_i^2} - p_0 \sum_i \frac{1}{\sigma_i^2} &= 0\\
  \sum_i \frac{n_i}{\sigma_i^2} &= p_0 \sum_i \frac{1}{\sigma_i^2}\\
  p_0 &= \boxed{\frac{\sum_i \frac{n_i}{\sigma_i^2}}{\sum_i \frac{1}{\sigma_i^2}}}
\end{align*}
$$

## Solving for the Uncertainty

Note that $\Delta \chi^2 = a (\delta p_0)^2$ where $a = \frac{1}{2} \frac{d^2}{dp_0^2} \chi^2 \approx 0.23$. Furthermore, note that $a \sigma_{p_0}^2 = 1$. Solving for $\sigma_{p_0}$ gives us $\sigma_{p_0} = 0.877$.

## Discussion II

The expressions obtained for $p_0$ and $\sigma_{p_0}$ are exactly those obtained from inverse variance weighting!
