---
layout: entry
title: "member_of"
shortdef: "Relationships between member and its group"
order: 3
---

This relation describes relationships of a member with a group, to which the member belong.

~~~ ann
70 subjects (50 men and 20 women; mean age, 63.1 y)
T1 Subject 0 11 70 subjects
T2 Subject 13 19 50 men
T3 Subject 24 32 20 women
R1 member_of Arg1:T2 Arg2:T1
R2 member_of Arg1:T3 Arg2:T1
~~~

This relaction can be used to describe the relation of a protein with its protein family.

~~~ ann
EGFR, HER2/neu and HER3 of the ErbB family.
T1 GGPs 0 4 EGFR
T2 GGPs 6 14 HER2/neu
T3 GGPs 19 23 HER3
T4 GGPs 31 41 ErbB family
R1 member_of Arg1:T1 Arg2:T4
R2 member_of Arg1:T2 Arg2:T4
R3 member_of Arg1:T3 Arg2:T4
~~~

<!---
This relation can be used to describe the relationships between events.
--->
