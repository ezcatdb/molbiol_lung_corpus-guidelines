---
layout: entry
title: "Measurement"
shortdef: "Measurement for lung diseases"
order: 4
---

The definition of 'Measurement' for lung diseases may be mostly based on <a href="https://en.wikipedia.org/wiki/Spirometry">spirometry</a>, and <a href="https://en.wikipedia.org/wiki/Oxygen_saturation_(medicine)">oxygen saturation</a>.

'Measurement', which can be a group in phenotype, will be annotated in this category. 
The following words/phrases should be annotated as 'Measurement'.

The definition of 'Measurement' is based on the Semantic types of 
- 'lbpr' (Laboratory Procedure)
- 'lbtr' (Laboratory or Test Result)
- 'clna' (Clinical Attribute)
- 'diap' (Diagnostic Procedure)

in the <a href="https://www.nlm.nih.gov/research/umls/">UMLS database</a>.

These words/phrases may suggest the state of [Disorder](), and usually appear along with the corresponding values.

Based on <a href="https://en.wikipedia.org/wiki/Spirometry">spirometry</a>:
- forced vital capacity (UMLS; C3714541)
- FVC (UMLS; C3714541)
- % predicted forced vital capacity (UMLS; C2919678)
- %FVC (UMLS; C2919678) 
- total lung capacity (UMLS; C0040509)
- TLC (UMLS; C0040509)
- Diffusion Capacity of the Lung for Carbon Monoxide (UMLS; C1516251)
- DLco (UMLS; C1516251)
- % Predicted Diffusion Capacity of the Lung for Carbon Monoxide (UMLS; C4054207)
- %DLco (UMLS; C4054207)
- forced expiratory volume in 1 second (UMLS; C0849974)
- FEV1 (UMLS; C0849974)
- FEV1% (UMLS; C0849974)
- FEV1/FVC ratio (UMLS; C3815113)

- Forced expiratory flow (UMLS; C3804964)
- FEF (UMLS; C3804964)
  - maximal (mid-)expiratory flow [Rate] (UMLS; C0024966)
  - FEF 25%-75% (UMLS; C0024966)
  - mean mid-expiratory flow rate (UMLS; C1306020)
  - MMFR (UMLS; C0024966 or C1306020)
- peak expiratory flow (UMLS; C1518922)
- PEF (UMLS; C1518922)
- tidal volume (UMLS; C0040210)
- TV (UMLS; C0040210)

~~~ ann
IPF patients with a forced vital capacity (FVC) of 50-80%.
T1 Disorder 0 3 IPF
T2 Measurement 19 41 forced vital capacity
T3 Measurement 43 46 FVC
T5 Subject 4 12 IPF patients
R3 Subject_Disorder Arg1:T5 Arg2:T1
~~~

Based on <a href="https://en.wikipedia.org/wiki/Oxygen_saturation_(medicine)">oxygen saturation</a>:
- oxygen saturation (UNLS; C0523807)
  - arterial oxygen saturation (UMLS; C0428175)
  - SaO2 (UMLS; C0428175)
  - venous oxygen saturation (UMLS; C0428176)
  - SvO2 (UMLS; C0428176)
  - peripheral oxygen saturation (UMLS; C2317096)
  - SpO2 (UMLS; C2317096)


The following words/phrases are not from Spirometry, but definitely 'Measurement', as they can suggest the state of [Disorder]() along with the corresponding values:
- 6-min walk distance (UMLS; C4055399)
- 6MWD (UMLS; C4055399)
- 6-min walk test (UMLS; C4055399)
- 6MWT (UMLS; C4055399)
- cardiopulmonary exercise test
- cardiac stress test
- cardiac diagnostic test
- CPX test
- maximal oxygen consumption
- peak oxygen consumption
- VO2 peak
- VO2 max

<!-- details -->
