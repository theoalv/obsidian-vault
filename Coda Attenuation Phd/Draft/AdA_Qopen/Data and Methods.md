1 Seismic dataset
- This study uses waveform data from the AdriaArray Seismic Network, a dense network of permanent and temporary seismic stations deployed across the Circum-Adriatic region with an average station spacing of approximately 50 km [ref Kolinsky 2025]. 
- The AdriaArray experiment covers the Adriatic Plate and its tectonically active surroundings, extending from the Alps in the north to the Calabrian Arc and mainland Greece in the south.
- Waveform data were obtained through the European Integrated Data Archive (EIDA) using the Federated Data Service Network (FDSN) web services.
- The analyzed dataset spans from 1 January 2022 to 1 April 2026. Only stations providing good-quality three-component waveform recordings were included in this study.
- When multiple three-component channel groups were available at a station, high-frequency channels (HH* or EH*) were preferentially selected to maximize the frequency bandwidth for the high-frequency coda envelope analysis.
1.1 Event Catalog and Phase Picking
- We combine all of the available event catalog from ISC reviewed, GFZ, INGV, and IRIS for the time window. we use crustal event (below 40 km depth) with magnitude of 2.5 to 4.5. We obtain a total of 5830 events from the combined catalog.
- To estimate the S wave arrival for an accurate bulk window analysis, we use SeisBench to do automatic phase picking. We use 3 conservative models and choose pick with higher uncertainty. If these 3 models fails, then move to nonconservative model. If all of these model fail we try to calculate pick with classic STA/LTA (obspy) with 2.5 threshold, and 0.5 s STA and 6 s LTA. if the STA/LTA method fail, we calculate theoretical pick. The theoretical pick is calculated with CRUST1.0 velocity model. First we calculate averaged velocity model for each event from the velocity model, then followed by calculate the arrival.
- For the coda envelope, we only analyze data from S wave arrival to ends of coda. Thus, we only focus on validating the S phase arrival. The S wave arrival is being validated with envelope peak. The arrival should earlier than the wave maximum, so we remove picks that tpeak-ts is negative. However from
2 Full Coda Envelope Inversion
- Coda envelope theory
- qopen implementation
- frequency bands and other parameters
- estimation of scattering and intrinsic attenuation
3  Validation
- modified peak delay fitting
- modified late lapse coda Qc fitting