---
title: "Ulva sp. as a hazardous material threatening the environment — A review"

author:
- Gracjana Budzałek:
    institute:
    - UG
    email: gbudzalek@gmail.com
- Kinga Wiśniewska:
    institute:
    - UW
    email: kinga.wisniewska@uwr.edu.pl
- Anna Dziubińska:
    institute:
    - UG
    email: anna.dziubinska@ug.edu.pl
- Sarah Postum:
    institute:
    - MTA
    email: spostuma@mta.ca
- Anna Woźniak:
    institute:
    - MU
    email: 
- Sylwia Śliwińska-Wilczewska:
    institute:
    - MTA
    - UG
    email: ssliwinskawilczews@mta.ca
    ORCID: ORCID 0000-0002-3147-6605
    correspondence: true
institute:
- UG: Institute of Oceanography, University of Gdansk, 46 Pilsudskiego St, P81-378, Gdynia, Poland
- MTA: Department of Biology, Mount Allison University, 53 York St., Sackville, NB, E4L 1C9, Canada
- UW: Department of Climatology and Atmosphere Protection, Faculty of Earth Sciences and Environmental Management, University of Wroclaw, Kosiby 8 St., 51–621 Wroclaw, Poland
- MU: Department of Nursing and Midwifery, Wroclaw Medical University, Bartla 5 St., 51–618 Wroclaw, Poland
output:
  bookdown::word_document2:
    reference_docx: Ulva_manuscript.docx
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
    - "--lua-filter=custom_filter.lua"
bibliography:
- BalticPhotoperiod.bib
- packages.bib
- faultycitations.bib
csl: "science-of-the-total-environment.csl"
---









<br>

# Abstract {.unnumbered}
<br>

*Ulva* sp. is a hazardous material widely distributed in oceans and estuaries worldwide, posing a significant environmental threat. Massive blooms, commonly referred to as Green Tides, have increased in frequency globally, driven by factors such as light availability, nutrient enrichment, rising sea surface temperatures, and salinity fluctuations. These blooms vary in location, species composition, ecological consequences, and underlying causes. Additionally, *Ulva* sp. produces bioactive compounds that inhibit growth and disrupt vital functions in various plant and animal species. This review summarizes current knowledge on *Ulva* sp., highlighting instances of harmful Green Tides over the past five decades, their detrimental effects on micro- and macroorganisms, and the hazardous compounds involved. Furthermore, we emphasize the need for interdisciplinary research to better understand the ecological risks associated with *Ulva* sp. and its potential implications for human health.

<br>

# Introduction {.unnumbered}

<br>

Aquatic green macroalgae Ulva is a genus that raises a lot of controversy. Ulva is a species that has recently been intensively promoted, especially in scientific journals focusing on the optimization and commercialization of new organisms for commercial purposes. Mass cultivation of Ulva sp. in outdoor open cultivation ponds of 1000 m2 can produce approximately 10 tons of dry biomass per year (Simon et al., 2022). Ulva sp. has gained recognition as a profitable food source, cosmetic product, or as an environmental bioremediation agent due to its ability to absorb large amounts of heavy metals and other hazardous pollutants (Mantri et al., 2020; Simon et al., 2022). 

However, despite its nutritional and commercial benefits, Ulva sp. poses environmental and potential health risks that merit caution and consideration. Unfortunately, the lack of sufficient knowledge about the ecophysiology of Ulva sp. and unified rules and methods for obtaining biomass may lead to numerous abuses. For instance, it is possible to use Ulva biomass from sewage treatment plants or dead thallus obtained after bloom event as a source of cosmetics or food products. It has now become a fact that algae-based food supplements may be harmful to human health due to the high content of heavy metals including cadmium (Cd), lead (Pb), or mercury (Hg) (Rzymski et al., 2015).

It is well-established that Ulva sp. produces a diverse array of harmful secondary metabolites. Nevertheless, the extent of their hazardous effects on the surrounding ecosystem remains uncertain. Given the ability of Ulva sp. to inhibit the growth of competing algal and plant species, as well as to cause the mortality of various animal taxa, including vertebrates, an important question arises whether Ulva sp. is actually a safe and beneficial organism, or rather a threat to the environment.

