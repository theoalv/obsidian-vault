Ref [[paasschens1997]]
Related to
[[RTE 1D Boltzmann Solution]]
[[Fourier Transformed Intensity]]
[[RTE 2D Boltzmann Solution]]

The solution is based on FT intensity for dimension d Eq 18
do IFT to obtain explicit formula for $P(r,t)$ 

in 2D eq 18 simplifies to
$$
P_N(k,\omega)=c^{-1}\left[(1-i\omega l/c)^2+k^2l^2\right]^{-(N+1)/2}
\tag{19}
$$
this equation has $(k^2+a^2)^{-v}$ structure --> solvable with bessel function
do IFT with respect to k for $N\ge1$ , we obtain
$$
P_N(r,\omega)=\frac{1}{cl^2}\left(\frac{r}{2l(1-i\omega l/c)}\right)^{-(N+1)/2}\times\frac{1}{\Gamma((N+1)/2)}K_{(N-1)/2}((1-i\omega l/c)r/l)
\tag{20}
$$
this equation also involves bessel function of the second kind $K_v(z)$ 
Bessel function is naturally arise in radial symmetry problem
$\mathcal{F}^{-1}[(k^2+a^2)^{-v}]$  always produce bessel function

use integral identity
$$
K_v(z)=\frac{\sqrt{\pi}(z/2)^v}{\Gamma\left(v+\frac{1}{2}\right)}\int_0^{\infty}d\xi(sinh\xi)^{2v}e^{-zcosh\xi}
\tag{21}
$$

and $cosh\xi=ct/r$ , IFT of Eq 20 is
$$
P_N(r,t)=\frac{e^{-ct/l}}{2\pi l^2}\frac{1}{(N-1)!}\left(1-\frac{r^2}{c^2t^2}\right)^{(N-2)/2}\times\Theta(ct-r),\quad N\ge1
\tag{22}
$$
this equation incorporate 
1. exponential attenuation $e^{-ct/l}$ 
2. Poisson-line scattering distribution $\left(\frac{ct}{l}\right)^{N-2}/(N-1)!$ 
3. Geometric factor $\left(1-\frac{r^2}{c^2t^2}\right)^{N-2}/2$ 
4. Step function (causality) $\Theta(ct-r)$ 

By summing all scattering order N, total intensity is
$$
P(r,t)=\frac{e^{-ct/l}}{2\pi l^2}\delta(ct-r)+\frac{1}{2\pi lct}\left(1=\frac{r^2}{c^2t^2}\right)^{1/2}\times exp[l^{-1}(\sqrt{c^2t^2-r^2}-ct)]\Theta(ct-r)
\tag{23}
$$
this equation contain 2 physical parts
1. Ballistic component (1st term RHS) arrive exactly at $r=ct$ 
2. Scattered component $r<ct$ 
when $t>>r/c$  solution approaches diffusion with $D=cl/2$ 

Next to obtain angular resolved intensity $P_N(\mathbf{r},t,\mathbf{\hat{s}})$, perform integral over $r_0$ in Eq 15
integrand vanishes for $r_0>r_{max}$ . with
$$
r_max=\frac{{ct}^2-r^2}{2(ct-r\mu)}
\tag{24}
$$ for $N\ge1$ 
$$
\begin{aligned}
P_N(\mathbf{r},t,\mu)
&=\frac{1}{2\pi l^N(N-2)!}\int_0^{r_{max}}dr_0e^{-ct/l}[(ct-r_0)^2-(\mathbf{r}-r_0\mathbf{\hat{s}}^2)]^{(N-3)/2}\\
&=\frac{e^{-ct/l}}{2\pi l(N-1!)}\frac{1}{ct-r\mu}\left(\frac{ct}{l}\right)^{N-1}\times\left(1-\frac{r^2}{c^2t^2}\right)^{(N-1)/2}
\Theta(ct-r)
\end{aligned}
\tag{25}
$$
summing over N, include ballistic contribution
$$
P(\mathbf{r},t,\mathbf{\hat{s}})=e^{-ct/l}\delta(\mathbf{r}-ct\mathbf{\hat{s}})\Theta(t)+\frac{1}{2\pi l(ct-\mathbf{r}\cdot\mathbf{\hat{s}})}\times exp[l^{-1}(\sqrt{c^2t^2-r^2}-ct)]\Theta(ct-r)
\tag{26}
$$
