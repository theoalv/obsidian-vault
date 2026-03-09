Ref [[sens-schonfelder2006]]
Related to
[[paasschens1997]]
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
The solution is from Paasschens (1997)
$$
G(t,r)\simeq\frac{e^{-v_0tg_0}}{4\pi r^2}\delta(r-v_0t)+\frac{(1-r^2/v_0^2t^2)^{1/8}}{(4\pi v_0t/3g_0)^{3/2}}e^{-v_0tg_0}\times K\left(v_0tg_0\left[1-\frac{r^2}{v_0^2t^2}\right]^{3/4}\right)H(v_0t-r)
\tag{3}
$$
where $K(x)\simeq e^x\sqrt{1+2.026/x}$ 

Assuming total reflection, at half space a mirror source with $G(t,r^+)$ is assumed.
At the surface, upward flux of the real source equals the downward flux, satisfying the boundary condition.
The GF of the half space is $G_h(t,\mathbf{x})=G(t,r)+G(t,r^+)$ 
receiver is assumed at $r^+$, then $G_h(t,\mathbf{x})=2G(t,r)$

Source funtion is assumed in the form $W\delta(\mathbf{r})\delta(t)$ 
The final model equation is
$$
\begin{align}
E_{mod}(t,\mathbf{x})
&=WR_iG_h(t,\mathbf{x})e^{-bt}\
\tag{4}\\
&=2WR_iG(t,r)e^{-bt}\
\tag{5}
\end{align}
$$

Observed energy density is formulated from bandpassed velocity seismogram $\dot{u}(t,r)$ 
$$
E_{obs}(t,r)=\frac{\rho_0}{2}\frac{\dot{u}(t,r)+\mathcal{H}^2(\dot{u}(t,r))}{2}
\tag{6}
$$
$\rho_0$ can be assumed (2700)

Inversion scheme --> estimate 