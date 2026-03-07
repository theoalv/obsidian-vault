Ref [[paasschens1997]]
related to
[[RTE 1D Boltzmann Solution]]
[[Fourier Transformed Intensity]]
derived from
[[IFT Intensity 2D]]

The solution of 2D Boltzmann RTE is based from FT of intensity.
The full formula FT Eq 18 is defined for 2D space then IFT to obtain intensity solution in time-space domain

Total Intensity 2D solution
$$
P(r,t)=\frac{e^{-ct/l}}{2\pi l^2}\delta(ct-r)+\frac{1}{2\pi lct}\left(1-\frac{r^2}{c^2t^2}\right)^{1/2}\times exp[l^{-1}(\sqrt{c^2t^2-r^2}-ct)]\Theta(ct-r)
\tag{23}
$$
Angular intensity Solution
$$
P(\mathbf{r},t,\mathbf{\hat{s}})=e^{-ct/l}\delta(\mathbf{r}-ct\mathbf{\hat{s}})\Theta(t)+\frac{1}{2\pi l(ct-\mathbf{r}\cdot\mathbf{\hat{s}})}\times exp[l^{-1}(\sqrt{c^2t^2-r^2}-ct)]\Theta(ct-r)
\tag{26}
$$

Total intensity 2D simulation
use $c=1$ with $t=2,4,6$  
if $l=1$ or moderate scattering level
![[Pasted image 20260307133922.png]]
spike is ballistic peak, for this case small amount of scattering occured
high spike --> strong ballistic intensity, low scattering
in transport region $r$