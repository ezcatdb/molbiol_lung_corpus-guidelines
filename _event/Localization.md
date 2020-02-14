---
layout: entry
title: "Localization"
category: "Biological process"
shortdef: "Localization/movement of entity"
order: 31
---

This event is based on the <a href="http://www.nactem.ac.uk/meta-knowledge/">GENIA-Meta-knowledge corpus</a> at <a href="http://www.nactem.ac.uk/">NaCTeM</a>.

This event indicates localization or movement of entity, such as [Cell]() and molecular entities including [GGPs]().

The following words/phrases can be triggers of localization event:

- accumulation
- localization, localized

~~~ ann
Accumulation of damaged mitochondria in lung epithelial cells.
T1 Localization 0 12 Accumulation
T2 Negative_regulation 16 23 damaged
T3 Cell_component 24 36 mitochondria
T4 Cell 40 61 lung epithelial cells
T5 Anatomical_entity 40 44 lung
E1 Localization:T1 Theme:T3 AtLoc:T4
E2 Negative_regulation:T2 Theme:T3
R1 part_of Arg1:T3 Arg2:T4
R2 part_of Arg1:T4 Arg2:T5
~~~
~~~ ann
BIRC5 is localized to the cytoplasm.
T1 GGPs 0 5 BIRC5
T2 Localization 10 19 localized
T3 Cell_component 27 36 cytoplasm
E1 Localization:T2 Theme:T1 AtLoc:T3
~~~

The following words/phrases can be triggers of movement event:

- infection
- metastasis
- invade, invasion

~~~ ann
Squamous cell carcinoma of the lung invaded the right main bronchus.
T1 Disorder 0 23 Squamous cell carcinoma
T2 Cell 0 23 Squamous cell carcinoma
T3 Anatomical_entity 31 35 lung
T4 Anatomical_entity 48 67 right main bronchus
T5 Localization 36 43 invaded
E1 Localization:T5 Theme:T2 fromLoc:T3 toLoc:T4
~~~
~~~ ann
Using PET-CT, we diagnosed liver metastases in the two patients.
T2 Anatomical_entity 27 32 liver
T4 Disorder 27 43 liver metastases
T5 Subject 51 63 two patients
T7 Localization 33 43 metastases
E2 Localization:T7 toLoc:T2
R1 Subject_Disorder Arg1:T5 Arg2:T4
~~~

Arguments:

The *atLoc*, *fromLoc* and *toLoc* for this event must be
- [Subject]()
- [Anatomical_entity]()
- [Cell]()
- [Cell_component]() and
- [Entity Property]()

The other argument, *Theme*, for this event can be any entities or events.

The *disorder* argument must be only [Disorder]().

<!--
The other arguments, such as *Cause*, *Theme*, *Participant*, and *Product*, for this event can be any entities or events.
-->

<!--details-->



