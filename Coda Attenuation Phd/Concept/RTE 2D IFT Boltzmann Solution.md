Ref [[paasschens1997]]
Related to
[[RTE 1D Boltzmann Solution]]
[[Fourier Transformed Intensity]]

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
