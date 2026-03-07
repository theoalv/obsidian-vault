Ref [[paasschens1997]]
[[RTE 1D Boltzmann Solution]]
[[Fourier Transformed Intensity]]
derived from
[[IFT Intensity 4D]]

The solution of 4D Boltzmann RTE is based from FT of intensity.
The full formula FT Eq 18 is defined for 4D space then IFT to obtain intensity solution in time-space domain

Total Intensity 4D solution
$$
P(r,t)=\frac{e^{-ct/l}}{2\pi^2r^3}\delta(r-ct)+\frac{1}{(\pi lct)^2}\left(1-\frac{r^2}{c^2t^2}+\frac{2l}{ct}\right)\times exp(-r^2/lct)\Theta(ct-r)
\tag{31}
$$
Angular intensity Solution
$$
P(r,t,\mu)=\frac{\pi e^{-ct/l}}{2r^3}\delta(r-ct)\delta(\mu-1^-)(1-\mu^2)^{-1/2}+\frac{exp(-r^2/lct)}{(\pi lct)^2}\times \frac{(1-y^2)(1+y^2-2\mu y)+2(1-\mu y)l/ct}{1+y^2-2\mu y}^2\times \Theta(ct-r)
\tag{32}
$$where  $y =r/ct$ 