Here, we reviewed the general classification and morphological differences of the Ulva genus and the locations of occurrence and physiological features that help this green algae adapt to changing environmental conditions. Next, we summarized available reports on the locations of Ulva sp. blooms in aquatic ecosystems and their broad consequences. We also presented the most frequently used methods for testing the biological activity of Ulva sp. and their active compounds that affect the surrounding ecosystem. At the end, we compiled reports on the harmful effects of Ulva on viruses, bacteria, fungi, micro- and macroalgae, as well as invertebrates and vertebrates. This article highlights the need for interdisciplinary research aimed at shedding light on the basic mechanisms governing the occurrence and succession of green algae in coastal seas as well as drawing the attention of the public to the fact that Ulva sp. is an organism that poses a real threat to the functioning of the aquatic environment and causes financial damage in a global scale.

<br>

# Classification and morphology of *Ulva* sp. {.unnumbered}

<br>

The genus *Ulva* was first described by Carolus Linnaeus in Species Plantarum (Linnaeus, 1753). In modern classification, Ulva belongs to the phylum Chlorophyta, class Ulvophyceae (K.R. Mattox & K.D. Stewart), order Ulvales (Blackman & Tansley), and family Ulvaceae (J.V. Lamouroux ex Dumortier) (Guiry & Guiry, 2024). Phylogenetic studies have merged Ulva and Enteromorpha into a single genus (Hayden et al., 2003; Shimada et al., 2003), with 102 taxonomically accepted species worldwide (Guiry & Guiry, 2024). The most commonly occurring *Ulva* species are shown in Fig. <a href="#fig:Ulvamorphology">1</a>.

![<span id="fig:Ulvamorphology"></span>**Fig. **1: Morphology of common *Ulva* species: (A) *Ulva compressa*; (B) *Ulva fasciata*; (C) *Ulva flexuosa*; (D) *Ulva intestinalis*; (E) *Ulva lactuca*; (F) *Ulva linza*; (G) *Ulva lobata*; (H) *Ulva ohnoi*; (I) *Ulva prolifera*; (J), or *Ulva rigida*.](../Output/Figures/Ulvamorphology.png)


Historically, species identification relied on morphological and anatomical traits, including thallus shape and size, presence of dentation, thickness, cell structure, and number of pyrenoids. However, these characteristics can be highly variable due to factors such as age, reproductive state, grazing pressure, and environmental conditions (Guiry & Guiry, 2024). Consequently, molecular markers are increasingly used for taxonomic classification, leading to the discovery of new free-floating Ulva species associated with Green Tides (Kazi et al., 2016; Kang et al., 2021; Wan et al., 2017; Krupnik et al., 2018).

The mature Ulva sp. thallus consists of a flattened, distromatic blade, where two layers of independent but closely associated cells form the structure. Thallus morphology varies widely, ranging from broad, irregularly lobed blades to linear, lanceolate, or oblanceolate shapes. Some species, such as U. reticulata, have perforated blades, while others, like U. rigida, U. scandinavica, and U. taeniata, remain unperforated. The thallus can grow up to one meter under optimal conditions (Guiry & Guiry, 2024). Pigmentation varies from dark green to pale yellow, and vegetative cells contain a single chloroplast and one or more pyrenoids. Starch content, which serves as a reserve material, fluctuates between 1.59% and 21.44%, depending on growth conditions and seasonality (Kazir et al., 2021).

Morphological variation in Ulva sp. is influenced not only by physical and chemical environmental factors but also by microbial associations. Major bacterial groups such as Bacteroidetes and Planctomycetes colonize U. australis surfaces (Tujula, 2006), and similar bacterial communities have been found in Ulva sp. from different habitats (Goecke et al., 2010). The interaction between Ulva sp. and bacteria is crucial for normal morphological development. In axenic culture, Ulva sp. loses its typical form, but co-cultivation with bacterial isolates restores its normal structure (Provasoli & Pintner, 1980). Spoerner et al. (2012) demonstrated that regulatory compounds secreted by Cytophaga MS6 (with auxin-like activity) and Roseobacter MS2 (with cytokinin-like activity) influence the growth and morphogenesis of U. mutabilis.

<br>

# Occurrence and physiology of *Ulva* sp. {.unnumbered}

<br>

Ulva sp. is a cosmopolitan genus found in oceans and estuaries worldwide (Guiry & Guiry, 2024). Its successful colonization across diverse environments is attributed to physiological, biochemical, and molecular adaptations. Ulva sp. is distributed across all seven continents, including Antarctica. Asia records the highest species diversity with 56 species, followed by Australia (40 species), Europe (38 species), North America (34 species), Africa (31 species), South America (20 species), and Antarctica (12 species) (Mantri et al., 2020).

