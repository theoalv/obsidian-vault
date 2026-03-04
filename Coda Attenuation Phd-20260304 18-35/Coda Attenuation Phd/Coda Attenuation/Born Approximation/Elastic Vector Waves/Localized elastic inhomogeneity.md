---
title: Localized elastic inhomogeneity
updated: 2026-02-07T08:27:57
created: 2026-02-05T10:41:05
---

Apply same procedure from scalar wave to vector wave
![image1](../../../../resources/0b75d77168054f5182873d5182338d7a.png)
![image2](../../../../resources/3f5fae72182a46dd860ac8ecfc8f5c3a.png)

Elastic wave equation for displacement vector wavefield u(x,t) is
![image3](../../../../resources/fd4dd7883c6e4ecab7115540d26f2553.png)
Overdot --\> time derivative
Stress tensor is defined by
![image4](../../../../resources/875e629138f1473a9446b75e57295e80.png)

We focus on scattering of plane wave by block of dimension L around the origin
P and S wave velocity are given by
![image5](../../../../resources/d1da8e27e1c24480960fb8c0945f01a5.png)
Small perturbations give this relationship
![image6](../../../../resources/194e7f4dad414a8381877a0766c04238.png)

Born approximation
![image7](../../../../resources/7ef5e75c37854180b79169f0b683fc3b.png)
Incident wave equation
![image8](../../../../resources/c3f1ef94865b425488423788be103cb0.png)
Scattered wave equation
![image9](../../../../resources/55eb1930fa004045881260fec7715423.png)
Rhs -\> equivalent body force --\> interaction of incident wave with medium inhomogeneity
![image10](../../../../resources/63995ecc84964b5fac74721f00fc1595.png)

Incident P wave case, propagating in third direction (parallel)
![image11](../../../../resources/c2db70eb0d9e493f868e57b4dcee24a2.png)
Equivalent body force
![image12](../../../../resources/103a41c36c2b4fcfaa41c806518c7acb.png)
density bulk gradients

Incident S wave case, propagating in 3rd direction, polarization in 1st direction
![image13](../../../../resources/9676f29ac8eb42b5a48d7a804de0c58c.png)
Equivalent body force
![image14](../../../../resources/3f4ea430966b46aeb5d720df1802f447.png)

To solve these equations, green function in 3D homogenous medium is needed, which satisfies
![image15](../../../../resources/199e7cbff4044424801ec3f8f072d5d0.png)
--\> apply an impulsive force, k direction at origin

Retarded green function is a sum of 3 terms
![image16](../../../../resources/a6860895744c4a71aa4e02c5c9b7c5fc.png)
far field P and S Near field
![image17](../../../../resources/b1e2ef7314f542fa821007abbd3d934c.png)

In the far field r\>\>L, first 2 terms is enough

**Scattering Amplitudes in cartesian**
PP scattering mode --\> scattered P wave in the far field for incident P wave
Convolution of G with equivalent body force

For far field approximation, r \>\> L
![image18](../../../../resources/f85cb6c74909443cad21cd7e0983da7a.png)
![image19](../../../../resources/a89a4c5578a34144aed2b886b795c156.png)
![image20](../../../../resources/7c72c3ff89c942b4a165f1eb4b90dec8.png)
Where gamma = alpha/beta
S wave velocity couples to PP scattering, means S wave heterogeneity controls P wave coda

![image21](../../../../resources/c0f1c776d23f4029b9a87d4365ca25ad.png)

For other case
![image22](../../../../resources/8bc8cdd10543481e919cc89a5aec1883.png)

![image23](../../../../resources/678a527bf908453e956abe69d64d29c8.png)

![image24](../../../../resources/ec1630a0a7644177b44bd956c7339bb0.png)

**Scattering Amplitudes in spherical**
Spherical coordinates
![image25](../../../../resources/c9e12ad8615a4a3c9fce9f7f779f4eff.png)
Scattering amplitudes
![image26](../../../../resources/d69f4602253a44068c23f8ba8893b69b.png)

![image27](../../../../resources/0b7f4b4c95f34ef09669ec471a82c86f.png)

![image28](../../../../resources/23f362d1d8c7423280157a00298330dc.png)

![image29](../../../../resources/13168cf689be4c8899985a12fa82b1ce.png)

