---
layout: entry
title: "is_equivalent"
shortdef: "Equivalent relations"
order: 1
---

Entity names and their abbreviated names should be connected with this relation, particularly if UMLS IDs are not available for those entities.

~~~ ann
Idiopathic pulmonary fibrosis (IPF) is a fatal condition. 
T1 Disorder 0 29 Idiopathic pulmonary fibrosis
T2 Disorder 31 34 IPF
R1 is_equivalent Arg1:T2 Arg2:T1
~~~

<!-- details -->
