Ref [[sens-schonfelder2006]]
Related to
[[RTE 3D Boltzmann Solution]]
[[Boltzmann Equation]]

Coda envelope modelled using RTE, governed by Boltzmann equation.
Restrict to isotropic scattering of S waves in half-space with isotropic source.
Effective energy density Green Function is
$$
G(t,\mathbf{r})=F(t,\mathbf{r})+v_0g_0\int_{-\infty}^{\infty} \int_V F(t-t',\mathbf{r}-\mathbf{r}')G(t',\mathbf{r}')dt'd\mathbf{r}'
\tag{1}
$$
where
$$
F(t,\mathbf{r})=\frac{1}{4\pi v_0r^2}H(t)\delta(t-r/v_0)e{-v_0g_0t}
\tag{2}
$$
The solution is 