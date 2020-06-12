---
layout: entry
title: "Speculated"
shortdef: "Speculation attributes for events"
order: 1
---

Event triggers, which are connected with Speculation cues or Method cues, should be ticked off with “Speculated” attributes.

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
~~~ ann
We hypothesized that direct implantation might have led to metastasis.
T1 Speculation_cue 3 15 hypothesized
T2 Artificial_process 21 40 direct implantation
T3 Speculation_cue 41 46 might
T4 Positive_regulation 52 58 led to
T5 Biological_process 59 69 metastasis
E1 Artificial_process:T2 
E2 Positive_regulation:T4 Cause:E1 Theme:T5 cue:T3 cue2:T1 
E3 Biological_process:T5
A1 Speculated E2
~~~
~~~ ann
Using PET-CT, we diagnosed liver metastases in the two patients.
T1 Method_cue 6 12 PET-CT
T2 Speculation_cue 17 26 diagnosed
T3 Anatomical_entity 27 32 liver metastases
T4 Biological_process 33 43 liver metastases
T5 Subject 51 63 two patients
T6 Disorder 27 43 liver metastases
E1 Biological_process:T4 Theme:T3 cue:T1 cue2:T2
A1 Speculated E1
A2 Certainty E1 Confirmed
R1 Subject_Disorder Arg1:T5 Arg2:T6
R2 part_of Arg1:T3 Arg2:T5
~~~

