---
layout: entry
title: "Negated"
shortdef: "Negation for Events"
order: 0
---

The `Negated` attribute is for event triggers that are negated.

In the following case, the event trigger, which is connected with the [Negation cue](), is negated, and indicated with a cross:
~~~ ann
The patient did not undergo lung resect.
T1 Subject 4 11 patient
T2 Negation_cue 16 19 not
T3 Anatomical_entity 28 32 lung
T4 Artificial_process 33 39 resect
E1 Artificial_process:T4 Theme:T3 Cue:T2
A1 Negated E1
R1 part_of Arg1:T3 Arg2:T1
~~~

<!--
On the other hand, the event trigger itself is negated, without any negation cue, in the following case:
~~~ ann
The unprotonated side chain of the amino acid.
T1 Protonation 4 16 unprotonated
T2 FunctionalGroup 17 27 side chain
T3 AminoAcid 35 45 amino acid
E1 Protonation:T1 Theme:T2
A1 Negated E1
R1 whole_group Arg1:T3 Arg2:T2
~~~
-->
