---
layout: entry
title: "Pathway"
category: "Molecular function"
shortdef: "Molecular pathway networks (metabolism, signaling)"
order: 72
---

<!---
This event is based on the <a href="http://www.nactem.ac.uk/meta-knowledge/">GENIA-Meta-knowledge corpus</a> at <a href="http://www.nactem.ac.uk/">NaCTeM</a>.
--->

This event describes Molecular pathway networks, such as metabolism and signaling pathways.

The following words/phrases can be triggers of this event:

- metabolic pathway (UMLS ID:C1291081)
  - metabolism
- signaling pathway (UMLS ID:C0037080)
  - signaling  
  - signaling cascade 
  - signalling
  - [protein] signaling
  - [protein] signaling pathway
  - [cell] signaling pathways
- molecular pathway (UMLS ID:C1706062)
  - pathway[s] (UMLS ID:C1706062)

The following examples are more specific pathways:
- EGFR signaling (UMLS ID:C3271839)
- ErbB signaling pathway (UMLS ID:C2984323)
- MAPK signaling  (UMLS ID:C1518102)
- PDGFR signaling (UMLS ID:C1155400)
- PI3K signaling (UMLS ID:C1817666) 
- VEGFR2 signaling pathway (UMLS ID:C3549205)
- integrin signaling (UMLS ID:C1512812)
- mTOR signaling (UMLS ID:C1515673)

~~~ ann
MAPK signaling pathway
T1 GGPs 0 4 MAPK
T3 Pathway 0 22 MAPK signaling pathway
E2 Pathway:T3 Participant:T1
~~~
~~~ ann
AKT2-mediated signaling pathway
T1 GGPs 0 4 AKT2
T2 Positive_regulation 5 13 mediated
T3 Pathway 14 31 signaling pathway
E1 Positive_regulation:T2 Cause:T1 Theme:E2
E2 Pathway:T3
~~~

Occasionally, more than one participant molecule can be included in this event.
~~~ ann
MEKK1/MEK1/ERK1 and AP-1 pathway
T1 GGPs 0 5 MEKK1
T2 GGPs 6 10 MEK1
T3 GGPs 11 15 ERK1
T4 GGPs 20 24 AP-1
T5 Pathway 0 32 MEKK1/MEK1/ERK1 and AP-1 pathway
E1 Pathway:T5 Participant:T1 Participant2:T2 Participant3:T3 Participant4:T4
~~~

Arguments:

*Participant* (optional; zero or more) for this event must be [GGPs](), [Organic_compound_other]() or [Pharmacological_substance](), which are molecular entities involved in the `Pathway`.

*atLoc* (optional; zero or one) indicates the location, such as [Cell_component](), [Cell]() or  [Anatomical_entity](), where `Pathway` event occurs.

<!---
The *atLoc*, *fromLoc* and *toLoc* for this event must be [Subject](), [Anatomical_entity](), [Cell](), [Cell_component]() and [Entity Property]().

The other arguments, such as *Cause*, *Theme*, *Participant*, and *Product*, for this event can be any entities or events.
--->

<!--details-->



