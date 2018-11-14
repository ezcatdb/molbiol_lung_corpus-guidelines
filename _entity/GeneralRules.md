---
layout: entry
title: General rules for entities
shortdef: "Entity rules"
order: 0
---

The top ranking of the priority for entities are as follows:
- [Disease]()
- [Protein_molecule]()
- [Cell]()
- [Pharmacological_substance]()
- [Anatomical_entity]()

There are general rules for entities, as follows:

 - Articles, such as "a", "an" and "the", are not included in the entities.
 
~~~ ann
A 40-year-old man had undergone right upper lobectomy for lung cancer.
T1 Subject 2 17 40-year-old man
T3 Disease 58 70 lung cancer
T4 Anatomical_entity 58 62 lung
R1 Subject_Disorder Arg1:T1 Arg2:T3
~~~
~~~ ann
The patient did not undergo lung resect.
T1 Subject 4 11 patient
T2 Negation_cue 16 19 not
T3 Anatomical_entity 28 32 lung
~~~
 
 - Numerals should be included in the entities, as they can suggest groups.

~~~ ann
Using PET-CT, we diagnosed liver metastases in the two patients.
T1 Anatomical_entity 27 32 liver
T4 Disease 27 43 liver metastases
T5 Subject 51 63 two patients
R1 Subject_Disorder Arg1:T5 Arg2:T4
~~~

 
 <!-- details -->
