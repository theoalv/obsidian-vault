Ref [[paasschens1997]]
Related to
[[RTE 1D Boltzmann Solution]]
[[Fourier Transformed Intensity]]
[[RTE 2D Boltzmann Solution]]
[[RTE 4D Boltzmann Solution]]

Based on FT intensity Eq 18, the equation for 3D is
$$
P_N(k,\omega)=c^{-1}l\left[\frac{1}{kl}arctan\left(\frac{kl}{1-i\omega l/c}\right)\right]^{N+1}
\tag{33}
$$
evaluating 3D angular integral gives arctan kernel --> only possible for N=0,1
then use interpolation from 2D and 4D solution
2D --> $(1-r^2/c^2t^2)^{(N-2)/2}$ 
4D --> $(1-r^2/c^2t^2)^{N-1}$
then approximation for 3D
$P_N\propto[1-r^2/(ct)^2]^{3N/4-1}$ 

The intensity must satisfy Poisson statistics of scattering events Eq 14
with normalization
$$
\int d\mathbf{r}P_N(\mathbf{r},t)=\frac{1}{N!}\left(\frac{ct}{l}\right)^Ne^{-ct/l}
\tag{34}
$$
means number of scattering evens follows a Poisson distribution
mean number of event $\langle N \rangle=ct/l$    

Combining interpolation exponent and normalization constraint, for $N\ge1$ 
$$
P_N(r,t)\simeq\frac{e^{-ct/l}}{\pi l^3}\frac{\Gamma\left}{}
$$