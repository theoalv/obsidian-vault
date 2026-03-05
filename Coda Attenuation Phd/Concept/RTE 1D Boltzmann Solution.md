RTE is Based on diffusion equation, 1D solution has been given by Hemmer
$$
P(r,t)=\frac{1}{2}e^{-ct/2l}\left[\delta(r-ct)+\frac{1}{2l}\Theta(ct-r)\times \left(I_0(\sqrt{c^2t^2-r^2})+ct\frac{I_1(\sqrt{c^2t^2-r^2}/2l)}{\sqrt{c^2t^2-r^2}}\right)\right]
$$
this equation calculate intensity $P(r,t)$ at point $r$ and time $t$ 
$ct$ is wavefront position, which $P$ should be zero in front of the wave $(r>ct)$, diffusion is at late lapse time
$\delta(r-ct)$ is the pulse delta function, $\Theta(x)$ function is zero for $x<0$ to ensure $P$ is zero in front of wavefront

