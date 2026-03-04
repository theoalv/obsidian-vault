---
title: First order smoothing method
updated: 2026-02-12T14:45:42
created: 2026-02-09T12:14:02
---

The First-Order Smoothing Method assumes that these fluctuations only interact with the medium over very short distances (about the size of the correlation distance a) to modify the stable mean wave

**Mean wave**
![image1](ca7f952726d94d57b9d39a990d52eb38.png)
Decompose the wavefield
![image2](44922408f5fd4592928e358b0bbe3d54.png)
![image3](d51ea5852ba24f8583294dc533873425.png)
![image4](36f2323cf5a34f019ad5d402fd1d702e.png)
![image5](062acbe90cf3411597abd0527224154e.png)
![image6](5906966edd3d4f8db652c47babbbede7.png)
![image7](27c591c7b938419e8f8fb309a8b40328.png)
![image8](2fa534c945b24c0189b2f3d61a8ac1c1.png)
![image9](d3f9ca29765d45c2827b7bf89a8df230.png)
![image10](4fde9031f9744e67baec138c8e12ef7c.png)
![image11](16455ffa3d214e8ca9a6da86f27d5296.png)
--\> first order smoothing
![image12](0cde7644e51b4f20aa4fa6b0a561973f.png)

**Mass operator**
Based on explicit form of \<L'GoL'\>
![image13](6d4d86173ecb4c129b5ac1febcde4614.png)
![image14](9f145baaec4e4c8a9cf0cdf00ea42063.png)
![image15](6a9112285ffc4f379711020c84bb94df.png)
![image16](3825ef70f1054d05b4b336df1cf4ee67.png)
![image17](3e7f6aa95bf64ba5af2f456f33bc4fe5.png)
In k-w domain, written as
![image18](6f6bd530a1a446bba3c3a6cfcaeaa54f.png)

Where M is mass operator, defined as
![image19](b787a69fab034dd9a8cee43993599949.png)
![image20](a53430d658cf4bae843405ce8178f95f.png)

![image21](f5ef78d98b704b3e84ce16ce520de773.png)
![image22](8a4b3abe31744c9d96230cafa37a81d6.png)
Mass operator means perturbation of the dispersion relation

**Mean Green function**
Mean green function in angular frequency domain definition
![image23](9a27a943348c4db69ed50e9a834337e2.png)
Apply first order smoothing method
![image24](c7630e474b3e47fc9307aef19cc11e18.png)

Written as
![image25](7b7a4060c28e44bfa070f87b7d26b0dc.png)
In k-w space, by using mass operator, written as
![image26](62fdda19f1c847619b8e286f16838e01.png)
Leads to
![image27](7337b34f128147248c2f58fc2230c35a.png)

Exponential ACF
![image28](7dfaabd592b74f278aa3ea784cc86e41.png)
By integrating over angle and radius, we get
![image29](9a5b8c89a6f04dc6837b8f63d753351a.png)
By substituting
![image30](11a16a1b519d41059821f0260802ee7b.png)

![image31](6c9c3b869bcb4cc89ee0244c36e57e3f.png)

![image32](f877dd6fb91540d88f708de908cf82dc.png)

![image33](4a2e9068cfed448f919f5876a1e0b195.png)

velocity shift scattering atten

![image34](8b91ef8329c34f26a22170d9a08eac30.png)
decays over distance a (no propagation)

Pole1 --\> coherent wave
Pole2 --\> near field mode (usually ignored)

The necessary conditions
![image35](2ba0c5dc02664da7af9933de4208ae77.png)
Multiple scattering is weak enough --\> all assumption valid (born approx, first order smoothing)
To make mean GF satisfy radiation condition
close the integral contour along the real axis and a half circle on the upper plane of the complex k-plane
![image36](93a992b8dd9a47f2a320b617607e02ee.png)
integral over the upper half circle is zero because of Jordan’s lemma
Calculating residue at 2 poles
![image37](ea9418014d084024bde9fbecb94b1288.png)

![image38](00bd374c5c1e431ba8bd34db35e4d1cf.png)
Second residue may be neglected
The final retarded mean green function equation
![image39](003308c98f51456a88efbec40205f08c.png)
Where the dispersion relation is given by ke1+
Real part -\> always larger than k0, velocity of mean wavefield is slower than unperturbed medium
Imag part -\> always positive, corresponds to attenuation per distance
![image40](24375a524cba4748a5c279b7f65367ba.png)
Then attenuation of mean wave is given as
![image41](1239faf48eef497890b76d370884bfb9.png)

General ACF
Green function may be rewritten as
![image42](daddda6d219e41c3bf6a0c2428ffa299.png)
When change in pole from k0 is small enough --\> general ACF formulation

![image43](273d0d48edef44aab37ed9e1abf1f414.png)
Substitute ke1+
![image44](b0272cedb6bf43a3acf25c85c3561a56.png)

![image45](f16957bc9ec54f7899868bc273f7e4e4.png)

Then can be rewritten as
![image46](fb0bc50ad4e542be93df380bd394e334.png)
Imaginary part always positive

Mean green function written as
![image47](ccd9d71a58b84e82a9aba6b49261f036.png)

Attenuation is
![image48](95b24359d3c14356ae1db1e00f7913d6.png)

