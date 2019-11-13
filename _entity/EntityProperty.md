---
layout: entry
title: "Entity Property"
shortdef: "various technical terms for lung diseases"
order: 100
---

{% comment %}TODO: entity type introduction {% endcomment %}

<!-- details -->

Technical terms, which are not any other Entity information, can be categorized into this category, 'Entity Property'.

The following words/phrases for [Disorder]() can be tentatively annotated for this category.
- stage I
- stage II
- stage IIIB
- stage IV
- stage IIIB/IV
- stable
- severe
- grade 1

~~~ ann
stage I lung cancer
T1 Entity_Property 0 7 stage I
T2 Disorder 8 19 lung cancer
~~~
~~~ ann
chemo-naïve stage IIIB/IV NSCLC
T1 Entity_Property 12 25 stage IIIB/IV
T2 Disorder 26 31 NSCLC
~~~

The following words/phrases for [Cell]() and [GGPs]() can be tentatively annotated for this category.

- null (UMLS ID:C0205160)
- (-) (UMLS ID:C0205160)
- (+) (UMLS ID:C1446409)

~~~ ann
CD4(+)CD28(null) T-cells
T1 GGPs 0 3 CD4
T2 Entity_Property 3 6 (+)
T3 GGPs 6 10 CD28
T4 Entity_Property 10 16 (null)
T5 Cell 17 24 T-cells
T6 Cell 0 24 CD4(+)CD28(null) T-cells
T7 Cell 0 6;16 24 CD4(+) T-cells
~~~


