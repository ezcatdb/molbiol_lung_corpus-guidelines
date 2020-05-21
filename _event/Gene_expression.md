---
layout: entry
title: "Gene_expression"
category: "Molecular function"
shortdef: "Gene expression"
order: 73
---

<!---
This event is based on the <a href="http://www.nactem.ac.uk/meta-knowledge/">GENIA-Meta-knowledge corpus</a> at <a href="http://www.nactem.ac.uk/">NaCTeM</a>.
--->

This event describes *gene expression* (UMLS ID:C0017262), which can be either *transcription* (UMLS ID:C0040649) or *translation* (UMLS ID:C1519614), or both the events.

The following words/phrases can be triggers of *transcription*  (UMLS ID:C0040649):

- *transcribe*; *transcribes*; *transcribed*; *transcription*
- *[mRNA] expression*
- *[mRNA] production*
- *[mRNA] synthesis*

The following words/phrases can be triggers of *translation* (UMLS ID:C1519614):

- *translate*; *translates*; *translated*; *translation*
- *[protein] biosynthesis*
- *[protein] formation*
- *[protein] expression*
- *[protein] synthesis*
- *protein level [increased/decreased]*

<!-- The following phrase was removed from example phrases for translation
- *[protein] level (increased)*
-->

The following words/phrases can be triggers of *gene expression* (UMLS ID:C0017262), if it is not clear whether *transcription* or *translation* is stated.

- *co-express*; *co-expresses*; *co-expressed*; *co-expression*
- *coexpress*; *coexpresses*; *coexpressed*; *coexpression*
- *hyperexpress*; *hyperexpresses*; *hyperexpressed*; *hyperexpression*
- *express*; *expresses*; *expressed*; *expression*
- *overexpress*; *overexpresses*; *overexpressed*; *overexpression*
- *produce*; *produces*; *produces*; *production*,
- *synthesize*; *synthesizes*; *synthesized*; *synthesis*
- *up-expression*

~~~ ann
LOXL1/LOXL2 gene expression and protein levels were increased.
T1 GGPs 0 5 LOXL1
T2 GGPs 6 11 LOXL2
T5 Gene_expression 12 27 gene expression
T6 Gene_expression 12 27 gene expression
T7 Gene_expression 32 46 protein levels
T8 Gene_expression 32 46 protein levels
T9 Positive_regulation 52 61 increased
T10 Positive_regulation 52 61 increased
T11 Positive_regulation 52 61 increased
T12 Positive_regulation 52 61 increased
E1 Gene_expression:T5 Theme:T1
E2 Gene_expression:T6 Theme:T2
E3 Gene_expression:T7 Theme:T1
E4 Gene_expression:T8 Theme:T2
E5 Positive_regulation:T9 Theme:E1
E6 Positive_regulation:T10 Theme:E2
E7 Positive_regulation:T11 Theme:E3
E8 Positive_regulation:T12 Theme:E4
~~~
~~~ ann
Serum level of KL-6 was elevated.
T1 Anatomical_entity 0 5 Serum
T2 Gene_expression 6 11 level
T3 GGPs 15 19 KL-6
T4 Positive_regulation 24 32 elevated
E1 Gene_expression:T2 Theme:T3 atLoc:T1
E2 Positive_regulation:T4 Theme:E1
~~~
~~~ ann
T-cells lose surface expression of CD28.
T1 Cell 0 7 T-cells
T2 Negative_regulation 8 12 lose
T3 Cell_component 13 20 surface
T4 Gene_expression 21 31 expression
T5 GGPs 35 39 CD28
E1 Negative_regulation:T2 Theme:E2 atLoc:T1
E2 Gene_expression:T4 Theme:T5
R1 part_of Arg1:T3 Arg2:T1
~~~

<!--
~~~ ann
LOXL1/LOXL2 gene expression and protein levels were increased.
T1 GGPs 0 5;12 16 LOXL1 gene
T2 GGPs 6 16 LOXL2 gene
T3 GGPs 0 5;32 39 LOXL1 protein
T4 GGPs 6 11;32 39 LOXL2 protein
T5 Gene_expression 12 27 gene expression
T6 Gene_expression 12 27 gene expression
T7 Gene_expression 32 46 protein levels
T8 Gene_expression 32 46 protein levels
T9 Positive_regulation 52 61 increased
T10 Positive_regulation 52 61 increased
T11 Positive_regulation 52 61 increased
T12 Positive_regulation 52 61 increased
E1 Gene_expression:T5 Theme:T1
E2 Gene_expression:T6 Theme:T2
E3 Gene_expression:T7 Theme:T3
E4 Gene_expression:T8 Theme:T4
E5 Positive_regulation:T9 Theme:E1
E6 Positive_regulation:T10 Theme:E2
E7 Positive_regulation:T11 Theme:E3
E8 Positive_regulation:T12 Theme:E4
~~~
-->

Arguments:

*Theme* for this event must be genes/gene products: [GGPs]().

*atLoc* indicates the section where the this event occurs : [Anatomical_entity](), [Cell](), [Cell_component]() and [Entity Property]().

<!---
The *atLoc*, *fromLoc* and *toLoc* for this event must be [Subject](), [Anatomical_entity](), [Cell](), [Cell_component]() and [Entity Property]().

The other arguments, such as *Cause*, *Theme*, *Participant*, and *Product*, for this event can be any entities or events.
--->

<!--details-->



