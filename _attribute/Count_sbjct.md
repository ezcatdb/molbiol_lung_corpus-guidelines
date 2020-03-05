---
layout: entry
title: "Count_sbjct"
shortdef: "Attribute for Subject with N count"
order: 10
---

The attribute, 'Count_sbjct', is for [Subject]() that is expressed "N= ***".

~~~ ann
Patients with IPF (n=25) and lung cancer (n=15)
T1 Subject 0 8 Patients
T2 Disorder 14 17 IPF
T3 Subject 19 23 n=25
T4 Disorder 29 40 lung cancer
T5 Subject 42 46 n=15
A1 Count_sbjct T3
A2 Count_sbjct T5
R1 Subject_Disorder Arg1:T3 Arg2:T2
R2 Subject_Disorder Arg1:T5 Arg2:T4
R3 member_of Arg1:T3 Arg2:T1
R4 member_of Arg1:T5 Arg2:T1
~~~
~~~ ann
controls (N=24)
T1 Subject 0 15 controls (N=24)
A1 Count_sbjct T1
~~~

<!--
-->
