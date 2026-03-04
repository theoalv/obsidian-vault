---
title: Site Amplification Measurements
updated: 2026-01-26T08:56:06
created: 2026-01-23T17:51:17
---

At sufficiently late lapse times, difference in S-coda amplitudes between stations are caused by site amplification

Relative CN amplification factor
![image1](8ba7592ea9e74349bdfad9b275e7daea.png)
Computing ratios relative to one reference site (k)

Choose lapse time when coda energy is uniformly distributed and contains both stations
As individual coda window can be noisy, then
Use many windows, earthquakes --\> average the ratios

S coda with direct S wave spectral ratio show a nearly identical site amplification
--\> confirms S-coda carries same site response as direct S waves
S coda advantages:
Insensitive to radiation pattern
Distance independent
--\> can be used even if azimuthal coverage is poor

During large scale applications to map site amp, results are stable across earthquakes and lapse time (**for most sites**)
Some of the result is lapse time dependent (local energy slow decay)
Cause --\> sedimentary basin, strong velocity contrast
--\> violates uniform coda assumption

CN method generally uses coda waves with small amplitudes
Large earthquakes often decrease ground rigidity --\> site amp changed

**CN Site amp practical steps:**
Data requirements:
- Aftershock dataset
- Station array, at least one at reference site (bedrock)
- Waveform (same instrument or IRC)
Steps:
1.  Preprocess waveform
2.  Choose frequency bands --\> octave bands
3.  Define S arrival time (Ts)
4.  Define lapse time (Tc)
5.  Compute coda amplitude
6.  Compute CN ratios
7.  Stack over time windows and event

<span style='font-weight:bold;background:#FFFF99'>Try compare CN site amp measurements with HVSR</span>
