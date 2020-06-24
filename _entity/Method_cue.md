---
layout: entry
title: "Method cue"
shortdef: "Cues by experimental study/clinical diagnosis types"
order: 109
---

The 'Method cue' may suggest confirmation/speculation degree of events.
This cue can be types of experimental studies/clinical examination to analyse biological events. 

Specific actions for experimental procedures/clinical examiniations should be annotated as [Artificial_process](). Such actions may make some effects on entities.

- ***(experimental/computational)*** analyses/tests/assays 

More concrete analysis names for the cue are as follows:

- [reversed-phase *etc.*] choromatography
- enzyme-linked immunosorbent assay (UMLS; C0014441)
- ELISA (UMLS; C0014441)
- chest X-ray (UMLS; C0039985)
- CT scan(s) (UMLS; C0040405)

<!--
- Mutagenesis
-->

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
Markers of fibrogenesis, including collagen and CTGF were evaluated by measuring mRNA level using RT-PCR.
T1 GGPs 0 7 Markers
T2 Biological_process 11 23 fibrogenesis
T3 GGPs 35 43 collagen
T4 GGPs 48 52 CTGF
T5 Speculation_cue 58 67 evaluated
T6 Speculation_cue 71 80 measuring
T7 Gene_expression 81 91 mRNA level
T8 Gene_expression 81 91 mRNA level
T9 Method_cue 98 104 RT-PCR
E1 Biological_process:T2 Participant:E2 Participant2:E3 cue:T5
E2 Gene_expression:T7 Theme:T3 cue:T6 cue2:T9
E3 Gene_expression:T8 Theme:T4 cue:T6 cue2:T9
R1 member_of Arg1:T3 Arg2:T1
R2 member_of Arg1:T4 Arg2:T1
A1 Speculated E1
A2 Speculated E2
A3 Speculated E3
~~~
<!--details-->
