---
title: "Growth vs. light-capture in PhycoCyanin and PhycoErythrin-rich picocyanobacteria, across photic regimes and growth phases"
author:
- Sylwia Śliwińska-Wilczewska:
    institute:
    - MTA
    - UG
    email: ssliwinskawilczews@mta.ca
- Marta Konik:
    institute:
    - VU
    - IOPAN
    email: mk@iopan.gda.pl
- Mireille Savoie:
    institute: MTA
    email: msavoie@mta.ca
- Naaman Omar:
    institute: MTA
    email: nomar@mta.ca
- Douglas A. Campbell:
    institute: MTA
    email: dcampbel@mta.ca
    correspondence: true
institute:
- MTA: Department of Biology, Mount Allison University, 53 York St., Sackville NB,
    Canada, E4L 1C9
- UG: "Institute of Oceanography, University of Gdansk, 46 Pilsudskiego St, P81-378,
    Gdynia, Poland"
- VU: Department of Geography, University of Victoria, Victoria, BC V8P 5C2, Canada
- IOPAN: "Institute of Oceanology, Polish Academy of Sciences, 81-712 Sopot, Poland"
output:
  bookdown::word_document2:
    reference_docx: Template.docx
    code-folding: show
    keep_md: yes
    fig.caption: yes
    toc: FALSE
    pandoc_args:
    - "--lua-filter=scholarly-metadata.lua"
    - "--lua-filter=author-info-blocks.lua"
  html_document:
    df_print: paged
  word_document:
    reference_docx: Template.docx
    code-folding: show
    keep_md: yes
    fig.caption: yes
    toc: FALSE
    pandoc_args:
    - "--lua-filter=scholarly-metadata.lua"
    - "--lua-filter=author-info-blocks.lua"
bibliography:
- BalticPhotoperiod.bib
- packages.bib
csl: "limnology-and-oceanography.csl"
---









# Abstract {.unnumbered}

Picocyanobacteria are the most abundant phytoplankters in aquatic ecosystems and are crucial to the optical properties of ocean water, influencing its colour and transparency. The genus *Synechococcus* occurs in tropical, subtropical, temperate and arctic zones, with long-term scenarios forecasting range  expansions of *Synechococcus* sp.

Our study demonstrated that cumulative diel photon dose consistently explain achieved growth rates (µ) of two PhycoCyanin(PC)-rich and two PhycoErythrin(PE)-rich strains of *Synechococcus*, across a matrix of 4 photoperiods and 6 peak Photosynthetically Active Radiation (PAR). Growth responses to cumulative diel photon dose, depending upon photoperiod and peak PAR varied across the strains. All the strains were generally opportunistic in exploiting higher light diel doses to achieve faster µ, although PE-rich strains suffered strong photoinhibition of growth under peak PAR 900 µmol photons m^−2^s^−1^ and 24 h photoperiod. The results revealed consistent patterns of light capture efficacy; Photosynthetically Usable Radiation (PUR)/PAR ratio and pigment content (Phycobiliprotein to Chl *a* ratio) across cumulative diel photon doses. The PE-rich strains showed a much higher PUR/PAR ratio and Phycobiliprotein/Chl *a* ratio under low cumulative diel photon dose, but decay reached a plateau close to the PC-rich strains as cumulative diel photon dose increased. The $\sigma$~PSII~' showed a consistent, sharp exponential decay in relation to cumulative diel photon dose, across different combinations of photoperiod and peak PAR. However, the PE-rich strains remained at the higher $\sigma$~PSII~' level under low cumulative diel photon dose than the PC-rich strains even as cumulative diel photon dose increased. The $\sigma$~PSII~' was related to the phycobilisome:chlorophyll *a* ratio, where the $\sigma$~PSII~' excited through phycobilisome absorbance at 590 nm were positively correlated with Phycobiliprotein to Chl *a* ratio. However, in the exponential growth phase, high variability was observed, likely related to regulatory control of $\sigma$~PSII~' beyond pigment composition. Under pre-stationary phase $\sigma$~PSII~' vs. Phycobiliprotein to Chl *a* ratio was better aligned, suggesting an increase in reliance upon compositional regulation to control light delivery to PSII, as opposed to shorter-term regulation. We also found that µ saturated under increasing PSII electron flux (*JV*~PSII~, e^−^cell^−1^d^−1^) for all strains; however, the achieved estimates of µmax varied depending upon peak diel PAR. 

Our results show the PE-rich strains are stronger light-harvesting competitors however, the PC-rich strains may have lower N-quotients for their light capture system. These differences help explain the differential seasonal prevalence of PE-rich and PC-rich picocyanobacteria in terms of the costs of exploitation of different photic regimes. This work provides an important link in forecasting global changes in the occurrence of PC-rich and PE-rich *Synechococcus* phenotypes in aquatic ecosystems in the context of future climate change.

# Introduction {.unnumbered}

The photic regime, comprised of Photosynthetically Active Radiation (PAR), photoperiod, and spectral quality, is a pivotal influence on the growth and productivity of phytoplankton within aquatic ecosystems. PAR refers to the spectral range of solar radiation, approximately 400-700 nm,  that is capable of driving photosynthesis. Photosynthetically Usable Radiation (PUR), in turn, is the fraction of PAR of wavelengths that can be absorbed by particularly cyanobacteria or algae [@morelAvailableUsableStored1978]. The PAR reaching a specific area, directly affects the physiology of cyanobacteria [@aguileraEcophysiologicalAnalysisReveals2023; @sliwinska-wilczewskaPhotosyntheticPigmentsChanges2020; @sliwinska-wilczewskaEcophysiologicalCharacteristicsRed2018]. Optimal PAR provide the energy for photosynthesis, and thus supports cyanobacteria growth and biomass production. The availability and distribution of PAR in aquatic ecosystems are influenced by cloud cover, water depth, and light attenuation due to water turbidity and suspended particles, including phytoplankton cells [@kirkLightPhotosynthesisAquatic1983; @fieldPrimaryProductionBiosphere1998; @torremorellAnnualPatternsPhytoplankton2009]. Cyanobacteria are also sensitive to changes in photoperiod, which serves as a key environmental cue for their metabolic activities and life cycle events [@huismanHowSinkingPhytoplankton2002; @alberteFunctionalOrganisationPhotosynthetic1980; @larochePelagicLightDependentMicrobiome2022]. The duration of light exposure within a day regulates physiological processes, including photosynthesis, growth, reproduction, and nutrient assimilation in cyanobacteria. Thus, in polar regions, characterized by prolonged periods of wintertime darkness and continuous daylight during summer, cyanobacteria encounter unique challenges. Light is the primary limiting factor for biomass production in winter, suppressing cyanobacteria growth and metabolic activity, whereas the extended daylight in summer boosts photosynthetic activity [@arrigoSeaIceEcosystems2014]. In temperate regions, seasonal variation in light-limitation is less pronounced, but cyanobacteria are still influenced by daily and seasonal fluctuations. There is a clear contrast between more favorable conditions for cyanobacteria growth in spring and summer, compared to fall and winter [@huismanHowSinkingPhytoplankton2002; @holtropVibrationalModesWater2021]. In the tropics, daylight remains nearly constant throughout the year [@behrenfeldClimatedrivenTrendsContemporary2006], and cyanobacteria productivity is rather controlled by nutrients resupply into the euphotic zone [@hutchinsMarinePhytoplanktonChanging2016; @liPhytoplanktonResponsesNitrogen2015], and mortality through viral lysis [@ortmannLysogenyLyticViral2002] and zooplankton grazing [@christakiGrowthGrazingProchlorococcus1999].

