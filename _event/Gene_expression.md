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
- *[protein] level (increased)*

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

Arguments:

*Theme* for this event must be genes/gene products: [GGPs]().

*AtLoc* indicates the section where the this event occurs, are located : [Anatomical_entity](), [Cell](), [Cell_component]() and [Entity Property]().

<!---
The *atLoc*, *fromLoc* and *toLoc* for this event must be [Subject](), [Anatomical_entity](), [Cell](), [Cell_component]() and [Entity Property]().

The other arguments, such as *Cause*, *Theme*, *Participant*, and *Product*, for this event can be any entities or events.
--->

<!--details-->


