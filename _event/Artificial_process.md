---
layout: entry
title: 'Artificial_process'
category: "Artificial process"
shortdef: "Artificial process, such as experimental procedures/medical treatments"
order: 0
---

This event describes 'Artificial processes', which are usually specific actions for experimental procedures/medical treatments. Thus, this event can affect entities.

Analysis/assay names should be annotated as [Method cue](), which may suggest confirmation/speculation degree of events.

The following words/phrases can be triggers for this event:
- treat/treatment
  - pretreatment (UMLS; C3539076)
- incubate/incubation (UMLS; C1439852)
  - preincubation
- addition
- culture/cultured (UMLS; C1449619)
  - coculture (UMLS; C0282547)
- transfection (UMLS; C0040669)
- exposure (UMLS; C0332157)
- administer/administration (UMLS; C1621583)
- adoptive transfer (UMLS; C0376518)
- concentrate (UMLS; C2003864)
- decellularize(d)/decellularization (UMLS; C3827823)
- surgery (UMLS; C0543467)

~~~ ann
IL-33 treatment
T1 GGPs 0 5 IL-33
T2 Artificial_process 6 15 treatment
E1 Artificial_process:T2 Instrument:T1
~~~
~~~ann
T cell blasts were treated with PMA.
T1 Cell 0 13 T cell blasts
T2 Artificial_process 19 26 treated
T3 Organic_compound_other 32 35 PMA
E1 Artificial_process:T2 Theme:T1 Instrument:T3
~~~
~~~ ann
The cancer cell line was treated with various concentration of paclitaxel for 24 hours.
T1 Cell 4 20 cancer cell line
T2 Artificial_process 25 32 treated
T3 Pharmacological_substance 63 73 paclitaxel
E1 Artificial_process:T2 Theme:T1 Instrument:T3
~~~
~~~ ann
Administration of IL-13 to mice.
T1 Artificial_process 0 14 Administration
T2 GGPs 18 23 IL-13
T3 Subject 27 31 mice
E1 Artificial_process:T1 Theme:T3 Instrument:T2
~~~
~~~ ann
Bronchoalveolar lavage fluids from 2 patients were concentrated by reversed-phase chromatography.
T1 Anatomical_entity 0 29 Bronchoalveolar lavage fluids
T2 Subject 35 45 2 patients
T3 Artificial_process 51 63 concentrated
T4 Method_cue 67 96 reversed-phase chromatography
E1 Artificial_process:T3 Theme:T1
R1 part_of Arg1:T1 Arg2:T2
~~~
~~~ ann
Fibroblasts are cultured on hydrogels with collagen and IL-13 for 8 days.
T1 Cell 0 11 Fibroblasts
T2 Artificial_process 16 24 cultured
T3 Organic_compound_other 28 37 hydrogels
T4 GGPs 43 51 collagen
T5 GGPs 56 61 IL-13
E1 Artificial_process:T2 Theme:T1 Instrument:T3 Instrument2:T4 Instrument3:T5
~~~
~~~ ann
Decellularized lung matrices
T1 Artificial_process 0 14 Decellularized
T2 Anatomical_entity 15 19 lung
T3 Anatomical_entity 20 27 matrices
E1 Artificial_process:T1 Product:T3
R1 part_of Arg1:T3 Arg2:T2
~~~
~~~ ann
The IPF patient underwent thoracoscopic surgery.
T1 Disorder 4 7 IPF
T2 Subject 4 15 IPF patient
T3 Artificial_process 26 47 thoracoscopic surgery
E1 Artificial_process:T3 Theme:T2
R1 Subject_Disorder Arg1:T2 Arg2:T1
~~~

Arguments:

The *Theme* for this event can be [Subject](), [Cell](), [GGPs](), [Organic_compound_other](), and [Pharmacological_substance]().

The *Instrument* for this event can be entities used to carry out an artificial process, such as [GGPs](), [Organic_compound_other](), and [Pharmacological_substance]().

<!--details-->
