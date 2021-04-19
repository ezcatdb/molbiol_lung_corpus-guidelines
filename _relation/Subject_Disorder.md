---
layout: entry
title: "Subject_Disorder"
shortdef: "relationships between subject and disorder (PHAEDRA)"
order: 110
---

This relation indicates relationships of [Subject]() with its disorder, [Disease]() or [Symptom](), and also [Phenotype]().

This relation is based on the <a href="http://www.nactem.ac.uk/">PHAEDRA corpus</a> at <a href="http://www.nactem.ac.uk/">NaCTeM</a>.

~~~ ann
IPF patients with a forced vital capacity (FVC) of 50-80%.
T1 Disorder 0 3 IPF
T2 Measurement 19 41 forced vital capacity
T3 Measurement 43 46 FVC
T5 Subject 0 12 IPF patients 
R3 Subject_Disorder Arg1:T5 Arg2:T1
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
Using PET-CT, we diagnosed liver metastases in the two patients.
T1 Anatomical_entity 27 32 liver
T2 Method_cue 6 12 PET-CT
T3 Artificial_process 17 26 diagnosed
T4 Disorder 27 43 liver metastases
T5 Subject 51 63 two patients
T6 Biological_process 33 43 metastases
E1 Artificial_process:T3 Theme:T4 cue:T2
E2 Biological_process:T6 atLoc:T1
R1 Subject_Disorder Arg1:T5 Arg2:T4
R2 part_of Arg1:T1 Arg2:T5
~~~
