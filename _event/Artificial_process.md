---
layout: entry
title: 'Artificial_process'
category: "Artificial process"
shortdef: "Artificial process, such as experimental procedures"
order: 0
---

This event is for 'Artificial process', which is usually experimental procedures.

The following words/phrases can be triggers for this event:
- treatment
  - pretreatment
- incubation
  - preincubation
- addition
- cultured
  - coculture
- transfection
- exposure

~~~ann
T cell blasts were treated with PMA.
T1 Cell 0 13 T cell blasts
T2 Artificial_process 19 26 treated
T3 Organic_compound_other 32 35 PMA
E1 Artificial_process:T2 Theme:T1 Theme2:T3
~~~

Arguments:

The *Theme* for this event can be [Cell](), [Organic_compound_other](), and [Pharmacological_substance]().


<!--details-->
