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

CXCL12 -> phosphorylation of SMAD3
~~~ ann
CXCL12-mediated SMAD3 phosphorylation
T1 GGPs 0 6 CXCL12
T2 GGPs 16 21 SMAD3
T3 Positive_regulation 7 15 mediated
T4 Conversion 22 37 phosphorylation
E1 Positive_regulation:T3 Cause:T1 Theme:E2
E2 Conversion:T4 Theme:T2
~~~


CXCL12 -> expression of CTGF

- *SMAD3 -> expression of CTGF*
- *SMAD3 -> stimulation by CXCL12* (to be deleted?)
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

Arguments:

*Theme* (optional; zero or more) indicates event or entity ([GGPs](), [Organic_compound_other](), etc.) that is positively regulated. For physical entity, *Theme*, whose function or quality is affected positively.

*Cause* (optional; zero or one) indicates event or entity ([GGPs](), [Organic_compound_other](), etc.) that is the stated cause of the regulation.

*AtLoc* (optional; zero or one) indicates the location where `Positive regulation` event occurs: [Cell_component](), [Cell]() or [Anatomical_entity]().

*Intermediary* (?)

<!---
The *atLoc*, *fromLoc* and *toLoc* for this event must be [Subject](), [Anatomical_entity](), [Cell](), [Cell_component]() and [Entity Property]().

The other arguments, such as *Cause*, *Theme*, *Participant*, and *Product*, for this event can be any entities or events.
--->

<!--details-->



