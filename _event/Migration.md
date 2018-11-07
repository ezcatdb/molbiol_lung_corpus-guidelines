---
layout: entry
title: "Migration"
category: "Biological process"
shortdef: "Migration/movement of entity"
order: 14
---

This event indicates movement of entity, such as [Cell]() and [Protein_molecule]().

The following words/phrases can be triggers of this event:

- infection
- metastasis

~~~ ann
Squamous cell carcinoma of the lung invaded the right main bronchus.
T1 Disease 0 23 Squamous cell carcinoma
T2 Cell 0 13 Squamous cell
T3 Anatomical_entity 31 35 lung
T4 Anatomical_entity 48 67 right main bronchus
T5 Migration 36 43 invaded
E1 Migration:T5 Theme:T1 fromLoc:T3 toLoc:T4
~~~
~~~ ann
Using PET-CT, we diagnosed liver metastases in the two patients.
T2 Anatomical_entity 27 32 liver
T4 Disease 27 43 liver metastases
T5 Subject 51 63 two patients
T7 Migration 33 43 metastases
E2 Migration:T7 toLoc:T2
R1 Subject_Disorder Arg1:T5 Arg2:T4
~~~

Arguments:

The *atLoc*, *fromLoc* and *toLoc* for this event must be [Subject](), [Anatomical_entity](), [Cell](), [Cell_component]() and [Entity Property]().

Another argument, *Theme*, for this event can be any entities, such as [Cell]() and molecule entities.

<!--details-->



