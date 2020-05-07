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
- *control*; *controls*; *controled*
- *depend*; *depends*; *depended*; *dependent*
- *elevate*; *elevates*; *elevated*; *elevation*
- *enhance*; *enhances*; *enhanced*
- *increase*; *increases*; *increased*
- *induce*; *induces*; *induced*; *induction*
- *mediate*; *mediates*; *mediated*
- *modulate*; *modulates*; *modulated*; *modulation*
- *necessary*
- *positively regulate*; *positively regulates*; *positively regulated*; *positive regulation*
- *promote*; *promotes*; *promoted*; *promotion*
- *require*; *requires*; *required*
- *regulate*; *regulates*; *regulated*; *regulation*
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
T1 GGPs 0 5 LOXL1
T2 GGPs 6 11 LOXL2
T5 Gene_expression 12 27 gene expression
T6 Gene_expression 12 27 gene expression
T9 Positive_regulation 52 61 increased
T10 Positive_regulation 52 61 increased
E1 Gene_expression:T5 Theme:T1
E2 Gene_expression:T6 Theme:T2
E5 Positive_regulation:T9 Theme:E1
E6 Positive_regulation:T10 Theme:E2
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

<!---
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
T18 Positive_regulation 20 29 increased
T19 Positive_regulation 20 29 increased
T20 Positive_regulation 20 29 increased
T21 Negative_regulation 99 108 decreased
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
E8 Positive_regulation:T18 Theme:E1 Subject:T17
E9 Positive_regulation:T19 Theme:E2 Subject:T17
E10 Positive_regulation:T20 Theme:E3 Subject:T17
E11 Negative_regulation:T14 Theme:E4 Subject:T15 Subject2:T16
E12 Negative_regulation:T21 Theme:E4 Subject:T17
R1 Subject_Disorder Arg1:T15 Arg2:T1
R2 Subject_Disorder Arg1:T16 Arg2:T2
A1 Negated E8
A2 Negated E9
A3 Negated E10
A4 Negated E12
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
T18 Positive_regulation 20 29 increased
T19 Positive_regulation 20 29 increased
T20 Positive_regulation 20 29 increased
T21 Negative_regulation 99 108 decreased
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
E8 Positive_regulation:T18 Theme:E1 Subject:T17
E9 Positive_regulation:T19 Theme:E2 Subject:T17
E10 Positive_regulation:T20 Theme:E3 Subject:T17
E11 Negative_regulation:T14 Theme:E4 Subject:T15 Subject2:T16
E12 Negative_regulation:T21 Theme:E4 Subject:T17
R1 Subject_Disorder Arg1:T15 Arg2:T1
R2 Subject_Disorder Arg1:T16 Arg2:T2
A1 Manner E8 low
A2 Manner E9 low
A3 Manner E10 low
A4 Manner E12 low
~~~
--->

The phrases, *Higher/lower*, should not be annotated as Regulation events.

~~~ ann
IPF sputum supernatants had increased concentrations of IGFBP-2, IL-8, TGF-β and KL-6 when compared to healthy subjects whereas COPD had higher IL-6 and TNF-α levels than IPF and HS.
T1 Disorder 0 3 IPF
T2 Anatomical_entity 4 10 sputum
T3 Anatomical_entity 11 23 supernatants
T4 GGPs 56 63 IGFBP-2
T5 GGPs 65 69 IL-8
T6 GGPs 71 76 TGF-β
T7 GGPs 81 85 KL-6
T8 Subject 103 119 healthy subjects
T9 Disorder 128 132 COPD
T10 GGPs 144 148 IL-6
T11 GGPs 153 158 TNF-α
T12 Disorder 171 174 IPF
T13 Subject 179 181 HS
T14 Gene_expression 38 52 concentrations
T15 Gene_expression 38 52 concentrations
T16 Gene_expression 38 52 concentrations
T17 Gene_expression 38 52 concentrations
T18 Gene_expression 159 165 levels
T19 Gene_expression 159 165 levels
T20 Positive_regulation 28 37 increased
T21 Positive_regulation 28 37 increased
T22 Positive_regulation 28 37 increased
T23 Positive_regulation 28 37 increased
E1 Gene_expression:T14 Theme:T4
E2 Gene_expression:T15 Theme:T5
E3 Gene_expression:T16 Theme:T6
E4 Gene_expression:T17 Theme:T7
E5 Gene_expression:T18 Theme:T10 disorder:T9
E6 Gene_expression:T19 Theme:T11 disorder:T9
E7 Positive_regulation:T20 Theme:E1 atLoc:T3 disorder:T1
E8 Positive_regulation:T21 Theme:E2 atLoc:T3 disorder:T1
E9 Positive_regulation:T22 Theme:E3 atLoc:T3 disorder:T1
E10 Positive_regulation:T23 Theme:E4 atLoc:T3 disorder:T1
R1 part_of Arg1:T3 Arg2:T2
~~~

