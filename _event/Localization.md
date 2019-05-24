---
layout: entry
title: "Localization"
category: "Biological process"
shortdef: "Localization of entity"
order: 31
---

This event is based on the <a href="http://www.nactem.ac.uk/meta-knowledge/">GENIA-Meta-knowledge corpus</a> at <a href="http://www.nactem.ac.uk/">NaCTeM</a>.

This event indicates localization of entity, such as [Cell]() and [GGPs]().

The following words/phrases can be triggers of this event:

- accumulation
- localization, localized

~~~ ann
Accumulation of damaged mitochondria in lung epithelial cells.
T1 Localization 0 12 Accumulation
T2 Negative_regulation 16 23 damaged
T3 Cell_component 24 36 mitochondria
T4 Cell 40 61 lung epithelial cells
T5 Anatomical_entity 40 44 lung
E1 Localization:T1 Theme:E2 AtLoc:T4
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

Arguments:

The *atLoc* for this event must be
- [Subject]()
- [Anatomical_entity]()
- [Cell]()
- [Cell_component]() and
- [Entity Property]().

The other arguments, such as *Cause*, *Theme*, *Participant*, and *Product*, for this event can be any entities or events.


<!--details-->



