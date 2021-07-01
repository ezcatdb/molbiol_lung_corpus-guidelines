---
layout: entry
title: "Correlation"
category: "Biological process"
shortdef: "Correlation between several entities/events; co-occurence of several events"
order: 23
---
<!---
This event is based on the <a href="http://www.nactem.ac.uk/meta-knowledge/">GENIA-Meta-knowledge corpus</a> at <a href="http://www.nactem.ac.uk/">NaCTeM</a>.
--->

This event describes "Correlation" or "Co-occurence" (UMLS ID:C0332281).

When several events/entities are correlated, this event will be selected. Or, when several events occur simultaneously, those events can be connected with this event.

If the cause and effect (or the causality) are not clear, the relation can be annotated with this `Correlation` event.

<!---
If it is not clear whether the trigger words are "positive" or "negative", this "Regulation" event will be selected.
--->

The following words/phrases can be triggers of this event:
- *involve*; *involved*; *involves*; *involvement*
- *accompany*; *accompanied*; *accompanies*
- *characterize*; *characterized*; *characterizes*; *characterization*
- *coincide*; *coincided*; *coincides*; *coincident*
- *correlate*; *correlated*; *correlates*; *correlation*
- *concomitant*; *concomitantly*
- *parallel*; *paralleled*; *parallels*
- *relate*; *related*; *relates*; *relation*
- *synergy*

The following words/phrases may be triggers, depending on the situations:
- *associate*; *associated*; *associates*; *association* (These can be also triggers for [Binding]() event)
- *combine*; *combined*; *combines*; *combination* (These can be also triggers for [Binding]() or [Conversion]())
- *couple*; *coupled*; *couples* (These can be also triggers for [Binding]() or [Conversion]())
- *link*; *linked*; *links* (These can be also triggers for [Binding]() or [Conversion]())
- *[play a/an ~] role [in ~ing]* (Depending on "*~ing*")

~~~ ann
Immune responses may be associated with the development of IPF.
T1 Biological_process 0 16 Immune responses
T2 Speculation_cue 17 20 may
T3 Correlation 24 34 associated
T4 Biological_process 44 55 development
T5 Disorder 59 62 IPF
E1 Biological_process:T1
E2 Correlation:T3 Theme:E1 Theme2:E3 Cue:T2
E3 Biological_process:T4 Theme:T5
A1 Speculated E2
~~~
~~~ ann
The reduction in collagen was associated with a reduction in macrophages and increased CXCL10.
T1 Negative_regulation 4 13 reduction
T2 GGPs 17 25 collagen
T3 Correlation 30 40 associated
T4 Negative_regulation 48 57 reduction
T5 Cell 61 72 macrophages
T6 Positive_regulation 77 86 increased
T7 GGPs 87 93 CXCL10
E1 Negative_regulation:T1 Theme:T2
E2 Correlation:T3 Theme:E1 Theme2:E3 Theme3:E4
E3 Negative_regulation:T4 Theme:T5
E4 Positive_regulation:T6 Theme:T7
~~~

Arguments:

*Theme* (two or more) indicates events, such as [Gene_expression](), or entities, such as [GGPs]() and [Organic_compound_other](), that are related. Function or quality of *Theme* are related.

The *atLoc* (optional) indicates the location where the `Correlation` event occurs: [Cell_component](), [Cell]() or [Anatomical_entity]().

The *disorder* (optional) indicates the [Disorder]() for which the `Correlation` event occurs.

The *Cue* argument (optional) is cues, such as [Negation cue](), [Speculation cue]() or [Method cue]().


<!---
The *atLoc*, *fromLoc* and *toLoc* for this event must be [Subject](), [Anatomical_entity](), [Cell](), [Cell_component]() and [Entity Property]().

The other arguments, such as *Cause*, *Theme*, *Participant*, and *Product*, for this event can be any entities or events.
--->

<!--details-->
