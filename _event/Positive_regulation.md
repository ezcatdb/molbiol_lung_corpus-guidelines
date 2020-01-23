---
layout: entry
title: "Positive_regulation"
category: "Biological process"
shortdef: "Positive regulation"
order: 22
---

This event is based on the <a href="http://www.nactem.ac.uk/meta-knowledge/">GENIA-Meta-knowledge corpus</a> at <a href="http://www.nactem.ac.uk/">NaCTeM</a>.

This event describes "activation/up-regulation" event (UMLS ID:C1879547).

The following words/phrases can be triggers of this event:

- *activate*; *activates*; *activated*; *activation*
- *cause*; *causes*; *caused*
- *depend*; *depends*; *depended*; *dependent*
- *elevate*; *elevates*; *elevated*; *elevation*
- *enhance*; *enhances*; *enhanced*
- *increase*; *increases*; *increased*
- *induce*; *induces*; *induced*; *induction*
- *mediate*; *mediates*; *mediated*
- *necessary*
- *positively regulate*; *positively regulates*; *positively regulated*; *positive regulation*
- *promote*; *promotes*; *promoted*; *promotion*
- *require*; *requires*; *required*
- *stimulate*; *stimulates*; *stimulated*; *stimulation*
- *transactivate*; *transactivates*; *transactivated*; *transactivation*
- *trigger*; *triggers*; *triggered*
- *up-regulate*; *up-regulates*; *up-regulated*; *up-regulation*
- *[in] response [to]*

Regarding the trigger word, '*mediate*', it is used differently from other trigger words, such as '*activate*' and '*stimulate*', as follows:

*A mediates B and C*

Here, this sentence may indicate the two following relationships:
- *A => B*
- *A => C*

('=>' indicates 'positive regulation')

~~~ ann
Beta-arrestin isoform 1 mediate desensitization and internalization.
T2      GGPs 0 23   Beta-arrestin isoform 1
T8      Positive_regulation 24 31      mediate
T9      Negative_regulation 32 47     desensitization
T10     Localization 52 67  internalization
E7      Positive_regulation:T8 Cause:T2 Theme:E9
E8      Negative_regulation:T9 Theme:T6
E9      Localization:T10 Theme:T6
E11     Positive_regulation:T8 Cause:T2 Theme:E8
~~~

The following sample sentence indicates:
- CXCL12 => phosphorylation of SMAD3
~~~ ann
CXCL12-mediated SMAD3 phosphorylation
T1 GGPs 0 6 CXCL12
T2 GGPs 16 21 SMAD3
T3 Positive_regulation 7 15 mediated
T4 Conversion 22 37 phosphorylation
E1 Positive_regulation:T3 Cause:T1 Theme:E2
E2 Conversion:T4 Theme:T2
~~~

The following sample sentence indicates:
- CXCL12 => expression of CTGF
- *SMAD3 => expression of CTGF*
~~~ ann
SMAD3 mediates CXCL12-stimulated CTGF expression.
T1 GGPs 0 5 SMAD3
T2 GGPs 15 21 CXCL12
T3 GGPs 33 37 CTGF
T4 Positive_regulation 6 14 mediates
T5 Positive_regulation 22 32 stimulated
T6 Gene_expression 38 49 expression
E1 Positive_regulation:T4 Cause:T1 Theme:E3
E2 Positive_regulation:T5 Cause:T2 Theme:E3
E3 Gene_expression:T6 Theme:T3
~~~

Considering the sample sentences, 2 & 3, the conclusion is:

CXCL12 => phosphorylation of SMAD3 => expression of CTGF

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

