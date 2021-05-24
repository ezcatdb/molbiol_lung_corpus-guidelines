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
- stage I (UMLS; C0441766)
- stage II (UMLS; C0441767)
- stage III (UMLS; C0441771)
- stage IIIB (UMLS; C0456599)
- stage IV (UMLS; C0441772)
- stage IIIB/IV 
- stable
- severe
- grade 1
- chronic phase (UMLS; C0457343)
- chronically progressive phase
- subacutely progressive phase
- subacute phase
- stable phase
- inflammatory phase

<!---
~~~ ann
stage I lung cancer
T1 Entity_Property 0 7 stage I
T2 Disorder 8 19 lung cancer
T3 Disorder 0 19 stage I lung cancer
R1 member_of Arg1:T3 Arg2:T2
~~~
~~~ ann
chemo-naïve stage IIIB/IV NSCLC
T1 Entity_Property 12 22 stage IIIB
T2 Entity_Property 12 18;23 25 stage IV
T3 Disorder 26 31 NSCLC
T4 Disorder 12 22;25 31 stage IIIB NSCLC
T5 Disorder 12 18;23 31 stage IV NSCLC
R1 member_of Arg1:T4 Arg2:T3
R2 member_of Arg1:T5 Arg2:T3
~~~
--->


The following words/phrases, which are used to indicate so-called *cell marker expression* or *immunophenotyping*, for [Cell]() and [GGPs]() can be tentatively annotated for this category.

- null (UMLS ID:C0205160)
- (-) (UMLS ID:C0205160)
- (+) (UMLS ID:C1446409)

In the following example, 'CD4(+) T-cells' have got a UMLS ID (C0039215), whereas 'CD4(+)CD28(null) T-cells' do not have an ID, so that [member_of]() relation is annotated to indicate their relationships.
~~~ ann
CD4(+)CD28(null) T-cells
T1 GGPs 0 3 CD4
T2 Entity_Property 3 6 (+)
T3 GGPs 6 10 CD28
T4 Entity_Property 10 16 (null)
T6 Cell 0 24 CD4(+)CD28(null) T-cells
T7 Cell 0 6;16 24 CD4(+) T-cells
R1 member_of Arg1:T6 Arg2:T7
~~~

The following words related to cell cycle (UMLS; C0007586) can be annotated in this category: (see <a href="https://en.wikipedia.org/wiki/Cell_cycle">Cell cycle</a>)
- cell cycle(UMLS; C0007586)
  - G1 phase (UMLS; C0079395)
  - G1/S [transition] checkpoint (UMLS; C1517340)
  - S phase (UMLS; C0080129)
  - G2 phase (UMLS; C0079396)
  - G2/M [transition] checkpoint (UMLS; C3549430)
  - M phase (UMLS; C0007591)
    - prophase 
    - prometaphase
    - metaphase 
    - anaphase 
    - telophase
