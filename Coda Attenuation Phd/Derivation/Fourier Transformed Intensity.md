RTE describes intensity radiation $P(r,t,\hat{s})$, dependent on place r, time t, and direction $\hat{s}$
![[Pasted image 20260306215726.png|443]]
based on boltzmann equation
$$
\frac{\partial}{c \partial t}P(\mathbf{r},t,\mathbf{\hat{s}})+\mathbf{\hat{s}}\cdot\nabla P(\mathbf{r},t,\mathbf{\hat{s}})=-\left(l^{-1}+l^{-1}_a\right)P(\mathbf{r},t,\mathbf{\hat{s}})+l^{-1}P(\mathbf{r},t)+c^{-1}S(\mathbf{r},t,\mathbf{\hat{s}})
\tag{3a}
$$
$$
P(\mathbf{r},t)=\int\frac{d\mathbf{\hat{s}}'}{\Omega_d}P(\mathbf{r},t,\mathbf{\hat{s}}')
\tag{3b}
$$
$S$ -> source term
$l$ -> mean free path
$l_a$ -> adsorption length

LHS 1st term --> rate of change of P in time evolution
LHS 2nd term --> balistic motion in $\mathbf{\hat{s}}$ 
RHS 1st term --> scattering and adsorption
RHS 2nd term --> scattering from other direction to $\mathbf{\hat{s}}$ 
RHS 3rd term --> source

simplified by assuming no adsorption $l_a \longrightarrow \infty$
isotropic point source defined as
$$
S(\mathbf{r},t,\mathbf{\hat{s}})=\delta(\mathbf{r})\delta(t)
\tag{4}
$$
need to seek eq 3 with P = 0 when t<0
due to spherical symmetry $P(\mathbf{r},t,\mathbf{\hat{s}})$ and $P(\mathbf{r},t)$ only depend on $r=|\mathbf{r}|$, $t$, and $\mu\equiv\mathbf{\hat{s}}\cdot\mathbf{r}/r$
equation 3 simplifies to
$$
l\left(\frac{\partial}{c\partial t}+\mu\frac{\partial}{\partial r}+\frac{1-\mu^2}{r}\frac{\partial}{\partial \mu}\right)P(r,t,\mu)=-P(r,t,\mu)+P(r,t)
\tag{5}
$$

time evolution + radial motion + angular change
$$
P(r,t)=\int_{-1}^1d\mu\rho_d(\mu)P(r,t,\mu)
\tag{6}
$$
weight function $\rho_d(\mu)$ defined by
$$
\rho_d(\mu)=\frac{\Gamma(d/2)}{\sqrt{\pi}\Gamma((d-1)/2)}\left(1-\mu^2\right)^{(d-3)/2},\quad d>1
\tag{7}
$$
in 3D --> constant
in 2D --> $1/\sqrt{1-\mu^2}$ 
1D is special case as there are only 2 direction $\mu=\pm1$ , 
particle can only move left or right
$\rho_1(\mu)=\frac{1}{2}\delta(\mu-1)+\frac{1}{2}\delta(\mu+1)$ 

To solve boltzmann equation, separate intensity contribution of scattering events N
$$
P=\sum_{N=0}^{\infty}P_N
\tag{8}
$$
$P_o$ --> balistic
$P_1$ --> single scattering
$P_2$ --> double scattering

Partial intensities $P_N$ satisfy
$$
\left(\frac{\partial}{c\partial t}+\mathbf{\hat{s}}\cdot\nabla+l^{-1}\right)P_N(\mathbf{r},t,\mathbf{\hat{s}})=l^{-1}P_N(\mathbf{r},t),\quad N>0
\tag{9a}
$$
$$
\left(\frac{\partial}{c\partial t}+\mathbf{\hat{s}}\cdot\nabla+l^{-1}\right)P_0(\mathbf{r},t,\mathbf{\hat{s}})=c^{-1}S(\mathbf{r},t)
\tag{9b}
$$
Ballistic particle $P_0$ **never scatter**, but still contain loss term $l^{-1}$ 
particle that scatter --> leave $P_0$ population
with probability $p(r)=\frac{1}{l}e^{-r/l}$ 