The broad distribution of Ulva sp. is due to its remarkable tolerance and adaptation to key environmental factors such as light, temperature, and salinity. It can thrive in both freshwater and marine habitats. Marine species typically inhabit coastal zones to depths of 40 meters (Chapman, 1956), while freshwater species have been documented in central Europe (e.g., Ulva flexuosa; Rybak, 2015) and on Japan's Ryukyu Islands (Ulva limnetica; Ichihara et al., 2009). Additionally, species like Ulva lactuca, Ulva rigida, Ulva compressa, and Ulva pertusa can tolerate salinity gradients ranging from less than 0.5 to 49 PSU (Hofmann et al., 2010). Seasonal growth patterns show increased abundance during spring and summer, as warmer temperatures enhance growth and reproduction (Caniguan et al., 2025; Uchimura et al., 2004). For instance, the optimal temperature for spore/gamete release and growth in U. prolifera is 20–27°C (Wang et al., 2007), with blooms typically occurring at 23–26°C (Li et al., 2018). Moreover, Ulva sp. exhibits a linear growth response to light intensity up to 30 μmol photons m−2s−1, reaching saturation above 70 μmol photons m−2s−1 (Fortes & Lüning, 1980). Its opportunistic nature—marked by rapid nutrient uptake and fast growth rates—can lead to explosive increases in biomass (Melton et al., 2016; Hu et al., 2017). Wu et al. (2022) noted that the formation of air sacs in Ulva is influenced by adaptive changes in temperature and light, while settlement in U. prolifera is triggered by temperatures exceeding the optimal range.
Ulva sp. reproduces both sexually and asexually. Its sexual cycle is characterized by an isomorphic alternation of generations, with morphologically similar but genetically distinct sporophyte and gametophyte phases. In addition, Ulva sp. can reproduce asexually through biflagellate zoospores and by parthenocarpy, enhancing its reproductive versatility (Mantri et al., 2020). The haploid thallus typically contains between 5 and 13 chromosomes (Guiry & Guiry, 2024).
Adaptation of the light-harvesting pigments is another key physiological feature. Ulva sp. contains chlorophyll a along with accessory pigments such as chlorophyll b and carotenoids (see Fig. 2). Recent analyses of absorption spectra and chromatographic retention times have confirmed the presence of carotenoids including lutein, β-carotene, neoxanthin, β-cryptoxanthin, violaxanthin, antheraxanthin, and zeaxanthin, although total pigment yield varies with species (Eismann et al., 2020).

<br>

![<span id="fig:SpectraUlva"></span>**Fig. **2: Whole-cell absorbance spectra of (A) *Ulva ohnoi*; (B) *Ulva fasciata*; (C) *Ulva lactuca*, together with emission spectra of the white LED lamp (yellow area), normalized to emission at 440 nm, and PUR (green area). Peaks characteristic of known pigments are labeled: Chl *a*, chlorophyll *a*; Chl *b*, chlorophyll *b*; Car, carotenoids.](../Output/Figures/SpectraUlva.png)

<br>

# Prevalence and consequences of *Ulva* sp. blooms {.unnumbered}

<br>

Ulva sp. is notorious for its rapid and uncontrolled proliferation, leading to phenomena known as Green Tides. Although these blooms share common traits, they vary widely in location, causative organisms, triggers, and impacts. Green Tides affect diverse sites and impose significant economic and environmental burdens, drawing attention from both scientists and policymakers (Ye et al., 2011). In addition to adversely impacting tourism (Villares et al., 1999), large algal mats can create a hostile physico-chemical environment. These mats may blanket surfaces, alter sediment chemistry (Raffaelli et al., 1989; Gamenick et al., 1996; Valiela et al., 1997), induce sulfide poisoning (Gamenick et al., 1996), and generate anoxic conditions at the water-sediment interface (Norkko et al., 2000). They can also modify bird feeding behaviors (Raffaelli et al., 1989), smother seagrass beds (den Hartog, 1994), and interfere with water use due to floating masses of detached algae. Additionally, they cause aesthetic issues such as odor nuisances and fouling of bathing waters (Montgomery et al., 1978; Charlier et al., 2008), and can alter benthic algal communities (Munda, 1993; Worm et al., 2001).
The frequency of massive Green Tides has increased worldwide (Smetacek & Zingone, 2013; see Fig. 3). Until 1999, Ulva sp. blooms were primarily recorded in Europe, the USA, South Africa, and Japan. Over the past 25 years, however, these blooms have spread significantly, with only Australia and Antarctica yet to report such events (see Fig. 3 and Table 1). The dispersal of free-floating thallus fragments can initiate new blooms in previously unaffected areas, posing serious ecological and economic challenges. Notably, newly identified species such as U. pseudo-ohnoi sp. nov. have also been implicated in massive bloom events (Lee et al., 2019).

