For a case where wavelength of the seismic wave is shorter than the correlation length of the medium, the wave will only experiences narrow angle forward scattering. In this case, conversion between P-S and backscattering can be ignored.

Thus we can use scalar formulation. Scalar wavefield equation as a superpotition of plane waves:
$$
u(x_{\perp},z,t)=\frac{1}{2\pi}\int_{-\infty}^{\infty}d\omega U(x_{\perp},z,t)e^{i(k_0z-\omega t)}
$$
where transverse coordinates $x_{\perp} = (x,y)$ on transverse plane, orthogonal to z direction
Envelope U contains amplitude and phase change, where exp is the wave dynamics (wiggle)

After substituting to scalar wave equation, it becomes
$$
\partial_z^{2}+2ik_0\partial_zU+\Delta_{\perp}U-2k_0^2\xi U=0 
$$

Because it is assumed that $ak_0 \gg 1$ , medium heterogeneity size is larger than wavelength. Envelope U changes slowly and the second derivative $\partial_z^2 = 0$

Then the final parabolic equation for $U$:
$$
2ik_0\partial_zU+\Delta_{\perp}U-2k_0^2\xi U=0 
$$
This equation can be solved with Rytov perturbation method:
$$
U(x_{\perp},z,t)=e^{\psi(x_{\perp},z,t))}=e^{\Delta lnA_0+i\Delta \varphi}
$$
Using green function
$$
\hat{G_{0}}(m_{\perp}, z, \omega) = \frac{i}{2k_0} e^{-\frac{i\,m_{\perp}^{2}z}{2k_0}} H(z)
$$

Then the equation become 
$$ \hat{\Psi}{(m_{\perp}, Z, \omega)} = 2k_0^2 \int_0^Z \hat{G_0}(m_{\perp}, Z-z, \omega)\, \hat{\xi}(m_{\perp}, z)\, dz $$
Markov Approximation --> extrapolate forward, without "past memory"
