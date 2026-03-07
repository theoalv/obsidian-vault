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
$$
P_N(r,t)\simeq\frac{e^{-ct/l}}{\pi l^3}\frac{\Gamma\left(\frac{3}{4}N+\frac{3}{2}\right)}{\sqrt{\pi}N!\Gamma\left(\frac{3}{4}N\right)}\left(\frac{ct}{l}\right)^{N-3}\times\left(1-\frac{r^2}{c^2t^2}\right)^{\frac{3}{4}N-1}\Theta(ct-r)
\tag{35}
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
