---
layout: entry
title: "Negative_regulation"
category: "Biological process"
shortdef: "Negative regulation"
order: 21
---

This event is based on the <a href="http://www.nactem.ac.uk/meta-knowledge/">GENIA-Meta-knowledge corpus</a> at <a href="http://www.nactem.ac.uk/">NaCTeM</a>.

This event describes "inactivation/inhibition/down-regulation" event (UMLS ID:C3463820).

The following words/phrases, which are verbs and nominalized verbs, can be triggers of this event:

- *abolish*, *abolishes*, *abolished*, *abolishment*
- *abrogate*, *abrogates*, *abrogated*, *abrogation*
- *attenuate*, *attenuates*, *attenuated*, *attenuation*
- *block*, *blocks*, *blocked*, *blocking*
- *decline*, *declines*, *declined*
- *decrease*, *decreases*, *decreased*
- *deprive*, *deprives*, *deprived*, *deprivation*
- *dimish*, *diminishes*, *dimished*
- *down-regulate*, *down-regulates*, *down-regulated*, *down-regulation*
- *impair*, *impairs*, *impaired*, *impairment*
- *inactivate*, *inactivates*, *inactivated*, *inactivation*
- *inhibit*, *inhibits*, *inhibited*, *inhibition*
- *negatively regulate*, *negatively regulates*, *negatively regulated*, *negative regulation*
- *prevent*, *prevents*, *prevented*, *prevention*
- *reduce*, *reduces*, *reduced*, *reduction*
- *remove*, *removes*, *removed*, *removal*
- *repress*, *represses*, *repressed*, *repression*
- *suppress*, *suppresses*, *suppressed*, *suppression*
- *damage*

~~~ ann
Phosphorylation of AKT2 was downregulated.
T1 Conversion 0 15 Phosphorylation
T2 GGPs 19 23 AKT
T3 Negative_regulation 28 41 downregulated
E1 Conversion:T1 Theme:T2
E2 Negative_regulation:T3 Theme:E1
~~~
~~~ ann
Accumulation of damaged mitochondria in lung epithelial cells.
T1 Localization 0 12 Accumulation
T2 Negative_regulation 16 23 damaged
T3 Cell_component 24 36 mitochondria
T4 Cell 40 61 lung epithelial cells
T5 Anatomical_entity 40 44 lung
E1 Localization:T1 Theme:T3 AtLoc:T4
E2 Negative_regulation:T2 Theme:T3
R1 part_of Arg1:T3 Arg2:T4
R2 part_of Arg1:T4 Arg2:T5
~~~


Moreover, the following words, which indicate roles, can also be triggers of this event.
- *inhibitor*, *inhibitors*

~~~ ann
PLC inhibitor, U-73122
T1 GGPs 0 3 PLC
T2 Negative_regulation 4 13 inhibitor
T3 Pharmacological_substance 15 22 U-73122
E1 Negative_regulation:T2 Cause:T3 Theme:T1
~~~
~~~ ann
Rho inhibitor C3 exotoxin
T1 GGPs 0 3 Rho
T2 Negative_regulation 4 13 inhibitor
T3 GGPs 14 25 C3 exotoxin
E1 Negative_regulation:T2 Cause:T3 Theme:T1
~~~

The following phrase can also be triggers of this event.
- *inhibitory effect(s)*

Moreover, [Disorder]() can be annotated along with this event.

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

Arguments:

*Theme* (optional; zero or more) indicates event or entity ([GGPs](), [Organic_compound_other](), etc.) that is negatively regulated. For physical entity, *Theme*, whose function or quality is affected negatively.

*Cause* (optional; zero or one) indicates event or entity ([GGPs](), [Organic_compound_other](), etc.) that is the stated cause of the regulation.

*AtLoc* (optional; zero or one) indicates the location where `Negative regulation` event occurs: [Cell_component](), [Cell]() or [Anatomical_entity]().

*Disorder* (optional) indicates the disorder for which `Positive regulation` event occurs: [Disorder]().

*Intermediary* (?)

<!---
The *atLoc*, *fromLoc* and *toLoc* for this event must be [Subject](), [Anatomical_entity](), [Cell](), [Cell_component]() and [Entity Property]().

The other arguments, such as *Cause*, *Theme*, *Participant*, and *Product*, for this event can be any entities or events.
--->

<!--details-->



