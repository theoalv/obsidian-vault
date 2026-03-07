Ref [[paasschens1997]]
related to
[[RTE 1D Boltzmann Solution]]
[[Fourier Transformed Intensity]]
[[RTE 2D Boltzmann Solution]]
[[RTE 4D Boltzmann Solution]]
derived from
[[IFT Intensity 3D]]

The 3D IFT cannot be directly solved analytically in same approach as 2D and 4D.
The solution only applicable for N = 0,1 and impossible for other N value.
The proposed solution is by doing interpolation between 2D and 4D

Total intensity formulation for 3D
Total intensity
$$
P(r,t)\simeq\frac{e^{-ct/l}}{4\pi r^2}\delta(r-ct)+\frac{(1-r^2/c^2t^2)^{1/8}}{(4\pi lct/3)^{3/2}}e^{-ct/l}\times G\left(\frac{ct}{l}\left[1-\frac{r^2}{c^2t^2}\right]^{3/4}\right)\Theta(ct-r)
\tag{36a}
$$
where
$$
\begin{aligned}
G(x)
&=8(3x)^{-3/2}\sum_{N=1}^{\infty}\frac{\Gamma\left(\frac{3}{4}N+\frac{3}{2}\right)}{\Gamma\left(\frac{3}{4}N\right)}\frac{x^N}{N!}\\
&\simeq e^x\sqrt{1+2.026/x}
\end{aligned}
\tag{36b}
$$
when $r,l<<ct$ the expression become diffusion solution
diffusion coefficient $D=\frac{cl}{3}$ 

simulation for different distances
![[Pasted image 20260308065441.png]]
after ballistic arrival there is decaying tails
however at larger times (4) the curve approaches diffusive profile