Occasionally, other events, which could be the *Theme* for this Positive_regulation event, are abbreviated in the sentences. In such cases, molecular entities can be the *Theme* for this event.

~~~ ann
No data are available as to whether IL-8 is elevated in sera of IPF patients.
T1 Speculation_cue 0 7 No data
T2 Speculation_cue 28 35 whether
T3 GGPs 36 40 IL-8
T4 Anatomical_entity 56 60 sera
T5 Disorder 64 67 IPF
T6 Subject 68 76 patients
T7 Positive_regulation 44 52 elevated
E1 Positive_regulation:T7 Theme:T3 atLoc:T4 disorder:T5 Cue:T1 Cue2:T2
R1 Subject_Disorder Arg1:T6 Arg2:T5
A1 Speculated E1
~~~

~~~ ann
luciferase activity was elevated.
T1 GGPs 0 10 luciferase
T2 Positive_regulation 24 32 elevated
E1 Positive_regulation:T2 Theme:T1
~~~

Other events can be arguments, such as *Theme* and *Cause*.
~~~ ann
LIGHT promoted cell cycle progression and proliferation of HLFs, but not alpha smooth muscle actin expression.
T1 GGPs 0 5 LIGHT
T2 Positive_regulation 6 14 promoted
T3 Positive_regulation 6 14 promoted
T4 Positive_regulation 6 14 promoted
T5 Cellular_process 15 37 cell cycle progression
T6 Cellular_process 42 55 proliferation
T7 Cell 59 63 HLFs
T8 Negation_cue 69 72 not
T9 GGPs 73 98 alpha smooth muscle actin
T10 Gene_expression 99 109 expression
E1 Positive_regulation:T2 Cause:T1 Theme:E4
E2 Positive_regulation:T3 Cause:T1 Theme:E5
E3 Positive_regulation:T4 Cause:T1 Theme:E6 Cue:T8
E4 Cellular_process:T5 Theme:T7
E5 Cellular_process:T6 Theme:T7
E6 Gene_expression:T10 Theme:T9
A1 Negated E3
~~~
~~~ ann
Activated alveolar epithelial cells have a compromised migration capacity, and also produce CTGF that contribute to fibroblast activation and matrix protein accumulation.
T1 Positive_regulation 0 9 Activated
T2 Cell 10 35 alveolar epithelial cells
T3 Negative_regulation 43 54 compromised
T4 Localization 55 64 migration
T5 Gene_expression 84 91 produce
T6 GGPs 92 96 CTGF
T7 Positive_regulation 102 112 contribute
T8 Positive_regulation 102 112 contribute
T9 Cell 116 126 fibroblast
T10 Positive_regulation 127 138 activation
T11 GGPs 142 156 matrix protein
T12 Localization 157 169 accumulation
E1 Positive_regulation:T1 Theme:T2
E2 Negative_regulation:T3 Theme:E3 AtLoc:T2
E3 Localization:T4 Theme:T2
E4 Gene_expression:T5 Theme:T6 AtLoc:T2
E5 Positive_regulation:T7 Theme:E7 Cause:T6
E6 Positive_regulation:T8 Theme:E8 Cause:T6
E7 Positive_regulation:T10 Theme:T9
E8 Localization:T12 Theme:T11 AtLoc:T2
~~~
~~~ ann
IPF is mainly driven by activated alveolar epithelial cells that have a compromised migration capacity.
T1 Disorder 0 3 IPF
T2 Positive_regulation 14 20 driven
T3 Positive_regulation 24 33 activated
T4 Cell 34 59 alveolar epithelial cells
T5 Negative_regulation 72 83 compromised
T6 Localization 84 93 migration
E1 Positive_regulation:T2 Theme:T1 Cause:E2
E2 Positive_regulation:T3 Theme:T4
E3 Negative_regulation:T5 Theme:E4 AtLoc:T4
E4 Localization:T6 Theme:T4
~~~

Arguments:

*Theme* (optional; zero or more) indicates event (such as [Gene_expression]()) or entity ([GGPs](), [Organic_compound_other](), etc.) that is positively regulated. For physical entity, *Theme*, whose function or quality is affected positively.

*Cause* (optional; zero or one) indicates event or entity ([GGPs](), [Organic_compound_other](), etc.) that is the stated cause of the regulation.

*AtLoc* (optional; zero or one) indicates the location where `Positive regulation` event occurs: [Cell_component](), [Cell]() or [Anatomical_entity]().

*Disorder* (optional) indicates the disorder for which `Positive regulation` event occurs: [Disorder]().

*Intermediary* (?)

<!---
The *atLoc*, *fromLoc* and *toLoc* for this event must be [Subject](), [Anatomical_entity](), [Cell](), [Cell_component]() and [Entity Property]().

The other arguments, such as *Cause*, *Theme*, *Participant*, and *Product*, for this event can be any entities or events.
--->

<!--details-->


