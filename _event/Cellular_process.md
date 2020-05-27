---
layout: entry
title: "Cellular_process"
category: "Cellular process"
shortdef: "Processes on cellular levels"
order: 50
---

This event is based on the <a href="http://www.nactem.ac.uk/meta-knowledge/">GENIA-Meta-knowledge corpus</a> at <a href="http://www.nactem.ac.uk/">NaCTeM</a>.

The following words/phrases can be triggers of this event:

- apoptosis (UMLS; C0162638)
- [cell] differentiation [process] (UMLS; C0007589)
- carcinogenesis (UMLS; C0596263)
- cellular crosstalk (UMLS; C0007582)
- intercellular communication process (UMLS; C0007582)
- cell injury (UMLS ID:C0599732)
- endoplasmic reticulum (ER) stress (UMLS; C3178870)
  - unfolded protein response (UMLS; C1155342)

The following words/phrases related to cell cycle (UMLS; C0007586) can be triggers of this event as well (see <a href="https://en.wikipedia.org/wiki/Cell_cycle">Cell cycle</a>):
  - cell cycle progression (UMLS; C1516334)
  - cell cycle control (UMLS; C1155872)
  - G1 [cell cycle] arrest (UMLS; C3178834)

~~~ ann
Cellular crosstalk between epithelial cells and fibroblasts.
T1 Cellular_process 0 18 Cellular crosstalk
T2 Cell 27 43 epithelial cells
T3 Cell 48 59 fibroblasts
E1 Cellular_process:T1 Participant:T2 Participant2:T3
~~~
~~~ ann
Epithelial cell injury
T1 Cell 0 15 Epithelial cell
T2 Cellular_process 16 22 injury
E1 Cellular_process:T2 Theme:T1
~~~

Arguments:

The *atLoc*, *fromLoc* and *toLoc* for this event must be
- [Cell]()
- [Cell_component]()
- [Entity Property]().

<!---
The other arguments, such as *Cause*, *Theme*, *Participant*, and *Product*, for this event can be any entities or events.
--->

<!--details-->



