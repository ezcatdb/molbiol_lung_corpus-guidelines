---
layout: entry
title: "Method Cue"
shortdef: "Cues by experimental study types"
order: 109
---

The 'Method cue' may suggest confirmation/speculation degree of events.
This cue can be types of experimental studies/clinical examination to analyse biological events. 

Specific actions for experimental procedures/clinical examiniations should be annotated as [Artificial_process](). Such actions may make some effect on entities.

- ***(experimental/computational)*** analyses/tests/assays 

More concrete analysis names for the cue are as follows:

- Mutagenesis
- [reversed-phase *etc.*] choromatography
- enzyme-linked immunosorbent assay (UMLS; C0014441)
- ELISA (UMLS; C0014441)
- chest X-ray (UMLS; C0039985)
- CT scan(s) (UMLS; C0040405)

~~~ ann
Bronchoalveolar lavage fluids from 2 patients were concentrated by reversed-phase chromatography.
T1 Anatomical_entity 0 29 Bronchoalveolar lavage fluids
T2 Subject 35 45 2 patients
T3 Artificial_process 51 63 concentrated
T4 Method_cue 67 96 reversed-phase chromatography
E1 Artificial_process:T3 Theme:T1
R1 part_of Arg1:T1 Arg2:T2
~~~

<!--details-->
