---
layout: entry
title: "Binding"
category: "Biological process"
shortdef: "Non-covalnet interaction between molecules"
order: 21
---

<!--
This event is based on the <a href="http://www.nactem.ac.uk/meta-knowledge/">GENIA-Meta-knowledge corpus</a> at <a href="http://www.nactem.ac.uk/">NaCTeM</a>.
-->

This event describes "non-covalent interaction" between molecules.

The following words/phrases can be triggers of this event:

- *interact*, *interacted*, *interacts*, *interaction*

~~~ ann
CTGF/TGF-beta interaction
T1 GGPs 0 4 CTGF
T2 GGPs 5 13 TGF-beta
T3 Binding 14 25 interaction
E1 Binding:T3 Theme:T1 Theme2:T2
~~~

Arguments:

*Theme* (optional; multiple) indicates molecular entities ([GGPs](), [Organic_compound_other](), [Pharmacological_substance](), etc.)

<!--details-->