<br>

![<span id="fig:Lolli"></span>**Fig. **3: Number of viruses, heterotrophic bacteria, fungi (Heterotrophs), micro- and macroalgae (Algae), invertebrates and vertebrates (Animals) affected by Ulva genus.](../Output/Figures/Lolli.png)

<br>

Multiple factors contribute to the formation and persistence of Ulva sp. blooms. The widespread distribution of both microscopic and macroscopic stages of Ulva sp. plays a role in the global outbreak of Green Tides (Teichberg et al., 2010; Jones et al., 2020). Excess nutrient inputs from agricultural runoff or wastewater discharge, combined with eutrophication, create ideal conditions for bloom formation (Teichberg et al., 2010). Additionally, the high surface-to-volume ratio of Ulva sp. enhances its rapid growth (Van Alstyne et al., 2015), and conditions such as brackish salinity and a pH near 7.0 have been linked to significant increases in biomass (Lin et al., 2011).
Green Tides have become a major concern for scientists, environmental organizations, and policymakers striving to mitigate their impacts on marine ecosystems and coastal communities. These large-scale blooms, particularly prevalent in nutrient-rich coastal areas (Kang & Chung, 2017), can alter light availability for phytoplankton and benthic communities over prolonged periods (Malta et al., 2003). For example, in the Venice Lagoon, a period of intense Ulva growth in the late 1980s was followed by a subsequent decline, which dramatically altered local conditions (Charlier et al., 2008). Furthermore, as Ulva biomass decomposes and sinks, oxygen depletion can lead to localized hypoxic "dead zones" (Hu & He, 2008).

Economic damages from Ulva sp. blooms are also significant. For instance, blooms of U. lactuca in coastal waters near urbanized and agricultural regions like Maui, Hawaii, result in annual losses exceeding 20 million dollars (Van Beukering & Cesar, 2004; Dailer et al., 2012). In Brittany, France, a Green Tide event led to the accumulation of 100,000 tonnes of Ulva biomass (primarily U. armoricana and U. rotundata), costing an estimated US 10–150 per tonne in cleaning and disposal expenses (Charlier et al., 2008). Similarly, in 2008, a 30-kilometer-long bloom of U. prolifera along the Qingdao coast in China required the disposal of over 1 million tonnes of biomass at a cost of US 30 million, employing 10,000 individuals (Ye et al., 2011; Shi et al., 2015; Mantri et al., 2020). The emergency response costs prior to the 2008 Beijing Olympic Games sailing competition in Qingdao were estimated at around 200 million euros, amounting to 5.84% of Qingdao Municipality's total income for that year (Berdalet et al., 2016).

<br>

# Methods of testing bioactivity of *Ulva* sp. {.unnumbered}

<br>

To assess the impact of Ulva sp. on other organisms, researchers employ a variety of investigative approaches. Common methods include adding extracts, conducting experiments with fresh thalli, performing co-culture assays, and carrying out field observations. In many studies, several methods are applied simultaneously for comparative analysis.
The most frequently used technique involves preparing extracts from dried Ulva sp. thalli. In this approach, a dry sample is ground and mixed with distilled water, seawater, or chemical reagents, followed by high-speed centrifugation or filtration. A specific dose of the resulting extract is then introduced to the target organism. A second method involves the use of cell-free filtrates. In this procedure, Ulva sp.—with a known biomass and maintained under controlled conditions—is cultivated for several days. The thalli are then removed, and the filtrate, containing bioactive compounds, is used to inoculate cultures of the target organisms. A third approach is the direct inoculation of fresh Ulva sp. thalli into cultures of the test organisms (Jin & Dong, 2003; Jin et al., 2005; Nan et al., 2008; Cai et al., 2011; Wang et al., 2012; Renjun et al., 2013; Accoroni et al., 2015; Lv et al., 2021; Salama et al., 2021). Additionally, isolation co-culture assays have been employed by Wang et al. (2006) and Jin and Dong (2003), whereby direct contact between the target species and Ulva sp. is prevented. Mesocosm experiments, using floating tanks deployed at the sampling site, allow Ulva sp. to be maintained under ambient conditions similar to its natural habitat (Tang & Gobler, 2011). Tang and Gobler (2011) also conducted bottle incubation experiments as part of their field studies.

<br>

