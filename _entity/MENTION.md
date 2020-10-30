---
layout: entry
title: "MENTION"
shortdef: "other technical terms for mutation info"
order: 101
---

{% comment %}TODO: entity type introduction {% endcomment %}

<!-- details -->

Technical terms for mutation information, which cannot be included in [GGPs](), can be categorized into this category, 'MENTION'.

~~~ ann
1G/2G MMP-1 and 5A/6A MMP-3 SNPs
T1 MENTION 0 5 1G/2G
T2 GGPs 6 11 MMP-1
T3 MENTION 16 21 5A/6A
T4 GGPs 22 27 MMP-3
T5 Molecular_function 28 32 SNPs
T6 Molecular_function 28 32 SNPs
E1 Molecular_function:T5 Theme:T2 Product:T1
E2 Molecular_function:T6 Theme:T4 Product:T3
~~~
