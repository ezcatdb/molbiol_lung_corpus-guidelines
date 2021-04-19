---
layout: entry
title: General rules for entities
shortdef: "Entity rules"
order: 0
---

The top ranking of the priority for entities are as follows:
- [Disorder]()
- [GGPs]()
- [Cell]()
- [Pharmacological_substance]()

<!--
- [Anatomical_entity]()
- [Protein_molecule]()
-->

There are general rules for entities, as follows:

 - Articles, such as "a", "an" and "the", are not included in the entities.
 
~~~ ann
A 40-year-old man had undergone right upper lobectomy for lung cancer.
T1 Subject 2 17 40-year-old man
T2 Artificial_process 32 53 right upper lobectomy
T3 Disorder 58 70 lung cancer
E1 Artificial_process:T2 Theme:T3
R1 Subject_Disorder Arg1:T1 Arg2:T3
~~~
~~~ ann
The patient did not undergo lung resect.
T1 Subject 4 11 patient
T2 Negation_cue 16 19 not
T3 Anatomical_entity 28 32 lung
T4 Artificial_process 33 39 resect
E1 Artificial_process:T4 Theme:T3 cue:T2
A1 Negated E1
~~~
 
 - Numerals should be included in the entities, as they can suggest groups.

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

 
 <!-- details -->