integrating transport operator (LHS)
$$
P_N(\mathbf{r},t,\mathbf{\hat{s}})=l^{-1}\int_0^{\infty}dr_0e^{-r_0/l}P_{N-1}\left(\mathbf{r}-r_0\mathbf{\hat{s}},t-r_0/c\right)
\tag{10a}
$$
$$
P_0(\mathbf{r},t,\mathbf{\hat{s}})=c^{-1}\int_0^{\infty}dr_0e^{-r_0/l}S\left(\mathbf{r}-r_0\mathbf{\hat{s}},t-r_0/c\right)
\tag{10b}
$$
particle has travel distance $r_0$, no scattering during travel $e^{-r_0/l}$ . then scatter

and angular average of intensity
$$
P_N(\mathbf{r},t)=\int d\mathbf{r_0}p_0(\mathbf{r_0})P_{N-1}\left(\mathbf{r}-\mathbf{r_0},t-r_0/c\right)
\tag{10a}
$$

$$
P_0(\mathbf{r},t)=lc^{-1}\int d\mathbf{r_0}p_0(\mathbf{r_0})S\left(\mathbf{r}-\mathbf{r_0},t-r_0/c\right)
\tag{10b}
$$
where
$$
p_0(\mathbf{r})=\frac{e^{-r/l}}{\Omega_dlr^{d-1}}
\tag{12}
$$
means probability density that next scattering occurs at distance **r**
ballistic signal decrease with distance because of longer path --> higher probability scattering

**Ballistic solution**
using source in eq 4, explicit expression for ballistic N=0 is
$$
\begin{aligned}
P_0(\mathbf{r},t,\mathbf{\hat{s}})&=e^{-ct/l}\delta(\mathbf{r}-ct\mathbf{\hat{s}})\Theta(t)\\
&=e^{-ct/l}\frac{\delta(r-ct)\delta(\mu-1^-)}{\Omega_dr^{d-1}\rho_d(\mu)}
\end{aligned}
\tag{13a}
$$
$1^-$ in $\delta$ function means it is a single-sided $\delta$ function
$$
P_0(\mathbf{r},t)=\frac{e^{-ct/l}}{\Omega_dr^{d-1}}\delta(r-ct)
\tag{13b}
$$
this formulate ballistic spike
particle travel $r=ct$ with attenuation $e^{-ct/l}$ 

**Multiple scattering solution**
based on recursion relation eq 11
$$
P_N(\mathbf{r},t)=l\left[\prod_{i=0}^N\int d\mathbf{r}_ip_0(\mathbf{r}_i)\right]\delta\left(ct-\sum_{i-0}^Nr_i\right)\delta\left(\mathbf{r}-\sum_{i-0}^Nr_i\right)
\tag{14a}
$$
$$
P_N(\mathbf{r},t,\mathbf{\hat{s}})=\Omega_dl\left[\prod_{i=0}^N\int d\mathbf{r}_ip_0(\mathbf{r}_i)\right]\delta\left(ct-\sum_{i-0}^Nr_i\right)\times\delta\left(\mathbf{r}-\sum_{i-0}^Nr_i\right)\delta\left(\mathbf{\hat{r}}_0-\mathbf{\hat{s}}\right)
\tag{14b}
$$
where $\mathbf{\hat{r}}_0=\mathbf{r}_0/|\mathbf{r}_0|$ 
each scattering path have $r_0,r_1,...,r_N$ 

this solution uses integration product over all possible step length $\prod_{i=0}^N\int dr_i$ 
however, most combination of $r_i$ correspond to **incorrect travel time and distance**
thus, it is followed by 2 constrains: time constrains and spatial displacement
$\sum_{i-0}^Nr_i=r=t$ 