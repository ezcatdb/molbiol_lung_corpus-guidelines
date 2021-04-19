---
layout: entry
title: "Negation cue"
shortdef: "Negation words and phrases"
order: 107
---

Negation words, such as "not", can be combined with event expressions.

~~~ ann
The patient did not undergo lung resect.
T1 Subject 4 11 patient
T2 Negation_cue 16 19 not
T3 Anatomical_entity 28 32 lung
T4 Artificial_process 33 39 resect
E1 Artificial_process:T4 Theme:T3 cue:T2
A1 Negated E1
R1 part_of Arg1:T3 Arg2:T1
~~~

However, even if the negation words can be identified as Negation_cue, such cues are not always connected with event expressions.

In addition to typical negation words, such as “no”, “not’, “none” and
“neither ~ nor ~”, the following words/phrases can be negation cues.

- instead of
- lack(s)/lacking
- loss/lost
- rather than
- other than
- without
- absence/absent
- barely
- failed to
- inability/incapable
- (very) little
- (very) poor
- (too/very) low

<!--
The reaction event words such as “unprotonated” and “unactivated”
should be clicked with “Negation” for the Event attributes, although
they do not have corresponding negation cues.

~~~ ann
"Unactivated" substrates
T1 Activation 1 12 Unactivated
T2 EntityProperty 0 24 "Unactivated" substrates
E1 Activation:T1 Theme:T2
A1 Negation E1
~~~


{% include image.html name="negated-event.png"
   caption="Example 8"
%}
-->