Cyanobacteria growth includes lag, exponential growth, stationary, and death phases [@reynoldsEcologyPhytoplankton2006]. During the lag phase, cyanobacteria acclimate to the environment and prepare for active growth by synthesizing essential cellular components. Exponential growth phase is marked by cell division and biomass accumulation, fueled by nutrient and light availability. If growth is limited by declining nutrients or light, or by accumulation of inhibitory factors, algae enter the stationary phase, characterized by a balance between cell division and death, leading to a plateau in population. The death phase occurs when  cyanobacteria cell death outruns division, leading to decomposition, contributing to nutrient recycling in aquatic ecosystems [@reynoldsEcologyPhytoplankton2006]. Cell death may also release toxins into the environment. Understanding the temporal progression of growth phases is thus essential for predicting cyanobacterial activity in a habitat, and their impact on ecosystem dynamics over time.

*Synechococcus*, a diverse genus of picocyanobacteria, exhibits a distribution spanning diverse geographical regions [@flombaumPresentFutureGlobal2013], with strains demonstrating a remarkable range of adaptations to environmental conditions. *Synechococcus*’ capacity to thrive across diverse marine and freshwater habitats positions it as a pivotal agent in energy and nutrient transfer within food webs and serves as a link connecting the microbial loop with higher trophic levels, offering direct sustenance to grazers, including zooplankton and small fish [@liCompositionUltraphytoplanktonCentral1995]. *Synechococcus*, as one of the two dominant picocyanobacterial genera in oceanic waters, also significantly affects light attenuation and availability for other photosynthetic organisms, and influences ocean colour, allowing satellite detection of *Synechococcus*-rich communities [@bracherObtainingPhytoplanktonDiversity2017; @xiGlobalRetrievalPhytoplankton2020]. General relations among optical absorption spectra and pigment compositions have been used to determine diagnostic pigment indices of major phytoplankton functional types [@vidussiPhytoplanktonPigmentDistribution2001; @fishwickFunctionalRelationshipsBiooptical2006; @hirataSynopticRelationshipsSurface2011]. Modeling suggests that *Synechococcus* abundance and ranges will increase  due to climate warming [@flombaumPresentFutureGlobal2013]. The projected changes may vary geographically and may include shifts in the spatial distribution of the main picocyanobacteria, as well as changes in the proportions among *Synechococcus* sp. lineages [@sixMarineSynechococcusPicocyanobacteria2021]. *Synechococcus* exhibits significant phenotypic diversity across lineages, encompassing strains rich in PhycoErythrin (PE-rich) or PhycoCyanin (PC-rich) [@haverkampColorfulMicrodiversitySynechococcus2009; @aguileraEcophysiologicalAnalysisReveals2023]. These phycobilin pigment-proteins are pivotal for light absorption during photosynthesis and confer distinctive colours to the picocyanobacteria. The disparate light preferences between PC-rich and PE-rich *Synechococcus* sp. strains influence their ecological niches. PC-rich strains thrive in environments with elevated light levels, such as surface waters and coastal regions, where blue light predominates. PE-rich strains exhibit adaptation to lower-light conditions, primarily inhabiting the deeper layers of the water column where green light prevails. PC-rich and PE-rich *Synechococcus* sp. strains thus predominantly occupy complementary habitats [@sixLightVariabilityIlluminates2007; @haverkampColorfulMicrodiversitySynechococcus2009; @sixMarineSynechococcusPicocyanobacteria2021].

Photic regimes and growth phases of PC-rich and PE-rich *Synechococcus* sp. may drive spatial and temporal variability of *Synechococcus* biomass and community lineage composition within aquatic environments, relating to varying metabolic costs between physiological strategies. Therefore, the aim of this research was to determine whether photic regimes and growth phases affect both growth and light-capture, and quantify the differences between impacts on PC-rich and PE-rich *Synechococcus* sp.

# Material and Methods {.unnumbered}

## Culture condition and experimental setup {.unnumbered}

