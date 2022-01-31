---
layout: entry
title: "Cellular_process"
category: "Cellular process"
shortdef: "Processes on cellular levels"
order: 50
---

This event is based on the <a href="http://www.nactem.ac.uk/meta-knowledge/">GENIA-Meta-knowledge corpus</a> at <a href="http://www.nactem.ac.uk/">NaCTeM</a>.

Among the biological processes, those processes on the cellular levels are categorized into this event.

The following words/phrases can be triggers of this event:

- apoptosis (UMLS; C0162638)
- [cell] differentiation [process] (UMLS; C0007589)
- carcinogenesis (UMLS; C0596263)
- cellular crosstalk (UMLS; C0007582)
- intercellular communication process (UMLS; C0007582)
- cell-cell interaction (UMLS; C0007582)
- cell injury (UMLS ID:C0599732)
- endoplasmic reticulum (ER) stress (UMLS; C3178870)
  - unfolded protein response (UMLS; C1155342)
- epithelial to mesenchymal transition (EMT) (UMLS; C1523298)

The following words/phrases related to cell cycle (UMLS; C0007586) can be triggers of this event as well (see <a href="https://en.wikipedia.org/wiki/Cell_cycle">Cell cycle</a>):
  - cell cycle progression (UMLS; C1516334)
  - cell cycle control (UMLS; C1155872)
  - G1 [cell cycle] arrest (UMLS; C3178834)

~~~ ann
apoptosis of mesenchymal cells
T1 Cellular_process 0 9 apoptosis
T2 Cell 13 30 mesenchymal cells
E1 Cellular_process:T1 Theme:T2
~~~
~~~ ann
apoptosis in fibroblasts
T1 Cellular_process 0 9 apoptosis
T2 Cell 13 24 fibroblasts
E1 Cellular_process:T1 Theme:T2
~~~

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
~~~ ann
Rapamycin pretreatment decreased the proportions of alveolar epithelial cells undergoing EMT in bleomycin-induced pulmonary fibrosis.
T1 Pharmacological_substance 0 9 Rapamycin
T2 Artificial_process 10 22 pretreatment
T3 Negative_regulation 23 32 decreased
T4 Cell 52 77 alveolar epithelial cells
T5 Cellular_process 89 92 EMT
T6 Pharmacological_substance 96 105 bleomycin
T7 Positive_regulation 106 113 induced
T8 Disorder 114 132 pulmonary fibrosis
E1 Artificial_process:T2 instrument:T1
E2 Negative_regulation:T3 Theme:E3 Cause:E1 disorder:T8
E3 Cellular_process:T5 Theme:T4
E4 Positive_regulation:T7 Theme:T8 Cause:T6
~~~

Arguments:

The *Cause* for this event is entities/events, which cause this event, whereas the *Theme* for this event is entities/events, which are targets of this events. 
Usually, the *Theme* for this event is [Cell]().

The *Participant* is entities/events, which are involved in this event.

The *Product* is entities/events, which is produced by this event.

The *atLoc* argument (optional) indicates the location at which this event occurs. 
The *fromLoc* (optional) indicates the location from which this event starts, whereas the *toLoc* (optional) indicates the location to which this event proceeds.

The *disorder* (optional) indicates the [Disorder]() for which the `Cellular process` event occurs.

The *Cue* argument (optional) is cues, such as [Negation cue](), [Speculation cue]() or [Method cue]().

<!---
The other arguments, such as *Cause*, *Theme*, *Participant*, and *Product*, for this event can be any entities or events.
--->

<!--details-->
