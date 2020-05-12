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
- *involve*; *involved*; *involves*
- *modify*; *modified*; *modifies*; *modification*

The following words/phrases may be triggers, depending on the situations:
- *associate*; *associated*; *associates*; *association* (These can be also triggers for [Binding]() event)
- *[play a/an ~] role [in ~ing]* (Depending on "*~ing*")

~~~ ann
interstitial pneumonia associated with collagen vascular diseases.
T1 Disorder 0 22 interstitial pneumonia
T2 Regulation 23 33 associated
T3 Disorder 39 65 collagen vascular diseases
E1 Regulation:T2 Cause:T3 Theme:T1
~~~
~~~ ann
lung fibrosis-associated cancers.
T1 Disorder 0 13 lung fibrosis
T2 Regulation 14 24 associated
T3 Disorder 25 32 cancers
E1 Regulation:T2 Cause:T1 Theme:T3
~~~

Arguments:

*Theme* (optional; zero or more) indicates event (such as [Gene_expression]()) or entity ([GGPs](), [Organic_compound_other](), etc.) that is positively regulated. For physical entity, *Theme*, whose function or quality is affected positively.

*Cause* (optional; zero or one) indicates event or entity ([GGPs](), [Organic_compound_other](), etc.) that is the stated cause of the regulation.

*atLoc* (optional; zero or one) indicates the location where `Regulation` event occurs: [Cell_component](), [Cell]() or [Anatomical_entity]().

*Disorder* (optional) indicates the disorder for which `Regulation` event occurs: [Disorder]().

*Intermediary* (?)

<!---
The *atLoc*, *fromLoc* and *toLoc* for this event must be [Subject](), [Anatomical_entity](), [Cell](), [Cell_component]() and [Entity Property]().

The other arguments, such as *Cause*, *Theme*, *Participant*, and *Product*, for this event can be any entities or events.
--->

<!--details-->


