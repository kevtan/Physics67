# Questions for Discussion

## 5.1

> One key difference between the Fourier transform of time-based signals and 2D images is that the data in each case is a function of different dimensions: time and space, respectively. What units are used for the corresponding "spatial frequency" in each direction (x and y) in the examples above? Does this make sense in the context of the previous notebook with our time-based signals and Fourier-transformed frequency space plots?

The units we use when analyzing signals that vary over space are inverse meters (i.e., inverse distance), which makes sense considering the units we use when analyzing signals that vary over time are inverse seconds (i.e., inverse time).

## 5.2

> We also have to consider the direction of the plane waves, so now we describe each possible wave not as a single frequency but as a vector with two values corresponding to each axis of the transformed image (written as $k_x$ and $k_y$ above). We call this quantity the "wavevector," and in each example above the wavevector points from the origin to the points with non-zero amplitude (the yellow dots). Why are there two wavevectors for a single plane wave? Hint: consider the symmetry of the plane wave in the original image.

There are 2 wavevectors for a single plane wave because we can consider the plane wave to be either moving right (i.e., in the +x direction) or left (i.e., in the -x direction).

## 6.1

> Before you run the code below that takes the Fourier transform of the above image, how do you expect the circular ripples will appear in 2D frequency space? Discuss with your groups then make your best guess, and justify your answer. Hint: again, think of the symmetries involved.

I expect the circular ripples to appear as circles of points in 2D frequency space. I think it should be a circle because I believe the wave number should be the same in all directions.

## 6.2

> Now that you have seen the transformed signal, can you explain how the ripples in the original image transform into the circular features in the Fourier transform? You can ignore the vertical and horizontal lines running through the center; these are due to the finite size of the image.

As predicted, the image's 2D frequency space representation was a circle. This must be due to the fact that circular ripples are the superposition of plane waves—of the same wave number—emanating in all directions.

## 7.1

> We mentioned above that the wavevectors describing the electronic plane wave states have an associated momentum defined by $\vec{p} = \hbar \vec{k}$. Using this relationship and the plot above, estimate the Fermi energy of Copper. Remember how momentum is related to kinetic energy in order to get the right formula, and also use the fact that the electrons in Copper have an effective mass $m_e = 0.38 \cdot m_0$, where $m_0$ is the rest mass of an electron (you can look up this value online). Ask the teachers for the actual value measured, and if you do this right you will have measured the Fermi energy to about 5 percent with very simple data processing.

The circle has a radius of $0.5 \texttt{ Angstroms}^{-1}$ so the Fermi wave number is $0.25 \texttt{ Angstroms}^{-1}$.

$$E = \frac{(\hbar c)^2k^2}{2m_ec^2} = \frac{(2000 \texttt{ eV} \texttt{ Angstroms})^2(0.25 \texttt{ Angstroms}^{-1})^2}{2 \cdot 0.38 \cdot 0.51 \texttt{ MeV}} = \boxed{0.645 \texttt{ eV}}$$

This is close to the measured Fermi energy of electrons at the surface of copper: $0.6\texttt{ eV}$.