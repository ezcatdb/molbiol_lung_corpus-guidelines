---
layout: entry
title: 'Artificial_process'
category: "Artificial process"
shortdef: "Artificial process, such as experimental procedures (GENIA)"
order: 0
---

This event describes 'Artificial process', which is usually experimental procedures.

The following words/phrases can be triggers for this event:
- treat/treatment
  - pretreatment
- incubate/incubation
  - preincubation
- addition
- culture/cultured
  - coculture
- transfection
- exposure
- administer/administration

~~~ann
T cell blasts were treated with PMA.
T1 Cell 0 13 T cell blasts
T2 Artificial_process 19 26 treated
T3 Organic_compound_other 32 35 PMA
E1 Artificial_process:T2 Theme:T1 Instrument:T3
~~~
~~~ ann
The cancer cell line was treated with various concentration of paclitaxel for 24 hours.
T1 Cell 4 20 cancer cell line
T2 Artificial_process 25 32 treated
T3 Pharmacological_substance 63 73 paclitaxel
E1 Artificial_process:T2 Theme:T1 Instrument:T3
~~~

Arguments:

The *Theme* for this event can be [Cell](), [GGPs](), [Organic_compound_other](), and [Pharmacological_substance]().

The *Instrument* for this event can be entities used to carry out an artificial process, such as [GGPs](), [Organic_compound_other](), and [Pharmacological_substance]().

<!--details-->
