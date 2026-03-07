Ref [[paasschens1997]]
Related to
[[RTE 1D Boltzmann Solution]]
[[Fourier Transformed Intensity]]

Based on Fourier Transformed intensity formulation eq 18, 
4D FT intensity is given by
$$
P_N(k,\omega)=2^{N+1}c^{-1}l)(\sqrt{(1-i\omega l/c)^2+k^2l^2})+1-i\omega l/c)^{-(N+1)}
\tag{27}
$$
use identity
$$
\int\frac{d\mathbf{k}}{(2\pi)^4}e^{i\mathbf{k}\cdot\mathbf{r}}f(\mathbf{|k|})=\frac{1}{4\pi^2r}\int_0^{\infty}dk\,k^2J_1(kr)f(k)
\tag{28}
$$
 when function depends only on $|k|$. the FT reduces to 1D integral involving Bessel function $J_1$
 then it becomes
 $$
P_N(r,t)=\frac{2^{N-1}e^{-ct/l}}{\pi^3il^Nr^{N+3}}\int_0^{\infty}dkJ_1(kr)k^{-2N}\times\int_{r/l-i\infty}^{r/l+i\infty}dz\,e^{zet/r}[\sqrt{k^2r^2+z^2}-z]^{N+1}
\tag{29}
$$
Inverse Fourier in k and Inverse Laplace in $\omega$ 
integral over $z$ yields
$$
i(N+1)(kr)^{N+1}J_{N+1}(kct)\Theta(t)r/ct
$$
 do integration over $k$ for $N\ge1$ 
 $$
P_N(r,t)=\frac{1}{\pi^2}e^{-ct/l}\frac{1}{ctl^3}\left(\frac{ct}{l}\right)^{N-3}\times\frac{N+1}{(N-1)!}\left[1-\frac{r^2}{c^2t^2}\right]^{N-1}\Theta(ct-r)
\tag{30}
$$

 