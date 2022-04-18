# Questions for Discussion

## E.1

> Measure the area of your desk, and compute how much your estimate would change in both absolute and relative terms if:
>
> (A) You had C_m wrong by 1 cm.
> (B) You had w_m wrong by 10%.
>
> Paste your work (including your values of l_m, w_m, B_m, C_m into the google doc template.

The values I measured were $C_m = 8.5$, $B_m = 3.85$, $l_m = 3.3$, and $w_m = 2.05$; these values gave me $A_m = 7244.81$. If I had $C_m$ wrong by 1 cm (i.e., by underestimating it by 1 cm), then the true area would be $A_m' = 9049.75$. This is 1804.94 greater, or, equivalently, 24.91% larger. If instead I had $w_m$ wrong by 10% (i.e., by underestimating it by 10%), then the true area would be $A_m'' = 7969.29$. This is 724.48 greater, or, equivalently, 10% larger.

## 1.1

> Connect the three figures we made above (cases 1, 2 and 3) to the formula for the propagation of errors given just above. Explain what corresponds to what, and if the numerical results that we got match the formula. Also explain the difference in the outcomes in the three cases in simple English.
>
> There is a lot going on here. So you should provide a lot of details.

First and foremost, the quantity of interest is a product so the two rules for error propagation apply (and the third does not). In case 1, where we had a 10% relative error for $l$, adding in quadrature would have given us the following, which matches the results from the figure. As you can see, the resultant uncertainty for the area is 10%.

$$\frac{\delta A}{A} = \sqrt{\left(\frac{\delta l}{l}\right)^2} = \frac{\delta l}{l} = \boxed{0.1}$$

In case 2, where we had a 10% relative error for $C$, adding in quadrature would have given us the following, which—again—matches the results from the figure. As you can see, the resultant uncertainty for the area is 20%.

$$\frac{\delta A}{A} = \sqrt{\left(2\frac{\delta C}{C}\right)^2} = 2\frac{\delta C}{C} = \boxed{0.2}$$

Finally, in case 3, where we had a 10% relative error for both $l$ and $w$, adding in quadrature would have given us the following, which—yet again—matches the results from the figure. As you can see, the resultant uncertainty for the area is 14%.

$$\frac{\delta A}{A} = \sqrt{\left(\frac{\delta l}{l}\right)^2 + \left(\frac{\delta w}{w}\right)^2} = \sqrt{0.01 + 0.01} = \sqrt{0.02} \approx \boxed{0.14}$$

## 1.2

We used random numbers to simulate the uncertainty in the measurement of variables that factor into the calculation of a quantity of interest and propagate that uncertainty through a computation to find the uncertainty of the quantity of interest. I thinks it's a good technique in the sense that it allows you to develop intuition for the propagation of error and approach the problem in less of an abstract manner. However, it has its limitations because the error measurements are going to be less precise (the true number could only be obtained in the limit as the number of measurements tends to infinity).

## 2.1

For the first example (i.e., observing the sun with a simple photo-detector), we have

$$\frac{\delta F_E}{F_E} = \sqrt{\left(\frac{\delta \hat{E}_\gamma}{\hat{E}_\gamma}\right)^2 + \left(\frac{\delta n_\gamma}{n_\gamma}\right)^2 + \left(\frac{\delta \eta}{\eta}\right)^2} = \sqrt{0.03^2 + 0.02^2 + 0.02^2} \approx \boxed{0.0412}$$

and

$$\frac{\delta P}{P} = \sqrt{\left(\frac{\delta F_E}{F_E}\right)^2} = \frac{\delta F_E}{F_E} \approx \boxed{0.0412}.$$

For the second example (i.e., observing the distant gamma ray pulsar Vela with a space-based telescope that's sensitive to gamma rays), we have

$$\frac{\delta F_E}{F_E} = \sqrt{\left(\frac{\delta \hat{E}_\gamma}{\hat{E}_\gamma}\right)^2 + \left(\frac{\delta n_\gamma}{n_\gamma}\right)^2 + \left(\frac{\delta \eta}{\eta}\right)^2 + \left(2\frac{\delta d}{d}\right)^2} = \sqrt{0.05^2 + 0.03^2 + 0.05^2 + 0.4^2} \approx \boxed{0.407}$$

and

$$\frac{\delta P}{P} = \sqrt{\left(\frac{\delta F_E}{F_E}\right)^2} = \frac{\delta F_E}{F_E} \approx \boxed{0.407}.$$

The total relative uncertainties are indeed roughly what I'd expect knowing the rules of adding in quadrature for error propagation. These results suggest that if we have an input with a large power and/or a great deal of associated uncertainty, we can largely ignore the uncertainties of the other inputs and still have a very good estimate of the resultant uncertainty. This is clearly shown in the second example where, if we were to have only considered the uncertainty in the distance $d$, we would've obtained an uncertainty in energy flux and power of $0.4$ (which is extremely close to $0.407$).
