---
title: Attenuation of High Frequency Seismic Waves
updated: 2026-02-12T11:28:57
created: 2026-02-11T07:42:18
---

Attenuation of High Frequency Seismic Waves
11 February 2026
7:42

Spatial attenuation for P and S wave quantified with Qp and Qs
--\> amplitude decrease exponentially with travel distance
![image1](d8e9b4a7a0dd4fe9b23caa857beff809.png)
In addition with geometrical spreading r-1
Attenuation measurement --\> spectral decay method
![image2](28630900b48e4e2bba09494a5fb8e158.png)
--\> measurements of spectral amplitudes vs. frequency for at least two propagation distances
Recent advancements --\> coda normalization, MLTWA

Current study Qs is more common than Qp
For low freq (\>0.05 hz) Qp-1/Qs-1 --\> ~0.4
For high freq (1-20hz) --\> 1 - 2

Intrinsic mechanism
Mechanism that converts vibration energy into heat --\> friction, viscosity, thermal relaxation
1.  Friction
Generally frequency independent, measured with crack aspect ratio d
2.  Viscous dissipation
Walsh model --\> liquid movement through cracks
Biot model --\> coupling of motion between fluid and solud matrix, extremely small attenuatrion for \<100hz
3.  Molecular relaxation
Thin films of water adsorbed to crack interact with rock by thermally activated motion --\> softening rock and adsorb energy
4.  Thermoelasticity
adiabatic compression heats rock when expand, then reduced by thermal diffusion --\> mainly Qp
Empty cracks induced stress concentration --\> thermoelasticity
Thermoelasticity can explain why Qp-1\>Qs-1, matches seismological observations

Scattering attenuation
Total attenuation has similar values with total scattering g0 --\> idea that scattering is the dominant mechanism
Traditional born theory predicts Qs increases with frequency, which contradict observed data
![image3](aad2fc7cabe94b0695ee8366d9b26d7a.png)

Two attempts to resolve this problem
1.  Isolating effect of travel time fluctuations
2.  Neglects scattering in the forward direction
Both approaches are equivalent

**Conventional born approximation scattering**
Based on g0/k0
![image4](cd6bb5c4225d4bcfb542511c0b0b649e.png)
Using exponential ACF, this formulation become
![image5](a8130119e5984c878906d20545c8a0b9.png)

![image6](626022c7acf84da8ae681292b3cdafd2.png)
This prediction increases linearly with frequency for high frequency, due to strong forward scattering

The Born approximation is valid only when the energy loss per distance L is small
![image7](a08a930bfd2b4d7ebc547609c158e906.png)

![image8](0f3f12448bab4e3ba1329239c28a6923.png)
first arrival travel-times are expected to vary considerably from trace to trace.
A blind application of the Born approximation thus predicts a large attenuation because of the relative travel-time shift due to the long wavelength structure.
Tu1 --\> small
Predicted scattering attenuation is small
--\> subtract the travel-time shift caused by the long wavelength components of velocity fluctuation and then calculate scattering amplitude based on the Born approximation

Scatterer divided into 2 --\> long wavelength scatterer and short wavelength scatterer
EL --\> shifts arrival time, forward scattering (needs to be removed)
ES --\> bounces energy to coda
Removed with cut off scattering angle, usually 29 degrees
--\> it will ignore all scatterers with angle less than that, or on counting wide scatter angle

In elastic wave
When equipartition state reached, coda wave will be dominated with S coda
PS \> SP
