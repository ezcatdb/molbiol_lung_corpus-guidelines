---
layout: entry
title: "Subject"
shortdef: "Subjects for clinical trials, patients, and experimental animals (PHAEDRA)"
order: 7
---

The name of this entity group is based on the <a href="http://www.nactem.ac.uk/PHAEDRA/">PHAEDRA corpus</a> at <a href="http://www.nactem.ac.uk/">NaCTeM</a>.

<!--
-->

Patients, and subjects for clinical trials, and experimental animals, such as mice, are categorized into this entity group.

This entity indicates 'individual level' above the [Anatomical_entity]().

~~~ ann
Subjects who underwent lung resect.
T1 Subject 0 8 Subjects
T3 Anatomical_entity 23 27 lung
T4 Artificial_process 28 34 resect
E1 Artificial_process:T4 Theme:T3
R1 part_of Arg1:T3 Arg2:T1
~~~
~~~ ann
A 40-year-old man had undergone right upper lobectomy for lung cancer.
T1 Subject 2 17 40-year-old man
T2 Artificial_process 32 53 right upper lobectomy
T3 Disorder 58 70 lung cancer
E1 Artificial_process:T2 Theme:T3
R1 Subject_Disorder Arg1:T1 Arg2:T3
~~~
~~~ ann
70 subjects (50 men and 20 women; mean age, 63.1 y)
T1 Subject 0 11 70 subjects
T2 Subject 13 19 50 men
T3 Subject 24 32 20 women
R1 member_of Arg1:T2 Arg2:T1
R2 member_of Arg1:T3 Arg2:T1
~~~
~~~ ann
Bleomycin-induced pulmonary fibrosis in mice.
T1 Pharmacological_substance 0 9 Bleomycin
T2 Regulation 10 17 induced
T3 Disorder 18 36 pulmonary fibrosis
T4 Subject 40 44 mice
E1 Regulation:T2 Cause:T1 atLoc:T4 Theme:T3
R1 Subject_Disorder Arg1:T4 Arg2:T3
~~~

~~~ ann
Ten healthy volunteers took 200 mg itraconazole or matched placebo once daily for 4 days.
T1 Subject 0 22 Ten healthy volunteers
T5 Pharmacological_substance 35 47 itraconazole
T6 Pharmacological_substance 59 66 placebo
T7 Artificial_process 23 27 took
E1 Artificial_process:T7 Theme:T1 Instrument:T5
E2 Artificial_process:T7 Theme:T1 Instrument:T6
~~~


~~~ ann
Using PET-CT, we diagnosed liver metastases in the two patients.
T1 Anatomical_entity 27 32 liver
T2 Method_cue 6 12 PET-CT
T3 Artificial_process 17 26 diagnosed
T4 Disorder 27 43 liver metastases
T5 Subject 51 63 two patients
T6 Localization 33 43 metastases
E1 Artificial_process:T3 Theme:T4 cue:T2
E2 Localization:T6 atLoc:T1
R1 Subject_Disorder Arg1:T5 Arg2:T4
R2 part_of Arg1:T1 Arg2:T5
~~~


Regarding UMLS IDs for this entity, the IDs will be assigned as follows:
- C0030705; patients
- C2986479; Healthy Control
- C0009932; Control Groups (Controls who are not healthy.)

Regarding attribute for this entity, [Count_sbjct]() has been defined.
~~~ ann
Patients with IPF (n=25) and lung cancer (n=15)
T1 Subject 0 8 Patients
T2 Disorder 14 17 IPF
T3 Subject 19 23 n=25
T4 Disorder 29 40 lung cancer
T5 Subject 42 46 n=15
A1 Count_sbjct T3
A2 Count_sbjct T5
R1 Subject_Disorder Arg1:T3 Arg2:T2
R2 Subject_Disorder Arg1:T5 Arg2:T4
R3 member_of Arg1:T3 Arg2:T1
R4 member_of Arg1:T5 Arg2:T1
~~~

<!-- details -->
