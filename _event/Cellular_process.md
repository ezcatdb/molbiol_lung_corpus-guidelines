---
layout: entry
title: "Cellular_process"
category: "Cellular process"
shortdef: "Processes on cellular levels"
order: 50
---

This event is based on the <a href="http://www.nactem.ac.uk/meta-knowledge/">GENIA-Meta-knowledge corpus</a> at <a href="http://www.nactem.ac.uk/">NaCTeM</a>.

The following words/phrases can be triggers of this event:

- apoptosis
- differentiation
- carcinogenesis
- angiogenesis
- cellular crosstalk
- cell cycle
  - G1 phase
  - G1 arrest
  - G1 checkpoint
  - G2 checkpoint

~~~ ann
Cellular crosstalk between epithelial cells and fibroblasts.
T1 Cellular_process 0 18 Cellular crosstalk
T2 Cell 27 43 epithelial cells
T3 Cell 48 59 fibroblasts
E1 Cellular_process:T1 Participant:T2 Participant2:T3
~~~

Arguments:

The *atLoc*, *fromLoc* and *toLoc* for this event must be
- [Cell](),
- [Cell_component]()
- [Entity Property]().

<!---
The other arguments, such as *Cause*, *Theme*, *Participant*, and *Product*, for this event can be any entities or events.
--->

<!--details-->



