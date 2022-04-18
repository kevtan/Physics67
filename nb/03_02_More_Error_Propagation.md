# Questions for Discussion

## 3.1

> Explain, in your own words, what is being shown in the two plots above. How does this relate to the uncertainty on the measurement of l.

The first of the two plots above shows the *absolute* spread of the simulated length measurements whereas the second shows the *relative* spread.

## 4.1

> Explain, again in your own words, what is being shown in the two plots above. How does this relate to the formula shown above, in particular the formula that includes the partial derivatives?

The first of the two plots above shows the linear relationship between the *absolute* length and area of desk whereas the second shows the linear relationship between these quantities on a *relative* scale. This relates to the formula with the partial derivatives because, when the only source of uncertainty is $l$, the formula reduces to

$$\frac{\delta A}{A} = \frac{\delta l}{l}$$

which is exactly the relationship captured in the second plot.

## 5.1

> How can we interpret the two plots above? What does it mean for our estimate of the uncertainty on A?

The first of the two plots above shows the *absolute* spread of the simulated area measurements whereas the second shows the *relative* spread. The second plot suggests that the uncertainty on A is 10% (i.e., the same as the uncertainty on length).

## 6.1

> How can we interpret the two plots above? What does it mean for our estimate of the uncertainty on A?

The first of the two plots above clearly shows that the relationship between the card length $C$ and the desk area $A$ is nonlinear (in fact it's quadratic). Because the slope of the orange line—the tangent at zero—is 2, we know $\frac{\delta A}{A} = 2\frac{\delta C}{C}$. This means that the relative uncertainty of $A$ should be twice that of the relative uncertainty of $C$. The second plot corroborates this fact because the relative uncertainty of $A$ is 20% when the relative uncertainty of $C$ is 10%.

## 6.2

> Why does this differ from the results we got when we considered the variation in A due to the variation in l?  

Because $A$ depends linearly on $l$ but quadratically on $C$ (recall that $A = wlC^2B^2$).

## 6.3

> Why did we draw the tangent line on the figure a few cells up?

Because the slope of this line tells us the constant factor in front of $\frac{\delta C}{C}$. The tangent line corresponds to the partial derivative term in the equation for the propagation of errors.

## 7.1

> This plot, and the plot before, are two dimensional versions of the plots what we used to illustrate how changes in one input variable cause changes in the outcome. Explain these plots, and what we can learn from them, in your own words.

These plots rely on a color map as the 3rd dimension to represent things like the fractional change in $A$ or the number of simulations. The first plot teaches us that not to expect the relative uncertainty in $A$ due to the 10% uncertainty in both $l$ and $w$ to be as large as the sum of the relative uncertainty in A due to a 10% uncertainty in $l$ and $w$ separately because, sometimes, the variations in $l$ and $w$ will tend to cancel each other out. These variations in $l$ and $w$ that cancel each other out occur along the line cutting diagonally from the top left corner to the bottom right corner in plot 2.

## 8.1

> Put it all together. Explain this plot in terms of what we have done and your understanding of propagation of errors.

As we can see, the relative uncertainty in $A$ here is not 20% (which would be the case if the relative uncertainty were the sum of the relative uncertainties under the assumptions of 10% variations in $l$ and $w$ independently). Instead, it's only 14%. This makes sense when considering the equation for the relative uncertainty (shown below).

$$\frac{\delta A}{A} = \sqrt{\left(\frac{\delta l}{l}\right)^2 + \left(\frac{\delta w}{w}\right)^2} = \sqrt{0.01 + 0.01} = \sqrt{0.02} \approx \boxed{0.1414}$$
