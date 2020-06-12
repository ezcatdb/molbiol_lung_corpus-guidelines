---
layout: entry
title: "Binding"
category: "Biological process"
shortdef: "Non-covalent interaction between molecules"
order: 21
---

<!--
This event is based on the <a href="http://www.nactem.ac.uk/meta-knowledge/">GENIA-Meta-knowledge corpus</a> at <a href="http://www.nactem.ac.uk/">NaCTeM</a>.
-->

This event describes "non-covalent interaction" between molecules, such as [GGPs](), [Organic_compound_other](), [Pharmacological_substance]() and [Inorganic_compound]().
 Moreover, this event is opposite to [Dissociation]().

However, covalent bond formation will be categorized in [Conversion]().

Moreover, interaction between molecules and [Cell]()/[Cell_component]() will be categorized in [Localization]().

Interaction between [Cell]()/[Cell_component]() will be categorized in [Cellular_process]().

UMLS ID for this event; Molecular Interaction Process (UMLS; C1167622).

The following words/phrases can be triggers of this event:

- *adhere*; *adheres*; *adhered*; *adhesion*
- *affinity*; *affinities*
- *assemble*; *assembles*; *assembled*; *assembly*
- *associate*; *associates*; *associated*; *association*
- *attach*; *attaches*; *attached*; *attachment*
- *bind*; *binds*; *bound*; *binding*
- *conjugate*; *conjugates*; *conjugated*
- *couple*; *couples*; *coupled*; *coupling*
- *dimer*; *dimers*
- *dimerize*; *dimerizes*; *dimerized*; *dimerization*
- *dock*; *docks*; *docked*; *docking*
- *form [a] complex*; *complex formation*
- *interact*, *interacted*, *interacts*, *interaction*
- *oligomerize*; *oligomerizes*; *oligomerized*; *oligomerization*
- *polymerize*; *polymerizes*; *polymerized*; *polymerization*

~~~ ann
CTGF/TGF-beta interaction
T1 GGPs 0 4 CTGF
T2 GGPs 5 13 TGF-beta
T3 Binding 14 25 interaction
E1 Binding:T3 Theme:T1 Theme2:T2
~~~
~~~ ann
Interaction of CXCL12 and CXC receptor 4
T1 Binding 0 11 Interaction
T2 GGPs 15 21 CXCL12
T3 GGPs 26 40 CXC receptor 4
E1 Binding:T1 Theme:T2 Theme2:T3
~~~
~~~ ann
TNFSF14 binds to HVEM on T lymphocytes.
T1 GGPs 0 7 TNFSF14
T2 Binding 8 13 binds
T3 GGPs 17 21 HVEM
T4 Cell 25 38 T lymphocytes
E1 Binding:T2 Theme:T1 Theme2:T3 atLoc:T4
~~~
~~~ ann
ERK/GLI-1 complex formation
T1 GGPs 0 3 ERK
T2 GGPs 4 9 GLI-1
T3 Binding 10 27 complex formation
E1 Binding:T3 Theme:T1 Theme2:T2
~~~
~~~ ann
ERK and GLI-1 form a complex.
T1 GGPs 0 3 ERK
T2 GGPs 8 13 GLI-1
T3 Binding 14 28 form a complex
E1 Binding:T3 Theme:T1 Theme2:T2
~~~

Arguments:

*Theme* (optional; multiple) indicates molecular entities ([GGPs](), [Organic_compound_other](), [Pharmacological_substance](), [Inorganic_compound](), etc.)

*atLoc* (optional; zero or one) indicates the location where `Binding` event occurs: [Cell_component](), [Cell]() or [Anatomical_entity]().

<!--details-->
