---
layout: entry
title: "Pharmacological_substance"
shortdef: "Medicine (PHAEDRA)"
order: 21
---

The name of this entity group is based on the <a href="http://www.nactem.ac.uk/PHAEDRA/">PHAEDRA corpus</a> at <a href="http://www.nactem.ac.uk/">NaCTeM</a>.

This entity is based on <a href="https://www.ebi.ac.uk/chembl/">ChEMBL</a> database.

Medicines are categorized into this entity group.

~~~ ann
PLC inhibitor, U-73122
T1 GGPs 0 3 PLC
T2 Negative_regulation 4 13 inhibitor
T3 Pharmacological_substance 15 22 U-73122
E1 Negative_regulation:T2 Cause:T3 Theme:T1
~~~


The following protein medicines can also be categorized in to this group.

- Nivolumab
- Tocilizumab

~~~ ann
Pirfenidone was dosed at 600 mg/day for the first 2 weeks.
T1 Pharmacological_substance 0 11 Pirfenidone
~~~

~~~ ann
The common adverse effects of Icotinib were rash and diarrhea.
T1 Regulation 4 26 common adverse effects
T2 Pharmacological_substance 30 38 Icotinib
T3 Disorder 44 48 rash
T4 Disorder 53 61 diarrhea
E1 Regulation:T1 Cause:T2 Theme:T3 Theme2:T4
~~~

Although 'placebo' is not any medicine, this word can be tentatively categorized into this entity.

~~~ ann
Ten healthy volunteers took 200 mg itraconazole or matched placebo once daily for 4 days.
T1 Subject 0 22 Ten healthy volunteers
T5 Pharmacological_substance 35 47 itraconazole
T6 Pharmacological_substance 59 66 placebo
~~~

<!-- details -->
