---
title: RTE in Integral Form
updated: 2026-03-04T14:34:48
created: 2026-02-24T12:43:47
---

**Scalar wave case**
RTE
![image1](92aea7e47c6c451aaf7123b6880eeee5.png)

LHS --\> transport along ray
First RHS --\> scattering loss (-g0)
Second RHS --\> scattering gain, scattered into q and from all direction q'
Third RHS --\> source term

**Integral Equation**
Split equation 7.80
![image2](8d02a83efea74548a5de9cb9a2ed59a9.png)
LHS --\> linear advection-attenuation operator
RHS --\> scattering from other direction, physical source

Define green function for 7.81
![image3](da7233183dc546c3b73dcfdd8c81562e.png)
Do FourierT in space and LaplaceT in time
![image4](97365609383f4455b25bda6227af4de5.png)
GR become
![image5](39d0375a5e964468bddc3d0ac28e0672.png)

![image6](18e5bef4fb1c498ba8e8d4037fc124d0.png)

![image7](9323cfdf445e454a9939aecf6a38da5b.png)

![image8](942dbf0224cd453ba389019a36ef0f46.png)

![image9](3fb3d3a52c134a0090ac7482ffc2a5c3.png)

Final integral RTE form

![image10](8a770c7a071d444682132caccf83c3af.png)

First term --\> direct energy from source, attenuated by scattering
Second term --\> energy that has been scattered at earlier points and then propagated to x,t

![image11](e345b9a3e7e24e358b6e912b6d46d985.png)

**Elastic wave case**
Now use Vp and Vs instead of uniform Vo
Define scattering modes between P and S
![image12](93d210a0800845218aca9aaf756041cf.png)

![image13](9b94f0c3a6f4476dbadde273e371ca75.png)
Simplified by axial symmetry assumption --\> scattering only depends on incident and scattered direction

Redefine directional distribution of energy density to P and S wave (fp and fs)
Total energy density defined as
![image14](5aee091bb8354d62a3ede4c2bc6ddc78.png)
RTE equation for both P and S wave case, extension of 7.80
![image15](5c81457ee10548d4b6fbc16d99696760.png)
P wave case
Transport = loss + PP scattering + SP conversion + source
In S wave case, SH and SV ignored --\> S only

**Isotropic radiation and isotropic scattering**
Radiation --\> from point source
Scattering --\> g for all modes
![image16](70d7c4f630b941ed889c723b4ecafbab.png)

![image17](b6464ecc7abb4ab2aaf37d81242ab365.png)

