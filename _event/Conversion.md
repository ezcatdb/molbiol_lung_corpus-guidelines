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

- *phosphorylate*, *phosphorylates*, *phosphorylated*, *phosphorylation(s)* (UMLS ID:C0031715)
  - autophosphorylation (UMLS ID:C0813988)
  - self-phosphorylation (UMLS ID:C0813988)
  - protein phosphorylation (UMLS ID:C0031715)
  - tyrosine autophosphorylation (UMLS ID:C0813988)
  - tyrosine phosphorylation (UMLS ID:C0031715)
  - hyperphosphorylation (UMLS ID:C0031715)
- *dephosphorylate*, *dephosphorylates*, *dephosphorylated*, *dephosphorylation* (UMLS ID:C3160734)
- *methylate*, *methylates*, *methylated*, *methylation* (UMLS ID:C0025723)
- *acetylate*, *acetylates*, *acetylated*, *acetylation* (UMLS ID:C0001038)
- *carboxymethylate*, *carboxymethylates*, *carboxymethylated*, *carboxymethylation* (UMLS ID:C0596262)
- *cleave*, *cleaves*, *cleaved*, *cleavage* (UMLS ID:C0596311)
  - *degrade*, *degrades*, *degraded*, *degradation*  (UMLS ID:C0596311)
- *cross-link*, *cross-links*, *cross-linked*, *cross-linking* (UMLS ID:C0332220)


The following ones can also be trigger words:
- [enzyme] hydrolysis  (UMLS ID:C0020291)
- proteolysis (UMLS ID:C0597304)

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
T4 Inorganic_compound 0 7 Phospho
E1 Conversion:T1 Theme:T2 Product:T3
R1 part_of Arg1:T4 Arg2:T3
~~~
~~~ ann
p-S6
T1 Conversion 0 2 p-
T2 GGPs 2 4 S6
T3 GGPs 0 4 p-S6
T4 Inorganic_compound 0 2 p-
E1 Conversion:T1 Theme:T2 Product:T3
R1 part_of Arg1:T4 Arg2:T3
~~~
~~~ ann
MMP-7 degrades elastin, generating elastin fragments.
T1 GGPs 0 5 MMP-7
T2 Conversion 6 14 degrades
T3 GGPs 15 22 elastin
T4 Positive_regulation 24 34 generating
T5 GGPs 35 52 elastin fragments
E1 Conversion:T2 Cause:T1 Theme:T3 Product:T5
E2 Positive_regulation:T4 Cause:E1 Theme:T5
R1 part_of Arg1:T5 Arg2:T3
~~~
~~~ ann
Extracellular matrix cross-linking enzymes
T1 Anatomical_entity 0 20 Extracellular matrix
T2 Conversion 21 34 cross-linking
T3 GGPs 0 42 Extracellular matrix cross-linking enzymes
E1 Conversion:T2 Theme:T1 Cause:T3
~~~

Arguments:

*Theme* for this event must be mostly molecular entities whose covalent bonds are converted: [GGPs](), [Organic_compound_other]() or possibly [Pharmacological_substance](). 
However, other entities such as [Cell](), [Cell_component]() and [Anatomical_entity](), which are composed of molecules to be converted, can also be *Theme* for this event.

*Product* (optional; zero or more) indicates the molecule(s) that could be produced by the 'Conversion' event: [GGPs]() or [Organic_compound_other](). 

*atLoc* indicates the section where the target molecules, to which the 'Conversion' occurs, are located : [Anatomical_entity](), [Cell](), [Cell_component]() and [Entity Property]().

<!---
The *atLoc*, *fromLoc* and *toLoc* for this event must be [Subject](), [Anatomical_entity](), [Cell](), [Cell_component]() and [Entity Property]().

The other arguments, such as *Cause*, *Theme*, *Participant*, and *Product*, for this event can be any entities or events.
--->

<!--details-->



