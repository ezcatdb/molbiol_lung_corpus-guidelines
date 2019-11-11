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

- metabolism
- metabolic pathway
- signaling  
- signaling cascade 
- signaling pathway 
- signalling  
- molecular pathway 
- pathway[s]  
- [protein] signaling
- [protein] signaling pathway
- [cell] signaling pathways

The following examples are more specific pathways:
- EGFR signaling
- ErbB signaling pathway
- MAPK signaling
- PDGFR signaling
- PI3K signaling 
- VEGFR2 signaling pathway
- integrin signaling
- mTOR signaling

~~~ ann
MAPK signaling pathway
T1 GGPs 0 4 MAPK
T2 Pathway 5 22 signaling pathway
T3 Pathway 0 22 MAPK signaling pathway
E1 Pathway:T2 Participant:T1
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

Arguments:
*Participant* (optional; zero or more) for this event must be [GGPs](), [Organic_compound_other]() or [Pharmacological_substance](), which are molecular entities participating in pathway.

*AtLoc* (optional; zero or one) indicates the location, such as [Cell_component](), [Cell]() or  [Anatomical_entity](), where `Pathway` event occurs.

<!---
The *atLoc*, *fromLoc* and *toLoc* for this event must be [Subject](), [Anatomical_entity](), [Cell](), [Cell_component]() and [Entity Property]().

The other arguments, such as *Cause*, *Theme*, *Participant*, and *Product*, for this event can be any entities or events.
--->

<!--details-->



