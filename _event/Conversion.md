---
layout: entry
title: "Conversion"
category: "Molecular process"
shortdef: "Changes in covalent bonds"
order: 71
---

<!---
This event is based on the <a href="http://www.nactem.ac.uk/meta-knowledge/">GENIA-Meta-knowledge corpus</a> at <a href="http://www.nactem.ac.uk/">NaCTeM</a>.
--->

This event describes the changes in covalent bonds of molecules, including modification of protein molecules and cleavage of covalent bonds.

The following words/phrases can be triggers of this event:

- autophosphorylation  
- phosphorylated  
- phosphorylation  
- phosphorylations  
- protein phosphorylation
- tyrosine autophosphorylation 
- tyrosine phosphorylation
- self-phosphorylation
- hyperphosphorylation
- dephosphorylation
- methylation
- acetylation
- cleavage  
- degradation  

~~~ ann
Phosphorylation of AKT2 was downregulated.
T1 Conversion 0 15 Phosphorylation
T2 GGPs 19 23 AKT
T3 Negative_regulation 28 40 downregulated
E1 Conversion:T1 Theme:T2
E2 Negative_regulation:T3 Theme:E1
~~~


Arguments:

<!---
The *atLoc*, *fromLoc* and *toLoc* for this event must be [Subject](), [Anatomical_entity](), [Cell](), [Cell_component]() and [Entity Property]().

The other arguments, such as *Cause*, *Theme*, *Participant*, and *Product*, for this event can be any entities or events.
--->

<!--details-->



