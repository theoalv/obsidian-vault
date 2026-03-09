---
title: Scattering by Random Velocity Inhomogeneities
updated: 2026-02-05T11:02:44
created: 2026-02-04T10:31:20
---
[[Localized Velocity Inhomogeneity]]
**Scattering Coefficient**
localized inhomogeneity defined only 1 scatterer --\> in medium contains many small heterogeneity and isotropic
Velocity fluctuates randomly (ensemble random functions) with zero mean
--\> characterized by ACF or PSDF (statistics)
Divide inhomogeneous medium into block L, with L \>\> a

![image1](9e96a755cba0443b9d85d83f5aea4623.png)

Born Approximation condition
![image2](55ca68864b714d4fa93a220a8b07d0a3.png)
As minimum dimensions of the scattering volume are of the order of a

Ensemble averaged scattering cross section
![image3](954774259e8444999d5424be46739a1c.png)
![image4](fdbca91206a34ddcafa4d833029e166c.png)
![image5](eb35771cc8ff4a6abd20ce7300c83cef.png)
We get
![image6](b0e509f283a545bd8a6b0d165453a29a.png)

Scattering coefficient (g) is then defined as
![image7](6e0462da94c44eb28e3ca3829f48b3b6.png)
![image8](ef00ead66e0c43ff80f70b378a602a7b.png)
Scattering coeff is directly related to PSDF of velocity fluctuation
When random media is statistically homogenous and isotropic --\> g is axially symmetric
Scattering pattern is not necessarily isotropic even if random media is

Ratio of scattered wavefield to incident wavefield defined as
![image9](ba19148c45cf4fcb84827dd5709727e0.png)

Total scattering coefficient defined as
![image10](bfdb7e1d31ac47aa832c2dff564d05e0.png)
Total --\> angular average

Transport (momentum transfer) scattering defined by
![image11](4dc1688f310047b1b9d2b859cf48cd39.png)
Which is the effective isotropic scattering in the multiple scattering regime --\> diffusion solution

Exponential ACF
We can substitute exponential ACF PSDF to the equation (P) to obtain
![image12](b6be3670097749bba5167fdb4714d59a.png)
![image13](756a00a174ab4793968b9b11dbd5e879.png)
![image14](a02e7a865d284a32815ab3ca214071b3.png)
Born approximation may fail near forward direction

![image15](d07afadcc9c24c6a9125a0a442024170.png)

Backscattering coefficient is defined as
![image16](6d28cb2ad473450a88550537352bfef0.png)
For small wavenumber --\> increases with the wavenumber
At large wavenumber --\> become uncorrelated with it

Total scattering is obtained by taking solid angle average
![image17](3508fec2f6504aadb6de795882d10823.png)
Both increased with wavenumber, although large wavenumber has lower scaling

Transport scattering is defined as
![image18](0b7f474c644846dcafb1121c0141fae0.png)
![image19](607e5bb2cd974516ad3873e53d9dd787.png)

![image20](da4c21b558f74ba0bcaf41c1873f2c65.png)

**Backscattering coefficient estimated from numerical simulation**
Jannaud et al 1991
Born theory assumes single scattering --\> coda waves is multiple scattering
Needs simulation to prove the validity of Born approximation

Based on
![image21](ebdc5ee981684b8abf5c037175bf317d.png)

Use gaussian ACF
![image22](db20be0ef93f4271bc99bccdd68b1d87.png)
![image23](67900537223242dcb5900efb58312109.png)

Simulation steps  
compute coda and direct wave power spectrum
Invert to estimate backscattering coefficient
![image24](a001c9a3062e4f53bc01e2e7860731b4.png)

![image25](881b63dbfa984a81b5bbe3954add3d9a.png)

