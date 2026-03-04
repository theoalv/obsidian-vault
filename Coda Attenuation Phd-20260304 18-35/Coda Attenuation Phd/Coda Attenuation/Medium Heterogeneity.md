---
title: Medium Heterogeneity
updated: 2026-01-28T08:11:59
created: 2025-12-09T08:57:31
---

Heterogeneity --\> velocity/density vary irregularly
Rocks can have different descriptions but still have the same heterogeneity statistics --\> same seismic behavior
Earth heterogeneity is highly irregular, not repeatable
Instead of describing exact structure --\> describe statistics
describe how strong are the fluctuations statistically? --\> **ACF and PSDF**
ACF --\> how similar is the medium at 2 points separated by distance r?
PSDF --\> FFT of ACF --\> how much heterogeneity in wavenumber domain?
Earth is one realization of a random medium --\> from ensemble of random media with same ACF and PSDF
Any random media with same ACF/PSDF are statistically equivalent for wave propagation
If we generate many random velocity models with same ACF/PSDF --\> each simulation give similar waveform
Then it is practical to compare statistics (mean amp, intensity, etc) rather than 1 waveform, because observed seismic quantities are themselves statistical (coda waves. Scattering)
Real seismic observation sample one earth but average over many scatterers, wavelength, path --\> ensemble like

The Vp in heterogeneous medium is not constant, but a sum of mean velocity (Vo) and perturbed velocity (dV) as a function of location
![image1](../../resources/3e748c013dbf4b3a8c299a92d0e0f8fa.png)
Which can be measured by fractional fluctuations of V --\> ξ(x)
![image2](../../resources/0c4e85f19f724643a41b47f4fc975813.png)

**For stationary process**
**Autocorrelation Function (ACF) R(x)**
Gives statistical measure of the spatial scale and the magnitude of **medium inhomogeneity**
--\> how similar the medium is at 2 separated points by distance x
![image3](../../resources/5d46f37f45ba4440bbc8e709543f6ff8.png)
![image4](../../resources/e9c660ee71b94f6b85eca3139cc84c9b.png)
![image5](../../resources/f3d99e2e985b48e89fe54ab4c50ea054.png)
![image6](../../resources/da804d0874014d23a0c1f7c7cff5f6a9.png)

**Power Spectral Density Function (PSDF) P(m)**
Describes how much of variance (power) for each wavenumber
Fourier transform of ACM --\> PSDF
By integrating angle in spherical coordinates, the IFT formulation become
![image7](../../resources/f70886f9b78a453d92bcc00a4cd6b18e.png)
![image8](../../resources/ca989a35e55f400ca32ffc6afba54d9e.png)
![image9](../../resources/4d5ad24f0e7c4946b7c327e1ea77dcd8.png)
![image10](../../resources/254da7ee1bf84872a4678a0fc23e643a.png)
Low wavenumber behaviour of PSDF must ensure this integral is finite
![image11](../../resources/e8b05731d5a44ec191bba927d417b4cb.png)
![image12](../../resources/d916ea00a78344818e04e0cc182708f5.png)
![image13](../../resources/0330b06122104f69aa93332f8cbcfc83.png)

**Stationary increment case**
When random function is not strictly stationary (homogenous) over all space, but **locally stationary**
![image14](../../resources/2312037301b146f2b5254d1f9b044d0d.png)
Stationary increment --\> field ξ(x) is not stationary, but increments are stationary
![image15](../../resources/90a70e9c7a1845fba633caab1386aacb.png)
Use structure function instead of ACF
![image16](../../resources/c656517d75c047e2a0e66b1448d85e70.png)
![image17](../../resources/d9c6d72e47bc43daaee7475fa8ea295a.png)
![image18](../../resources/eeedf59c96114977835c584c653cb223.png)
For stationary increment, the field do not need to have finite variance, only increments do
--\> allow more low-wavenumber power (more low freq energy)

**Realization of random media**
For a given PSDF P(m), it is necessary to make realizations of random media ξ(x)
- ![image19](../../resources/35534c5d81484a06b0e2898c8838382b.png)
- Phase spectrum φ(m) is random between 0 and 2π
Random medium is synthesized by IFFT
![image20](../../resources/971c2fdc3bcf4bbeae63dab598c22f47.png)
Where
![image21](../../resources/2cc57650b779475997501850a4e122d9.png)
Changing random seed changes the φ(m) --\> totally new random medium field, but P(m) stays the same
- Every realization has the same PSDF
- Spatial pattern changes
- Averaging many realizations --\> theoretical covariance (ACF)
In random medium, the statistics matter and exact shapes of heterogeneity are irrelevant

**Types of ACF and PSDF random media**
**Gaussian model**
ACF formulation
![image22](../../resources/238e66c754634273b1e95e03d9223a3c.png)
For 2D PSDF
![image23](../../resources/64e265a9d8724b5a99f7b24600666cda.png)
3D PSDF
![image24](../../resources/ba3c9ef6eb304bc18655c6e947b4d9ee.png)

**Von Karman Model**
For 2D model
![image25](../../resources/081a55b997ed4673a0187bc59eaa7de0.png)
The smoothness is depend on K parameter
K\[0,1\] --\> 1 is the smoothest
---
![image26](../../resources/59c71e75562f42c9a013a7fe7648743e.png)
![image27](../../resources/481af98f0abe44909391db4ecd40c2d5.png)
--\> same with expected value in probability theory
![image28](../../resources/09ac001562a8458b9ad7d45703054cc1.png)
![image29](../../resources/3413da52f5224c4c8388cb7daccf4f01.png)
Example
For N random media with different random seeds (i.e random phase)
![image30](../../resources/c09bf9d923be43e1961a1d418857c950.png)
If all samples averaged --\> ensemble average
Each realization is a different map of heterogeneity
--\> stacking all maps and averaged all pixel --\> ensemble average

Ensemble average vs spatial average
Ensemble --\> average over many realizations
Spatial --\> average over space in a single realization
For stationary random field --\> ensemble ≈ spatial
--\> that’s why one random medium can be used for numerical simulations

---
**Correlation length (a)**
![image31](../../resources/1c569e90a0fa4d0b9f7418716cb43a82.png)
- If 2 points are separated by a distance \<a --\> have similar values
- Separated by more than a --\> uncorrelated

---
**Inhomogeneity from log data**
Test from DH-11 downhole Vs log data

**ACF** --\> autocorrelate data

Have similar pattern with von-karman model

**PSDF** --\> FFT

