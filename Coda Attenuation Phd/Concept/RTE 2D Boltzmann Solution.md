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
in transport region $r<ct$ --> distribution of scattered particle
in front of wave $r>ct$ intensity is zero

for higher scattering level case $l=0.3$ 
![[Pasted image 20260307134426.png]]
Ballistic intensity is significantly reduced, as most energy is scattered
scattering tail dominates this case as $l$ is low

for lower scattering level case $l=5$
![[Pasted image 20260307134632.png]]
little to no scattering occured in this case, most of energy is in ballistic
it is evident that ballistic intensity is energy that not yet scattered, the probability of scattering is controlled by $l$ value

2D space-time map simulation
with same configuration, here is map for moderate scattering $l=1$
![[Pasted image 20260307144750.png]]
white area is zero intensity area, as $c=1$ then $t=r$
ballistic is in $t=r$ line, as there is moderate scattering then ballistic intensity at low distance is stronger

high scattering case $l=0.3$
![[Pasted image 20260307145143.png]]
in this case, the ballistic intensity is gone at high distance
scattered intensity is higher and still evident in longer time

low to no scattering case $l=5$
![[Pasted image 20260307145701.png]]
in this case, scattering intensity is low and nearly uniform
most of intensity concentrated near wavefront $r=t$ as higher $l$ means lower probability of scattering