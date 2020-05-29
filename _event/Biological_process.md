---
layout: entry
title: "Biological_process"
category: "Biological process"
shortdef: "Biological process beyond cellular/molecular levels"
order: 10
---

This event is based on the <a href="http://www.nactem.ac.uk/meta-knowledge/">GENIA-Meta-knowledge corpus</a> at <a href="http://www.nactem.ac.uk/">NaCTeM</a>.

The category of this event will be difficult to be classified into other biological events, such as [Cellular_process]() and [Molecular_function]().

The following words/phrases can be triggers of this event:

- organogenesis (UMLS; C0242290)
  - angiogenesis [process] (UMLS; C0302600)
- fibrogenesis (UMLS; C0596570)
  - fibrotic response
  - profibrotic response
- pathogenesis (UMLS; C0699748)
  - immunopathogenesis
  - etiopathogenesis
- pathophysiological mechanism
- acute exacerbation (UMLS; C0743630)
- angiostasis
- resistance (UMLS; C1514892)
- homeostasis (UMLS; C0019868)
- sensitivity (UMLS; C2349185)
- remodeling
- cilium biogenesis (UMLS; C1155941)
- cilium assembly (UMLS; C1155941)
- inflammatory response (UMLS; C1155266)
- immune response [process] (UMLS; C0301872)

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
pathogenesis of IPF
T1 Biological_process 0 12 pathogenesis
T2 Disorder 16 19 IPF
E1 Biological_process:T1 Theme:T2
~~~

Arguments:

The *atLoc*, *fromLoc* and *toLoc* for this event must be [Subject](), [Anatomical_entity](), [Cell](), [Cell_component]() and [Entity Property]().

The other arguments, such as *Cause*, *Theme*, *Participant*, and *Product*, for this event can be any entities or events.


<!--details-->



