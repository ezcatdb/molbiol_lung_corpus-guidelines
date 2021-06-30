---
layout: entry
title: "Regulation"
category: "Biological process"
shortdef: "Regulation"
order: 20
---
<!---
This event is based on the <a href="http://www.nactem.ac.uk/meta-knowledge/">GENIA-Meta-knowledge corpus</a> at <a href="http://www.nactem.ac.uk/">NaCTeM</a>.
--->

This event describes "regulation process" event (UMLS ID:C1327622).

If it is not clear whether the trigger words are "positive" or "negative", this "Regulation" event will be selected.

The following words/phrases can be triggers of this event:
- *affect*; *affected*; *affects*
- *alter*; *altered*; *alters* 
- *change*; *changed*; *changes*
- *effect*
- *influence*; *influenced*; *influences*
- *modify*; *modified*; *modifies*; *modification*

The following words/phrases may be triggers, depending on the situations:
- *[play a/an ~] role [in ~ing]* (Depending on "*~ing*")

~~~ ann
Immune responses may affect the development of IPF.
T1 Biological_process 0 16 Immune responses
T2 Speculation_cue 17 20 may
T3 Regulation 21 27 affect
T4 Biological_process 32 43 development
T5 Disorder 47 50 IPF
E1 Biological_process:T1
E2 Regulation:T3 Cause:E1 Theme:E3 Cue:T2
E3 Biological_process:T4 Theme:T5
A1 Speculated E2
~~~

<!--
~~~
-->

Arguments:

The *Theme* (optional; zero or one) indicates events, such as [Gene_expression](), or entities, such as [GGPs](), and [Organic_compound_other](), that are regulated. Function or quality of *Theme* can be affected.

The *Cause* (optional; zero or one) indicates events or entities, such as [GGPs](), [Organic_compound_other](), that are the stated cause of the regulation.

The *atLoc* (optional) indicates the location where `Regulation` event occurs: [Cell_component](), [Cell]() or [Anatomical_entity]().

The *disorder* (optional) indicates the [Disorder]() for which `Regulation` event occurs.

The *Cue* argument (optional) is cues, such as [Negation cue](), [Speculation cue]() or [Method cue]().

<!---
The *atLoc*, *fromLoc* and *toLoc* for this event must be [Subject](), [Anatomical_entity](), [Cell](), [Cell_component]() and [Entity Property]().

The other arguments, such as *Cause*, *Theme*, *Participant*, and *Product*, for this event can be any entities or events.
--->

<!--details-->



