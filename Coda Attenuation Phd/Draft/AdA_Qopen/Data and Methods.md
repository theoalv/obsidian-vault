1 Seismic dataset
- This study uses waveform data from the AdriaArray Seismic Network, a dense network of permanent and temporary seismic stations deployed across the Circum-Adriatic region with an average station spacing of approximately 50 km [ref Kolinsky 2025]. 
- The AdriaArray experiment covers the Adriatic Plate and its tectonically active surroundings, extending from the Alps in the north to the Calabrian Arc and mainland Greece in the south.
- Waveform data were obtained through the European Integrated Data Archive (EIDA) using the Federated Data Service Network (FDSN) web services.
- The analyzed dataset spans from 1 January 2022 to 1 April 2026. Only stations providing good-quality three-component waveform recordings were included in this study.
- When multiple three-component channel groups were available at a station, high-frequency channels (HH* or EH*) were preferentially selected to maximize the frequency bandwidth for the high-frequency coda envelope analysis.
1.1 Event Catalog and Phase Picking
- Earthquake catalogs were compiled by merging the reviewed catalogs provided by the International Seismological Centre (ISC), GFZ, INGV, and IRIS for the study period. Duplicate events were identified based on their origin times, and when duplicate entries were found, the ISC Reviewed Catalog was given the highest priority because it provides the most thoroughly reviewed event information. Only crustal earthquakes with focal depths shallower than 40 km and magnitudes between 2.5 and 4.5 were retained. The resulting merged catalog initially contained 5,830 earthquakes.
- The use of accurate S-wave arrival times to define the bulk and coda windows used in the attenuation analysis will improve the result. Therefore, automatic S-wave phase picking was performed using the SeisBench framework. Three conservative pretrained models, namely PhaseNet (STEAD), GPD (INSTANCE), and EQTransformer (original), were applied sequentially, with minimum probability threshold of 0.3. When multiple models produced valid S-wave picks, the arrival time associated with the highest confidence score was selected. If none of the conservative models produced a reliable pick, the EQTransformer _original_nonconservative_ model was applied. When SeisBench failed to identify an S-wave arrival, a classical STA/LTA picker implemented in ObsPy was used with an STA window of 0.5 s, an LTA window of 6 s, and a trigger threshold of 2.5. If the STA/LTA picker also failed, the theoretical S-wave arrival time was calculated using the CRUST1.0 velocity model by constructing a one-dimensional average velocity profile for each source–receiver pair.
- For the coda envelope, we only analyze data from S wave arrival to ends of coda. Thus, we only focus on validating the S phase arrival. The S wave arrival is being validated with envelope peak. The arrival should earlier than the wave maximum, so we remove picks that tpeak-ts is negative and also we remove data with SNR below 4. There are 7.1% from the total phases that falls into this category, those picks were not used.
2 Full Coda Envelope Inversion
- Coda envelope theory
- qopen implementation
- frequency bands and other parameters
- estimation of scattering and intrinsic attenuation
3  Validation
- modified peak delay fitting
- modified late lapse coda Qc fitting