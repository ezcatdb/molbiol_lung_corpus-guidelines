---
layout: entry
title: "Localization"
category: "Biological process"
shortdef: "Localization/movement of entity"
order: 31
---

This event is based on the <a href="http://www.nactem.ac.uk/meta-knowledge/">GENIA-Meta-knowledge corpus</a> at <a href="http://www.nactem.ac.uk/">NaCTeM</a>.

This event indicates localization or movement of entities, such as [Cell]() and molecular entities including [GGPs]().

The following words/phrases can be triggers of localization event:

- accumulation
- localization, localized (UMLS ID:C0475264 -> C1744691)
- adhesion

~~~ ann
Accumulation of damaged mitochondria in lung epithelial cells.
T1 Localization 0 12 Accumulation
T2 Negative_regulation 16 23 damaged
T3 Cell_component 24 36 mitochondria
T4 Cell 40 61 lung epithelial cells
T5 Anatomical_entity 40 44 lung
E1 Localization:T1 Theme:T3 atLoc:T4
E2 Negative_regulation:T2 Theme:T3
R1 part_of Arg1:T3 Arg2:T4
R2 part_of Arg1:T4 Arg2:T5
~~~
~~~ ann
BIRC5 is localized to the cytoplasm.
T1 GGPs 0 5 BIRC5
T2 Localization 10 19 localized
T3 Cell_component 27 36 cytoplasm
E1 Localization:T2 Theme:T1 atLoc:T3
~~~

The following words/phrases can be triggers of movement event:

- infection (This can be [Disorder]())
- metastasis
- invade, invasion
- migration
  - cell migration (UMLS ID:C1622501)
- chemotactic activity (UMLS ID:C0008018)
- chemotaxis (UMLS ID:C0008018)
- cellular infiltrate/infiltration
- (cellular) secretion (UMLS ID:C0036536)
  - release (UMLS ID:C0036536)

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
T1 Anatomical_entity 27 32 liver
T2 Method_cue 6 12 PET-CT
T3 Artificial_process 17 26 diagnosed
T4 Disorder 27 43 liver metastases
T5 Subject 51 63 two patients
T6 Localization 33 43 metastases
E1 Artificial_process:T3 Theme:T4 Cue:T2
E2 Localization:T6 atLoc:T1
R1 Subject_Disorder Arg1:T5 Arg2:T4
R2 part_of Arg1:T1 Arg2:T5
~~~
~~~ ann
lung alveolar epithelial cell migration
T1 Anatomical_entity 0 4 lung
T2 Cell 5 29 alveolar epithelial cell
T3 Localization 30 39 migration
E1 Localization:T3 Theme:T2 atLoc:T1
R1 part_of Arg1:T2 Arg2:T1
~~~
~~~ ann
IL-8 secretion
T1 GGPs 0 4 IL-8
T2 Localization 5 14 secretion
E1 Localization:T2 Theme:T1
~~~
~~~ ann
TNF-alpha release by alveolar macrophages
T1 GGPs 0 9 TNF-alpha
T2 Localization 10 17 release
T3 Cell 21 41 alveolar macrophages
E1 Localization:T2 Theme:T1 fromLoc:T3
~~~

The following cases, in which the words such as "foci" or "focus" can be annotated as event trigger for this event, might be special:
Here, these words may be tentatively assigned the same ID as "localization" (UMLS ID:C0475264).
- fibroblast foci
- fibroblastic foci 
- myofibroblast-rich focus core
- fibroblastic focus

~~~ ann
fibroblastic foci
T1 Cell 0 12 fibroblastic
T2 Localization 13 17 foci
E1 Localization:T2 Theme:T1
~~~
~~~ ann
myofibroblast-rich focus core
T1 Cell 0 13 myofibroblast
T2 Localization 19 29 focus core
E1 Localization:T2 Theme:T1
~~~
- 
Arguments:

The *atLoc* argument indicates the location at which this event occurs. 
The *fromLoc* indicates the location from which this event starts, whereas the *toLoc* indicates the location to which this event proceeds.
The *atLoc*, *fromLoc* and *toLoc* for this event must be
- [Subject]()
- [Anatomical_entity]()
- [Cell]()
- [Cell_component]()

The other argument, *Theme*, for this event can be any entities, which are targets of this event.

The *disorder* argument must be [Disorder]().

The *Cue* argument is cues, such as [Negation cue](), [Speculation cue]() or [Method cue]().


<!--
The other arguments, such as *Cause*, *Theme*, *Participant*, and *Product*, for this event can be any entities or events.
-->

<!--details-->



