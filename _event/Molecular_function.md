---
layout: entry
title: "Molecular_function"
category: "Molecular process"
shortdef: "Processes on molecular level"
order: 70
---

This event is based on the <a href="http://www.nactem.ac.uk/meta-knowledge/">GENIA-Meta-knowledge corpus</a> at <a href="http://www.nactem.ac.uk/">NaCTeM</a>.

This event describes biological events at molecular levels.

The following words/phrases can be triggers of this event:

- mutation (if naturally occured) (UMLS ID:C0026882)
- polymorphism (genetic polymorphism) (UMLS ID:C0032529)

- [enzyme] activity (UMLS ID:C0243102)
  - catalytic activity (UMLS ID:C0243102)

~~~ ann
Infulence of methylenetetrahydrofolate reductase C677T polymorphism on the risk of lung cancer
T1 GGPs 13 54 methylenetetrahydrofolate reductase C677T
T2 Molecular_function 55 67 polymorphism
T3 Disorder 83 94 lung cancer
T4 Anatomical_entity 83 87 lung
E1 Molecular_function:T2 Product:T1
~~~
~~~ ann
Studies on MTHFR C677T polymorphism and lung cancer ... The C677T polymorphism was correlated with a risk of NSCLC.
T1 GGPs 11 22 MTHFR C677T
T2 Molecular_function 23 35 polymorphism
T3 Disorder 40 51 lung cancer
T4 GGPs 60 65  C677T
T5 Molecular_function 66 78 polymorphism
T6 Disorder 109 114 NSCLC
E1 Molecular_function:T2 Product:T1
E2 Molecular_function:T5 Product:T1
R1 Coreference Arg1:T4 Arg2:T1
~~~
~~~ ann
MMP-7 activity in regard to elastin degradation
T1 GGPs 0 5 MMP-7
T2 Molecular_function 6 14 activity
T3 GGPs 28 35 elastin
T4 Conversion 36 47 elastin 
E1 Molecular_function:T2 Cause:T1
E2 Conversion:T4 Theme:T3 Cause:E1
~~~

Arguments:

The *atLoc*, *fromLoc* and *toLoc* for this event must be
- [Cell](),
- [Cell_component]()
- [GGPs]()
- [Pharmacological_substance]()
- [Organic_compound_other]()
- [Inorganic_compound]()
- [Entity Property]()

The other arguments, such as *Cause*, *Theme*, *Participant*, and *Product*, for this event can be molecular entities or events.


<!--details-->



