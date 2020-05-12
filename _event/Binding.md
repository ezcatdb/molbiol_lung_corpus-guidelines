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

However, interaction between molecules and [Cell]()/[Cell_component]() will be categorized in [Localization]().

Interaction between [Cell]()/[Cell_component]() will be categorized in [Cellular_process]().

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

Arguments:

*Theme* (optional; multiple) indicates molecular entities ([GGPs](), [Organic_compound_other](), [Pharmacological_substance](), [Inorganic_compound](), etc.)

*atLoc* (optional; zero or one) indicates the location where `Binding` event occurs: [Cell_component](), [Cell]() or [Anatomical_entity]().

<!--details-->
