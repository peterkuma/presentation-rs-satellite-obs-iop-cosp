## Ross Sea Cloud Satellite Observations
### Objectives

\begin{columns}
\column{0.5\linewidth}
\begin{itemize}
\item Establish cloud climatology (*) over RS \& RIS as seen by CloudSat/CALIPSO
\item Follow-up on work by Coggins et al. (2016) on synoptic classification
in the region
\item Determine how cloud vertical distribution and properties vary with seasons
and synoptic regimes
\end{itemize}
\column{0.4\linewidth}
\includegraphics[width=50mm]{img/map.pdf}
\end{columns}

## Ross Sea Cloud Satellite Observations
### Coggins regimes

\footnotesize
Weak Northern Cyclonic (WNC), Strong Northern Cyclonic (SNC),
Ross Ice Shelf airstream (RAS), Weak Southern Cyclonic (WSC),
Weak Synoptic (WS)

\centering
\includegraphics[width=0.6\linewidth]{img/Coggins-regimes.pdf}

## Ross Sea Cloud Satellite Observations
### CloudSat-CALIPSO datasets

- Datasets:
    - 2B-GEOPROF-LIDAR P_R04 (2006--2011)
    - 2B-CLDCLASS-LIDAR P_R04 (2007--2011)
    - 2B-GEOPROF-LIDAR P_R05 (2006--2016)

---

## Ross Sea Cloud Satellite Observations
### Ice shelf vs. sea

\includegraphics[width=\linewidth]{img/cloud_incidence_by_phase_regime.pdf}

---

## Ross Sea Cloud Satellite Observations
### What is the role of seasons compared to weather regimes

\vspace{3mm}
\begin{columns}[onlytextwidth]
\column{0.65\linewidth}
\includegraphics[width=\textwidth]{img/cloud_layers_hist_cldclass.pdf}
\column{0.35\linewidth}
\includegraphics[width=\textwidth]{img/cloud_incidence_information_gain_ris_type.pdf}
\end{columns}

## Ross Sea Cloud Satellite Observations

### 2B-GEOPROF-LIDAR P_R04 data issues

\vspace{5mm}
\begin{columns}[onlytextwidth]
\column{0.5\textwidth}
\includegraphics[width=\linewidth]{img/cloud_incidence_multi.pdf}
\column{0.5\textwidth}
\includegraphics[width=\linewidth]{img/correction_factor.pdf}
\par
\footnotesize
Ratio of cloud occurrence at 8.3 km rel. to 8 km
\end{columns}

## IOP
### Objectives

- Create a comprehensive multi-year dataset of ground-based and in-situ observations of
C&A in the SO

- Use them for NZESM evaluation and improve C&A parametrisation in the SO

## IOP
### Instruments

\begin{columns}
\column{0.4\linewidth}
\begin{itemize}
\item Ceilometer: Lufft CHM 15k, Vaisala CL51
\item Radar: Metek MRR-2
\item Radiosondes
\item Sky-viewing camera
\item AWS, pyranometers
\item Aerosols (NIWA)
\end{itemize}
\column{0.4\linewidth}
\includegraphics[width=40mm]{img/instruments.pdf}
\end{columns}

## IOP
### Complementing observations

\centering
\includegraphics[width=0.55\linewidth]{img/iop.pdf}

<!--
## IOP
### Observation campaigns

- Aurora Australis
- Macquaire Island (2016--)
- RV Tangaroa (2015), 2\texttimes
- HMNZS Wellington (2016)
- RV Tangaroa (2017)
- Nathaniel B. Palmer (2017)
 -->

## IOP
### Plans

- Complete dataset:
    - All deployments
    - Well-documented
    - Standard data formats: NetCDF/HDF5 (CF)
    - Publicly available

## COSP
### Objectives

- Evaluation of NZESM using ground and in-situ observations of C&A
in the Southern Ocean
- Use the COSP satellite simulator developed by CFMIP

## COSP
### Observations

- Ground-based and in-situ:
    - IOP
    - ARM
- Satellite:
    - Passive VIS & IR: ISCCP, MODIS, MISR, ...
    - Radiative budget: CERES
    - Active: CloudSat, CALIPSO (possibly GLAS, CATS, EarthCARE)
    - Passive microwave (total column water): AMSR-E (Aqua), AMSR-2 (GCOM-W1),
    SSM/I (DMSP), MIS (NPOESS), TMI (TRMM)

## COSP
### Simulators

- ACTSIM -- lidar simulator
    - Input: water/ice mixing ratio (convective and stratiform),
    effective radius of cloud/ice particles
    - Output: backscatter

- QuickBeam -- radar (CloudSat) simulator

## COSP
### Comparing the same thing

\begin{columns}
\column{0.3\linewidth}
\begin{itemize}
\item Analogy: `Blind men and an elephant'
\end{itemize}
\column{0.6\linewidth}
\includegraphics[width=65mm]{img/blind-men-and-an-elephant.jpg}
\end{columns}

- Same physical quantity
- Resolution problem
- Spatial/temporal co-location
- Choice of False Alarm Ratio

## COSP
### Mean seasonal cloud fraction (Bromwich et al., 2012)

\centering
\includegraphics[width=0.55\linewidth]{img/Bromwich.png}

## COSP
### Ceilometer (IOP) vs. CALIPSO

- 2017-03-21 05:00 UTC, Campbell Plateau

\includegraphics[width=\linewidth]{img/iop-calipso.pdf}

## COSP
### Model vs. observation vs. reality

\begin{tabular}{p{0.45\textwidth} p{0.45\textwidth}}
\textbf{Model} &
\textbf{Observation}\\
\footnotesize
Cloud vertical distribution, fraction, phase, liquid/ice mixing ratio \newline
Droplet size distribution/effective radius \newline
Cloud subsampling (McICA) and overlap \newline
Radiative transfer approximations \newline
Cloud types: convective, stratus \newline
Temperature profile and gas concentration &
\footnotesize
Cloud fraction, top, base, optical depth, geometric depth \newline
Backscatter, radar reflectivity \newline
Cloud types: Cu, St, Sc, DC, Ci \newline
Temperature, humidity, pressure profile \newline
Affected by error (type I, II, Gaussian, ...), bias, limited
view, coverage, spatial/temporal res., spectral res.
\end{tabular}

\begin{tabular}{p{0.8\textwidth}}
\textbf{Reality}\\
\footnotesize
Cloud droplet and ice crystal distribution \newline
Aerosol distribution \newline
Temperature profile and gas concentration
\end{tabular}

## COSP
### NZESM

- Nudged
- Unnudged
- COSP:
    - From model fields to pseudo-observations to derived properties

## COSP
### The other way round

- Assimilation
- From observations to model fields (with proper uncertainty evaluation)
- Can we put multiple observations together?

## COSP
### Upscaling

- Correlating ground-based observations with satellite observations
- Deriving pseudo ground-based observations based on satellite observations:
    - If we know what the satellite instruments sees, what would ground-based
    instruments be likely to see?

## COSP
### Challenges

- Subsampling (cloud resolving model)
- Nudging
- Small and irregular temporal and spatial coverage
- From backscatter to cloud layers