#  The effect of *Ulva* sp. on surrounding ecosystem {.unnumbered}

<br>

Evidence indicates that Ulva sp. exhibits significant bioactivity against a variety of heterotrophic microorganisms, microalgae, seaweeds, grazers, and other animals. Most research has focused on species such as Ulva lactuca, U. fasciata, and U. rigida (see Fig. 4), with a detailed summary provided in the Supplementary Materials.

<br>

## *Ulva* sp. as a hazardous material affecting heterotrophic microorganisms {.unnumbered}

<br>

Research has demonstrated that various Ulva species can impact viruses, bacteria, and fungi (Figs. 4–7). Studies have documented effects on 20 different virus types, 22 heterotrophic bacterial types, and 28 fungal taxa, with Ulva lactuca being the most extensively tested—against 50 different taxa of heterotrophic microorganisms. Generally, these studies report a strongly or moderately inhibitory effect of *Ulva* compounds on microbial development. Notably, only certain species within the Aspergillus genus have exhibited growth stimulation under the influence of compounds secreted by Ulva lactuca (see Fig. 7). Frequently tested bacteria include strains of *Bacillus*, *Escherichia*, and *Staphylococcus* (Fig. 6). Recent research also indicates that Ulva can actively inhibit viruses, including SARS-CoV-2 (Fig. 5).

<br>

## *Ulva* sp. as a hazardous material affecting microalgae and seaweeds in the aquatic environment {.unnumbered}

<br>

Our comparative analysis reveals that both micro- and macroalgae constitute the largest group of organisms evaluated for the effects of Ulva compounds (Fig. 8). Testing has encompassed 21 taxa within Dinoflagellata, 17 within Heterokontophyta, 13 within Chlorophyta, 7 within Rhodophyta, 3 each from Cyanobacteria and Haptophyta, and single taxa from the Cryptista and Euglenophyta classes. The majority of these organisms exhibit strong to moderate growth inhibition. Although a few studies suggest that Ulva may negatively affect marine vascular plants such as Zostera (Olyarnik & Stachowicz, 2012), some reports indicate that compounds secreted by Ulva can positively influence terrestrial crops and vegetables; however, these effects appear to be of limited ecological significance.

<br>

## Ulva sp. as a hazardous material affecting invertebrates and vertebrates {.unnumbered}

<br>

Research indicates that Ulva sp. secretes compounds that adversely affect the development and physiology of various invertebrates and vertebrates (Figs. 4, 9; see Supplementary Materials). Investigations have covered seven animal phyla: 14 taxa from Arthropoda, 8 from Mollusca, 4 from Chordata, and one taxon each from Rotifera, Echinodermata, Porifera, and Platyhelminthes. The majority of these studies report growth inhibition or mortality following exposure to Ulva-derived compounds. However, some taxa, including Artemia, Brachionus, Cebidichthys, Inimicus, and Sparus, have shown resistance. Conversely, species such as Danio, Haliotis, and Litopenaeus may experience growth stimulation under the influence of compounds from certain Ulva genera.

Additionally, Ulva sp. is typically free of macroinvertebrate colonization due to the production of antifouling agents in the thallus boundary layer. These waterborne toxic macromolecules originate both from the thalli and their associated epibiotic bacteria (Harder et al., 2004). For example, U. reticulata secretes bioactive substances, supplemented by bacterial compounds, to repel fouling organisms (Dobretsov & Qian, 2002; Harder et al., 2004). Egan et al. (2000) further reported that bacteria on the surface of U. lactuca inhibit the growth of bacteria, fungi, invertebrate larvae, and microalgae, although research in this area remains limited.

<br>

# Active compounds and secondary metabolites of *Ulva* sp. {.unnumbered}

<br>

Ulva sp. harbors a diverse array of bioactive compounds, many of which have yet to be fully characterized for their potential harmful effects. The thallus of Ulva sp. contains amino acids such as cysteinolic acid, cysteic acid, proline, glutamic acid, and chondrine (Holdt & Kraan, 2011). It also comprises various secondary metabolites including terpenes, polyphenolic compounds, hexapeptides, diterpenoids, and steroids (Fujimura & Kajiwara, 1990; Flodin & Whitfield, 1999; Awad, 2000; Chakraborty et al., 2010a, b; Yildiz et al., 2012; Ennamany et al., 1998). Notably, taurine—an amino acid present in Ulva sp.—has been shown to act as a broad-spectrum cytoprotective agent (Ito & Hori, 1989; Peña-Rodríguez et al., 2011).

