---
layout: entry
title: "Conversion"
category: "Molecular function"
shortdef: "Changes in covalent bonds"
order: 71
---

<!---
This event is based on the <a href="http://www.nactem.ac.uk/meta-knowledge/">GENIA-Meta-knowledge corpus</a> at <a href="http://www.nactem.ac.uk/">NaCTeM</a>.
--->

This event describes the changes in covalent bonds of molecules, including modification of protein molecules and cleavage of covalent bonds.

The following words/phrases can be triggers of this event:

- phosphorylated  
- phosphorylation  
- phosphorylations  
  - autophosphorylation
  - self-phosphorylation
  - protein phosphorylation
  - tyrosine autophosphorylation 
  - tyrosine phosphorylation
  - hyperphosphorylation
- dephosphorylation
- methylation
- acetylation
- carboxymethylation
- cleavage  
- degradation  

Moreover, *enzyme activity*, which changes covalent bonds of [Organic_compound_other]() or [GGPs](), can be trigger words for this event.

- [enzyme] activity
- [enzyme] hydrolysis

~~~ ann
Phosphorylation of AKT2 was downregulated.
T1 Conversion 0 15 Phosphorylation
T2 GGPs 19 23 AKT
T3 Negative_regulation 28 41 downregulated
E1 Conversion:T1 Theme:T2
E2 Negative_regulation:T3 Theme:E1
~~~
~~~ ann
Phospho-S6
T1 Conversion 0 7 Phospho
T2 GGPs 8 10 S6
T3 GGPs 0 10 Phospho-S6
E1 Conversion:T1 Theme:T2 Product:T3
~~~
~~~ ann
luciferase activity
T1 GGPs 0 10 luciferase
T2 Conversion 0 19 luciferase activity
E1 Conversion:T2
~~~

Arguments:

*Theme* for this event must be molecules whose covalent bonds are converted: [GGPs](), [Organic_compound_other]() or possibly [Pharmacological_substance]().

*Product* (optional; zero or more) indicates the molecule(s) that could be produced by the 'Conversion' event: [GGPs]() or [Organic_compound_other](). 

*AtLoc* indicates the section where the target molecules, to which the 'Conversion' occurs, are located : [Anatomical_entity](), [Cell](), [Cell_component]() and [Entity Property]().

<!---
The *atLoc*, *fromLoc* and *toLoc* for this event must be [Subject](), [Anatomical_entity](), [Cell](), [Cell_component]() and [Entity Property]().

The other arguments, such as *Cause*, *Theme*, *Participant*, and *Product*, for this event can be any entities or events.
--->

<!--details-->



