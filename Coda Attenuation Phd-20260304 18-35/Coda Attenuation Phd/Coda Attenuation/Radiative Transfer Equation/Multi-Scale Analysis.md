---
title: Multi-Scale Analysis
updated: 2026-02-24T12:43:03
created: 2026-02-18T08:34:15
---

Multi-Scale Analysis
18 February 2026
8:34

**Multi scaling**
Mean wave scaled with x, t
![image1](../../../resources/3c35f8f918c24ea59602fff12d4bc6e5.png)
Individual wave vibrates very vast, while seismic energy spreads slowly
Averaging with x,t only --\> kills signal

Fast (micro) scales --\> x,t
![image2](../../../resources/d99cdc76f1de41d783e86807fcfe818c.png)
Time scale wave period
Slow (macro) scales --\> X,T
![image3](../../../resources/a2a65a79687c44269cea65329408f16a.png)
![image4](../../../resources/c7ac4efac06e497ca9b5fece29a06ef9.png)

Based on slow variable, wave equation and its transform can be written as
![image5](../../../resources/77aefec603b0433d8aad55ea1cac6b63.png)

Cell size must satisfy
![image6](../../../resources/faa529fcd3624179924e9c6a05039f68.png)
--\> medium inside cell statistically stationary
ACF and PSDF meaningfull
![image7](../../../resources/c11bc663233a40a890cdca85d3eb64eb.png)

![image8](../../../resources/83f07a8c81ae4e5ea62138595d46c74a.png)
![image9](../../../resources/5f7049743e9747ba9d470e521ecc4136.png)

![image10](../../../resources/cdf8b652461b4699bdd3a3250fcfe59a.png)

![image11](../../../resources/660af7c872ab460b9eb65d84a2b7d249.png)
--\> equal to mean energy density
![image12](../../../resources/61b7e856502948078ea9ac52f5bba8a8.png)
![image13](../../../resources/b307d0d4f295437dacaf5afb4adb1237.png)

![image14](../../../resources/23313a496892444d9bf8ca2eb8e4693b.png)

![image15](../../../resources/2d46f83da24246f1936343f8c5cda61b.png)

Taylor expand L0
LHS --\> deterministic transport
RHS --\> random scattering

This is equation U for macro variables only (slow)
![image16](../../../resources/1fd289be53f44f8aa5d594079695ba10.png)

![image17](../../../resources/1df7ae5c1f4445099d528de769730d57.png)
![image18](../../../resources/ebae33d95f05478da0f1159f95769e55.png)

![image19](../../../resources/2a25e7cb635b4adea8736026210996b0.png)
![image20](../../../resources/c2e42b1b57544ee384e177619c603660.png)
![image21](../../../resources/c7a87ac9d9304dd2b61706aef57f088d.png)
Evaluate fluctuation wave in the cell as
![image22](../../../resources/b2a98950c02b4c3eb055d3ece69361f6.png)

![image23](../../../resources/16bbc058af5d499f98249192218d851e.png)
![image24](../../../resources/a20acba834f6449fb7b7236b848e9b53.png)

![image25](../../../resources/5ba492a358e34052a01197e9f0f84432.png)
![image26](../../../resources/b1215a02bfd14c21a0e5619e2113b8e2.png)
RHS --\> scattering terms
Expand U (7.51)

![image27](../../../resources/757c40b1e88e4b7a95190b9e98dae849.png)

Substitute U' (7.58)
![image28](../../../resources/63ff809e3be349bc81ad93658b303523.png)
![image29](../../../resources/44b8dfcfcd184daba85571f205517d87.png)

![image30](../../../resources/9308d34a53f74067bf7091a2ed602ad3.png)
Taking ensemble average for 7.63 and use 7.50
![image31](../../../resources/775d56dae83a4090acb60ff5254be961.png)
Performing integral over k'
![image32](../../../resources/f534bbc7812a4505971c87caf4216323.png)
Use integral kernel

![image33](../../../resources/a489f03f04f9467b9ef05664ec9e3ec2.png)
Leads to greens function rule

![image34](../../../resources/51845a920417438bb370f0f19de88a0a.png)
![image35](../../../resources/2698d57e195b43b8ad7aaec927a4cdb4.png)

![image36](../../../resources/93d449b7a5f84f51a26bcd505aa0cc31.png)

![image37](../../../resources/42d79cfa04954d578e4ff55621ac8c7f.png)

Final equation in closed form
![image38](../../../resources/c39c84c56ed04fa8b461bff4c72afec2.png)

**Directional distribution of Mean Energy Density**
Taking space time average of the energy density of waves in cell --\> avg over ensemble of random media
E(**X**,T) can be formulated as

![image39](../../../resources/3c27da6d254e469fb19cdd87b30d3de0.png)

Where
![image40](../../../resources/231f81200346426fa3fc1551fcac8029.png)

MED can be written as
![image41](../../../resources/2b4d0e50379849229635d2afeb8897a0.png)

![image42](../../../resources/e9f366ba545545af877e71b1a32df986.png)
![image43](../../../resources/461e1742865b4fe6b83bd8b5b2709440.png)

Total MED is
![image44](../../../resources/d857ec7b475d49df9fac3d75024740f0.png)
Product
![image45](../../../resources/3c62019c472e48b0ae93ae16a07447c9.png)
Is energy flux density in direction q
Substitute 7.72 to 7.70 we obtain
![image46](../../../resources/3d204a345a704677988165f83f6d0205.png)
This is RTE Boltzmann equation

Rewriting Boltzmann Equation by incorporating scattering coefficients
If RTE is using fast variables x,t
![image47](../../../resources/47a1520076b74bd6b9ada47de8dbecdb.png)
![image48](../../../resources/d3ee649283084a149fad833c286ff372.png)

Scattering coefficient can be defined as
![image49](../../../resources/e67964f829214fd3b3abbff3e1031974.png)
Total scattering coefficient
![image50](../../../resources/88489592d5c34dc08ab6247eabe1b0ae.png)
Perform integral over solid angle
![image51](../../../resources/2bec751546b148bc8c562c9afd02a2e7.png)

Final equation
![image52](../../../resources/31391937431c401d842f4c5455d400dd.png)

