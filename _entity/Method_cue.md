---
layout: entry
title: "Method Cue"
shortdef: "Cues by experimental study types"
order: 109
---

This cue may suggest confirmation degree of events.
This cue can be types of experimental studies to analyse biological events. 

Specific action for experimental procedures should be annotated as [Artificial_process]().

- ***(experimental/computational)*** analyses/tests/assays 

More concrete analysis names for the cue are as follows:

- Mutagenesis
- [reversed-phase *etc.*] choromatography
- enzyme-linked immunosorbent assay (UMLS; C0014441)
- ELISA (UMLS; C0014441)

~~~ ann
Bronchoalveolar lavage fluids from 2 patients were concentrated by reversed-phase chromatography.
T1 Anatomical_entity 0 30 Bronchoalveolar lavage fluids
T2 Subject 36 46 2 patients
T3 Artificial_process 52 64 concentrated
T4 Method_cue 68 97 reversed-phase chromatography
E1 Artificial_process:T3 Theme:T1
R1 part_of Arg1:T1 Arg2:T2
~~~

<!--details-->