~~~ ann
Protein levels were increased in both IPF and HP for MMP-8, MMP-9, and protein-C, whereas VEGF was decreased compared with control.
T1 Disorder 38 41 IPF
T2 Disorder 46 48 HP
T3 GGPs 53 58 MMP-8
T4 GGPs 60 65 MMP-9
T5 GGPs 71 80 protein-C
T6 GGPs 90 94 VEGF
T7 Gene_expression 0 14 Protein levels
T8 Gene_expression 0 14 Protein levels
T9 Gene_expression 0 14 Protein levels
T10 Gene_expression 0 14 Protein levels
T11 Positive_regulation 20 29 increased
T12 Positive_regulation 20 29 increased
T13 Positive_regulation 20 29 increased
T14 Negative_regulation 99 108 decreased
T15 Subject 38 41 IPF
T16 Subject 46 48 HP
T17 Subject 123 130 control 
E1 Gene_expression:T7 Theme:T3
E2 Gene_expression:T8 Theme:T4
E3 Gene_expression:T9 Theme:T5
E4 Gene_expression:T10 Theme:T6
E5 Positive_regulation:T11 Theme:E1 Disorder:T1 Disorder2:T2
E6 Positive_regulation:T12 Theme:E2 Disorder:T1 Disorder2:T2
E7 Positive_regulation:T13 Theme:E3 Disorder:T1 Disorder2:T2
E8 Negative_regulation:T14 Theme:E4 Disorder:T1 Disorder2:T2
R1 Subject_Disorder Arg1:T15 Arg2:T1
R2 Subject_Disorder Arg1:T16 Arg2:T2
~~~
~~~ ann
Protein levels were increased in both IPF and HP for MMP-8, MMP-9, and protein-C, whereas VEGF was decreased compared with control.
T1 Disorder 38 41 IPF
T2 Disorder 46 48 HP
T3 GGPs 53 58 MMP-8
T4 GGPs 60 65 MMP-9
T5 GGPs 71 80 protein-C
T6 GGPs 90 94 VEGF
T7 Gene_expression 0 14 Protein levels
T8 Gene_expression 0 14 Protein levels
T9 Gene_expression 0 14 Protein levels
T10 Gene_expression 0 14 Protein levels
T11 Positive_regulation 20 29 increased
T12 Positive_regulation 20 29 increased
T13 Positive_regulation 20 29 increased
T14 Negative_regulation 99 108 decreased
T18 Negative_regulation 99 108 decreased
T15 Subject 38 41 IPF
T16 Subject 46 48 HP
T17 Subject 123 130 control 
E1 Gene_expression:T7 Theme:T3
E2 Gene_expression:T8 Theme:T4
E3 Gene_expression:T9 Theme:T5
E4 Gene_expression:T10 Theme:T6
E5 Positive_regulation:T11 Theme:E1 Subject:T15 Subject2:T16
E6 Positive_regulation:T12 Theme:E2 Subject:T15 Subject2:T16
E7 Positive_regulation:T13 Theme:E3 Subject:T15 Subject2:T16
E8 Negative_regulation:T14 Theme:E4 Subject:T15 Subject2:T16
E9 Negative_regulation:T18 Theme:E4 Subject:T17
R1 Subject_Disorder Arg1:T15 Arg2:T1
R2 Subject_Disorder Arg1:T16 Arg2:T2
A1 Negated E9
~~~

Arguments:

*Theme* (optional; zero or more) indicates event or entity ([GGPs](), [Organic_compound_other](), etc.) that is positively regulated. For physical entity, *Theme*, whose function or quality is affected positively.

*Cause* (optional; zero or one) indicates event or entity ([GGPs](), [Organic_compound_other](), etc.) that is the stated cause of the regulation.

*AtLoc* (optional; zero or one) indicates the location where `Positive regulation` event occurs: [Cell_component](), [Cell]() or [Anatomical_entity]().

*Disorder* (optional) indicates the disorder for which `Positive regulation` event occurs: [Disorder]().

*Intermediary* (?)

<!---
The *atLoc*, *fromLoc* and *toLoc* for this event must be [Subject](), [Anatomical_entity](), [Cell](), [Cell_component]() and [Entity Property]().

The other arguments, such as *Cause*, *Theme*, *Participant*, and *Product*, for this event can be any entities or events.
--->

<!--details-->



