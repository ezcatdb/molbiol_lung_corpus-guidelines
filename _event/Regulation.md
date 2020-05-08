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
- *modify*; *modified*; *modifies*; *modification*
- *alter*; *altered*; *alters* 
- *change*; *changed*; *changes*
- *affect*; *affected*; *affects*
- *effect*
- *influence*; *influenced*; *influences*
- *[play a/an ~] role [in ~ing]*
- *associate*; *associated*; *associates*; *association*
- *involve*; *involved*; *involves*

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



