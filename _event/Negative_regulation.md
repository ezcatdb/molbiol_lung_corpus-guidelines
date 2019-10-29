---
layout: entry
title: "Negative_regulation"
category: "Biological process"
shortdef: "Negative regulation"
order: 21
---

This event is based on the <a href="http://www.nactem.ac.uk/meta-knowledge/">GENIA-Meta-knowledge corpus</a> at <a href="http://www.nactem.ac.uk/">NaCTeM</a>.

The following words/phrases can be triggers of this event:

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
E1 Localization:T1 Theme:E2 AtLoc:T4
E2 Negative_regulation:T2 Theme:T3
R1 part_of Arg1:T3 Arg2:T4
R2 part_of Arg1:T4 Arg2:T5
~~~


Arguments:

<!---
The *atLoc*, *fromLoc* and *toLoc* for this event must be [Subject](), [Anatomical_entity](), [Cell](), [Cell_component]() and [Entity Property]().

The other arguments, such as *Cause*, *Theme*, *Participant*, and *Product*, for this event can be any entities or events.
--->

<!--details-->



