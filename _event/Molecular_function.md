---
layout: entry
title: "Molecular_function"
category: "Molecular function"
shortdef: "Processes on molecular level"
order: 70
---

This event is based on the <a href="http://www.nactem.ac.uk/meta-knowledge/">GENIA-Meta-knowledge corpus</a> at <a href="http://www.nactem.ac.uk/">NaCTeM</a>.

This event describes the biological events on the molecular levels.

The following words/phrases can be triggers of this event:

- mutation (if naturally occured) (UMLS ID:C0026882)
  - deletion [mutation] (UMLS ID:C1511760)
- polymorphism (genetic polymorphism) (UMLS ID:C0032529)

- molecular mechanism (UMLS; C0678659)
- biochemical mechanism (UMLS; C0678659)
- [enzyme] activity (UMLS ID:C0243102)
  - catalytic activity (UMLS ID:C0243102)
- biosynthesis (anabolism, or biosynthetic process) (UMLS; C0220781)
- degradation (catabolism, or breakdown) (UMLS; C0699900)
- chemoattractant activity (UMLS; C1149381) (If chemotaxis, [Cellular_process]())
- immunoreactivity (UMLS; C0597879) (If it meant immunoassay, [Method cue]())
- (indirect) interaction (UMLS; C1148560 (originally for Molecular function))(in case where it is difficult to determine whether it is a direct interaction between molecules [Binding]())

~~~ ann
Infulence of methylenetetrahydrofolate reductase C677T polymorphism on the risk of lung cancer
T1 GGPs 13 54 methylenetetrahydrofolate reductase C677T
T2 Molecular_function 55 67 polymorphism
T3 Disorder 83 94 lung cancer
T4 Anatomical_entity 83 87 lung
T5 Regulation 0 9 Infulence
T6 Genetic_info 49 54 C677T
E1 Molecular_function:T2 Product:T1
E2 Regulation:T5 Cause:E1 Theme:T3
~~~
~~~ ann
Studies on MTHFR C677T polymorphism and lung cancer ... The C677T polymorphism was correlated with a risk of NSCLC.
T1 GGPs 11 22 MTHFR C677T
T2 Molecular_function 23 35 polymorphism
T3 Disorder 40 51 lung cancer
T4 GGPs 60 65  C677T
T5 Molecular_function 66 78 polymorphism
T6 Disorder 109 114 NSCLC
T7 Speculation 0 7 Studies
T8 Correlation 83 93 correlated
T9 Genetic_info 17 22  C677T
T10 Genetic_info 60 65  C677T
E1 Molecular_function:T2 Product:T1 Cue:T7
E2 Molecular_function:T5 Product:T4
E3 Correlation:T8 Theme:E2 Theme2:T6
A1 Speculated E1
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

The *Cause* for this event is entities/events, which cause this event, whereas the *Theme* for this event is entities/events, which are targets of this events. 
Usually, the *Theme* for this event is molecular entities.
- [GGPs]()
- [Pharmacological_substance]()
- [Organic_compound_other]()
- [Inorganic_compound]()

The *Participant* is molecular entities, which are involved in this event.

The *Product* is molecular entities, which is produced by this event.

The *atLoc* argument (optional) indicates the location at which this event occurs. 
The *fromLoc* (optional) indicates the location from which this event starts, whereas the *toLoc* (optional) indicates the location to which this event proceeds.

The *atLoc*, *fromLoc* and *toLoc* for this event can be
- [Cell](),
- [Cell_component]()

The *disorder* (optional) indicates the [Disorder]() for which the `Molecular function` event occurs.

The *Cue* argument (optional) is cues, such as [Negation cue](), [Speculation cue]() or [Method cue]().


<!--details-->
