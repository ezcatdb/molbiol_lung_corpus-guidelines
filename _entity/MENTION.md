---
layout: entry
title: "MENTION"
shortdef: "other technical terms for mutation info"
order: 101
---

{% comment %}TODO: entity type introduction {% endcomment %}

<!-- details -->

Technical terms for mutation information, which cannot be included in [GGPs](), can be categorized into this category, 'MENTION'.
The following words must be typical mutation info:
 - 1G/2G
 - rs1800925(C/T)
 - rs1800925 T allele
 - CC genotype
 - genotypes CT and TT
 
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
~~~ ann
SNP type 5A/6A at position -1612/-1617 of the MMP-3 gene
T1 Molecular_function 0 3 SNP
T2 MENTION 9 38 5A/6A at position -1612/-1617
T3 GGPs 45 56 MMP-3 gene
E1 Molecular_function:T1 Theme:T3 Product:T2
~~~
