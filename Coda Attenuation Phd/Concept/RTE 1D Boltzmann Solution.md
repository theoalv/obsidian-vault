related to
[[IFT Intensity 2D]]

RTE is Based on diffusion equation, 1D solution has been given by Hemmer
$$
P(r,t)=\frac{1}{2}e^{-ct/2l}\left[\delta(r-ct)+\frac{1}{2l}\Theta(ct-r)\times \left(I_0(\sqrt{c^2t^2-r^2})+ct\frac{I_1(\sqrt{c^2t^2-r^2}/2l)}{\sqrt{c^2t^2-r^2}}\right)\right]
$$
this equation calculate intensity $P(r,t)$ at point $r$ and time $t$ 
$ct$ is wavefront position, which $P$ should be zero in front of the wave $(r>ct)$, diffusion is at late lapse time
$\delta(r-ct)$ is the pulse delta function, $\Theta(x)$ step function is zero for $x<0$ to ensure $P$ is zero in front of wavefront
$I_0$ and $I_1$ are Bessel functions

This is simulation of 1D RTE with $c=1$ and $l=1$ ![[Pasted image 20260305135739.png]]
dotted line is wavefront location $ct$ , the simulation shows a decay in position and time with no intensity in front of wavefront

References
[[paasschens1997]]