Two non-axenic PhycoCyanin(PC)-rich (CCBA_056 or CCBA_077) strains and two PhycoErythrin(PE)-rich (CCBA_048 or CCBA_127) strains of *Synechococcus* were obtained from the Culture Collection of Baltic Algae (CCBA; https://ccba.ug.edu.pl/pages/en/home.php). Pre-cultures of picocyanobacteria strains were kept in Tissue Culture Flasks (VWR International, Cat. No. 10062-872, PA, USA) and were transferred to fresh f/2 media [@guillardCulturePhytoplanktonFeeding1975] at salinity of 8 PSU (which corresponds to their natural habitat) every two weeks, under a photoperiod of 12 h and Photosynthetically Active Radiation (PAR) of 10 µmol photons m^−2^s^−1^ supplied from cool white fluorescent tubes, at 22℃.

Cultures of each strain were grown in 8 x 80 mL round bottom cylindrical glass tubes in a Multi-Cultivator MC 1000-OD (Photon Systems Instruments, Drásov, Czech Republic). Each culture tube contained 75 mL of f/2 medium inoculated with 5 mL of growing pre-culture, to achieve exponential growth from the beginning of the experiment, with little to no lag phase upon inoculation. Culture tubes were inoculated in the afternoon, and the first photoperiods followed in the morning so that peak PAR occurs around noon each day.

Cultures grew at 22℃, with photoperiods of 8, 12, 16, or 24 h, with peak PAR of 30, 90, 180, 300, 600, or 900 µµmol photons m^−2^s^−1^ supplied from white LED lamps, independently to each culture tube. To approximate diel cycles, the photoperiods of 8 – 16 h were applied in a sinuisoidal shape, while the 24-hour photoperiod was applied continuously in a square shape. The area under the sinuisoidal  curve is 1/2 the area under a square of equal width, the 24 h square photoperiod cultures received 4 times the diel photon dose of the 12 h sinuisoidal  photoperiod cultures.

Culture tubes were closed with a silicone inert silicone stopper perforated by an aeration input tube extending to the bottom of the culture tube, and a pressure outlet tube. Aeration with a total air flow rate of around ~ 140 mL min^−1^ tube^−1^ ensured mixing and provided sufficient air/CO2 supply to cultures through the entire culture volume. The pH of tested cultures did not fluctuate fiercely during the experiment and remained at approximately 8-9. Light, temperature, optical density, and aeration gas of the Multi-Cultivator system were monitored and controlled via the Photobioreactor Control Software (Photon Systems Instruments, Drásov, Czech Republic).

## The growth curve and chlorophyll specific exponential growth rate analysis {.unnumbered}

Picocyanobacterial growth was monitored every 5 minutes by automatically recording OD~680~, OD~720~, and ΔOD (ΔOD = OD~680~ – OD~720~) for 14 days, independently for each culture tube. The exceptions were experiments conducted with a photoperiod of 24 h and light of 600 or 900 µmol photons m^−2^s^−1^, which lasted 7 days (Fig S1-S3 in Supplementary materials).

The exponential chlorophyll specific exponential growth rates (µ) were determined by fitting logistic growth curves to plots of the chlorophyll *a* proxy of ΔOD vs. elapsed time for each combination of strain, photoperiod, and peak PAR (Fig. S4 in Supplementary materials).

The 1^st^ derivative of OD~680~ taken over 1 h increments was computed. The time when the cultures reached their maximum absolute hourly growth (tMaxAHG) of the 1^st^ derivative of OD~680~, was taken as the time of transition from exponential to pre-stationary growth phases (Fig. <a href="#fig:FirstDerivative">1</a>).

![<span id="fig:FirstDerivative"></span>Figure 1: **Example of a growth curve (tracked as OD~720~, OD~680~, or ΔOD; red solid lines, left y-axis) of PE-rich culture of *Synechococcus* sp. (048) vs. elapsed time (d, x-axis).** 1^st^ derivative of OD~680~ taken over 1 h increments (black solid line, right y-axis); solid blue line shows logistic fits of chlorophyll proxy OD~680~ – OD~720~ (ΔOD) vs. elapsed time. The vertical red dot dash line represents the time when the culture reached the maximum of the 1^st^ derivative of OD~680~, or maximum absolute hourly growth (tMaxAHG), taken as the time of transition from exponential to pre-stationary growth phases.](../Output/Figures/Fig_FirstDerivative.png)

## Determining the number of cells {.unnumbered}

The number of picocyanobacterial cells was calculated using linear regression models based on cell suspension density (cell mL^−1^), counted using a PAMAS S40 GO Particle counter (PAMAS Partikelmess- und Analysesysteme GmbH, Rutesheim, Germany) and OD~680~ measured using a CLARIOstar Plus Plate Reader (BMG, Labtech, Ortenberg, Germany). Linear correlations between N and OD~680~ for individual strains were used to estimate the number of cells based on OD measurements obtained from the Multi-Cultivator system (Tab. S1, Supplementary materials).

## Whole-cell absorbance spectra measurements {.unnumbered}

Absorbance measurements on intact cells in suspension were conducted in an integrating cavity upgrade spectrophotometer (OLIS CLARiTY 17 UV/Vis/NIR, On-Line Instrument Systems, Inc., Bogart, GA, USA) according to [@blakeSituSpectroscopyIntact2012] with modifications. 8 mL of f/2 medium were added to both the sample and reference observation cavities of the spectrophotometer. After recording a baseline from 375 to 710 nm, 1 mL was withdrawn from the sample cavity and replaced with 1 mL of the cell suspension of tested picocyanobacteria. The pathlength corrected absorbance per cm was performed by determining the Javorfi coefficients [@javorfiQuantitativeSpectrophotometryUsing2006] as described in the equipment manual.

## Estimating Photosynthetically Usable Radiation (PUR) {.unnumbered}

Using whole-cell absorbance spectra of *Synechococcus* sp. cultures (Fig. <a href="#fig:OlisSpectra">2</a>) we estimated Photosynthetically Usable Radiation (PUR) according to [@morelAvailableUsableStored1978]. We normalized the obtained whole-cell Absorbances (A) and the Emission spectra of the white LED lamps (Em) taking over 400 nm to 700 nm to a reference wavelength of 440 nm. PUR is then the ratio of the sum of Absorbance Normalized to 440 nm (NormA~440nm~) ✕ sum of Emission spectra Normalized to 440 nm (NormEm~440nm~) to the sum of the Emission spectra Normalized to 440 nm (NormEm~440nm~) multiplied by the PAR (Eq. (1)).

$$\begin{equation}
  PUR=\frac{∑(NormA_440nm~✕~NormEm_440nm)}{∑(NormEm_440nm)}~✕~PAR
  \qquad(1)
\end{equation}$$

![<span id="fig:OlisSpectra"></span>Figure 2: **Whole-cell absorbance spectra of PC-rich (solid green lines) or PE-rich (dashed red lines) cultures of *Synechococcus* sp.** Representative absorbance spectra, normalized to A~440nm~, were measured from the exponential or pre-stationary phases of growth, together with emission spectra of the white LED lamp used for PAR, normalized to emission at 440 nm (Em~440nm~, light gray area), in this example PAR was 300 µmol photons m^−2^s^−1^. Estimated Photosynthetically Usable Radiation (PUR) is shown as a green area for the PC-rich strain and a red area for the PE-rich strain, with PUR given for each culture (µE = µmol photons m^−2^s^−1^). Peaks characteristic of known pigments are labeled; Chl *a*, chlorophyll *a*; PC, phycocyanin; PE, phycoerythrin; PUB, phycourobilin; Car, carotenoids.](../Output/Figures/Fig_OlisSpectra.png)

## Pigment content analysis {.unnumbered}

The pigment content: chlorophyll *a* (Chl *a*), carotenoids (Car), phycoerythrin (PE), phycocyanin (PC), and allophycocyanin (APC) in *Synechococcus* sp. cultures over time was estimated with previously determined linear correlations between pigment content obtained by extraction technique and absorbance values of individual pigment peaks (nm) obtained from the whole-cell absorbance spectra. Linear regression, coefficient of determination, Pearson correlation coefficients, and *p*-value were presented in Tab. S2 (Supplementary materials). The sum of phycobilins (PE, PC, APC protein; Phycobiliprotein) to Chl *a* ratio (µg/µg) for individual strains was also calculated.

Pigments extraction were performed using formula from Strickland and Parsons [@stricklandPracticalHandBook1972] for Ch *a* and Car concentrations. PE, PC, and APC were calculated based on Bennett and Bogorad [@bennettCOMPLEMENTARYCHROMATICADAPTATION1973]. The extracts contained photosynthetic pigments were measured using a CLARIOstar Plus Plate Reader (BMG, Labtech, Ortenberg, Germany), at wavelengths of 480, 665, and 750 nm for Chl *a* and Car calculation and at 565, 620, 650, and 750 nm for PE, PC, and APC. The values of individual pigment peaks (nm) from the whole-cell absorbance spectra were obtained by Olis-modernized Cary 14 UV/Vis/NIR with Integrating Sphere upgrade spectrophotometer (On-Line Instrument Systems, Inc., Bogart, GA, USA). For the linear model, the following wavelengths were analyzed: 480 (Car), 565 (PE), 620 (PC), 650 (APC), and 665 (Chl *a*) nm.

## Estimating cumulative diel PAR {.unnumbered}

Based on the length and shape of the photoperiod (sine wave for photoperiod of 8 – 16 h; square for photoperiod of 24 h) and the given light level, we estimated the value of the cumulative diel PAR dose (µmol photons m^−2^d^−1^). For a photoperiod arranged in the shape of a sine wave we used Eq. (2). For a continuous 24 h photoperiod we used Eq. (3).

$$\begin{equation}
\begin{split}
  PAR~dose~(µmol~photons~m^{−2}~d^{−1})= \\ \frac{PAR~(µmol~photons~m^{−2}~s^{−1})⋅60~(s~min^{−1})⋅60~(min~h^{−1})⋅photoperiod~(h~d^{−1})}{2}
  \qquad(2)
\end{split}
\end{equation}$$

$$\begin{equation}
\begin{split}
  PAR~dose~(µmol~photons~m^{−2}~d^{−1})= \\ PAR~(µmol~photons~m^{−2}~s^{−1})⋅60~(s~min^{−1})⋅60~(min~h^{−1})⋅photoperiod~(h~d^{−1})
  \qquad(3)
\end{split}
\end{equation}$$

## Changes effective absorption cross section of PSII and PSII flux {.unnumbered}
xxx I really need Doug help here!

Calculation of the absorption cross section of PSII photochemistry ($\sigma$~PSII~'; nm^2^ quanta^−1^) under ambient light through an iterative curve fit to the saturation phase of a Fast Repetition Rate fluorometry (FRRf) single turnover (ST) measurement of tested picocyanobacteria were obtained using SoliSense laser-induced fluorescence transient (LIFT) fluorometer equipped with a prototype temperature control unit (LIFT-REM, Soliense Inc., New York, USA). PSII electron flux (JV~PSII~; e^−^cell^−1^d^−1^) was calculated according to the method proposed by [Campbell?; Oxborough et al., 2012]. 

PC-rich and PE-rich picocyanobacteria were measured under diel peak PAR growth light under a blue LED (Ex~445nm~) and orange (Ex~590nm~) excitation. Excitation protocols were used to manipulate the level of photosynthetic activity and chlorophyll fluorescence (ChlF). Flash Power for blue excitation was 60000 and for orange excitation was 14000 µmol photons m^−2^s^−1^. The intensity of the blue and orange LIFT LED in DC mode and excitation power were calibrated using a quantum sensor (LI-250, LI-COR, Inc.). Data were collected during a rapid light curve (RLC; Fig. <a href="#fig:LIFT">3</a>) sequence during which light intensity was increased from 0 to 320 µmol photons m^−2^s^−1^ and then decreased from 320 to 0 µmol photons m^−2^s^−1^ with a 1-s pause in darkness between measurements. Acquisitions were made at 10-s intervals. [Campbell and Kolber?; Kolber et al., 2005; Oxborough et al., 2012].


Kolber, Z., Klimov, D., Ananyev, G., Rascher, U., Berry, J., & Osmond, B. (2005). Measuring photosynthetic parameters at a distance: laser induced fluorescence transient (LIFT) method for remote measurements of photosynthesis in terrestrial vegetation. Photosynthesis research, 84, 121-129.

Oxborough, K., Moore, C. M., Suggett, D. J., Lawson, T., Chan, H. G., & Geider, R. J. (2012). Direct estimation of functional PSII reaction center concentration and PSII electron flux on a volume basis: a new approach to the analysis of Fast Repetition Rate fluorometry (FRRf) data. Limnology and Oceanography: Methods, 10(3), 142-154.

Keller, B., Vass, I., Matsubara, S., Paul, K., Jedmowski, C., Pieruschka, R., ... & Muller, O. (2019). Maximum fluorescence and electron transport kinetics determined by light-induced fluorescence transients (LIFT) for photosynthesis phenotyping. Photosynthesis Research, 140, 221-233.

![<span id="fig:LIFT"></span>Figure 3: **Single turnover (ST) fluorescence induction by Fast Repetition Rate fluorometry (FRRf).** Examples of fluorescence yield vs. elapsed time (µs) are shown for PE-rich culture of *Synechococcus* sp. (048) in the dark (dark-adapted; 0 µmol photons m^−2^s^−1^) and under actinic PAR (in this example 80 µmol photons m^−2^s^−1^) measured using blue LED (Ex~445nm~) or orange (Ex~590nm~) excitation (A). The ST technique delivers a series of flashlets for non-intrusive, repeated monitoring of chlorophyll fluorescence parameters (including *F*~0~, *F*', *F*~m~, *F*~m~', τ~1~-τ~3~, τ~1~'-τ~3~', σ~PSII~, and σ~PSII~'). Bottom panel shows a rapid light curve (RLC), estimated with with a three parameter model [@harrisonPhotosynthesisirradianceRelationshipsPolar1986], for PSII electron flux (*JV*~PSII~; e^−^L^−1^s^−1^) vs. actinic PAR measured under blue LED (Ex~445nm~) or orange (Ex~590nm~) excitation (B).](../Output/Figures/Fig_LIFT.png)

## Statistical analysis {.unnumbered}

All analysis of obtained results was conducted using R version 4.3.0 [@rcoreteamLanguageEnvironmentStatistical2019] running under RStudio [@teamrstudio.RStudioIntegratedDevelopment2015]. To determine significant differences in studied experiments the “stats” v. 3.6.2 R standard packages were used. This package provides basic statistical functions, including the *lm()* function for linear regression, *aov()* function for ANOVA, and *t.test()* function for t-test. The *SSasymp()* function (Self-Starting Nls Asymptotic Regression Model) was used to perform a single phase exponential decay fit model and to estimate exponential decay parameters (y0, the starting value; yf, the value at infinite times; $\lambda$, exponential decay constant) [@serwayModernPhysics2004]. A modified Levenberg-Marquardt fitting algorithm [@elzhovMinpackLmInterface2023] was used for estimating logistic fits of chlorophyll proxy OD~680~ – OD~720~ vs. elapsed time for each combination of strain, photoperiod, and peak PAR. We also used *nlsLM()* function [@elzhovMinpackLmInterface2023] to perform a three parameter model ($\alpha$, initial slope of curve; $\beta$, reflecting the photoinhibition process; P~max~, the maximum rate of growth curve) proposed by Harrison and Platt [@harrisonPhotosynthesisirradianceRelationshipsPolar1986].

Linear regressions were used to calculate the number of cells (N mL^−1^) and pigment content (µg mL^−1^) for two PhycoCyanin(PC)-rich cultures (056, 077) and two PhycoErythrin(PE)-rich cultures (048, 127) of *Synechococcus* sp. originating from the Baltic Sea. Linear regression, coefficient of determination (R square), Pearson correlation coefficients (R), and *p*-value were presented in Table S1-S2 (in Supplemental material).

We performed three-way factorial ANOVA of chlorophyll specific exponential growth rate, estimated from logistic fits of chlorophyll proxy OD~680~ – OD~720~ vs. cumulative diel PUR dose and cumulative diel PAR dose (Table S3, Sxxx), PUR/PAR ratio vs. cumulative diel PAR dose (Table S6), Phycobiliprotein to Chl *a* ratio vs. cumulative diel PAR dose (Table S8), and effective absorption cross section of PSII ($\sigma$~PSII~'; nm^2^ quanta^−1^) measured under diel peak PAR growth light under Ex~445nm~ (blue) or under Ex~590nm~ (orange) excitation in relation to the cumulative diel PAR dose or in relation to the Phycobiliprotein to Chl *a* ratio (Table S10, S12, S14, S16 in Supplemental material). We also run three-way factorial ANOVA of chlorophyll specific exponential growth rate, estimated from logistic fits of chlorophyll proxy OD~680~ – OD~720~ vs. PSII electron flux (JV~PSII~; e^−^cell^−1^d^−1^) (Table Sxxx).

To examine statistical differences between models, we performed one-way ANOVA of a three parameter model [@harrisonPhotosynthesisirradianceRelationshipsPolar1986] from pooled data and data fit across different photoperiods (8, 12, 16, or 24) or data fit across different peak PAR (30, 90, 180, 300, 600 together with 900) from chlorophyll specific exponential growth rate vs. cumulative diel PUR dose or vs. PSII electron flux (JV~PSII~; e^−^cell^−1^d^−1^), for two PhycoCyanin(PC)-rich cultures (056, 077) and two PhycoErythrin(PE)-rich cultures (048, 127) of *Synechococcus* sp. originating from the Baltic Sea, grown at 30, 90, 180, 300, 600, or 900 peak PAR µmol photons m^−2^s^−1^; and photoperiods of 8, 12, 16, or 24 h (Table S4-S5 in Supplemental material). One-way ANOVA was also used to examine statistical differences between single phase exponential decay fit model of pooled data across different strains for a given phase of growth and across different phase of growth for a given strain from PUR/PAR ratio (Table Sxxx), Phycobiliprotein to Chl *a* ratio (Table Sxxx), and effective absorption cross section of PSII ($\sigma$~PSII~'; nm^2^ quanta^−1^) measured under diel peak PAR growth light under Ex~590nm~ (orange) excitation in relation to the cumulative diel PAR dose (µmol photons m^−2^d^−1^) (Table S7, S9, S13 in Supplemental material).

T-test of linear fit model of pooled data across different strains for a given phase of growth and across different phase of growth for a given strain from effective absorption cross section of PSII ($\sigma$~PSII~'; nm^2^ quanta^−1^) measured under diel peak PAR growth light under Ex~445nm~ (blue) excitation in relation to the cumulative diel PAR dose (µmol photons m^−2^d^−1^) or in relation to the Phycobiliprotein to Chl *a* ratio, as well as from effective absorption cross section of PSII ($\sigma$~PSII~' or $\sigma$~PSII~; nm^2^ quanta^−1^) measured under Ex~590nm~ (orange) excitation in relation to the Phycobiliprotein to Chl *a* ratio was performed (Table S11, S15, S17 in Supplemental material).

Statistical differences for all analyzes were determined at the level of significance $\alpha$ = 0.05. Manuscript was prepared as a Rmarkdown document [@handelAndreasHandelCustom2020]. Figures were plotted using “ggplot” [@wickhamDataAnalysis2016] R package.

# Results {.unnumbered}

## Changes in chlorophyll specific exponential growth rate {.unnumbered}

In this study, the chlorophyll specific exponential growth rates (μ; d^−1^) vs. cumulative diel photon dose (µmol photons m^−2^d^−1^) for two PhycoCyanin(PC)-rich cultures (056, 077) and two PhycoErythrin(PE)-rich cultures (048, 127) of *Synechococcus* sp. originating from the Baltic Sea were determined. Growth rates were estimated from logistic fits of chlorophyll proxy OD~680~ - OD~720~ vs. elapsed time for picocyanobacteria cultures grown at 30, 90, 180, 300, 600 or 900 peak PAR µmol photons m^−2^s^−1^ (µE); and photoperiods of 8, 12, 16, or 24 h (Fig. <a href="#fig:GrowthRatePhotoperiod"><strong>??</strong></a>). 

Analyzed phenotypes of *Synechococcus* sp. showed varying chlorophyll specific exponential growth rates (μ) under different photoperiod and light conditions. Three-way factorial ANOVA showed that individual factor (irradiance, photoperiod, and strain) and their interactions significantly affected the μ, estimated from logistic fits of chlorophyll proxy OD~680~ - OD~720~ vs. elapsed time (ANOVA, *p* < 0.05 for all; Table S3). All tested strains were able to grow even under peak PAR 900 µmol photons m^−2^s^−1^ and 24 h photoperiod, except PE-rich_048. The highest growth rate was recorded for *Synechococcus* sp. PE-rich_127 (μ = 4.5 d^−1^) and PC-rich_056 (μ = 3.4 d^−1^) at the 180 µmol photons m^−2^s^−1^ and photoperiod of 24 h.  

We also found that cumulative diel photon dose consistently explains achieved μ across a matrix of photoperiods and peak PAR. Every strain showed distinct growth responses to cumulative diel photon dose, depending upon photoperiod. One-way ANOVA of a three parameter model [@harrisonPhotosynthesisirradianceRelationshipsPolar1986] from μ for two PC-rich and two PE-rich cultures of *Synechococcus* sp. showed significant difference between model performed from pooled data and data fit across all tested photoperiods (8, 12, 16, or 24 h; ANOVA, *p* < 0.05, Table S4 in Supplemental material). Strains also showed distinct growth responses to cumulative diel photon dose, depending upon peak PAR. In supplemental data (Fig. S5), strains generally showed peak-PAR specific responses to cumulative diel photon dose, that differ from a single light response model fit to the pooled data from a strain. Exceptions were observed in the strains PC-rich_077 and PE-rich_048 with the peak PAR of 600 or 900 µmol photons m^−2^s^−1^, which were not significantly different from the pooled data model (Table S5 in Supplemental material). A caveat to these findings is that cumulative diel photon dose is a product of photoperiod and PAR, so the highest levels of cumulative photon dose are only achieved under the 600 or 900 µmol photons m^−2^s^−1^.

Growth rate saturated under increasing cumulative diel PAR for all strains however, the achieved estimates of µ~max~ varied depending upon photoperiod and peak diel PAR. Growth rates vs. cumulative diel PUR relationships, estimated for exponential phase cultures, followed similar patterns (Fig. S6 and Table Sxxx in Supplemental material).

![<span id="fig:GrowthRatePhotoperiodPUR"></span>Figure 4: **Chlorophyll specific exponential growth rates (d^−1^) vs. cumulative diel Photosynthetically Usable Radiation (PUR, µmol photons m^−2^d^−1^).** Growth rates (+/- SE falling within symbols) were estimated from logistic fits of chlorophyll proxy OD~680~ - OD~720~ vs. elapsed time (Fig. 1, S4), for two PhycoCyanin(PC)-rich cultures (056, 077) and two PhycoErythrin(PE)-rich cultures (048, 127) of *Synechococcus* sp. originating from the Baltic Sea. Cultures were grown at 30 (dark gray), 90 (light gray), 180 (purple), 300 (red), 600 (orange), or 900 (yellow) peak PAR µmol photons m^−2^s^−1^ (µE); and photoperiods of 8 (square), 12 (circle), 16 (triangle), or 24 (diamond) h. Solid blue line shows a fit of the pooled growth rates for each strain, with a three parameter model [@harrisonPhotosynthesisirradianceRelationshipsPolar1986]. We also fit the same model separately for 8 (dotted line), 12 (long dash line), 16 (dashed line), or 24 (two dash line) h photoperiods, since for all strains they were each significantly different (ANOVA, *p* < 0.05) from the fit of pooled data.](../Output/Figures/Fig_GrowthRate_Photoperiod_PUR.png)


## Decreasing PUR/PAR ratio and Phycobiliprotein to Chl *a* ratio with increasing cumulative diel PAR dose {.unnumbered}

Changes of PUR/PAR ratio vs. cumulative diel PAR dose (µmol photons m^−2^d^−1^) for two PC-rich cultures (056, 077) and two PE-rich (048, 127) cultures of *Synechococcus* sp. grown at 30, 90, 180, 300, 600, or 900 peak PAR µmol photons m^−2^s^−1^ (µE); and photoperiods of 8, 12, 16, or 24 h were estimated (Fig. <a href="#fig:PURPARRatio">5</a>). Three-way factorial ANOVA showed that individual factor (cumulative diel photon dose, phase of growth, or strain) but not the interactions of these 3 factors, affected the PUR/PAR ratio (ANOVA, *p* < 0.05, Table S6). 

Strains also showed consistent patterns of light capture efficacy (PUR/PAR ratio) across cumulative diel photon doses. The ratio of PUR/PAR decayed exponentially in relation to cumulative photon dose, across different combinations of photoperiod and peak PAR. Although all strains followed a similar trend, the single phase exponential decay fit models varied significantly among strains during their exponential phase of growth (ANOVA, *p* < 0.05, Table S7). The exception was the fit of the models PE-rich_048 and PE-rich_127 (ANOVA, *p* > 0.05). During pre-stationary phase this response dampens and even disappears (ANOVA, *p* > 0.05, Table S7). Significant differences between the fit models for different phases of growth within all given strains with the exception of PC-rich_056 were also noted (ANOVA; *p* < 0.05, Table S7). Moreover, the PUR/PAR ratio was significantly higher in the PE-rich strains under low cumulative diel photon dose during their exponential phase of growth; however, decay towards a plateau close to the PC-rich strains as cumulative diel photon dose increases.


![<span id="fig:PURPARRatio"></span>Figure 5: **Changes of PUR/PAR ratio vs. cumulative diel PAR photon dose (µmol photons m^−2^d^−1^).** PUR/PAR ratio was estimated for two PhycoCyanin(PC)-rich cultures (056, 077) and two PhycoErythrin(PE)-rich cultures (048, 127) of *Synechococcus* sp. originating from the Baltic Sea. Cultures were grown at 30 (dark gray), 90 (light gray), 180 (purple), 300 (red), 600 (orange), or 900 (yellow) peak PAR µmol photons m^−2^s^−1^ (µE); and photoperiods of 8 (square), 12 (circle), 16 (triangle), or 24 (diamond) h. Figure presents data (smaller symbols) and means (bigger symbols) from exponential or  pre-stationary phase of growth. Blue solid line shows single phase exponential decay fit for data from each strain and growth phase, with fit parameters presented. Different lowercase letters indicate statistically significant differences between the fit models for different strains within a given phase of growth. Different uppercase letters indicate statistically significant differences between the fit models for different phases of growth within a given strain (ANOVA; *p* < 0.05).](../Output/Figures/Fig_PURPARRatio.png)

![<span id="fig:PhycoChlaRatio"></span>Figure 6: **Changes of total Phyco/Chl *a* ratio vs. cumulative diel photon dose (µmol photons m^−2^d^−1^).** Total Phyco/Chl *a* ratio was estimated for two PhycoCyanin(PC)-rich cultures (056, 077) and two PhycoErythrin(PE)-rich cultures (048, 127) of *Synechococcus* sp. originating from the Baltic Sea. Cultures were grown at 30 (dark gray), 90 (light gray), 180 (purple), 300 (red), 600 (orange), or 900 (yellow) peak PAR µmol photons m^−2^s^−1^ (µE); and photoperiods of 8 (square), 12 (circle), 16 (triangle), or 24 (diamond) h. Figure presents data (smaller symbols) and means (bigger symbols) from exponential or pre-stationary phase of growth. Blue solid line shows single phase exponential decay fit for data from each strain and growth phase, fit parameters are presented. Different lowercase letters indicate statistically significant differences between the fit models for different strains within a given phase of growth. Different uppercase letters indicate statistically significant differences between the fit models for different phases of growth within a given strain (ANOVA; *p* < 0.05).](../Output/Figures/Fig_PhycoChlaRatio.png)

## Decreasing effective absorption cross section of PSII with increasing cumulative diel PAR dose {.unnumbered}

In this work, we estimated the effective absorption cross section of PSII ($\sigma$~PSII~'; nm^2^ quanta^−1^) measured under diel peak PAR growth light vs. cumulative diel photon dose (µmol photons m^−2^d^−1^). $\sigma$~PSII~' was estimated using FRRf induction curves using Ex~590nm~ (orange) excitation, for two PC-rich (056, 077) and two PE-rich (048, 127) cultures of *Synechococcus* sp. grown at 30, 90, 180, 300, 600, or 900 peak PAR µmol photons m^−2^s^−1^ (µE); and photoperiods of 8, 12, 16, or 24 h (Fig. <a href="#fig:Sigma590">7</a>). The $\sigma$~PSII~' measured under diel peak PAR growth light under Ex~445nm~ (blue) excitation vs. cumulative diel photon dose was shown in Supplementary material (Fig. S10, Table S10-S11).

Similarly to the PUR/PAR ratio, three-way factorial ANOVA showed that individual factor (cumulative diel photon dose, phase of growth, or strain) and their interactions, significantly affected the $\sigma$~PSII~' measured under diel peak PAR growth light under Ex~590nm~ excitation (ANOVA, *p* < 0.05; Table S12 in Supplemental material).

All strains showed consistent patterns of effective absorption cross section for PSII photochemistry across cumulative diel photon doses. The $\sigma$~PSII~' examined a consistent, sharp exponential decay in relation to cumulative photon dose, across different combinations of photoperiod and peak PAR. Although all strains showed this response pattern, the exponential decay fit models differ significantly among two PC-rich strains and PE-rich_048 during their exponential phase of growth (ANOVA, *p* < 0.05; Table S13 in Supplemental material). During pre-stationary phase this response dampens but persists. Additionally, the significant differences between the fit models for different phases of growth within all given strains, with the exception of PE-rich_048, were also presented (ANOVA; *p* < 0.05, Table S13).

The PE-rich strains showed higher $\sigma$~PSII~' under low cumulative diel photon dose, and remain higher than the PC-rich strains even as cumulative diel photon dose increases.

![<span id="fig:Sigma590"></span>Figure 7: **Effective absorption cross section of PSII** (σ~PSII~'; nm^2^ quanta^−1^) **measured under diel peak PAR growth light vs. cumulative diel PAR photon dose (µmol photons m^−2^d^−1^).** Effective absorption cross section of PSII (σ~PSII~'; nm^2^ quanta^−1^) was estimated using FRRf induction curves with excitation of phycobilisomes (Ex~590nm~, orange), for two PhycoCyanin(PC)-rich cultures (056, 077) and two PhycoErythrin(PE)-rich cultures (048, 127) of *Synechococcus* sp. originating from the Baltic Sea. Cultures were grown at 30 (dark gray), 90 (light gray), 180 (purple), 300 (red), 600 (orange), or 900 (yellow) peak PAR µmol photons m^−2^s^−1^ (µE); and photoperiods of 8 (square), 12 (circle), 16 (triangle), or 24 (diamond) h. Figure presents data (smaller symbols) and means (bigger symbols) from exponential or pre-stationary phase of growth. Blue solid line shows single phase exponential decay fit for data from each strain and growth phase. Different lowercase letters indicate statistically significant differences between the fit models for different strains within a given phase of growth. Different uppercase letters indicate statistically significant differences between the fit models for different phases of growth within a given strain (ANOVA; *p* < 0.05).](../Output/Figures/Fig_Sigma590.png)


Changes of effective absorption cross section of PSII ($\sigma$~PSII~'; nm^2^ quanta^−1^) measured under diel peak PAR growth light under Ex~590nm~ (orange) excitation vs. total Phyco/Chl *a* ratio, for PC-rich_056, PC-rich_077, PE-rich_048, and PE-rich_127 cultures of *Synechococcus* sp. grown at 30, 90, 180, 300, 600, or 900 peak PAR µmol photons m^−2^s^−1^ (µE); and photoperiods of 8, 12, 16, or 24 h were demonstrated (Fig. <a href="#fig:SigmaPig590">8</a>). Changes of effective absorption cross section of PSII ($\sigma$~PSII~; nm^2^ quanta^−1^) measured at the dark period under Ex~590nm~ (orange) excitation vs. total Phyco/Chl *a* ratio were shown in Supplementary material (Fig. S9, Table Sxxx). Also, the $\sigma$~PSII~' measured under diel peak PAR growth light under Ex~445nm~ (blue) excitation vs. total Phyco/Chl *a* ratio was shown in Fig. S11 and Table S14-S15.

In this work we found that $\sigma$~PSII~' showed a consistent relation to phycobilisome:chlorophyll ratio. Three-way factorial ANOVA showed that individual factor (cumulative diel photon dose, phase of growth, or strain) and their interactions, significantly affected the $\sigma$~PSII~' measured under diel peak PAR growth light under Ex~590nm~ excitation relation to the total Phyco/Chl *a* ratio (ANOVA, *p* < 0.05; Table S16 in Supplemental material). 

The $\sigma$~PSII~' excited through chlorophyll absorbance at Ex~445nm~ was consistently small across strains and growth conditions, since in cyanobacteria the number of chlorophyll serving PSII is nearly fixed (CITATIONS DOUG, Fig. S11). For $\sigma$~PSII~' excited through phycobilisome absorbance at Ex~590nm~, strains show consistent positive correlation with total Phyco/Chl *a* ratio. 
Strains in exponential growth show significant scatter around this positive relation, likely related to regulatory control of $\sigma$~PSII~', beyond pigment composition. Under pre-stationary phase the relationship between $\sigma$~PSII~' and total Phyco/Chl *a* ratio was more consistent, suggesting an increase in reliance upon compositional regulation to control light delivery to PSII, as opposed to shorter-term regulation.

The linear fits also vary significantly among strains. The linear fit models differ significantly among PC-rich_077 and two PE-rich strains during their exponential phase of growth. During pre-stationary phase we noted significant differences between two PC-rich strains and PE-rich_048. Moreover, the significant differences between the fit models for different phases of growth were noted for PC-rich strains 056 and 077 (t-test; *p* < 0.05, Table S17). 

![<span id="fig:SigmaPig590"></span>Figure 8: **Changes of effective absorption cross section of PSII** (σ~PSII~'; nm^2^ quanta^−1^) **measured under diel peak PAR growth light with excitation of phycobilisomes (Ex~590nm~, orange) vs. the ratio of sum of µg phycobilins (PE, PC, APC protein, total Phyco)/µg Chl *a*;** for two PhycoCyanin(PC)-rich cultures (056, 077) and two PhycoErythrin(PE)-rich cultures (048, 127) of *Synechococcus* sp. originating from the Baltic Sea. Cultures were grown at 30 (dark gray), 90 (light gray), 180 (purple), 300 (red), 600 (orange), or 900 (yellow) peak PAR µmol photons m^−2^s^−1^ (µE); and photoperiods of 8 (square), 12 (circle), 16 (triangle), or 24 (diamond) h. Figure presents data (smaller symbols) and means (bigger symbols) from exponential or pre-stationary phase of growth. Blue solid line shows linear model fit for data from each strain and growth phase. Different lowercase letters indicate statistically significant differences between the fit models for different strains within a given phase of growth. Different uppercase letters indicate statistically significant differences between the fit models for different phases of growth within a given strain (t-test; *p* < 0.05).](../Output/Figures/Fig_SigmaPig590.png)

## Changes in PSII flux {.unnumbered}

![<span id="fig:GrowthRateJVPSII"></span>Figure 9: **Chlorophyll specific exponential growth rates (d^−1^) vs. PSII flux (*JV*~PSII~; e^−^cell^−1^d^−1^) measured under diel peak PAR growth light.** Growth rates (+/- SE falling within symbols) were estimated from logistic fits of chlorophyll proxy OD~680~ - OD~720~ vs. elapsed time (Fig. S4). PSII flux (*JV*~PSII~; e^−^cell^−1^d^−1^) was estimated using FRRf induction curves with excitation of chlorophyll (Ex~445nm~, blue), for two PhycoCyanin(PC)-rich cultures (056, 077) and two PhycoErythrin(PE)-rich cultures (048, 127) of *Synechococcus* sp. originating from the Baltic Sea. Cultures were grown at 30 (dark gray), 90 (light gray), 180 (purple), 300 (red), 600 (orange), or 900 (yellow) peak PAR µmol photons m^−2^s^−1^ (µE); and photoperiods of 8 (square), 12 (circle), 16 (triangle), or 24 (diamond) h. Solid blue line shows a fit of the pooled growth rates for each strain, with a three parameter model [@harrisonPhotosynthesisirradianceRelationshipsPolar1986]. We also fit the same model separately for 8 (dotted line), 12 (long dash line), 16 (dashed line), or 24 (two dash line) h photoperiods, only when they were significantly different (ANOVA, *p* < 0.05) from the fit of pooled data.](../Output/Figures/Fig_GrowthRate_JVPSII_Photoperiod.png)

# Discussion {.unnumbered}

## Photic regime significance for picocyanobacteria growth {.unnumbered}

### Photoperiod length {.unnumbered}

Changes in photoperiod trigger adaptive responses, shaping the temporal dynamics and community structure of phytoplankton [@huismanHowSinkingPhytoplankton2002; @alberteFunctionalOrganisationPhotosynthetic1980; @larochePelagicLightDependentMicrobiome2022]. 
This work revealed that not only the daily dose of light, but also the length of exposure affected the picocyanobacteria growth rate. The PE-rich and PC-rich strains of *Synechococcus* sp. showed faster chlorophyll specific exponential growth rates with increasing photoperiod, including constant light conditions. This is particularly important in regions with a longer photoperiod but relatively low irradiances, for example, in the Arctic and Antarctic regions, where PC-strains may become dominant species in the surface waters.

xxx - paper about existence pico in arctic. Maybe different regions? 

Here, we confirmed that *Synechococcus* sp. can exist and even become the dominant faction of phytoplankton in all geographic zones on Earth as long as they have access to light. In regions with a longer photoperiod (summer in the temperate zone and summer at the poles), PC-strains may become dominant species in the surface waters whereas some of PC-strains of *Synechococcus* sp. may be less numerous than PE-strains in surface waters (where the light intensity could be extremely high) when the photoperiod is quite low (autumn and winter in temperate zones and tropical water throughout the year). Our research has also highlighted the possibility of occurrence of both PE-rich and PC-rich Synechococcus sp. in conditions of continuous irradiation. Thus, it can be predicted that *Synechococcus* may become the dominant fraction of phytoplankton during the Arctic summer near the poles regions regardless of their genetic lineages and pigments composition.


### Photosynthetically Active Radiation (PAR) {.unnumbered}

Numerous studies have highlighted the significance of PAR and light intensity as a key driver of phytoplankton productivity and its influence on ecosystem dynamics, biogeochemical cycling, and food web interactions [e.g., @kirkLightPhotosynthesisAquatic1983; @fieldPrimaryProductionBiosphere1998; @torremorellAnnualPatternsPhytoplankton2009; @churilovaPhytoplanktonBloomPhotosynthetically2020]. 

*Synechococcus* sp., a widely studied picocyanobacterial genus, exhibits remarkable adaptability to different light intensities, particularly under white light conditions. White light encompasses the entire visible spectrum, and *Synechococcus* sp. has developed various strategies to optimize its photosynthetic efficiency across a range of light intensities. Under high-light conditions, *Synechococcus* employs photoprotective mechanisms to prevent the harmful effects of excess light energy. These include the dissipation of excess energy as heat via non-photochemical quenching (NPQ) and the regulation of antenna pigments, such as phycobilisomes, to balance light absorption and energy transfer. In contrast, under low-light conditions, *Synechococcus* sp. increases the expression of light-harvesting complexes to enhance light absorption and capture [@chenGenomicTranscriptomicEvidence2022; @dufresneUnravelingGenomicMosaic2008; @mella-floresProchlorococcusSynechococcusHave2012]. 

In this study, chlorophyll specific exponential growth rates of the PE-rich and PC-rich *Synechococcus* sp. strains increased at the light levels, although some strains suffered photoinhibition. The *Synechococcus* sp. strains reached a plateau in the light intensity range of 180-300 µmol photons m^−2^s^−1^. Growth at 900 µmol photons m^−2^s^−1^ was also noted but not as efficient as under moderate light. Even though PE-rich *Synechococcus* sp. are more adapted to lower-light conditions and remain deeper in the water column, our findings prove that several strains may survive under high-irradiance conditions, implying much wider tolerance range that reported in the literature [citationxxx] that needs to be accounted for while developing large-scale phytoplankton models.



Our research shows that an increase in light intensity can result in the dominance of both PE-rich and PC-rich picocyanobacteria in aquatic ecosystems and confirmed the possibility of occurrence of *Synechococcus* sp. in extremely high irradiance conditions.


### Photosynthetically Usable Radiation (PUR) {.unnumbered}

PUR is always smaller than PAR (PUR < PAR) and depends on the spectral composition of the submarine radiant energy available to algae and their pigment composition determining the spectral absorption properties [@morelAvailableUsableStored1978]. 

PUR plays a fundamental role in the growth and productivity of phytoplankton within aquatic ecosystems [@behrenfeldClimatedrivenTrendsContemporary2006; @falkowskiGlobalCarbonCycle2000; @morelOpticalModelingUpper1988]. Phytoplankton, as primary producers, heavily rely on PUR for their energy acquisition through photosynthesis. The availability of PUR directly influences the photosynthetic rates and overall metabolic activity of phytoplankton. High levels of PUR promote optimal photosynthetic efficiency, leading to enhanced growth, reproduction, and biomass accumulation. Conversely, insufficient or suboptimal PUR availability can limit the metabolic processes and growth of phytoplankton. 

The spatial and temporal distribution of PUR within aquatic ecosystems is influenced by various factors, including solar zenith angle, water depth, water clarity, and the presence of light-absorbing substances such as dissolved organic matter [@morelAvailableUsableStored1978; @morelOpticalModelingUpper1988]. 


Understanding the dynamics and availability of PUR is crucial for comprehending the variability of picocyanobacteria communities in different aquatic environments. 



## Photic regime and and growth phases significance for picocyanobacteria light-capture {.unnumbered}

### PUR/PAR ratio {.unnumbered}

As we face ongoing environmental changes, including alterations in light regimes due to climate change and human activities, assessing the impact of changing PUR on picocyanobacteria communities becomes increasingly important for predicting and managing the response of aquatic ecosystems.

In this study, the PE-rich strains always had a higher PUR/PAR ratio than the PC-rich strains. The PUR/PAR ratio decreased with increasing light in the PE-rich strains, while it initially increased under low light and short photoperiod in the PC-rich strains. Our results indicate that PE-rich strains of *Synechococcus* sp., due to their high content of phycoerythrin, can better use the available radiation. Therefore, their long-term dominance in the environment can be postulated, especially in places where access to light is limited.

### Pigments content {.unnumbered}

Temporal variations in cell-specific pigment content of *Synechococcus* sp. were observed during the growth phase, characterized by an initial increase followed by a sharp decrease. These trends exhibited dependency on growth, light intensity, and photoperiod, manifesting subsequent to the attainment of daily maximum absolute growth. Maximum pigment content was documented under conditions of low irradiance and extended photoperiod. Moreover, PC-rich strains had more pigments in the cell compared to PE-rich strains of *Synechococcus* sp.

Pigment dynamics are profoundly influenced by the prevailing light regimes. Primary photosynthetic pigments in *Synechococcus* sp. comprise chlorophyll *a*, responsible for light energy capture. Under low-light conditions, picocyanobacteria tend to increase their chlorophyll *a* content to enhance light absorption and maximize energy capture for photosynthesis. Conversely, high-light conditions often lead to a decrease in chlorophyll *a* content, serving as a photoprotective mechanism against excessive irradiation. In addition to chlorophyll *a*, picocyanobacteria utilize phycobilins, including phycocyanin and phycoerythrin, as accessory pigments to enhance light harvesting efficiency. Adapting to low-light environments, picocyanobacteria enhance phycobilin production to compensate for limited irradiance, thereby optimizing their photosynthetic capabilities. The chlorophyll/phycobilin ratio serves as a valuable indicator of the prevailing light conditions and the balance between chlorophyll-based and phycobilin-based light harvesting strategies. Elevated light intensities result in a decreased chlorophyll/phycobilin ratio as picocyanobacteria allocate resources towards efficient phycobilin-mediated light capture. These intricate changes in pigment composition and ratios represent vital adaptations that enable picocyanobacteria to optimize photosynthetic efficiency and thrive in dynamic light environments [@chakdarCyanobacterialPhycobilinsProduction2016; @stadnichukCyanobacterialPhycobilisomesPhycobiliproteins2015; @bealeBiosynthesisCyanobacterialTetrapyrrole1994].

### Effective absorption cross section of PSII and PSII flux per unit volume {.unnumbered}

# Conclusion {.unnumbered}

Understanding the influence of light intensity and photoperiod on the dynamics of picocyanobacteria is imperative for predicting their spatial distribution across various geographic regions and their response to observed environmental changes. Our findings have substantiated that *Synechococcus* sp., irrespective of its genetic lineages and pigment composition, can thrive and even dominate the phytoplankton community worldwide when exposed to sufficient light. Furthermore, our investigations have demonstrated the survival capacity of both PE-rich and PC-rich *Synechococcus* sp. strains under conditions of exceptionally high and continuous irradiation. Consequently, it can be predicted that *Synechococcus* sp. has the potential to emerge as the prevailing phytoplankton component during the Arctic summer near polar regions. Nevertheless, our results showed the PE-rich strains are stronger light-harvesting competitors as they tend to live deeper in the water column, but the PC-rich strains may have lower N-quotients for their light capture system. Additionally, we anticipate that PC-rich strains of *Synechococcus* sp. could be less abundant than PE-rich strains in surface waters, where light intensity tends to be extremely high, especially during periods of reduced photoperiod, such as autumn and winter in temperate zones and throughout the year in tropical waters. Conversely, in regions characterized by an extended photoperiod i.e., summer in the temperate zone and summer at the poles, PC-rich strains may assume dominance in surface waters. These differences may help explain differential seasonal prevalences of *Synechococcus* sp., in terms of the costs of exploitation of different photic regimes.

# Acknowledgements {.unnumbered}

We would like to thank Carlie Barnhill (Mount Allison Student) who assisted with code for import of Multi-Cultivator growth data files.

# Funding sources {.unnumbered}

Canada Research Chair in Phytoplankton Ecophysiology (DAC)

Latitude & Light; NSERC of Canada Discovery Grant (DAC)

# Data sources {.unnumbered}

Data sources chapter provide links to any data used from external providers:

URL for MetaDataCatalog: https://docs.google.com/spreadsheets/d/1ZXpwR7Gfto-uRzVdXzMpQF4frbrvMLH_IyLqonFZRSw/edit#gid=0

URL for tMaxAHG Catalog: https://docs.google.com/spreadsheets/d/1ksY7xlg9wOsICOBRmZkHPKdd9KOislNwPDzyuJ3UIUI/edit#gid=0

URL for pigments Catalog (correlation): https://docs.google.com/spreadsheets/d/1EvogE5pFlGT9H304E3dqXKwh26dWI9r_snSPhZCHWiU/edit#gid=0

URL for ClarioStar Growth Catalog (correlation): https://docs.google.com/spreadsheets/d/1cfyxO1bFSeEMlMnx1vAyuskk3Un_bqkE9-uUSc-jwhE/edit#gid=0


------------------------------------------------------------------------------------------------------------
Research Question:
Does cumulative diel photon dose consistently explain achieved growth rates across a matrix of photoperiods and peak PAR?

Test:  Do strains show distinct growth responses to cumulative diel photon dose, depending upon photoperiod?
  Yes.  Every strain shows photoperiod-specific responses to cumulative diel photon dose that differ from a single light response model fit to the pooled data from a strain.
  

Test:  Do strains show distinct growth responses to cumulative diel photon dose, depending upon peak PAR?
  Yes.  In supplmental data, strains generally show peak-PAR specific responses to cumulative diel photon dose, that differ from a single light response model fit to the pooled data from a strain. Exceptions are that for strains 77 and 48 peak PAR of 600 or 900 µmol photons m^−2^d^−1^ are not significantly different from the pooled data model.  A caveat to this findings is that cumulative diel photon dose is, of course, a product of photoperiod and PAR, so the highest levels of cumulative photon dose are only achieved under the 600 or 900 µmol photons m^−2^d^−1^.
  
All four strains show saturation of growth rate under increasing cumulative diel PAR, but the achieved estimates of µ~max~ vary depending upon photoperiod and peak diel PAR.  Plots of growth rates vs. cumulative diel PUR, estimated for exponential phase cultures, show similar patterns (Supplemental).
-------------------------------------------------------------------------------
Research Question:
Do strains show consistent patterns of light capture efficacy (PUR/PAR ratio) across cumulative diel photon doses?

Yes.
The ratio of PUR/PAR shows a consistent exponential decay in relation to cumulative photon dose, across different combinations of photoperiod and peak PAR.
Although all strains shows this response pattern, the exponential decay model parameters differ significantly among strains.
During pre-stationary phase this response dampens and even disappears. 
The PE-rich strains show a much higher PUR/PAR ratio under low cumulative diel photon dose, but decay towards a plateau close to the PC-rich strains as cumulative diel photon dose increases.
-----------------------------------------------------------------------------------------------------

Research Question:
Do strains show consistent patterns of effective absorption cross section for PSII photochemistry across cumulative diel photon doses?

Yes.
The \u03C3~PSII~' shows a consistent, sharp exponential decay in relation to cumulative photon dose, across different combinations of photoperiod and peak PAR.
Although all strains shows this response pattern, the exponential decay model parameters differ significantly among strains.
During pre-stationary phase this response dampens but persists. 
The PE-rich strains show a much higher \u03C3~PSII~' under low cumulative diel photon dose, and remain higher than the PC-rich strains even as cumulative diel photon dose increases.
------------------------------------------------------------------------------------------------------

Research Question:
Does \u03C3~PSII~' show a consistent relation to phycobilisome:chlorophyll ratio?
The \u03C3~PSII~' excited through chlorophyll absorbance at 445 nm was consistently small across strains and growth conditions, since in cyanobacteria the number of chlorophyll serving PSII is nearly fixed (CITATIONS DOUG). For \u03C3~PSII~' excited through phycobilisome absorbance at 590 nm, strains show consistent positive correlation with phycobilin:chlorophyll ratio.  Strains in exponential growth show significant scatter around this positive relation, likely related to regulatory control of \u03C3~PSII~', beyond pigment composition. Under pre-stationary phase the plots of \u03C3~PSII~' vs. phycobilin:chlorophyll show much less scatter, suggesting an increase in reliance upon compositional regulation to control light delivery to PSII, as opposed to shorter term regulation.

The linear fits also vary significantly among strains.
---------------------------------------------------------------------------------------------------

# References {.unnumbered}