Moreover, Ulva sp. contains polyunsaturated fatty acids; extracts from U. rigida have demonstrated antimicrobial activity (Ismail et al., 2018). Sulphated polysaccharides, particularly ulvan—a water-soluble compound constituting approximately 8–29% of the dry weight of Ulva—have been noted for their anticoagulant activity through thrombin inhibition and potentiation of heparin cofactor II (Mao et al., 2006). Ulvan is also reported to possess anticancer, antiviral, hypocholesterolemic, hypolipidemic, and neuroprotective properties (Kaeffer et al., 1999; Smit, 2004; Rahimi et al., 2016; Li et al., 2017, 2018; Olasehinde et al., 2019). In contrast, Barakat et al. (2022) reported that ulvan adversely affected microalgae and certain bacterial and fungal species, such as Klebsiella pneumoniae, Staphylococcus epidermidis, Enterococcus faecalis, and Candida albicans. Additionally, studies by Alamsjah et al. (2008) indicated significant cell mortality in several microalgal taxa—caused by compounds from U. fasciata and U. pertusa—with tetraenoic acid and α-linolenic acid identified as key inhibitory agents. Lv et al. (2021) further demonstrated that hexadecanoic acid, octadecatetrienoic acid, and octadecenoic acid produced by U. linza induce cell death in species such as Prorocentrum minimum and Platymonas helgolandica. These findings underscore that Ulva sp. synthesizes a range of secondary metabolites with potent bioactivities that may have deleterious effects on various organisms.

<br>

**Table 9.**
Bioactive compounds produced by Ulva sp. and their biological activity on tested organisms.

<br>

# Conclusions {.unnumbered}

<br>

This review demonstrates that *Ulva* sp. is a globally distributed macroalga whose extensive physiological and molecular adaptations enable its widespread occurrence. Although Ulva sp. offers potential benefits for commercial applications such as food production, cosmetics, and bioremediation, its propensity to form massive blooms—known as Green Tides—poses significant environmental and economic challenges. The diverse methods employed to test the bioactivity of Ulva sp. reveal that its secondary metabolites have far-reaching inhibitory effects on heterotrophic microorganisms, microalgae, seaweeds, and even various invertebrates and vertebrates. These compounds, including amino acids, terpenes, polyphenolics, and sulphated polysaccharides, underscore the dual nature of *Ulva* sp. as both a resource and a hazardous material.
The evidence presented highlights the critical need for further interdisciplinary research to elucidate the mechanisms underlying Ulva sp. blooms and to develop effective management strategies. Such efforts are essential to mitigate the ecological disruptions and economic losses associated with these events, while also safeguarding human health and the integrity of marine ecosystems. Ultimately, a balanced approach that integrates advanced molecular techniques with traditional ecological assessments will be key to addressing the complex challenges posed by *Ulva* sp.

<br>

# CRediT authorship contribution statement {.unnumbered}

<br>

**Gracjana Budzałek**: Writing – original draft, Resources, Methodology, Investigation, Data curation, Conceptualization. **Kinga Wiśniewska**: Writing – original draft, Validation, Resources, Methodology, Investigation, Data curation. **Anna Dziubińska**: Writing – original draft, Validation, Resources, Methodology, Investigation, Data curation. **Sarah Postuma** Resources, Investigation, Data curation. **Anna Woźniak**: Resources, Investigation, Data curation. **Sylwia Śliwińska-Wilczewska**: Supervision, Project administration, Writing – original draft, Resources, Methodology, Investigation, Data curation, Funding acquisition, Conceptualization, Validation. 

<br>

# Declaration of Competing Interest {.unnumbered}

<br>

The authors declare that they have no known competing financial interests or personal relationships that could have appeared to influence the work reported in this paper.

<br>

# Acknowledgements {.unnumbered}

<br>

This work was supported by Canada Research Chair in Phytoplankton Ecophysiology (Douglass A. Campbell from Mount Allison University, Canada) and Latitude & Light; NSERC of Canada Discovery Grant (Douglass A. Campbell from Mount Allison University, Canada), and funded by DS. 531-O500-D717-25 (S.Ś-W.) and DS. 531-O402-D031-25 (A.D.).

<br>

# Data availability {.unnumbered}

Data supporting this study is available on:
https://github.com/FundyPhytoPhys/SynBaltic/Ulva (public GitHub Repository).

Code to perform data processing and analyses is available at https://github.com/FundyPhytoPhys/SynBaltic/Ulva.

<br>

# References {.unnumbered}
