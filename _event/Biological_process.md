---
layout: entry
title: "Biological_process"
category: "Biological process"
shortdef: "Biological process beyond cellular/molecular levels"
order: 10
---

This event is based on the <a href="http://www.nactem.ac.uk/meta-knowledge/">GENIA-Meta-knowledge corpus</a> at <a href="http://www.nactem.ac.uk/">NaCTeM</a>.

This event will be difficult to be classified into the other biological events, such as [Cellular_process]() and [Molecular_function](), as it is on higher level than the other events.

The following words/phrases can be triggers of this event:

- organogenesis (UMLS; C0242290)
  - angiogenesis [process] (UMLS; C0302600)
- fibrogenesis (UMLS; C0596570)
  - fibrotic response
  - profibrotic response
- pathogenesis (UMLS; C0699748)
  - immunopathogenesis
  - etiopathogenesis
  - development [of some disease]
- pathophysiological mechanism
- acute exacerbation (UMLS; C0743630)
- angiostasis (UMLS; C3179230)
- resistance (UMLS; C1514892)
- homeostasis (UMLS; C0019868)
- sensitivity (UMLS; C2349185)
- [tissue] remodeling (UMLS; C1820201)
- cilium biogenesis (UMLS; C1155941)
- cilium assembly (UMLS; C1155941)
- inflammatory response (UMLS; C1155266)
- immune response [process] (UMLS; C0301872)
- injury
  - tissue damage (UMLS; C0010957) 
  - scarring (UMLS; C0008767 (for Cicatrization))
- adverse event (UMLS; C0877248)

~~~ ann
matrix remodeling phase
T1 Anatomical_entity 0 6 matrix
T2 Biological_process 7 17 remodeling
E1 Biological_process:T2 Theme:T1
~~~
~~~ ann
lung fibrogenesis
T1 Anatomical_entity 0 4 lung
T2 Biological_process 5 17 fibrogenesis
E1 Biological_process:T2 Theme:T1
~~~
~~~ ann
Markers of fibrogenesis, including collagen and CTGF were evaluated by measuring mRNA level using RT-PCR.
T1 GGPs 0 7 Markers
T2 Biological_process 11 23 fibrogenesis
T3 GGPs 35 43 collagen
T4 GGPs 48 52 CTGF
T5 Speculation_cue 58 67 evaluated
T6 Speculation_cue 71 80 measuring
T7 Gene_expression 81 91 mRNA level
T8 Gene_expression 81 91 mRNA level
T9 Method_cue 98 104 RT-PCR
E1 Biological_process:T2 Participant:E2 Participant2:E3 cue:T5
E2 Gene_expression:T7 Theme:T3 Cue:T6 Cue2:T9
E3 Gene_expression:T8 Theme:T4 Cue:T6 Cue2:T9
R1 member_of Arg1:T3 Arg2:T1
R2 member_of Arg1:T4 Arg2:T1
A1 Speculated E1
A2 Speculated E2
A3 Speculated E3
~~~
~~~ ann
pathogenesis of IPF
T1 Biological_process 0 12 pathogenesis
T2 Disorder 16 19 IPF
E1 Biological_process:T1 Theme:T2
~~~
~~~ ann
Extracellular matrix remodeling due to the collagen crosslinking
T1 Anatomical_entity 0 20 Extracellular matrix
T2 Biological_process 21 31 remodeling
T3 GGPs 43 51 collagen
T4 Conversion 52 64 crosslinking
E1 Biological_process:T2 Theme:T1 Cause:E2
E2 Conversion:T4 Theme:T3
~~~
~~~ ann
epithelial injury
T1 Cell 0 10 epithelial
T2 Biological_process 11 17 injury
E1 Biological_process:T2 Theme:T1
~~~
~~~ ann
injured lung
T1 Biological_process 0 7 injured
T2 Anatomical_entity 8 12 lung
E1 Biological_process:T1 Theme:T2
~~~
~~~ ann
In the murine model of schistosomiasis, IL-13 has emerged as a central mediator of chronic infection-induced liver pathology.
T1 Subject 7 19 murine model
T2 Disorder 23 38 schistosomiasis
T3 GGPs 40 45 IL-13
T4 Positive_regulation 71 79 mediator
T5 Disorder 83 100 chronic infection
T6 Positive_regulation 101 108 induced
T7 Anatomical_entity 109 114 liver
T8 Biological_process 115 124 pathology
E1 Positive_regulation:T4 Theme:E3 Cause:T3 disorder:T2
E2 Positive_regulation:T6 Theme:E3 Cause:T5
E3 Biological_process:T8 Theme:T7
R1 Subject_Disorder Arg1:T1 Arg2:T2
~~~

Arguments:

The *atLoc*, *fromLoc* and *toLoc* arguments for this event must be [Subject](), [Anatomical_entity](), [Cell](), and [Cell_component](), which are the locations where this event occurs. 
The *atLoc* argument indicates the location at which this event occurs. 
The *fromLoc* indicates the location from which this event starts, whereas the *toLoc* indicates the location to which this event proceeds.

The other arguments, such as *Cause*, *Theme*, *Participant*, and *Product*, for this event can be any entities or events.

The *Cause* for this event is entities/events, which cause this event, whereas the *Theme* for this event is entities/events, which are targets of this events. 

The *Participant* is entities/events, which are involved in this event.

The *Product* is entities/events, which is produced by this event.

The *disorder* argument is [Disorder]().

The *Cue* argument is cues, such as [Negation cue](), [Speculation cue]() or [Method cue]().


<!--details-->



